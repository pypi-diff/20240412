# Comparing `tmp/butler-connect-0.9.0.tar.gz` & `tmp/butler-connect-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.9.0.tar", last modified: Fri Apr 12 07:04:15 2024, max compression
+gzip compressed data, was "butler-connect-0.9.0b0.tar", last modified: Tue Apr  9 11:18:14 2024, max compression
```

## Comparing `butler-connect-0.9.0.tar` & `butler-connect-0.9.0b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:04:15.452138 butler-connect-0.9.0/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     3861 2024-04-12 07:04:15.451136 butler-connect-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     1759 2024-04-09 11:18:02.000000 butler-connect-0.9.0/README.md
--rw-rw-rw-   0        0        0      738 2024-04-12 07:03:55.000000 butler-connect-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 07:04:15.452138 butler-connect-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 07:04:15.423168 butler-connect-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 07:04:15.426168 butler-connect-0.9.0/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.9.0/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    20896 2024-04-09 11:17:10.000000 butler-connect-0.9.0/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:04:15.430169 butler-connect-0.9.0/src/butlerDescription/
--rw-rw-rw-   0        0        0      229 2023-11-22 09:46:59.000000 butler-connect-0.9.0/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.9.0/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.9.0/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1411 2024-02-01 08:52:12.000000 butler-connect-0.9.0/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     3238 2024-02-01 08:51:24.000000 butler-connect-0.9.0/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:04:15.450141 butler-connect-0.9.0/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     3861 2024-04-12 07:04:15.000000 butler-connect-0.9.0/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-12 07:04:15.000000 butler-connect-0.9.0/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:04:15.000000 butler-connect-0.9.0/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-12 07:04:15.000000 butler-connect-0.9.0/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2024-04-12 07:04:15.000000 butler-connect-0.9.0/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.616445 butler-connect-0.9.0b0/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.9.0b0/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-09 11:18:14.615446 butler-connect-0.9.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1759 2024-04-09 11:18:02.000000 butler-connect-0.9.0b0/README.md
+-rw-rw-rw-   0        0        0      743 2024-04-09 10:28:26.000000 butler-connect-0.9.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 11:18:14.616445 butler-connect-0.9.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.588840 butler-connect-0.9.0b0/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.590840 butler-connect-0.9.0b0/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.9.0b0/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    20896 2024-04-09 11:17:10.000000 butler-connect-0.9.0b0/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.593840 butler-connect-0.9.0b0/src/butlerDescription/
+-rw-rw-rw-   0        0        0      229 2023-11-22 09:46:59.000000 butler-connect-0.9.0b0/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.9.0b0/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.9.0b0/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1411 2024-02-01 08:52:12.000000 butler-connect-0.9.0b0/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     3238 2024-02-01 08:51:24.000000 butler-connect-0.9.0b0/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:18:14.614434 butler-connect-0.9.0b0/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2024-04-09 11:18:14.000000 butler-connect-0.9.0b0/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.9.0/LICENSE` & `butler-connect-0.9.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/PKG-INFO` & `butler-connect-0.9.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.9.0
+Version: 0.9.0b0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `butler-connect-0.9.0/README.md` & `butler-connect-0.9.0b0/README.md`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/pyproject.toml` & `butler-connect-0.9.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.9.0"
+version = "0.9.0_beta"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.9.0/src/butlerConnect/pikaButler.py` & `butler-connect-0.9.0b0/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/src/butlerDescription/control.py` & `butler-connect-0.9.0b0/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/src/butlerDescription/group.py` & `butler-connect-0.9.0b0/src/butlerDescription/group.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/src/butlerDescription/signal.py` & `butler-connect-0.9.0b0/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.9.0/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.9.0b0/src/butler_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.9.0
+Version: 0.9.0b0
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

