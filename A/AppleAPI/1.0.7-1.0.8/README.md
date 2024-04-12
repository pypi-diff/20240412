# Comparing `tmp/AppleAPI-1.0.7.tar.gz` & `tmp/AppleAPI-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppleAPI-1.0.7.tar", last modified: Sun Apr  7 08:20:29 2024, max compression
+gzip compressed data, was "AppleAPI-1.0.8.tar", last modified: Fri Apr 12 06:57:18 2024, max compression
```

## Comparing `AppleAPI-1.0.7.tar` & `AppleAPI-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:29.848033 AppleAPI-1.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:29.844033 AppleAPI-1.0.7/AppleAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/AppleAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/AppleAPI/apple_api_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14535 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/AppleAPI/appstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/AppleAPI/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:29.844033 AppleAPI-1.0.7/AppleAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:20:29.000000 AppleAPI-1.0.7/AppleAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 08:20:29.000000 AppleAPI-1.0.7/AppleAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:20:29.000000 AppleAPI-1.0.7/AppleAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:20:29.000000 AppleAPI-1.0.7/AppleAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 08:20:29.000000 AppleAPI-1.0.7/AppleAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:20:29.844033 AppleAPI-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:20:29.848033 AppleAPI-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 08:20:25.000000 AppleAPI-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:57:18.258393 AppleAPI-1.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:57:18.254393 AppleAPI-1.0.8/AppleAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/AppleAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/AppleAPI/apple_api_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/AppleAPI/appstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/AppleAPI/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:57:18.254393 AppleAPI-1.0.8/AppleAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 06:57:18.000000 AppleAPI-1.0.8/AppleAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 06:57:18.000000 AppleAPI-1.0.8/AppleAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:57:18.000000 AppleAPI-1.0.8/AppleAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 06:57:18.000000 AppleAPI-1.0.8/AppleAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 06:57:18.000000 AppleAPI-1.0.8/AppleAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 06:57:18.258393 AppleAPI-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:57:18.258393 AppleAPI-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-12 06:57:14.000000 AppleAPI-1.0.8/setup.py
```

### Comparing `AppleAPI-1.0.7/AppleAPI/apple_api_agent.py` & `AppleAPI-1.0.8/AppleAPI/apple_api_agent.py`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.7/AppleAPI/appstore.py` & `AppleAPI-1.0.8/AppleAPI/appstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
         resourceIds = self.agent.list_appstore_version(appleId, filters={"versionString":appstore_version, "platform":"IOS"})
         if resourceIds:
             resourceId = resourceIds[0].id
         else:
             die("未找到资源id")
         print(f"资源id:{resourceId}")
         locale_list = self.agent.list_localization(resourceId)
+        print(f"本地化语言：{locale_list}")
         for (local,screenshotDic) in screenshots.items():
             in_locals = list(filter(lambda item: item.locale.lower() == local.lower(), locale_list))
             if not in_locals:
                 select_local = self.agent.create_localization(resourceId, local)
                 print(f"创建App本地化语言：{local}")
             else:
                 select_local = in_locals[0]
@@ -305,15 +306,15 @@
                     screenshots = self.agent.list_app_screenshot(set_id)
                     if screenshots:
                         # 删除所有已存在截图
                         for item in screenshots:
                             self.agent.delete_app_screenshot(item.id)
                 else:
                     print(f'未找到 {screenshotType} 截图集，准备创建')
-                    set_id = self.agent.create_app_screenshot_set(select_local.id, screenshotType)
+                    set_id = self.agent.create_app_screenshot_set(select_local.id, screenshotType.name)
  
                 retry = 0
                 # 获取dir下的所有图片文件路径
                 for file in Path(dir).iterdir():
                     if file.is_file() and file.suffix.lower() in ['.png', '.jpg', '.jpeg']:
                         screenshot = self.agent.create_app_screenshot(set_id, file)
                         while True:
```

### Comparing `AppleAPI-1.0.7/AppleAPI/models.py` & `AppleAPI-1.0.8/AppleAPI/models.py`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.7/AppleAPI.egg-info/PKG-INFO` & `AppleAPI-1.0.8/AppleAPI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,15 +49,14 @@
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXX
     -----END PRIVATE KEY----- 
     """
 
-    app = AppStore(issuer_id, key_id, key)
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
@@ -72,14 +71,15 @@
         }
     }   
     devices = {
         'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx设备id' : '设备名称(可选)，比如：iphone6s'
     }
     # https://developer.apple.com/documentation/appstoreconnectapi/capabilitytype
     capabilitys = ['ASSOCIATED_DOMAINS'] # APPLE_ID_AUTH
+    app = AppStore(issuer_id, key_id, key, save_fold_name=email)
     # 创建Bundle Id
     app.create_bundle_id(bundle_id=bundle_id, bundle_name=name, capabilitys=capabilitys)
     # 添加测试设备
     app.add_devices(devices=devices)
     # 创建证书
     app.create_certificate(is_dev=False, email=email, developer_name=developer_name, password=password, country=country)
     # 创建描述文件
```

### Comparing `AppleAPI-1.0.7/LICENSE` & `AppleAPI-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.7/PKG-INFO` & `AppleAPI-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -49,15 +49,14 @@
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXX
     -----END PRIVATE KEY----- 
     """
 
-    app = AppStore(issuer_id, key_id, key)
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
@@ -72,14 +71,15 @@
         }
     }   
     devices = {
         'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx设备id' : '设备名称(可选)，比如：iphone6s'
     }
     # https://developer.apple.com/documentation/appstoreconnectapi/capabilitytype
     capabilitys = ['ASSOCIATED_DOMAINS'] # APPLE_ID_AUTH
+    app = AppStore(issuer_id, key_id, key, save_fold_name=email)
     # 创建Bundle Id
     app.create_bundle_id(bundle_id=bundle_id, bundle_name=name, capabilitys=capabilitys)
     # 添加测试设备
     app.add_devices(devices=devices)
     # 创建证书
     app.create_certificate(is_dev=False, email=email, developer_name=developer_name, password=password, country=country)
     # 创建描述文件
```

### Comparing `AppleAPI-1.0.7/README.md` & `AppleAPI-1.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
     XXXXXXXX
     -----END PRIVATE KEY----- 
     """
 
-    app = AppStore(issuer_id, key_id, key)
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
@@ -50,14 +49,15 @@
         }
     }   
     devices = {
         'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx设备id' : '设备名称(可选)，比如：iphone6s'
     }
     # https://developer.apple.com/documentation/appstoreconnectapi/capabilitytype
     capabilitys = ['ASSOCIATED_DOMAINS'] # APPLE_ID_AUTH
+    app = AppStore(issuer_id, key_id, key, save_fold_name=email)
     # 创建Bundle Id
     app.create_bundle_id(bundle_id=bundle_id, bundle_name=name, capabilitys=capabilitys)
     # 添加测试设备
     app.add_devices(devices=devices)
     # 创建证书
     app.create_certificate(is_dev=False, email=email, developer_name=developer_name, password=password, country=country)
     # 创建描述文件
```

### Comparing `AppleAPI-1.0.7/setup.py` & `AppleAPI-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='AppleAPI',  # 包名字
-    version='1.0.7',  # 包版本
+    version='1.0.8',  # 包版本
     author='影孤清',  # 作者
     author_email='yingguqing@163.com',  # 作者邮箱
     keywords='ios apple appstore app store connect api appstoreconnectapi',
     description='App Store Connect API',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yingguqing/AppleAPI',  # 包的主页
```

