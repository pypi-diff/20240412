# Comparing `tmp/lazyqyweixin-0.0.6.tar.gz` & `tmp/lazyqyweixin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyqyweixin-0.0.6.tar", last modified: Sat Mar 23 02:24:21 2024, max compression
+gzip compressed data, was "lazyqyweixin-0.0.7.tar", last modified: Fri Apr 12 03:44:21 2024, max compression
```

## Comparing `lazyqyweixin-0.0.6.tar` & `lazyqyweixin-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-23 02:24:21.178389 lazyqyweixin-0.0.6/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1307 2024-03-23 02:24:21.178203 lazyqyweixin-0.0.6/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      911 2024-03-20 10:07:30.000000 lazyqyweixin-0.0.6/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-23 02:24:21.177114 lazyqyweixin-0.0.6/lazyqyweixin/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     7093 2024-03-21 09:04:08.000000 lazyqyweixin-0.0.6/lazyqyweixin/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    12427 2024-03-23 02:23:46.000000 lazyqyweixin-0.0.6/lazyqyweixin/internal_app.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-23 02:24:21.178005 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1307 2024-03-23 02:24:21.000000 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      251 2024-03-23 02:24:21.000000 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-03-23 02:24:21.000000 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       31 2024-03-23 02:24:21.000000 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       13 2024-03-23 02:24:21.000000 lazyqyweixin-0.0.6/lazyqyweixin.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-03-23 02:24:21.178436 lazyqyweixin-0.0.6/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      902 2024-03-23 02:23:46.000000 lazyqyweixin-0.0.6/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-12 03:44:21.540209 lazyqyweixin-0.0.7/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1307 2024-04-12 03:44:21.539993 lazyqyweixin-0.0.7/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      911 2024-03-20 10:07:30.000000 lazyqyweixin-0.0.7/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-12 03:44:21.538932 lazyqyweixin-0.0.7/lazyqyweixin/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     7109 2024-04-12 03:41:55.000000 lazyqyweixin-0.0.7/lazyqyweixin/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    12427 2024-03-23 02:23:46.000000 lazyqyweixin-0.0.7/lazyqyweixin/internal_app.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-12 03:44:21.539775 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1307 2024-04-12 03:44:21.000000 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      251 2024-04-12 03:44:21.000000 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-12 03:44:21.000000 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       31 2024-04-12 03:44:21.000000 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       13 2024-04-12 03:44:21.000000 lazyqyweixin-0.0.7/lazyqyweixin.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-12 03:44:21.540262 lazyqyweixin-0.0.7/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      902 2024-04-12 03:43:53.000000 lazyqyweixin-0.0.7/setup.py
```

### Comparing `lazyqyweixin-0.0.6/PKG-INFO` & `lazyqyweixin-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqyweixin
-Version: 0.0.6
+Version: 0.0.7
 Summary: 企业微信接口封装
 Home-page: https://gitee.com/ZeroSeeker/lazyqyweixin
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyqyweixin-0.0.6/README.md` & `lazyqyweixin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lazyqyweixin-0.0.6/lazyqyweixin/__init__.py` & `lazyqyweixin-0.0.7/lazyqyweixin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         mode=AES.MODE_CBC,
         iv=key[:16])
     # 使用BASE64对密文进行解码，然后AES-CBC解密
 
     plain_text = cryptor.decrypt(base64.b64decode(encrypt))
     encoding = chardet.detect(plain_text).get("encoding")
     showlog.info(f'猜测编码：{encoding}')
-    if encoding in ["ascii", "utf-8"]:
+    if encoding in ["ascii", "utf-8", "Windows-1252"]:
         pass
     else:
         encoding = "utf-8"
     showlog.info(f"使用编码：{encoding}")
     plain_text = plain_text.decode(encoding)
     res["decode_content"] = plain_text
     # print("plain_text",plain_text)
```

### Comparing `lazyqyweixin-0.0.6/lazyqyweixin/internal_app.py` & `lazyqyweixin-0.0.7/lazyqyweixin/internal_app.py`

 * *Files identical despite different names*

### Comparing `lazyqyweixin-0.0.6/lazyqyweixin.egg-info/PKG-INFO` & `lazyqyweixin-0.0.7/lazyqyweixin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyqyweixin
-Version: 0.0.6
+Version: 0.0.7
 Summary: 企业微信接口封装
 Home-page: https://gitee.com/ZeroSeeker/lazyqyweixin
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyqyweixin-0.0.6/setup.py` & `lazyqyweixin-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazyqyweixin",
-    version="0.0.6",
+    version="0.0.7",
     description="企业微信接口封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazyqyweixin",
     packages=setuptools.find_packages(),
```

