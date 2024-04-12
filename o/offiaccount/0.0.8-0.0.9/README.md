# Comparing `tmp/offiaccount-0.0.8.tar.gz` & `tmp/offiaccount-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offiaccount-0.0.8.tar", last modified: Sun Mar  3 12:14:33 2024, max compression
+gzip compressed data, was "offiaccount-0.0.9.tar", last modified: Fri Apr 12 17:51:40 2024, max compression
```

## Comparing `offiaccount-0.0.8.tar` & `offiaccount-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.342183 offiaccount-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-03 12:14:25.000000 offiaccount-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-03 12:14:33.342183 offiaccount-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-03 12:14:25.000000 offiaccount-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.338183 offiaccount-0.0.8/offiaccount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.338183 offiaccount-0.0.8/offiaccount/base/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/base/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.338183 offiaccount-0.0.8/offiaccount/draft/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/draft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/draft/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.342183 offiaccount-0.0.8/offiaccount/material/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/material/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.342183 offiaccount-0.0.8/offiaccount/publish/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/publish/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.342183 offiaccount-0.0.8/offiaccount/sendall/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/sendall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-03 12:14:25.000000 offiaccount-0.0.8/offiaccount/sendall/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 12:14:33.342183 offiaccount-0.0.8/offiaccount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-03 12:14:33.000000 offiaccount-0.0.8/offiaccount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-03 12:14:33.000000 offiaccount-0.0.8/offiaccount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 12:14:33.000000 offiaccount-0.0.8/offiaccount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-03 12:14:33.000000 offiaccount-0.0.8/offiaccount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-03 12:14:33.000000 offiaccount-0.0.8/offiaccount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 12:14:33.342183 offiaccount-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-03 12:14:25.000000 offiaccount-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-12 17:51:34.000000 offiaccount-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 17:51:40.157660 offiaccount-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 17:51:34.000000 offiaccount-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.153660 offiaccount-0.0.9/offiaccount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.153660 offiaccount-0.0.9/offiaccount/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/base/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/offiaccount/draft/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/draft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/draft/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/offiaccount/material/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/material/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/offiaccount/publish/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/publish/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/offiaccount/sendall/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/sendall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-12 17:51:34.000000 offiaccount-0.0.9/offiaccount/sendall/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:51:40.157660 offiaccount-0.0.9/offiaccount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 17:51:40.000000 offiaccount-0.0.9/offiaccount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 17:51:40.000000 offiaccount-0.0.9/offiaccount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:51:40.000000 offiaccount-0.0.9/offiaccount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 17:51:40.000000 offiaccount-0.0.9/offiaccount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 17:51:40.000000 offiaccount-0.0.9/offiaccount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:51:40.157660 offiaccount-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 17:51:34.000000 offiaccount-0.0.9/setup.py
```

### Comparing `offiaccount-0.0.8/LICENSE` & `offiaccount-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/PKG-INFO` & `offiaccount-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: offiaccount
-Version: 0.0.8
+Version: 0.0.9
 Summary: WeChat Official Account API
 Home-page: https://github.com/JiauZhang/offiaccount
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: WeChat,Official Account,WeChat API
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 
-### 生成 Token
 ```shell
-python3 get_token.py --appid YOUR_APPID --secret YOUR_SECRET
-# 输出的 ip 需要提前添加到白名单中，否则无法获取 token
-ip: YOUR_IP
-access_token: YOUR_ACCESS_TOKEN
+pip install offiaccount
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `offiaccount-0.0.8/offiaccount/base/api.py` & `offiaccount-0.0.9/offiaccount/base/api.py`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/offiaccount/base/tokenizer.py` & `offiaccount-0.0.9/offiaccount/base/tokenizer.py`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/offiaccount/draft/api.py` & `offiaccount-0.0.9/offiaccount/draft/api.py`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/offiaccount/material/api.py` & `offiaccount-0.0.9/offiaccount/material/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,22 @@
             'type': 'image',
             'access_token': self.access_token,
         }
         files = {'media': open(filename, 'rb')}
         r = self.client.post(add_url, params=params, files=files).json()
         return r
 
+    def delete(self, media_id):
+        # https://developers.weixin.qq.com/doc/offiaccount/Asset_Management/Deleting_Permanent_Assets.html
+        del_url = self.base_url + '/material/del_material'
+        params = {'access_token': self.access_token}
+        json = {'media_id': media_id}
+        r = self.client.post(del_url, params=params, json=json).json()
+        return r
+
     def get(self, media_id):
         get_url = self.base_url + '/get?access_token=' + self.access_token
         pass
 
     def batchget(self, type, offset=0, count=20):
         # https://developers.weixin.qq.com/doc/offiaccount/Asset_Management/Get_materials_list.html
         _type_allow_list = ['image', 'video', 'voice', 'news']
```

### Comparing `offiaccount-0.0.8/offiaccount/publish/api.py` & `offiaccount-0.0.9/offiaccount/publish/api.py`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/offiaccount.egg-info/PKG-INFO` & `offiaccount-0.0.9/offiaccount.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: offiaccount
-Version: 0.0.8
+Version: 0.0.9
 Summary: WeChat Official Account API
 Home-page: https://github.com/JiauZhang/offiaccount
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: WeChat,Official Account,WeChat API
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 
-### 生成 Token
 ```shell
-python3 get_token.py --appid YOUR_APPID --secret YOUR_SECRET
-# 输出的 ip 需要提前添加到白名单中，否则无法获取 token
-ip: YOUR_IP
-access_token: YOUR_ACCESS_TOKEN
+pip install offiaccount
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `offiaccount-0.0.8/offiaccount.egg-info/SOURCES.txt` & `offiaccount-0.0.9/offiaccount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `offiaccount-0.0.8/setup.py` & `offiaccount-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'offiaccount',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.8',
+    version = '0.0.9',
     license = 'GPL-2.0',
     description = 'WeChat Official Account API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/offiaccount',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

