# Comparing `tmp/shellplus-0.0.8b0.tar.gz` & `tmp/shellplus-0.0.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellplus-0.0.8b0.tar", last modified: Thu Apr 11 17:04:56 2024, max compression
+gzip compressed data, was "shellplus-0.0.8b1.tar", last modified: Fri Apr 12 18:58:25 2024, max compression
```

## Comparing `shellplus-0.0.8b0.tar` & `shellplus-0.0.8b1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.269070 shellplus-0.0.8b0/
--rw-rw-rw-   0        0        0     1096 2024-04-11 17:04:56.267170 shellplus-0.0.8b0/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.8b0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 17:04:56.269070 shellplus-0.0.8b0/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-04-11 17:04:23.000000 shellplus-0.0.8b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.258621 shellplus-0.0.8b0/shellplus/
--rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.8b0/shellplus/__init__.py
--rw-rw-rw-   0        0        0      743 2024-04-02 09:16:37.000000 shellplus-0.0.8b0/shellplus/colors1.py
--rw-rw-rw-   0        0        0     1046 2024-04-11 16:26:02.000000 shellplus-0.0.8b0/shellplus/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.266169 shellplus-0.0.8b0/shellplus.egg-info/
--rw-rw-rw-   0        0        0     1096 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 18:58:25.362839 shellplus-0.0.8b1/
+-rw-rw-rw-   0        0        0     1096 2024-04-12 18:58:25.361838 shellplus-0.0.8b1/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.8b1/README.md
+-rw-rw-rw-   0        0        0       93 2024-04-12 18:57:34.000000 shellplus-0.0.8b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:58:25.362839 shellplus-0.0.8b1/setup.cfg
+-rw-rw-rw-   0        0        0      804 2024-04-12 18:50:37.000000 shellplus-0.0.8b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:58:25.351960 shellplus-0.0.8b1/shellplus/
+-rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.8b1/shellplus/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-04-12 18:48:57.000000 shellplus-0.0.8b1/shellplus/colors1.py
+-rw-rw-rw-   0        0        0     1046 2024-04-11 16:26:02.000000 shellplus-0.0.8b1/shellplus/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:58:25.359836 shellplus-0.0.8b1/shellplus.egg-info/
+-rw-rw-rw-   0        0        0     1096 2024-04-12 18:58:25.000000 shellplus-0.0.8b1/shellplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-04-12 18:58:25.000000 shellplus-0.0.8b1/shellplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 18:58:25.000000 shellplus-0.0.8b1/shellplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-12 18:58:25.000000 shellplus-0.0.8b1/shellplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 18:58:25.000000 shellplus-0.0.8b1/shellplus.egg-info/top_level.txt
```

### Comparing `shellplus-0.0.8b0/PKG-INFO` & `shellplus-0.0.8b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.8b0
+Version: 0.0.8b1
 License: Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: rich
```

### Comparing `shellplus-0.0.8b0/README.md` & `shellplus-0.0.8b1/README.md`

 * *Files identical despite different names*

### Comparing `shellplus-0.0.8b0/setup.py` & `shellplus-0.0.8b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='shellplus',
-    version='0.0.8b0',
+    version='0.0.8b1',
     packages=find_packages(),
     install_requires=[
         'rich',  # Add any other dependencies here
     ],
     setup_requires=['wheel'],  # Add 'wheel' to setup_requires
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `shellplus-0.0.8b0/shellplus/styles.py` & `shellplus-0.0.8b1/shellplus/styles.py`

 * *Files identical despite different names*

### Comparing `shellplus-0.0.8b0/shellplus.egg-info/PKG-INFO` & `shellplus-0.0.8b1/shellplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.8b0
+Version: 0.0.8b1
 License: Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: rich
```

