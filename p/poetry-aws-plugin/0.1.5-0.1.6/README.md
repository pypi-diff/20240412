# Comparing `tmp/poetry_aws_plugin-0.1.5.tar.gz` & `tmp/poetry_aws_plugin-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.5.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.6.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.5.tar` & `poetry_aws_plugin-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.5/LICENSE
--rw-r--r--   0        0        0     2634 2024-04-05 23:55:14.069809 poetry_aws_plugin-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.5/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     6606 2024-04-06 00:14:58.477846 poetry_aws_plugin-0.1.5/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-06 00:08:26.653834 poetry_aws_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.6/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     7219 2024-04-12 01:34:59.890781 poetry_aws_plugin-0.1.6/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-12 01:06:27.466848 poetry_aws_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.6/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.5/LICENSE` & `poetry_aws_plugin-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.5/README.md` & `poetry_aws_plugin-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,31 +28,36 @@
 You must ensure that your AWS credentials are configured and discoverable by `boto3`. The [`boto3` documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials) has details on how to configure your credentials and the order in which they searched.
 
 When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
-2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run `codeartifact.GetAuthorizationToken`.
+2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 
 **To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
 
 For example:
 
 ```bash
-export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'
-poetry install
+POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>' poetry install
 ```
 
 or
 
 ```bash
 echo "export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'" >> ~/.bashrc
 source ~/.bashrc
 poetry install
 ```
 
 You can find more details in AWS's [CodeArtifact authentication and tokens documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/tokens-authentication.html) and [CodeArtifact IAM documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/security_iam_service-with-iam.html).
 
 # Misc
 
-You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reduce poetry configuration.
+You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reducing poetry configuration.
+
+For example:
+
+```bash
+POETRY_AWS_PLUGIN_AUTH_TOKEN='<codeartifact-authorization-token>' poetry install
+```
```

### Comparing `poetry_aws_plugin-0.1.5/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.6/poetry_aws_plugin/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,58 +4,84 @@
 
 import boto3
 import requests
 
 from botocore.exceptions import ClientError
 from cleo.io.io import IO, Verbosity
 from poetry.exceptions import PoetryException
-from poetry.plugins import Plugin
 from poetry.poetry import Poetry
+from poetry.plugins import Plugin
+from poetry.publishing.uploader import Uploader
 from poetry.utils.authenticator import Authenticator
-from poetry.utils.password_manager import HTTPAuthCredential
 
 POETRY_AWS_PLUGIN_ROLE_ARN_VAR = "POETRY_AWS_PLUGIN_ROLE_ARN"
 POETRY_AWS_PLUGIN_SESSION_NAME = "poetry-aws-plugin"
 POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR = "POETRY_AWS_PLUGIN_AUTH_TOKEN"
 
 UNAUTHORIZED_STATUS_CODES = (401, 403)
-CODEARTIFACT_URL_REGEX = r"^https://([a-z][a-z-]*)-(\d+)\.d\.codeartifact\.[^.]+\.amazonaws\.com/.*$"
+CODEARTIFACT_URL_REGEX = r"^https://([a-z][a-z-]*)-(\d+)\.d\.codeartifact\.[^.]+\.amazonaws\.com.*$"
 
 RETRY_ERROR_MESSAGE = f"""
 Make sure you have AWS credentials configured and up-to-date
 
 Then make sure you have atleast one of the following:
     1. Authorization for CodeArtifact with your current credentials
     2. Authorization for an IAM role that has access to CodeArtifact and
        environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' set to that role's ARN
 """
 
 
 def patch(io: IO):
-    request = Authenticator.request
 
     def is_retryable(response: requests.Response) -> bool:
         if response.status_code not in UNAUTHORIZED_STATUS_CODES:
             return False
         if not re.match(CODEARTIFACT_URL_REGEX, response.url):
             return False
         return True
 
+
+    def get_auth_token(domain: str, domain_owner: str) -> str:
+        io.write_line(
+            "Getting new CodeArtifact authorization token for "
+            f"domain '{domain}' and domain owner '{domain_owner}'",
+            verbosity=Verbosity.VERBOSE,
+        )
+
+        is_valid = validate_credentials()
+        if not is_valid:
+            return ""
+
+        # We'll try these methods to get the CodeArtifact token
+        methods = [
+            get_auth_token_with_current_credentials,
+            get_auth_token_with_iam_role,
+            get_auth_token_from_env,
+        ]
+        for method in methods:
+            auth_token = method(domain, domain_owner)
+            if auth_token:
+                return auth_token
+
+        return ""
+
+
     def validate_credentials() -> bool:
         try:
             boto3.client("sts").get_caller_identity()
             return True
         except ClientError as err:
             io.write_line(f"Error using current credentials: {err}")
             return False
         except Exception as err:
             io.write_line("Unexpected error while validating AWS credentials")
             io.write_line(RETRY_ERROR_MESSAGE)
             raise err
 
+
     def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
         try:
             token_response = boto3.client("codeartifact").get_authorization_token(
                 domain=domain,
                 domainOwner=domain_owner,
             )
             return token_response["authorizationToken"]
@@ -67,14 +93,15 @@
         except Exception as err:
             io.write_line(
                 f"Unexpected error while getting CodeArtifact authorization token: {err}",
                 verbosity=Verbosity.VERBOSE,
             )
         return ""
 
+
     def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
         role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
         if not role_arn:
             io.write_line(
                 f"Error getting CodeArtifact token using IAM role: "
                 f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found",
                 verbosity=Verbosity.VERBOSE,
@@ -107,77 +134,66 @@
             io.write_line(
                 "Unexpected error while assuming CodeArtifact role "
                 f"and getting CodeArtifact authorization token: {err}",
                 verbosity=Verbosity.VERBOSE,
             )
         return ""
 
+
     def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
         return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
-    def get_auth_token(domain: str, domain_owner: str) -> str:
+
+    def patched_session_send(self: requests.Session, request: requests.PreparedRequest, **kwargs: Any) -> requests.Response:
+        response = requests.Session.send(self, request, **kwargs)
+        if not is_retryable(response):
+            return response
+
         io.write_line(
-            "Getting new CodeArtifact authorization token for "
-            f"domain '{domain}' and domain owner '{domain_owner}'",
+            "Failed to get authorization for CodeArtifact",
             verbosity=Verbosity.VERBOSE,
         )
 
-        is_valid = validate_credentials()
-        if not is_valid:
-            return ""
+        match = re.match(CODEARTIFACT_URL_REGEX, response.url)
+        domain, domain_owner = match.groups()
 
-        # We'll try these methods to get the CodeArtifact token
-        methods = [
-            get_auth_token_with_current_credentials,
-            get_auth_token_with_iam_role,
-            get_auth_token_from_env,
-        ]
-        for method in methods:
-            auth_token = method(domain, domain_owner)
-            if auth_token:
-                return auth_token
+        auth_token = get_auth_token(domain, domain_owner)
+        if not auth_token:
+            raise PoetryException(RETRY_ERROR_MESSAGE)
 
-        return ""
+        io.write_line("Successfully got CodeArtifact authorization token\nRetrying request", verbosity=Verbosity.VERBOSE)
 
-    def patched_request(
-        self: Authenticator,
-        method: str,
-        url: str,
-        raise_for_status: bool = True,
-        **kwargs: Any,
-    ) -> requests.Response:
-        response = request(self, method=method, url=url, raise_for_status=False, **kwargs)
+        # Use the received auth token for the session
+        self.auth = ("aws", auth_token)
 
-        if is_retryable(response):
-            io.write_line(
-                "Failed to get authorization for CodeArtifact",
-                verbosity=Verbosity.VERBOSE,
-            )
+        # And create a new request using the new auth
+        new_request = request.copy()
 
-            match = re.match(CODEARTIFACT_URL_REGEX, response.url)
-            domain, domain_owner = match.groups()
+        # We must call prepare_hook after prepare_auth
+        # https://github.com/psf/requests/blob/31ebb8102c00f8cf8b396a6356743cca4362e07b/src/requests/models.py#L376
+        new_request.prepare_auth(self.auth, request.url)
+        new_request.prepare_hooks(request.hooks)
 
-            auth_token = get_auth_token(domain, domain_owner)
-            if not auth_token:
-                raise PoetryException(RETRY_ERROR_MESSAGE)
+        # And finally we retry the request
+        return requests.Session.send(self, new_request, **kwargs)
 
-            io.write_line(
-                "Successfully got CodeArtifact authorization token! Retrying request...",
-                verbosity=Verbosity.VERBOSE,
-            )
 
-            # Overwrite the credentials for this URL
-            self._credentials[url] = HTTPAuthCredential(username="aws", password=auth_token)
+    def patched_authenticator_create_session(self: Authenticator) -> requests.Session:
+        session = authenticator_create_session(self)
+        session.send = patched_session_send.__get__(session)
+        return session
 
-            # Now retry the original request with new credentials
-            return request(self, method=method, url=url, raise_for_status=raise_for_status, **kwargs)
+    def patched_uploader_make_session(self: Uploader) -> requests.Session:
+        session = uploader_make_session(self)
+        session.send = patched_session_send.__get__(session)
+        return session
 
-        if raise_for_status:
-            response.raise_for_status()
-        return response
+    authenticator_create_session = Authenticator.create_session
+    uploader_make_session = Uploader.make_session
 
-    Authenticator.request = patched_request
+    Authenticator.create_session = patched_authenticator_create_session
+    Uploader.make_session = patched_uploader_make_session
 
 
 class PoetryAwsPlugin(Plugin):
     def activate(self, _: Poetry, io: IO) -> None:
         patch(io)
```

### Comparing `poetry_aws_plugin-0.1.5/pyproject.toml` & `poetry_aws_plugin-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.5"
+version = "0.1.6"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.5/PKG-INFO` & `poetry_aws_plugin-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.5
+Version: 0.1.6
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -48,32 +48,37 @@
 You must ensure that your AWS credentials are configured and discoverable by `boto3`. The [`boto3` documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html#configuring-credentials) has details on how to configure your credentials and the order in which they searched.
 
 When poetry runs a command that uses CodeArtifact and fails to authorize, the plugin will automatically attempt to get the authorization token and retry the command.
 
 Your AWS credentials must be authorized to do atleast one of the following:
 
 1. Run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
-2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run `codeartifact.GetAuthorizationToken`.
+2. Run [`sts.AssumeRole`](https://docs.aws.amazon.com/cli/latest/reference/sts/assume-role.html) to assume a role with authorization to run [`codeartifact.GetAuthorizationToken`](https://docs.aws.amazon.com/cli/latest/reference/codeartifact/get-authorization-token.html).
 
 **To use IAM roles to authorize, set the environment variable `POETRY_AWS_PLUGIN_ROLE_ARN` to the role's ARN before running any poetry commands**.
 
 For example:
 
 ```bash
-export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'
-poetry install
+POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>' poetry install
 ```
 
 or
 
 ```bash
 echo "export POETRY_AWS_PLUGIN_ROLE_ARN='arn:aws:codeartifact:<region>:<account-id>:repository/<domain>/<domain-owner>/<repository>'" >> ~/.bashrc
 source ~/.bashrc
 poetry install
 ```
 
 You can find more details in AWS's [CodeArtifact authentication and tokens documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/tokens-authentication.html) and [CodeArtifact IAM documentation](https://docs.aws.amazon.com/codeartifact/latest/ug/security_iam_service-with-iam.html).
 
 # Misc
 
-You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reduce poetry configuration.
+You can also authorize by setting the environment variable `POETRY_AWS_PLUGIN_AUTH_TOKEN` to the CodeArtifact authorization token. This may be useful in CI/CD pipelines and reducing poetry configuration.
+
+For example:
+
+```bash
+POETRY_AWS_PLUGIN_AUTH_TOKEN='<codeartifact-authorization-token>' poetry install
+```
```

