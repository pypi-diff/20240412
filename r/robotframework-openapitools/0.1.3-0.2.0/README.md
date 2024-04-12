# Comparing `tmp/robotframework_openapitools-0.1.3.tar.gz` & `tmp/robotframework_openapitools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapitools-0.1.3.tar", max compression
+gzip compressed data, was "robotframework_openapitools-0.2.0.tar", max compression
```

## Comparing `robotframework_openapitools-0.1.3.tar` & `robotframework_openapitools-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.1.3/LICENSE
--rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.1.3/docs/README.md
--rwxr-xr-x   0        0        0     3371 2024-04-05 14:46:36.513338 robotframework_openapitools-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.1.3/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    31970 2024-04-05 14:38:46.773098 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_executors.py
--rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_reader.py
--rwxr-xr-x   0        0        0    27138 2024-04-05 14:47:48.776430 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec
--rwxr-xr-x   0        0        0    15546 2024-03-15 20:22:54.832269 robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.1.3/src/OpenApiDriver/py.typed
--rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.1.3/src/OpenApiLibCore/__init__.py
--rwxr-xr-x   0        0        0    12080 2024-02-12 14:16:27.195985 robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_base.py
--rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_utils.py
--rwxr-xr-x   0        0        0      112 2024-03-06 08:33:13.925424 robotframework_openapitools-0.1.3/src/OpenApiLibCore/oas_cache.py
--rwxr-xr-x   0        0        0    33102 2024-04-05 14:47:48.144349 robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    62223 2024-04-05 14:05:14.902473 robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.py
--rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.1.3/src/OpenApiLibCore/py.typed
--rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.1.3/src/OpenApiLibCore/value_utils.py
--rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.1.3/src/roboswag/__init__.py
--rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.1.3/src/roboswag/__main__.py
--rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.1.3/src/roboswag/auth.py
--rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.1.3/src/roboswag/cli.py
--rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.1.3/src/roboswag/core.py
--rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.1.3/src/roboswag/generate/__init__.py
--rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.1.3/src/roboswag/generate/generate.py
--rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.1.3/src/roboswag/generate/models/__init__.py
--rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.1.3/src/roboswag/generate/models/api.py
--rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.1.3/src/roboswag/generate/models/definition.py
--rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.1.3/src/roboswag/generate/models/endpoint.py
--rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.1.3/src/roboswag/generate/models/parameter.py
--rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/response.py
--rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/tag.py
--rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/models/utils.py
--rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/api_init.jinja
--rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/models.jinja
--rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/generate/templates/paths.jinja
--rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.1.3/src/roboswag/logger.py
--rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/__init__.py
--rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/core.py
--rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/schema.py
--rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.1.3/src/roboswag/validate/text_response.py
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0    11558 2024-02-12 15:55:24.206229 robotframework_openapitools-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0      185 2024-03-08 15:13:37.215159 robotframework_openapitools-0.2.0/docs/README.md
+-rwxr-xr-x   0        0        0     3371 2024-04-12 13:00:01.288060 robotframework_openapitools-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1331 2024-03-06 16:35:05.537954 robotframework_openapitools-0.2.0/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32851 2024-04-12 12:59:35.488243 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_executors.py
+-rwxr-xr-x   0        0        0     4652 2024-03-15 20:22:54.832269 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    28323 2024-04-12 13:08:13.742460 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15214 2024-04-12 12:59:35.504855 robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:42:12.630853 robotframework_openapitools-0.2.0/src/OpenApiDriver/py.typed
+-rwxr-xr-x   0        0        0     1591 2024-02-12 14:16:27.194996 robotframework_openapitools-0.2.0/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0    11764 2024-04-12 12:59:35.521702 robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_base.py
+-rwxr-xr-x   0        0        0     2903 2024-02-12 14:16:27.196984 robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_utils.py
+-rwxr-xr-x   0        0        0      112 2024-03-06 08:33:13.925424 robotframework_openapitools-0.2.0/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    33102 2024-04-12 13:08:13.149393 robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    63998 2024-04-12 12:59:35.521702 robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.py
+-rwxr-xr-x   0        0        0        0 2024-01-31 08:43:45.640076 robotframework_openapitools-0.2.0/src/OpenApiLibCore/py.typed
+-rwxr-xr-x   0        0        0    18145 2024-01-31 08:43:45.640833 robotframework_openapitools-0.2.0/src/OpenApiLibCore/value_utils.py
+-rwxr-xr-x   0        0        0      223 2024-03-06 16:35:05.808004 robotframework_openapitools-0.2.0/src/roboswag/__init__.py
+-rwxr-xr-x   0        0        0       35 2024-02-12 15:55:24.208754 robotframework_openapitools-0.2.0/src/roboswag/__main__.py
+-rwxr-xr-x   0        0        0     1323 2024-03-06 16:35:03.918414 robotframework_openapitools-0.2.0/src/roboswag/auth.py
+-rwxr-xr-x   0        0        0     2216 2024-03-06 16:35:05.748050 robotframework_openapitools-0.2.0/src/roboswag/cli.py
+-rwxr-xr-x   0        0        0     2870 2024-03-06 16:35:03.983780 robotframework_openapitools-0.2.0/src/roboswag/core.py
+-rwxr-xr-x   0        0        0       59 2024-02-12 15:55:24.222947 robotframework_openapitools-0.2.0/src/roboswag/generate/__init__.py
+-rwxr-xr-x   0        0        0     4706 2024-03-06 16:35:04.067930 robotframework_openapitools-0.2.0/src/roboswag/generate/generate.py
+-rwxr-xr-x   0        0        0        0 2024-02-12 15:55:24.223963 robotframework_openapitools-0.2.0/src/roboswag/generate/models/__init__.py
+-rwxr-xr-x   0        0        0     8528 2024-03-06 16:35:04.137359 robotframework_openapitools-0.2.0/src/roboswag/generate/models/api.py
+-rwxr-xr-x   0        0        0      841 2024-03-06 16:35:03.958474 robotframework_openapitools-0.2.0/src/roboswag/generate/models/definition.py
+-rwxr-xr-x   0        0        0     2304 2024-03-06 16:35:04.024928 robotframework_openapitools-0.2.0/src/roboswag/generate/models/endpoint.py
+-rwxr-xr-x   0        0        0      682 2024-03-06 16:35:03.991681 robotframework_openapitools-0.2.0/src/roboswag/generate/models/parameter.py
+-rwxr-xr-x   0        0        0      257 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/response.py
+-rwxr-xr-x   0        0        0      561 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/tag.py
+-rwxr-xr-x   0        0        0     1550 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/models/utils.py
+-rwxr-xr-x   0        0        0      621 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/api_init.jinja
+-rwxr-xr-x   0        0        0      357 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/models.jinja
+-rwxr-xr-x   0        0        0     3191 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/generate/templates/paths.jinja
+-rwxr-xr-x   0        0        0     1025 2024-03-06 16:35:04.038806 robotframework_openapitools-0.2.0/src/roboswag/logger.py
+-rwxr-xr-x   0        0        0      188 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/core.py
+-rwxr-xr-x   0        0        0      711 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/schema.py
+-rwxr-xr-x   0        0        0      527 2024-02-12 15:55:24.225590 robotframework_openapitools-0.2.0/src/roboswag/validate/text_response.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 robotframework_openapitools-0.2.0/PKG-INFO
```

### Comparing `robotframework_openapitools-0.1.3/LICENSE` & `robotframework_openapitools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/pyproject.toml` & `robotframework_openapitools-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapitools"
-version = "0.1.3"
+version = "0.2.0"
 description = "A set of Robot Framework libraries to test APIs for which the OAS is available."
 license = "Apache-2.0"
 authors = [
     "Bartlomiej Hirsz <bartek.hirsz@gmail.com>",
     "Mateusz Nojek <matnojek@gmail.com>",
     "Robin Mackaij <r.a.mackaij@gmail.com>"
 ]
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/__init__.py` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,33 @@
         """
         url: str = run_keyword("get_valid_url", path, method)
         response = self.session.request(
             method=method,
             url=url,
             verify=False,
         )
-        assert response.status_code == 401
+        if response.status_code != 401:
+            raise AssertionError(f"Response {response.status_code} was not 401.")
+
+    @keyword
+    def test_forbidden(self, path: str, method: str) -> None:
+        """
+        Perform a request for `method` on the `path`, with the provided authorization.
+
+        This keyword only passes if the response code is 403: Forbidden.
+
+        For this keyword to pass, the authorization parameters used to initialize the
+        library should grant insufficient access rights to the target endpoint.
+        > Note: No headers or (json) body are send with the request. For security
+        reasons, the access rights validation should be checked first.
+        """
+        url: str = run_keyword("get_valid_url", path, method)
+        response: Response = run_keyword("authorized_request", url, method)
+        if response.status_code != 403:
+            raise AssertionError(f"Response {response.status_code} was not 403.")
 
     @keyword
     def test_invalid_url(
         self, path: str, method: str, expected_status_code: int = 404
     ) -> None:
         """
         Perform a request for the provided 'path' and 'method' where the url for
@@ -256,17 +274,15 @@
         ):
             logger.info("Performing request without optional properties and parameters")
             url = run_keyword("get_valid_url", path, method)
             request_data = self.get_request_data(method=method, endpoint=path)
             params = request_data.get_required_params()
             headers = request_data.get_required_headers()
             json_data = (
-                request_data.get_required_properties_dict()
-                if request_data.has_body
-                else None
+                request_data.get_minimal_body_dict() if request_data.has_body else None
             )
             original_data = None
             if method == "PATCH":
                 original_data = self.get_original_data(url=url)
             run_keyword(
                 "perform_validated_request",
                 path,
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec`

 * *Files 1% similar despite different names*

#### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-05T14:47:49+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
-  <version>0.1.3</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-12T13:08:14+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapidriver.py" lineno="352">
+  <version>0.2.0</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="144">
       <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
@@ -282,15 +282,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Test Endpoint" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="157">
+    <kw name="Test Endpoint" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="175">
       <arguments repr="path: str, method: str, status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -302,15 +302,31 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
       <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
-    <kw name="Test Invalid Url" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="115">
+    <kw name="Test Forbidden" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="116">
+      <arguments repr="path: str, method: str">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
+          <name>path</name>
+          <type name="str" typedoc="string">str</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
+          <name>method</name>
+          <type name="str" typedoc="string">str</type>
+        </arg>
+      </arguments>
+      <doc>&lt;p&gt;Perform a request for &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; on the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt;, with the provided authorization.&lt;/p&gt;
+&lt;p&gt;This keyword only passes if the response code is 403: Forbidden.&lt;/p&gt;
+&lt;p&gt;For this keyword to pass, the authorization parameters used to initialize the library should grant insufficient access rights to the target endpoint. &amp;gt; Note: No headers or (json) body are send with the request. For security reasons, the access rights validation should be checked first.&lt;/p&gt;</doc>
+      <shortdoc>Perform a request for `method` on the `path`, with the provided authorization.</shortdoc>
+    </kw>
+    <kw name="Test Invalid Url" source="/workspaces/robotframework-openapitools/src/OpenApiDriver/openapi_executors.py" lineno="133">
       <arguments repr="path: str, method: str, expected_status_code: int = 404">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -444,14 +460,15 @@
       <doc>&lt;p&gt;All arguments are converted to Unicode strings.&lt;/p&gt;</doc>
       <accepts>
         <type>Any</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Test Endpoint</usage>
+        <usage>Test Forbidden</usage>
         <usage>Test Invalid Url</usage>
         <usage>Test Unauthorized</usage>
       </usages>
     </type>
     <type name="tuple" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#tuple&quot;&gt;tuple&lt;/a&gt; literals. They are converted to actual tuples using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including tuples and other containers.&lt;/p&gt;
 &lt;p&gt;If the type has nested types like &lt;code&gt;tuple[str, int, int]&lt;/code&gt;, items are converted to those types automatically. This in new in Robot Framework 6.0.&lt;/p&gt;
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiDriver/openapidriver.py` & `robotframework_openapitools-0.2.0/src/OpenApiDriver/openapidriver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,362 +1,363 @@
-"""
-# OpenApiDriver for Robot Framework®
-
-OpenApiDriver is an extension of the Robot Framework® DataDriver library that allows
-for generation and execution of test cases based on the information in an OpenAPI
-document (also known as Swagger document).
-This document explains how to use the OpenApiDriver library.
-
-For more information about Robot Framework®, see http://robotframework.org.
-
-For more information about the DataDriver library, see
-https://github.com/Snooz82/robotframework-datadriver.
-
----
-
-> Note: OpenApiDriver is still under development so there are currently
-restrictions / limitations that you may encounter when using this library to run
-tests against an API. See [Limitations](#limitations) for details.
-
----
-
-## Installation
-
-If you already have Python >= 3.8 with pip installed, you can simply run:
-
-`pip install --upgrade robotframework-openapidriver`
-
----
-
-## OpenAPI (aka Swagger)
-
-The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
-to RESTful APIs, see https://swagger.io/specification/
-
-The OpenApiDriver module implements a reader class that generates a test case for
-each path, method and response (i.e. every response for each endpoint) that is defined
-in an OpenAPI document, typically an openapi.json or openapi.yaml file.
-
-> Note: OpenApiDriver is designed for APIs based on the OAS v3
-The library has not been tested for APIs based on the OAS v2.
-
----
-
-## Getting started
-
-Before trying to use OpenApiDriver to run automatic validations on the target API
-it's recommended to first ensure that the openapi document for the API is valid
-under the OpenAPI Specification.
-
-This can be done using the command line interface of a package that is installed as
-a prerequisite for OpenApiDriver.
-Both a local openapi.json or openapi.yaml file or one hosted by the API server
-can be checked using the `prance validate <reference_to_file>` shell command:
-
-```shell
-prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
-Processing "http://localhost:8000/openapi.json"...
- -> Resolving external references.
-Validates OK as OpenAPI 3.0.2!
-
-prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
-Processing "/tests/files/petstore_openapi.yaml"...
- -> Resolving external references.
-Validates OK as OpenAPI 3.0.2!
-```
-
-You'll have to change the url or file reference to the location of the openapi
-document for your API.
-
-> Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the OAS to not use recursion is recommended.
-OpenApiDriver has limited support for parsing OpenAPI documents with
-recursion in them. See the `recursion_limit` and `recursion_default` parameters.
-
-If the openapi document passes this validation, the next step is trying to do a test
-run with a minimal test suite.
-The example below can be used, with `source` and `origin` altered to fit your situation.
-
-``` robotframework
-*** Settings ***
-Library            OpenApiDriver
-...                    source=http://localhost:8000/openapi.json
-...                    origin=http://localhost:8000
-Test Template      Validate Using Test Endpoint Keyword
-
-*** Test Cases ***
-Test Endpoint for ${method} on ${path} where ${status_code} is expected
-
-*** Keywords ***
-Validate Using Test Endpoint Keyword
-    [Arguments]    ${path}    ${method}    ${status_code}
-    Test Endpoint
-    ...    path=${path}    method=${method}    status_code=${status_code}
-
-```
-
-Running the above suite for the first time is likely to result in some
-errors / failed tests.
-You should look at the Robot Framework `log.html` to determine the reasons
-for the failing tests.
-Depending on the reasons for the failures, different solutions are possible.
-
-Details about the OpenApiDriver library parameters that you may need can be found
-[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).
-
-The OpenApiDriver also support handling of relations between resources within the scope
-of the API being validated as well as handling dependencies on resources outside the
-scope of the API. In addition there is support for handling restrictions on the values
-of parameters and properties.
-
-Details about the `mappings_path` variable usage can be found
-[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).
-
----
-
-## Limitations
-
-There are currently a number of limitations to supported API structures, supported
-data types and properties. The following list details the most important ones:
-- Only JSON request and response bodies are supported.
-- No support for per-path authorization levels (only simple 401 / 403 validation).
-
-"""
-
-from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
-
-from DataDriver import DataDriver
-from requests.auth import AuthBase
-from requests.cookies import RequestsCookieJar as CookieJar
-from robot.api.deco import library
-
-from OpenApiDriver.openapi_executors import OpenApiExecutors, ValidationLevel
-from OpenApiDriver.openapi_reader import OpenApiReader
-
-
-@library(scope="TEST SUITE", doc_format="ROBOT")
-class OpenApiDriver(OpenApiExecutors, DataDriver):
-    """
-    Visit the [https://github.com/MarketSquare/robotframework-openapidriver | library page]
-    for an introduction and examples.
-    """
-
-    def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
-        self,
-        source: str,
-        origin: str = "",
-        base_path: str = "",
-        included_paths: Optional[Iterable[str]] = None,
-        ignored_paths: Optional[Iterable[str]] = None,
-        ignored_responses: Optional[Iterable[int]] = None,
-        ignored_testcases: Optional[Iterable[Tuple[str, str, int]]] = None,
-        response_validation: ValidationLevel = ValidationLevel.WARN,
-        disable_server_validation: bool = True,
-        mappings_path: Union[str, Path] = "",
-        invalid_property_default_response: int = 422,
-        default_id_property_name: str = "id",
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        require_body_for_invalid_url: bool = False,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        username: str = "",
-        password: str = "",
-        security_token: str = "",
-        auth: Optional[AuthBase] = None,
-        cert: Optional[Union[str, Tuple[str, str]]] = None,
-        verify_tls: Optional[Union[bool, str]] = True,
-        extra_headers: Optional[Dict[str, str]] = None,
-        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
-        proxies: Optional[Dict[str, str]] = None,
-    ):
-        """
-         == Base parameters ==
-
-         === source ===
-         An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
-
-         === origin ===
-         The server (and port) of the target server. E.g. ``https://localhost:8000``
-
-        === base_path ===
-         The routing between ``origin`` and the endpoints as found in the ``paths``
-         section in the openapi document.
-         E.g. ``/petshop/v2``.
-
-         == Test case generation and execution ==
-
-         === included_paths ===
-         A list of paths that will be included when generating the test cases.
-         The ``*`` character can be used at the end of a partial path to include all paths
-         starting with the partial path (wildcard include).
-
-         === ignored_paths ===
-         A list of paths that will be ignored when generating the test cases.
-         The ``*`` character can be used at the end of a partial path to ignore all paths
-         starting with the partial path (wildcard ignore).
-
-         === ignored_responses ===
-         A list of responses that will be ignored when generating the test cases.
-
-         === ignored_testcases ===
-         A list of specific test cases that, if it would be generated, will be ignored.
-         Specific test cases to ignore must be specified as a ``Tuple`` or ``List``
-         of ``path``, ``method`` and ``response``.
-
-         === response_validation ===
-         By default, a ``WARN`` is logged when the Response received after a Request does not
-         comply with the schema as defined in the openapi document for the given operation. The
-         following values are supported:
-
-         - ``DISABLED``: All Response validation errors will be ignored
-         - ``INFO``: Any Response validation erros will be logged at ``INFO`` level
-         - ``WARN``: Any Response validation erros will be logged at ``WARN`` level
-         - ``STRICT``: The Test Case will fail on any Response validation errors
-
-         === disable_server_validation ===
-         If enabled by setting this parameter to ``True``, the Response validation will also
-         include possible errors for Requests made to a server address that is not defined in
-         the list of servers in the openapi document. This generally means that if there is a
-         mismatch, every Test Case will raise this error. Note that ``localhost`` and
-         ``127.0.0.1`` are not considered the same by Response validation.
-
-         == API-specific configurations ==
-
-         === mappings_path ===
-         See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
-         for an in-depth explanation.
-
-         === invalid_property_default_response ===
-         The default response code for requests with a JSON body that does not comply
-         with the schema.
-         Example: a value outside the specified range or a string value
-         for a property defined as integer in the schema.
-
-         === default_id_property_name ===
-         The default name for the property that identifies a resource (i.e. a unique
-         entity) within the API.
-         The default value for this property name is ``id``.
-         If the target API uses a different name for all the resources within the API,
-         you can configure it globally using this property.
-
-         If different property names are used for the unique identifier for different
-         types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
-
-         === faker_locale ===
-         A locale string or list of locale strings to pass to the Faker library to be
-         used in generation of string data for supported format types.
-
-         === require_body_for_invalid_url ===
-         When a request is made against an invalid url, this usually is because of a "404" request;
-         a request for a resource that does not exist. Depending on API implementation, when a
-         request with a missing or invalid request body is made on a non-existent resource,
-         either a 404 or a 422 or 400 Response is normally returned. If the API being tested
-         processes the request body before checking if the requested resource exists, set
-         this parameter to True.
-
-         == Parsing parameters ==
-
-         === recursion_limit ===
-         The recursion depth to which to fully parse recursive references before the
-         `recursion_default` is used to end the recursion.
-
-         === recursion_default ===
-         The value that is used instead of the referenced schema when the
-         `recursion_limit` has been reached.
-         The default `{}` represents an empty object in JSON.
-         Depending on schema definitions, this may cause schema validation errors.
-         If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
-         can be tried as an alternative.
-
-         == Security-related parameters ==
-         _Note: these parameters are equivalent to those in the ``requests`` library._
-
-         === username ===
-         The username to be used for Basic Authentication.
-
-         === password ===
-         The password to be used for Basic Authentication.
-
-         === security_token ===
-         The token to be used for token based security using the ``Authorization`` header.
-
-         === auth ===
-         A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
-         to be used for authentication instead of the ``username`` and ``password``.
-
-         === cert ===
-         The SSL certificate to use with all requests.
-         If string: the path to ssl client cert file (.pem).
-         If tuple: the ('cert', 'key') pair.
-
-         === verify_tls ===
-         Whether or not to verify the TLS / SSL certificate of the server.
-         If boolean: whether or not to verify the server TLS certificate.
-         If string: path to a CA bundle to use for verification.
-
-         === extra_headers ===
-         A dictionary with extra / custom headers that will be send with every request.
-         This parameter can be used to send headers that are not documented in the
-         openapi document or to provide an API-key.
-
-         === cookies ===
-         A dictionary or [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
-         to send with all requests.
-
-         === proxies ===
-         A dictionary of 'protocol': 'proxy url' to use for all requests.
-        """
-        included_paths = included_paths if included_paths else ()
-        ignored_paths = ignored_paths if ignored_paths else ()
-        ignored_responses = ignored_responses if ignored_responses else ()
-        ignored_testcases = ignored_testcases if ignored_testcases else ()
-
-        mappings_path = Path(mappings_path).as_posix()
-        OpenApiExecutors.__init__(
-            self,
-            source=source,
-            origin=origin,
-            base_path=base_path,
-            response_validation=response_validation,
-            disable_server_validation=disable_server_validation,
-            mappings_path=mappings_path,
-            invalid_property_default_response=invalid_property_default_response,
-            default_id_property_name=default_id_property_name,
-            faker_locale=faker_locale,
-            require_body_for_invalid_url=require_body_for_invalid_url,
-            recursion_limit=recursion_limit,
-            recursion_default=recursion_default,
-            username=username,
-            password=password,
-            security_token=security_token,
-            auth=auth,
-            cert=cert,
-            verify_tls=verify_tls,
-            extra_headers=extra_headers,
-            cookies=cookies,
-            proxies=proxies,
-        )
-
-        read_paths_method = self.read_paths
-        DataDriver.__init__(
-            self,
-            reader_class=OpenApiReader,
-            read_paths_method=read_paths_method,
-            included_paths=included_paths,
-            ignored_paths=ignored_paths,
-            ignored_responses=ignored_responses,
-            ignored_testcases=ignored_testcases,
-        )
-
-
-class DocumentationGenerator(OpenApiDriver):
-    __doc__ = OpenApiDriver.__doc__
-
-    @staticmethod
-    def get_keyword_names() -> List[str]:
-        """Curated keywords for libdoc and libspec."""
-        return [
-            "test_unauthorized",
-            "test_invalid_url",
-            "test_endpoint",
-        ]  # pragma: no cover
+"""
+# OpenApiDriver for Robot Framework®
+
+OpenApiDriver is an extension of the Robot Framework® DataDriver library that allows
+for generation and execution of test cases based on the information in an OpenAPI
+document (also known as Swagger document).
+This document explains how to use the OpenApiDriver library.
+
+For more information about Robot Framework®, see http://robotframework.org.
+
+For more information about the DataDriver library, see
+https://github.com/Snooz82/robotframework-datadriver.
+
+---
+
+> Note: OpenApiDriver is still under development so there are currently
+restrictions / limitations that you may encounter when using this library to run
+tests against an API. See [Limitations](#limitations) for details.
+
+---
+
+## Installation
+
+If you already have Python >= 3.8 with pip installed, you can simply run:
+
+`pip install --upgrade robotframework-openapidriver`
+
+---
+
+## OpenAPI (aka Swagger)
+
+The OpenAPI Specification (OAS) defines a standard, language-agnostic interface
+to RESTful APIs, see https://swagger.io/specification/
+
+The OpenApiDriver module implements a reader class that generates a test case for
+each path, method and response (i.e. every response for each endpoint) that is defined
+in an OpenAPI document, typically an openapi.json or openapi.yaml file.
+
+> Note: OpenApiDriver is designed for APIs based on the OAS v3
+The library has not been tested for APIs based on the OAS v2.
+
+---
+
+## Getting started
+
+Before trying to use OpenApiDriver to run automatic validations on the target API
+it's recommended to first ensure that the openapi document for the API is valid
+under the OpenAPI Specification.
+
+This can be done using the command line interface of a package that is installed as
+a prerequisite for OpenApiDriver.
+Both a local openapi.json or openapi.yaml file or one hosted by the API server
+can be checked using the `prance validate <reference_to_file>` shell command:
+
+```shell
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
+Processing "http://localhost:8000/openapi.json"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
+Processing "/tests/files/petstore_openapi.yaml"...
+ -> Resolving external references.
+Validates OK as OpenAPI 3.0.2!
+```
+
+You'll have to change the url or file reference to the location of the openapi
+document for your API.
+
+> Note: Although recursion is technically allowed under the OAS, tool support is limited
+and changing the OAS to not use recursion is recommended.
+OpenApiDriver has limited support for parsing OpenAPI documents with
+recursion in them. See the `recursion_limit` and `recursion_default` parameters.
+
+If the openapi document passes this validation, the next step is trying to do a test
+run with a minimal test suite.
+The example below can be used, with `source` and `origin` altered to fit your situation.
+
+``` robotframework
+*** Settings ***
+Library            OpenApiDriver
+...                    source=http://localhost:8000/openapi.json
+...                    origin=http://localhost:8000
+Test Template      Validate Using Test Endpoint Keyword
+
+*** Test Cases ***
+Test Endpoint for ${method} on ${path} where ${status_code} is expected
+
+*** Keywords ***
+Validate Using Test Endpoint Keyword
+    [Arguments]    ${path}    ${method}    ${status_code}
+    Test Endpoint
+    ...    path=${path}    method=${method}    status_code=${status_code}
+
+```
+
+Running the above suite for the first time is likely to result in some
+errors / failed tests.
+You should look at the Robot Framework `log.html` to determine the reasons
+for the failing tests.
+Depending on the reasons for the failures, different solutions are possible.
+
+Details about the OpenApiDriver library parameters that you may need can be found
+[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).
+
+The OpenApiDriver also support handling of relations between resources within the scope
+of the API being validated as well as handling dependencies on resources outside the
+scope of the API. In addition there is support for handling restrictions on the values
+of parameters and properties.
+
+Details about the `mappings_path` variable usage can be found
+[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).
+
+---
+
+## Limitations
+
+There are currently a number of limitations to supported API structures, supported
+data types and properties. The following list details the most important ones:
+- Only JSON request and response bodies are supported.
+- No support for per-path authorization levels (only simple 401 / 403 validation).
+
+"""
+
+from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+
+from DataDriver import DataDriver
+from requests.auth import AuthBase
+from requests.cookies import RequestsCookieJar as CookieJar
+from robot.api.deco import library
+
+from OpenApiDriver.openapi_executors import OpenApiExecutors, ValidationLevel
+from OpenApiDriver.openapi_reader import OpenApiReader
+
+
+@library(scope="TEST SUITE", doc_format="ROBOT")
+class OpenApiDriver(OpenApiExecutors, DataDriver):
+    """
+    Visit the [https://github.com/MarketSquare/robotframework-openapidriver | library page]
+    for an introduction and examples.
+    """
+
+    def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
+        self,
+        source: str,
+        origin: str = "",
+        base_path: str = "",
+        included_paths: Optional[Iterable[str]] = None,
+        ignored_paths: Optional[Iterable[str]] = None,
+        ignored_responses: Optional[Iterable[int]] = None,
+        ignored_testcases: Optional[Iterable[Tuple[str, str, int]]] = None,
+        response_validation: ValidationLevel = ValidationLevel.WARN,
+        disable_server_validation: bool = True,
+        mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        require_body_for_invalid_url: bool = False,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
+        username: str = "",
+        password: str = "",
+        security_token: str = "",
+        auth: Optional[AuthBase] = None,
+        cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
+        extra_headers: Optional[Dict[str, str]] = None,
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
+    ):
+        """
+         == Base parameters ==
+
+         === source ===
+         An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
+
+         === origin ===
+         The server (and port) of the target server. E.g. ``https://localhost:8000``
+
+        === base_path ===
+         The routing between ``origin`` and the endpoints as found in the ``paths``
+         section in the openapi document.
+         E.g. ``/petshop/v2``.
+
+         == Test case generation and execution ==
+
+         === included_paths ===
+         A list of paths that will be included when generating the test cases.
+         The ``*`` character can be used at the end of a partial path to include all paths
+         starting with the partial path (wildcard include).
+
+         === ignored_paths ===
+         A list of paths that will be ignored when generating the test cases.
+         The ``*`` character can be used at the end of a partial path to ignore all paths
+         starting with the partial path (wildcard ignore).
+
+         === ignored_responses ===
+         A list of responses that will be ignored when generating the test cases.
+
+         === ignored_testcases ===
+         A list of specific test cases that, if it would be generated, will be ignored.
+         Specific test cases to ignore must be specified as a ``Tuple`` or ``List``
+         of ``path``, ``method`` and ``response``.
+
+         === response_validation ===
+         By default, a ``WARN`` is logged when the Response received after a Request does not
+         comply with the schema as defined in the openapi document for the given operation. The
+         following values are supported:
+
+         - ``DISABLED``: All Response validation errors will be ignored
+         - ``INFO``: Any Response validation erros will be logged at ``INFO`` level
+         - ``WARN``: Any Response validation erros will be logged at ``WARN`` level
+         - ``STRICT``: The Test Case will fail on any Response validation errors
+
+         === disable_server_validation ===
+         If enabled by setting this parameter to ``True``, the Response validation will also
+         include possible errors for Requests made to a server address that is not defined in
+         the list of servers in the openapi document. This generally means that if there is a
+         mismatch, every Test Case will raise this error. Note that ``localhost`` and
+         ``127.0.0.1`` are not considered the same by Response validation.
+
+         == API-specific configurations ==
+
+         === mappings_path ===
+         See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
+         for an in-depth explanation.
+
+         === invalid_property_default_response ===
+         The default response code for requests with a JSON body that does not comply
+         with the schema.
+         Example: a value outside the specified range or a string value
+         for a property defined as integer in the schema.
+
+         === default_id_property_name ===
+         The default name for the property that identifies a resource (i.e. a unique
+         entity) within the API.
+         The default value for this property name is ``id``.
+         If the target API uses a different name for all the resources within the API,
+         you can configure it globally using this property.
+
+         If different property names are used for the unique identifier for different
+         types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
+
+         === faker_locale ===
+         A locale string or list of locale strings to pass to the Faker library to be
+         used in generation of string data for supported format types.
+
+         === require_body_for_invalid_url ===
+         When a request is made against an invalid url, this usually is because of a "404" request;
+         a request for a resource that does not exist. Depending on API implementation, when a
+         request with a missing or invalid request body is made on a non-existent resource,
+         either a 404 or a 422 or 400 Response is normally returned. If the API being tested
+         processes the request body before checking if the requested resource exists, set
+         this parameter to True.
+
+         == Parsing parameters ==
+
+         === recursion_limit ===
+         The recursion depth to which to fully parse recursive references before the
+         `recursion_default` is used to end the recursion.
+
+         === recursion_default ===
+         The value that is used instead of the referenced schema when the
+         `recursion_limit` has been reached.
+         The default `{}` represents an empty object in JSON.
+         Depending on schema definitions, this may cause schema validation errors.
+         If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
+         can be tried as an alternative.
+
+         == Security-related parameters ==
+         _Note: these parameters are equivalent to those in the ``requests`` library._
+
+         === username ===
+         The username to be used for Basic Authentication.
+
+         === password ===
+         The password to be used for Basic Authentication.
+
+         === security_token ===
+         The token to be used for token based security using the ``Authorization`` header.
+
+         === auth ===
+         A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
+         to be used for authentication instead of the ``username`` and ``password``.
+
+         === cert ===
+         The SSL certificate to use with all requests.
+         If string: the path to ssl client cert file (.pem).
+         If tuple: the ('cert', 'key') pair.
+
+         === verify_tls ===
+         Whether or not to verify the TLS / SSL certificate of the server.
+         If boolean: whether or not to verify the server TLS certificate.
+         If string: path to a CA bundle to use for verification.
+
+         === extra_headers ===
+         A dictionary with extra / custom headers that will be send with every request.
+         This parameter can be used to send headers that are not documented in the
+         openapi document or to provide an API-key.
+
+         === cookies ===
+         A dictionary or [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
+         to send with all requests.
+
+         === proxies ===
+         A dictionary of 'protocol': 'proxy url' to use for all requests.
+        """
+        included_paths = included_paths if included_paths else ()
+        ignored_paths = ignored_paths if ignored_paths else ()
+        ignored_responses = ignored_responses if ignored_responses else ()
+        ignored_testcases = ignored_testcases if ignored_testcases else ()
+
+        mappings_path = Path(mappings_path).as_posix()
+        OpenApiExecutors.__init__(
+            self,
+            source=source,
+            origin=origin,
+            base_path=base_path,
+            response_validation=response_validation,
+            disable_server_validation=disable_server_validation,
+            mappings_path=mappings_path,
+            invalid_property_default_response=invalid_property_default_response,
+            default_id_property_name=default_id_property_name,
+            faker_locale=faker_locale,
+            require_body_for_invalid_url=require_body_for_invalid_url,
+            recursion_limit=recursion_limit,
+            recursion_default=recursion_default,
+            username=username,
+            password=password,
+            security_token=security_token,
+            auth=auth,
+            cert=cert,
+            verify_tls=verify_tls,
+            extra_headers=extra_headers,
+            cookies=cookies,
+            proxies=proxies,
+        )
+
+        read_paths_method = self.read_paths
+        DataDriver.__init__(
+            self,
+            reader_class=OpenApiReader,
+            read_paths_method=read_paths_method,
+            included_paths=included_paths,
+            ignored_paths=ignored_paths,
+            ignored_responses=ignored_responses,
+            ignored_testcases=ignored_testcases,
+        )
+
+
+class DocumentationGenerator(OpenApiDriver):
+    __doc__ = OpenApiDriver.__doc__
+
+    @staticmethod
+    def get_keyword_names() -> List[str]:
+        """Curated keywords for libdoc and libspec."""
+        return [
+            "test_unauthorized",
+            "test_forbidden",
+            "test_invalid_url",
+            "test_endpoint",
+        ]  # pragma: no cover
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/__init__.py` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_base.py` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-"""
-Module holding the (base) classes that can be used by the user of the OpenApiLibCore
-to implement custom mappings for dependencies between resources in the API under
-test and constraints / restrictions on properties of the resources.
-"""
-
-from abc import ABC
-from copy import deepcopy
-from dataclasses import dataclass, fields
-from logging import getLogger
-from random import choice, shuffle
-from typing import Any, Dict, List, Optional, Union
-from uuid import uuid4
-
-from OpenApiLibCore import value_utils
-
-logger = getLogger(__name__)
-
-NOT_SET = object()
-SENTINEL = object()
-
-
-def resolve_schema(schema: Dict[str, Any]) -> Dict[str, Any]:
-    """
-    Helper function to resolve allOf, anyOf and oneOf instances in a schema.
-
-    The schemas are used to generate values for headers, query parameters and json
-    bodies to be able to make requests.
-    """
-    # Schema is mutable, so deepcopy to prevent mutation of original schema argument
-    resolved_schema = deepcopy(schema)
-
-    # allOf / anyOf / oneOf may be nested, so recursively resolve the dict-typed values
-    for key, value in resolved_schema.items():
-        if isinstance(value, dict):
-            resolved_schema[key] = resolve_schema(value)
-
-    # When handling allOf there should no duplicate keys, so the schema parts can
-    # just be merged after resolving the individual parts
-    if schema_parts := resolved_schema.pop("allOf", None):
-        for schema_part in schema_parts:
-            resolved_part = resolve_schema(schema_part)
-            resolved_schema = merge_schemas(resolved_schema, resolved_part)
-    # Handling anyOf and oneOf requires extra logic to deal with the "type" information.
-    # Some properties / parameters may be of different types and each type may have its
-    # own restrictions e.g. a parameter that accepts an enum value (string) or an
-    # integer value within a certain range.
-    # Since the library needs all this information for different purposes, the
-    # schema_parts cannot be merged, so a helper property / key "types" is introduced.
-    any_of = resolved_schema.pop("anyOf", [])
-    one_of = resolved_schema.pop("oneOf", [])
-    schema_parts = any_of if any_of else one_of
-
-    for schema_part in schema_parts:
-        resolved_part = resolve_schema(schema_part)
-        if isinstance(resolved_part, dict) and "type" in resolved_part.keys():
-            if "types" in resolved_schema.keys():
-                resolved_schema["types"].append(resolved_part)
-            else:
-                resolved_schema["types"] = [resolved_part]
-        else:
-            resolved_schema = merge_schemas(resolved_schema, resolved_part)
-
-    return resolved_schema
-
-
-def merge_schemas(first: Dict[str, Any], second: Dict[str, Any]) -> Dict[str, Any]:
-    """Helper method to merge two schemas, recursively."""
-    merged_schema = deepcopy(first)
-    for key, value in second.items():
-        # for existing keys, merge dict and list values, leave others unchanged
-        if key in merged_schema.keys():
-            if isinstance(value, dict):
-                # if the key holds a dict, merge the values (e.g. 'properties')
-                merged_schema[key].update(value)
-            elif isinstance(value, list):
-                # if the key holds a list, extend the values (e.g. 'required')
-                merged_schema[key].extend(value)
-            else:
-                logger.warning(
-                    f"key '{key}' with value '{merged_schema[key]}' not "
-                    f"updated to '{value}'"
-                )
-        else:
-            merged_schema[key] = value
-    return merged_schema
-
-
-class ResourceRelation(ABC):  # pylint: disable=too-few-public-methods
-    """ABC for all resource relations or restrictions within the API."""
-
-    property_name: str
-    error_code: int
-
-
-@dataclass
-class PathPropertiesConstraint(ResourceRelation):
-    """The resolved path for the endpoint."""
-
-    path: str
-    property_name: str = "id"
-    error_code: int = 404
-
-
-@dataclass
-class PropertyValueConstraint(ResourceRelation):
-    """The allowed values for property_name."""
-
-    property_name: str
-    values: List[Any]
-    invalid_value: Any = NOT_SET
-    invalid_value_error_code: int = 422
-    error_code: int = 422
-
-
-@dataclass
-class IdDependency(ResourceRelation):
-    """The path where a valid id for the property_name can be gotten (using GET)."""
-
-    property_name: str
-    get_path: str
-    operation_id: Optional[str] = None
-    error_code: int = 422
-
-
-@dataclass
-class IdReference(ResourceRelation):
-    """The path where a resource that needs this resource's id can be created (using POST)."""
-
-    property_name: str
-    post_path: str
-    error_code: int = 422
-
-
-@dataclass
-class UniquePropertyValueConstraint(ResourceRelation):
-    """The value of the property must be unique within the resource scope."""
-
-    property_name: str
-    value: Any
-    error_code: int = 422
-
-
-Relation = Union[
-    IdDependency,
-    IdReference,
-    PathPropertiesConstraint,
-    PropertyValueConstraint,
-    UniquePropertyValueConstraint,
-]
-
-
-@dataclass
-class Dto(ABC):
-    """Base class for the Dto class."""
-
-    @staticmethod
-    def get_parameter_relations() -> List[Relation]:
-        """Return the list of Relations for the header and query parameters."""
-        return []
-
-    def get_parameter_relations_for_error_code(self, error_code: int) -> List[Relation]:
-        """Return the list of Relations associated with the given error_code."""
-        relations: List[Relation] = [
-            r
-            for r in self.get_parameter_relations()
-            if r.error_code == error_code
-            or (
-                getattr(r, "invalid_value_error_code", None) == error_code
-                and getattr(r, "invalid_value", None) != NOT_SET
-            )
-        ]
-        return relations
-
-    @staticmethod
-    def get_relations() -> List[Relation]:
-        """Return the list of Relations for the (json) body."""
-        return []
-
-    def get_relations_for_error_code(self, error_code: int) -> List[Relation]:
-        """Return the list of Relations associated with the given error_code."""
-        relations: List[Relation] = [
-            r
-            for r in self.get_relations()
-            if r.error_code == error_code
-            or (
-                getattr(r, "invalid_value_error_code", None) == error_code
-                and getattr(r, "invalid_value", None) != NOT_SET
-            )
-        ]
-        return relations
-
-    def get_invalidated_data(
-        self,
-        schema: Dict[str, Any],
-        status_code: int,
-        invalid_property_default_code: int,
-    ) -> Dict[str, Any]:
-        """Return a data set with one of the properties set to an invalid value or type."""
-        properties: Dict[str, Any] = self.as_dict()
-
-        schema = resolve_schema(schema)
-
-        relations = self.get_relations_for_error_code(error_code=status_code)
-        # filter PathProperyConstraints since in that case no data can be invalidated
-        relations = [
-            r for r in relations if not isinstance(r, PathPropertiesConstraint)
-        ]
-        property_names = [r.property_name for r in relations]
-        if status_code == invalid_property_default_code:
-            # add all properties defined in the schema, including optional properties
-            property_names.extend((schema["properties"].keys()))
-            # remove duplicates
-            property_names = list(set(property_names))
-        if not property_names:
-            raise ValueError(
-                f"No property can be invalidated to cause status_code {status_code}"
-            )
-        # shuffle the property_names so different properties on the Dto are invalidated
-        # when rerunning the test
-        shuffle(property_names)
-        for property_name in property_names:
-            # if possible, invalidate a constraint but send otherwise valid data
-            id_dependencies = [
-                r
-                for r in relations
-                if isinstance(r, IdDependency) and r.property_name == property_name
-            ]
-            if id_dependencies:
-                invalid_value = uuid4().hex
-                logger.debug(
-                    f"Breaking IdDependency for status_code {status_code}: replacing "
-                    f"{properties[property_name]} with {invalid_value}"
-                )
-                properties[property_name] = invalid_value
-                return properties
-
-            invalid_value_from_constraint = [
-                r.invalid_value
-                for r in relations
-                if isinstance(r, PropertyValueConstraint)
-                and r.property_name == property_name
-                and r.invalid_value_error_code == status_code
-            ]
-            if (
-                invalid_value_from_constraint
-                and invalid_value_from_constraint[0] is not NOT_SET
-            ):
-                properties[property_name] = invalid_value_from_constraint[0]
-                logger.debug(
-                    f"Using invalid_value {invalid_value_from_constraint[0]} to "
-                    f"invalidate property {property_name}"
-                )
-                return properties
-
-            value_schema = schema["properties"][property_name]
-            value_schema = resolve_schema(value_schema)
-
-            # Filter "type": "null" from the possible types since this indicates an
-            # optional / nullable property that can only be invalidated by sending
-            # invalid data of a non-null type
-            if value_schemas := value_schema.get("types"):
-                if len(value_schemas) > 1:
-                    value_schemas = [
-                        schema for schema in value_schemas if schema["type"] != "null"
-                    ]
-                value_schema = choice(value_schemas)
-
-            # there may not be a current_value when invalidating an optional property
-            current_value = properties.get(property_name, SENTINEL)
-            if current_value is SENTINEL:
-                # the current_value isn't very relevant as long as the type is correct
-                # so no logic to handle Relations / objects / arrays here
-                property_type = value_schema["type"]
-                if property_type == "object":
-                    current_value = {}
-                elif property_type == "array":
-                    current_value = []
-                else:
-                    current_value = value_utils.get_valid_value(value_schema)
-
-            values_from_constraint = [
-                r.values[0]
-                for r in relations
-                if isinstance(r, PropertyValueConstraint)
-                and r.property_name == property_name
-            ]
-
-            invalid_value = value_utils.get_invalid_value(
-                value_schema=value_schema,
-                current_value=current_value,
-                values_from_constraint=values_from_constraint,
-            )
-            properties[property_name] = invalid_value
-            logger.debug(
-                f"Property {property_name} changed to {invalid_value} (received from "
-                f"get_invalid_value)"
-            )
-            return properties
-        logger.warning("get_invalidated_data returned unchanged properties")
-        return properties  # pragma: no cover
-
-    def as_dict(self) -> Dict[Any, Any]:
-        """Return the dict representation of the Dto."""
-        result = {}
-
-        for field in fields(self):
-            field_name = field.name
-            if field_name not in self.__dict__:
-                continue
-            original_name = field.metadata["original_property_name"]
-            result[original_name] = getattr(self, field_name)
-
-        return result
+"""
+Module holding the (base) classes that can be used by the user of the OpenApiLibCore
+to implement custom mappings for dependencies between resources in the API under
+test and constraints / restrictions on properties of the resources.
+"""
+
+from abc import ABC
+from copy import deepcopy
+from dataclasses import dataclass, fields
+from logging import getLogger
+from random import choice, shuffle
+from typing import Any, Dict, List, Optional, Union
+from uuid import uuid4
+
+from OpenApiLibCore import value_utils
+
+logger = getLogger(__name__)
+
+NOT_SET = object()
+SENTINEL = object()
+
+
+def resolve_schema(schema: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Helper function to resolve allOf, anyOf and oneOf instances in a schema.
+
+    The schemas are used to generate values for headers, query parameters and json
+    bodies to be able to make requests.
+    """
+    # Schema is mutable, so deepcopy to prevent mutation of original schema argument
+    resolved_schema = deepcopy(schema)
+
+    # allOf / anyOf / oneOf may be nested, so recursively resolve the dict-typed values
+    for key, value in resolved_schema.items():
+        if isinstance(value, dict):
+            resolved_schema[key] = resolve_schema(value)
+
+    # When handling allOf there should no duplicate keys, so the schema parts can
+    # just be merged after resolving the individual parts
+    if schema_parts := resolved_schema.pop("allOf", None):
+        for schema_part in schema_parts:
+            resolved_part = resolve_schema(schema_part)
+            resolved_schema = merge_schemas(resolved_schema, resolved_part)
+    # Handling anyOf and oneOf requires extra logic to deal with the "type" information.
+    # Some properties / parameters may be of different types and each type may have its
+    # own restrictions e.g. a parameter that accepts an enum value (string) or an
+    # integer value within a certain range.
+    # Since the library needs all this information for different purposes, the
+    # schema_parts cannot be merged, so a helper property / key "types" is introduced.
+    any_of = resolved_schema.pop("anyOf", [])
+    one_of = resolved_schema.pop("oneOf", [])
+    schema_parts = any_of if any_of else one_of
+
+    for schema_part in schema_parts:
+        resolved_part = resolve_schema(schema_part)
+        if isinstance(resolved_part, dict) and "type" in resolved_part.keys():
+            if "types" in resolved_schema.keys():
+                resolved_schema["types"].append(resolved_part)
+            else:
+                resolved_schema["types"] = [resolved_part]
+        else:
+            resolved_schema = merge_schemas(resolved_schema, resolved_part)
+
+    return resolved_schema
+
+
+def merge_schemas(first: Dict[str, Any], second: Dict[str, Any]) -> Dict[str, Any]:
+    """Helper method to merge two schemas, recursively."""
+    merged_schema = deepcopy(first)
+    for key, value in second.items():
+        # for existing keys, merge dict and list values, leave others unchanged
+        if key in merged_schema.keys():
+            if isinstance(value, dict):
+                # if the key holds a dict, merge the values (e.g. 'properties')
+                merged_schema[key].update(value)
+            elif isinstance(value, list):
+                # if the key holds a list, extend the values (e.g. 'required')
+                merged_schema[key].extend(value)
+            else:
+                logger.debug(
+                    f"key '{key}' with value '{merged_schema[key]}' not "
+                    f"updated to '{value}'"
+                )
+        else:
+            merged_schema[key] = value
+    return merged_schema
+
+
+class ResourceRelation(ABC):  # pylint: disable=too-few-public-methods
+    """ABC for all resource relations or restrictions within the API."""
+
+    property_name: str
+    error_code: int
+
+
+@dataclass
+class PathPropertiesConstraint(ResourceRelation):
+    """The resolved path for the endpoint."""
+
+    path: str
+    property_name: str = "id"
+    error_code: int = 404
+
+
+@dataclass
+class PropertyValueConstraint(ResourceRelation):
+    """The allowed values for property_name."""
+
+    property_name: str
+    values: List[Any]
+    invalid_value: Any = NOT_SET
+    invalid_value_error_code: int = 422
+    error_code: int = 422
+
+
+@dataclass
+class IdDependency(ResourceRelation):
+    """The path where a valid id for the property_name can be gotten (using GET)."""
+
+    property_name: str
+    get_path: str
+    operation_id: Optional[str] = None
+    error_code: int = 422
+
+
+@dataclass
+class IdReference(ResourceRelation):
+    """The path where a resource that needs this resource's id can be created (using POST)."""
+
+    property_name: str
+    post_path: str
+    error_code: int = 422
+
+
+@dataclass
+class UniquePropertyValueConstraint(ResourceRelation):
+    """The value of the property must be unique within the resource scope."""
+
+    property_name: str
+    value: Any
+    error_code: int = 422
+
+
+Relation = Union[
+    IdDependency,
+    IdReference,
+    PathPropertiesConstraint,
+    PropertyValueConstraint,
+    UniquePropertyValueConstraint,
+]
+
+
+@dataclass
+class Dto(ABC):
+    """Base class for the Dto class."""
+
+    @staticmethod
+    def get_parameter_relations() -> List[Relation]:
+        """Return the list of Relations for the header and query parameters."""
+        return []
+
+    def get_parameter_relations_for_error_code(self, error_code: int) -> List[Relation]:
+        """Return the list of Relations associated with the given error_code."""
+        relations: List[Relation] = [
+            r
+            for r in self.get_parameter_relations()
+            if r.error_code == error_code
+            or (
+                getattr(r, "invalid_value_error_code", None) == error_code
+                and getattr(r, "invalid_value", None) != NOT_SET
+            )
+        ]
+        return relations
+
+    @staticmethod
+    def get_relations() -> List[Relation]:
+        """Return the list of Relations for the (json) body."""
+        return []
+
+    def get_relations_for_error_code(self, error_code: int) -> List[Relation]:
+        """Return the list of Relations associated with the given error_code."""
+        relations: List[Relation] = [
+            r
+            for r in self.get_relations()
+            if r.error_code == error_code
+            or (
+                getattr(r, "invalid_value_error_code", None) == error_code
+                and getattr(r, "invalid_value", None) != NOT_SET
+            )
+        ]
+        return relations
+
+    def get_invalidated_data(
+        self,
+        schema: Dict[str, Any],
+        status_code: int,
+        invalid_property_default_code: int,
+    ) -> Dict[str, Any]:
+        """Return a data set with one of the properties set to an invalid value or type."""
+        properties: Dict[str, Any] = self.as_dict()
+
+        schema = resolve_schema(schema)
+
+        relations = self.get_relations_for_error_code(error_code=status_code)
+        # filter PathProperyConstraints since in that case no data can be invalidated
+        relations = [
+            r for r in relations if not isinstance(r, PathPropertiesConstraint)
+        ]
+        property_names = [r.property_name for r in relations]
+        if status_code == invalid_property_default_code:
+            # add all properties defined in the schema, including optional properties
+            property_names.extend((schema["properties"].keys()))
+            # remove duplicates
+            property_names = list(set(property_names))
+        if not property_names:
+            raise ValueError(
+                f"No property can be invalidated to cause status_code {status_code}"
+            )
+        # shuffle the property_names so different properties on the Dto are invalidated
+        # when rerunning the test
+        shuffle(property_names)
+        for property_name in property_names:
+            # if possible, invalidate a constraint but send otherwise valid data
+            id_dependencies = [
+                r
+                for r in relations
+                if isinstance(r, IdDependency) and r.property_name == property_name
+            ]
+            if id_dependencies:
+                invalid_value = uuid4().hex
+                logger.debug(
+                    f"Breaking IdDependency for status_code {status_code}: replacing "
+                    f"{properties[property_name]} with {invalid_value}"
+                )
+                properties[property_name] = invalid_value
+                return properties
+
+            invalid_value_from_constraint = [
+                r.invalid_value
+                for r in relations
+                if isinstance(r, PropertyValueConstraint)
+                and r.property_name == property_name
+                and r.invalid_value_error_code == status_code
+            ]
+            if (
+                invalid_value_from_constraint
+                and invalid_value_from_constraint[0] is not NOT_SET
+            ):
+                properties[property_name] = invalid_value_from_constraint[0]
+                logger.debug(
+                    f"Using invalid_value {invalid_value_from_constraint[0]} to "
+                    f"invalidate property {property_name}"
+                )
+                return properties
+
+            value_schema = schema["properties"][property_name]
+            value_schema = resolve_schema(value_schema)
+
+            # Filter "type": "null" from the possible types since this indicates an
+            # optional / nullable property that can only be invalidated by sending
+            # invalid data of a non-null type
+            if value_schemas := value_schema.get("types"):
+                if len(value_schemas) > 1:
+                    value_schemas = [
+                        schema for schema in value_schemas if schema["type"] != "null"
+                    ]
+                value_schema = choice(value_schemas)
+
+            # there may not be a current_value when invalidating an optional property
+            current_value = properties.get(property_name, SENTINEL)
+            if current_value is SENTINEL:
+                # the current_value isn't very relevant as long as the type is correct
+                # so no logic to handle Relations / objects / arrays here
+                property_type = value_schema["type"]
+                if property_type == "object":
+                    current_value = {}
+                elif property_type == "array":
+                    current_value = []
+                else:
+                    current_value = value_utils.get_valid_value(value_schema)
+
+            values_from_constraint = [
+                r.values[0]
+                for r in relations
+                if isinstance(r, PropertyValueConstraint)
+                and r.property_name == property_name
+            ]
+
+            invalid_value = value_utils.get_invalid_value(
+                value_schema=value_schema,
+                current_value=current_value,
+                values_from_constraint=values_from_constraint,
+            )
+            properties[property_name] = invalid_value
+            logger.debug(
+                f"Property {property_name} changed to {invalid_value} (received from "
+                f"get_invalid_value)"
+            )
+            return properties
+        logger.warning("get_invalidated_data returned unchanged properties")
+        return properties  # pragma: no cover
+
+    def as_dict(self) -> Dict[Any, Any]:
+        """Return the dict representation of the Dto."""
+        result = {}
+
+        for field in fields(self):
+            field_name = field.name
+            if field_name not in self.__dict__:
+                continue
+            original_name = field.metadata["original_property_name"]
+            result[original_name] = getattr(self, field_name)
+
+        return result
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 1% similar despite different names*

#### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-05T14:47:48+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="377">
-  <version>0.1.3</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2024-04-12T13:08:13+00:00" specversion="5" source="/workspaces/robotframework-openapitools/src/OpenApiLibCore/openapi_libcore.py" lineno="404">
+  <version>0.2.0</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
-    <init name="__init__" lineno="385">
+    <init name="__init__" lineno="412">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
@@ -194,15 +194,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1490">
+    <kw name="Authorized Request" lineno="1535">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -288,39 +288,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1394">
+    <kw name="Ensure In Use" lineno="1439">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type name="IdReference">IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="783">
+    <kw name="Get Ids From Url" lineno="810">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1171">
+    <kw name="Get Invalid Json Data" lineno="1216">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -335,40 +335,40 @@
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1219">
+    <kw name="Get Invalidated Parameters" lineno="1264">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type name="RequestData">RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1137">
+    <kw name="Get Invalidated Url" lineno="1182">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="1031">
+    <kw name="Get Json Data For Dto Class" lineno="1058">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type name="Dict" typedoc="dictionary">
             Dict[str, Any]
             <type name="str" typedoc="string">str</type>
             <type name="Any" typedoc="Any">Any</type>
@@ -390,15 +390,15 @@
           <type name="str" typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1438">
+    <kw name="Get Json Data With Conflict" lineno="1483">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -412,54 +412,54 @@
           <name>conflict_status_code</name>
           <type name="int" typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1159">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1204">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="823">
+    <kw name="Get Request Data" lineno="850">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="687">
+    <kw name="Get Valid Id For Endpoint" lineno="714">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="647">
+    <kw name="Get Valid Url" lineno="674">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type name="str" typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -467,15 +467,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;This keyword returns a valid url for the given &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; and &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;If the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; contains path parameters the Get Valid Id For Endpoint keyword will be executed to retrieve valid ids for the path parameters.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: if valid ids cannot be retrieved within the scope of the API, the &lt;span class=&quot;name&quot;&gt;PathPropertiesConstraint&lt;/span&gt; Relation can be used. More information can be found &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;</doc>
       <shortdoc>This keyword returns a valid url for the given `endpoint` and `method`.</shortdoc>
     </kw>
-    <kw name="Set Origin" lineno="554">
+    <kw name="Set Origin" lineno="581">
       <arguments repr="origin: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="origin: str">
           <name>origin</name>
           <type name="str" typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Update the &lt;span class=&quot;name&quot;&gt;origin&lt;/span&gt; after the library is imported.&lt;/p&gt;
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 import sys
 from copy import deepcopy
 from dataclasses import Field, dataclass, field, make_dataclass
 from functools import cached_property
 from itertools import zip_longest
 from logging import getLogger
 from pathlib import Path
-from random import choice
+from random import choice, sample
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
 from uuid import uuid4
 
 from openapi_core import Config, OpenAPI, Spec
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
@@ -354,14 +354,41 @@
         required_properties = self.dto_schema.get("required", [])
         required_properties_dict: Dict[str, Any] = {}
         for key, value in (self.dto.as_dict()).items():
             if key in required_properties:
                 required_properties_dict[key] = value
         return required_properties_dict
 
+    def get_minimal_body_dict(self) -> Dict[str, Any]:
+        required_properties_dict = self.get_required_properties_dict()
+
+        min_properties = self.dto_schema.get("minProperties", 0)
+        number_of_optional_properties_to_add = min_properties - len(
+            required_properties_dict
+        )
+
+        if number_of_optional_properties_to_add < 1:
+            return required_properties_dict
+
+        optional_properties_dict = {
+            k: v
+            for k, v in self.dto.as_dict().items()
+            if k not in required_properties_dict
+        }
+        optional_properties_to_keep = sample(
+            sorted(optional_properties_dict), number_of_optional_properties_to_add
+        )
+        optional_properties_dict = {
+            k: v
+            for k, v in optional_properties_dict.items()
+            if k in optional_properties_to_keep
+        }
+
+        return {**required_properties_dict, **optional_properties_dict}
+
     def get_required_params(self) -> Dict[str, str]:
         """Get the params dict containing only the required query parameters."""
         required_parameters = [
             p.get("name") for p in self.parameters if p.get("required")
         ]
         return {k: v for k, v in self.params.items() if k in required_parameters}
 
@@ -1079,15 +1106,35 @@
                 endpoint=id_get_path, method="get"
             )
             logger.debug(f"get_dependent_id for {id_get_path} returned {valid_id}")
             return valid_id
 
         json_data: Dict[str, Any] = {}
 
+        property_names = []
         for property_name in schema.get("properties", []):
+            if constrained_values := get_constrained_values(property_name):
+                # do not add properties that are configured to be ignored
+                if IGNORE in constrained_values:
+                    continue
+            property_names.append(property_name)
+
+        max_properties = schema.get("maxProperties")
+        if max_properties and len(property_names) > max_properties:
+            required_properties = schema.get("required", [])
+            number_of_optional_properties = max_properties - len(required_properties)
+            optional_properties = [
+                name for name in property_names if name not in required_properties
+            ]
+            selected_optional_properties = sample(
+                optional_properties, number_of_optional_properties
+            )
+            property_names = required_properties + selected_optional_properties
+
+        for property_name in property_names:
             properties_schema = schema["properties"][property_name]
 
             property_type = properties_schema.get("type")
             if property_type is None:
                 property_types = properties_schema.get("types")
                 if property_types is None:
                     if properties_schema.get("properties") is not None:
@@ -1098,17 +1145,14 @@
                         json_data[property_name] = nested_data
                         continue
                 selected_type_schema = choice(property_types)
                 property_type = selected_type_schema["type"]
             if properties_schema.get("readOnly", False):
                 continue
             if constrained_values := get_constrained_values(property_name):
-                # do not add properties that are configured to be ignored
-                if IGNORE in constrained_values:
-                    continue
                 json_data[property_name] = choice(constrained_values)
                 continue
             if (
                 dependent_id := get_dependent_id(
                     property_name=property_name, operation_id=operation_id
                 )
             ) is not None:
@@ -1127,14 +1171,15 @@
                     schema=properties_schema["items"],
                     dto_class=DefaultDto,
                     operation_id=operation_id,
                 )
                 json_data[property_name] = [array_data]
                 continue
             json_data[property_name] = value_utils.get_valid_value(properties_schema)
+
         return json_data
 
     @keyword
     def get_invalidated_url(self, valid_url: str) -> Optional[str]:
         """
         Return an url with all the path parameters in the `valid_url` replaced by a
         random UUID.
```

### Comparing `robotframework_openapitools-0.1.3/src/OpenApiLibCore/value_utils.py` & `robotframework_openapitools-0.2.0/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/auth.py` & `robotframework_openapitools-0.2.0/src/roboswag/auth.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/cli.py` & `robotframework_openapitools-0.2.0/src/roboswag/cli.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/core.py` & `robotframework_openapitools-0.2.0/src/roboswag/core.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/generate.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/generate.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/api.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/api.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/definition.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/definition.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/endpoint.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/parameter.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/parameter.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/tag.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/tag.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/models/utils.py` & `robotframework_openapitools-0.2.0/src/roboswag/generate/models/utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/templates/api_init.jinja` & `robotframework_openapitools-0.2.0/src/roboswag/generate/templates/api_init.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/generate/templates/paths.jinja` & `robotframework_openapitools-0.2.0/src/roboswag/generate/templates/paths.jinja`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/logger.py` & `robotframework_openapitools-0.2.0/src/roboswag/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/validate/schema.py` & `robotframework_openapitools-0.2.0/src/roboswag/validate/schema.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/src/roboswag/validate/text_response.py` & `robotframework_openapitools-0.2.0/src/roboswag/validate/text_response.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapitools-0.1.3/PKG-INFO` & `robotframework_openapitools-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapitools
-Version: 0.1.3
+Version: 0.2.0
 Summary: A set of Robot Framework libraries to test APIs for which the OAS is available.
 Home-page: https://github.com/MarketSquare/robotframework-openapitools
 License: Apache-2.0
 Author: Bartlomiej Hirsz
 Author-email: bartek.hirsz@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

