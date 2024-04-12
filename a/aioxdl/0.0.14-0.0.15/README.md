# Comparing `tmp/aioxdl-0.0.14.tar.gz` & `tmp/aioxdl-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.14.tar", last modified: Fri Apr 12 09:03:17 2024, max compression
+gzip compressed data, was "aioxdl-0.0.15.tar", last modified: Fri Apr 12 10:15:53 2024, max compression
```

## Comparing `aioxdl-0.0.14.tar` & `aioxdl-0.0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:17.022974 aioxdl-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 09:03:09.000000 aioxdl-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 09:03:17.022974 aioxdl-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 09:03:09.000000 aioxdl-0.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:17.018974 aioxdl-0.0.14/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 09:03:09.000000 aioxdl-0.0.14/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 09:03:09.000000 aioxdl-0.0.14/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-12 09:03:09.000000 aioxdl-0.0.14/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:17.022974 aioxdl-0.0.14/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 09:03:17.000000 aioxdl-0.0.14/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 09:03:17.000000 aioxdl-0.0.14/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:03:17.000000 aioxdl-0.0.14/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:03:16.000000 aioxdl-0.0.14/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 09:03:17.000000 aioxdl-0.0.14/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 09:03:17.000000 aioxdl-0.0.14/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:03:17.022974 aioxdl-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 09:03:09.000000 aioxdl-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.552060 aioxdl-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 10:15:45.000000 aioxdl-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:15:53.552060 aioxdl-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 10:15:45.000000 aioxdl-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.548060 aioxdl-0.0.15/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.552060 aioxdl-0.0.15/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:15:53.552060 aioxdl-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 10:15:45.000000 aioxdl-0.0.15/setup.py
```

### Comparing `aioxdl-0.0.14/LICENSE` & `aioxdl-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.14/PKG-INFO` & `aioxdl-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.14
+Version: 0.0.15
 Summary: Python fast downloader
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.14 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.15 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.14/README.md` & `aioxdl-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.14/aioxdl/module.py` & `aioxdl-0.0.15/aioxdl/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class Downloader:
 
     def __init__(self, message=None):
         self.tsize = 0
         self.dsize = 0
         self.error = None
         self.chunk = 1024
-        self.timeo = 1000
         self.imssg = message
         self.stime = time.time()
         self.etime = "ERROR : Timeout"
 
 #=================================================================================================
 
     async def filename(self, filelink):
@@ -38,15 +37,15 @@
 
     async def checkurl(self, url, timeout=20):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 return 200 if response.status == 200 else response.status
 
     async def display(self, progress):
-        await progress(self.imssg, self.stime, self.tsize, self.dsize) if progress else None
+        await progress(self.imssg, time.time(), self.tsize, self.dsize) if progress else None
 
 #=================================================================================================
 
     async def download(self, url, location, timeout, progress):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsize += await self.getsizes(response)
```

### Comparing `aioxdl-0.0.14/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.15/aioxdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.14
+Version: 0.0.15
 Summary: Python fast downloader
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.14 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.15 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.14/setup.py` & `aioxdl-0.0.15/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.14',
+    version='0.0.15',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='Python fast downloader',
```

