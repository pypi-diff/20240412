# Comparing `tmp/encryptedcode-1.0.4.tar.gz` & `tmp/encryptedcode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encryptedcode-1.0.4.tar", last modified: Sun Dec  3 05:54:07 2023, max compression
+gzip compressed data, was "encryptedcode-1.1.0.tar", last modified: Fri Apr 12 16:55:59 2024, max compression
```

## Comparing `encryptedcode-1.0.4.tar` & `encryptedcode-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-12-03 05:54:07.781812 encryptedcode-1.0.4/
--rw-rw-rw-   0        0        0      726 2023-12-03 05:54:07.778815 encryptedcode-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-12-03 03:50:20.000000 encryptedcode-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-12-03 05:54:07.760825 encryptedcode-1.0.4/encryptedcode/
--rw-rw-rw-   0        0        0        0 2023-12-02 21:44:29.000000 encryptedcode-1.0.4/encryptedcode/__init__.py
--rw-rw-rw-   0        0        0     3323 2023-12-03 03:48:52.000000 encryptedcode-1.0.4/encryptedcode/encrypted_code.py
-drwxrwxrwx   0        0        0        0 2023-12-03 05:54:07.775817 encryptedcode-1.0.4/encryptedcode.egg-info/
--rw-rw-rw-   0        0        0      726 2023-12-03 05:54:07.000000 encryptedcode-1.0.4/encryptedcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-12-03 05:54:07.000000 encryptedcode-1.0.4/encryptedcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-03 05:54:07.000000 encryptedcode-1.0.4/encryptedcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-12-03 05:54:07.000000 encryptedcode-1.0.4/encryptedcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-03 05:54:07.781812 encryptedcode-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-12-03 05:51:56.000000 encryptedcode-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:55:59.944157 encryptedcode-1.1.0/
+-rw-rw-rw-   0        0        0      741 2024-04-12 16:55:59.943162 encryptedcode-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-12-03 03:50:20.000000 encryptedcode-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 16:55:59.922004 encryptedcode-1.1.0/encryptedcode/
+-rw-rw-rw-   0        0        0        0 2023-12-02 21:44:29.000000 encryptedcode-1.1.0/encryptedcode/__init__.py
+-rw-rw-rw-   0        0        0     4606 2024-04-12 16:37:24.000000 encryptedcode-1.1.0/encryptedcode/encrypted_code.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:55:59.939144 encryptedcode-1.1.0/encryptedcode.egg-info/
+-rw-rw-rw-   0        0        0      741 2024-04-12 16:55:59.000000 encryptedcode-1.1.0/encryptedcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-12 16:55:59.000000 encryptedcode-1.1.0/encryptedcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:55:59.000000 encryptedcode-1.1.0/encryptedcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-12 16:55:59.000000 encryptedcode-1.1.0/encryptedcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:55:59.947156 encryptedcode-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      691 2024-04-12 16:34:19.000000 encryptedcode-1.1.0/setup.py
```

### Comparing `encryptedcode-1.0.4/PKG-INFO` & `encryptedcode-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: encryptedcode
-Version: 1.0.4
+Version: 1.1.0
 Summary: This library can be used to encrypt and decrypt passwords using the new L0123 algorithm.
 Home-page: https://github.com/leoGlez01/password_encode.git
 Author: Leandro Gonzalez Espinosa
 Author-email: lworkgonzalez01@gmail.com
 License: MIT
-Keywords: encrypt,encode,decode,algorithm
+Keywords: encryptation,encrypted,encode,decode,algorithm
 Description-Content-Type: text/markdown
 
 # New Encoding Algorithm
 
 This package is imported absolutely in your .py files, for example: 'from encryptedcode.encrypted_code import encode', and contains two functions, one for encoding called encode() and another for decoding called decode() using the new L0123 algorithm created by Ing Software Leandro Gonzalez Espinosa
```

### Comparing `encryptedcode-1.0.4/encryptedcode/encrypted_code.py` & `encryptedcode-1.1.0/encryptedcode/encrypted_code.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,31 @@
 import random
+import os
+import platform
+
+SECRET_KEY_FILE = 'secret_key.txt'
+
+if platform.system() != 'Windows':
+    SECRET_KEY_FILE = '.' + SECRET_KEY_FILE
+
+def get_secret_key():
+    if os.path.exists(SECRET_KEY_FILE):
+        with open(SECRET_KEY_FILE, 'r') as f:
+            secret_key = f.read()
+    else:
+        secret_key = input("Type your secret phrase, please don't share it!")
+        with open(SECRET_KEY_FILE, 'w') as f:
+            f.write(secret_key)
+        
+        if platform.system() == 'Windows':
+            import ctypes
+            FILE_ATTRIBUTE_HIDDEN = 0x02
+            ctypes.windll.kernel32.SetFileAttributesW(SECRET_KEY_FILE, FILE_ATTRIBUTE_HIDDEN)
+
+    return secret_key
 
 
 def encode(cadena):
     mapping = {
         "$": "a",
         "@": "e",
         "#": "0",
@@ -67,29 +90,40 @@
 
     nueva_cadena = ""
     for caracter in cadena:
         if caracter in mapping:
             nueva_cadena += mapping[caracter]
         else:
             nueva_cadena += caracter
+    
+    selfkey = get_secret_key()
+
+    encoded_key = ""
+    for char in selfkey:
+        if char in mapping:
+            encoded_key += mapping[char]
+        else:
+            encoded_key += char
+
 
     secret_key = (
         random.choice("df")
         + random.choice("hj")
         + random.choice("$^")
         + random.choice("%")
         + random.choice("#@")
         + random.choice("!?")
         + random.choice("-_")
         + random.choice("&f")
         + random.choice("vb")
         + "."
         + "L0123"
     )
-    encrypted = nueva_cadena + "." + secret_key
+
+    encrypted = nueva_cadena + "." + secret_key+"."+ encoded_key
     return encrypted
 
 
 def decode(cadena):
     map = {
         "$": "a",
         "@": "e",
@@ -159,8 +193,16 @@
         if caracter in map_inv:
             nueva_cadena += map_inv[caracter]
         elif caracter == ".":
             break
         else:
             nueva_cadena += caracter
 
-    return nueva_cadena
+    secret = input("Type your secret phrase for decode please!")
+
+    if os.path.exists(SECRET_KEY_FILE):
+        with open(SECRET_KEY_FILE, 'r') as f:
+            secretfile = f.read()
+            if secret != secretfile:
+                return ("This phrase is wrong and don't match whit the saved one.")
+            else:
+                return nueva_cadena
```

### Comparing `encryptedcode-1.0.4/encryptedcode.egg-info/PKG-INFO` & `encryptedcode-1.1.0/encryptedcode.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: encryptedcode
-Version: 1.0.4
+Version: 1.1.0
 Summary: This library can be used to encrypt and decrypt passwords using the new L0123 algorithm.
 Home-page: https://github.com/leoGlez01/password_encode.git
 Author: Leandro Gonzalez Espinosa
 Author-email: lworkgonzalez01@gmail.com
 License: MIT
-Keywords: encrypt,encode,decode,algorithm
+Keywords: encryptation,encrypted,encode,decode,algorithm
 Description-Content-Type: text/markdown
 
 # New Encoding Algorithm
 
 This package is imported absolutely in your .py files, for example: 'from encryptedcode.encrypted_code import encode', and contains two functions, one for encoding called encode() and another for decoding called decode() using the new L0123 algorithm created by Ing Software Leandro Gonzalez Espinosa
```

### Comparing `encryptedcode-1.0.4/setup.py` & `encryptedcode-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 setup(
     name="encryptedcode",
     python_version="3.12.0",
-    version="1.0.4",
+    version="1.1.0",
     description="This library can be used to encrypt and decrypt passwords using the new L0123 algorithm.",
     long_description=readme.read(),
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Leandro Gonzalez Espinosa",
     author_email="lworkgonzalez01@gmail.com",
     packages=["encryptedcode"],
-    keywords=["encrypt", "encode", "decode", "algorithm"],
+    keywords=["encryptation", "encrypted","encode", "decode", "algorithm"],
     url="https://github.com/leoGlez01/password_encode.git",
     license="MIT",
     include_package_data=True,
 )
```

