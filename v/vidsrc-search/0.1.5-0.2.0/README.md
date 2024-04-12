# Comparing `tmp/vidsrc-search-0.1.5.tar.gz` & `tmp/vidsrc-search-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc-search-0.1.5.tar", last modified: Thu Apr 11 00:30:01 2024, max compression
+gzip compressed data, was "vidsrc-search-0.2.0.tar", last modified: Fri Apr 12 03:31:17 2024, max compression
```

## Comparing `vidsrc-search-0.1.5.tar` & `vidsrc-search-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:30:01.280340 vidsrc-search-0.1.5/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:03:32.000000 vidsrc-search-0.1.5/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     1417 2024-04-11 00:30:01.280098 vidsrc-search-0.1.5/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      668 2024-04-11 00:03:32.000000 vidsrc-search-0.1.5/README.md
--rw-r--r--   0 Dev        (502) staff       (20)      854 2024-04-11 00:29:54.000000 vidsrc-search-0.1.5/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-11 00:30:01.280381 vidsrc-search-0.1.5/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:30:01.275204 vidsrc-search-0.1.5/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:30:01.277707 vidsrc-search-0.1.5/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1235 2024-04-10 22:54:38.000000 vidsrc-search-0.1.5/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     4741 2024-04-11 00:29:34.000000 vidsrc-search-0.1.5/src/vidsrc_search/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     2763 2024-04-11 00:29:21.000000 vidsrc-search-0.1.5/src/vidsrc_search/download.py
--rw-r--r--   0 Dev        (502) staff       (20)     1249 2024-04-10 22:39:47.000000 vidsrc-search-0.1.5/src/vidsrc_search/json_utils.py
--rw-r--r--   0 Dev        (502) staff       (20)     5325 2024-04-11 00:29:04.000000 vidsrc-search-0.1.5/src/vidsrc_search/search.py
--rw-r--r--   0 Dev        (502) staff       (20)      891 2024-04-11 00:27:58.000000 vidsrc-search-0.1.5/src/vidsrc_search/uninstall.py
--rw-r--r--   0 Dev        (502) staff       (20)     6621 2024-04-11 00:28:41.000000 vidsrc-search-0.1.5/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-11 00:30:01.279800 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1417 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      490 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       44 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-11 00:30:01.000000 vidsrc-search-0.1.5/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.257791 vidsrc-search-0.2.0/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc-search-0.2.0/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 03:31:17.257609 vidsrc-search-0.2.0/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc-search-0.2.0/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)      837 2024-04-12 02:31:05.000000 vidsrc-search-0.2.0/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-12 03:31:17.257830 vidsrc-search-0.2.0/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.254444 vidsrc-search-0.2.0/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.256298 vidsrc-search-0.2.0/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1666 2024-04-12 03:28:41.000000 vidsrc-search-0.2.0/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2200 2024-04-12 00:21:20.000000 vidsrc-search-0.2.0/src/vidsrc_search/argparsing.py
+-rw-r--r--   0 Dev        (502) staff       (20)     5313 2024-04-12 02:49:25.000000 vidsrc-search-0.2.0/src/vidsrc_search/library.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1905 2024-04-12 02:39:37.000000 vidsrc-search-0.2.0/src/vidsrc_search/modules.py
+-rw-r--r--   0 Dev        (502) staff       (20)     7554 2024-04-12 03:25:02.000000 vidsrc-search-0.2.0/src/vidsrc_search/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)     8534 2024-04-12 03:27:36.000000 vidsrc-search-0.2.0/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 03:31:17.257428 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     1799 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      455 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-12 03:31:17.000000 vidsrc-search-0.2.0/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc-search-0.1.5/LICENSE` & `vidsrc-search-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc-search-0.1.5/PKG-INFO` & `vidsrc-search-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.5
+Version: 0.2.0
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,33 +15,40 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: thefuzz
 Requires-Dist: tabulate
 Requires-Dist: requests
-Requires-Dist: pywebview
 
 ## Overview
 
-PyMovie is a command-line utility program that searches [VidSrc](https://vidsrc.to)'s API to provide movies for free. 
+Vidsrc-search is a command-line utility program that searches [VidSrc](https://vidsrc.to)'s API to provide movies for free.
 
 ## Installation
 
 ```bash
 pip install --upgrade vidsrc-search
 vidsrc-search help
 ```
 
 ## Usage
 
 ```
-Usage: vidsrc-search <command> [options]       
-                                               
-Available commands:                            
-    help        shows this menu                
-    search      search a movie by name         
+Usage: vidsrc-search <command> [option] [flags]
+
+Available commands:
+    help        shows this menu
+    search      search a movie by name
     library     actions regarding the movie lib
-                                               
-Use 'vidsrc-search help <command>' for info    
-on a specific command.                         
+
+Use 'vidsrc-search help <command>' for info on a
+specific command. Arguments are parsed strictly in
+the order above
 ```
+
+## Implementation
+
+VidSrc provides an API to access links to specific movies hosted on their website. When you select a movie to be viewed, this program will cache the site data from VidSrc into an html file stored on disk. The program then does some proprocessing to the html webpage to remove annoying ad/redirect elements.
+
+If you would like to view the raw website without preprocessing, you can disable this feature using the `--raw` flag. Additionally, you can use the `--new` flag to re-cache an already cached website.
+
```

### Comparing `vidsrc-search-0.1.5/pyproject.toml` & `vidsrc-search-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.1.5"
+version = "0.2.0"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
@@ -19,16 +19,15 @@
 ]
 
 keywords = ["movie", "video", "search"]
 dependencies = [
     "aiohttp",
     "thefuzz",
     "tabulate",
-    "requests",
-    "pywebview"
+    "requests"
 ]
 
 requires-python = ">=3.6"
 
 [project.urls]
 Homepage = "https://github.com/SomedudeX/vidsrc-search"
```

### Comparing `vidsrc-search-0.1.5/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc-search-0.2.0/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.1.5
+Version: 0.2.0
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,33 +15,40 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: thefuzz
 Requires-Dist: tabulate
 Requires-Dist: requests
-Requires-Dist: pywebview
 
 ## Overview
 
-PyMovie is a command-line utility program that searches [VidSrc](https://vidsrc.to)'s API to provide movies for free. 
+Vidsrc-search is a command-line utility program that searches [VidSrc](https://vidsrc.to)'s API to provide movies for free.
 
 ## Installation
 
 ```bash
 pip install --upgrade vidsrc-search
 vidsrc-search help
 ```
 
 ## Usage
 
 ```
-Usage: vidsrc-search <command> [options]       
-                                               
-Available commands:                            
-    help        shows this menu                
-    search      search a movie by name         
+Usage: vidsrc-search <command> [option] [flags]
+
+Available commands:
+    help        shows this menu
+    search      search a movie by name
     library     actions regarding the movie lib
-                                               
-Use 'vidsrc-search help <command>' for info    
-on a specific command.                         
+
+Use 'vidsrc-search help <command>' for info on a
+specific command. Arguments are parsed strictly in
+the order above
 ```
+
+## Implementation
+
+VidSrc provides an API to access links to specific movies hosted on their website. When you select a movie to be viewed, this program will cache the site data from VidSrc into an html file stored on disk. The program then does some proprocessing to the html webpage to remove annoying ad/redirect elements.
+
+If you would like to view the raw website without preprocessing, you can disable this feature using the `--raw` flag. Additionally, you can use the `--new` flag to re-cache an already cached website.
+
```

