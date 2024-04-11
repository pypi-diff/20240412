# Comparing `tmp/masterqa-1.9.0.tar.gz` & `tmp/masterqa-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterqa-1.9.0.tar", last modified: Fri Dec  1 22:35:02 2023, max compression
+gzip compressed data, was "masterqa-1.9.1.tar", last modified: Thu Apr 11 23:53:40 2024, max compression
```

## Comparing `masterqa-1.9.0.tar` & `masterqa-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-12-01 22:35:02.226246 masterqa-1.9.0/
--rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.9.0/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.9.0/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.9.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3152 2023-12-01 22:35:02.226195 masterqa-1.9.0/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.9.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-12-01 22:35:02.225346 masterqa-1.9.0/masterqa/
--rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.9.0/masterqa/__init__.py
--rwxr-xr-x   0 michael    (501) staff       (20)    17607 2023-06-24 20:37:34.000000 masterqa-1.9.0/masterqa/master_qa.py
--rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.9.0/masterqa/settings.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-12-01 22:35:02.226030 masterqa-1.9.0/masterqa.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3152 2023-12-01 22:35:02.000000 masterqa-1.9.0/masterqa.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      310 2023-12-01 22:35:02.000000 masterqa-1.9.0/masterqa.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-12-01 22:35:02.000000 masterqa-1.9.0/masterqa.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-12-01 22:35:02.000000 masterqa-1.9.0/masterqa.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        9 2023-12-01 22:35:02.000000 masterqa-1.9.0/masterqa.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.9.0/pytest.ini
--rwxr-xr-x   0 michael    (501) staff       (20)       82 2023-12-01 22:33:16.000000 masterqa-1.9.0/requirements.txt
--rwxr-xr-x   0 michael    (501) staff       (20)      188 2023-12-01 22:35:02.226441 masterqa-1.9.0/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     4218 2023-12-01 22:33:16.000000 masterqa-1.9.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-11 23:53:40.491121 masterqa-1.9.1/
+-rw-r--r--   0 michael    (501) staff       (20)     1682 2022-12-06 03:15:26.000000 masterqa-1.9.1/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1080 2022-12-06 03:15:26.000000 masterqa-1.9.1/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      100 2022-12-06 03:15:26.000000 masterqa-1.9.1/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3152 2024-04-11 23:53:40.491075 masterqa-1.9.1/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     2616 2023-01-24 04:43:53.000000 masterqa-1.9.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-11 23:53:40.490268 masterqa-1.9.1/masterqa/
+-rwxr-xr-x   0 michael    (501) staff       (20)       48 2022-12-06 03:15:26.000000 masterqa-1.9.1/masterqa/__init__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    17607 2023-06-24 20:37:34.000000 masterqa-1.9.1/masterqa/master_qa.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      718 2022-12-06 03:15:26.000000 masterqa-1.9.1/masterqa/settings.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-04-11 23:53:40.490915 masterqa-1.9.1/masterqa.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3152 2024-04-11 23:53:40.000000 masterqa-1.9.1/masterqa.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      310 2024-04-11 23:53:40.000000 masterqa-1.9.1/masterqa.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-04-11 23:53:40.000000 masterqa-1.9.1/masterqa.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2024-04-11 23:53:40.000000 masterqa-1.9.1/masterqa.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2024-04-11 23:53:40.000000 masterqa-1.9.1/masterqa.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1440 2023-04-21 19:32:04.000000 masterqa-1.9.1/pytest.ini
+-rwxr-xr-x   0 michael    (501) staff       (20)       82 2024-04-11 23:39:09.000000 masterqa-1.9.1/requirements.txt
+-rwxr-xr-x   0 michael    (501) staff       (20)      188 2024-04-11 23:53:40.491304 masterqa-1.9.1/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     4218 2024-04-11 23:39:09.000000 masterqa-1.9.1/setup.py
```

### Comparing `masterqa-1.9.0/.gitignore` & `masterqa-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/LICENSE` & `masterqa-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/PKG-INFO` & `masterqa-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.9.0
+Version: 1.9.1
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: seleniumbase>=4.21.7
+Requires-Dist: seleniumbase>=4.25.3
 Requires-Dist: pdbp>=1.5.0
 Requires-Dist: tabcompleter>=1.3.0
 Requires-Dist: sbvirtualdisplay>=1.3.0
 
 # MasterQA
 
 [![pypi](https://img.shields.io/pypi/v/masterqa.svg)](https://pypi.python.org/pypi/masterqa) [![Build Status](https://github.com/masterqa/MasterQA/workflows/CI%20build/badge.svg)](https://github.com/masterqa/MasterQA/actions)
```

### Comparing `masterqa-1.9.0/README.md` & `masterqa-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/masterqa/master_qa.py` & `masterqa-1.9.1/masterqa/master_qa.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/masterqa/settings.py` & `masterqa-1.9.1/masterqa/settings.py`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/masterqa.egg-info/PKG-INFO` & `masterqa-1.9.1/masterqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: masterqa
-Version: 1.9.0
+Version: 1.9.1
 Summary: Automation-Assisted Manual Testing - https://masterqa.com
 Home-page: https://github.com/masterqa/MasterQA
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: seleniumbase>=4.21.7
+Requires-Dist: seleniumbase>=4.25.3
 Requires-Dist: pdbp>=1.5.0
 Requires-Dist: tabcompleter>=1.3.0
 Requires-Dist: sbvirtualdisplay>=1.3.0
 
 # MasterQA
 
 [![pypi](https://img.shields.io/pypi/v/masterqa.svg)](https://pypi.python.org/pypi/masterqa) [![Build Status](https://github.com/masterqa/MasterQA/workflows/CI%20build/badge.svg)](https://github.com/masterqa/MasterQA/actions)
```

### Comparing `masterqa-1.9.0/pytest.ini` & `masterqa-1.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `masterqa-1.9.0/setup.py` & `masterqa-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,27 +67,27 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="masterqa",
-    version="1.9.0",
+    version="1.9.1",
     description="Automation-Assisted Manual Testing - https://masterqa.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X"],
     url="https://github.com/masterqa/MasterQA",
     author="Michael Mintz",
     author_email="mdmintz@gmail.com",
     maintainer="Michael Mintz",
     license="MIT",
     python_requires=">=3.7",
     install_requires=[
-        "seleniumbase>=4.21.7",
+        "seleniumbase>=4.25.3",
         "pdbp>=1.5.0",
         "tabcompleter>=1.3.0",
         "sbvirtualdisplay>=1.3.0",
     ],
     packages=["masterqa"],
     entry_points={
         "nose.plugins": []
```

