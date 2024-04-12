# Comparing `tmp/prodpadlm_client-0.1.1.4.tar.gz` & `tmp/prodpadlm_client-0.1.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodpadlm_client-0.1.1.4.tar", last modified: Thu Apr 11 23:51:51 2024, max compression
+gzip compressed data, was "prodpadlm_client-0.1.1.4.1.tar", last modified: Fri Apr 12 16:41:23 2024, max compression
```

## Comparing `prodpadlm_client-0.1.1.4.tar` & `prodpadlm_client-0.1.1.4.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.488406 prodpadlm_client-0.1.1.4/
--rw-rw-rw-   0        0        0    11556 2024-04-08 06:33:36.000000 prodpadlm_client-0.1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    15472 2024-04-11 23:51:51.485396 prodpadlm_client-0.1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.400010 prodpadlm_client-0.1.1.4/prodpadlm_client/
--rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/__init__.py
--rw-rw-rw-   0        0        0    10775 2024-04-11 22:04:07.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.476251 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-10 11:04:40.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/_types.py
--rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/messages.py
--rw-rw-rw-   0        0        0     2052 2024-04-11 22:01:54.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/stream_messages.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.481260 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/
--rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/__init__.py
--rw-rw-rw-   0        0        0     6250 2024-04-11 22:39:06.000000 prodpadlm_client-0.1.1.4/prodpadlm_client/resources/api.py
-drwxrwxrwx   0        0        0        0 2024-04-11 23:51:51.484064 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/
--rw-rw-rw-   0        0        0    15472 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-11 23:51:51.000000 prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      958 2024-04-11 23:51:37.000000 prodpadlm_client-0.1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 23:51:51.488406 prodpadlm_client-0.1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      938 2024-04-11 22:47:39.000000 prodpadlm_client-0.1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:41:23.426875 prodpadlm_client-0.1.1.4.1/
+-rw-rw-rw-   0        0        0    11556 2024-04-08 06:33:36.000000 prodpadlm_client-0.1.1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    15471 2024-04-12 16:41:23.422450 prodpadlm_client-0.1.1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1413 2024-04-08 07:39:29.000000 prodpadlm_client-0.1.1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 16:41:23.377442 prodpadlm_client-0.1.1.4.1/prodpadlm_client/
+-rw-rw-rw-   0        0        0       49 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/__init__.py
+-rw-rw-rw-   0        0        0    10775 2024-04-11 22:04:07.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:41:23.414263 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:03:15.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-10 11:04:40.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/_types.py
+-rw-rw-rw-   0        0        0     3112 2024-04-08 01:09:30.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/messages.py
+-rw-rw-rw-   0        0        0     2052 2024-04-11 22:01:54.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/stream_messages.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:41:23.417931 prodpadlm_client-0.1.1.4.1/prodpadlm_client/resources/
+-rw-rw-rw-   0        0        0        0 2024-04-08 08:01:13.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/resources/__init__.py
+-rw-rw-rw-   0        0        0     6224 2024-04-12 16:38:15.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client/resources/api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:41:23.420447 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/
+-rw-rw-rw-   0        0        0    15471 2024-04-12 16:41:23.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2024-04-12 16:41:23.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:41:23.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-12 16:41:23.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-12 16:41:23.000000 prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      960 2024-04-12 16:40:59.000000 prodpadlm_client-0.1.1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:41:23.426875 prodpadlm_client-0.1.1.4.1/setup.cfg
```

### Comparing `prodpadlm_client-0.1.1.4/LICENSE.txt` & `prodpadlm_client-0.1.1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/PKG-INFO` & `prodpadlm_client-0.1.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: prodpadlm_client
-Version: 0.1.1.4
+Version: 0.1.1.4.1
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
-Author: Ayo Kehinde Samuel
 Author-email: Ayo Kehinde Samuel <samkehindeayo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,16 +207,17 @@
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/Stosan/prodpadlm-client.git
 Project-URL: Issues, https://github.com/Stosan/prodpadlm-client/issues
 Project-URL: Changelog, https://github.com/Stosan/prodpadlm-client/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.0
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: httpx
 Requires-Dist: pydantic-settings
 Requires-Dist: langchain
 Requires-Dist: langchain-core
 
 # ProdPadLM - Client
```

### Comparing `prodpadlm_client-0.1.1.4/README.md` & `prodpadlm_client-0.1.1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client/client.py` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client/client.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/_types.py` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/_types.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/messages.py` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/messages.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client/client_types/stream_messages.py` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client/client_types/stream_messages.py`

 * *Files identical despite different names*

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client/resources/api.py` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client/resources/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             messages: Iterable[MessageParam],
             model: str = "",
             stop_sequences: List[str] = "",
             system: str = "",
             temperature: float = 0.7,
             top_k: int = 0,
             top_p: float = 0,
-            stream: Literal[False] | Literal[True] = False,
+            stream: bool = False,
         ) -> Message:
             response = self._post.post(
                 self.url + "/api/v1/generate",
                 json={
                     "max_tokens": max_tokens,
                     "messages": messages,
                     "model": model,
```

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/PKG-INFO` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: prodpadlm_client
-Version: 0.1.1.4
+Version: 0.1.1.4.1
 Summary: Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡
-Author: Ayo Kehinde Samuel
 Author-email: Ayo Kehinde Samuel <samkehindeayo@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,16 +207,17 @@
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/Stosan/prodpadlm-client.git
 Project-URL: Issues, https://github.com/Stosan/prodpadlm-client/issues
 Project-URL: Changelog, https://github.com/Stosan/prodpadlm-client/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.0
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: httpx
 Requires-Dist: pydantic-settings
 Requires-Dist: langchain
 Requires-Dist: langchain-core
 
 # ProdPadLM - Client
```

### Comparing `prodpadlm_client-0.1.1.4/prodpadlm_client.egg-info/SOURCES.txt` & `prodpadlm_client-0.1.1.4.1/prodpadlm_client.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE.txt
 README.md
 pyproject.toml
-setup.py
 prodpadlm_client/__init__.py
 prodpadlm_client/client.py
 prodpadlm_client.egg-info/PKG-INFO
 prodpadlm_client.egg-info/SOURCES.txt
 prodpadlm_client.egg-info/dependency_links.txt
 prodpadlm_client.egg-info/requires.txt
 prodpadlm_client.egg-info/top_level.txt
```

### Comparing `prodpadlm_client-0.1.1.4/pyproject.toml` & `prodpadlm_client-0.1.1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prodpadlm_client"
-version = "0.1.1.4"
+version = "0.1.1.4.1"
 authors = [
   { name="Ayo Kehinde Samuel", email="samkehindeayo@gmail.com" },
 ]
 description = "Production LaunchPad for Language Models [Client] - ⚡ Ship Open Source LLMs to production faster and efficiently ⚡"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
```

