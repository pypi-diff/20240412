# Comparing `tmp/changeln-2.0.0.1.tar.gz` & `tmp/changeln-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changeln-2.0.0.1.tar", last modified: Mon Mar 11 15:38:48 2024, max compression
+gzip compressed data, was "changeln-2.0.1.tar", last modified: Fri Apr 12 18:40:26 2024, max compression
```

## Comparing `changeln-2.0.0.1.tar` & `changeln-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.510567 changeln-2.0.0.1/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-11 15:33:16.000000 changeln-2.0.0.1/LICENSE
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1411 2024-03-11 15:38:48.510567 changeln-2.0.0.1/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1155 2024-03-11 15:33:59.000000 changeln-2.0.0.1/README.md
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.506567 changeln-2.0.0.1/changeln/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        2 2023-12-27 07:50:36.000000 changeln-2.0.0.1/changeln/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      823 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/__main__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.506567 changeln-2.0.0.1/changeln/src/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        2 2023-12-27 07:50:36.000000 changeln-2.0.0.1/changeln/src/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.506567 changeln-2.0.0.1/changeln/src/features/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/features/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2604 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/features/group_make.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.506567 changeln-2.0.0.1/changeln/src/support/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4868 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/conf.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.510567 changeln-2.0.0.1/changeln/src/support/data/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/data/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1144 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/data/config.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2291 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/data/template.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      617 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/dependency.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1376 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/helper.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1784 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/output.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5769 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/parse_git.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1884 2024-03-11 15:33:16.000000 changeln-2.0.0.1/changeln/src/support/texts.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-11 15:38:48.510567 changeln-2.0.0.1/changeln.egg-info/
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1411 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      692 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/SOURCES.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/dependency_links.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       52 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/entry_points.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      141 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/requires.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       16 2024-03-11 15:38:48.000000 changeln-2.0.0.1/changeln.egg-info/top_level.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-03-11 15:38:48.510567 changeln-2.0.0.1/setup.cfg
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1742 2024-03-11 15:38:26.000000 changeln-2.0.0.1/setup.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.306872 changeln-2.0.1/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:02:39.000000 changeln-2.0.1/LICENSE
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1411 2024-04-12 18:40:26.306872 changeln-2.0.1/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1159 2024-03-16 15:02:39.000000 changeln-2.0.1/README.md
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.302872 changeln-2.0.1/changeln/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        2 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      823 2024-04-12 18:39:18.000000 changeln-2.0.1/changeln/__main__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.302872 changeln-2.0.1/changeln/src/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        2 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.302872 changeln-2.0.1/changeln/src/features/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/features/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2791 2024-04-12 18:35:56.000000 changeln-2.0.1/changeln/src/features/group_make.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.302872 changeln-2.0.1/changeln/src/support/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4868 2024-04-12 18:26:27.000000 changeln-2.0.1/changeln/src/support/conf.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.302872 changeln-2.0.1/changeln/src/support/data/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/data/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1144 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/data/config.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2291 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/data/template.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      408 2024-04-12 18:27:20.000000 changeln-2.0.1/changeln/src/support/dependency.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1376 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/helper.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1784 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/output.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5769 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/parse_git.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1884 2024-03-16 15:02:39.000000 changeln-2.0.1/changeln/src/support/texts.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-12 18:40:26.306872 changeln-2.0.1/changeln.egg-info/
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1411 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      692 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/SOURCES.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/dependency_links.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       52 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/entry_points.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      141 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/requires.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       16 2024-04-12 18:40:26.000000 changeln-2.0.1/changeln.egg-info/top_level.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-04-12 18:40:26.306872 changeln-2.0.1/setup.cfg
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1742 2024-04-12 18:26:27.000000 changeln-2.0.1/setup.py
```

### Comparing `changeln-2.0.0.1/LICENSE` & `changeln-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/PKG-INFO` & `changeln-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changeln
-Version: 2.0.0.1
+Version: 2.0.1.0
 Summary: The application allows you to generate CHANGELOG files based on Git tags.
 Home-page: https://github.com/keygenqt/changeln
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `changeln-2.0.0.1/README.md` & `changeln-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Changeln
 ===================
 
 ### Subscribe and like! <img src="https://github.com/keygenqt/changeln/blob/main/data/other/star.gif?raw=true" width="16px"/>
 
-[![PyPI version](https://badge.fury.io/py/changeln.svg)](https://badge.fury.io/py/changeln)
+[![PyPI version](https://badge.fury.io/py/changeln.svg?v=1)](https://badge.fury.io/py/changeln)
 
 ![picture](https://github.com/keygenqt/changeln/blob/main/data/banners/banner_round.png?raw=true)
 
 The application allows you to generate CHANGELOG files based on Git tags.
 
 #### Documentation:
 <p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 Changeln =================== ### Subscribe and like! [https://github.com/
 keygenqt/changeln/blob/main/data/other/star.gif?raw=true][![PyPI version]
-(https://badge.fury.io/py/changeln.svg)](https://badge.fury.io/py/changeln) !
-[picture](https://github.com/keygenqt/changeln/blob/main/data/banners/
+(https://badge.fury.io/py/changeln.svg?v=1)](https://badge.fury.io/py/changeln)
+![picture](https://github.com/keygenqt/changeln/blob/main/data/banners/
 banner_round.png?raw=true) The application allows you to generate CHANGELOG
 files based on Git tags. #### Documentation:
 _[_d_a_t_a_/_o_t_h_e_r_/_s_e_e___m_o_r_e_._g_i_f_]
 ### License ``` Copyright 2021-2024 Vitaliy Zarubin Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
```

### Comparing `changeln-2.0.0.1/changeln/__main__.py` & `changeln-2.0.1/changeln/__main__.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/features/group_make.py` & `changeln-2.0.1/changeln/src/features/group_make.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathlib import Path
 
 import markdown as mark
 from mako.template import Template
 from weasyprint import HTML
 
 from changeln.src.support.conf import OutType
-from changeln.src.support.output import echo_stdout
+from changeln.src.support.output import echo_stdout, echo_stderr
 from changeln.src.support.parse_git import ParseGit
 from changeln.src.support.texts import AppTexts
 
 
 # Generate html from template mako
 def _gen_changelog(ctx) -> str:
     """Common gen changelog."""
@@ -53,14 +53,20 @@
 
     return '\n'.join([line.strip() for line in re.sub(r'\n\n+', '\n\n', out).split('\n')])
 
 
 def group_make(ctx: {}, output: str):
     """Generate changelog."""
 
+    # Check folder has .git
+    git_folder = Path(os.getcwd()) / '.git'
+    if not git_folder.is_dir():
+        echo_stderr(AppTexts.not_found_git_folder())
+        exit(1)
+
     try:
         out_md = _gen_changelog(ctx)
     except Exception as e:
         echo_stdout(AppTexts.error_template_parse(e))
         exit(1)
 
     out_path = ctx.obj.get_path_out()
```

### Comparing `changeln-2.0.0.1/changeln/src/support/conf.py` & `changeln-2.0.1/changeln/src/support/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from changeln.src.support.data.template import CHANGELOG_TEMPLATE
 from changeln.src.support.helper import get_path_file
 from changeln.src.support.output import echo_stdout, echo_stderr
 from changeln.src.support.texts import AppTexts
 
 # Data versions
 APP_NAME = 'changeln'
-APP_VERSION = '2.0.0'
+APP_VERSION = '2.0.1'
 
 # Default path config
 PATH_CONF = './.changeln/changeln.yaml'
 PATH_MAKO = './.changeln/changeln.mako'
 
 
 # Verbose output types
```

### Comparing `changeln-2.0.0.1/changeln/src/support/data/config.py` & `changeln-2.0.1/changeln/src/support/data/config.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/support/data/template.py` & `changeln-2.0.1/changeln/src/support/data/template.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/support/helper.py` & `changeln-2.0.1/changeln/src/support/helper.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/support/output.py` & `changeln-2.0.1/changeln/src/support/output.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/support/parse_git.py` & `changeln-2.0.1/changeln/src/support/parse_git.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln/src/support/texts.py` & `changeln-2.0.1/changeln/src/support/texts.py`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/changeln.egg-info/PKG-INFO` & `changeln-2.0.1/changeln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changeln
-Version: 2.0.0.1
+Version: 2.0.1.0
 Summary: The application allows you to generate CHANGELOG files based on Git tags.
 Home-page: https://github.com/keygenqt/changeln
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `changeln-2.0.0.1/changeln.egg-info/SOURCES.txt` & `changeln-2.0.1/changeln.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `changeln-2.0.0.1/setup.py` & `changeln-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 """
 
 setuptools.setup(
     name='changeln',
-    version='2.0.0.1',
+    version='2.0.1.0',
     author='Vitaliy Zarubin',
     author_email='keygenqt@gmail.com',
     description='The application allows you to generate CHANGELOG files based on Git tags.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/keygenqt/changeln",
     packages=setuptools.find_packages(exclude=['*tests.*', '*tests']),
```

