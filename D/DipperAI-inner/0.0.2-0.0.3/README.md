# Comparing `tmp/DipperAI-inner-0.0.2.tar.gz` & `tmp/DipperAI-inner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DipperAI-inner-0.0.2.tar", last modified: Fri Apr 12 12:52:47 2024, max compression
+gzip compressed data, was "DipperAI-inner-0.0.3.tar", last modified: Fri Apr 12 13:22:27 2024, max compression
```

## Comparing `DipperAI-inner-0.0.2.tar` & `DipperAI-inner-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.136443 DipperAI-inner-0.0.2/
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.127071 DipperAI-inner-0.0.2/DipperAI_inner/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/__init__.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.131286 DipperAI-inner-0.0.2/DipperAI_inner/maas/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/aigcaas.py
--rw-r--r--   0 wangjia    (502) staff       (20)     7457 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/core.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2569 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/huggingface.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2306 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/modelscope.py
--rw-r--r--   0 wangjia    (502) staff       (20)      113 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/main.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.131775 DipperAI-inner-0.0.2/DipperAI_inner/resources/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:47.000000 DipperAI-inner-0.0.2/DipperAI_inner/resources/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/resources/config.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.132827 DipperAI-inner-0.0.2/DipperAI_inner/utils/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:35.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2439 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/cache.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/common.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2258 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/logger.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.135679 DipperAI-inner-0.0.2/DipperAI_inner/vendor/
--rw-r--r--   0 wangjia    (502) staff       (20)       29 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)    10767 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/alibaba.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/aws.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/local.py
--rw-r--r--   0 wangjia    (502) staff       (20)       55 2024-04-12 12:51:59.000000 DipperAI-inner-0.0.2/DipperAI_inner/version.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.129540 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/
--rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/PKG-INFO
--rw-r--r--   0 wangjia    (502) staff       (20)      787 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/SOURCES.txt
--rw-r--r--   0 wangjia    (502) staff       (20)        1 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/dependency_links.txt
--rw-r--r--   0 wangjia    (502) staff       (20)       63 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/requires.txt
--rw-r--r--   0 wangjia    (502) staff       (20)       15 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/top_level.txt
--rw-r--r--   0 wangjia    (502) staff       (20)     1087 2024-04-12 09:49:12.000000 DipperAI-inner-0.0.2/LICENSE
--rw-r--r--   0 wangjia    (502) staff       (20)       41 2024-04-12 12:47:27.000000 DipperAI-inner-0.0.2/MANIFEST.in
--rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:52:47.136028 DipperAI-inner-0.0.2/PKG-INFO
--rw-r--r--   0 wangjia    (502) staff       (20)     2338 2024-04-12 09:46:54.000000 DipperAI-inner-0.0.2/README.md
--rw-r--r--   0 wangjia    (502) staff       (20)       38 2024-04-12 12:52:47.136493 DipperAI-inner-0.0.2/setup.cfg
--rw-r--r--   0 wangjia    (502) staff       (20)     3688 2024-04-12 12:50:55.000000 DipperAI-inner-0.0.2/setup.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.956482 DipperAI-inner-0.0.3/
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.950495 DipperAI-inner-0.0.3/DipperAI_inner/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/__init__.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.953100 DipperAI-inner-0.0.3/DipperAI_inner/maas/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/maas/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/maas/aigcaas.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     7472 2024-04-12 13:21:27.000000 DipperAI-inner-0.0.3/DipperAI_inner/maas/core.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2584 2024-04-12 13:21:05.000000 DipperAI-inner-0.0.3/DipperAI_inner/maas/huggingface.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2306 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/maas/modelscope.py
+-rw-r--r--   0 wangjia    (502) staff       (20)      113 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/main.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.953702 DipperAI-inner-0.0.3/DipperAI_inner/resources/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:47.000000 DipperAI-inner-0.0.3/DipperAI_inner/resources/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/resources/config.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.954830 DipperAI-inner-0.0.3/DipperAI_inner/utils/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:35.000000 DipperAI-inner-0.0.3/DipperAI_inner/utils/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2439 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/utils/cache.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/utils/common.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2258 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/utils/logger.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.955829 DipperAI-inner-0.0.3/DipperAI_inner/vendor/
+-rw-r--r--   0 wangjia    (502) staff       (20)       29 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/vendor/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)    10767 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/vendor/alibaba.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/vendor/aws.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.3/DipperAI_inner/vendor/local.py
+-rw-r--r--   0 wangjia    (502) staff       (20)       55 2024-04-12 12:51:59.000000 DipperAI-inner-0.0.3/DipperAI_inner/version.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 13:22:27.951763 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 13:22:27.000000 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/PKG-INFO
+-rw-r--r--   0 wangjia    (502) staff       (20)      787 2024-04-12 13:22:27.000000 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)        1 2024-04-12 13:22:27.000000 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)       63 2024-04-12 13:22:27.000000 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/requires.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)       15 2024-04-12 13:22:27.000000 DipperAI-inner-0.0.3/DipperAI_inner.egg-info/top_level.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)     1087 2024-04-12 09:49:12.000000 DipperAI-inner-0.0.3/LICENSE
+-rw-r--r--   0 wangjia    (502) staff       (20)       41 2024-04-12 12:47:27.000000 DipperAI-inner-0.0.3/MANIFEST.in
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 13:22:27.956193 DipperAI-inner-0.0.3/PKG-INFO
+-rw-r--r--   0 wangjia    (502) staff       (20)     2338 2024-04-12 09:46:54.000000 DipperAI-inner-0.0.3/README.md
+-rw-r--r--   0 wangjia    (502) staff       (20)       38 2024-04-12 13:22:27.956543 DipperAI-inner-0.0.3/setup.cfg
+-rw-r--r--   0 wangjia    (502) staff       (20)     3688 2024-04-12 13:22:04.000000 DipperAI-inner-0.0.3/setup.py
```

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/maas/core.py` & `DipperAI-inner-0.0.3/DipperAI_inner/maas/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def get_service_config(self, user_config: dict) -> dict:
         """
         get service config
         :return: dict
         """
         # 补充配置
         config_func_name = self.get_config_func_name()
-        lib_module = importlib.import_module('resources.config')
+        lib_module = importlib.import_module('DipperAI_inner.resources.config')
         return getattr(lib_module, config_func_name)(user_config)
 
     def get_model_meta(self) -> dict:
         """
         the MaaS module needs to rewrite this method, primarily for handling the model_url.
         It involves parsing the model_url to extract the model_id and model_version.
         :return: dict
```

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/maas/huggingface.py` & `DipperAI-inner-0.0.3/DipperAI_inner/maas/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def get_service_config(self, user_config: dict) -> dict:
         """
         get service config
         :return: dict
         """
         # 补充配置
         config_func_name = self.get_config_func_name()
-        lib_module = importlib.import_module('resources.config')
+        lib_module = importlib.import_module('DipperAI_inner.resources.config')
         return getattr(lib_module, config_func_name)(user_config, name=self.get_resource_name(),
             model_id=self.model_id, model_task=self.__get_task(), access_token=self.access_token, library=self.__get_library())
 
     def __get_library(self) -> str:
         """
         获取模型库地址
         """
```

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/maas/modelscope.py` & `DipperAI-inner-0.0.3/DipperAI_inner/maas/modelscope.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/resources/config.py` & `DipperAI-inner-0.0.3/DipperAI_inner/resources/config.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/utils/cache.py` & `DipperAI-inner-0.0.3/DipperAI_inner/utils/cache.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/utils/logger.py` & `DipperAI-inner-0.0.3/DipperAI_inner/utils/logger.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner/vendor/alibaba.py` & `DipperAI-inner-0.0.3/DipperAI_inner/vendor/alibaba.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner.egg-info/PKG-INFO` & `DipperAI-inner-0.0.3/DipperAI_inner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DipperAI-inner
-Version: 0.0.2
+Version: 0.0.3
 Summary: DipperAI inner package
 Home-page: https://github.com/DipperAI/DipperAI
 Author: jiaw127
 Author-email: jiaw127@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `DipperAI-inner-0.0.2/DipperAI_inner.egg-info/SOURCES.txt` & `DipperAI-inner-0.0.3/DipperAI_inner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/LICENSE` & `DipperAI-inner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/PKG-INFO` & `DipperAI-inner-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DipperAI-inner
-Version: 0.0.2
+Version: 0.0.3
 Summary: DipperAI inner package
 Home-page: https://github.com/DipperAI/DipperAI
 Author: jiaw127
 Author-email: jiaw127@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `DipperAI-inner-0.0.2/README.md` & `DipperAI-inner-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.2/setup.py` & `DipperAI-inner-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'DipperAI-inner'
 DESCRIPTION = 'DipperAI inner package'
 URL = 'https://github.com/DipperAI/DipperAI'
 EMAIL = 'jiaw127@163.com'
 AUTHOR = 'jiaw127'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "colorama==0.4.6",
     "Requests==2.31.0",
     "ruff==0.2.2",
     "pre-commit==3.6.2"
```

