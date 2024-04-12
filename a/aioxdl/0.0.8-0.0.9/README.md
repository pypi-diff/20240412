# Comparing `tmp/aioxdl-0.0.8.tar.gz` & `tmp/aioxdl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.8.tar", last modified: Thu Apr 11 16:32:52 2024, max compression
+gzip compressed data, was "aioxdl-0.0.9.tar", last modified: Fri Apr 12 04:46:36 2024, max compression
```

## Comparing `aioxdl-0.0.8.tar` & `aioxdl-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.712731 aioxdl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 16:32:46.000000 aioxdl-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 16:32:52.712731 aioxdl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 16:32:46.000000 aioxdl-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.708730 aioxdl-0.0.8/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 16:32:46.000000 aioxdl-0.0.8/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-11 16:32:46.000000 aioxdl-0.0.8/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:32:52.712731 aioxdl-0.0.8/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 16:32:52.000000 aioxdl-0.0.8/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:32:52.712731 aioxdl-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 16:32:46.000000 aioxdl-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:46:36.193224 aioxdl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 04:46:30.000000 aioxdl-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-12 04:46:36.193224 aioxdl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-12 04:46:30.000000 aioxdl-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:46:36.193224 aioxdl-0.0.9/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 04:46:30.000000 aioxdl-0.0.9/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-12 04:46:30.000000 aioxdl-0.0.9/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:46:36.193224 aioxdl-0.0.9/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 04:46:36.000000 aioxdl-0.0.9/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 04:46:36.193224 aioxdl-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 04:46:30.000000 aioxdl-0.0.9/setup.py
```

### Comparing `aioxdl-0.0.8/LICENSE` & `aioxdl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.8/PKG-INFO` & `aioxdl-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.8
+Version: 0.0.9
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,31 +39,43 @@
 ```bash
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
-import time, asyncio
+import asyncio
 from aioxdl import Downloader
 
 async def progress(_, stime, tsize, dsize):
+    # stime = start_time
+    # tsize = total_size
+    # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
     loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
 
-#===[ PROGRESS FUNCTION ]===
 
-# stime = start time
-# tsize = total size
-# dsize = download size
+```
+
+## GET FILENAME
+```python
+from aioxdl import Downloader
+
+async def main():
+    core = Downloader()
+    link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
+    name = await core.filename(link)
+    print(name)
 
+asyncio.run(main())
 ```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.8 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.9 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -10,16 +10,18 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
-## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
+## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() loca = "./
-Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
-18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
-= file if core.error == None else core.error print(fine) asyncio.run(main())
-#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
-= download size ```
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
+(percentage)) async def main(): core = Downloader() loca = "./Downloads/
+testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" file =
+await core.start(link, loca, progress=progress) fine = file if core.error ==
+None else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl import Downloader async def main(): core = Downloader()
+link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" name = await
+core.filename(link) print(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.8/README.md` & `aioxdl-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,43 @@
 ```bash
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
-import time, asyncio
+import asyncio
 from aioxdl import Downloader
 
 async def progress(_, stime, tsize, dsize):
+    # stime = start_time
+    # tsize = total_size
+    # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
     loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
 
-#===[ PROGRESS FUNCTION ]===
 
-# stime = start time
-# tsize = total size
-# dsize = download size
+```
+
+## GET FILENAME
+```python
+from aioxdl import Downloader
+
+async def main():
+    core = Downloader()
+    link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
+    name = await core.filename(link)
+    print(name)
 
+asyncio.run(main())
 ```
+
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
-## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
+## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() loca = "./
-Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
-18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
-= file if core.error == None else core.error print(fine) asyncio.run(main())
-#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
-= download size ```
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
+(percentage)) async def main(): core = Downloader() loca = "./Downloads/
+testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" file =
+await core.start(link, loca, progress=progress) fine = file if core.error ==
+None else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl import Downloader async def main(): core = Downloader()
+link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" name = await
+core.filename(link) print(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.8/aioxdl/module.py` & `aioxdl-0.0.9/aioxdl/module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time, aiohttp, asyncio
+from urllib.parse import unquote, urlparse
 #=================================================================================================
 
 class Downloader:
 
     def __init__(self, message=None):
         self.tsize = 0
         self.dsize = 0
@@ -11,14 +12,22 @@
         self.timeo = 1000
         self.imssg = message
         self.stime = time.time()
         self.etime = "ERROR : Timeout"
 
 #=================================================================================================
 
+    async def filename(self, url):
+        find01 = urlparse(url)
+        find02 = os.path.basename(find01.path)
+        find03 = unquote(find02)
+        return find03
+
+#=================================================================================================
+    
     async def getsizes(self, response):
         return int(response.headers.get("Content-Length", 0)) or 0
 
     async def checkurl(self, url, timeout=20):
         async with aiohttp.ClientSession() as session:
             async with session.get(url, timeout=timeout) as response:
                 return 200 if response.status == 200 else response.status
```

### Comparing `aioxdl-0.0.8/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.9/aioxdl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.8
+Version: 0.0.9
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,31 +39,43 @@
 ```bash
 pip install aioxdl
 ```
 
 ## USAGE
 
 ```python
-import time, asyncio
+import asyncio
 from aioxdl import Downloader
 
 async def progress(_, stime, tsize, dsize):
+    # stime = start_time
+    # tsize = total_size
+    # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
     loca = "./Downloads/testfile.mkv"
     link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
 
-#===[ PROGRESS FUNCTION ]===
 
-# stime = start time
-# tsize = total size
-# dsize = download size
+```
+
+## GET FILENAME
+```python
+from aioxdl import Downloader
+
+async def main():
+    core = Downloader()
+    link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh"
+    name = await core.filename(link)
+    print(name)
 
+asyncio.run(main())
 ```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.8 Summary: python helper
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.9 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -10,16 +10,18 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: ~=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: aiohttp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
-## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import time,
+## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
-dsize): percentage = round((dsize / tsize) * 100, 2) print("COMPLETED :
-{}%".format(percentage)) async def main(): core = Downloader() loca = "./
-Downloads/testfile.mkv" link = "https://www.tg-x.workers.dev/dl/
-18357?hash=AgADIh" file = await core.start(link, loca, progress=progress) fine
-= file if core.error == None else core.error print(fine) asyncio.run(main())
-#===[ PROGRESS FUNCTION ]=== # stime = start time # tsize = total size # dsize
-= download size ```
+dsize): # stime = start_time # tsize = total_size # dsize = download_size
+percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
+(percentage)) async def main(): core = Downloader() loca = "./Downloads/
+testfile.mkv" link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" file =
+await core.start(link, loca, progress=progress) fine = file if core.error ==
+None else core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME
+```python from aioxdl import Downloader async def main(): core = Downloader()
+link = "https://www.tg-x.workers.dev/dl/18357?hash=AgADIh" name = await
+core.filename(link) print(name) asyncio.run(main()) ```
```

### Comparing `aioxdl-0.0.8/setup.py` & `aioxdl-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.8',
+    version='0.0.9',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     install_requires=['aiohttp'],
     long_description=long_description,
```

