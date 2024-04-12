# Comparing `tmp/jhu-1.4.1.tar.gz` & `tmp/jhu-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhu-1.4.1.tar", last modified: Wed Apr 10 01:50:53 2024, max compression
+gzip compressed data, was "jhu-1.4.2.tar", last modified: Fri Apr 12 09:08:49 2024, max compression
```

## Comparing `jhu-1.4.1.tar` & `jhu-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.611858 jhu-1.4.1/
--rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.4.1/LICENSE
--rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-10 01:50:53.609788 jhu-1.4.1/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)     1624 2024-04-10 01:50:15.000000 jhu-1.4.1/README.md
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.601236 jhu-1.4.1/jhu/
--rw-r--r--   0 hujian     (501) staff       (20)       21 2024-04-10 01:48:06.000000 jhu-1.4.1/jhu/__init__.py
--rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-01-05 07:00:28.000000 jhu-1.4.1/jhu/auth.py
--rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.4.1/jhu/email.py
--rw-r--r--   0 hujian     (501) staff       (20)     3062 2024-04-10 01:48:10.000000 jhu-1.4.1/jhu/security.py
--rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.4.1/jhu/webhook.py
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-10 01:50:53.608638 jhu-1.4.1/jhu.egg-info/
--rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)      254 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/SOURCES.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/dependency_links.txt
--rw-r--r--   0 hujian     (501) staff       (20)       42 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/requires.txt
--rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-10 01:50:53.000000 jhu-1.4.1/jhu.egg-info/top_level.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.4.1/jhu.egg-info/zip-safe
--rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-10 01:50:53.612168 jhu-1.4.1/setup.cfg
--rwxr-xr-x   0 hujian     (501) staff       (20)     1592 2024-04-10 01:47:56.000000 jhu-1.4.1/setup.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.854325 jhu-1.4.2/
+-rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.4.2/LICENSE
+-rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-12 09:08:49.853584 jhu-1.4.2/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)     1706 2024-04-12 08:24:25.000000 jhu-1.4.2/README.md
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.849614 jhu-1.4.2/jhu/
+-rw-r--r--   0 hujian     (501) staff       (20)       21 2024-04-12 09:07:47.000000 jhu-1.4.2/jhu/__init__.py
+-rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-01-05 07:00:28.000000 jhu-1.4.2/jhu/auth.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.4.2/jhu/email.py
+-rw-r--r--   0 hujian     (501) staff       (20)     2620 2024-04-12 09:05:59.000000 jhu-1.4.2/jhu/security.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.4.2/jhu/webhook.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.852937 jhu-1.4.2/jhu.egg-info/
+-rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)      254 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/SOURCES.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/dependency_links.txt
+-rw-r--r--   0 hujian     (501) staff       (20)       42 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/requires.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/top_level.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.4.2/jhu.egg-info/zip-safe
+-rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-12 09:08:49.854451 jhu-1.4.2/setup.cfg
+-rwxr-xr-x   0 hujian     (501) staff       (20)     1592 2024-04-12 08:23:43.000000 jhu-1.4.2/setup.py
```

### Comparing `jhu-1.4.1/LICENSE` & `jhu-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jhu-1.4.1/PKG-INFO` & `jhu-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.1
+Version: 1.4.2
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `jhu-1.4.1/README.md` & `jhu-1.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # JHU(Join Happy Utils)
 > 这个是我自己编写的一个python工具库,简化或者自动化的帮助我做一些工作
 
 # ChangeLog
+## V1.4.2(2024-04-12)
+### security.py
+- 整合了HashAPI和AESAPI的解密功能
+
 ## V1.4.1(2024-04-10)
 ### security.py
 - 废弃fernetAPI,改为AESAPI,并采用ECB模式; 同样的明文加密后的内容是一致的
 
 ## V1.4.0(2024-04-09)
 ### security.py
 - 追加了对称加密
```

### Comparing `jhu-1.4.1/jhu/auth.py` & `jhu-1.4.2/jhu/auth.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.1/jhu/email.py` & `jhu-1.4.2/jhu/email.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.1/jhu/security.py` & `jhu-1.4.2/jhu/security.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,72 +9,55 @@
 from Cryptodome.Util.Padding import pad,unpad
 from jose import jwt
 
 
 class AESAPI:
     def __init__(self,key:str) -> None:
         # ECB模式,加密结果固定
-        self.cipher = AES.new(key.encode(),AES.MODE_ECB)
+        self._cipher = AES.new(key.encode(),AES.MODE_ECB)
     
-    def encrypt(self,plain_text:str):
-        """加密
+    @property
+    def cipher(self):
+        return self._cipher
+    
+    def encrypt(self,plain_text:str)->str:
+        """加密:pad->encrypt->b64encode
         """
 
         # 对明文进行补全至块大小的填充
         padded_text = pad(plain_text.encode(), AES.block_size)
 
         # 加密
         ciphertext = self.cipher.encrypt(padded_text)
 
         # 返回Base64编码的密文
         return b64encode(ciphertext).decode()
     
-    def decrypt(self,encrypted_value:str):
-        """解密
+    def decrypt(self,encrypted_value:str)->str:
+        """解密:b64decode->decrypt->unpad
         """
 
         # 将Base64编码的密文解码为字节
-        ciphertext = b64decode(encrypted_value.encode())
+        ciphertext = b64decode(encrypted_value)
 
         # 解密
         decrypted_text = unpad(self.cipher.decrypt(ciphertext), AES.block_size)
 
         # 将解密后的字节串转换回字符串
-        original_message = decrypted_text.decode()
+        return decrypted_text.decode()
 
-        return original_message
-        
-class HashAPI:
-    def __init__(self,key:str) -> None:
-       """Hash对象
-       
-       Args:
-        key:str,加密密钥
-       """
-       self.__key = key
 
-    @property
-    def key(self):
-       return self.__key
-    
-    def hash_text(self,plain_text:str)->str:
-        """将明文哈希加密
+class HashAPI:
+    def hash(self,plain_text:str)->str:
+        """明文哈希加密
         """
         return hashpw(plain_text.encode(),gensalt()).decode()
-
-    def decrypt(self,hash_text:str)->str:
-        """解密哈希文本
-        """
-        cipher = AES.new(self.key.encode(),AES.MODE_ECB)
-        enc_text = b64decode(hash_text)
-        dec_text = unpad(cipher.decrypt(enc_text),AES.block_size).decode()
-        return dec_text
-
-    def verifty(self,plain_text:str,hash_text:str)->bool:
-        """验证明文文本和哈希加密文本内容是否一致
+    
+    def verify(self,plain_text:str,hash_text:str)->bool:
+        """验证明文和密文的内容是否一致
         """
         return checkpw(plain_text.encode(),hash_text.encode())
 
 
 class JWTAPI:
     def __init__(self,key:str,expire_min:int,algorithm:str='HS256') -> None:
         """JWT对象
```

### Comparing `jhu-1.4.1/jhu/webhook.py` & `jhu-1.4.2/jhu/webhook.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.1/jhu.egg-info/PKG-INFO` & `jhu-1.4.2/jhu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.1
+Version: 1.4.2
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `jhu-1.4.1/setup.py` & `jhu-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     password = # 这里改成放申请下来的token
 6. twine upload dist/* 可上传安装,需要输入pypi的用户名和密码
 """
 from setuptools import setup, find_packages
 
 setup(
     name='jhu',  # 包的名称
-    version='1.4.1',  # 包的版本,每次更新或升级包都需要更新它
+    version='1.4.2',  # 包的版本,每次更新或升级包都需要更新它
     description='jhu是一个工具包,简化或自动化的做一些任务',  # 包的描述
     author='J.Hu',  # 作者
     email='joestarhu@163.com',  # 作者邮箱
     url='https://github.com/joestarhu/jhu',  # 项目地址
     packages=find_packages(
         exclude=['test', 'examples', 'script', 'tutorials']),   # 包内不需要引用的文件
     classifiers=[
```

