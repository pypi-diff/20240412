# Comparing `tmp/MistralGPTIntegration-0.0.2.tar.gz` & `tmp/MistralGPTIntegration-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MistralGPTIntegration-0.0.2.tar", last modified: Sat Jan 27 16:32:11 2024, max compression
+gzip compressed data, was "MistralGPTIntegration-0.0.3.tar", last modified: Fri Apr 12 13:23:15 2024, max compression
```

## Comparing `MistralGPTIntegration-0.0.2.tar` & `MistralGPTIntegration-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 16:32:11.398587 MistralGPTIntegration-0.0.2/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-01-27 15:32:42.000000 MistralGPTIntegration-0.0.2/LICENSE
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 16:32:11.397487 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2957 2024-01-27 16:32:11.000000 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      365 2024-01-27 16:32:11.000000 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-01-27 16:32:11.000000 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       10 2024-01-27 16:32:11.000000 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       28 2024-01-27 16:32:11.000000 MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2957 2024-01-27 16:32:11.398457 MistralGPTIntegration-0.0.2/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2369 2024-01-27 16:32:09.000000 MistralGPTIntegration-0.0.2/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 16:32:11.397845 MistralGPTIntegration-0.0.2/mistralgptintegration/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       46 2024-01-27 15:35:08.000000 MistralGPTIntegration-0.0.2/mistralgptintegration/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1397 2024-01-27 15:49:29.000000 MistralGPTIntegration-0.0.2/mistralgptintegration/integration.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-01-27 16:32:11.398629 MistralGPTIntegration-0.0.2/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      796 2024-01-27 16:32:09.000000 MistralGPTIntegration-0.0.2/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 16:32:11.398172 MistralGPTIntegration-0.0.2/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 15:33:41.000000 MistralGPTIntegration-0.0.2/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2109 2024-01-27 15:44:57.000000 MistralGPTIntegration-0.0.2/tests/test_integration.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 13:23:15.412033 MistralGPTIntegration-0.0.3/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-01-27 15:32:42.000000 MistralGPTIntegration-0.0.3/LICENSE
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 13:23:15.410513 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2957 2024-04-12 13:23:15.000000 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      365 2024-04-12 13:23:15.000000 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-12 13:23:15.000000 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       17 2024-04-12 13:23:15.000000 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       28 2024-04-12 13:23:15.000000 MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2957 2024-04-12 13:23:15.411891 MistralGPTIntegration-0.0.3/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2369 2024-01-27 16:32:28.000000 MistralGPTIntegration-0.0.3/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 13:23:15.410874 MistralGPTIntegration-0.0.3/mistralgptintegration/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       46 2024-01-27 16:32:28.000000 MistralGPTIntegration-0.0.3/mistralgptintegration/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1397 2024-01-27 16:32:28.000000 MistralGPTIntegration-0.0.3/mistralgptintegration/integration.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-12 13:23:15.412081 MistralGPTIntegration-0.0.3/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      803 2024-04-12 13:23:12.000000 MistralGPTIntegration-0.0.3/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 13:23:15.411248 MistralGPTIntegration-0.0.3/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-01-27 16:32:28.000000 MistralGPTIntegration-0.0.3/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2109 2024-01-27 16:32:28.000000 MistralGPTIntegration-0.0.3/tests/test_integration.py
```

### Comparing `MistralGPTIntegration-0.0.2/LICENSE` & `MistralGPTIntegration-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MistralGPTIntegration-0.0.2/MistralGPTIntegration.egg-info/PKG-INFO` & `MistralGPTIntegration-0.0.3/MistralGPTIntegration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistralGPTIntegration
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration utility for Mistral AI API to provide GPT-based functionalities.
 Home-page: https://github.com/chigwell/MistralGPTIntegration
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `MistralGPTIntegration-0.0.2/PKG-INFO` & `MistralGPTIntegration-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MistralGPTIntegration
-Version: 0.0.2
+Version: 0.0.3
 Summary: Integration utility for Mistral AI API to provide GPT-based functionalities.
 Home-page: https://github.com/chigwell/MistralGPTIntegration
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `MistralGPTIntegration-0.0.2/README.md` & `MistralGPTIntegration-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `MistralGPTIntegration-0.0.2/mistralgptintegration/integration.py` & `MistralGPTIntegration-0.0.3/mistralgptintegration/integration.py`

 * *Files identical despite different names*

### Comparing `MistralGPTIntegration-0.0.2/setup.py` & `MistralGPTIntegration-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='MistralGPTIntegration',
-    version='0.0.2',
+    version='0.0.3',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='Integration utility for Mistral AI API to provide GPT-based functionalities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/MistralGPTIntegration',
     packages=find_packages(),
     install_requires=[
-        'mistralai',
+        'mistralai==0.1.8',
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
```

### Comparing `MistralGPTIntegration-0.0.2/tests/test_integration.py` & `MistralGPTIntegration-0.0.3/tests/test_integration.py`

 * *Files identical despite different names*

