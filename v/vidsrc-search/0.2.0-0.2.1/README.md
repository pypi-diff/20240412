# Comparing `tmp/vidsrc-search-0.2.0.tar.gz` & `tmp/vidsrc-search-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc-search-0.2.0.tar", last modified: Fri Apr 12 03:31:17 2024, max compression
+gzip compressed data, was "vidsrc-search-0.2.1.tar", last modified: Fri Apr 12 06:29:54 2024, max compression
```

## Comparing `vidsrc-search-0.2.0.tar` & `vidsrc-search-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.257791 vidsrc-search-0.2.0/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc-search-0.2.0/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 03:31:17.257609 vidsrc-search-0.2.0/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc-search-0.2.0/README.md
--rw-r--r--   0 Dev        (502) staff       (20)      837 2024-04-12 02:31:05.000000 vidsrc-search-0.2.0/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-12 03:31:17.257830 vidsrc-search-0.2.0/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.254444 vidsrc-search-0.2.0/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.256298 vidsrc-search-0.2.0/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1666 2024-04-12 03:28:41.000000 vidsrc-search-0.2.0/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     2200 2024-04-12 00:21:20.000000 vidsrc-search-0.2.0/src/vidsrc_search/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     5313 2024-04-12 02:49:25.000000 vidsrc-search-0.2.0/src/vidsrc_search/library.py
--rw-r--r--   0 Dev        (502) staff       (20)     1905 2024-04-12 02:39:37.000000 vidsrc-search-0.2.0/src/vidsrc_search/modules.py
--rw-r--r--   0 Dev        (502) staff       (20)     7554 2024-04-12 03:25:02.000000 vidsrc-search-0.2.0/src/vidsrc_search/search.py
--rw-r--r--   0 Dev        (502) staff       (20)     8534 2024-04-12 03:27:36.000000 vidsrc-search-0.2.0/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.257428 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      455 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 06:29:54.715870 vidsrc-search-0.2.1/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc-search-0.2.1/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 06:29:54.715666 vidsrc-search-0.2.1/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc-search-0.2.1/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)      837 2024-04-12 06:29:10.000000 vidsrc-search-0.2.1/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-12 06:29:54.715912 vidsrc-search-0.2.1/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 06:29:54.712721 vidsrc-search-0.2.1/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 06:29:54.714427 vidsrc-search-0.2.1/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1666 2024-04-12 03:33:24.000000 vidsrc-search-0.2.1/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2213 2024-04-12 06:17:23.000000 vidsrc-search-0.2.1/src/vidsrc_search/argparsing.py
+-rw-r--r--   0 Dev        (502) staff       (20)     5314 2024-04-12 04:55:16.000000 vidsrc-search-0.2.1/src/vidsrc_search/library.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1907 2024-04-12 06:18:05.000000 vidsrc-search-0.2.1/src/vidsrc_search/modules.py
+-rw-r--r--   0 Dev        (502) staff       (20)     7690 2024-04-12 06:25:59.000000 vidsrc-search-0.2.1/src/vidsrc_search/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)     8534 2024-04-12 06:29:07.000000 vidsrc-search-0.2.1/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 06:29:54.715462 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      455 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-12 06:29:54.000000 vidsrc-search-0.2.1/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc-search-0.2.0/LICENSE` & `vidsrc-search-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.2.0/PKG-INFO` & `vidsrc-search-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `vidsrc-search-0.2.0/README.md` & `vidsrc-search-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.2.0/pyproject.toml` & `vidsrc-search-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.2.0"
+version = "0.2.1"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/__main__.py` & `vidsrc-search-0.2.1/src/vidsrc_search/__main__.py`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/argparsing.py` & `vidsrc-search-0.2.1/src/vidsrc_search/argparsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Dict, Any
+from typing import List, Tuple, Dict, Any, Union
 
 
 class ArgumentsError(Exception):
     def __init__(
         self,
         message: str,
         code: int = 1
@@ -25,15 +25,15 @@
 
 def is_stacked_flag(flag: str) -> bool:
     if len(flag) <= 2:
         return False
     return flag[0] == "-" and flag[1] != "-"
 
 
-def process_bool_flag(flag: tuple) -> int | str:
+def process_bool_flag(flag: tuple) -> Union[int, str]:
     if not is_int(flag[1]):
         return flag[1]
     return bool(int(flag[1]))
 
 
 def split_arguments(argv: List[str]) -> Tuple[Any, Any]:
     for index, arg in enumerate(argv):
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/library.py` & `vidsrc-search-0.2.1/src/vidsrc_search/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,8 +151,8 @@
     size = get_folder_size_recursive(path)
 
     units = ["bytes", "kb", "mb", "gb", "tb"]
     index = 0
     while size >= 1024:
         size /= 1024
         index += 1
-    print(f"total disk usage by vidsrc-search: {round(size, 2)}{units[index]}")
+    print(f"total disk usage by vidsrc-search: {round(size, 2)} {units[index]}")
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/modules.py` & `vidsrc-search-0.2.1/src/vidsrc_search/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         sys.exit(0)
     if args["module"] == ["help", "library"]:
         utils.show_help_lib()
         sys.exit(0)
     if args["module"] == ["help", "search"]:
         utils.show_help_search()
         sys.exit(0)
-    if args["module"] == ["libary", "download"]:
+    if args["module"] == ["library", "download"]:
         library.handle_download()
         sys.exit(0)
-    if args["module"] == ["libary", "remove"]:
+    if args["module"] == ["library", "remove"]:
         library.handle_remove()
         sys.exit(0)
     if args["module"] == ["library", "size"]:
         library.get_size()
         sys.exit(0)
     if args["module"][0] == "search":
         if len(args["module"]) == 2:
@@ -44,10 +44,10 @@
         else:
             raise ArgumentsError(f"expected 1 positional argument for command 'search', got {len(args['module']) - 1} instead")
     if args["module"][0] not in AvailableBaseArguments:
         raise ArgumentsError(f"'{args['module'][0]}' is not a valid positional command")
     if args["module"][0] == "version":
         raise ArgumentsError(f"expected 0 positional argument for command 'version', got {len(args['module']) - 1} instead")
     if len(args["module"]) == 1:
-        raise ArgumentsError(f"command '{args["module"][0]}' requires another positional argument")
+        raise ArgumentsError(f"command '{args['module'][0]}' requires another positional argument")
     raise ArgumentsError(f"received invalid positional command(s): {' '.join(args['module'])}")
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/search.py` & `vidsrc-search-0.2.1/src/vidsrc_search/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 def delete_substring(text, start_offset, end_offset):
     deleted_text = text[:start_offset - 1] + text[end_offset + 1:]
     return deleted_text
 
 
 def process_html(path: str) -> None:
-    print(f"infno: processing html")
+    print(f"info: processing html")
     with open(path, "r") as f:
         content = f.readlines()
         content = ''.join(content)
         while True:
             parser = FileProcesser()
             parser.feed(content)
             if len(parser.positions_tag) == 0:
@@ -132,14 +132,19 @@
     utils.check_internet()
 
     number = index + 1
     title = results[index]["Title"]
     url = results[index]["URL"]
     id = results[index]["IMDB ID"]
 
+    if raw:
+        print(f"info: opening #{number} '{title}' in new browser window")
+        webbrowser.open(url)
+        return
+
     print()
     print(f"info: checking for local cache")
     if os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")) and recache:
         print(f"info: local cache found: recaching by requesting remote html per user request")
         response = requests.get(url)
         print(f"info: remote html request status code is {response.status_code}")
         with open(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"), "w") as f:
@@ -150,25 +155,24 @@
         print(f"info: local cache not found: Caching by requesting remote html")
         response = requests.get(url)
         print(f"info: remote html request status code is {response.status_code}")
         with open(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"), "w") as f:
             print(f"info: writing remote html content to local cache")
             f.write(response.content.decode())
             print(f"info: finished caching html")
-    if not raw:
-        process_html(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
+    process_html(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
     print(f"info: opening #{number} '{title}' in new browser window")
     webbrowser.open("file://" + os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
     return
     
 
 def handle_search(query: str, raw: bool = True, recache: bool = False) -> None:
     print(f"info: searching json library for '{query}'")
-    print(f"info: open raw website: {raw}")
-    print(f"info: recaching website: {recache}")
+    print(f"info: open raw website: {str(raw).lower()}")
+    print(f"info: recaching website: {str(recache).lower()}")
     results = search_library(query)
     if results == None:
         print(f"info: '{query}' not found in movies library")
         print(f"info: vidsrc-search terminating due to entry not found")
         return
     print_movies(results)
     open_index = ask_open_index(results)
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search/utils.py` & `vidsrc-search-0.2.1/src/vidsrc_search/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import shutil
 import asyncio
 import requests
 
 import platform
 
-__version__ = "v0.2.0"
+__version__ = "v0.2.1"
 
 
 HELP_TEXT = ("\
 usage: vidsrc-search <command> [option] [flags]     \n\
                                                     \n\
 available commands:                                 \n\
     help        shows this menu                     \n\
```

### Comparing `vidsrc-search-0.2.0/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc-search-0.2.1/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

