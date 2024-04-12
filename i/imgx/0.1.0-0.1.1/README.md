# Comparing `tmp/imgx-0.1.0.tar.gz` & `tmp/imgx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgx-0.1.0.tar", last modified: Fri Apr  5 10:37:39 2024, max compression
+gzip compressed data, was "imgx-0.1.1.tar", last modified: Fri Apr 12 08:34:23 2024, max compression
```

## Comparing `imgx-0.1.0.tar` & `imgx-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-05 10:37:39.476074 imgx-0.1.0/
--rw-r--r--   0 mina       (501) staff       (20)      156 2024-04-05 10:34:18.000000 imgx-0.1.0/AUTHORS.rst
--rw-r--r--   0 mina       (501) staff       (20)     3469 2024-04-05 10:34:18.000000 imgx-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 mina       (501) staff       (20)       89 2024-04-05 10:34:18.000000 imgx-0.1.0/HISTORY.rst
--rw-r--r--   0 mina       (501) staff       (20)     1068 2024-04-05 10:34:18.000000 imgx-0.1.0/LICENSE
--rw-r--r--   0 mina       (501) staff       (20)      262 2024-04-05 10:34:18.000000 imgx-0.1.0/MANIFEST.in
--rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-05 10:37:39.476306 imgx-0.1.0/PKG-INFO
--rw-r--r--   0 mina       (501) staff       (20)      810 2024-04-05 10:34:18.000000 imgx-0.1.0/README.rst
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-05 10:37:39.469165 imgx-0.1.0/docs/
--rw-r--r--   0 mina       (501) staff       (20)      605 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/Makefile
--rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/authors.rst
--rwxr-xr-x   0 mina       (501) staff       (20)     4730 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/conf.py
--rw-r--r--   0 mina       (501) staff       (20)       33 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/contributing.rst
--rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/history.rst
--rw-r--r--   0 mina       (501) staff       (20)      301 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/index.rst
--rw-r--r--   0 mina       (501) staff       (20)     1086 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/installation.rst
--rw-r--r--   0 mina       (501) staff       (20)      802 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/make.bat
--rw-r--r--   0 mina       (501) staff       (20)       27 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/readme.rst
--rw-r--r--   0 mina       (501) staff       (20)       63 2024-04-05 10:34:18.000000 imgx-0.1.0/docs/usage.rst
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-05 10:37:39.470644 imgx-0.1.0/imgx/
--rw-r--r--   0 mina       (501) staff       (20)      122 2024-04-05 10:34:18.000000 imgx-0.1.0/imgx/__init__.py
--rw-r--r--   0 mina       (501) staff       (20)      390 2024-04-05 10:34:18.000000 imgx-0.1.0/imgx/cli.py
--rw-r--r--   0 mina       (501) staff       (20)       19 2024-04-05 10:34:18.000000 imgx-0.1.0/imgx/imgx.py
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-05 10:37:39.474452 imgx-0.1.0/imgx.egg-info/
--rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/PKG-INFO
--rw-r--r--   0 mina       (501) staff       (20)      531 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/SOURCES.txt
--rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/dependency_links.txt
--rw-r--r--   0 mina       (501) staff       (20)       39 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/entry_points.txt
--rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/not-zip-safe
--rw-r--r--   0 mina       (501) staff       (20)       11 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/requires.txt
--rw-r--r--   0 mina       (501) staff       (20)        5 2024-04-05 10:37:39.000000 imgx-0.1.0/imgx.egg-info/top_level.txt
--rw-r--r--   0 mina       (501) staff       (20)      419 2024-04-05 10:37:39.477489 imgx-0.1.0/setup.cfg
--rw-r--r--   0 mina       (501) staff       (20)     1339 2024-04-05 10:34:18.000000 imgx-0.1.0/setup.py
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-05 10:37:39.475648 imgx-0.1.0/tests/
--rw-r--r--   0 mina       (501) staff       (20)       34 2024-04-05 10:34:18.000000 imgx-0.1.0/tests/__init__.py
--rw-r--r--   0 mina       (501) staff       (20)      964 2024-04-05 10:34:18.000000 imgx-0.1.0/tests/test_imgx.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 08:34:23.896367 imgx-0.1.1/
+-rw-r--r--   0 mina       (501) staff       (20)      156 2024-04-05 10:34:18.000000 imgx-0.1.1/AUTHORS.rst
+-rw-r--r--   0 mina       (501) staff       (20)     3469 2024-04-05 10:34:18.000000 imgx-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 mina       (501) staff       (20)       89 2024-04-05 10:34:18.000000 imgx-0.1.1/HISTORY.rst
+-rw-r--r--   0 mina       (501) staff       (20)     1068 2024-04-05 10:34:18.000000 imgx-0.1.1/LICENSE
+-rw-r--r--   0 mina       (501) staff       (20)      262 2024-04-05 10:34:18.000000 imgx-0.1.1/MANIFEST.in
+-rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-12 08:34:23.896502 imgx-0.1.1/PKG-INFO
+-rw-r--r--   0 mina       (501) staff       (20)      810 2024-04-05 10:34:18.000000 imgx-0.1.1/README.rst
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 08:34:23.887604 imgx-0.1.1/docs/
+-rw-r--r--   0 mina       (501) staff       (20)      605 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/Makefile
+-rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 mina       (501) staff       (20)     4730 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/conf.py
+-rw-r--r--   0 mina       (501) staff       (20)       33 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/contributing.rst
+-rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/history.rst
+-rw-r--r--   0 mina       (501) staff       (20)      301 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/index.rst
+-rw-r--r--   0 mina       (501) staff       (20)     1086 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/installation.rst
+-rw-r--r--   0 mina       (501) staff       (20)      802 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/make.bat
+-rw-r--r--   0 mina       (501) staff       (20)       27 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/readme.rst
+-rw-r--r--   0 mina       (501) staff       (20)       63 2024-04-05 10:34:18.000000 imgx-0.1.1/docs/usage.rst
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 08:34:23.890886 imgx-0.1.1/imgx/
+-rw-r--r--   0 mina       (501) staff       (20)      122 2024-04-05 10:34:18.000000 imgx-0.1.1/imgx/__init__.py
+-rw-r--r--   0 mina       (501) staff       (20)      514 2024-04-12 08:28:01.000000 imgx-0.1.1/imgx/cli.py
+-rw-r--r--   0 mina       (501) staff       (20)       19 2024-04-05 10:34:18.000000 imgx-0.1.1/imgx/imgx.py
+-rw-r--r--   0 mina       (501) staff       (20)     3901 2024-04-12 08:30:44.000000 imgx-0.1.1/imgx/process_module.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 08:34:23.894861 imgx-0.1.1/imgx.egg-info/
+-rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/PKG-INFO
+-rw-r--r--   0 mina       (501) staff       (20)      554 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/SOURCES.txt
+-rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/dependency_links.txt
+-rw-r--r--   0 mina       (501) staff       (20)       39 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/entry_points.txt
+-rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-05 10:37:39.000000 imgx-0.1.1/imgx.egg-info/not-zip-safe
+-rw-r--r--   0 mina       (501) staff       (20)       45 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/requires.txt
+-rw-r--r--   0 mina       (501) staff       (20)        5 2024-04-12 08:34:23.000000 imgx-0.1.1/imgx.egg-info/top_level.txt
+-rw-r--r--   0 mina       (501) staff       (20)      419 2024-04-12 08:34:23.897546 imgx-0.1.1/setup.cfg
+-rw-r--r--   0 mina       (501) staff       (20)     1380 2024-04-12 08:21:29.000000 imgx-0.1.1/setup.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 08:34:23.895614 imgx-0.1.1/tests/
+-rw-r--r--   0 mina       (501) staff       (20)       34 2024-04-05 10:34:18.000000 imgx-0.1.1/tests/__init__.py
+-rw-r--r--   0 mina       (501) staff       (20)      964 2024-04-05 10:34:18.000000 imgx-0.1.1/tests/test_imgx.py
```

### Comparing `imgx-0.1.0/CONTRIBUTING.rst` & `imgx-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/LICENSE` & `imgx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/PKG-INFO` & `imgx-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Image processing package
 Home-page: https://github.com/M-Farag/imgx
 Author: Mina Amin
 Author-email: mina.farag@icloud.com
 License: MIT license
 Keywords: imgx
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `imgx-0.1.0/README.rst` & `imgx-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/docs/Makefile` & `imgx-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/docs/conf.py` & `imgx-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/docs/installation.rst` & `imgx-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/docs/make.bat` & `imgx-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imgx-0.1.0/imgx.egg-info/PKG-INFO` & `imgx-0.1.1/imgx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Image processing package
 Home-page: https://github.com/M-Farag/imgx
 Author: Mina Amin
 Author-email: mina.farag@icloud.com
 License: MIT license
 Keywords: imgx
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `imgx-0.1.0/imgx.egg-info/SOURCES.txt` & `imgx-0.1.1/imgx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 imgx/__init__.py
 imgx/cli.py
 imgx/imgx.py
+imgx/process_module.py
 imgx.egg-info/PKG-INFO
 imgx.egg-info/SOURCES.txt
 imgx.egg-info/dependency_links.txt
 imgx.egg-info/entry_points.txt
 imgx.egg-info/not-zip-safe
 imgx.egg-info/requires.txt
 imgx.egg-info/top_level.txt
```

### Comparing `imgx-0.1.0/setup.py` & `imgx-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', ]
+requirements = ['Click>=7.0', 'Pillow>=8.0','piexif','shutil','pathlib']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Mina Amin",
     author_email='mina.farag@icloud.com',
     python_requires='>=3.6',
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='imgx',
     name='imgx',
     packages=find_packages(include=['imgx', 'imgx.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M-Farag/imgx',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `imgx-0.1.0/tests/test_imgx.py` & `imgx-0.1.1/tests/test_imgx.py`

 * *Files identical despite different names*

