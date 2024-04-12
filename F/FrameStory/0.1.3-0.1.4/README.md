# Comparing `tmp/FrameStory-0.1.3.tar.gz` & `tmp/FrameStory-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FrameStory-0.1.3.tar", last modified: Sun Apr  7 11:44:55 2024, max compression
+gzip compressed data, was "FrameStory-0.1.4.tar", last modified: Fri Apr 12 08:57:09 2024, max compression
```

## Comparing `FrameStory-0.1.3.tar` & `FrameStory-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:44:55.800804 FrameStory-0.1.3/
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:44:55.799851 FrameStory-0.1.3/FrameStory.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3571 2024-04-07 11:44:55.000000 FrameStory-0.1.3/FrameStory.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      298 2024-04-07 11:44:55.000000 FrameStory-0.1.3/FrameStory.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-07 11:44:55.000000 FrameStory-0.1.3/FrameStory.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      104 2024-04-07 11:44:55.000000 FrameStory-0.1.3/FrameStory.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       18 2024-04-07 11:44:55.000000 FrameStory-0.1.3/FrameStory.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-04 13:56:00.000000 FrameStory-0.1.3/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3571 2024-04-07 11:44:55.800685 FrameStory-0.1.3/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2642 2024-04-07 11:44:19.000000 FrameStory-0.1.3/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:44:55.800075 FrameStory-0.1.3/frame_story/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:48.000000 FrameStory-0.1.3/frame_story/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3479 2024-04-04 14:52:48.000000 FrameStory-0.1.3/frame_story/video_describer.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-07 11:44:55.800840 FrameStory-0.1.3/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1278 2024-04-07 11:44:19.000000 FrameStory-0.1.3/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:44:55.800394 FrameStory-0.1.3/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-04 14:52:48.000000 FrameStory-0.1.3/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1805 2024-04-04 14:52:48.000000 FrameStory-0.1.3/tests/test_video_describer.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 08:57:09.589976 FrameStory-0.1.4/
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 08:57:09.588980 FrameStory-0.1.4/FrameStory.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3570 2024-04-12 08:57:09.000000 FrameStory-0.1.4/FrameStory.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      298 2024-04-12 08:57:09.000000 FrameStory-0.1.4/FrameStory.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-12 08:57:09.000000 FrameStory-0.1.4/FrameStory.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      104 2024-04-12 08:57:09.000000 FrameStory-0.1.4/FrameStory.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       18 2024-04-12 08:57:09.000000 FrameStory-0.1.4/FrameStory.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1073 2024-04-04 13:56:00.000000 FrameStory-0.1.4/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3570 2024-04-12 08:57:09.589843 FrameStory-0.1.4/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2641 2024-04-12 08:57:01.000000 FrameStory-0.1.4/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 08:57:09.589193 FrameStory-0.1.4/frame_story/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:45:34.000000 FrameStory-0.1.4/frame_story/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3479 2024-04-07 11:45:34.000000 FrameStory-0.1.4/frame_story/video_describer.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-12 08:57:09.590021 FrameStory-0.1.4/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1278 2024-04-12 08:57:01.000000 FrameStory-0.1.4/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-12 08:57:09.589525 FrameStory-0.1.4/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-07 11:45:34.000000 FrameStory-0.1.4/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1805 2024-04-07 11:45:34.000000 FrameStory-0.1.4/tests/test_video_describer.py
```

### Comparing `FrameStory-0.1.3/FrameStory.egg-info/PKG-INFO` & `FrameStory-0.1.4/FrameStory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameStory
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for creating video descriptions by analyzing and extracting significant frames.
 Home-page: https://github.com/chigwell/FrameStory
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/FrameStory.svg)](https://badge.fury.io/py/frame_story)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/frame_story)
+[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/FrameStory)
 
 # Frame Story
 
 `FrameStory` is a Python package designed for extracting and describing significant frames from videos. Leveraging state-of-the-art machine learning models, it can provide detailed descriptions of video content, making it a powerful tool for content analysis, accessibility, and summarization.
 
 ## Installation
```

### Comparing `FrameStory-0.1.3/LICENSE` & `FrameStory-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FrameStory-0.1.3/PKG-INFO` & `FrameStory-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FrameStory
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for creating video descriptions by analyzing and extracting significant frames.
 Home-page: https://github.com/chigwell/FrameStory
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/FrameStory.svg)](https://badge.fury.io/py/frame_story)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/frame_story)
+[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/FrameStory)
 
 # Frame Story
 
 `FrameStory` is a Python package designed for extracting and describing significant frames from videos. Leveraging state-of-the-art machine learning models, it can provide detailed descriptions of video content, making it a powerful tool for content analysis, accessibility, and summarization.
 
 ## Installation
```

### Comparing `FrameStory-0.1.3/README.md` & `FrameStory-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/FrameStory.svg)](https://badge.fury.io/py/frame_story)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/frame_story)
+[![Downloads](https://static.pepy.tech/badge/FrameStory)](https://pepy.tech/project/FrameStory)
 
 # Frame Story
 
 `FrameStory` is a Python package designed for extracting and describing significant frames from videos. Leveraging state-of-the-art machine learning models, it can provide detailed descriptions of video content, making it a powerful tool for content analysis, accessibility, and summarization.
 
 ## Installation
```

### Comparing `FrameStory-0.1.3/frame_story/video_describer.py` & `FrameStory-0.1.4/frame_story/video_describer.py`

 * *Files identical despite different names*

### Comparing `FrameStory-0.1.3/setup.py` & `FrameStory-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FrameStory',
-    version='0.1.3',
+    version='0.1.4',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description='A Python package for creating video descriptions by analyzing and extracting significant frames.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/FrameStory',
     packages=find_packages(),
```

### Comparing `FrameStory-0.1.3/tests/test_video_describer.py` & `FrameStory-0.1.4/tests/test_video_describer.py`

 * *Files identical despite different names*

