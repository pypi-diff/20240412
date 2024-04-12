# Comparing `tmp/signapse-1.0.13.tar.gz` & `tmp/signapse-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.13.tar", last modified: Thu Apr 11 11:38:47 2024, max compression
+gzip compressed data, was "signapse-1.0.14.tar", last modified: Fri Apr 12 10:24:17 2024, max compression
```

## Comparing `signapse-1.0.13.tar` & `signapse-1.0.14.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:47.000000 signapse-1.0.13/
--rw-rw-r--   0     1001     1001     1065 2024-04-04 10:20:56.000000 signapse-1.0.13/LICENSE.txt
--rw-r--r--   0     1001     1001     2769 2024-04-11 11:38:47.000000 signapse-1.0.13/PKG-INFO
--rw-rw-r--   0     1001     1001     1637 2024-04-05 09:17:43.000000 signapse-1.0.13/README.md
--rw-r--r--   0     1001     1001       38 2024-04-11 11:38:47.000000 signapse-1.0.13/setup.cfg
--rw-rw-r--   0     1001     1001     1395 2024-04-11 11:37:03.000000 signapse-1.0.13/setup.py
-drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:46.000000 signapse-1.0.13/signapse/
--rw-rw-r--   0     1001     1001      463 2024-04-04 11:18:15.000000 signapse-1.0.13/signapse/__init__.py
--rw-rw-r--   0     1001     1001     6566 2024-04-09 10:40:55.000000 signapse-1.0.13/signapse/build_opt.py
--rw-rw-r--   0     1001     1001     9366 2024-04-08 14:49:55.000000 signapse-1.0.13/signapse/compute.py
--rw-rw-r--   0     1001     1001     2662 2024-04-04 10:51:14.000000 signapse-1.0.13/signapse/constants.py
--rw-rw-r--   0     1001     1001     7511 2024-04-08 15:02:14.000000 signapse-1.0.13/signapse/create.py
--rw-rw-r--   0     1001     1001     1225 2024-04-04 11:11:01.000000 signapse-1.0.13/signapse/create_model.py
--rw-rw-r--   0     1001     1001    21879 2024-04-08 10:17:01.000000 signapse-1.0.13/signapse/heatmaps.py
--rw-rw-r--   0     1001     1001     4652 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/lang_sam.py
--rw-rw-r--   0     1001     1001     4444 2024-04-08 10:09:21.000000 signapse-1.0.13/signapse/lang_utils.py
--rw-rw-r--   0     1001     1001    17696 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/models_utils.py
--rw-rw-r--   0     1001     1001     3888 2024-04-04 14:23:34.000000 signapse-1.0.13/signapse/mp_utils.py
--rw-rw-r--   0     1001     1001     5793 2024-04-09 10:56:58.000000 signapse-1.0.13/signapse/poses.py
--rw-rw-r--   0     1001     1001     3403 2024-04-09 10:57:12.000000 signapse-1.0.13/signapse/preprocessing.py
--rw-rw-r--   0     1001     1001     2610 2023-12-03 23:04:06.000000 signapse-1.0.13/signapse/utils.py
-drwxr-xr-x   0     1001     1001        0 2024-04-11 11:38:46.000000 signapse-1.0.13/signapse.egg-info/
--rw-r--r--   0     1001     1001     2769 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/PKG-INFO
--rw-r--r--   0     1001     1001      491 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/SOURCES.txt
--rw-r--r--   0     1001     1001        1 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/dependency_links.txt
--rw-r--r--   0     1001     1001      300 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/requires.txt
--rw-r--r--   0     1001     1001        9 2024-04-11 11:38:42.000000 signapse-1.0.13/signapse.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2024-04-12 10:24:17.000000 signapse-1.0.14/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2712 2024-04-12 10:24:17.000000 signapse-1.0.14/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     1637 2024-04-05 09:17:43.000000 signapse-1.0.14/README.md
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2024-04-12 10:24:17.000000 signapse-1.0.14/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     1396 2024-04-12 10:23:25.000000 signapse-1.0.14/setup.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2024-04-12 10:24:15.000000 signapse-1.0.14/signapse/
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      463 2024-04-04 11:18:15.000000 signapse-1.0.14/signapse/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6566 2024-04-09 10:40:55.000000 signapse-1.0.14/signapse/build_opt.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     9366 2024-04-08 14:49:55.000000 signapse-1.0.14/signapse/compute.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2662 2024-04-04 10:51:14.000000 signapse-1.0.14/signapse/constants.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7511 2024-04-08 15:02:14.000000 signapse-1.0.14/signapse/create.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     1225 2024-04-04 11:11:01.000000 signapse-1.0.14/signapse/create_model.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    21879 2024-04-08 10:17:01.000000 signapse-1.0.14/signapse/heatmaps.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4652 2023-12-03 23:04:06.000000 signapse-1.0.14/signapse/lang_sam.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4444 2024-04-08 10:09:21.000000 signapse-1.0.14/signapse/lang_utils.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    17696 2023-12-03 23:04:06.000000 signapse-1.0.14/signapse/models_utils.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3888 2024-04-04 14:23:34.000000 signapse-1.0.14/signapse/mp_utils.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5793 2024-04-09 10:56:58.000000 signapse-1.0.14/signapse/poses.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3403 2024-04-09 10:57:12.000000 signapse-1.0.14/signapse/preprocessing.py
+-rw-rw-r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2610 2023-12-03 23:04:06.000000 signapse-1.0.14/signapse/utils.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2024-04-12 10:24:16.000000 signapse-1.0.14/signapse.egg-info/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2712 2024-04-12 10:24:10.000000 signapse-1.0.14/signapse.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      479 2024-04-12 10:24:11.000000 signapse-1.0.14/signapse.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2024-04-12 10:24:11.000000 signapse-1.0.14/signapse.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      284 2024-04-12 10:24:11.000000 signapse-1.0.14/signapse.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        9 2024-04-12 10:24:11.000000 signapse-1.0.14/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.13/PKG-INFO` & `signapse-1.0.14/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.13
+Version: 1.0.14
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
 Requires-Dist: essentials
 Requires-Dist: setuptools
 Requires-Dist: wheel==0.38.4
 Requires-Dist: mediapipe==0.10.3
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: opencv-python-headless==4.7.0.72
 Requires-Dist: pandas==2.0.3
-Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
 Requires-Dist: torch==1.11.0
 Requires-Dist: torchvision==0.12.0
```

### Comparing `signapse-1.0.13/README.md` & `signapse-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/setup.py` & `signapse-1.0.14/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.13',
+    version='1.0.14',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
@@ -25,15 +25,15 @@
         'essentials',
         'setuptools',
         'wheel==0.38.4',
         'mediapipe==0.10.3',
         'opencv-python==4.7.0.72',
         'opencv-python-headless==4.7.0.72',
         'pandas==2.0.3',
-        'pickle5==0.0.11',
+    #    'pickle5==0.0.11',
         'protobuf==3.20.*',
         'boto3 == 1.24.47',
         'ffmpeg-python == 0.2.0',
         'scipy == 1.8,',
         'pycpd==2.0.0',
     #    'torch==1.11.0+cu113',
     #    'torchvision==0.12.0+cu113',
```

### Comparing `signapse-1.0.13/signapse/build_opt.py` & `signapse-1.0.14/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/compute.py` & `signapse-1.0.14/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/constants.py` & `signapse-1.0.14/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/create.py` & `signapse-1.0.14/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/create_model.py` & `signapse-1.0.14/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/heatmaps.py` & `signapse-1.0.14/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/lang_sam.py` & `signapse-1.0.14/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/lang_utils.py` & `signapse-1.0.14/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/models_utils.py` & `signapse-1.0.14/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/mp_utils.py` & `signapse-1.0.14/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/poses.py` & `signapse-1.0.14/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/preprocessing.py` & `signapse-1.0.14/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse/utils.py` & `signapse-1.0.14/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.13/signapse.egg-info/PKG-INFO` & `signapse-1.0.14/signapse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.13
+Version: 1.0.14
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
 Requires-Dist: essentials
 Requires-Dist: setuptools
 Requires-Dist: wheel==0.38.4
 Requires-Dist: mediapipe==0.10.3
 Requires-Dist: opencv-python==4.7.0.72
 Requires-Dist: opencv-python-headless==4.7.0.72
 Requires-Dist: pandas==2.0.3
-Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
 Requires-Dist: torch==1.11.0
 Requires-Dist: torchvision==0.12.0
```

