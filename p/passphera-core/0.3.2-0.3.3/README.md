# Comparing `tmp/passphera-core-0.3.2.tar.gz` & `tmp/passphera-core-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passphera-core-0.3.2.tar", last modified: Thu Apr 11 00:07:45 2024, max compression
+gzip compressed data, was "passphera-core-0.3.3.tar", last modified: Fri Apr 12 14:05:34 2024, max compression
```

## Comparing `passphera-core-0.3.2.tar` & `passphera-core-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:07:45.037207 passphera-core-0.3.2/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:07:45.037207 passphera-core-0.3.2/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.3.2/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:07:45.035207 passphera-core-0.3.2/passphera_core/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      141 2024-04-11 00:07:34.000000 passphera-core-0.3.2/passphera_core/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)      155 2024-04-10 23:57:17.000000 passphera-core-0.3.2/passphera_core/exceptions.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     7855 2024-04-10 23:57:17.000000 passphera-core-0.3.2/passphera_core/generator.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-11 00:07:45.036207 passphera-core-0.3.2/passphera_core.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-11 00:07:44.000000 passphera-core-0.3.2/passphera_core.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      254 2024-04-11 00:07:44.000000 passphera-core-0.3.2/passphera_core.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-11 00:07:44.000000 passphera-core-0.3.2/passphera_core.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-11 00:07:44.000000 passphera-core-0.3.2/passphera_core.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-11 00:07:45.037207 passphera-core-0.3.2/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-11 00:07:34.000000 passphera-core-0.3.2/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-12 14:05:34.918173 passphera-core-0.3.3/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-12 14:05:34.918173 passphera-core-0.3.3/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.3.3/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-12 14:05:34.916173 passphera-core-0.3.3/passphera_core/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       91 2024-04-12 14:04:49.000000 passphera-core-0.3.3/passphera_core/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      155 2024-04-10 23:57:17.000000 passphera-core-0.3.3/passphera_core/exceptions.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     7821 2024-04-12 14:04:49.000000 passphera-core-0.3.3/passphera_core/generator.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-12 14:05:34.917173 passphera-core-0.3.3/passphera_core.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-12 14:05:34.000000 passphera-core-0.3.3/passphera_core.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      254 2024-04-12 14:05:34.000000 passphera-core-0.3.3/passphera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-12 14:05:34.000000 passphera-core-0.3.3/passphera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-12 14:05:34.000000 passphera-core-0.3.3/passphera_core.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-12 14:05:34.918173 passphera-core-0.3.3/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-12 14:04:49.000000 passphera-core-0.3.3/setup.py
```

### Comparing `passphera-core-0.3.2/PKG-INFO` & `passphera-core-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.3.2
+Version: 0.3.3
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.3.2/passphera_core/generator.py` & `passphera-core-0.3.3/passphera_core/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,17 +215,16 @@
     def generate_password(self) -> str:
         """
         Generate a strong password string using the raw password (add another layer of encryption to it)
         :return: str: The generated strong password
         """
         old_algorithm = self._algorithm_name
         self._algorithm_name = 'affine'
-        self._update_algorithm_properties()
         self._password = self.generate_raw_password()
         self._algorithm_name = old_algorithm
-        self._update_algorithm_properties()
+        self._password = self.generate_raw_password()
         for char, replacement in self._chars_replacements.items():
             self._password = self._password.replace(char, replacement)
         for char in self._password:
             if char in self._text:
                 self._password = self._password.replace(char, char.upper())
         return self._password
```

### Comparing `passphera-core-0.3.2/passphera_core.egg-info/PKG-INFO` & `passphera-core-0.3.3/passphera_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.3.2
+Version: 0.3.3
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.3.2/setup.py` & `passphera-core-0.3.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='passphera-core',
-    version='0.3.2',
+    version='0.3.3',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     url='https://github.com/passphera/core',
     description='The core system of passphera project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['passphera_core'],
```

