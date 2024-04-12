# Comparing `tmp/turkish_profile_generator-0.1.8.tar.gz` & `tmp/turkish_profile_generator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish_profile_generator-0.1.8.tar", last modified: Fri Apr 12 21:36:57 2024, max compression
+gzip compressed data, was "turkish_profile_generator-0.1.9.tar", last modified: Fri Apr 12 21:38:46 2024, max compression
```

## Comparing `turkish_profile_generator-0.1.8.tar` & `turkish_profile_generator-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/
--rw-rw-rw-   0        0        0     1085 2024-04-12 21:18:22.000000 turkish_profile_generator-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2024-04-12 21:20:56.000000 turkish_profile_generator-0.1.8/README.md
--rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      136 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1949 2024-04-12 21:30:06.000000 turkish_profile_generator-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.322962 turkish_profile_generator-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.354251 turkish_profile_generator-0.1.8/src/turkish_profile_generator/
--rw-rw-rw-   0        0        0     4366 2024-04-12 21:36:34.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator/UserProfileGenerator.py
--rw-rw-rw-   0        0        0      164 2024-04-12 21:36:41.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.385455 turkish_profile_generator-0.1.8/tests/
--rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.1.8/tests/test_module1.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:38:46.362416 turkish_profile_generator-0.1.9/
+-rw-rw-rw-   0        0        0     1085 2024-04-12 21:18:22.000000 turkish_profile_generator-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2721 2024-04-12 21:38:46.362416 turkish_profile_generator-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2024-04-12 21:20:56.000000 turkish_profile_generator-0.1.9/README.md
+-rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      136 2024-04-12 21:38:46.362416 turkish_profile_generator-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1949 2024-04-12 21:30:06.000000 turkish_profile_generator-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:38:46.308991 turkish_profile_generator-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 21:38:46.331168 turkish_profile_generator-0.1.9/src/turkish_profile_generator/
+-rw-rw-rw-   0        0        0     4366 2024-04-12 21:36:34.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator/UserProfileGenerator.py
+-rw-rw-rw-   0        0        0      164 2024-04-12 21:38:42.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:38:46.362416 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/
+-rw-rw-rw-   0        0        0     2721 2024-04-12 21:38:46.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-04-12 21:38:46.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 21:38:46.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-12 21:38:46.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-12 21:38:46.000000 turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 21:38:46.346804 turkish_profile_generator-0.1.9/tests/
+-rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.1.9/tests/test_module1.py
```

### Comparing `turkish_profile_generator-0.1.8/LICENSE` & `turkish_profile_generator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.8/PKG-INFO` & `turkish_profile_generator-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
```

### Comparing `turkish_profile_generator-0.1.8/README.md` & `turkish_profile_generator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.8/setup.py` & `turkish_profile_generator-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.8/src/turkish_profile_generator/UserProfileGenerator.py` & `turkish_profile_generator-0.1.9/src/turkish_profile_generator/UserProfileGenerator.py`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/PKG-INFO` & `turkish_profile_generator-0.1.9/src/turkish_profile_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
```

