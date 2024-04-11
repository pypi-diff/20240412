# Comparing `tmp/stellrent-auth-0.0.2.tar.gz` & `tmp/stellrent-auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellrent-auth-0.0.2.tar", last modified: Thu Apr 11 17:35:38 2024, max compression
+gzip compressed data, was "stellrent-auth-0.0.3.tar", last modified: Thu Apr 11 18:30:11 2024, max compression
```

## Comparing `stellrent-auth-0.0.2.tar` & `stellrent-auth-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)     1066 2024-04-11 13:50:40.000000 stellrent-auth-0.0.2/LICENSE
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)      156 2024-04-11 13:50:40.000000 stellrent-auth-0.0.2/MANIFEST.in
--rw-r--r--   0 marcus    (1000) marcus    (1000)      813 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/PKG-INFO
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)       34 2024-04-11 13:50:41.000000 stellrent-auth-0.0.2/README.md
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)      885 2024-04-11 15:17:55.000000 stellrent-auth-0.0.2/pyproject.toml
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)       73 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/setup.cfg
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)      993 2024-04-11 17:35:15.000000 stellrent-auth-0.0.2/setup.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/stellrent_auth/
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:34:47.000000 stellrent-auth-0.0.2/stellrent_auth/__init__.py
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)     7911 2024-04-11 16:26:29.000000 stellrent-auth-0.0.2/stellrent_auth/auth.py
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/stellrent_auth.egg-info/
--rw-r--r--   0 marcus    (1000) marcus    (1000)      813 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/PKG-INFO
--rw-r--r--   0 marcus    (1000) marcus    (1000)      338 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/SOURCES.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/dependency_links.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)      103 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/requires.txt
--rw-r--r--   0 marcus    (1000) marcus    (1000)       15 2024-04-11 17:35:38.000000 stellrent-auth-0.0.2/stellrent_auth.egg-info/top_level.txt
-drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:35:38.589040 stellrent-auth-0.0.2/tests/
--rwxr-xr-x   0 marcus    (1000) marcus    (1000)      287 2024-04-11 16:26:49.000000 stellrent-auth-0.0.2/tests/test_environment_variables.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     1066 2024-04-11 13:50:40.000000 stellrent-auth-0.0.3/LICENSE
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      156 2024-04-11 13:50:40.000000 stellrent-auth-0.0.3/MANIFEST.in
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      814 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/PKG-INFO
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       34 2024-04-11 13:50:41.000000 stellrent-auth-0.0.3/README.md
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      867 2024-04-11 18:29:35.000000 stellrent-auth-0.0.3/pyproject.toml
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)       73 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/setup.cfg
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      972 2024-04-11 18:29:13.000000 stellrent-auth-0.0.3/setup.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/stellrent_auth/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 17:34:47.000000 stellrent-auth-0.0.3/stellrent_auth/__init__.py
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)     7911 2024-04-11 16:26:29.000000 stellrent-auth-0.0.3/stellrent_auth/auth.py
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/stellrent_auth.egg-info/
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      814 2024-04-11 18:30:11.000000 stellrent-auth-0.0.3/stellrent_auth.egg-info/PKG-INFO
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      338 2024-04-11 18:30:11.000000 stellrent-auth-0.0.3/stellrent_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)        1 2024-04-11 18:30:11.000000 stellrent-auth-0.0.3/stellrent_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)      103 2024-04-11 18:30:11.000000 stellrent-auth-0.0.3/stellrent_auth.egg-info/requires.txt
+-rw-r--r--   0 marcus    (1000) marcus    (1000)       15 2024-04-11 18:30:11.000000 stellrent-auth-0.0.3/stellrent_auth.egg-info/top_level.txt
+drwxr-xr-x   0 marcus    (1000) marcus    (1000)        0 2024-04-11 18:30:11.488061 stellrent-auth-0.0.3/tests/
+-rwxr-xr-x   0 marcus    (1000) marcus    (1000)      287 2024-04-11 16:26:49.000000 stellrent-auth-0.0.3/tests/test_environment_variables.py
```

### Comparing `stellrent-auth-0.0.2/LICENSE` & `stellrent-auth-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stellrent-auth-0.0.2/PKG-INFO` & `stellrent-auth-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stellrent-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: OAUTH2 and OpenID standards
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-auth
 Project-URL: Issues, https://github.com/stellrent/stellrent-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stellrent-auth
 Oatuh2 standards
```

### Comparing `stellrent-auth-0.0.2/pyproject.toml` & `stellrent-auth-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "stellrent-auth"
-dynamic = ["version", "description"]
+version = '0.0.3'
 authors = [
   { name="Marcus Rodrigues Magalhães", email="marcusrodrigues.magalhaes@stellantis.com" },
 ]
 readme = "README.md"
 # license = 'MIT'
-requires-python = '>=3.7'
+requires-python = '>=3.11'
 classifiers = [
     'Development Status :: 4 - Beta',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Framework :: Pytest',
```

### Comparing `stellrent-auth-0.0.2/setup.py` & `stellrent-auth-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 def readme():
     with open('README.md') as readme_file:
         return readme_file.read()
     
 setup(
     name='stellrent-auth',
-    version="0.0.2",
     author='Marcus R. Magalhães',
     author_email='marcusrodrigues.magalhaes@stellantis.com',
     description='OAUTH2 and OpenID standards',
     packages=['stellrent_auth'],
     include_package_data=True,
     long_description=readme(),
     long_description_content_type='text/markdown',
```

### Comparing `stellrent-auth-0.0.2/stellrent_auth/auth.py` & `stellrent-auth-0.0.3/stellrent_auth/auth.py`

 * *Files identical despite different names*

### Comparing `stellrent-auth-0.0.2/stellrent_auth.egg-info/PKG-INFO` & `stellrent-auth-0.0.3/stellrent_auth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stellrent-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: OAUTH2 and OpenID standards
 Author: Marcus R. Magalhães
 Author-email: Marcus Rodrigues Magalhães <marcusrodrigues.magalhaes@stellantis.com>
 Project-URL: Homepage, https://github.com/stellrent/stellrent-auth
 Project-URL: Issues, https://github.com/stellrent/stellrent-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # stellrent-auth
 Oatuh2 standards
```

