# Comparing `tmp/ERA_V2_Architecture-0.1.4.tar.gz` & `tmp/ERA_V2_Architecture-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERA_V2_Architecture-0.1.4.tar", last modified: Fri Apr 12 11:59:09 2024, max compression
+gzip compressed data, was "ERA_V2_Architecture-0.1.5.tar", last modified: Fri Apr 12 13:01:55 2024, max compression
```

## Comparing `ERA_V2_Architecture-0.1.4.tar` & `ERA_V2_Architecture-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.496620 ERA_V2_Architecture-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.418750 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/
--rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.480258 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/
--rw-rw-rw-   0        0        0      107 2024-04-11 11:51:53.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/__init__.py
--rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/models.py
--rw-rw-rw-   0        0        0     3061 2024-04-12 11:56:27.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/resnet.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:59:09.480258 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/
--rw-rw-rw-   0        0        0      473 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-12 11:59:09.000000 ERA_V2_Architecture-0.1.4/ERA_V2_Architecture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-12 11:59:09.494788 ERA_V2_Architecture-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 11:59:09.496620 ERA_V2_Architecture-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-12 11:56:39.000000 ERA_V2_Architecture-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:01:55.411123 ERA_V2_Architecture-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:01:55.373884 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/
+-rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:01:55.407244 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/
+-rw-rw-rw-   0        0        0      651 2024-04-12 13:00:58.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/CIFAR10Albumentations.py
+-rw-rw-rw-   0        0        0      309 2024-04-12 12:55:01.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/__init__.py
+-rw-rw-rw-   0        0        0     2947 2024-04-12 12:56:49.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/gradCAM.py
+-rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/models.py
+-rw-rw-rw-   0        0        0     3061 2024-04-12 11:56:27.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/resnet.py
+-rw-rw-rw-   0        0        0     2567 2024-04-12 12:49:51.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:01:55.409315 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-04-12 13:01:55.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-12 13:01:55.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:01:55.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-12 13:01:55.000000 ERA_V2_Architecture-0.1.5/ERA_V2_Architecture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-12 13:01:55.410107 ERA_V2_Architecture-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:01:55.411123 ERA_V2_Architecture-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-12 13:01:18.000000 ERA_V2_Architecture-0.1.5/setup.py
```

### Comparing `ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/models.py` & `ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/models.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.4/ERA_V2_Architecture/model/resnet.py` & `ERA_V2_Architecture-0.1.5/ERA_V2_Architecture/model/resnet.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.4/setup.py` & `ERA_V2_Architecture-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ERA_V2_Architecture",
-    version="0.1.4",
+    version="0.1.5",
     author="Xianping Wu",
     author_email="xianpingwu@hotmail.com",
     description="The ERA-V2 course network architectures",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url="https://github.com/ping-Mel/ERAV2-Architecture.git",
     packages=find_packages(),
```

