# Comparing `tmp/easyencryption-0.1.8.5.tar.gz` & `tmp/easyencryption-0.1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.8.5.tar", last modified: Fri Apr 12 15:09:33 2024, max compression
+gzip compressed data, was "easyencryption-0.1.8.6.tar", last modified: Fri Apr 12 15:29:39 2024, max compression
```

## Comparing `easyencryption-0.1.8.5.tar` & `easyencryption-0.1.8.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.995749 easyencryption-0.1.8.5/
--rw-rw-rw-   0        0        0     3839 2024-04-12 15:09:32.995749 easyencryption-0.1.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     2416 2023-07-29 16:53:46.000000 easyencryption-0.1.8.5/README.md
--rw-rw-rw-   0        0        0      723 2024-04-12 15:09:32.997792 easyencryption-0.1.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1829 2024-04-12 15:08:42.000000 easyencryption-0.1.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.970043 easyencryption-0.1.8.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.980995 easyencryption-0.1.8.5/src/easyencryption/
--rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.5/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.5/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.5/src/easyencryption/ascii.py
--rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.5/src/easyencryption/blake.py
--rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.5/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.5/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.5/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.5/src/easyencryption/sha.py
--rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.5/src/easyencryption/shake.py
--rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.5/src/easyencryption/xor.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:09:32.994222 easyencryption-0.1.8.5/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3839 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 15:09:32.000000 easyencryption-0.1.8.5/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.464102 easyencryption-0.1.8.6/
+-rw-rw-rw-   0        0        0     4118 2024-04-12 15:29:39.464102 easyencryption-0.1.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2676 2024-04-12 15:21:00.000000 easyencryption-0.1.8.6/README.md
+-rw-rw-rw-   0        0        0      723 2024-04-12 15:29:39.469700 easyencryption-0.1.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1840 2024-04-12 15:29:09.000000 easyencryption-0.1.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.432022 easyencryption-0.1.8.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.443230 easyencryption-0.1.8.6/src/easyencryption/
+-rw-rw-rw-   0        0        0      597 2024-04-12 14:46:58.000000 easyencryption-0.1.8.6/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1351 2024-04-12 14:46:22.000000 easyencryption-0.1.8.6/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1294 2024-04-12 14:47:06.000000 easyencryption-0.1.8.6/src/easyencryption/ascii.py
+-rw-rw-rw-   0        0        0      955 2023-07-29 23:54:23.000000 easyencryption-0.1.8.6/src/easyencryption/blake.py
+-rw-rw-rw-   0        0        0     1457 2023-07-29 16:48:16.000000 easyencryption-0.1.8.6/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     2812 2023-07-29 23:49:56.000000 easyencryption-0.1.8.6/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1980 2023-07-29 17:27:46.000000 easyencryption-0.1.8.6/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2095 2023-08-07 00:18:36.000000 easyencryption-0.1.8.6/src/easyencryption/sha.py
+-rw-rw-rw-   0        0        0     1361 2023-07-29 23:54:11.000000 easyencryption-0.1.8.6/src/easyencryption/shake.py
+-rw-rw-rw-   0        0        0     1304 2024-04-12 14:46:21.000000 easyencryption-0.1.8.6/src/easyencryption/xor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:29:39.463085 easyencryption-0.1.8.6/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     4118 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 15:29:39.000000 easyencryption-0.1.8.6/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.8.5/PKG-INFO` & `easyencryption-0.1.8.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.5
+Version: 0.1.8.6
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,27 +28,30 @@
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
+Requires-Dist: os
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.8.5/README.md` & `easyencryption-0.1.8.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

### Comparing `easyencryption-0.1.8.5/setup.cfg` & `easyencryption-0.1.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/setup.py` & `easyencryption-0.1.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-version = "0.1.8.5"
+version = "0.1.8.6"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -21,15 +21,16 @@
     python_requires='>=3.6',
     install_requires=[
     "setuptools>=42",
     "cryptography",
     "pycryptodomex",
     "pycryptodome",
     "wheel",
-    "eciespy"
+    "eciespy",
+    "os"
     ],
     project_urls={
         'Discord Server': 'https://discord.com/invite/mPU3HybBs9',
         'Bug Tracker': 'https://github.com/BlazenBoi/easyencryption/issues',
         'Source': 'https://github.com/BlazenBoi/easyencryption',
     },
     classifiers=[
```

### Comparing `easyencryption-0.1.8.5/src/easyencryption/__init__.py` & `easyencryption-0.1.8.6/src/easyencryption/__init__.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/aes.py` & `easyencryption-0.1.8.6/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/ascii.py` & `easyencryption-0.1.8.6/src/easyencryption/ascii.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/blake.py` & `easyencryption-0.1.8.6/src/easyencryption/blake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/ecc.py` & `easyencryption-0.1.8.6/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/fernet.py` & `easyencryption-0.1.8.6/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/rsa.py` & `easyencryption-0.1.8.6/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/sha.py` & `easyencryption-0.1.8.6/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/shake.py` & `easyencryption-0.1.8.6/src/easyencryption/shake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption/xor.py` & `easyencryption-0.1.8.6/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.8.5/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.8.6/src/easyencryption.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.8.5
+Version: 0.1.8.6
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,27 +28,30 @@
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
+Requires-Dist: os
 
 In Progress...
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
-ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
-XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.
-Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.<br />
+XOR - XOR algorithm of encryption and decryption converts the plain text in the format ASCII bytes and uses XOR procedure to convert it to a specified byte.<br />
+Shake - SHAKE encryption algorithm is a method for enforcing mathematic tolerances, and uses alot of math operations to find slight drifts.<br />
+Blake - Blake is an improved version of SHA-3 optimized for 64 bit platforms.<br />
+Ascii - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA, Shake, or Blake hashing because of the checking methods.<br /><br />
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
```

