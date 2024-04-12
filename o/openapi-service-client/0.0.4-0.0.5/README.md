# Comparing `tmp/openapi_service_client-0.0.4.tar.gz` & `tmp/openapi_service_client-0.0.5.tar.gz`

## Comparing `openapi_service_client-0.0.4.tar` & `openapi_service_client-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,50 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/client.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/client_configuration.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/__init__.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client.py
--rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/client/test_client_live.py
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/README.md
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/anthropic.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/cohere.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/converter.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/llm_provider.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/openai.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/payload_extractor.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_complex_request_body_mixed.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_anthropic.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_cohere.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_openai.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_cohere_conversion.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_openai_conversion.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/complex_types_openapi_service.json
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/PKG-INFO
```

### Comparing `openapi_service_client-0.0.4/.github/workflows/tests.yml` & `openapi_service_client-0.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/client.py` & `openapi_service_client-0.0.5/src/openapi_service_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,43 @@
-import json
 from typing import Any, Dict
 
-from openapi_service_client.client_configuration import OpenAPIServiceClientConfiguration
+from openapi_service_client.client_configuration import ClientConfiguration
 from openapi_service_client.http_client import VALID_HTTP_METHODS
 from openapi_service_client.request_builder import RequestBuilder
 from openapi_service_client.spec import Operation
 
 
 class OpenAPIServiceClient:
     def __init__(
         self,
-        client_config: OpenAPIServiceClientConfiguration,
+        client_config: ClientConfiguration,
     ):
         self.openapi_spec = client_config.get_openapi_spec()
         self.http_client = client_config.get_http_client()
         self.request_builder = RequestBuilder(client_config)
+        self.payload_extractor = client_config.get_payload_extractor()
 
     def get_operations(self) -> Dict[str, Dict[str, Operation]]:
         operations: Dict[str, Dict[str, Operation]] = {}
         for path, path_item in self.openapi_spec.get_paths().items():
             operations[path] = {}
             for method, operation in path_item.items():
                 if method in VALID_HTTP_METHODS:
                     operations[path][method] = operation
         return operations
 
-    def _find_function_params(self, payload: Dict[str, Any]) -> Dict[str, Any]:
-        if isinstance(payload, dict):
-            if "name" in payload and "arguments" in payload:
-                return payload
-            for _, value in payload.items():
-                if isinstance(value, dict):
-                    result = self._find_function_params(value)
-                    if result:
-                        return result
-        raise OpenAPIClientError("No OpenAI function-calling JSON payload found", payload)
-
-    def invoke(self, openai_fc_payload: Dict[str, Any]) -> Any:
-        fn_invocation_payload = self._find_function_params(openai_fc_payload)
-
-        # fn_invocation_payload guaranteed to have "name" and "arguments" keys from here on
-        arguments = fn_invocation_payload.get("arguments")
-        if isinstance(arguments, str):
-            # it should always be a JSON string, but you never know with all LLM providers
-            try:
-                args = json.loads(arguments)
-            except json.JSONDecodeError as e:
-                raise OpenAPIClientError(f"Error parsing OpenAI function-calling arguments: {e!s}", arguments) from e
-        elif isinstance(arguments, dict):
-            args = arguments
-        else:
-            raise OpenAPIClientError(f"Invalid arguments type: {type(arguments)}", arguments)
+    def invoke(self, function_payload: Dict[str, Any]) -> Any:
+        fn_invocation_payload = self.payload_extractor.extract_function_invocation(function_payload)
+        if not fn_invocation_payload:
+            raise OpenAPIClientError(
+                f"Failed to extract function invocation payload from {function_payload} using "
+                f"{self.payload_extractor.__class__.__name__}. Ensure the payload format matches the expected "
+                "structure for the designated LLM extractor."
+            )
+        # fn_invocation_payload, if not empty, guaranteed to have "name" and "arguments" keys from here on
         operation = self.openapi_spec.find_operation_by_id(fn_invocation_payload.get("name"))
-        request = self.request_builder.build_request(operation, **args)
+        request = self.request_builder.build_request(operation, **fn_invocation_payload.get("arguments"))
         return self.http_client.send_request(request)
 
 
 class OpenAPIClientError(Exception):
     pass
```

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/client_configuration.py` & `openapi_service_client-0.0.5/src/openapi_service_client/client_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 import os
 from pathlib import Path
-from typing import Any, Dict, Optional, Protocol, Union
+from typing import Any, Dict, List, Optional, Protocol, Union
 
 from openapi_service_client.config import (
     ApiKeyAuthentication,
     AuthenticationStrategy,
     HTTPAuthentication,
     HttpClientConfig,
     OAuthAuthentication,
     PassThroughAuthentication,
 )
 from openapi_service_client.http_client import AbstractHttpClient, RequestsHttpClient
+from openapi_service_client.providers import LLMProvider, OpenAILLMProvider
+from openapi_service_client.providers.payload_extractor import FunctionPayloadExtractor
 from openapi_service_client.spec import OpenAPISpecification
 
 
-class OpenAPIServiceClientConfiguration(Protocol):
+class ClientConfiguration(Protocol):
 
     def get_http_client(self) -> AbstractHttpClient:
         pass
 
     def get_http_client_config(self) -> HttpClientConfig:
         pass
 
     def get_auth_config(self) -> AuthenticationStrategy:
         pass
 
     def get_openapi_spec(self) -> OpenAPISpecification:
         pass
 
+    def get_tools_definitions(self) -> List[Dict[str, Any]]:
+        pass
+
+    def get_payload_extractor(self) -> FunctionPayloadExtractor:
+        pass
 
-class DefaultOpenAPIServiceClientConfiguration(OpenAPIServiceClientConfiguration):
+
+class _DefaultOpenAPIServiceClientConfiguration(ClientConfiguration):
 
     def __init__(
         self,
-        openapi_spec: Union[str, Dict[str, Any]],
+        openapi_spec: Union[str, Path],
         credentials: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None,
         http_client: Optional[AbstractHttpClient] = None,
+        http_client_config: Optional[HttpClientConfig] = None,
+        provider: Optional[LLMProvider] = None,
     ):
         if isinstance(openapi_spec, (str, Path)) and os.path.isfile(openapi_spec):
             self.openapi_spec = OpenAPISpecification.from_file(openapi_spec)
         elif isinstance(openapi_spec, dict):
             self.openapi_spec = OpenAPISpecification.from_dict(openapi_spec)
         else:
             raise ValueError("Invalid OpenAPI specification format. Expected file path or dictionary.")
 
         self.credentials = credentials
-        self.http_client = http_client or RequestsHttpClient(self.get_http_client_config())
+        self.http_client = http_client or RequestsHttpClient(http_client_config)
+        self.http_client_config = http_client_config or HttpClientConfig()
+        self.provider = provider or OpenAILLMProvider()
 
     def get_openapi_spec(self) -> OpenAPISpecification:
         return self.openapi_spec
 
     def get_http_client(self) -> AbstractHttpClient:
         return self.http_client
 
     def get_http_client_config(self) -> HttpClientConfig:
-        return HttpClientConfig()
+        return self.http_client_config
+
+    def get_tools_definitions(self) -> List[Dict[str, Any]]:
+        return self.provider.get_schema_converter(self.openapi_spec).convert()
+
+    def get_payload_extractor(self) -> FunctionPayloadExtractor:
+        return self.provider.get_payload_extractor()
 
     def get_auth_config(self) -> AuthenticationStrategy:
         if self.credentials is None:
             return PassThroughAuthentication()
 
         if isinstance(self.credentials, AuthenticationStrategy):
             return self.credentials
@@ -94,34 +112,48 @@
         elif "access_token" in credentials:
             token_type = credentials.get("token_type", "Bearer")
             return OAuthAuthentication(access_token=credentials["access_token"], token_type=token_type)
         else:
             raise ValueError("Unable to create authentication from provided credentials: {credentials}")
 
 
-class OpenAPIServiceClientConfigurationBuilder:
+class ClientConfigurationBuilder:
     def __init__(self):
-        self._openapi_spec: Union[str, Dict[str, Any], None] = None
+        self._openapi_spec: Union[str, Path, None] = None
         self._credentials: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None
         self._http_client: Optional[AbstractHttpClient] = None
+        self._http_client_config: Optional[HttpClientConfig] = None
+        self._provider: Optional[LLMProvider] = None
 
-    def with_openapi_spec(self, openapi_spec: Union[str, Dict[str, Any]]) -> "OpenAPIServiceClientConfigurationBuilder":
+    def with_openapi_spec(self, openapi_spec: Union[str, Path]) -> "ClientConfigurationBuilder":
         self._openapi_spec = openapi_spec
         return self
 
     def with_credentials(
         self, credentials: Union[str, Dict[str, Any], AuthenticationStrategy]
-    ) -> "OpenAPIServiceClientConfigurationBuilder":
+    ) -> "ClientConfigurationBuilder":
         self._credentials = credentials
         return self
 
-    def with_http_client(self, http_client: AbstractHttpClient) -> "OpenAPIServiceClientConfigurationBuilder":
+    def with_http_client(self, http_client: AbstractHttpClient) -> "ClientConfigurationBuilder":
         self._http_client = http_client
         return self
 
-    def build(self) -> OpenAPIServiceClientConfiguration:
+    def with_http_client_config(self, http_client_config: HttpClientConfig) -> "ClientConfigurationBuilder":
+        self._http_client_config = http_client_config
+        return self
+
+    def with_provider(self, provider: LLMProvider) -> "ClientConfigurationBuilder":
+        self._provider = provider
+        return self
+
+    def build(self) -> ClientConfiguration:
         if self._openapi_spec is None:
             raise ValueError("OpenAPI specification must be provided to build a configuration.")
 
-        return DefaultOpenAPIServiceClientConfiguration(
-            openapi_spec=self._openapi_spec, credentials=self._credentials, http_client=self._http_client
+        return _DefaultOpenAPIServiceClientConfiguration(
+            openapi_spec=self._openapi_spec,
+            credentials=self._credentials,
+            http_client=self._http_client,
+            http_client_config=self._http_client_config,
+            provider=self._provider,
         )
```

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.5/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.5/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.5/src/openapi_service_client/request_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict
 
-from openapi_service_client.client import OpenAPIServiceClientConfiguration
+from openapi_service_client.client import ClientConfiguration
 from openapi_service_client.config import PassThroughAuthentication
 from openapi_service_client.spec import Operation
 
 
 class RequestBuilder:
     def __init__(
         self,
-        client_config: OpenAPIServiceClientConfiguration,
+        client_config: ClientConfiguration,
     ):
         self.openapi_parser = client_config.get_openapi_spec()
         self.http_client = client_config.get_http_client()
         self.auth_config = client_config.get_auth_config() or PassThroughAuthentication()
 
     def build_request(self, operation: Operation, **kwargs) -> Any:
         url = self._build_url(operation, **kwargs)
```

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.5/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.5/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/conftest.py` & `openapi_service_client-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/client/test_client.py` & `openapi_service_client-0.0.5/tests/client/test_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 
 from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from tests.conftest import FastAPITestClient
 
 """
 Tests OpenAPIServiceClient with three FastAPI apps for different parameter types:
 
 - **greet_mix_params_body**: A POST endpoint `/greet/<name>` accepting a JSON payload with a message, returning a
 greeting with the name from the URL and the message from the payload.
@@ -64,56 +64,59 @@
 
     return app
 
 
 class TestOpenAPI:
 
     def test_greet_mix_params_body(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_mix_params_body_app()),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_mix_params_body_app()))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John", "message": "Bonjour"}',
                 "name": "greet",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Bonjour, John from mix_params_body!"}
 
     def test_greet_params_only(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_params_only_app()),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_params_only_app()))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetParams",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from params_only!"}
 
     def test_greet_request_body_only(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_request_body_only_app()),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_request_body_only_app()))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John", "message": "Hola"}',
                 "name": "greetBody",
             },
             "type": "function",
```

### Comparing `openapi_service_client-0.0.4/tests/client/test_client_auth.py` & `openapi_service_client-0.0.5/tests/client/test_client_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     HTTPAuthorizationCredentials,
     HTTPBasic,
     HTTPBasicCredentials,
     HTTPBearer,
 )
 
 from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.config import ApiKeyAuthentication, HTTPAuthentication, OAuthAuthentication
 from tests.conftest import FastAPITestClient
 
 API_KEY = "secret_api_key"
 BASIC_AUTH_USERNAME = "admin"
 BASIC_AUTH_PASSWORD = "secret_password"
 
@@ -130,116 +130,122 @@
 
     return app
 
 
 class TestOpenAPIAuth:
 
     def test_greet_api_key_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_api_key_auth_app()),
-                credentials=ApiKeyAuthentication(API_KEY),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_api_key_auth_app()))
+            .with_credentials(ApiKeyAuthentication(API_KEY))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKey",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_auth, using secret_api_key"}
 
     def test_greet_basic_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_basic_auth_app()),
-                credentials=HTTPAuthentication(BASIC_AUTH_USERNAME, BASIC_AUTH_PASSWORD),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_basic_auth_app()))
+            .with_credentials(HTTPAuthentication(BASIC_AUTH_USERNAME, BASIC_AUTH_PASSWORD))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetBasicAuth",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from basic_auth, using admin"}
 
     def test_greet_api_key_query_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_api_key_query_app()),
-                credentials=ApiKeyAuthentication(API_KEY_QUERY),
-            ),
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_api_key_query_app()))
+            .with_credentials(ApiKeyAuthentication(API_KEY_QUERY))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKeyQuery",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_query_auth, using secret_api_key_query"}
 
     def test_greet_api_key_cookie_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_api_key_cookie_app()),
-                credentials=ApiKeyAuthentication(API_KEY_COOKIE),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_api_key_cookie_app()))
+            .with_credentials(ApiKeyAuthentication(API_KEY_COOKIE))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetApiKeyCookie",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from api_key_cookie_auth, using secret_api_key_cookie"}
 
     def test_greet_bearer_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_bearer_auth_app()),
-                credentials=HTTPAuthentication(token=BEARER_TOKEN),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_bearer_auth_app()))
+            .with_credentials(HTTPAuthentication(token=BEARER_TOKEN))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetBearerAuth",
             },
             "type": "function",
         }
         response = client.invoke(payload)
         assert response == {"greeting": "Hello, John from bearer_auth, using secret_bearer_token"}
 
     def test_greet_oauth_auth(self, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_greeting_service.yml",
-                http_client=FastAPITestClient(create_greet_oauth_auth_app()),
-                credentials=OAuthAuthentication(OAUTH_TOKEN),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_greeting_service.yml")
+            .with_http_client(FastAPITestClient(create_greet_oauth_auth_app()))
+            .with_credentials(OAuthAuthentication(OAUTH_TOKEN))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"name": "John"}',
                 "name": "greetOAuth",
             },
             "type": "function",
```

### Comparing `openapi_service_client-0.0.4/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.5/tests/client/test_client_complex_request_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel
 
 from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from tests.conftest import FastAPITestClient
 
 
 class Customer(BaseModel):
     name: str
     email: str
 
@@ -48,19 +48,21 @@
     return app
 
 
 class TestComplexRequestBody:
 
     @pytest.mark.parametrize("spec_file_path", ["openapi_order_service.yml", "openapi_order_service.json"])
     def test_create_order(self, spec_file_path, test_files_path):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / spec_file_path, http_client=FastAPITestClient(create_order_app())
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / spec_file_path)
+            .with_http_client(FastAPITestClient(create_order_app()))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         order_json = {
             "customer": {"name": "John Doe", "email": "john@example.com"},
             "items": [
                 {"product": "Product A", "quantity": 2},
                 {"product": "Product B", "quantity": 1},
             ],
         }
```

### Comparing `openapi_service_client-0.0.4/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.5/tests/client/test_client_error_handling.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import pytest
 from fastapi import FastAPI, HTTPException
 
 from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import DefaultOpenAPIServiceClientConfiguration
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.http_client import HttpClientError
 from tests.conftest import FastAPITestClient
 
 
 def create_error_handling_app() -> FastAPI:
     app = FastAPI()
 
@@ -18,20 +18,21 @@
 
     return app
 
 
 class TestErrorHandling:
     @pytest.mark.parametrize("status_code", [400, 401, 403, 404, 500])
     def test_http_error_handling(self, test_files_path, status_code):
-        client = OpenAPIServiceClient(
-            DefaultOpenAPIServiceClientConfiguration(
-                openapi_spec=test_files_path / "openapi_error_handling.yml",
-                http_client=FastAPITestClient(create_error_handling_app()),
-            )
+        builder = ClientConfigurationBuilder()
+        config = (
+            builder.with_openapi_spec(test_files_path / "openapi_error_handling.yml")
+            .with_http_client(FastAPITestClient(create_error_handling_app()))
+            .build()
         )
+        client = OpenAPIServiceClient(config)
         json_error = {"status_code": status_code}
         payload = {
             "type": "function",
             "function": {
                 "arguments": json.dumps(json_error),
                 "name": "raiseHttpError",
             },
```

### Comparing `openapi_service_client-0.0.4/tests/client/test_client_live.py` & `openapi_service_client-0.0.5/tests/client/test_client_live.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import json
 import os
 
 import pytest
 
 from openapi_service_client.client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import OpenAPIServiceClientConfigurationBuilder
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
 
 class TestClientLive:
 
     @pytest.mark.skipif("SERPERDEV_API_KEY" not in os.environ, reason="SERPERDEV_API_KEY not set")
     def test_serperdev(self, test_files_path):
-        builder = OpenAPIServiceClientConfigurationBuilder()
+        builder = ClientConfigurationBuilder()
         config = (
             builder.with_openapi_spec(test_files_path / "serper.yaml")
             .with_credentials(os.getenv("SERPERDEV_API_KEY"))
             .build()
         )
         serper_api = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
                 "arguments": '{"q": "Who was Zoran Djindjic?"}',
-                "name": "search",
+                "name": "serperdev_search",
             },
             "type": "function",
         }
         response = serper_api.invoke(payload)
         assert "politician" in str(response)
 
     def test_github(self, test_files_path):
-        builder = OpenAPIServiceClientConfigurationBuilder()
+        builder = ClientConfigurationBuilder()
         config = builder.with_openapi_spec(test_files_path / "github_compare.yml").build()
         api = OpenAPIServiceClient(config)
 
         params = {"owner": "deepset-ai", "repo": "haystack", "basehead": "main...add_default_adapter_filters"}
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
```

### Comparing `openapi_service_client-0.0.4/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.5/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.5/tests/test_files/openapi_greeting_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.5/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.5/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/tests/test_files/serper.yaml` & `openapi_service_client-0.0.5/tests/test_files/serper.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   version: 1.0.0
   description: API for performing search queries
 servers:
   - url: https://google.serper.dev
 paths:
   /search:
     post:
-      operationId: search
+      operationId: serperdev_search
       description: Search the web with Google
       requestBody:
         required: true
         content:
           application/json:
             schema:
               type: object
```

### Comparing `openapi_service_client-0.0.4/.gitignore` & `openapi_service_client-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/LICENSE` & `openapi_service_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.4/README.md` & `openapi_service_client-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,162 @@
+Metadata-Version: 2.3
+Name: openapi-service-client
+Version: 0.0.5
+Summary: A client library for invoking APIs based on provided OpenAPI specifications
+Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
+Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
+Project-URL: Source, https://github.com/vblagoje/openapi-service-client
+Author-email: Vladimir Blagojevic <dovlex@gmail.com>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
+Requires-Dist: jsonref
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # OpenAPI Service Client
 [![PyPI - Version](https://img.shields.io/pypi/v/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
-OpenAPI Service Client is a Python library that enables seamless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the OpenAI function-calling JSON format, making it easy to integrate with LLM-generated function calls.
+OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
+
+## Motivation
+
+The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services regardless of the LLM provider.
+
+The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, making it a versatile tool for integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling payload formats.
 
 ## Features
 
-- Seamless integration with LLM-generated function calls using OpenAI's function-calling JSON format
-- Automatic handling of REST invocations and data retrieval based on OpenAPI specifications
-- Support for various authentication strategies, including API key and HTTP authentication
+- Easy integration with LLM-generated function calls using various function-calling JSON formats
+- Support for various LLM providers, including OpenAI, Anthropic, and Cohere
+- Automatic handling of REST invocations based on OpenAPI specifications
+- Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
 - Flexible configuration options for adapting the client behavior
-- Easy integration with existing Python projects
+- Extensible architecture for adding support for additional LLM providers and function-calling payload formats
+
 
 ## Installation
 
 You can install OpenAPI Service Client using pip:
 
 ```shell
 pip install openapi-service-client
 ```
 
 ## Usage
 
 To effectively use the `OpenAPIServiceClient`, follow these steps to configure and invoke operations on your target API defined by an OpenAPI specification.
 
-### Step 1: Configuration
-
-Begin by creating a client configuration using the `OpenAPIServiceClientConfigurationBuilder`. This configuration includes the path to your OpenAPI specification and the authentication details.
-
-#### Configuration Example:
+### OpenAI Example
 
 ```python
-from openapi_service_client import OpenAPIServiceClient
-from openapi_service_client.client_configuration import OpenAPIServiceClientConfigurationBuilder
-
-# Initialize the configuration builder
-config_builder = OpenAPIServiceClientConfigurationBuilder()
+import os
+from openai import OpenAI
+from openapi_service_client.client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
+
+builder = ClientConfigurationBuilder()
+config = (
+    builder.with_openapi_spec("path/to/serper.yaml")
+    .with_credentials(os.getenv("SERPERDEV_API_KEY"))
+    .build()
+)
+
+client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
+tool_choice = config.get_tools_definitions()
+response = client.chat.completions.create(
+    model="gpt-3.5-turbo",
+    messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
+    tools=[{"type": "function", "function": tool_choice[0]}],
+    tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
+)
+
+tool_payloads = response.choices[0].message.tool_calls
+serper_api = OpenAPIServiceClient(config)
+response = serper_api.invoke(tool_payloads[0].to_dict())
 
-# Build the configuration
-config = (config_builder
-          .with_openapi_spec("/path/to/your/openapi_spec.yaml")
-          .with_credentials("your_api_key_or_bearer_token")
-          .build())
-
-# Create the client with the configured settings
-api_client = OpenAPIServiceClient(config)
+assert "inventions" in str(response)
 ```
 
-This example demonstrates a basic setup. You can further customize the configuration by specifying additional parameters such as a custom HTTP client or advanced authentication strategies.
-
-### Step 2: Invoking API Operations
-With the client configured, you can invoke operations defined in your OpenAPI specification. Simply pass OpenAI function-calling JSON payloads to the `invoke` method to call the desired operation.
+### Anthropic Example
 
 ```python
-operation_payload = {
-    "id": "call_UNIQUEID123456",
-    "function": {
-        "arguments": "{\"location\": \"San Francisco, CA\", \"num_days\": 3}",
-        "name": "weather_forecast"
-    },
-    "type": "function"
-}
-
-# Execute the operation
-response = api_client.invoke(operation_payload)
-print(response)
-```
-
-In this example, operation_payload contains the necessary information to call the weather_forecast operation, specifying the city and the number of forecast days as arguments. The invoke method sends the request to the API and returns the response.
-
-### Notes on Authentication
-
-The `with_credentials` method in the configuration builder accommodates a variety of authentication mechanisms to suit different API security requirements:
-
-- **API Key Authentication:** Use `ApiKeyAuthentication` when your API requires an API key. This class supports adding the API key in the request header, query parameters, or cookies, based on the API's specification.
+import os
+import anthropic
+from openapi_service_client.client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
+from openapi_service_client.providers import AnthropicLLMProvider
+
+
+builder = ClientConfigurationBuilder()
+config = (
+    builder.with_openapi_spec("path/to/serper.yaml")
+    .with_credentials(os.getenv("SERPERDEV_API_KEY"))
+    .with_provider(AnthropicLLMProvider())
+    .build()
+)
+
+client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
+tool_choice = config.get_tools_definitions()
+
+response = client.beta.tools.messages.create(
+    model="claude-3-opus-20240229",
+    max_tokens=1024,
+    tools=[tool_choice[0]],
+    messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
+)
+
+tool_payload = response.content[1].to_dict()
+serper_api = OpenAPIServiceClient(config)
+response = serper_api.invoke(tool_payload)
 
-    ```python
-    from openapi_service_client.config import ApiKeyAuthentication
-    config_builder.with_credentials(ApiKeyAuthentication(api_key="your_api_key"))
-    ```
-
-- **HTTP Authentication:** For APIs using HTTP Basic or Bearer Authentication, `HTTPAuthentication` allows you to specify credentials. Provide a username and password for Basic authentication, or a token for Bearer authentication.
-
-    ```python
-    from openapi_service_client.config import HTTPAuthentication
-
-    # For Basic Auth
-    config_builder.with_credentials(HTTPAuthentication(username="user", password="pass"))
-
-    # For Bearer Token
-    config_builder.with_credentials(HTTPAuthentication(token="your_bearer_token"))
-    ```
-
-- **OAuth2 Authentication:** Use `OAuthAuthentication` for APIs secured with OAuth2. Specify your access token and, if necessary, the token type (defaults to "Bearer").
-
-    ```python
-    from openapi_service_client.config import OAuthAuthentication
-
-    config_builder.with_credentials(OAuthAuthentication(access_token="your_access_token", token_type="Bearer"))
-    ```
-
-Each authentication strategy is designed to integrate seamlessly with the OpenAPI specification's security schemes, ensuring your API calls are correctly authenticated according to the API's requirements.
-
-#### Implicit Credentials
-
-For a more straightforward setup, the `with_credentials` method allows passing a token directly as a string (or a dictionary), enabling implicit determination of the appropriate authentication strategy based on the API's security requirements.
-
-```python
-config_builder.with_credentials("your_bearer_token")
+assert "inventions" in str(response)
 ```
+### Cohere Example
 
-This method simplifies client configuration for APIs that accept a single token, automatically applying the correct authentication strategy without manual selection.
+```python
+import os
+import cohere
+from openapi_service_client.client import OpenAPIServiceClient
+from openapi_service_client.client_configuration import ClientConfigurationBuilder
+from openapi_service_client.providers import CohereLLMProvider
+
+builder = ClientConfigurationBuilder()
+config = (
+    builder.with_openapi_spec("path/to/serper.yaml")
+    .with_credentials(os.getenv("SERPERDEV_API_KEY"))
+    .with_provider(CohereLLMProvider())
+    .build()
+)
+
+client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
+tool_choices = config.get_tools_definitions()
+
+response = client.chat(
+    model="command-r",
+    preamble="A preamble aka system prompt goes here.",
+    tools=tool_choices,
+    message="Do a google search: Who was Nikola Tesla?",
+)
+
+tool_payload = response.tool_calls[0].dict()
+serper_api = OpenAPIServiceClient(config)
+response = serper_api.invoke(tool_payload)
 
+assert "inventions" in str(response)
+```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
 
 The client handles the REST invocation by constructing the appropriate HTTP request based on the OpenAPI specification. It takes care of parameter placing (path, query, requestBody etc.), payload formatting, authentication, and error handling. The response from the API is then returned to the caller for further processing.
```

### Comparing `openapi_service_client-0.0.4/pyproject.toml` & `openapi_service_client-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pyyaml",
   "requests",
+  "jsonref"
 ]
 
 [project.urls]
 Documentation = "https://github.com/vblagoje/openapi-service-client/blob/main/README.md"
 Issues = "https://github.com/vblagoje/openapi-service-client/issues"
 Source = "https://github.com/vblagoje/openapi-service-client"
 
@@ -37,15 +38,17 @@
 
 [tool.hatch.envs.default]
 dependencies = [
   "httpx",
   "fastapi",
   "coverage[toml]>=6.5",
   "pytest",
-  "pydantic",
+  "openai",
+  "anthropic",
+  "cohere",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
@@ -60,20 +63,22 @@
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
+  "isort>=5.13.0",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/openapi_service_client}"
 style = [
   "ruff check {args:.}",
   "black --check --diff {args:.}",
+  "isort --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
   "ruff check {args:.}",
   "style",
 ]
 all = [
@@ -82,32 +87,37 @@
 ]
 
 [tool.black]
 target-version = ["py37"]
 line-length = 120
 skip-string-normalization = true
 
+[tool.isort]
+profile = "black"
+line_length = 120
+src_paths = ["src", "tests"]
+
+
 [[tool.mypy.overrides]]
 module = "pydantic"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "openapi_service_client.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "fastapi.*"
 ignore_missing_imports = true
 
-
-
 [[tool.mypy.overrides]]
-module = "pydantic_settings"
+module = "jsonref.*"
 ignore_missing_imports = true
 
+
 [tool.mypy]
 namespace_packages = true
 explicit_package_bases = true
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
```

