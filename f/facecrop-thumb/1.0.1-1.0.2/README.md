# Comparing `tmp/facecrop-thumb-1.0.1.tar.gz` & `tmp/facecrop-thumb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facecrop-thumb-1.0.1.tar", last modified: Fri Apr 12 15:05:59 2024, max compression
+gzip compressed data, was "facecrop-thumb-1.0.2.tar", last modified: Fri Apr 12 15:18:41 2024, max compression
```

## Comparing `facecrop-thumb-1.0.1.tar` & `facecrop-thumb-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:05:58.995185 facecrop-thumb-1.0.1/
--rw-rw-rw-   0        0        0     1092 2024-04-12 11:58:00.000000 facecrop-thumb-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1204 2024-04-12 15:05:58.993183 facecrop-thumb-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1577 2024-04-12 12:03:25.000000 facecrop-thumb-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 15:05:58.992184 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/
--rw-rw-rw-   0        0        0     1204 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:05:58.000000 facecrop-thumb-1.0.1/facecrop_thumb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-04-12 14:43:37.000000 facecrop-thumb-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 15:05:58.995185 facecrop-thumb-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1481 2024-04-12 14:57:09.000000 facecrop-thumb-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:18:41.490595 facecrop-thumb-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-12 11:58:00.000000 facecrop-thumb-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1204 2024-04-12 15:18:41.489601 facecrop-thumb-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1577 2024-04-12 12:03:25.000000 facecrop-thumb-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 15:18:41.483627 facecrop-thumb-1.0.2/facecrop-thumb/
+-rw-rw-rw-   0        0        0        0 2024-04-12 15:10:13.000000 facecrop-thumb-1.0.2/facecrop-thumb/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-12 15:16:49.000000 facecrop-thumb-1.0.2/facecrop-thumb/__main__.py
+-rw-rw-rw-   0        0        0      283 2024-04-12 10:33:36.000000 facecrop-thumb-1.0.2/facecrop-thumb/face_detection.py
+-rw-rw-rw-   0        0        0      788 2024-04-12 10:33:30.000000 facecrop-thumb-1.0.2/facecrop-thumb/image_processing.py
+-rw-rw-rw-   0        0        0     1042 2024-04-12 12:37:35.000000 facecrop-thumb-1.0.2/facecrop-thumb/main.py
+-rw-rw-rw-   0        0        0     2461 2024-04-12 12:37:45.000000 facecrop-thumb-1.0.2/facecrop-thumb/thumbnail_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:18:41.489601 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/
+-rw-rw-rw-   0        0        0     1204 2024-04-12 15:18:41.000000 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2024-04-12 15:18:41.000000 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:18:41.000000 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-12 15:18:41.000000 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 15:18:41.000000 facecrop-thumb-1.0.2/facecrop_thumb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-04-12 14:43:37.000000 facecrop-thumb-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:18:41.491654 facecrop-thumb-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-04-12 15:18:27.000000 facecrop-thumb-1.0.2/setup.py
```

### Comparing `facecrop-thumb-1.0.1/LICENSE` & `facecrop-thumb-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facecrop-thumb-1.0.1/PKG-INFO` & `facecrop-thumb-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facecrop-thumb
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate thumbnails of detected faces in images using Python.
 Home-page: https://github.com/mr-vaibh/facecrop-thumb
 Author: Vaibhav Shukla
 Author-email: shuklavaibhav336@example.com
 License: MIT
 Keywords: face detection thumbnail image-processing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `facecrop-thumb-1.0.1/README.md` & `facecrop-thumb-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `facecrop-thumb-1.0.1/facecrop_thumb.egg-info/PKG-INFO` & `facecrop-thumb-1.0.2/facecrop_thumb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facecrop-thumb
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate thumbnails of detected faces in images using Python.
 Home-page: https://github.com/mr-vaibh/facecrop-thumb
 Author: Vaibhav Shukla
 Author-email: shuklavaibhav336@example.com
 License: MIT
 Keywords: face detection thumbnail image-processing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `facecrop-thumb-1.0.1/setup.py` & `facecrop-thumb-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='facecrop-thumb',
-    version='1.0.1',
+    version='1.0.2',
     description='Generate thumbnails of detected faces in images using Python.',
     long_description='FaceCropThumb is a Python package for generating thumbnails of detected faces in images. It utilizes the MTCNN (Multi-Task Cascaded Convolutional Neural Network) for accurate face detection and OpenCV for image processing.',
     url='https://github.com/mr-vaibh/facecrop-thumb',
     author='Vaibhav Shukla',
     author_email='shuklavaibhav336@example.com',
     license='MIT',
     classifiers=[
@@ -24,13 +24,8 @@
     ],
     keywords='face detection thumbnail image-processing',
     packages=find_packages(),
     install_requires=[
         'mtcnn>=0.1.1',
         'opencv-python>=4.9.0.80',
     ],
-    entry_points={
-        'console_scripts': [
-            'facecrop-thumb=facecrop_thumb.main:main',
-        ],
-    },
 )
```

