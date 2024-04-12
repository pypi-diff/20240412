# Comparing `tmp/prelude-cli-1.7.1.tar.gz` & `tmp/prelude-cli-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.7.1.tar", last modified: Thu Apr 11 20:57:01 2024, max compression
+gzip compressed data, was "prelude-cli-1.7.2.tar", last modified: Thu Apr 11 21:12:04 2024, max compression
```

## Comparing `prelude-cli-1.7.1.tar` & `prelude-cli-1.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.202824 prelude-cli-1.7.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      909 2024-04-11 20:57:01.202717 prelude-cli-1.7.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.7.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.196599 prelude-cli-1.7.1/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude-cli-1.7.1/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.198422 prelude-cli-1.7.1/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/templates/README.md
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.201673 prelude-cli-1.7.1/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.7.1/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)    10050 2024-04-11 16:14:14.000000 prelude-cli-1.7.1/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude-cli-1.7.1/prelude_cli/views/generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8143 2024-01-05 14:14:44.000000 prelude-cli-1.7.1/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     4674 2024-03-21 18:38:20.000000 prelude-cli-1.7.1/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude-cli-1.7.1/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 20:57:01.202368 prelude-cli-1.7.1/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      909 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-11 20:57:01.000000 prelude-cli-1.7.1/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.7.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2024-04-11 20:57:01.203155 prelude-cli-1.7.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 21:12:04.888604 prelude-cli-1.7.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      933 2024-04-11 21:12:04.888500 prelude-cli-1.7.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.7.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 21:12:04.882655 prelude-cli-1.7.2/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude-cli-1.7.2/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude-cli-1.7.2/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 21:12:04.884550 prelude-cli-1.7.2/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude-cli-1.7.2/prelude_cli/templates/README.md
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude-cli-1.7.2/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 21:12:04.887614 prelude-cli-1.7.2/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude-cli-1.7.2/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.7.2/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)    10050 2024-04-11 16:14:14.000000 prelude-cli-1.7.2/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude-cli-1.7.2/prelude_cli/views/generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8143 2024-01-05 14:14:44.000000 prelude-cli-1.7.2/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     4674 2024-03-21 18:38:20.000000 prelude-cli-1.7.2/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude-cli-1.7.2/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-11 21:12:04.888172 prelude-cli-1.7.2/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      933 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      660 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       41 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-11 21:12:04.000000 prelude-cli-1.7.2/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.7.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      673 2024-04-11 21:12:04.888888 prelude-cli-1.7.2/setup.cfg
```

### Comparing `prelude-cli-1.7.1/LICENSE` & `prelude-cli-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/PKG-INFO` & `prelude-cli-1.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.1
+Version: 1.7.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: prelude-sdk==1.7.1
 Requires-Dist: click>8
 Requires-Dist: rich
+Requires-Dist: dateutil
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
 
 - IAM: manage your account 
 - Build: write and maintain your collection of security tests
```

### Comparing `prelude-cli-1.7.1/prelude_cli/cli.py` & `prelude-cli-1.7.2/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/templates/README.md` & `prelude-cli-1.7.2/prelude_cli/templates/README.md`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/build.py` & `prelude-cli-1.7.2/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/configure.py` & `prelude-cli-1.7.2/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/detect.py` & `prelude-cli-1.7.2/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/generate.py` & `prelude-cli-1.7.2/prelude_cli/views/generate.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/iam.py` & `prelude-cli-1.7.2/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/partner.py` & `prelude-cli-1.7.2/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli/views/shared.py` & `prelude-cli-1.7.2/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.7.2/prelude_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.1
+Version: 1.7.2
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: prelude-sdk==1.7.1
 Requires-Dist: click>8
 Requires-Dist: rich
+Requires-Dist: dateutil
 
 # Prelude CLI
 
 Interact with the full range of features in Prelude Detect, organized by:
 
 - IAM: manage your account 
 - Build: write and maintain your collection of security tests
```

### Comparing `prelude-cli-1.7.1/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.7.2/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.7.1/setup.cfg` & `prelude-cli-1.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.7.1
+version = 1.7.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -16,14 +16,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	prelude-sdk == 1.7.1
 	click > 8
 	rich
+	dateutil
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
 
 [egg_info]
 tag_build =
```

