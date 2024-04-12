# Comparing `tmp/aioxdl-0.0.15.tar.gz` & `tmp/aioxdl-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.15.tar", last modified: Fri Apr 12 10:15:53 2024, max compression
+gzip compressed data, was "aioxdl-0.0.16.tar", last modified: Fri Apr 12 10:29:06 2024, max compression
```

## Comparing `aioxdl-0.0.15.tar` & `aioxdl-0.0.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.552060 aioxdl-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 10:15:45.000000 aioxdl-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:15:53.552060 aioxdl-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 10:15:45.000000 aioxdl-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.548060 aioxdl-0.0.15/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-12 10:15:45.000000 aioxdl-0.0.15/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:15:53.552060 aioxdl-0.0.15/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 10:15:53.000000 aioxdl-0.0.15/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:15:53.552060 aioxdl-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 10:15:45.000000 aioxdl-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.519681 aioxdl-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 10:28:59.000000 aioxdl-0.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:29:06.519681 aioxdl-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 10:28:59.000000 aioxdl-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.515681 aioxdl-0.0.16/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.519681 aioxdl-0.0.16/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:29:06.519681 aioxdl-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 10:28:59.000000 aioxdl-0.0.16/setup.py
```

### Comparing `aioxdl-0.0.15/LICENSE` & `aioxdl-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.15/PKG-INFO` & `aioxdl-0.0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.15
+Version: 0.0.16
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.15 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.16 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.15/README.md` & `aioxdl-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.15/aioxdl/module.py` & `aioxdl-0.0.16/aioxdl/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 #=================================================================================================
 
 class Downloader:
 
     def __init__(self, message=None):
         self.tsize = 0
         self.dsize = 0
+        self.stime = 0
         self.error = None
         self.chunk = 1024
         self.imssg = message
-        self.stime = time.time()
         self.etime = "ERROR : Timeout"
 
 #=================================================================================================
 
     async def filename(self, filelink):
         command = {"quiet": True,  "no_warnings": True, "logger": EXlogger()}
         with YoutubeDL(command) as ydl:
@@ -37,15 +37,15 @@
 
     async def checkurl(self, url, timeout=20):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 return 200 if response.status == 200 else response.status
 
     async def display(self, progress):
-        await progress(self.imssg, time.time(), self.tsize, self.dsize) if progress else None
+        await progress(self.imssg, self.stime, self.tsize, self.dsize) if progress else None
 
 #=================================================================================================
 
     async def download(self, url, location, timeout, progress):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 self.tsize += await self.getsizes(response)
@@ -59,21 +59,22 @@
                         try: await self.display(progress)
                         except Exception: pass
 
                 return location if location else None
 
 #=================================================================================================
 
-    async def start(self, url, location, timeout=1000, progress=None):
+    async def start(self, url, flocations, timeout=1000, progress=None):
         try:
-            location = await self.download(url, location, timeout, progress)
+            self.stime = time.time()
+            flocations = await self.download(url, flocations, timeout, progress)
         except aiohttp.ClientConnectorError as errors:
             self.error = errors
         except asyncio.TimeoutError:
             self.error = self.etime
         except Exception as errors:
             self.error = errors
 
-        return location
+        return flocations
 
 #=================================================================================================
```

### Comparing `aioxdl-0.0.15/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.16/aioxdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.15
+Version: 0.0.16
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
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.15 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.16 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.15/setup.py` & `aioxdl-0.0.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.15',
+    version='0.0.16',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='Python fast downloader',
```

