# Comparing `tmp/praetorian-cli-0.7.2.tar.gz` & `tmp/praetorian_cli-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praetorian-cli-0.7.2.tar", last modified: Sun Apr  7 01:42:51 2024, max compression
+gzip compressed data, was "praetorian_cli-0.8.tar", last modified: Fri Apr 12 20:26:35 2024, max compression
```

## Comparing `praetorian-cli-0.7.2.tar` & `praetorian_cli-0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.743020 praetorian-cli-0.7.2/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-07 01:42:51.742900 praetorian-cli-0.7.2/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian-cli-0.7.2/README.md
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.736954 praetorian-cli-0.7.2/praetorian_cli/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian-cli-0.7.2/praetorian_cli/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)      624 2024-04-04 16:57:50.000000 praetorian-cli-0.7.2/praetorian_cli/cli.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.739567 praetorian-cli-0.7.2/praetorian_cli/handlers/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian-cli-0.7.2/praetorian_cli/handlers/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2118 2024-04-07 01:32:46.000000 praetorian-cli-0.7.2/praetorian_cli/handlers/account.py
--rw-r--r--   0 privateducky   (501) staff       (20)     4313 2024-04-07 01:41:55.000000 praetorian-cli-0.7.2/praetorian_cli/handlers/backend.py
--rw-r--r--   0 privateducky   (501) staff       (20)      436 2024-04-07 01:29:50.000000 praetorian-cli-0.7.2/praetorian_cli/handlers/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.740634 praetorian-cli-0.7.2/praetorian_cli/sdk/
--rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2793 2024-04-07 01:33:46.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/chaos.py
--rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/keychain.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.742290 praetorian-cli-0.7.2/praetorian_cli/sdk/test/
--rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/__init__.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-07 01:31:02.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_file_upload.py
--rw-r--r--   0 privateducky   (501) staff       (20)     2418 2024-04-07 01:32:14.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_job_capabilities.py
--rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-07 01:32:19.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_link_account.py
--rw-r--r--   0 privateducky   (501) staff       (20)      748 2024-04-07 01:32:29.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_manual_risk.py
--rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-07 01:31:41.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_nvd.py
--rw-r--r--   0 privateducky   (501) staff       (20)     1814 2024-04-07 01:31:28.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_seed.py
--rw-r--r--   0 privateducky   (501) staff       (20)      879 2024-04-07 01:31:15.000000 praetorian-cli-0.7.2/praetorian_cli/sdk/test/utils.py
-drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-07 01:42:51.742633 praetorian-cli-0.7.2/praetorian_cli.egg-info/
--rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/PKG-INFO
--rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/SOURCES.txt
--rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/dependency_links.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/entry_points.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/requires.txt
--rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-07 01:42:51.000000 praetorian-cli-0.7.2/praetorian_cli.egg-info/top_level.txt
--rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian-cli-0.7.2/pyproject.toml
--rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-07 01:42:51.743457 praetorian-cli-0.7.2/setup.cfg
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.256895 praetorian_cli-0.8/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-12 20:26:35.256725 praetorian_cli-0.8/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)     1111 2024-03-23 18:37:05.000000 praetorian_cli-0.8/README.md
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.246191 praetorian_cli-0.8/praetorian_cli/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:07:07.000000 praetorian_cli-0.8/praetorian_cli/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      674 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/cli.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.249585 praetorian_cli-0.8/praetorian_cli/handlers/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:32.000000 praetorian_cli-0.8/praetorian_cli/handlers/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2843 2024-04-12 20:26:25.000000 praetorian_cli-0.8/praetorian_cli/handlers/account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     5002 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/handlers/backend.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1186 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/handlers/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.250637 praetorian_cli-0.8/praetorian_cli/sdk/
+-rw-r--r--   0 privateducky   (501) staff       (20)        0 2024-03-02 18:06:24.000000 praetorian_cli-0.8/praetorian_cli/sdk/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3125 2024-04-11 14:42:01.000000 praetorian_cli-0.8/praetorian_cli/sdk/chaos.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     3357 2024-03-23 18:37:05.000000 praetorian_cli-0.8/praetorian_cli/sdk/keychain.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.255509 praetorian_cli-0.8/praetorian_cli/sdk/test/
+-rw-r--r--   0 privateducky   (501) staff       (20)      432 2024-03-23 18:37:05.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/__init__.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1280 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_file_upload.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     2484 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_job_capabilities.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      987 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_link_account.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      741 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_manual_risk.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      623 2024-04-08 21:35:19.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_nvd.py
+-rw-r--r--   0 privateducky   (501) staff       (20)     1831 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/test_seed.py
+-rw-r--r--   0 privateducky   (501) staff       (20)      988 2024-04-10 11:11:30.000000 praetorian_cli-0.8/praetorian_cli/sdk/test/utils.py
+drwxr-xr-x   0 privateducky   (501) staff       (20)        0 2024-04-12 20:26:35.256394 praetorian_cli-0.8/praetorian_cli.egg-info/
+-rw-r--r--   0 privateducky   (501) staff       (20)     1613 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/PKG-INFO
+-rw-r--r--   0 privateducky   (501) staff       (20)      866 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)        1 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       54 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/entry_points.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       23 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/requires.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)       15 2024-04-12 20:26:35.000000 praetorian_cli-0.8/praetorian_cli.egg-info/top_level.txt
+-rw-r--r--   0 privateducky   (501) staff       (20)      103 2024-03-03 04:04:12.000000 praetorian_cli-0.8/pyproject.toml
+-rw-r--r--   0 privateducky   (501) staff       (20)      673 2024-04-12 20:26:35.257398 praetorian_cli-0.8/setup.cfg
```

### Comparing `praetorian-cli-0.7.2/PKG-INFO` & `praetorian_cli-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.7.2
+Version: 0.8.0
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `praetorian-cli-0.7.2/README.md` & `praetorian_cli-0.8/README.md`

 * *Files identical despite different names*

### Comparing `praetorian-cli-0.7.2/praetorian_cli/cli.py` & `praetorian_cli-0.8/praetorian_cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
 from praetorian_cli.sdk.keychain import Keychain
+from praetorian_cli.handlers.account import chaos
 from praetorian_cli.handlers.backend import chaos
 
 
 @click.group(invoke_without_command=True)
 @click.version_option()
 @click.pass_context
 @click.option('--profile', default='United States', help='The keychain profile to use', show_default=True)
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/handlers/account.py` & `praetorian_cli-0.8/praetorian_cli/handlers/account.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 import random
 
-from utils import chaos
-from utils import handle_api_error
 from base64 import b64encode
+
+from praetorian_cli.handlers.utils import chaos
+from praetorian_cli.handlers.utils import handle_api_error
 from praetorian_cli.sdk.keychain import verify_credentials
 
 
 @chaos.command('accounts')
 @click.pass_obj
 @handle_api_error
 def my_accounts(controller):
@@ -17,17 +18,18 @@
         print(f"{hit['key']}")
 
 
 @chaos.command('link-account')
 @click.pass_obj
 @handle_api_error
 @click.argument('username')
-def link_account(controller, username, secret):
+@click.option('-config', '--config', default="", help="Add an optional configuration")
+def link_account(controller, username, config):
     """ Link another Chaos account to yours """
-    result = controller.link_account(username=username, config='')
+    result = controller.link_account(username=username, config=config)
     print(f"{result['key']}")
 
 
 @chaos.command('unlink-account')
 @click.pass_obj
 @handle_api_error
 @click.argument('username')
@@ -36,37 +38,57 @@
     result = controller.unlink_account(username=username)
     print(f"{result['key']}")
 
 
 @chaos.command('add-webhook')
 @click.pass_obj
 @handle_api_error
-@verify_credentials
 def add_webhook(controller):
-    """ Create a webhook for adding assets and risks """
+    """ Authenticated URL for adding assets and risks """
     pin = str(random.randint(10000, 99999))
+    controller.link_account(username="hook", config=pin)
     username = b64encode(controller.keychain.username.encode('utf8'))
     encoded_string = username.decode('utf8')
     encoded_username = encoded_string.rstrip('=')
-
-    controller.link_account(username="hook", config=pin)
     print(f'{controller.keychain.api}/hook/{encoded_username}/{pin}')
 
 
-@chaos.command('integrate-slack')
+@chaos.command('link-slack')
 @click.pass_obj
 @handle_api_error
 @click.argument('webhook')
-def integrate_slack(controller, webhook):
+def link_slack(controller, webhook):
+    """ Send all new risks to Slack """
     controller.link_account('slack', webhook)
 
 
-@chaos.command('integrate-jira')
+@chaos.command('link-jira')
 @click.pass_obj
 @handle_api_error
 @click.argument('domain')
 @click.argument('access_token')
 @click.argument('project_key')
 @click.argument('issue_type_id')
-def integrate_jira(controller, domain, access_token, project_key, issue_type_id):
+def link_jira(controller, domain, access_token, project_key, issue_type_id):
+    """ Send all new risks to JIRA """
     config = {'domain': domain, 'accessToken': access_token, 'projectKey': project_key, 'issueId': issue_type_id}
     controller.link_account('jira', config)
+
+
+@chaos.command('link-amazon')
+@click.pass_obj
+@handle_api_error
+@click.argument('access_key')
+@click.argument('secret_key')
+def link_amazon(controller, access_key, secret_key):
+    """ Enumerate Amazon for Assets """
+    config = {'accessKey': access_key, 'secretKey': secret_key}
+    controller.link_account('amazon', config)
+
+
+@chaos.command('link-github')
+@click.pass_obj
+@handle_api_error
+@click.argument('pat')
+def link_github(controller, pat):
+    """ Allow Chaos to scan your private repos """
+    controller.link_account('github', pat)
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/handlers/backend.py` & `praetorian_cli-0.8/praetorian_cli/handlers/backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 import os
 import click
 
 from praetorian_cli.handlers.utils import chaos
+from praetorian_cli.handlers.utils import Status
 from praetorian_cli.handlers.utils import handle_api_error
 
 
 @chaos.command('seeds')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_seeds(controller, seed):
     """ Fetch seed domains """
     result = controller.my(dict(key=f'#seed#{seed}'))
     for hit in result.get('seeds', []):
         print(f"{hit['key']}")
+        print(hit)
 
 
 @chaos.command('assets')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_assets(controller, seed):
     """ Fetch existing assets """
     result = controller.my(dict(key=f'#asset#{seed}'))
     for hit in result.get('assets', []):
         print(f"{hit['key']}")
-
+        print(hit)
 
 @chaos.command('risks')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
 def my_risks(controller, seed):
     """ Fetch current risks """
     result = controller.my(dict(key=f'#risk#{seed}'))
     for hit in result.get('risks', []):
         print(f"{hit['key']}")
+        print(hit)
 
-
-@chaos.command('jobs')
+@chaos.command('services')
 @click.pass_obj
 @handle_api_error
 @click.option('-seed', '--seed', default="", help="Filter by seed domain")
-def my_jobs(controller, seed):
-    """ Fetch past, present and future jobs """
-    result = controller.my(dict(key=f'#job#{seed}'))
-    for hit in result.get('jobs', []):
+def my_services(controller, seed):
+    """ Fetch recently seen services """
+    result = controller.my(dict(key=f'#service#{seed}'))
+    for hit in result.get('services', []):
         print(f"{hit['key']}")
 
 
-@chaos.command('services')
+@chaos.command('jobs')
 @click.pass_obj
 @handle_api_error
-@click.option('-port', '--port', default="", help="Filter by port")
-def my_services(controller, port):
-    """ Fetch recently seen services """
-    result = controller.my(dict(key=f'#service#{port}'))
-    for hit in result.get('services', []):
+@click.option('-updated', '--updated', default="", help="Fetch jobs since date")
+def my_jobs(controller, updated):
+    """ Fetch past, present and future jobs """
+    result = controller.my(dict(key=f'#job#{updated}'))
+    for hit in result.get('jobs', []):
         print(f"{hit['key']}")
 
 
 @chaos.command('files')
 @click.pass_obj
 @handle_api_error
-@click.option('-key', '--key', default="", help="Filter by relative path")
-def my_files(controller, key):
+@click.option('-name', '--name', default="", help="Filter by relative path")
+def my_files(controller, name):
     """ Fetch all file names """
-    result = controller.my(dict(key=f'#file#{key}'))
+    result = controller.my(dict(key=f'#file#{name}'))
     for hit in result.get('files', []):
         print(f"{hit['key']}")
 
 
 @chaos.command('threats')
 @click.pass_obj
 @handle_api_error
@@ -82,39 +84,41 @@
         print(f"{hit['key']}")
 
 
 @chaos.command('add-seed')
 @click.pass_obj
 @handle_api_error
 @click.argument('seed')
-@click.option('-comment', '--comment', default="", help="Add a description")
-def add_seed(controller, seed, comment):
+@click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
+@click.option('-comment', '--comment', default="", help="Add a comment")
+def add_seed(controller, seed, status, comment=""):
     """ Add a new seed domain """
-    controller.upsert_seed(seed, status=0, comment=comment)
+    controller.add_asset(seed, status=status, comment=comment)
 
 
-@chaos.command('freeze-seed')
+@chaos.command('update-asset')
 @click.pass_obj
 @handle_api_error
-@click.argument('seed')
-def freeze_seed(controller, seed):
-    """ Freeze a seed domain  """
-    controller.upsert_seed(seed, 1)
+@click.argument('key')
+@click.option('-status', '--status', type=click.Choice(['AA', 'AF']), required=False, default="AA")
+@click.option('-comment', '--comment', help="Add a comment")
+def update_asset(controller, key, status, comment=''):
+    """ Update any asset or seed """
+    controller.update_asset(key, status=status, comment=comment)
 
 
 @chaos.command('add-risk')
 @click.pass_obj
 @handle_api_error
 @click.argument('key')
-@click.option('-finding', '--finding', required=True, help="Generic risk identifier")
-@click.option('-status', '--status', type=click.IntRange(0, 3), required=False, help="Open (0) Closed (1) Rejected (2) Triage (3)")
-@click.option('-severity', '--severity', type=click.IntRange(0, 4), required=False, help="Info (0) Med (1) High (2) Critical (3)")
-def add_risk(controller, composite, finding, status=0, severity=0):
+@click.option('-name', '--name', required=True, help="Generic risk identifier")
+@click.option('-status', '--status', type=click.Choice([s.value for s in Status]), required=False, default='TO')
+def add_risk(controller, key, name, status):
     """ Apply a risk to an asset key """
-    print(controller.add_risk(key, finding, status, severity))
+    print(controller.add_risk(key, name, status))
 
 
 @chaos.command('upload')
 @click.pass_obj
 @handle_api_error
 @click.argument('name')
 def upload(controller, name):
@@ -128,16 +132,30 @@
 @click.argument('key')
 @click.argument('path')
 def download(controller, key, path):
     """ Download any previous uploaded file """
     controller.download(key, path)
 
 
+@chaos.command('search')
+@click.pass_obj
+@handle_api_error
+@click.option('-term', '--term', help="Enter a search term")
+def search(controller, term=""):
+    """ Query the data store for arbitrary matches """
+    resp = controller.my(dict(key=term))
+    for key, value in resp.items():
+        if isinstance(value, list):
+            for hit in value:
+                print(f"{hit['key']}")
+
+
 @chaos.command('test')
 @click.pass_obj
 def trigger_all_tests(controller):
+    """ Run integration test suite """
     try:
         import pytest
     except ModuleNotFoundError:
         print("Install pytest using 'pip install pytest' to run this command")
     test_directory = os.path.relpath("praetorian_cli/sdk/test", os.getcwd())
     pytest.main([test_directory])
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/chaos.py` & `praetorian_cli-0.8/praetorian_cli/sdk/chaos.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,41 @@
     def my(self, params: dict) -> {}:
         resp = requests.get(f"{self.keychain.api}/my", params=params, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def add_risk(self, key: str, finding: str, status: int = 0, severity: int = 0):
-        data = dict(key=key, finding=finding, status=status, severity=severity)
+    def add_risk(self, key: str, name: str, status: str):
+        data = dict(key=key, name=name, status=status)
 
         resp = requests.post(f"{self.keychain.api}/risk", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
-    def upsert_seed(self, dns: str, status: int, comment: str = "") -> {}:
-        data = {"seed": dns, "status": status, "description": comment}
+    def add_asset(self, seed: str, status: str, comment: str = "") -> {}:
+        data = {"seed": seed, "status": status, "comment": comment}
 
         resp = requests.post(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
+    def update_asset(self, key: str, status: str, comment: str = "") -> {}:
+        data = {"key": key, "status": status, "comment": comment}
+
+        resp = requests.put(f"{self.keychain.api}/asset", json=data, headers=self.keychain.headers)
+        if not resp.ok:
+            raise Exception(f'[{resp.status_code}] Request failed')
+        return resp.json()
+
+    @verify_credentials
     def link_account(self, username: str, config: str):
         resp = requests.post(f"{self.keychain.api}/account/{username}", json={'config':config}, headers=self.keychain.headers)
         if not resp.ok:
             raise Exception(f'[{resp.status_code}] Request failed')
         return resp.json()
 
     @verify_credentials
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/keychain.py` & `praetorian_cli-0.8/praetorian_cli/sdk/keychain.py`

 * *Files identical despite different names*

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_file_upload.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_job_capabilities.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_job_capabilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from praetorian_cli.sdk.test.utils import Utils
+from praetorian_cli.sdk.test.utils import Utils, threshold
 
 from praetorian_cli.sdk.test import BaseTest
 
 
 class TestJob(BaseTest):
 
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
         self.seed = "contoso.com"
-        self.capabilities = ['vulnerability', 'whois', 'subfinder', 'cidr', 'portscan', 'code', 'secrets']
+        self.capabilities = ['vulnerability', 'whois', 'subfinder', 'cidr', 'portscan', 'github', 'secrets']
         self.utils = Utils(self.chaos)
 
     def test_my_jobs(self):
-        response = self.utils.key(dict(key=f'#job#{self.seed}'), 300, 60)
+        response = self.utils.wait_for_key(dict(key=f'#job#{threshold()}'), 300, 60)
         assert response.get('jobs'), "Received empty response for my jobs"
 
+        found_seed = False
         for my_job in response.get('jobs', []):
             print(my_job)
             assert my_job['username'] == self.username, "Job did not have username"
-            assert self.seed in my_job['key'], "Job key did not have required seed"
-            assert my_job['key'].split('#')[
-                       -2] in self.capabilities, "Job capability is not in defined capabilities"
+            assert my_job['source'] in self.capabilities, "Job capability is not in defined capabilities"
+            if self.seed in my_job['key']:
+                found_seed = True
+        assert found_seed, "Failed to find job with seed"
 
     def test_my_assets(self):
         response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'), 40, 5)
         assert response.get('assets'), "Received empty response for my assets"
 
         for my_asset in response.get('assets', []):
             assert my_asset['username'] == self.username, f"Job did not have username = {self.username}"
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_link_account.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_link_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class TestLinkAccount(BaseTest):
 
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
         self.link_account_name = f"chaos_cli_test_{random.randint(0, 9999)}"
 
     def test_link_account(self):
-        response = self.chaos.link_account(username=self.link_account_name, secret="")
+        response = self.chaos.link_account(username=self.link_account_name, config="")
         assert response['member'] == self.link_account_name
         my_accounts=self.chaos.my(dict(key=f'#account#{self.username}'))['accounts']
         assert any(account.get("member") == self.link_account_name for account in my_accounts)
 
     def test_unlink_account(self):
         response = self.chaos.unlink_account(username=self.link_account_name)
         assert response['member'] == self.link_account_name
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_manual_risk.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_manual_risk.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 
 class TestRisk(BaseTest):
 
     def setup_class(self):
         self.chaos, self.username = BaseTest.setup_chaos(self)
         self.seed = "contoso.com"
-        self.finding = "Foobar Finding"
+        self.name = "Foobar Finding"
         self.utils = Utils(self.chaos)
 
     def test_risk(self):
         self.utils.add_seed(self.seed)
         response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'))
         assert response, "Received empty response for my Assets"
 
-        self.chaos.add_risk(dict(key=f'#asset#{self.seed}'), self.finding)
+        self.chaos.add_risk(key=f'#asset#{self.seed}', name=self.name)
         my_risk = self.chaos.my(dict(key=f'#risk#{self.seed}'))
         assert my_risk is not None
         self.utils.freeze_seed(self.seed)
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_nvd.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_nvd.py`

 * *Files identical despite different names*

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/test_seed.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/test_seed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from praetorian_cli.sdk.test import BaseTest
-from praetorian_cli.sdk.test.utils import Utils
+from praetorian_cli.sdk.test.utils import Utils, threshold
 
 
 @pytest.fixture(scope="class", params=["contoso.com", "1.1.1.1/32"])
 def seed(request):
     request.cls.seed = request.param
 
 
@@ -24,24 +24,24 @@
     def test_my_seed(self):
         response = self.chaos.my(dict(key=f'#seed#{self.seed}'))
         for my_seed in response['seeds']:
             assert my_seed['username'] == self.username, f"Seed did not have username = {self.username}"
             assert my_seed['seed'] in self.seed
 
     def test_my_job(self):
-        response = self.utils.wait_for_key(dict(key=f'#job#{self.seed}'))
+        response = self.utils.wait_for_key(dict(key=f'#job#{threshold()}'))
         assert response is not None, "Received empty response for my Jobs"
         for job in response['jobs']:
-            assert job['name'] is not '', "Job Capability is empty"
+            assert job['source'] is not '', "Job Capability is empty"
             assert job['status'] is not None, "Job Status is empty"
 
     def test_my_asset(self):
         response = self.utils.wait_for_key(dict(key=f'#asset#{self.seed}'))
         assert response is not None, "Received empty response for my Assets"
         for asset in response['assets']:
             assert asset['seed'] == self.seed, "Seed is empty"
-            assert asset['ip'] or asset['dns'], "Asset fields IP and DNS are both empty"
+            assert asset['name'] or asset['dns'], "Asset fields IP and DNS are both empty"
 
     def test_delete_seed(self):
         response = self.utils.freeze_seed(self.seed)
         assert response['seed'] == self.seed
         assert response['status'] is 1
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli/sdk/test/utils.py` & `praetorian_cli-0.8/praetorian_cli/sdk/test/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import time
+from datetime import datetime, timedelta
 
 
+def threshold():
+    return datetime.utcnow().strftime('%Y-%m-%d')
+
 def assert_files_equal(file1_path, file2_path):
     with open(file1_path, 'r') as file1:
         content1 = file1.read()
 
     with open(file2_path, 'r') as file2:
         content2 = file2.read()
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli.egg-info/PKG-INFO` & `praetorian_cli-0.8/praetorian_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praetorian-cli
-Version: 0.7.2
+Version: 0.8.0
 Summary: For interacting with the Chaos API
 Home-page: https://github.com/praetorian-inc/praetorian-cli
 Author: Praetorian Labs
 Author-email: research@praetorian.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `praetorian-cli-0.7.2/praetorian_cli.egg-info/SOURCES.txt` & `praetorian_cli-0.8/praetorian_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `praetorian-cli-0.7.2/setup.cfg` & `praetorian_cli-0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = praetorian-cli
-version = 0.7.2
+version = 0.8.0
 author = Praetorian Labs
 author_email = research@praetorian.com
 description = For interacting with the Chaos API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/praetorian-inc/praetorian-cli
 classifiers =
```

