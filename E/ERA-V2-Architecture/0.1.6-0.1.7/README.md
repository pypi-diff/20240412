# Comparing `tmp/ERA_V2_Architecture-0.1.6.tar.gz` & `tmp/ERA_V2_Architecture-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERA_V2_Architecture-0.1.6.tar", last modified: Fri Apr 12 13:46:17 2024, max compression
+gzip compressed data, was "ERA_V2_Architecture-0.1.7.tar", last modified: Fri Apr 12 13:51:18 2024, max compression
```

## Comparing `ERA_V2_Architecture-0.1.6.tar` & `ERA_V2_Architecture-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:17.729822 ERA_V2_Architecture-0.1.6/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:17.654173 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/
--rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:17.724725 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/
--rw-rw-rw-   0        0        0      711 2024-04-12 13:44:23.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/CIFAR10Albumentations.py
--rw-rw-rw-   0        0        0      377 2024-04-12 13:45:34.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/__init__.py
--rw-rw-rw-   0        0        0     2947 2024-04-12 12:56:49.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/gradCAM.py
--rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/models.py
--rw-rw-rw-   0        0        0     3061 2024-04-12 11:56:27.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/resnet.py
--rw-rw-rw-   0        0        0     4140 2024-04-12 13:44:59.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/util.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:17.726828 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture.egg-info/
--rw-rw-rw-   0        0        0      473 2024-04-12 13:46:17.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-04-12 13:46:17.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:46:17.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-12 13:46:17.000000 ERA_V2_Architecture-0.1.6/ERA_V2_Architecture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-12 13:46:17.727830 ERA_V2_Architecture-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 13:46:17.729877 ERA_V2_Architecture-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-12 13:46:02.000000 ERA_V2_Architecture-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:51:18.392009 ERA_V2_Architecture-0.1.7/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:51:18.339693 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/
+-rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:51:18.386927 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/
+-rw-rw-rw-   0        0        0      711 2024-04-12 13:44:23.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/CIFAR10Albumentations.py
+-rw-rw-rw-   0        0        0      377 2024-04-12 13:45:34.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/__init__.py
+-rw-rw-rw-   0        0        0     2947 2024-04-12 12:56:49.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/gradCAM.py
+-rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/models.py
+-rw-rw-rw-   0        0        0     3061 2024-04-12 11:56:27.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/resnet.py
+-rw-rw-rw-   0        0        0     4200 2024-04-12 13:49:58.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:51:18.388923 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-04-12 13:51:18.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-12 13:51:18.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:51:18.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-12 13:51:18.000000 ERA_V2_Architecture-0.1.7/ERA_V2_Architecture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-12 13:51:18.390796 ERA_V2_Architecture-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:51:18.392009 ERA_V2_Architecture-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-12 13:50:16.000000 ERA_V2_Architecture-0.1.7/setup.py
```

### Comparing `ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/CIFAR10Albumentations.py` & `ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/CIFAR10Albumentations.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/gradCAM.py` & `ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/gradCAM.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/models.py` & `ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/models.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/resnet.py` & `ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/resnet.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.6/ERA_V2_Architecture/model/util.py` & `ERA_V2_Architecture-0.1.7/ERA_V2_Architecture/model/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from torchvision import datasets
 from torch.utils.data import DataLoader
 import torch.nn.functional as F
 from tqdm import tqdm
 import albumentations as A
 from albumentations.pytorch import ToTensorV2
 from torchvision import transforms
+from .CIFAR10Albumentations import CIFAR10Albumentations
+
 
 def initialize_device(seed=1):
     use_cuda = torch.cuda.is_available()
     print("CUDA Available?", use_cuda)
     torch.manual_seed(seed)
     if use_cuda:
         torch.cuda.manual_seed(seed)
```

### Comparing `ERA_V2_Architecture-0.1.6/setup.py` & `ERA_V2_Architecture-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ERA_V2_Architecture",
-    version="0.1.6",
+    version="0.1.7",
     author="Xianping Wu",
     author_email="xianpingwu@hotmail.com",
     description="The ERA-V2 course network architectures",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url="https://github.com/ping-Mel/ERAV2-Architecture.git",
     packages=find_packages(),
```

