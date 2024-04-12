# Comparing `tmp/easyencryption-0.1.8.6.tar.gz` & `tmp/easyencryption-0.1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.6.tar", last modified: Fri Apr 12 15:29:39 2024, max compression
+gzip compressed data, was "easyencryption-0.1.8.7.tar", last modified: Fri Apr 12 15:34:16 2024, max compression
```

## Comparing `easyencryption-0.1.8.6.tar` & `easyencryption-0.1.8.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.464102 easyencryption-0.1.8.6/
--rw-rw-rw-   0        0        0     4118 2024-04-12 15:29:39.464102 easyencryption-0.1.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.1.8.6/README.md
--rw-rw-rw-   0        0        0      723 2024-04-12 15:29:39.469700 easyencryption-0.1.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1840 2024-04-12 15:29:09.000000 easyencryption-0.1.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.432022 easyencryption-0.1.8.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.443230 easyencryption-0.1.8.6/src/easyencryption/
--rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.6/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.6/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.6/src/easyencryption/ascii.py
--rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.6/src/easyencryption/blake.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.6/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.6/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.6/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.6/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.6/src/easyencryption/shake.py
--rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.6/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.463085 easyencryption-0.1.8.6/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     4118 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:34:16.836743 easyencryption-0.1.8.7/
+-rw-rw-rw-   0        0        0     4099 2024-04-12 15:34:16.836743 easyencryption-0.1.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.1.8.7/README.md
+-rw-rw-rw-   0        0        0      723 2024-04-12 15:34:16.838264 easyencryption-0.1.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1829 2024-04-12 15:32:58.000000 easyencryption-0.1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:34:16.811275 easyencryption-0.1.8.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 15:34:16.822486 easyencryption-0.1.8.7/src/easyencryption/
+-rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.7/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.7/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.7/src/easyencryption/ascii.py
+-rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.7/src/easyencryption/blake.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.7/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.7/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.7/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.7/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.7/src/easyencryption/shake.py
+-rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.7/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:34:16.834698 easyencryption-0.1.8.7/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     4099 2024-04-12 15:34:16.000000 easyencryption-0.1.8.7/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-12 15:34:16.000000 easyencryption-0.1.8.7/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:34:16.000000 easyencryption-0.1.8.7/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-12 15:34:16.000000 easyencryption-0.1.8.7/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 15:34:16.000000 easyencryption-0.1.8.7/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.6/PKG-INFO` & `easyencryption-0.1.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.6
+Version: 0.1.8.7
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,15 +28,14 @@
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
-Requires-Dist: os
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
```

### Comparing `easyencryption-0.1.8.6/README.md` & `easyencryption-0.1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/setup.cfg` & `easyencryption-0.1.8.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/setup.py` & `easyencryption-0.1.8.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-version = "0.1.8.6"
+version = "0.1.8.7"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -21,16 +21,15 @@
     python_requires='>=3.6',
     install_requires=[
     "setuptools>=42",
     "cryptography",
     "pycryptodomex",
     "pycryptodome",
     "wheel",
-    "eciespy",
-    "os"
+    "eciespy"
     ],
     project_urls={
         'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
         'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
         'Source': 'https://github.com/BlazenBoi/easyencryption',
     },
     classifiers=[
```

### Comparing `easyencryption-0.1.8.6/src/easyencryption/__init__.py` & `easyencryption-0.1.8.7/src/easyencryption/__init__.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/aes.py` & `easyencryption-0.1.8.7/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/ascii.py` & `easyencryption-0.1.8.7/src/easyencryption/ascii.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/blake.py` & `easyencryption-0.1.8.7/src/easyencryption/blake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/ecc.py` & `easyencryption-0.1.8.7/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/fernet.py` & `easyencryption-0.1.8.7/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/rsa.py` & `easyencryption-0.1.8.7/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/sha.py` & `easyencryption-0.1.8.7/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/shake.py` & `easyencryption-0.1.8.7/src/easyencryption/shake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption/xor.py` & `easyencryption-0.1.8.7/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.6/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.7/src/easyencryption.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.6
+Version: 0.1.8.7
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,15 +28,14 @@
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
-Requires-Dist: os
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
```

