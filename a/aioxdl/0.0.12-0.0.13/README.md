# Comparing `tmp/aioxdl-0.0.12.tar.gz` & `tmp/aioxdl-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.12.tar", last modified: Fri Apr 12 08:23:15 2024, max compression
+gzip compressed data, was "aioxdl-0.0.13.tar", last modified: Fri Apr 12 08:36:07 2024, max compression
```

## Comparing `aioxdl-0.0.12.tar` & `aioxdl-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:23:15.550332 aioxdl-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 08:23:05.000000 aioxdl-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-12 08:23:15.550332 aioxdl-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 08:23:05.000000 aioxdl-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:23:15.550332 aioxdl-0.0.12/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 08:23:05.000000 aioxdl-0.0.12/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 08:23:05.000000 aioxdl-0.0.12/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-12 08:23:05.000000 aioxdl-0.0.12/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:23:15.550332 aioxdl-0.0.12/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 08:23:15.000000 aioxdl-0.0.12/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:23:15.550332 aioxdl-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 08:23:05.000000 aioxdl-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:36:07.330878 aioxdl-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 08:36:01.000000 aioxdl-0.0.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-12 08:36:07.330878 aioxdl-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-12 08:36:01.000000 aioxdl-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:36:07.326878 aioxdl-0.0.13/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 08:36:01.000000 aioxdl-0.0.13/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 08:36:01.000000 aioxdl-0.0.13/aioxdl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-12 08:36:01.000000 aioxdl-0.0.13/aioxdl/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:36:07.330878 aioxdl-0.0.13/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 08:36:07.000000 aioxdl-0.0.13/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:36:07.330878 aioxdl-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 08:36:01.000000 aioxdl-0.0.13/setup.py
```

### Comparing `aioxdl-0.0.12/LICENSE` & `aioxdl-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.12/PKG-INFO` & `aioxdl-0.0.13/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.12
+Version: 0.0.13
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,23 +52,21 @@
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    loca = "./Downloads/testfile.mkv"
     link = "https://example.link/file.txt"
+    loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
-
-
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl import Downloader
 
 async def main():
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.12 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.13 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,14 @@
 dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
-(percentage)) async def main(): core = Downloader() loca = "./Downloads/
-testfile.mkv" link = "https://example.link/file.txt" file = await core.start
+(percentage)) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
 (link, loca, progress=progress) fine = file if core.error == None else
 core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
 aioxdl import Downloader async def main(): core = Downloader() link = "https://
 example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
 (main()) ```
```

### Comparing `aioxdl-0.0.12/README.md` & `aioxdl-0.0.13/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,21 @@
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    loca = "./Downloads/testfile.mkv"
     link = "https://example.link/file.txt"
+    loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
-
-
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl import Downloader
 
 async def main():
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
-(percentage)) async def main(): core = Downloader() loca = "./Downloads/
-testfile.mkv" link = "https://example.link/file.txt" file = await core.start
+(percentage)) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
 (link, loca, progress=progress) fine = file if core.error == None else
 core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
 aioxdl import Downloader async def main(): core = Downloader() link = "https://
 example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
 (main()) ```
```

### Comparing `aioxdl-0.0.12/aioxdl/module.py` & `aioxdl-0.0.13/aioxdl/module.py`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.12/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.13/aioxdl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.12
+Version: 0.0.13
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,23 +52,21 @@
     # tsize = total_size
     # dsize = download_size
     percentage = round((dsize / tsize) * 100, 2)
     print("COMPLETED : {}%".format(percentage))
 
 async def main():
     core = Downloader()
-    loca = "./Downloads/testfile.mkv"
     link = "https://example.link/file.txt"
+    loca = await core.filename(link)
     file = await core.start(link, loca, progress=progress)
     fine = file if core.error == None else core.error
     print(fine)
 
 asyncio.run(main())
-
-
 ```
 
 ## GET FILENAME
 ```python
 from aioxdl import Downloader
 
 async def main():
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.12 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.13 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,14 @@
 dlp
                               ð¦ _A_I_O_ _D_O_W_N_L_O_A_D_E_R
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install aioxdl ``` ## USAGE ```python import
 asyncio from aioxdl import Downloader async def progress(_, stime, tsize,
 dsize): # stime = start_time # tsize = total_size # dsize = download_size
 percentage = round((dsize / tsize) * 100, 2) print("COMPLETED : {}%".format
-(percentage)) async def main(): core = Downloader() loca = "./Downloads/
-testfile.mkv" link = "https://example.link/file.txt" file = await core.start
+(percentage)) async def main(): core = Downloader() link = "https://
+example.link/file.txt" loca = await core.filename(link) file = await core.start
 (link, loca, progress=progress) fine = file if core.error == None else
 core.error print(fine) asyncio.run(main()) ``` ## GET FILENAME ```python from
 aioxdl import Downloader async def main(): core = Downloader() link = "https://
 example.link/file.txt" name = await core.filename(link) print(name) asyncio.run
 (main()) ```
```

### Comparing `aioxdl-0.0.12/setup.py` & `aioxdl-0.0.13/setup.py`

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
-    version='0.0.12',
+    version='0.0.13',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='Python fast downloader',
```

