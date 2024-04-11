# Comparing `tmp/AITracker-0.9.0.tar.gz` & `tmp/AITracker-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AITracker-0.9.0.tar", last modified: Thu Apr 11 22:06:04 2024, max compression
+gzip compressed data, was "AITracker-0.9.1.tar", last modified: Thu Apr 11 22:29:22 2024, max compression
```

## Comparing `AITracker-0.9.0.tar` & `AITracker-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:06:04.195915 AITracker-0.9.0/
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)    35148 2024-04-08 01:15:01.000000 AITracker-0.9.0/LICENSE.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2637 2024-04-11 22:06:04.195241 AITracker-0.9.0/PKG-INFO
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      635 2024-04-11 17:38:51.000000 AITracker-0.9.0/README.md
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1800 2024-04-11 22:05:51.000000 AITracker-0.9.0/pyproject.toml
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 22:06:04.196086 AITracker-0.9.0/setup.cfg
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:06:04.184463 AITracker-0.9.0/src/
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:06:04.190704 AITracker-0.9.0/src/AITracker/
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     6952 2024-04-11 20:42:46.000000 AITracker-0.9.0/src/AITracker/AITrackerModel.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2404 2024-04-10 20:07:39.000000 AITracker-0.9.0/src/AITracker/AITrackerNetwork.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     3823 2024-03-19 04:01:33.000000 AITracker-0.9.0/src/AITracker/DataValidation.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)    13617 2024-04-09 05:51:37.000000 AITracker-0.9.0/src/AITracker/UpdateH5.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 17:40:32.000000 AITracker-0.9.0/src/AITracker/__init__.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 20:42:01.000000 AITracker-0.9.0/src/AITracker/setup.py
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:06:04.194276 AITracker-0.9.0/src/AITracker.egg-info/
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2637 2024-04-11 22:06:04.000000 AITracker-0.9.0/src/AITracker.egg-info/PKG-INFO
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      393 2024-04-11 22:06:04.000000 AITracker-0.9.0/src/AITracker.egg-info/SOURCES.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)        1 2024-04-11 22:06:04.000000 AITracker-0.9.0/src/AITracker.egg-info/dependency_links.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      736 2024-04-11 22:06:04.000000 AITracker-0.9.0/src/AITracker.egg-info/requires.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)       10 2024-04-11 22:06:04.000000 AITracker-0.9.0/src/AITracker.egg-info/top_level.txt
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:29:22.666902 AITracker-0.9.1/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)    35148 2024-04-08 01:15:01.000000 AITracker-0.9.1/LICENSE.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 22:29:22.666216 AITracker-0.9.1/PKG-INFO
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      635 2024-04-11 17:38:51.000000 AITracker-0.9.1/README.md
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      937 2024-04-11 22:29:11.000000 AITracker-0.9.1/pyproject.toml
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 22:29:22.667131 AITracker-0.9.1/setup.cfg
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:29:22.654862 AITracker-0.9.1/src/
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:29:22.661857 AITracker-0.9.1/src/AITracker/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     6952 2024-04-11 20:42:46.000000 AITracker-0.9.1/src/AITracker/AITrackerModel.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2404 2024-04-10 20:07:39.000000 AITracker-0.9.1/src/AITracker/AITrackerNetwork.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     3823 2024-03-19 04:01:33.000000 AITracker-0.9.1/src/AITracker/DataValidation.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)    13617 2024-04-09 05:51:37.000000 AITracker-0.9.1/src/AITracker/UpdateH5.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 17:40:32.000000 AITracker-0.9.1/src/AITracker/__init__.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 20:42:01.000000 AITracker-0.9.1/src/AITracker/setup.py
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 22:29:22.665353 AITracker-0.9.1/src/AITracker.egg-info/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 22:29:22.000000 AITracker-0.9.1/src/AITracker.egg-info/PKG-INFO
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      393 2024-04-11 22:29:22.000000 AITracker-0.9.1/src/AITracker.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)        1 2024-04-11 22:29:22.000000 AITracker-0.9.1/src/AITracker.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      118 2024-04-11 22:29:22.000000 AITracker-0.9.1/src/AITracker.egg-info/requires.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)       10 2024-04-11 22:29:22.000000 AITracker-0.9.1/src/AITracker.egg-info/top_level.txt
```

### Comparing `AITracker-0.9.0/LICENSE.txt` & `AITracker-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/PKG-INFO` & `AITracker-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,29 @@
 Metadata-Version: 2.1
 Name: AITracker
-Version: 0.9.0
+Version: 0.9.1
 Summary: The AITracker neural network and it's implementation.
 Author: Jacob Hogrefe and Emilio Cruz
 Project-URL: Homepage, https://github.com/AITrackerDev/AITracker
 Project-URL: Issues, https://github.com/AITrackerDev/AITracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: absl-py==0.2.1
-Requires-Dist: astunparse==1.6.3
-Requires-Dist: certifi==2024.2.2
-Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: dlib==19.24.4
-Requires-Dist: flatbuffers==24.3.25
-Requires-Dist: gast==0.5.4
-Requires-Dist: google-pasta==0.2.0
-Requires-Dist: grpcio==1.62.1
 Requires-Dist: h5py==3.11.0
-Requires-Dist: idna==3.7
-Requires-Dist: joblib==1.4.0
-Requires-Dist: keras==3.2.1
-Requires-Dist: libclang==18.1.1
-Requires-Dist: Markdown==3.6
-Requires-Dist: markdown-it-py==3.0.0
-Requires-Dist: MarkupSafe==2.1.5
-Requires-Dist: mdurl==0.1.2
-Requires-Dist: ml-dtypes==0.3.2
-Requires-Dist: namex==0.0.7
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: opt-einsum==3.3.0
-Requires-Dist: optree==0.11.0
-Requires-Dist: packaging==24.0
-Requires-Dist: protobuf==4.25.3
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: rich==13.7.1
 Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0
-Requires-Dist: six==1.16.0
-Requires-Dist: tensorboard==2.16.2
-Requires-Dist: tensorboard-data-server==0.7.2
 Requires-Dist: tensorflow==2.16.1
-Requires-Dist: tensorflow-io-gcs-filesystem==0.36.0
-Requires-Dist: termcolor==2.4.0
-Requires-Dist: threadpoolctl==3.4.0
-Requires-Dist: typing_extensions==4.11.0
-Requires-Dist: urllib3==2.2.1
-Requires-Dist: Werkzeug==3.0.2
-Requires-Dist: wrapt==1.16.0
 
 # AITracker
 
 ## What is this?
 
 AITracker is a deep learning neural network designed to take an image of a person's eyes and determine the direction they are looking in. This repo is a Python module designed to be as easy to use as possible.
```

### Comparing `AITracker-0.9.0/README.md` & `AITracker-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/src/AITracker/AITrackerModel.py` & `AITracker-0.9.1/src/AITracker/AITrackerModel.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/src/AITracker/AITrackerNetwork.py` & `AITracker-0.9.1/src/AITracker/AITrackerNetwork.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/src/AITracker/DataValidation.py` & `AITracker-0.9.1/src/AITracker/DataValidation.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/src/AITracker/UpdateH5.py` & `AITracker-0.9.1/src/AITracker/UpdateH5.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.0/src/AITracker.egg-info/PKG-INFO` & `AITracker-0.9.1/src/AITracker.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,29 @@
 Metadata-Version: 2.1
 Name: AITracker
-Version: 0.9.0
+Version: 0.9.1
 Summary: The AITracker neural network and it's implementation.
 Author: Jacob Hogrefe and Emilio Cruz
 Project-URL: Homepage, https://github.com/AITrackerDev/AITracker
 Project-URL: Issues, https://github.com/AITrackerDev/AITracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: absl-py==0.2.1
-Requires-Dist: astunparse==1.6.3
-Requires-Dist: certifi==2024.2.2
-Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: dlib==19.24.4
-Requires-Dist: flatbuffers==24.3.25
-Requires-Dist: gast==0.5.4
-Requires-Dist: google-pasta==0.2.0
-Requires-Dist: grpcio==1.62.1
 Requires-Dist: h5py==3.11.0
-Requires-Dist: idna==3.7
-Requires-Dist: joblib==1.4.0
-Requires-Dist: keras==3.2.1
-Requires-Dist: libclang==18.1.1
-Requires-Dist: Markdown==3.6
-Requires-Dist: markdown-it-py==3.0.0
-Requires-Dist: MarkupSafe==2.1.5
-Requires-Dist: mdurl==0.1.2
-Requires-Dist: ml-dtypes==0.3.2
-Requires-Dist: namex==0.0.7
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: opt-einsum==3.3.0
-Requires-Dist: optree==0.11.0
-Requires-Dist: packaging==24.0
-Requires-Dist: protobuf==4.25.3
-Requires-Dist: Pygments==2.17.2
-Requires-Dist: requests==2.31.0
-Requires-Dist: rich==13.7.1
 Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0
-Requires-Dist: six==1.16.0
-Requires-Dist: tensorboard==2.16.2
-Requires-Dist: tensorboard-data-server==0.7.2
 Requires-Dist: tensorflow==2.16.1
-Requires-Dist: tensorflow-io-gcs-filesystem==0.36.0
-Requires-Dist: termcolor==2.4.0
-Requires-Dist: threadpoolctl==3.4.0
-Requires-Dist: typing_extensions==4.11.0
-Requires-Dist: urllib3==2.2.1
-Requires-Dist: Werkzeug==3.0.2
-Requires-Dist: wrapt==1.16.0
 
 # AITracker
 
 ## What is this?
 
 AITracker is a deep learning neural network designed to take an image of a person's eyes and determine the direction they are looking in. This repo is a Python module designed to be as easy to use as possible.
```

