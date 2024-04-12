# Comparing `tmp/unique_sdk-0.7.0.tar.gz` & `tmp/unique_sdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_sdk-0.7.0.tar", max compression
+gzip compressed data, was "unique_sdk-0.7.1.tar", max compression
```

## Comparing `unique_sdk-0.7.0.tar` & `unique_sdk-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1065 2023-12-20 10:59:43.221525 unique_sdk-0.7.0/LICENSE
--rw-r--r--   0        0        0    12693 2024-03-26 17:46:03.955332 unique_sdk-0.7.0/README.md
--rw-r--r--   0        0        0     1400 2024-03-26 17:46:30.699261 unique_sdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2594 2024-03-22 15:20:22.648673 unique_sdk-0.7.0/unique_sdk/__init__.py
--rw-r--r--   0        0        0    11523 2024-03-22 15:15:41.984136 unique_sdk-0.7.0/unique_sdk/_api_requestor.py
--rw-r--r--   0        0        0     3603 2023-12-20 10:05:35.196658 unique_sdk-0.7.0/unique_sdk/_api_resource.py
--rw-r--r--   0        0        0       46 2023-12-19 11:10:11.782500 unique_sdk-0.7.0/unique_sdk/_api_version.py
--rw-r--r--   0        0        0     2912 2024-01-15 18:56:14.302977 unique_sdk-0.7.0/unique_sdk/_error.py
--rw-r--r--   0        0        0     2512 2023-12-20 13:46:51.674076 unique_sdk-0.7.0/unique_sdk/_http_client.py
--rw-r--r--   0        0        0     3949 2023-12-20 10:11:33.905909 unique_sdk-0.7.0/unique_sdk/_list_object.py
--rw-r--r--   0        0        0      270 2023-12-19 14:12:32.854687 unique_sdk-0.7.0/unique_sdk/_object_classes.py
--rw-r--r--   0        0        0      255 2023-12-19 14:12:32.854681 unique_sdk-0.7.0/unique_sdk/_request_options.py
--rw-r--r--   0        0        0    10525 2023-12-20 10:13:15.837741 unique_sdk-0.7.0/unique_sdk/_unique_object.py
--rw-r--r--   0        0        0      576 2023-12-19 14:02:36.001115 unique_sdk-0.7.0/unique_sdk/_unique_response.py
--rw-r--r--   0        0        0     5902 2024-01-15 18:56:14.303293 unique_sdk-0.7.0/unique_sdk/_util.py
--rw-r--r--   0        0        0       18 2023-12-19 11:10:11.800792 unique_sdk-0.7.0/unique_sdk/_version.py
--rw-r--r--   0        0        0     2855 2023-12-20 14:19:43.409880 unique_sdk-0.7.0/unique_sdk/_webhook.py
--rw-r--r--   0        0        0        0 2023-12-14 16:33:56.848215 unique_sdk-0.7.0/unique_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0     1738 2024-01-25 14:58:47.770432 unique_sdk-0.7.0/unique_sdk/api_resources/_chat_completion.py
--rw-r--r--   0        0        0     2955 2024-03-22 15:15:41.984293 unique_sdk-0.7.0/unique_sdk/api_resources/_content.py
--rw-r--r--   0        0        0      374 2023-12-29 10:21:45.185710 unique_sdk-0.7.0/unique_sdk/api_resources/_event.py
--rw-r--r--   0        0        0     2384 2024-03-22 15:20:22.648780 unique_sdk-0.7.0/unique_sdk/api_resources/_integrated.py
--rw-r--r--   0        0        0     4937 2024-03-22 15:15:41.984879 unique_sdk-0.7.0/unique_sdk/api_resources/_message.py
--rw-r--r--   0        0        0     1185 2024-03-22 15:15:41.985560 unique_sdk-0.7.0/unique_sdk/api_resources/_search.py
--rw-r--r--   0        0        0     1366 2024-01-25 12:16:29.401575 unique_sdk-0.7.0/unique_sdk/api_resources/_search_string.py
--rw-r--r--   0        0        0    13153 1970-01-01 00:00:00.000000 unique_sdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-22 20:34:45.135463 unique_sdk-0.7.1/LICENSE
+-rw-r--r--   0        0        0    12693 2024-03-27 13:36:17.907620 unique_sdk-0.7.1/README.md
+-rw-r--r--   0        0        0     1400 2024-04-12 07:43:35.937528 unique_sdk-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2594 2024-03-22 15:16:21.679272 unique_sdk-0.7.1/unique_sdk/__init__.py
+-rw-r--r--   0        0        0    11523 2024-03-22 15:16:21.683007 unique_sdk-0.7.1/unique_sdk/_api_requestor.py
+-rw-r--r--   0        0        0     3603 2024-02-27 19:23:40.262420 unique_sdk-0.7.1/unique_sdk/_api_resource.py
+-rw-r--r--   0        0        0       46 2024-02-22 20:34:45.142217 unique_sdk-0.7.1/unique_sdk/_api_version.py
+-rw-r--r--   0        0        0     2912 2024-02-22 20:34:45.142578 unique_sdk-0.7.1/unique_sdk/_error.py
+-rw-r--r--   0        0        0     2512 2024-02-22 20:34:45.142765 unique_sdk-0.7.1/unique_sdk/_http_client.py
+-rw-r--r--   0        0        0     3949 2024-02-22 20:34:45.142939 unique_sdk-0.7.1/unique_sdk/_list_object.py
+-rw-r--r--   0        0        0      270 2024-02-22 20:34:45.143185 unique_sdk-0.7.1/unique_sdk/_object_classes.py
+-rw-r--r--   0        0        0      255 2024-02-22 20:34:45.143412 unique_sdk-0.7.1/unique_sdk/_request_options.py
+-rw-r--r--   0        0        0    10525 2024-02-22 20:34:45.143669 unique_sdk-0.7.1/unique_sdk/_unique_object.py
+-rw-r--r--   0        0        0      576 2024-02-22 20:34:45.143826 unique_sdk-0.7.1/unique_sdk/_unique_response.py
+-rw-r--r--   0        0        0     5902 2024-02-22 20:34:45.144184 unique_sdk-0.7.1/unique_sdk/_util.py
+-rw-r--r--   0        0        0       18 2024-02-22 20:34:45.144336 unique_sdk-0.7.1/unique_sdk/_version.py
+-rw-r--r--   0        0        0     2855 2024-02-22 20:34:45.144492 unique_sdk-0.7.1/unique_sdk/_webhook.py
+-rw-r--r--   0        0        0        0 2024-02-22 20:34:45.144734 unique_sdk-0.7.1/unique_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0     1738 2024-02-22 20:34:45.144922 unique_sdk-0.7.1/unique_sdk/api_resources/_chat_completion.py
+-rw-r--r--   0        0        0     3005 2024-04-11 09:50:40.483379 unique_sdk-0.7.1/unique_sdk/api_resources/_content.py
+-rw-r--r--   0        0        0      374 2024-02-22 20:34:45.145139 unique_sdk-0.7.1/unique_sdk/api_resources/_event.py
+-rw-r--r--   0        0        0     2368 2024-04-12 07:31:40.291232 unique_sdk-0.7.1/unique_sdk/api_resources/_integrated.py
+-rw-r--r--   0        0        0     4937 2024-03-22 15:16:21.690047 unique_sdk-0.7.1/unique_sdk/api_resources/_message.py
+-rw-r--r--   0        0        0     1235 2024-04-11 09:50:40.488785 unique_sdk-0.7.1/unique_sdk/api_resources/_search.py
+-rw-r--r--   0        0        0     1366 2024-02-22 20:34:45.147647 unique_sdk-0.7.1/unique_sdk/api_resources/_search_string.py
+-rw-r--r--   0        0        0    13153 1970-01-01 00:00:00.000000 unique_sdk-0.7.1/PKG-INFO
```

### Comparing `unique_sdk-0.7.0/LICENSE` & `unique_sdk-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/README.md` & `unique_sdk-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/pyproject.toml` & `unique_sdk-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unique-sdk"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = [
     "Konstantin Krauss <konstantin@unique.ch>",
     "Andreas Hauri <andreas@unique.ch>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `unique_sdk-0.7.0/unique_sdk/__init__.py` & `unique_sdk-0.7.1/unique_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_api_requestor.py` & `unique_sdk-0.7.1/unique_sdk/_api_requestor.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_api_resource.py` & `unique_sdk-0.7.1/unique_sdk/_api_resource.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_error.py` & `unique_sdk-0.7.1/unique_sdk/_error.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_http_client.py` & `unique_sdk-0.7.1/unique_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_list_object.py` & `unique_sdk-0.7.1/unique_sdk/_list_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_unique_object.py` & `unique_sdk-0.7.1/unique_sdk/_unique_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_unique_response.py` & `unique_sdk-0.7.1/unique_sdk/_unique_response.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_util.py` & `unique_sdk-0.7.1/unique_sdk/_util.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/_webhook.py` & `unique_sdk-0.7.1/unique_sdk/_webhook.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_chat_completion.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_chat_completion.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_content.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import ClassVar, List, Literal, Optional, TypedDict, cast
+from typing import Any, ClassVar, Dict, List, Literal, Optional, TypedDict, cast
 
 from typing_extensions import NotRequired, Unpack
 
 from unique_sdk._api_resource import APIResource
 from unique_sdk._request_options import RequestOptions
 
 
@@ -72,14 +72,15 @@
 
     id: str
     key: str
     url: Optional[str]
     title: Optional[str]
     updatedAt: str
     chunks: List[Chunk]
+    metadata: Optional[Dict[str, Any]]
 
     @classmethod
     def search(
         cls, user_id: str, company_id: str, **params: Unpack["Content.SearchParams"]
     ) -> "Content":
         return cast(
             "Content",
```

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_integrated.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_integrated.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         **params: Unpack["Integrated.CreateStream"],
     ) -> "Message":
         """
         Executes a call to the language model and streams to the chat in real-time.
         It automatically inserts references that are mentioned by the model.
         In the form of [sourceX]. The reference documents must be given as a list in searchContext.
         """
-        url = "%s/%s/stream-completion" % (cls.class_url(), "chat")
+        url = "/integrated/chat/stream-completions"
         print("stream", url, user_id, company_id, params)
         return cast(
             "Message",
             cls._static_request(
                 "post",
                 url,
                 user_id,
```

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_message.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_message.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_search.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import ClassVar, List, Literal, Optional, cast
+from typing import Any, ClassVar, Dict, List, Literal, Optional, cast
 
 from typing_extensions import NotRequired, Unpack
 
 from unique_sdk._api_resource import APIResource
 from unique_sdk._request_options import RequestOptions
 
 
@@ -25,14 +25,15 @@
     updatedAt: str
     url: Optional[str]
     title: Optional[str]
     key: Optional[str]
     order: int
     startPage: int
     endPage: int
+    metadata: Optional[Dict[str, Any]]
 
     @classmethod
     def create(
         cls, user_id: str, company_id: str, **params: Unpack["Search.CreateParams"]
     ) -> "Search":
         return cast(
             "Search",
```

### Comparing `unique_sdk-0.7.0/unique_sdk/api_resources/_search_string.py` & `unique_sdk-0.7.1/unique_sdk/api_resources/_search_string.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.7.0/PKG-INFO` & `unique_sdk-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 License: MIT
 Author: Konstantin Krauss
 Author-email: konstantin@unique.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

