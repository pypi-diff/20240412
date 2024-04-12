# Comparing `tmp/easyencryption-0.1.8.4.tar.gz` & `tmp/easyencryption-0.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.4.tar", last modified: Sat Jul 29 17:28:52 2023, max compression
+gzip compressed data, was "easyencryption-0.1.8.5.tar", last modified: Fri Apr 12 15:09:33 2024, max compression
```

## Comparing `easyencryption-0.1.8.4.tar` & `easyencryption-0.1.8.5.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.158166 easyencryption-0.1.8.4/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:28:52.158166 easyencryption-0.1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.4/README.md
--rw-rw-rw-   0        0        0      723 2023-07-29 17:28:52.160175 easyencryption-0.1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1994 2023-07-29 17:27:54.000000 easyencryption-0.1.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:28:51.618762 easyencryption-0.1.8.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.143131 easyencryption-0.1.8.4/src/easyencryption/
--rw-rw-rw-   0        0        0      467 2023-07-29 16:43:27.000000 easyencryption-0.1.8.4/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-07-29 17:00:49.000000 easyencryption-0.1.8.4/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1672 2023-07-29 16:47:28.000000 easyencryption-0.1.8.4/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.4/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1097 2023-07-29 17:21:25.000000 easyencryption-0.1.8.4/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.4/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2043 2023-07-29 16:50:30.000000 easyencryption-0.1.8.4/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1878 2023-07-29 16:44:10.000000 easyencryption-0.1.8.4/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2023-07-29 17:28:52.157654 easyencryption-0.1.8.4/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3674 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 17:28:51.000000 easyencryption-0.1.8.4/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.995749 easyencryption-0.1.8.5/
+-rw-rw-rw-   0        0        0     3839 2024-04-12 15:09:32.995749 easyencryption-0.1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.5/README.md
+-rw-rw-rw-   0        0        0      723 2024-04-12 15:09:32.997792 easyencryption-0.1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1829 2024-04-12 15:08:42.000000 easyencryption-0.1.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.970043 easyencryption-0.1.8.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.980995 easyencryption-0.1.8.5/src/easyencryption/
+-rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.5/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.5/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.5/src/easyencryption/ascii.py
+-rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.5/src/easyencryption/blake.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.5/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.5/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.5/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.5/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.5/src/easyencryption/shake.py
+-rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.5/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.994222 easyencryption-0.1.8.5/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3839 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.4/PKG-INFO` & `easyencryption-0.1.8.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.4
+Version: 0.1.8.5
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -22,14 +22,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
```

### Comparing `easyencryption-0.1.8.4/README.md` & `easyencryption-0.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.4/setup.cfg` & `easyencryption-0.1.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.4/setup.py` & `easyencryption-0.1.8.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-##with open('src/easyencryption/__init__.py', 'r') as f:
-    ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.8.4"
+version = "0.1.8.5"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -22,15 +20,16 @@
     packages=find_packages(include=['easyencryption']),
     python_requires='>=3.6',
     install_requires=[
     "setuptools>=42",
     "cryptography",
     "pycryptodomex",
     "pycryptodome",
-    "wheel"
+    "wheel",
+    "eciespy"
     ],
     project_urls={
         'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
         'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
         'Source': 'https://github.com/BlazenBoi/easyencryption',
     },
     classifiers=[
```

### Comparing `easyencryption-0.1.8.4/src/easyencryption/aes.py` & `easyencryption-0.1.8.5/src/easyencryption/aes.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
       key = open("aeseasyencryption.key", "rb").read()
     return key
   except:
     await genkey()
     key = open("aeseasyencryption.key", "rb").read()
     return key
 
-
 async def aesencrypt(slogan:str):
     key = await callkey()
     BS = AES.block_size
     pad = lambda s: s + (BS - len(s) % BS) * chr(BS - len(s) % BS)
 
     slogan = base64.b64encode(pad(slogan).encode('utf8'))
     iv = Crypto.Random.get_random_bytes(AES.block_size)
```

### Comparing `easyencryption-0.1.8.4/src/easyencryption/custom.py` & `easyencryption-0.1.8.5/src/easyencryption/ascii.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random, math
 
-async def customencrypt(string:str):
+async def asciiencrypt(string:str):
     asciis = []
     biggest = 0
     for char in enumerate(string):
         charascii = ord(char[1])
         rand = math.floor(random.random() * (126-charascii))
         if (charascii + rand) > biggest:
             biggest = charascii + rand
@@ -15,35 +15,21 @@
     for charascii in asciis:
         firststring += chr(charascii["Total"] + randadd)
         secondstring += chr(charascii["Rand"] + 65 + randadd)
     middle = chr(randadd + 65)
     finalstring = firststring + middle + secondstring
     return finalstring
 
-async def customdecrypt(string:str):
+async def asciidecrypt(string:str):
     middle = string[(len(string)-1)//2:(len(string)+2)//2]
     randadd = ord(middle) - 65
     h = len(string)//2
     mod = (len(string) + 1) % 2
     string = string[:h - mod] + string[h + 1:]
     encoded, added = string[:len(string)//2], string[len(string)//2:]
     finalstring = ""
     iternum = 0
     for ascii in enumerate(added):
         add = ord(ascii[1]) - 65 - randadd
         finalstring += chr(ord(encoded[iternum]) - add - randadd)
         iternum += 1
-    return finalstring
-
-async def customencrypttimes(string:str, times:int):
-    iternum = 0
-    while iternum < times:
-        string = await customencrypt(string)
-        iternum += 1
-    return string
-
-async def customdecrypttimes(string:str, times:int):
-    iternum = 0
-    while iternum < times:
-        string = await customdecrypt(string)
-        iternum += 1
-    return string
+    return finalstring
```

### Comparing `easyencryption-0.1.8.4/src/easyencryption/ecc.py` & `easyencryption-0.1.8.5/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.4/src/easyencryption/rsa.py` & `easyencryption-0.1.8.5/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.4/src/easyencryption/sha.py` & `easyencryption-0.1.8.5/src/easyencryption/sha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import hashlib, codecs, secrets
 
 async def gensalt():
     generated_salt = secrets.token_hex(32)
-    with open("hashsalt.key", "wb") as key_file:
+    with open("shasalteasyencryption.key", "wb") as key_file:
         key_file.write(codecs.encode(generated_salt))
     return generated_salt
 
 async def callsalt():
   try:
-    key = open("hashsalt.key", "rb").read()
+    key = open("shasalteasyencryption.key", "rb").read()
     if str(key) == "b''":
       await gensalt()
-      key = open("hashsalt.key", "rb").read()
+      key = open("shasalteasyencryption.key", "rb").read()
     return key
   except:
     await gensalt()
-    key = open("hashsalt.key", "rb").read()
+    key = open("shasalteasyencryption.key", "rb").read()
     return key
 
 async def sha224encrypt(string:str):
     salt = codecs.decode(await callsalt())
     hashing = hashlib.sha3_224(codecs.encode(salt + string))
     return hashing.hexdigest()
```

### Comparing `easyencryption-0.1.8.4/src/easyencryption/xor.py` & `easyencryption-0.1.8.5/src/easyencryption/xor.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,24 +33,8 @@
 
 async def xorencrypt(slogan:str):
       key = await callkey()
       return await crypt(slogan, key=key, encode = True)
 
 async def xordecrypt(coded_slogan:bytes):
       key = await callkey()
-      return await crypt(coded_slogan, key=key, decode = True)
-
-async def xorencrypttimes(slogan:str, times:int):
-      key = await callkey()
-      iternum = 0
-      while iternum < times:
-            slogan = codecs.decode(await crypt(slogan, key=key, encode = True))
-            iternum += 1
-      return codecs.encode(slogan)
-
-async def xordecrypttimes(coded_slogan:bytes, times:int):
-      key = await callkey()
-      iternum = 0
-      while iternum < times:
-            coded_slogan = codecs.encode(await crypt(coded_slogan, key=key, decode = True))
-            iternum += 1
-      return codecs.decode(coded_slogan)
+      return await crypt(coded_slogan, key=key, decode = True)
```

### Comparing `easyencryption-0.1.8.4/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.5/src/easyencryption.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.4
+Version: 0.1.8.5
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -22,14 +22,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: setuptools>=42
+Requires-Dist: cryptography
+Requires-Dist: pycryptodomex
+Requires-Dist: pycryptodome
+Requires-Dist: wheel
+Requires-Dist: eciespy
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
```

