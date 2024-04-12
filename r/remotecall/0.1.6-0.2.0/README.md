# Comparing `tmp/remotecall-0.1.6.tar.gz` & `tmp/remotecall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotecall-0.1.6.tar", last modified: Thu Dec 28 12:48:56 2023, max compression
+gzip compressed data, was "remotecall-0.2.0.tar", last modified: Fri Apr 12 08:36:14 2024, max compression
```

## Comparing `remotecall-0.1.6.tar` & `remotecall-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.063790 remotecall-0.1.6/
--rw-r--r--   0 slaine   (1355619077) 1965124760     1481 2023-03-11 14:26:45.000000 remotecall-0.1.6/LICENSE
--rw-r--r--   0 slaine   (1355619077) 1965124760     8112 2023-12-28 12:48:56.063525 remotecall-0.1.6/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760     7640 2023-03-19 20:05:21.000000 remotecall-0.1.6/README.md
--rw-r--r--   0 slaine   (1355619077) 1965124760       38 2023-12-28 12:48:56.063885 remotecall-0.1.6/setup.cfg
--rw-r--r--   0 slaine   (1355619077) 1965124760     1171 2023-12-04 05:14:08.000000 remotecall-0.1.6/setup.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.027988 remotecall-0.1.6/src/
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.053077 remotecall-0.1.6/src/remotecall/
--rw-r--r--   0 slaine   (1355619077) 1965124760     1110 2023-12-04 05:14:08.000000 remotecall-0.1.6/src/remotecall/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3488 2023-12-04 05:14:08.000000 remotecall-0.1.6/src/remotecall/__main__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      218 2023-12-28 12:47:55.000000 remotecall-0.1.6/src/remotecall/_meta.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.058593 remotecall-0.1.6/src/remotecall/authentication/
--rw-r--r--   0 slaine   (1355619077) 1965124760      768 2023-03-17 11:15:02.000000 remotecall-0.1.6/src/remotecall/authentication/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2369 2023-03-19 09:02:03.000000 remotecall-0.1.6/src/remotecall/authentication/authenticator.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3680 2023-12-28 12:47:55.000000 remotecall-0.1.6/src/remotecall/client.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4710 2023-12-04 05:14:08.000000 remotecall-0.1.6/src/remotecall/clientfactory.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     5504 2023-03-11 14:36:05.000000 remotecall-0.1.6/src/remotecall/codecs.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.060705 remotecall-0.1.6/src/remotecall/constants/
--rw-r--r--   0 slaine   (1355619077) 1965124760        0 2023-04-20 11:46:26.000000 remotecall-0.1.6/src/remotecall/constants/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      174 2023-04-20 11:38:21.000000 remotecall-0.1.6/src/remotecall/constants/headers.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      204 2023-03-19 20:17:29.000000 remotecall-0.1.6/src/remotecall/constants/statuscodes.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3555 2023-11-26 12:20:21.000000 remotecall-0.1.6/src/remotecall/endpoint.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      456 2023-03-16 18:22:04.000000 remotecall-0.1.6/src/remotecall/errors.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.062785 remotecall-0.1.6/src/remotecall/extras/
--rw-r--r--   0 slaine   (1355619077) 1965124760        0 2023-08-11 10:04:34.000000 remotecall-0.1.6/src/remotecall/extras/__init__.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     1075 2023-08-11 09:29:37.000000 remotecall-0.1.6/src/remotecall/extras/imagecodec.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     2067 2023-08-11 09:29:37.000000 remotecall-0.1.6/src/remotecall/extras/numpycodec.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      629 2023-03-20 07:34:11.000000 remotecall-0.1.6/src/remotecall/gethandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     6170 2023-03-20 07:48:34.000000 remotecall-0.1.6/src/remotecall/posthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     4734 2023-12-04 05:14:08.000000 remotecall-0.1.6/src/remotecall/requesthandler.py
--rw-r--r--   0 slaine   (1355619077) 1965124760      721 2023-12-04 05:14:08.000000 remotecall-0.1.6/src/remotecall/response.py
--rw-r--r--   0 slaine   (1355619077) 1965124760     3249 2023-05-01 19:13:47.000000 remotecall-0.1.6/src/remotecall/server.py
-drwxr-xr-x   0 slaine   (1355619077) 1965124760        0 2023-12-28 12:48:56.057342 remotecall-0.1.6/src/remotecall.egg-info/
--rw-r--r--   0 slaine   (1355619077) 1965124760     8112 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/PKG-INFO
--rw-r--r--   0 slaine   (1355619077) 1965124760      957 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/SOURCES.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/dependency_links.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       50 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/entry_points.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760        1 2023-02-07 05:13:42.000000 remotecall-0.1.6/src/remotecall.egg-info/not-zip-safe
--rw-r--r--   0 slaine   (1355619077) 1965124760       94 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/requires.txt
--rw-r--r--   0 slaine   (1355619077) 1965124760       11 2023-12-28 12:48:55.000000 remotecall-0.1.6/src/remotecall.egg-info/top_level.txt
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.699923 remotecall-0.2.0/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1481 2023-03-11 14:26:45.000000 remotecall-0.2.0/LICENSE
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     8112 2024-04-12 08:36:14.699618 remotecall-0.2.0/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     7640 2023-03-19 20:05:21.000000 remotecall-0.2.0/README.md
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)       38 2024-04-12 08:36:14.700040 remotecall-0.2.0/setup.cfg
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1171 2023-12-04 05:14:08.000000 remotecall-0.2.0/setup.py
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.657236 remotecall-0.2.0/src/
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.672098 remotecall-0.2.0/src/remotecall/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1110 2024-04-03 13:43:32.000000 remotecall-0.2.0/src/remotecall/__init__.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     3488 2023-12-04 05:14:08.000000 remotecall-0.2.0/src/remotecall/__main__.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)    22261 2024-04-05 06:06:57.000000 remotecall-0.2.0/src/remotecall/_codecs copy 2.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)    21802 2024-04-04 08:57:03.000000 remotecall-0.2.0/src/remotecall/_codecs copy.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      218 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/_meta.py
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.694364 remotecall-0.2.0/src/remotecall/authentication/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      768 2023-03-17 11:15:02.000000 remotecall-0.2.0/src/remotecall/authentication/__init__.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     2369 2023-03-19 09:02:03.000000 remotecall-0.2.0/src/remotecall/authentication/authenticator.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     4272 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/client.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     4761 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/clientfactory.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)    20757 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/codecs.py
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.697171 remotecall-0.2.0/src/remotecall/constants/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2023-04-20 11:46:26.000000 remotecall-0.2.0/src/remotecall/constants/__init__.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      174 2023-04-20 11:38:21.000000 remotecall-0.2.0/src/remotecall/constants/headers.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      204 2023-03-19 20:17:29.000000 remotecall-0.2.0/src/remotecall/constants/statuscodes.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     3871 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/endpoint.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      456 2023-03-16 18:22:04.000000 remotecall-0.2.0/src/remotecall/errors.py
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.699103 remotecall-0.2.0/src/remotecall/extras/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2023-08-11 10:04:34.000000 remotecall-0.2.0/src/remotecall/extras/__init__.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1069 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/extras/imagecodec.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1801 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/extras/numpycodec.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     2395 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/gethandler.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     6894 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/posthandler.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     4855 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/requesthandler.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      721 2023-12-04 05:14:08.000000 remotecall-0.2.0/src/remotecall/response.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     3690 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/server.py
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)      416 2024-04-12 06:49:07.000000 remotecall-0.2.0/src/remotecall/utils.py
+drwxr-xr-x   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        0 2024-04-12 08:36:14.692337 remotecall-0.2.0/src/remotecall.egg-info/
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     8112 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/PKG-INFO
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)     1045 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/SOURCES.txt
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        1 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/dependency_links.txt
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)       50 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/entry_points.txt
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)        1 2023-02-07 05:13:42.000000 remotecall-0.2.0/src/remotecall.egg-info/not-zip-safe
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)       94 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/requires.txt
+-rw-r--r--   0 slaine   (1355619077) OPTOFIDELITY\Domain Users (1965124760)       11 2024-04-12 08:36:14.000000 remotecall-0.2.0/src/remotecall.egg-info/top_level.txt
```

### Comparing `remotecall-0.1.6/LICENSE` & `remotecall-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/PKG-INFO` & `remotecall-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecall
-Version: 0.1.6
+Version: 0.2.0
 Summary: The module provides functionality to expose Python functions to be called remotely over ethernet.
 Home-page: https://gitlab.com/slaine/remotecall.git/
 Author: Sami Laine
 Author-email: sami.jy.laine@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `remotecall-0.1.6/README.md` & `remotecall-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/setup.py` & `remotecall-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/__init__.py` & `remotecall-0.2.0/src/remotecall/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/__main__.py` & `remotecall-0.2.0/src/remotecall/__main__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/authentication/__init__.py` & `remotecall-0.2.0/src/remotecall/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/authentication/authenticator.py` & `remotecall-0.2.0/src/remotecall/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/client.py` & `remotecall-0.2.0/src/remotecall/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
 from typing import Any
+from typing import Type
+from typing import Optional
 import logging
+
 import requests
 
 from .codecs import Codec
 from .codecs import Codecs
 from .constants import headers
 from .errors import ClientError
 from .errors import ServerError
@@ -42,55 +45,67 @@
         self._cert_file = cert_file
         self._ssl_enabled = True
 
     def set_authentication(self, authentication):
         """Set authentication method."""
         self._authentication = authentication
 
-    def call(self, function_name: str, timeout=None, **kwargs):
+    def call(self, function_name: str, timeout: Optional[float] = None, **kwargs):
         """Call remote function with arguments."""
         logger.debug("Preparing to call %s.", function_name)
         url = self._get_url(function_name)
         multipart_form_data = self._encode_multipart_form_data(fields=kwargs)
 
         logger.debug("Sending POST request %s.", url)
 
         response = self._session.post(
             url=url,
             files=multipart_form_data,
             verify=self._cert_file,
             auth=self._authentication,
-            timeout=timeout
+            timeout=timeout,
         )
 
         logger.debug("Received status code: %s.", response.status_code)
 
         if response.status_code >= 500:
             self._log_response(response)
             raise ServerError(f"Server error: {response.text}", response.status_code)
 
         if response.status_code >= 400:
             self._log_response(response)
             raise ClientError(f"Client error: {response.text}", response.status_code)
 
         return self._get_response_value(response)
 
+    def register_type(self, class_object: Type):
+        """Register a type class.
+
+        Codecs can use registered class objects to encode and decode that type of objects.
+
+        For example, by registering Enum, dataclass or namedtuple makes it possible to use these
+        as arguments or return types.
+        """
+        codec = self._codecs.get_codec_by_type(class_object)
+        codec.register_type(class_object.__name__, class_object)
+
     def _get_url(self, command: str) -> str:
         return f"{self.server_url}/{command}"
 
     def _encode_multipart_form_data(self, fields: dict[str, Any]) -> dict[str, tuple]:
         logger.debug("Encoding multipart/form-data ...")
         form_data = {}
 
         for name, value in fields.items():
             logger.debug("Get codec for '%s.", type(value))
             codec = self._codecs.get_codec_by_value(value)
 
             logger.debug("Encoding '%s' with %s.", name, codec)
-            form_data[name] = (None, codec.encode(value), codec.get_content_type())
+            encoded_value, content_type = codec.encode(value)
+            form_data[name] = (None, encoded_value, content_type)
 
         return form_data
 
     @classmethod
     def _log_response(cls, response: requests.Response):
         logger.debug("Response:")
         logger.debug("  status: %s", response.status_code)
@@ -100,11 +115,9 @@
     def _get_response_value(self, response: requests.Response):
         content_type = response.headers.get(str(headers.CONTENT_TYPE))
 
         if not content_type:
             return response.content
 
         codec = self._codecs.get_codec_by_content_type(content_type)
-
         logger.debug("Using %s to decode '%s' response.", codec, content_type)
-
-        return codec.decode(response.content)
+        return codec.decode(response.content, content_type)
```

### Comparing `remotecall-0.1.6/src/remotecall/clientfactory.py` & `remotecall-0.2.0/src/remotecall/clientfactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,25 @@
-import typing
 from typing import Optional
 from typing import Any
 
-"""
-Example:
-    {
-        "endpoints": [
-            {
-                "name": "foo",
-                "documentation": "Foo.\n\nTest docstring.",
-                "parameters": [
-                    {
-                        "name": "a",
-                        "annotation": "int"
-                    },
-                    {
-                        "name": "b",
-                        "annotation": "str",
-                        "default": "foo"
-                    }
-                ],
-                "return_annotation": "bool"
-            }
-        ],
-        "address": {
-            "hostname": "127.0.0.1",
-            "port": 8000
-        }
-    }
-"""
+
+def return_annotation_to_str(annotation: list[str]) -> str:
+    if not annotation:
+        return " -> None"
+    if len(annotation) == 1:
+        return f" -> {annotation[0]}"
+    return f" -> typing.Union[{', '.join(annotation)}]"
+
+
+def parameter_annotation_to_str(annotation: list[str], optional: bool) -> str:
+    if optional:
+        return f": typing.Optional[{annotation[0]}]"
+    if len(annotation) == 1:
+        return f": {annotation[0]}"
+    return f": typing.Union[{', '.join(annotation)}]"
 
 
 class ClientFactory:
     def __init__(self, definition: dict, class_name: Optional[str] = None):
         self._definition = definition
         self._client_class_name = class_name or "Client"
 
@@ -45,22 +32,20 @@
         c.doc = self._definition.get("documentation", "")
         c.methods.append(self.generate_init_method((host, port)))
 
         endpoints = self._definition.get("endpoints", [])
         for endpoint in endpoints:
             name = endpoint.get("name")
             doc = endpoint.get("documentation")
-            return_annotation = endpoint.get("return_annotation")
+            return_annotation = return_annotation_to_str(endpoint.get("returnAnnotation"))
 
             m = Method(name=name, return_annotation=return_annotation, doc=doc)
             c.methods.append(m)
             for parameter in endpoint.get("parameters", []):
-                p = Parameter(
-                    parameter["name"], parameter["annotation"], parameter.get("default", None)
-                )
+                p = Parameter.from_dict(parameter)
                 m.parameters.append(p)
 
         lines = ["from __future__ import annotations\n"]
         lines.append("import typing")
         lines.append("from typing import Optional\n")
         lines.append("from remotecall import BaseClient\n\n")
         lines.append(str(c))
@@ -72,21 +57,32 @@
         return (
             f"    def __init__(self, server_address={server_address}):\n"
             f"        super().__init__(server_address=server_address)\n"
         )
 
 
 class Parameter:
-    def __init__(self, name: str, annotation: str, default: Any):
+    @classmethod
+    def from_dict(cls, definition: dict):
+        return cls(
+            definition["name"],
+            definition["annotation"],
+            definition.get("default", None),
+            definition["optional"],
+        )
+
+    def __init__(self, name: str, annotation: str, default: Any, optional: bool):
         self.name = name
         self.annotation = annotation
         self.default = default
+        self.optional = optional
 
     def __str__(self):
-        lines = [f"{self.name}: {self.annotation}"]
+        lines = [self.name]
+        lines.append(parameter_annotation_to_str(self.annotation, self.optional))
 
         if self.default is not None:
             lines.append(f" = {self.default}")
 
         return "".join(lines)
 
 
@@ -103,17 +99,15 @@
 
         # Signature
         for parameter in self.parameters:
             lines.append(f", {parameter}")
         lines.append(")")
 
         # Return type
-        if self.return_annotation:
-            lines.append(f" -> {self.return_annotation}")
-
+        lines.append(self.return_annotation)
         lines.append(":\n")
 
         # Docstring
         if self.doc:
             lines.append(self.indent * 2)
             lines.append(f'"""{self.doc}\n')
             lines.append(self.indent * 2)
```

### Comparing `remotecall-0.1.6/src/remotecall/extras/imagecodec.py` & `remotecall-0.2.0/src/remotecall/extras/imagecodec.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,35 +6,32 @@
 import typing
 import io
 import base64
 
 from PIL import Image
 
 from remotecall import Codec
+from remotecall.codecs import T
 
 
-class ImageCodec(Codec):
+class ImageCodec(Codec[T]):
     IMAGE_FORMAT = "png"
 
     @classmethod
     def is_matching_content_type(cls, content_type: str) -> bool:
         return content_type.startswith("application/image")
 
     @classmethod
     def is_matching_type(cls, type_: typing.Type) -> bool:
-        return issubclass(type_, cls.get_type())
-
-    @classmethod
-    def get_type(cls) -> typing.Type:
-        return Image.Image
+        return issubclass(type_, Image.Image)
 
     def get_content_type(self) -> str:
         return f"application/image-{self.IMAGE_FORMAT}"
 
-    def encode(self, image: Image) -> bytes:
+    def encode(self, image: T) -> tuple[bytes, str]:
         buffer = io.BytesIO()
         image.save(buffer, format=self.IMAGE_FORMAT)
-        return base64.b64encode(buffer.getvalue())
+        return base64.b64encode(buffer.getvalue()), self.get_content_type()
 
-    def decode(self, data: bytes) -> Image:
+    def decode(self, data: bytes, content_type: str) -> T:
         base64_str = io.BytesIO(base64.b64decode(data))
         return Image.open(base64_str)
```

### Comparing `remotecall-0.1.6/src/remotecall/extras/numpycodec.py` & `remotecall-0.2.0/src/remotecall/extras/numpycodec.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,68 +2,58 @@
 
 Usage:
     from remotecall.extracodecs.imagecodec import NumPyCodec
 """
 from __future__ import annotations
 
 import typing
+from typing import Type
 
 import numpy as np
 from numpy.typing import NDArray, DTypeLike
 
 from remotecall import Codec
+from remotecall.codecs import T
 
 
-class NumPyCodec(Codec):
+class NumPyCodec(Codec[NDArray]):
     """NumPy codec.
 
     Example NumPy codec.
     """
 
     @classmethod
     def is_matching_content_type(cls, content_type: str) -> bool:
         return content_type.startswith("application/numpy")
 
     @classmethod
     def is_matching_type(cls, type_: typing.Type) -> bool:
         return type_ == np.ndarray
 
     @classmethod
-    def create_by_value(cls, array: NDArray) -> NumPyCodec:
-        return cls(shape=array.shape, dtype=array.dtype)
-
-    @classmethod
-    def create_by_content_type(cls, content_type: str) -> NumPyCodec:
-        shape, data_type = cls._get_shape_and_data_type(content_type)
-        return cls(shape=shape, dtype=data_type)
-
-    @classmethod
     def _get_shape_and_data_type(cls, content_type: str) -> tuple[list, DTypeLike]:
         """Extract shape and dtype from content-type.
 
         Content-type string is expected to be like "numpy-uint8-1080x1920x3".
         """
         fields = content_type.split("-")
         return (
             [int(dimension) for dimension in fields[2].split("x")],
             np.dtype(fields[1])
         )
 
-    def __init__(self, shape: list, dtype: DTypeLike):
-        self.shape = shape
-        self.dtype = dtype
+    def get_encode_type(self) -> Type:
+        return NDArray
 
-    @classmethod
-    def get_type(cls) -> typing.Type:
-        return np.ndarray
-
-    def encode(self, array: NDArray) -> bytes:
-        return array.tobytes()
+    def encode(self, array: T) -> tuple[bytes, str]:
+        return array.tobytes(), self._get_content_type(array)
 
-    def decode(self, data: bytes) -> NDArray:
-        return np.ndarray(shape=self.shape, dtype=self.dtype, buffer=data)
+    def decode(self, data: bytes, content_type: str) -> T:
+        shape, data_type = self._get_shape_and_data_type(content_type)
+        return np.ndarray(shape=shape, dtype=data_type, buffer=data)
 
-    def get_content_type(self) -> str:
+    @classmethod
+    def _get_content_type(cls, array: NDArray) -> str:
         # Example output: "numpy-uint8-1080x1920x3"
-        dtype_name = str(self.dtype)
-        shape_name = "x".join(map(str, self.shape))
+        dtype_name = str(array.dtype)
+        shape_name = "x".join(map(str, array.shape))
         return f"application/numpy-{dtype_name}-{shape_name}"
```

### Comparing `remotecall-0.1.6/src/remotecall/posthandler.py` & `remotecall-0.2.0/src/remotecall/posthandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,197 +1,211 @@
-from __future__ import annotations
-
-import cgi
-from dataclasses import dataclass
-import re
-import logging
-import typing
-from typing import BinaryIO
-from typing import Optional
-
-from .response import Response
-from .errors import ClientError
-from .constants import headers
-from .constants.headers import CONTENT_TYPE
-from .constants.headers import CONTENT_DISPOSITION
-from .constants.statuscodes import TYPE_ERROR
-from .constants.statuscodes import BAD_REQUEST
-from .constants.statuscodes import SERVICE_UNAVAILABLE
-
-if typing.TYPE_CHECKING:
-    from .endpoint import Endpoint
-    from .requesthandler import HTTPRequestHandler
-
-
-logger = logging.getLogger(__name__)
-
-
-@dataclass
-class MultiPartFormDataField:
-    name: str
-    content_type: str
-    data: bytes
-
-
-class PostHandler:
-
-    def __init__(self, request: HTTPRequestHandler):
-        self.request = request
-        self._server = self.request.get_server()
-        self._codecs = self._server.codecs
-
-    def handle(self) -> Response:  # pylint: disable=broad-exception-caught
-        endpoint_name = self.request.path_component
-
-        try:
-            endpoint = self._server.endpoints[endpoint_name]
-        except KeyError as err:
-            raise ClientError(f"Unknown endpoint: '{endpoint_name}'", BAD_REQUEST) from err
-
-        if not endpoint.enabled:
-            raise ClientError("Endpoint disabled.", SERVICE_UNAVAILABLE)
-
-        try:
-            arguments = self.get_arguments(endpoint)
-        except ValueError as err:
-            raise ClientError(
-                f"Failed to parse request arguments: {err}", BAD_REQUEST
-            ) from err
-
-        try:
-            return_value = endpoint(**arguments)
-        except TypeError as err:
-            raise ClientError(str(err), TYPE_ERROR) from err
-
-        try:
-            codec = self._codecs.get_codec_by_value(return_value)
-            logger.debug("Using %s to decode return value.", codec)
-            response = Response(codec.encode(return_value), codec.get_content_type())
-        except Exception as err:
-            raise ClientError(
-                f"Failed to encode return value: {err}", TYPE_ERROR
-            ) from err
-
-        return response
-
-    def get_arguments(self, endpoint: Endpoint) -> dict:
-        logger.debug("Get arguments.")
-
-        arguments = {}
-
-        request = self.request
-        content_length = request.content_length
-        content_type_header = request.headers.get(CONTENT_TYPE)
-
-        if not content_type_header:
-            logger.debug("No arguments ('content-type' not set).")
-            return arguments
-
-        request_content_type, options = cgi.parse_header(content_type_header)
-        if request_content_type != headers.MULTIPART_FORM_DATA:
-            raise ClientError(
-                f"Invalid content-type: '{request_content_type}'.", BAD_REQUEST,
-            )
-
-        boundary = options.get(headers.BOUNDARY)
-
-        if not boundary:
-            raise ClientError("Boundary not defined.", BAD_REQUEST)
-
-        fields = self.read_multipart_form_data(request.rfile, content_length, boundary)
-
-        for field in fields:
-            arguments[field.name] = self.decode_multipart_form_data(field, endpoint)
-
-        return arguments
-
-    def decode_multipart_form_data(self, field: MultiPartFormDataField, endpoint: Endpoint):
-        try:
-            parameter = endpoint.get_parameter(field.name)
-        except KeyError as err:
-            raise ClientError(
-                f"{endpoint.name}() got unexpected parameter: {field.name}", BAD_REQUEST
-            ) from err
-
-        if field.content_type:
-            codec = self._codecs.get_codec_by_content_type(field.content_type)
-        else:
-            codec = self._codecs.get_codec_by_type(parameter.annotation or str)
-
-        logger.debug("Using %s to decode '%s'.", codec, field.name)
-
-        return codec.decode(field.data)
-
-    @classmethod
-    def read_multipart_form_data(
-        cls, rfile: BinaryIO, length: int, boundary: str
-    ) -> list[MultiPartFormDataField]:
-        """
-        Example:
-            b'--40c00dbb9994e1de1cf94bce01c4e734'
-            b'Content-Disposition: form-data; name="text"'
-            b'Content-Type: application/str'
-            b''
-            b'Hello world'
-            b'--40c00dbb9994e1de1cf94bce01c4e734--'
-            b''
-        """
-
-        def read_lines(rfile: BinaryIO, length: int) -> list[bytes]:
-            bytes_count = 0
-
-            for line in rfile:
-                yield line
-
-                bytes_count += len(line)
-                if bytes_count >= length:
-                    break
-
-        def get_name(text: str) -> Optional[str]:
-            # Example:
-            #   Content-Disposition: form-data; name="a"; filename="a"
-            try:
-                return re.search('name="(.+?)"', text).group(1)
-            except AttributeError:
-                logger.warning("Expecting name field in '%s'.", text)
-                return None
-
-        def get_content_type(text: str) -> str:
-            return text.split(":")[1].strip()
-
-        fields = []
-        name = None
-        content_type = None
-        delimiter = b"--" + boundary.encode()
-        expect_data = False
-        data = []
-
-        for line in read_lines(rfile, length):
-            # logger.debug(line)
-
-            # Note: this will also catch the end delimiter with trailing dashes ('--').
-            if line.startswith(delimiter):
-                if expect_data:
-                    fields.append(
-                        MultiPartFormDataField(name, content_type, b"\r\n".join(data).rstrip())
-                    )
-                    data.clear()
-
-                expect_data = False
-                continue
-
-            if expect_data:
-                data.append(line)
-                continue
-
-            if not line or line == b"\r\n":
-                expect_data = True
-                continue
-
-            text = line.decode().lower()
-
-            if text.startswith(CONTENT_DISPOSITION):
-                name = get_name(text)
-            elif text.startswith(CONTENT_TYPE):
-                content_type = get_content_type(text)
-
-        return fields
+from __future__ import annotations
+
+import cgi
+from dataclasses import dataclass
+import re
+import logging
+import typing
+from typing import BinaryIO
+from typing import Optional
+
+from .response import Response
+from .errors import ClientError
+from .constants import headers
+from .constants.headers import CONTENT_TYPE
+from .constants.headers import CONTENT_DISPOSITION
+from .constants.statuscodes import TYPE_ERROR
+from .constants.statuscodes import BAD_REQUEST
+from .constants.statuscodes import SERVICE_UNAVAILABLE
+
+if typing.TYPE_CHECKING:
+    from .endpoint import Endpoint
+    from .requesthandler import HTTPRequestHandler
+
+
+logger = logging.getLogger(__name__)
+
+
+@dataclass
+class MultiPartFormDataField:
+    name: str
+    content_type: str
+    data: bytes
+
+
+class PostHandler:
+    def __init__(self, request: HTTPRequestHandler):
+        self.request = request
+        self._server = self.request.get_server()
+        self._codecs = self._server.codecs
+
+    def handle(self) -> Response:  # pylint: disable=broad-exception-caught
+        endpoint_name = self.request.path_component
+
+        try:
+            endpoint = self._server.endpoints[endpoint_name]
+        except KeyError as err:
+            raise ClientError(
+                f"Unknown endpoint: '{endpoint_name}'", BAD_REQUEST
+            ) from err
+
+        if not endpoint.enabled:
+            raise ClientError("Endpoint disabled.", SERVICE_UNAVAILABLE)
+
+        try:
+            arguments = self.get_arguments(endpoint)
+        except ValueError as err:
+            raise ClientError(
+                f"Failed to parse request arguments: {err}", BAD_REQUEST
+            ) from err
+
+        try:
+            return_value = endpoint(**arguments)
+        except TypeError as err:
+            raise ClientError(str(err), TYPE_ERROR) from err
+
+        try:
+            codec = self._codecs.get_codec_by_value(return_value)
+            logger.debug("Using %s to decode return value.", codec)
+            data_bytes, content_type = codec.encode(return_value)
+            response = Response(data_bytes, content_type)
+        except Exception as err:
+            raise ClientError(
+                f"Failed to encode return value: {err}", TYPE_ERROR
+            ) from err
+
+        return response
+
+    def get_arguments(self, endpoint: Endpoint) -> dict:
+        logger.debug("Get arguments.")
+
+        arguments = {}
+
+        request = self.request
+        content_length = request.content_length
+        content_type_header = request.headers.get(CONTENT_TYPE)
+
+        if not content_type_header:
+            logger.debug("No arguments ('content-type' not set).")
+            return arguments
+
+        request_content_type, options = cgi.parse_header(content_type_header)
+        if request_content_type != headers.MULTIPART_FORM_DATA:
+            raise ClientError(
+                f"Invalid content-type: '{request_content_type}'.",
+                BAD_REQUEST,
+            )
+
+        boundary = options.get(headers.BOUNDARY)
+
+        if not boundary:
+            raise ClientError("Boundary not defined.", BAD_REQUEST)
+
+        fields = self.read_multipart_form_data(request.rfile, content_length, boundary)
+
+        for field in fields:
+            arguments[field.name] = self.decode_multipart_form_data(field, endpoint)
+
+        return arguments
+
+    def decode_multipart_form_data(
+        self, field: MultiPartFormDataField, endpoint: Endpoint
+    ):
+        field_name = field.name
+        logger.debug("Decoding multipart/form-data '%s'." % field_name)
+
+        try:
+            parameter = endpoint.parameters[field_name]
+        except KeyError as err:
+            raise ClientError(
+                f"{endpoint.name}() got unexpected parameter: {field_name}", BAD_REQUEST
+            ) from err
+
+        content_type = field.content_type
+
+        if not content_type:
+            raise RuntimeError(
+                f"Multipart/form-data field '{field_name}' is missing 'content-type'. Content-type "
+                "is needed to select the correct codec to decode the field data."
+            )
+
+        logger.debug("Content-type of '%s' field: '%s'.", field_name, content_type)
+        codec = parameter.get_codec_by_content_type(content_type)
+        logger.debug("Using %s to decode '%s'.", codec, field_name)
+        return codec.decode(field.data, content_type)
+
+    @classmethod
+    def read_multipart_form_data(
+        cls, rfile: BinaryIO, length: int, boundary: str
+    ) -> list[MultiPartFormDataField]:
+        """
+        Example:
+            b'--40c00dbb9994e1de1cf94bce01c4e734'
+            b'Content-Disposition: form-data; name="text"'
+            b'Content-Type: application/str'
+            b''
+            b'Hello world'
+            b'--40c00dbb9994e1de1cf94bce01c4e734--'
+            b''
+        """
+
+        def read_lines(rfile: BinaryIO, length: int) -> list[bytes]:
+            bytes_count = 0
+
+            for line in rfile:
+                yield line
+
+                bytes_count += len(line)
+                if bytes_count >= length:
+                    break
+
+        def get_name(text: str) -> Optional[str]:
+            # Example:
+            #   Content-Disposition: form-data; name="a"; filename="a"
+            try:
+                return re.search('name="(.+?)"', text).group(1)
+            except AttributeError:
+                logger.warning("Expecting name field in '%s'.", text)
+                return None
+
+        def get_content_type(text: str) -> str:
+            return text.split(":")[1].strip()
+
+        fields = []
+        name = None
+        content_type = None
+        delimiter = b"--" + boundary.encode()
+        expect_data = False
+        data = []
+
+        for line in read_lines(rfile, length):
+            # logger.debug(line)
+
+            # Note: this will also catch the end delimiter with trailing dashes ('--').
+            if line.startswith(delimiter):
+                if expect_data:
+                    fields.append(
+                        MultiPartFormDataField(
+                            name, content_type, b"\r\n".join(data).rstrip()
+                        )
+                    )
+                    data.clear()
+
+                expect_data = False
+                continue
+
+            if expect_data:
+                data.append(line)
+                continue
+
+            if not line or line == b"\r\n":
+                expect_data = True
+                continue
+
+            text = line.decode().lower()
+
+            if text.startswith(CONTENT_DISPOSITION):
+                name = get_name(text)
+            elif text.startswith(CONTENT_TYPE):
+                content_type = get_content_type(text)
+
+        return fields
```

### Comparing `remotecall-0.1.6/src/remotecall/requesthandler.py` & `remotecall-0.2.0/src/remotecall/requesthandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def get_server(self) -> Server:
         return self.server  # self.server is referring to http.server.BaseServer.
 
     def do_HEAD(self):  # pylint: disable=invalid-name
         logger.debug("Received HEAD request '%s'", self.path_component)
         self.send_response(200)
-        self.send_header('Content-type', 'application/json; charset=utf-8')
+        self.send_header("Content-type", "application/json; charset=utf-8")
         self.end_headers()
         logger.debug("Finished HEAD request '%s'", self.path_component)
 
     def do_GET(self):  # pylint: disable=invalid-name
         logger.debug("Received GET request '%s'", self.path_component)
         self._handle_get()
         logger.debug("Finished GET request '%s'", self.path_component)
@@ -71,38 +71,43 @@
     @authenticate
     def _handle_post(self):
         try:
             handler = PostHandler(self)
             response = handler.handle()
         except ClientError as err:
             logger.exception(err)
-            response = self._create_error_response(message=err.message, status_code=err.status_code)
+            response = self._create_error_response(
+                message=err.message, status_code=err.status_code
+            )
         except Exception as err:  # pylint: disable=broad-exception-caught
             logger.exception(err)
 
             # Handler is expected to identify expectable errors. This try-catch block catches
             # unexpected server errors that could not be identified.
-            response = self._create_error_response(message=str(err), status_code=SERVER_ERROR)
+            response = self._create_error_response(
+                message=str(err), status_code=SERVER_ERROR
+            )
 
         self._send_response(response)
 
     @authenticate
     def _handle_get(self):
         try:
             handler = GetHandler(self)
             response = handler.handle()
         except Exception as err:  # pylint: disable=broad-exception-caught
             logger.exception(err)
-            response = self._create_error_response(message=str(err), status_code=SERVER_ERROR)
+            response = self._create_error_response(
+                message=str(err), status_code=SERVER_ERROR
+            )
 
         self._send_response(response)
 
     def _send_response(self, response: Response):
-        """Send response.
-        """
+        """Send response."""
         logger.debug("Sending response..")
         bytes_to_send = b"" if response.value is None else response.value
 
         try:
             self.send_response(response.status_code)
 
             if response.content_type:
@@ -118,14 +123,15 @@
 
     def _create_error_response(self, message: str, status_code: int) -> Response:
         logger.error(message)
         logger.debug(str(self))
 
         server = self.get_server()
         codec = server.codecs.get_codec_by_value(message)
-        return Response(codec.encode(message), codec.get_content_type(), status_code=status_code)
+        data_bytes, content_type = codec.encode(message)
+        return Response(data_bytes, content_type, status_code=status_code)
 
     def __str__(self):
         info = []
         info.append(f"{self.path}")
         info.append(f"{str(self.headers).strip()}")
         return "\n".join(info)
```

### Comparing `remotecall-0.1.6/src/remotecall/response.py` & `remotecall-0.2.0/src/remotecall/response.py`

 * *Files identical despite different names*

### Comparing `remotecall-0.1.6/src/remotecall/server.py` & `remotecall-0.2.0/src/remotecall/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import http.server
 import logging
 import typing
 from typing import Optional
+import inspect
 from .endpoint import Endpoint
 from .requesthandler import HTTPRequestHandler
 from .codecs import Codec
 from .codecs import Codecs
 from .authentication import Authenticator
 
 
@@ -30,40 +31,52 @@
     def url(self) -> str:
         """Server URL."""
         hostname, port = self.server_address
         scheme = "https" if self.ssl_enabled else "http"
         return f"{scheme}://{hostname}:{port}"
 
     @classmethod
-    def _create_endpoint(cls, function: typing.Callable, name: str = None):
+    def _create_endpoint(cls, callable: typing.Callable, name: str = None):
         """Create endpoint."""
+        if not isinstance(callable, typing.Callable):
+            raise ValueError(f"Expecting callable but got '{callable}'.")
+
+        if not inspect.isroutine(callable):
+            if not name:
+                name = callable.__name__
+            # Expecting a callable to be class implementing __call__.
+            return cls._create_endpoint(getattr(callable, "__call__"), name)
+
         if not name:
             try:
-                name = function.__name__
+                name = callable.__name__
             except AttributeError as err:
-                logger.warning("Endpoint name is optional if the value can be read from "
-                               "the provided function by calling function.__name__.")
-                raise ValueError("Endpoint name not provided and exposed function raised the "
-                                 f"following error when calling function.__name__: {err}") from err
+                logger.warning(
+                    "Endpoint name is optional if the value can be read from "
+                    "the provided function by calling function.__name__."
+                )
+                raise ValueError(
+                    "Endpoint name not provided and exposed function raised the "
+                    f"following error when calling function.__name__: {err}"
+                ) from err
 
-        return Endpoint(name, function)
+        return Endpoint(name, callable)
 
     def expose(self, function: typing.Callable, name: str = None):
         """Expose a function with given name.
 
         Name of the callable shall be used if name is not given. The name is resolved by calling
         __name__ of the callable.
         """
         logger.debug("Exposing %s ...", function)
 
         endpoint = self._create_endpoint(function, name)
+        endpoint.setup(self.codecs)
         self.endpoints[endpoint.name] = endpoint
 
-        logger.debug("Exposed %s as %s", function, endpoint)
-
     @property
     def ssl_enabled(self) -> bool:
         """Is SLL enabled."""
         return self._ssl_enabled
 
     def use_ssl(self, cert_file: str, key_file: str, password=None):
         """Use SSL.
```

### Comparing `remotecall-0.1.6/src/remotecall.egg-info/PKG-INFO` & `remotecall-0.2.0/src/remotecall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotecall
-Version: 0.1.6
+Version: 0.2.0
 Summary: The module provides functionality to expose Python functions to be called remotely over ethernet.
 Home-page: https://gitlab.com/slaine/remotecall.git/
 Author: Sami Laine
 Author-email: sami.jy.laine@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `remotecall-0.1.6/src/remotecall.egg-info/SOURCES.txt` & `remotecall-0.2.0/src/remotecall.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 LICENSE
 README.md
 setup.py
 src/remotecall/__init__.py
 src/remotecall/__main__.py
+src/remotecall/_codecs copy 2.py
+src/remotecall/_codecs copy.py
 src/remotecall/_meta.py
 src/remotecall/client.py
 src/remotecall/clientfactory.py
 src/remotecall/codecs.py
 src/remotecall/endpoint.py
 src/remotecall/errors.py
 src/remotecall/gethandler.py
 src/remotecall/posthandler.py
 src/remotecall/requesthandler.py
 src/remotecall/response.py
 src/remotecall/server.py
+src/remotecall/utils.py
 src/remotecall.egg-info/PKG-INFO
 src/remotecall.egg-info/SOURCES.txt
 src/remotecall.egg-info/dependency_links.txt
 src/remotecall.egg-info/entry_points.txt
 src/remotecall.egg-info/not-zip-safe
 src/remotecall.egg-info/requires.txt
 src/remotecall.egg-info/top_level.txt
```

