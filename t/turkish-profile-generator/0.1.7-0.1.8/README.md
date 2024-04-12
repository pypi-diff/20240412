# Comparing `tmp/turkish_profile_generator-0.1.7.tar.gz` & `tmp/turkish_profile_generator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish_profile_generator-0.1.7.tar", last modified: Fri Apr 12 21:33:01 2024, max compression
+gzip compressed data, was "turkish_profile_generator-0.1.8.tar", last modified: Fri Apr 12 21:36:57 2024, max compression
```

## Comparing `turkish_profile_generator-0.1.7.tar` & `turkish_profile_generator-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 21:33:01.122660 turkish_profile_generator-0.1.7/
--rw-rw-rw-   0        0        0     1085 2024-04-12 21:18:22.000000 turkish_profile_generator-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:33:01.122660 turkish_profile_generator-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2024-04-12 21:20:56.000000 turkish_profile_generator-0.1.7/README.md
--rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      136 2024-04-12 21:33:01.122660 turkish_profile_generator-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1949 2024-04-12 21:30:06.000000 turkish_profile_generator-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:33:01.060157 turkish_profile_generator-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 21:33:01.091429 turkish_profile_generator-0.1.7/src/turkish_profile_generator/
--rw-rw-rw-   0        0        0      478 2024-04-12 21:17:39.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator/UserProfileGenerator.py
--rw-rw-rw-   0        0        0       59 2024-04-12 21:32:57.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:33:01.107035 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:33:00.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2024-04-12 21:33:00.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 21:33:00.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-12 21:33:00.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-12 21:33:00.000000 turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 21:33:01.107035 turkish_profile_generator-0.1.7/tests/
--rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.1.7/tests/test_module1.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/
+-rw-rw-rw-   0        0        0     1085 2024-04-12 21:18:22.000000 turkish_profile_generator-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2721 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2024-04-12 21:20:56.000000 turkish_profile_generator-0.1.8/README.md
+-rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      136 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1949 2024-04-12 21:30:06.000000 turkish_profile_generator-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.322962 turkish_profile_generator-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.354251 turkish_profile_generator-0.1.8/src/turkish_profile_generator/
+-rw-rw-rw-   0        0        0     4366 2024-04-12 21:36:34.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator/UserProfileGenerator.py
+-rw-rw-rw-   0        0        0      164 2024-04-12 21:36:41.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.391976 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/
+-rw-rw-rw-   0        0        0     2721 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-12 21:36:57.000000 turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 21:36:57.385455 turkish_profile_generator-0.1.8/tests/
+-rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.1.8/tests/test_module1.py
```

### Comparing `turkish_profile_generator-0.1.7/LICENSE` & `turkish_profile_generator-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.7/PKG-INFO` & `turkish_profile_generator-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
```

### Comparing `turkish_profile_generator-0.1.7/README.md` & `turkish_profile_generator-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.7/setup.py` & `turkish_profile_generator-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.1.7/src/turkish_profile_generator.egg-info/PKG-INFO` & `turkish_profile_generator-0.1.8/src/turkish_profile_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
```

