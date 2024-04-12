# Comparing `tmp/DipperAI-inner-0.0.1.tar.gz` & `tmp/DipperAI-inner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DipperAI-inner-0.0.1.tar", last modified: Fri Apr 12 12:23:33 2024, max compression
+gzip compressed data, was "DipperAI-inner-0.0.2.tar", last modified: Fri Apr 12 12:52:47 2024, max compression
```

## Comparing `DipperAI-inner-0.0.1.tar` & `DipperAI-inner-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:23:33.357093 DipperAI-inner-0.0.1/
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:23:33.351702 DipperAI-inner-0.0.1/DipperAI_inner/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/__init__.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:23:33.354874 DipperAI-inner-0.0.1/DipperAI_inner/maas/
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/maas/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/maas/aigcaas.py
--rw-r--r--   0 wangjia    (502) staff       (20)     7457 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/maas/core.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2569 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/maas/huggingface.py
--rw-r--r--   0 wangjia    (502) staff       (20)     2306 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/maas/modelscope.py
--rw-r--r--   0 wangjia    (502) staff       (20)      113 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/main.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:23:33.356049 DipperAI-inner-0.0.1/DipperAI_inner/vendor/
--rw-r--r--   0 wangjia    (502) staff       (20)       29 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/vendor/__init__.py
--rw-r--r--   0 wangjia    (502) staff       (20)    10767 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/vendor/alibaba.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/vendor/aws.py
--rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/vendor/local.py
--rw-r--r--   0 wangjia    (502) staff       (20)       55 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.1/DipperAI_inner/version.py
-drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:23:33.356405 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/
--rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:23:33.000000 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/PKG-INFO
--rw-r--r--   0 wangjia    (502) staff       (20)      590 2024-04-12 12:23:33.000000 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/SOURCES.txt
--rw-r--r--   0 wangjia    (502) staff       (20)        1 2024-04-12 12:23:33.000000 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/dependency_links.txt
--rw-r--r--   0 wangjia    (502) staff       (20)       63 2024-04-12 12:23:33.000000 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/requires.txt
--rw-r--r--   0 wangjia    (502) staff       (20)       15 2024-04-12 12:23:33.000000 DipperAI-inner-0.0.1/DipperAI_inner.egg-info/top_level.txt
--rw-r--r--   0 wangjia    (502) staff       (20)     1087 2024-04-12 09:49:12.000000 DipperAI-inner-0.0.1/LICENSE
--rw-r--r--   0 wangjia    (502) staff       (20)       26 2024-04-12 09:46:54.000000 DipperAI-inner-0.0.1/MANIFEST.in
--rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:23:33.356779 DipperAI-inner-0.0.1/PKG-INFO
--rw-r--r--   0 wangjia    (502) staff       (20)     2338 2024-04-12 09:46:54.000000 DipperAI-inner-0.0.1/README.md
--rw-r--r--   0 wangjia    (502) staff       (20)       38 2024-04-12 12:23:33.357147 DipperAI-inner-0.0.1/setup.cfg
--rw-r--r--   0 wangjia    (502) staff       (20)     3688 2024-04-12 12:19:49.000000 DipperAI-inner-0.0.1/setup.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.136443 DipperAI-inner-0.0.2/
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.127071 DipperAI-inner-0.0.2/DipperAI_inner/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/__init__.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.131286 DipperAI-inner-0.0.2/DipperAI_inner/maas/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/aigcaas.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     7457 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/core.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2569 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/huggingface.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2306 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/maas/modelscope.py
+-rw-r--r--   0 wangjia    (502) staff       (20)      113 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/main.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.131775 DipperAI-inner-0.0.2/DipperAI_inner/resources/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:47.000000 DipperAI-inner-0.0.2/DipperAI_inner/resources/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/resources/config.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.132827 DipperAI-inner-0.0.2/DipperAI_inner/utils/
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:49:35.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2439 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/cache.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/common.py
+-rw-r--r--   0 wangjia    (502) staff       (20)     2258 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/utils/logger.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.135679 DipperAI-inner-0.0.2/DipperAI_inner/vendor/
+-rw-r--r--   0 wangjia    (502) staff       (20)       29 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/__init__.py
+-rw-r--r--   0 wangjia    (502) staff       (20)    10767 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/alibaba.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/aws.py
+-rw-r--r--   0 wangjia    (502) staff       (20)        0 2024-04-12 12:17:58.000000 DipperAI-inner-0.0.2/DipperAI_inner/vendor/local.py
+-rw-r--r--   0 wangjia    (502) staff       (20)       55 2024-04-12 12:51:59.000000 DipperAI-inner-0.0.2/DipperAI_inner/version.py
+drwxr-xr-x   0 wangjia    (502) staff       (20)        0 2024-04-12 12:52:47.129540 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/PKG-INFO
+-rw-r--r--   0 wangjia    (502) staff       (20)      787 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)        1 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)       63 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/requires.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)       15 2024-04-12 12:52:47.000000 DipperAI-inner-0.0.2/DipperAI_inner.egg-info/top_level.txt
+-rw-r--r--   0 wangjia    (502) staff       (20)     1087 2024-04-12 09:49:12.000000 DipperAI-inner-0.0.2/LICENSE
+-rw-r--r--   0 wangjia    (502) staff       (20)       41 2024-04-12 12:47:27.000000 DipperAI-inner-0.0.2/MANIFEST.in
+-rw-r--r--   0 wangjia    (502) staff       (20)     2941 2024-04-12 12:52:47.136028 DipperAI-inner-0.0.2/PKG-INFO
+-rw-r--r--   0 wangjia    (502) staff       (20)     2338 2024-04-12 09:46:54.000000 DipperAI-inner-0.0.2/README.md
+-rw-r--r--   0 wangjia    (502) staff       (20)       38 2024-04-12 12:52:47.136493 DipperAI-inner-0.0.2/setup.cfg
+-rw-r--r--   0 wangjia    (502) staff       (20)     3688 2024-04-12 12:50:55.000000 DipperAI-inner-0.0.2/setup.py
```

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner/maas/core.py` & `DipperAI-inner-0.0.2/DipperAI_inner/maas/core.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner/maas/huggingface.py` & `DipperAI-inner-0.0.2/DipperAI_inner/maas/huggingface.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner/maas/modelscope.py` & `DipperAI-inner-0.0.2/DipperAI_inner/maas/modelscope.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner/vendor/alibaba.py` & `DipperAI-inner-0.0.2/DipperAI_inner/vendor/alibaba.py`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner.egg-info/PKG-INFO` & `DipperAI-inner-0.0.2/DipperAI_inner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DipperAI-inner
-Version: 0.0.1
+Version: 0.0.2
 Summary: DipperAI inner package
 Home-page: https://github.com/DipperAI/DipperAI
 Author: jiaw127
 Author-email: jiaw127@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `DipperAI-inner-0.0.1/DipperAI_inner.egg-info/SOURCES.txt` & `DipperAI-inner-0.0.2/DipperAI_inner.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,11 +11,17 @@
 DipperAI_inner.egg-info/requires.txt
 DipperAI_inner.egg-info/top_level.txt
 DipperAI_inner/maas/__init__.py
 DipperAI_inner/maas/aigcaas.py
 DipperAI_inner/maas/core.py
 DipperAI_inner/maas/huggingface.py
 DipperAI_inner/maas/modelscope.py
+DipperAI_inner/resources/__init__.py
+DipperAI_inner/resources/config.py
+DipperAI_inner/utils/__init__.py
+DipperAI_inner/utils/cache.py
+DipperAI_inner/utils/common.py
+DipperAI_inner/utils/logger.py
 DipperAI_inner/vendor/__init__.py
 DipperAI_inner/vendor/alibaba.py
 DipperAI_inner/vendor/aws.py
 DipperAI_inner/vendor/local.py
```

### Comparing `DipperAI-inner-0.0.1/LICENSE` & `DipperAI-inner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/PKG-INFO` & `DipperAI-inner-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DipperAI-inner
-Version: 0.0.1
+Version: 0.0.2
 Summary: DipperAI inner package
 Home-page: https://github.com/DipperAI/DipperAI
 Author: jiaw127
 Author-email: jiaw127@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `DipperAI-inner-0.0.1/README.md` & `DipperAI-inner-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `DipperAI-inner-0.0.1/setup.py` & `DipperAI-inner-0.0.2/setup.py`

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
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "colorama==0.4.6",
     "Requests==2.31.0",
     "ruff==0.2.2",
     "pre-commit==3.6.2"
```

