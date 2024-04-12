# Comparing `tmp/aioxdl-0.0.7.tar.gz` & `tmp/aioxdl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.7.tar", last modified: Thu Apr 11 15:22:45 2024, max compression
+gzip compressed data, was "aioxdl-0.0.8.tar", last modified: Thu Apr 11 16:32:52 2024, max compression
```

## Comparing `aioxdl-0.0.7.tar` & `aioxdl-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:22:45.705129 aioxdl-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:22:35.000000 aioxdl-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 15:22:45.701130 aioxdl-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 15:22:35.000000 aioxdl-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:22:45.701130 aioxdl-0.0.7/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 15:22:35.000000 aioxdl-0.0.7/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-11 15:22:35.000000 aioxdl-0.0.7/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:22:45.701130 aioxdl-0.0.7/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 15:22:45.000000 aioxdl-0.0.7/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:22:45.705129 aioxdl-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 15:22:35.000000 aioxdl-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.712731 aioxdl-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 16:32:46.000000 aioxdl-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 16:32:52.712731 aioxdl-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 16:32:46.000000 aioxdl-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.708730 aioxdl-0.0.8/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 16:32:46.000000 aioxdl-0.0.8/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-11 16:32:46.000000 aioxdl-0.0.8/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.712731 aioxdl-0.0.8/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:32:52.712731 aioxdl-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 16:32:46.000000 aioxdl-0.0.8/setup.py
```

### Comparing `aioxdl-0.0.7/LICENSE` & `aioxdl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.7/PKG-INFO` & `aioxdl-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.7
+Version: 0.0.8
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.7 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.8 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.7/README.md` & `aioxdl-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.7/aioxdl/module.py` & `aioxdl-0.0.8/aioxdl/module.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         self.tsize = 0
         self.dsize = 0
         self.error = None
         self.chunk = 1024
         self.timeo = 1000
         self.imssg = message
         self.stime = time.time()
+        self.etime = "ERROR : Timeout"
 
 #=================================================================================================
 
     async def getsizes(self, response):
         return int(response.headers.get("Content-Length", 0)) or 0
 
     async def checkurl(self, url, timeout=20):
@@ -46,16 +47,16 @@
 #=================================================================================================
 
     async def start(self, url, location, timeout=1000, progress=None):
         try:
             location = await self.download(url, location, timeout, progress)
         except aiohttp.ClientConnectorError as errors:
             self.error = errors
-        except asyncio.TimeoutError as errors:
-            self.error = errors
+        except asyncio.TimeoutError:
+            self.error = self.etime
         except Exception as errors:
             self.error = errors
 
         return location
 
 #=================================================================================================
```

### Comparing `aioxdl-0.0.7/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.8/aioxdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.7
+Version: 0.0.8
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.7 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.8 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.7/setup.py` & `aioxdl-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.7',
+    version='0.0.8',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     install_requires=['aiohttp'],
     long_description=long_description,
```

