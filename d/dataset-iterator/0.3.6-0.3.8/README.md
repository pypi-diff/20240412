# Comparing `tmp/dataset_iterator-0.3.6.tar.gz` & `tmp/dataset_iterator-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.3.6.tar", last modified: Thu Feb 22 10:57:49 2024, max compression
+gzip compressed data, was "dataset_iterator-0.3.8.tar", last modified: Fri Apr 12 15:13:22 2024, max compression
```

## Comparing `dataset_iterator-0.3.6.tar` & `dataset_iterator-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    10141 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/LICENSE.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/PKG-INFO
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2412 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/README.md
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/dataset_iterator/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      577 2023-09-10 13:32:11.000000 dataset_iterator-0.3.6/dataset_iterator/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3655 2023-09-13 08:48:24.000000 dataset_iterator-0.3.6/dataset_iterator/concat_iterator.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/dataset_iterator/datasetIO/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      320 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/__init__.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2468 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1794 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3011 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/group_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     2923 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/h5pyIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1306 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/memoryIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3632 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    13528 2023-08-07 12:58:09.000000 dataset_iterator-0.3.6/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    11436 2023-10-05 15:08:59.000000 dataset_iterator-0.3.6/dataset_iterator/helpers.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    18859 2024-02-22 10:54:22.000000 dataset_iterator-0.3.6/dataset_iterator/image_data_generator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3656 2023-12-28 15:01:55.000000 dataset_iterator-0.3.6/dataset_iterator/index_array_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    56541 2023-12-28 15:25:18.000000 dataset_iterator-0.3.6/dataset_iterator/multichannel_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    13765 2023-09-14 15:54:20.000000 dataset_iterator-0.3.6/dataset_iterator/pre_processing.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    19516 2024-02-22 10:24:52.000000 dataset_iterator-0.3.6/dataset_iterator/tile_utils.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)    11863 2023-11-09 12:16:49.000000 dataset_iterator-0.3.6/dataset_iterator/tracking_iterator.py
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     5279 2023-11-18 10:49:07.000000 dataset_iterator-0.3.6/dataset_iterator/utils.py
-drwxrwxr-x   0 jollion   (1000) jollion   (1000)        0 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/dataset_iterator.egg-info/
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     3541 2024-02-22 10:57:49.000000 dataset_iterator-0.3.6/dataset_iterator.egg-info/PKG-INFO
--rw-rw-r--   0 jollion   (1000) jollion   (1000)      924 2024-02-22 10:57:49.000000 dataset_iterator-0.3.6/dataset_iterator.egg-info/SOURCES.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)        1 2024-02-22 10:57:49.000000 dataset_iterator-0.3.6/dataset_iterator.egg-info/dependency_links.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       65 2024-02-22 10:57:49.000000 dataset_iterator-0.3.6/dataset_iterator.egg-info/requires.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       17 2024-02-22 10:57:49.000000 dataset_iterator-0.3.6/dataset_iterator.egg-info/top_level.txt
--rw-rw-r--   0 jollion   (1000) jollion   (1000)       38 2024-02-22 10:57:49.173658 dataset_iterator-0.3.6/setup.cfg
--rw-rw-r--   0 jollion   (1000) jollion   (1000)     1466 2024-02-22 10:30:00.000000 dataset_iterator-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57974 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19770 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-12 15:13:22.000000 dataset_iterator-0.3.8/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 15:13:22.000000 dataset_iterator-0.3.8/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:13:22.000000 dataset_iterator-0.3.8/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 15:13:22.000000 dataset_iterator-0.3.8/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 15:13:22.000000 dataset_iterator-0.3.8/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:13:22.134598 dataset_iterator-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 15:13:18.000000 dataset_iterator-0.3.8/setup.py
```

### Comparing `dataset_iterator-0.3.6/LICENSE.txt` & `dataset_iterator-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/PKG-INFO` & `dataset_iterator-0.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.3.6
-Summary: data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator
+Version: 0.3.8
+Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
+Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.9.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
-License: UNKNOWN
-Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.4.tar.gz
 Keywords: Iterator,Dataset,Image,Numpy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: h5py>=2.9
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: scikit-image
+Requires-Dist: tensorflow
+Requires-Dist: keras
 
 # Dataset Iterator
 This repo contains keras iterator classes for multi-channel (time-lapse) images contained in dataset files such as hdf5.
 
 ## Dataset structure:
 One dataset file can contain several sub-datasets (dataset_name0, dataset_name1, etc...), the iterator will iterate through all of them as if they were concatenated.
 
@@ -70,9 +75,7 @@
 - There is currently an implementation of DatasetIO for .h5 files (`H5pyIO`), as well as dataset composed of multiple images files supported by PILLOW (`MultipleFileIO`).
 - one can also concatenate datasets from different files:
   - if a dataset is split into several files that contain the same channels: use `ConcatenateDatasetIO`
   - if a dataset contains channels in different files, use: `MultipleDatasetIO`
 
 # Demo
 See this notebook for a demo: [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1J-UPivwyNTpyLhOMfzhfG0pIl6gDD9I5)
-
-
```

### Comparing `dataset_iterator-0.3.6/README.md` & `dataset_iterator-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/dataset_iterator/__init__.py` & `dataset_iterator-0.3.8/dataset_iterator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 from .index_array_iterator import IndexArrayIterator
 from .multichannel_iterator import MultiChannelIterator
 from .tracking_iterator import TrackingIterator
 from .tile_utils import extract_tiles, augment_tiles, extract_tile_function, extract_tile_random_zoom_function, augment_tiles_inplace
 from .image_data_generator import get_image_data_generator
 
 from .datasetIO import DatasetIO, H5pyIO, MultipleFileIO, MultipleDatasetIO, ConcatenateDatasetIO, MemoryIO
-from .utils import enrich_with_hardest_indices
+from .hard_sample_mining import HardSampleMiningCallback
 from .concat_iterator import ConcatIterator
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/datasetIO.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return dataset
     elif isinstance(dataset, str):
         if dataset.endswith(".h5") or dataset.endswith(".hdf5"):
             from .h5pyIO import H5pyIO
             return H5pyIO(dataset, mode)
         elif os.path.isdir(dataset):
             from .multiple_fileIO import MultipleFileIO # import when needed -> IO libraries may be missing
-            return MultipleFileIO(dataset, 1) # consider that directory contains files, each file corresponds to a single image with same dimensions
+            return MultipleFileIO(dataset, True) # consider that directory contains files, each file corresponds to a single image with same dimensions
         elif dataset.lower().endswith(('.tif', '.tiff')):
             from .multiple_fileIO import MultipleFileIO
-            return MultipleFileIO(os.path.abspath(os.path.join(dataset, os.pardir)), 0)
+            return MultipleFileIO(os.path.abspath(os.path.join(dataset, os.pardir)), False)
     elif isinstance(dataset, (tuple, list)):
         from .concatenate_datasetIO import ConcatenateDatasetIO
         return ConcatenateDatasetIO(dataset) if len(dataset)>1 else get_datasetIO(dataset[0])
     raise ValueError("File type not supported (yet)")
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.__lock__ = threading.Lock()
         self.h5py_file=None
 
     def _get_file(self):
         if self.h5py_file is None:
             with self.__lock__:
                 if self.h5py_file is None:
-                    self.h5py_file = h5py.File(self.path, self.mode, libver='latest', swmr=True) # use https://docs.h5py.org/en/stable/swmr.html
+                    self.h5py_file = h5py.File(self.path, self.mode, libver='latest', swmr=True, locking=False, driver=None) # use https://docs.h5py.org/en/stable/swmr.html
         return self.h5py_file
 
     def close(self):
         if self.h5py_file is not None:
             self.h5py_file.close()
             self.h5py_file = None
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/memoryIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/memoryIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.3.6/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.3.8/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from .datasetIO import DatasetIO
 import threading
 import os
 from os import listdir
 from os.path import isfile, join
 from tensorflow.keras.utils import img_to_array
+from math import log10
 import numpy as np
 try:
     from PIL import Image as pil_image
 except ImportError:
     pil_image = None
+try:
+    from tifffile import imwrite as tiff_write
+except ImportError:
+    tiff_write = None
 
 if pil_image is not None:
     _PIL_INTERPOLATION_METHODS = {
         'nearest': pil_image.NEAREST,
         'bilinear': pil_image.BILINEAR,
         'bicubic': pil_image.BICUBIC,
     }
@@ -26,16 +31,16 @@
 class MultipleFileIO(DatasetIO):
     """Allows to iterate an image dataset that contains several image files compatible with PILLOW
 
     Parameters
     ----------
     directory : string
         Each subdirectory in this directory will be considered to contain images from one channel with the name of the channel corresponding to the name of the subdirectory
-    n_image_per_file : int
-        how many images contains each file.
+    one_image_per_file : boolean
+        whether each file contains a single frame or not.
         if n_image_per_file == 1 the following structure is expected :
             path
             ├── ...
             ├── dataset_name0
             │   ├── channel0
             │   │   ├──frame0 (= single frame image)
             │   │   ├──frame1
@@ -82,44 +87,45 @@
     supported_image_fun : type
         function that takes a file name as argument and return whether the file is a supported image type
 
     Attributes
     ----------
     image_shape : tuple
         target image shape
-    n_image_per_file
+    one_image_per_file
     supported_image_fun
     channel_map_interpolation : interpolation function for each channel, or None
     data_format
     data_type
 
     """
-    def __init__(self, directory, n_image_per_file, target_shape=None, channel_map_interpolation=None , data_format='channels_last', data_type='float32', supported_image_fun = lambda f : f.lower().endswith(('.png', '.tif', '.tiff'))):
+    def __init__(self, directory, one_image_per_file, target_shape=None, channel_map_interpolation=None, data_format='channels_last', data_type='float32', supported_image_fun = lambda f : f.lower().endswith(('.png', '.tif', '.tiff')), write_format='tif'):
         super().__init__()
         self.path = directory
         if pil_image is None:
             raise ImportError('Could not import PIL.Image. The use of `MultipleFilesIO` requires PIL.')
         if channel_map_interpolation is not None:
             assert target_shape is not None, "target_shape must be provided if channel_map_interpolation is provided"
-        self.n_image_per_file = n_image_per_file
+        self.one_image_per_file = one_image_per_file
         self.image_shape = target_shape
         self.supported_image_fun = supported_image_fun
         self.channel_map_interpolation = {c:get_interpolation_function(target_shape, i) for c,i in channel_map_interpolation.items()} if channel_map_interpolation is not None else None
         self.channel_map_nn_interpolation = {c:i=='nearest' for c,i in channel_map_interpolation.items() } if channel_map_interpolation is not None else None # flag channels that have nearest neighbor interpolation to avoid converting them to float
         self.data_format = data_format
         self.dtype = data_type
         self.crop_function = get_crop_function(target_shape) if target_shape is not None else None
+        self.write_format = write_format.lower().replace('.', '')
 
     def close(self):
         pass
 
     def get_dataset_paths(self, channel_keyword, group_keyword=None):
         channel_keyword = fix_keyword(channel_keyword)
         all_dirs = scandir(self.path)
-        if self.n_image_per_file==1:
+        if self.one_image_per_file:
             return [d for d in all_dirs if os.path.basename(d) == channel_keyword and (group_keyword is None or group_keyword in d) ]
         else:
             if len(all_dirs)==0:
                 all_dirs = [self.path]
             filtered_dirs = all_dirs if group_keyword is None else [d for d in all_dirs if group_keyword in d]
             all_imgs = []
             for d in filtered_dirs:
@@ -127,54 +133,84 @@
                 all_imgs.extend(self.get_images(d, name = channel_keyword, npy=True))
             return all_imgs
 
     def __getitem__(self, path):
         return self.get_dataset(path)
 
     def get_dataset(self, path):
-        if self.n_image_per_file==1:
+        if self.one_image_per_file:
             channel_keyword = os.path.basename(os.path.normpath(path))
             return ImageListWrapper(path, self, channel_keyword)
         else:
             channel_keyword = os.path.splitext(os.path.basename(path))[0]
             return ImageWrapper(path, self, channel_keyword)
 
     def get_attribute(self, path, attribute_name):
         return None
 
     def create_dataset(self, path, **create_dataset_kwargs):
         pass
 
     def __contains__(self, key):
-        if self.n_image_per_file==1: # datasets are channel folders
+        if self.one_image_per_file: # datasets are channel folders
             for root, dirs, files in os.walk(self.path):
                 if key in dirs:
                     return True
             return False
         else: # datasets are channel files
             for root, dirs, files in os.walk(self.path):
                 if key in files:
                     return True
             return False
 
     def write_direct(self, path, data, source_sel=None, dest_sel=None):
-        if source_sel is not None or dest_sel is not None:
-            assert self.n_image_per_file == 1, "index selection is only supported if n_image_per_file==1"
-        if self.n_image_per_file == 1:
+        if (source_sel is not None or dest_sel is not None) and not self.one_image_per_file:
+            assert (source_sel is None or source_sel == np.s_[0:data.shape[0]]) and (dest_sel is None or dest_sel == np.s_[0:data.shape[0]]), "index selection is only supported if one_image_per_file is True"
+        if not os.path.isabs(path):
+            path = os.path.join(self.path, path)
+        if self.one_image_per_file:
             if not os.path.isdir(path):
                 os.makedirs(path)
-            n_zeros = int(math.log10( len(data) )) + 1
+            n_zeros = int(log10( len(data) )) + 1
             if dest_sel is None:
                 dest_sel = source_sel
             for i, j in zip(source_sel, dest_sel):
-                np.save(os.path.join(path, str(j).zfill(n_zeros)), data[i], allow_pickle=True)
+                self.write(os.path.join(path, str(j).zfill(n_zeros)), data[i])
         else:
             if not os.path.isdir(get_parent_path(path)):
                 os.makedirs(get_parent_path(path))
-            np.save(path, data)
+            self.write(path, data)
+
+    def write(self, path, data):
+        if self.write_format == 'tif' or self.write_format == 'tiff' or self.write_format == "ome.tif" or self.write_format == "ome.tiff" and tiff_write is not None:
+            if len(data.shape) == 2:
+                dimorder = "YX"
+            elif len(data.shape) == 3:
+                if self.data_format=='channels_last':
+                    data = np.transpose(data, axes=[2, 0, 1])
+                dimorder = "CYX"
+            elif len(data.shape) == 4:
+                if self.one_image_per_file:
+                    if self.data_format == 'channels_last':
+                        data = np.transpose(data, axes=[3, 0, 1, 2])
+                    dimorder = "CZYX"
+                else:
+                    if self.data_format == 'channels_last':
+                        data = np.transpose(data, axes=[0, 3, 1, 2])
+                    dimorder = "TCYX"
+            elif len(data.shape) == 5:
+                if self.data_format == 'channels_last':
+                    data = np.transpose(data, axes=[0, 4, 1, 2, 3])
+                dimorder = "TCZYX"
+            else :
+                raise ValueError("Rank >5 not supported")
+            format = "ome.tif" if len(data.shape)>3 else self.write_format # force OME-TIFF
+            tiff_write(f"{path}.{format}", data=data, ome=True, metadata={'axes': dimorder})
+        else: # fallback to numpy
+            np.save(path, data, allow_pickle=True)
 
     def get_images(self, path, name = None, npy=False):
         if npy:
             return [join(path, f) for f in listdir(path) if f.lower().endswith('.npy') and (name is None or name in f)]
         else:
             return [join(path, f) for f in listdir(path) if self.supported_image_fun(f.lower()) and (name is None or name in f)]
 
@@ -219,23 +255,23 @@
 
 # one file with multiple images
 class ImageWrapper():
     def __init__(self, path, mfileIO, channel_keyword):
         self.path = path
         self.mfileIO=mfileIO
         self.npy = path.endswith('.npy')
-        if mfileIO.n_image_per_file==0 or mfileIO.image_shape is None: # get shape from image file
+        if not mfileIO.one_image_per_file or mfileIO.image_shape is None: # get shape from image file
             if self.npy:
                 img = np.load(self.path, mmap_mode='r')
                 self.shape = img.shape
             else:
                 self.image = pil_image.open(self.path)
                 self.shape = (self.image.n_frames,) + (mfileIO.image_shape if mfileIO.image_shape is not None else self.image.size[::-1])
         else:
-            self.shape = (mfileIO.n_image_per_file,)+mfileIO.image_shape
+            self.shape = (1,) + mfileIO.image_shape
         self.image = None
         self.interpolator = self.mfileIO.channel_map_interpolation[channel_keyword] if self.mfileIO.channel_map_interpolation is not None else None
         if self.interpolator is None and self.mfileIO.crop_function is not None:
             self.interpolator = self.mfileIO.crop_function
         self.convert = not self.mfileIO.channel_map_nn_interpolation[channel_keyword] if self.mfileIO.channel_map_nn_interpolation is not None else False
         if self.npy:
             assert self.interpolator is None, "interpolation not supported (yet) with npy files"
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/helpers.py` & `dataset_iterator-0.3.8/dataset_iterator/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,26 @@
     return min_range, max_range
 
 def get_histogram(dataset, channel_keyword:str, bins, bin_size=None, sum_to_one:bool=False, group_keyword:str=None, batch_size:int=1, return_min_and_bin_size:bool=False, smooth_scale:float = 0., smooth_scale_in_bin_unit:bool=True):
     iterator = MultiChannelIterator(dataset=dataset, channel_keywords=[channel_keyword], group_keyword=group_keyword, input_channels=[0], output_channels=[], batch_size=batch_size, incomplete_last_batch_mode=0)
     if bins is None:
         assert bin_size is not None
         vmin, vmax = get_min_and_max(dataset, channel_keyword, batch_size=batch_size)
-        n_bins = round( (vmax - vmin) / bin_size )
-        bin_size = (vmax - vmin) / n_bins
-        bins = np.linspace(vmin, vmax, num=n_bins+1)
-    if isinstance(bins, int):
+        n_bins = int( 1 + (vmax - vmin ) / bin_size )
+        bin_size = (vmax - vmin ) / (n_bins - 1)
+        bins = np.linspace(vmin, vmax + bin_size, num=n_bins+1)
+        #print(f"range: [{vmin}; {vmax}] nbins: {n_bins} binsize: {bin_size} bins: {bins}")
+    elif isinstance(bins, int):
+        assert bins>1, "at least 2 bins"
         vmin, vmax = get_min_and_max(dataset, channel_keyword, batch_size=batch_size)
-        bin_size = (vmax - vmin)/bins
-        bins = np.linspace(vmin, vmax, num=bins+1)
+        bin_size = (vmax - vmin)/(bins-1)
+        bins = np.linspace(vmin, vmax + bin_size, num=bins+1)
+    else:
+        assert isinstance(bins, (list, tuple))
+        vmin = bins[0]
     histogram = None
     for i in range(len(iterator)):
         batch = iterator[i]
         histo, _ = np.histogram(batch, bins)
         if histogram is None:
             histogram = histo
         else:
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.3.8/dataset_iterator/image_data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,26 @@
 
         """
 
     def __init__(self, generators:list):
         assert is_list(generators), "generator must be a list"
         self.generators = generators
 
+    def get_constant_transform(self, image_shape: tuple):
+        all_params = {}
+        for i, g in enumerate(self.generators):
+            if g is not None:
+                try:
+                    params = g.get_constant_transform(image_shape)
+                    if params is not None:
+                        all_params[i] = params
+                except AttributeError:
+                    pass
+        return all_params
+
     def get_random_transform(self, image_shape:tuple):
         all_params = {}
         for i, g in enumerate(self.generators):
             if g is not None:
                 try:
                     params = g.get_random_transform(image_shape)
                     if params is not None:
@@ -87,15 +99,15 @@
                 try:
                     g.adjust_augmentation_param_from_mask(parameters[i], mask)
                 except AttributeError:
                     pass
 
     def apply_transform(self, img, aug_params:dict):
         for i, g in enumerate(self.generators):
-            if g is not None:
+            if g is not None and i in aug_params:
                 try:
                     im2 = g.apply_transform(img, aug_params[i])
                     if im2 is not None:
                         img = im2
                 except AttributeError:
                     pass
         return img
@@ -107,14 +119,15 @@
                     im2 = g.standardize(img)
                     if im2 is not None:
                         img = im2
                 except AttributeError:
                     pass
         return img
 
+
 # image scaling
 SCALING_MODES = ["RANDOM_CENTILES", "RANDOM_MIN_MAX", "FLUORESCENCE", "BRIGHT_FIELD", "CONSTANT"]
 def get_random_scaling_function(mode="RANDOM_CENTILES", dataset=None, channel_name:str=None, **kwargs):
     data_gen = ScalingImageGenerator(mode, dataset, channel_name, **kwargs)
     def fun(img):
         params = data_gen.get_random_transform(img.shape)
         return data_gen.apply_transform(img, params)
@@ -138,30 +151,51 @@
         elif mode == "RANDOM_CENTILES":
             self.min_centile_range = kwargs.get("min_centile_range", [0.1, 5])
             self.max_centile_range = kwargs.get("max_centile_range", [95, 99.9])
             assert self.min_centile_range[0] <= self.min_centile_range[1], "invalid min range"
             assert self.max_centile_range[0] <= self.max_centile_range[1], "invalid max range"
             assert self.min_centile_range[0] < self.max_centile_range[1], "invalid min and max range"
             self.saturate = kwargs.get("saturate", True)
+            self.min_centile = kwargs.get("min_centile", np.mean(self.min_centile_range))
+            self.max_centile = kwargs.get("max_centile", np.mean(self.max_centile_range))
         elif mode == "RANDOM_MIN_MAX":
             self.min_range = kwargs.get("min_range", 0.1)
             self.range = kwargs.get("range", [0, 1])
         elif mode == "FLUORESCENCE" or mode == "BRIGHT_FIELD":
             fluo = mode == "FLUORESCENCE"
             if "per_image" not in kwargs:
                 kwargs["per_image"] = dataset is None
             self.per_image = kwargs.get("per_image", True)
             if not self.per_image and dataset is None:
                 assert "scale_range" in kwargs and "center_range" in kwargs, "if no dataset is provided, scale_range and center_range must be provided"
                 self.scale_range = kwargs["scale_range"]
                 self.center_range = kwargs["center_range"]
+                self.center = kwargs.get("center", np.mean(self.center_range))
+                self.scale = kwargs.get("scale", np.mean(self.scale_range))
             else:
-                center_range, scale_range = get_center_scale_range(dataset, channel_name=channel_name, fluorescence=fluo, **kwargs)
+                center_range, scale_range = get_center_scale_range(dataset, channel_name=channel_name, fluorescence=fluo, return_center=True, **kwargs)
+                if len(center_range)==3:
+                    self.center = center_range[-1]
+                    center_range = center_range[:2]
+                else:
+                    self.center = np.mean(center_range)
                 self.scale_range = scale_range
                 self.center_range = center_range
+                self.scale = np.mean(scale_range)
+
+    def get_constant_transform(self, image_shape):
+        params = {"constant":True}
+        if self.mode == "RANDOM_MIN_MAX":
+            params["vmin"] = 0.
+            params["vmax"] = 1.
+        elif self.mode == "FLUORESCENCE" or self.mode == "BRIGHT_FIELD":
+            params["center"] = self.center
+            params["scale"] = self.scale
+        return params
+
     def get_random_transform(self, image_shape):
         params = {}
         if self.mode == "RANDOM_CENTILES":
             pmin = random()
             pmax = random()
             cmin = self.min_centile_range[0] + (self.min_centile_range[1] - self.min_centile_range[0]) * pmin
             cmax = self.max_centile_range[0] + (self.max_centile_range[1] - self.max_centile_range[0]) * pmax
@@ -192,17 +226,20 @@
             destination["center"] = source["center"]
             destination["scale"] = source["scale"]
 
     def apply_transform(self, img, aug_params):
         if self.mode=="CONSTANT":
             return (img - self.center) / self.scale
         if self.mode == "RANDOM_CENTILES":
-            min0, min1, max0, max1 = np.percentile(img, self.min_centile_range + self.max_centile_range)
-            cmin = min0 + (min1 - min0) * aug_params["cmin"]
-            cmax = max0 + (max1 - max0) * aug_params["cmax"]
+            if aug_params.get("constant", False):
+                cmin, cmax = np.percentile(img, [self.min_centile, self.max_centile])
+            else: # random
+                min0, min1, max0, max1 = np.percentile(img, self.min_centile_range + self.max_centile_range)
+                cmin = min0 + (min1 - min0) * aug_params["cmin"]
+                cmax = max0 + (max1 - max0) * aug_params["cmax"]
             if self.saturate:
                 img = adjust_histogram_range(img, min=0, max=1, initial_range=[cmin,  cmax])  # will saturate values under cmin or over cmax, as in real life.
             else:
                 scale = 1. / (cmax - cmin)
                 img = (img - cmin) * scale
             return img
         elif self.mode == "RANDOM_MIN_MAX":
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.3.8/dataset_iterator/multichannel_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         should be None or of same length as output_channels.
         For each output channel, if not None, the corresponding function is applied to the output batch of same index.
         Applied after channels_postprocessing_function.
     channels_postprocessing_function : callable
         input is a dict mapping channel index to batch
         applied after image_data_generators and before weight_map_functions / output_postprocessing_functions if any.
     extract_tile_function : callable
-        function that inputs a batch and a bool (that is true if the batch is a mask), splits it into tiles and concatenate along batch axis.
+        function that inputs a batch and 2 bool (1st is true if the batch is a mask, 2nd is true if tiling can be random False if it should be constant), splits it into tiles and concatenate along batch axis.
         when the iterator has several channels, the function must handle a list of batches (and a list of bool) to tile them simultaneously.
         Applied before channels_postprocessing_function and after image_data_generators
     mask_channels : list of ints
         index of channels that contain binary (or labeled) images. Used to detect the presence/abscence of segmented objects at image borders
     output_multiplicity : int
         output = (output) * output_multiplicity
     input_multiplicity : int
@@ -327,14 +327,33 @@
             self.datasetIO = None
             self.ds_array = None
             self.ads_array = None
 
     def close(self):
         self._close_datasetIO()
 
+    def disable_random_transforms(self, data_augmentation:bool=True, channels_postprocessing:bool=False):
+        params = dict()
+        if data_augmentation:
+            params["perform_data_augmentation"] = self.perform_data_augmentation
+            self.perform_data_augmentation = False
+            params["elasticdeform_parameters"] = self.elasticdeform_parameters
+            self.elasticdeform_parameters = None
+        if channels_postprocessing:
+            params["channels_postprocessing_function"] = self.channels_postprocessing_function
+            self.channels_postprocessing_function = None
+        return params
+
+    def enable_random_transforms(self, parameters):
+        if "perform_data_augmentation" in parameters:
+            self.perform_data_augmentation = parameters.get("perform_data_augmentation", True)
+        if "elasticdeform_parameters" in parameters:
+            self.elasticdeform_parameters = parameters.get("elasticdeform_parameters", None)
+        if "channels_postprocessing_function" in parameters:
+            self.channels_postprocessing_function = parameters["channels_postprocessing_function"]
     def train_test_split(self, **options):
         """Split this iterator in two distinct iterators
 
         Parameters
         ----------
 
         **options : dictionary
@@ -420,18 +439,18 @@
             if self.return_image_index:
                 if isinstance(input, tuple):
                     input = list(input)
                 if not isinstance(input, list):
                     input = [input]
                 input.append(batch_by_channel[-1])
             output = _apply_multiplicity(output, self.output_multiplicity) # removes None batches
-            return (input, output)
+            return input, output
 
     def _get_batch_by_channel(self, index_array, perform_augmentation, input_only=False, perform_elasticdeform=True, perform_tiling=True, **kwargs):
-        if self.datasetIO is None: # for concurency issues: file is open lazyly by each worker
+        if self.datasetIO is None: # each worker opens file is open file
             self._open_datasetIO()
         index_array = np.copy(index_array) # so that main index array is not modified
         index_ds = self._get_ds_idx(index_array) # modifies index_array
 
         batch_by_channel = dict()
         channels = self.input_channels if input_only else [c_idx for c_idx, key in enumerate(self.channel_keywords) if key is not None]
         #if len(self.mask_channels)>0 and self.mask_channels[0] in channels: # put mask channel first so it can be used for determining some data augmentation parameters
@@ -520,15 +539,15 @@
                 batch_by_channel[chan_idx] = batches[i]
 
     def _apply_tiling(self, batch_by_channel):
         if self.extract_tile_function is not None:
             channels = [c for c in batch_by_channel.keys() if not isinstance(c, str) and c>=0]
             batches = [batch_by_channel[chan_idx] for chan_idx in channels]
             is_mask = [chan_idx in self.mask_channels for chan_idx in channels]
-            batches = self.extract_tile_function(batches, is_mask)
+            batches = self.extract_tile_function(batches, is_mask, allow_random=self.perform_data_augmentation)
             n_tiles = batches[0].shape[0]//batch_by_channel[channels[0]].shape[0]
             for i, chan_idx in enumerate(channels):
                 batch_by_channel[chan_idx] = batches[i]
             if self.return_image_index and n_tiles>1:
                 batch_by_channel[-1] = np.tile(batch_by_channel[-1], (n_tiles, 1)) # transmit tiling to image index
 
     def _get_input_batch(self, batch_by_channel, ref_chan_idx, aug_param_array):
@@ -579,27 +598,27 @@
         type
             batch of image for the channel of index chan_idx
 
         """
 
         batch, index_a = self._read_image_batch(index_ds, index_array, chan_idx, ref_chan_idx, aug_param_array, **kwargs)
         # apply augmentation
-        image_data_generator = self.image_data_generators[chan_idx] if self.perform_data_augmentation and perform_augmentation and self.image_data_generators!=None else None
-        for i in range(batch.shape[0]):
-            if image_data_generator!=None:
-                params = self._get_data_augmentation_parameters(chan_idx, ref_chan_idx, batch, i, index_ds, index_array)
-                if aug_param_array is not None and params is not None:
-                    if chan_idx!=ref_chan_idx:
-                        try:
-                            self.image_data_generators[chan_idx].transfer_parameters(aug_param_array[i][ref_chan_idx], params)
-                        except AttributeError:
-                            pass
-                    for k,v in params.items():
-                        aug_param_array[i][chan_idx][k]=v
-                batch[i] = self._apply_augmentation(batch[i], chan_idx, params)
+        if self.image_data_generators is not None and self.image_data_generators[chan_idx] is not None:
+            for i in range(batch.shape[0]):
+                params = self._get_data_augmentation_parameters(chan_idx, ref_chan_idx, batch, i, constant=not (perform_augmentation and self.perform_data_augmentation))
+                if params is not None:
+                    if aug_param_array is not None:
+                        if chan_idx!=ref_chan_idx:
+                            try:
+                                self.image_data_generators[chan_idx].transfer_parameters(aug_param_array[i][ref_chan_idx], params)
+                            except AttributeError:
+                                pass
+                        for k,v in params.items():
+                            aug_param_array[i][chan_idx][k]=v
+                    batch[i] = self._apply_augmentation(batch[i], chan_idx, params)
         if chan_idx==ref_chan_idx and self.return_image_index:
             return batch, index_a
         else:
             return batch
 
     def _apply_augmentation(self, img, chan_idx, aug_params):
         image_data_generator = self.image_data_generators[chan_idx]
@@ -614,19 +633,25 @@
         images = [read_fun(chan_idx, ds_idx, im_idx) for i, (ds_idx, im_idx) in enumerate(zip(index_ds, index_array))]
         if is_array:
             ensure_same_shape(images) # zero-pad if shape differs
         batch = np.stack(images)
         index_a = np.copy(index_array)[..., np.newaxis] if self.return_image_index else None
         return batch, index_a
 
-    def _get_data_augmentation_parameters(self, chan_idx, ref_chan_idx, batch, idx, index_ds, index_array):
+    def _get_data_augmentation_parameters(self, chan_idx, ref_chan_idx, batch, idx, constant:bool = False):
         if self.image_data_generators is None or self.image_data_generators[chan_idx] is None:
             return None
-        params = self.image_data_generators[chan_idx].get_random_transform(batch.shape[1:])
-        if  params is not None and chan_idx==ref_chan_idx and chan_idx in self.mask_channels:
+        if constant:
+            if hasattr(self.image_data_generators[chan_idx], "get_constant_transform"):
+                params = self.image_data_generators[chan_idx].get_constant_transform(batch.shape[1:])
+            else:
+                params = None
+        else:
+            params = self.image_data_generators[chan_idx].get_random_transform(batch.shape[1:])
+        if params is not None and chan_idx==ref_chan_idx and chan_idx in self.mask_channels:
             try:
                 self.image_data_generators[chan_idx].adjust_augmentation_param_from_mask(params, batch[idx,...,0])
             except AttributeError: # data generator does not have this method
                 pass
         return params
 
     def _read_image(self, chan_idx, ds_idx, im_idx):
@@ -666,79 +691,81 @@
 
     def inspect_indices(self, index_array):
         a = np.array(index_array, dtype=np.int)
         i = self._get_ds_idx(a)
         p = [self.paths[ii] for ii in i]
         return(a, i, p)
 
-    def predict(self, output, model, output_keys, write_every_n_batches = 100, n_output_channels=1, output_image_shapes = None, prediction_function=None, apply_to_prediction=None, close_outputIO=True, **create_dataset_options):
-        of = get_datasetIO(output, 'a')
+    def predict(self, output, output_channels, write_every_n_batches=100, n_output_channels=1, output_image_shapes=None, model=None, prediction_function=None, apply_to_prediction=None, close_outputIO=True, **create_dataset_options):
+        of = get_datasetIO(output, 'a') if output is not None else self.datasetIO
+        assert model is not None or prediction_function is not None, "either model or predict_function should be provided"
+
         if output_image_shapes is None:
             output_image_shapes = self.channel_image_shapes[0] if len(self.channel_image_shapes[0])==self.n_spatial_dims else self.channel_image_shapes[0][:-1]
-        if not isinstance(output_keys, (list, tuple)):
-            output_keys = [output_keys]
+        if not isinstance(output_channels, (list, tuple)):
+            output_channels = [output_channels]
         if not isinstance(output_image_shapes, list):
             output_image_shapes = [output_image_shapes]
-        output_image_shapes = ensure_multiplicity(len(output_keys), output_image_shapes)
-        n_output_channels = ensure_multiplicity(len(output_keys), n_output_channels)
+        output_image_shapes = ensure_multiplicity(len(output_channels), output_image_shapes)
+        n_output_channels = ensure_multiplicity(len(output_channels), n_output_channels)
         output_shapes = [ois+(nc,) for ois, nc in zip(output_image_shapes, n_output_channels)]
         # set iterators parameters for prediction & record them
         batch_index = self.batch_index
         self.batch_index=0
         shuffle = self.shuffle
         self.shuffle=False
         self.reset()
         self._set_index_array() # if shuffle was true
 
         if np.any(self.index_array[1:] < self.index_array[:-1]):
             raise ValueError('Index array should be monotonically increasing')
 
-        buffer = [np.zeros(shape = (min(len(self) * self.batch_size, write_every_n_batches*self.batch_size),)+output_shapes[oidx], dtype=self.dtype) for oidx,k in enumerate(output_keys)]
+        buffer = [np.zeros(shape = (min(len(self) * self.batch_size, write_every_n_batches*self.batch_size),)+output_shapes[oidx], dtype=self.dtype) for oidx,k in enumerate(output_channels)]
         if prediction_function is None:
-            pred_fun = lambda model, input : model.predict(input)
+            pred_fun = lambda input : model.predict(input)
         else:
             pred_fun = prediction_function
 
         for ds_i, ds_i_i, ds_i_len in zip(*np.unique(self._get_ds_idx(self.index_array), return_index=True, return_counts=True)):
-            self._ensure_dataset(of, output_shapes, output_keys, ds_i, **create_dataset_options)
-            paths = [replace_last(self.paths[ds_i], self.channel_keywords[0], output_key) for output_key in output_keys]
+            self._ensure_dataset(of, output_shapes, output_channels, ds_i, **create_dataset_options)
+            paths = [replace_last(self.paths[ds_i], self.channel_keywords[0], output_key) for output_key in output_channels]
             index_arrays = np.array_split(self.index_array[ds_i_i:(ds_i_i+ds_i_len)], ceil(ds_i_len/self.batch_size))
             print("predictions for dataset:", self.paths[ds_i])
             unsaved_batches = 0
             buffer_idx = 0
             output_idx = 0
             start_pred = time.time()
             for i, index_array in enumerate(index_arrays):
                 batch_by_channel, aug_param_array, ref_chan_idx = self._get_batch_by_channel(index_array, perform_augmentation=self.perform_data_augmentation, input_only=True)
                 input = self._get_input_batch(batch_by_channel, ref_chan_idx, aug_param_array)
-                cur_pred = pred_fun(model, input)
+                cur_pred = pred_fun(input)
                 if apply_to_prediction is not None:
                     cur_pred = apply_to_prediction(cur_pred)
                 if not isinstance(cur_pred, (list, tuple)):
                     cur_pred = [cur_pred]
-                assert len(cur_pred)==len(output_keys), 'prediction should have as many output as output_keys argument. # output keys: {} # predictions: {}'.format(len(output_keys), len(cur_pred))
-                for oidx in range(len(output_keys)):
+                assert len(cur_pred)==len(output_channels), 'prediction should have as many output as output_keys argument. # output keys: {} # predictions: {}'.format(len(output_channels), len(cur_pred))
+                for oidx in range(len(output_channels)):
                     assert cur_pred[oidx].shape[1:] == output_shapes[oidx], "prediction shape differs from output shape for output idx={} : prediction: {} target: {}".format(oidx, cur_pred[oidx].shape[1:], output_shapes[oidx])
                 #print("predicted: {}->{}".format(output_idx, cur_pred[0].shape[0]))
-                for oidx in range(len(output_keys)):
+                for oidx in range(len(output_channels)):
                     buffer[oidx][buffer_idx:(buffer_idx+cur_pred[oidx].shape[0])] = cur_pred[oidx]
                 buffer_idx+=cur_pred[0].shape[0] # assumes all outputs have same batch size
                 unsaved_batches +=1
                 if unsaved_batches==write_every_n_batches or i==len(index_arrays)-1:
                     start_save = time.time()
                     #print("dest sel: {} -> {}".format(output_idx, output_idx+buffer_idx))
-                    for oidx in range(len(output_keys)):
+                    for oidx in range(len(output_channels)):
                         of.write_direct(paths[oidx], buffer[oidx], source_sel=np.s_[0:buffer_idx], dest_sel=np.s_[output_idx:(output_idx+buffer_idx)])
                     end_save = time.time()
                     print("#{} batches ({} images) computed in {}s and saved in {}s".format(unsaved_batches, buffer_idx, start_save-start_pred, end_save-start_save))
                     unsaved_batches=0
                     output_idx+=buffer_idx
                     buffer_idx=0
                     start_pred = time.time()
-        if close_outputIO:
+        if close_outputIO and output is not None:
             of.close()
 
         # reset iterators parameters
         self.shuffle = shuffle
         self.batch_index = batch_index
 
     def _ensure_dataset(self, output_file, output_shapes, output_keys, ds_i, **create_dataset_options):
@@ -791,58 +818,52 @@
         if self.void_mask_proportion is not None: # if void_mask_proportion is set. Use case: in case there are too many void masks -> some are randomly removed
             try:
                 void_masks = self.void_masks
             except AttributeError:
                 self.void_masks = self._get_void_masks()
                 void_masks = self.void_masks
             bins = np.bincount(void_masks) #[not void ; void]
+            index_a = self._get_index_array()
             if len(bins)==2:
                 if self.void_mask_proportion[0]==0 and self.void_mask_proportion[1]==0: # remove all void masks
-                    index_a = np.delete(self.allowed_indexes, np.flatnonzero(void_masks))
+                    index_a = np.delete(index_a, np.flatnonzero(void_masks))
                 else:
                     # test right bound
                     target_void_count = int( (self.void_mask_proportion[1] / (1 - self.void_mask_proportion[1]) ) * bins[0] )
                     n_rem = bins[1] - target_void_count
                     if n_rem>0:
                         idx_void = np.flatnonzero(void_masks)
                         to_rem = np.random.choice(idx_void, n_rem, replace=False)
                         print(f"adjust void mask prop: from {bins[0]/(bins[0]+bins[1])} to max {self.void_mask_proportion[1]} remove : {to_rem.shape[0]/self.allowed_indexes.shape[0]} ")
-                        index_a = np.delete(self.allowed_indexes, to_rem)
+                        index_a = np.delete(index_a, to_rem)
                     else: # test left bound
                         target_void_count = int( (self.void_mask_proportion[0] / (1 - self.void_mask_proportion[0])) * bins[0])
                         n_add = target_void_count - bins[1]
                         if n_add>0:
                             idx_void = np.flatnonzero(void_masks)
                             to_add = np.random.choice(idx_void, n_add, replace=False)
-                            index_a = np.append(self.allowed_indexes, to_add)
-                        else:
-                            index_a = self.allowed_indexes
-            else:  # only void or only not void
-                #print("void mask bins: ", bins)
-                index_a = self.allowed_indexes
+                            index_a = np.append(index_a, to_add)
         elif self.group_proportion is not None: # generate a batch with user-defined proportion in each group
             # pick indices for each group
-            if self.allowed_indexes is None:
-                indices_per_group = [np.random.randint(low=self.grp_off[i], high=self.grp_len[i], size=int((self.grp_len[i] - self.grp_off[i])*self.group_proportion[i]+0.5) ) for i in range(len(self.group_map_paths))]
-                index_a = np.concatenate(indices_per_group)
-            else:
-                index_array = np.copy(self.allowed_indexes) # index within group
-                index_grp = self._get_grp_idx(index_array) # group index
-                allowed_indexes_per_group = [self.allowed_indexes[index_grp==i] for i in range(len(self.group_map_paths))]
-                indexes_per_group = [ pick_from_array(allowed_indexes_per_group[i], self.group_proportion[i]) for i in range(len(self.group_map_paths)) ]
-                index_a = np.concatenate(indexes_per_group)
+            index_array = self._get_index_array(choice=False) # index within group
+            index_grp = self._get_grp_idx(index_array) # group index
+            allowed_indexes_per_group = [index_array[index_grp==i] for i in range(len(self.group_map_paths))]
+            proba_per_group = [self.index_probability[index_grp==i] if self.index_probability is not None else None for i in range(len(self.group_map_paths))]
+            if self.index_probability is not None: # sum to one
+                proba_per_group = [p / np.sum(p) for p in proba_per_group]
+            indexes_per_group = [ pick_from_array(allowed_indexes_per_group[i], self.group_proportion[i], p=proba_per_group[i]) for i in range(len(self.group_map_paths)) ]
+            index_a = np.concatenate(indexes_per_group)
             self.group_proportion_init = True
         else:
-            index_a = self.allowed_indexes
+            index_a = self._get_index_array()
         if self.shuffle:
             self.index_array = np.random.permutation(index_a)
         else:
             self.index_array = np.copy(index_a)
-        self._ensure_step_number()
-        self._n = len(self.index_array)
+        self._ensure_step_number() # also sets n
 
     def evaluate(self, model, metrics, perform_data_augmentation=True, reset_allowed_indices=False, progress_callback=None, return_metadata=False):
         """Evaluates model on this iterator.
 
         Parameters
         ----------
         model : object
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/pre_processing.py` & `dataset_iterator-0.3.8/dataset_iterator/pre_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     vmax = uniform(vmin+min_range, range[1])
     return vmin, vmax
 
 def random_histogram_range(img, min_range=0.1, range=[0,1]):
     min, max = compute_histogram_range(min_range, range)
     return adjust_histogram_range(img, min, max)
 
-def get_histogram_normalization_center_scale_ranges(histogram, bins, center_percentile_extent, scale_percentile_range, verbose=False):
+def get_histogram_normalization_center_scale_ranges(histogram, bins, center_percentile_extent, scale_percentile_range, return_mode:bool=False, verbose=False):
     mode_value = get_modal_value(histogram, bins)
     mode_percentile = get_percentile_from_value(histogram, bins, mode_value)
     print("mode value={}, mode percentile={}".format(mode_value, mode_percentile))
     assert mode_percentile<scale_percentile_range[0], "mode percentile is {} and must be lower than lower bound of scale_percentile_range={}".format(mode_percentile, scale_percentile_range)
     if is_list(center_percentile_extent):
         assert len(center_percentile_extent) == 2
     else:
@@ -36,20 +36,22 @@
     percentiles = [max(0, mode_percentile-center_percentile_extent[0]), min(100, mode_percentile+center_percentile_extent[1])]
     scale_percentile_range = ensure_multiplicity(2, scale_percentile_range)
     if isinstance(scale_percentile_range, tuple):
         scale_percentile_range = list(scale_percentile_range)
     percentiles = percentiles + scale_percentile_range
     values = get_percentile(histogram, bins, percentiles)
     mode_range = [values[0], values[1] ]
+    if return_mode:
+        mode_range.append(mode_value)
     scale_range = [values[2] - mode_value, values[3] - mode_value]
     if verbose:
         print("normalization_center_scale: modal value: {}, center_range: [{}; {}] scale_range: [{}; {}]".format(mode_value, mode_range[0], mode_range[1], scale_range[0], scale_range[1]))
     return mode_range, scale_range
 
-def get_center_scale_range(dataset, channel_name:str = "/raw", fluorescence:bool = False, bf_sd_factor:float=3., fluo_scale_centile_range:list=[75, 99.9], fluo_center_centile_extent:list=[20, 30], per_image:bool=True, verbose:bool=True):
+def get_center_scale_range(dataset, channel_name:str = "/raw", fluorescence:bool = False, bf_sd_factor:float=3., fluo_scale_centile_range:list=[75, 99.9], fluo_center_centile_extent:list=[20, 30], per_image:bool=True, return_center:bool=False, verbose:bool=True):
     """Computes a range for center and for scale factor for data augmentation.
     Image can then be normalized using a random center C in the center range and a random scaling factor in the scale range: I -> (I - C) / S
 
     Parameters
     ----------
     dataset : datasetIO/path(str) OR list/tuple of datasetIO/path(str)
     channel_name : str
@@ -83,29 +85,31 @@
         return scale_range, center_range
     if fluorescence:
         if per_image:
             center_range, scale_range = [0, 1], [0, 1]
         else:
             bins = get_histogram_bins_IPR(*get_histogram(dataset, channel_name, bins=1000), n_bins=256, percentiles=[0, 95], verbose=verbose)
             histo, _ = get_histogram(dataset, channel_name, bins=bins)
-            center_range, scale_range = get_histogram_normalization_center_scale_ranges(histo, bins, fluo_center_centile_extent, fluo_scale_centile_range, verbose=True)
+            center_range, scale_range = get_histogram_normalization_center_scale_ranges(histo, bins, fluo_center_centile_extent, fluo_scale_centile_range, return_mode=return_center, verbose=True)
             if verbose:
                 print("center: [{}; {}] / scale: [{}; {}]".format(center_range[0], center_range[1], scale_range[0], scale_range[1]))
         return center_range, scale_range
     else:
         if per_image:
             center_range, scale_range = [- bf_sd_factor, bf_sd_factor], [1. / bf_sd_factor, bf_sd_factor]
         else:
             mean, sd = get_mean_sd(dataset, channel_name, per_channel=True)
             mean, sd = np.mean(mean), np.mean(sd)
             if verbose:
                 print("mean: {} sd: {}".format(mean, sd))
             center_range, scale_range = [mean - bf_sd_factor * sd, mean + bf_sd_factor * sd], [sd / bf_sd_factor, sd * bf_sd_factor]
             if verbose:
                 print("center: [{}; {}] / scale: [{}; {}]".format(center_range[0], center_range[1], scale_range[0], scale_range[1]))
+            if return_center:
+                center_range.append(mean)
         return center_range, scale_range
 
 
 # bluring, noise
 def random_gaussian_blur(img, sigma=(1, 2)):
     if is_list(sigma):
         assert len(sigma)==2 and sigma[0]<=sigma[1], "sigma should be a range"
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/tile_utils.py` & `dataset_iterator-0.3.8/dataset_iterator/tile_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from numpy.random import randint, random
 from .utils import ensure_multiplicity, is_null
 from scipy.ndimage import zoom
 
 OVERLAP_MODE = ["NO_OVERLAP", "ALLOW", "FORCE"]
 
 def extract_tile_function(tile_shape, perform_augmentation=True, overlap_mode=OVERLAP_MODE[1], min_overlap=1, n_tiles=None, random_stride=False, augmentation_rotate=True):
-    def func(batch, is_mask):
-        tiles = extract_tiles(batch, tile_shape=tile_shape, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride, return_coords=False)
-        if perform_augmentation:
-            tiles = augment_tiles_inplace(tiles, rotate = augmentation_rotate and all([s==tile_shape[0] for s in tile_shape]), n_dims=len(tile_shape))
+    def func(batch, is_mask:bool, allow_random:bool=True):
+        tiles = extract_tiles(batch, tile_shape=tile_shape, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride if allow_random else False, return_coords=False)
+        if perform_augmentation and allow_random:
+            tiles = augment_tiles_inplace(tiles, rotate=augmentation_rotate and all([s==tile_shape[0] for s in tile_shape]), n_dims=len(tile_shape))
         return tiles
     return func
 
 def extract_tiles(batch, tile_shape, overlap_mode=OVERLAP_MODE[1], min_overlap=1, n_tiles=None, random_stride=True, return_coords=False):
     """Extract tiles.
 
     Parameters
@@ -64,22 +64,22 @@
         return tiles, tile_coords
     else:
         return tiles
 
 def extract_tile_random_zoom_function(tile_shape, perform_augmentation=True, overlap_mode=OVERLAP_MODE[1], min_overlap=1, n_tiles=None, random_stride=True, augmentation_rotate=True, zoom_range=[0.9, 1.1], aspect_ratio_range=[0.9, 1.1], zoom_probability:float=0.5, interpolation_order=1, random_channel_jitter_shape=None):
     if (is_null(zoom_range, 1) or is_null(zoom_range, 0)) and is_null(random_channel_jitter_shape, 0):
         return extract_tile_function(tile_shape, perform_augmentation=perform_augmentation, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride, augmentation_rotate=augmentation_rotate)
-    def func(batch, is_mask):
+    def func(batch, is_mask:bool, allow_random:bool=True):
         if isinstance(batch, (list, tuple)):
             is_mask = ensure_multiplicity(len(batch), is_mask)
             order = [0 if m else interpolation_order for m in is_mask]
         else:
             order = 0 if is_mask else interpolation_order
-        tiles = extract_tiles_random_zoom(batch, tile_shape=tile_shape, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride, zoom_range=zoom_range, aspect_ratio_range=aspect_ratio_range, zoom_probability=zoom_probability, interpolation_order=order, random_channel_jitter_shape=random_channel_jitter_shape)
-        if perform_augmentation:
+        tiles = extract_tiles_random_zoom(batch, tile_shape=tile_shape, overlap_mode=overlap_mode, min_overlap=min_overlap, n_tiles=n_tiles, random_stride=random_stride if allow_random else False, zoom_range=zoom_range if allow_random else [1., 1.], aspect_ratio_range=aspect_ratio_range if allow_random else [1., 1.], zoom_probability=zoom_probability if allow_random else 0., interpolation_order=order, random_channel_jitter_shape=random_channel_jitter_shape if allow_random else None)
+        if perform_augmentation and allow_random:
             tiles = augment_tiles_inplace(tiles, rotate=augmentation_rotate and all([s==tile_shape[0] for s in tile_shape]), n_dims=len(tile_shape))
         return tiles
     return func
 
 def extract_tiles_random_zoom(batch, tile_shape, overlap_mode=OVERLAP_MODE[1], min_overlap=1, n_tiles=None, random_stride=False, zoom_range=[0.9, 1.1], aspect_ratio_range=[0.9, 1.1], zoom_probability:float=0.5, interpolation_order=1, random_channel_jitter_shape=None):
     """Extract tiles with random zoom.
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.3.8/dataset_iterator/tracking_iterator.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,30 @@
                 return 1
             self.frame_subsampling = fs
         else:
             def fs():
                 return frame_subsampling
             self.frame_subsampling = fs
 
+    def disable_random_transforms(self, data_augmentation:bool=True, channels_postprocessing:bool=False):
+        params = super().disable_random_transforms(data_augmentation, channels_postprocessing)
+        params["frame_subsampling"] = self.frame_subsampling
+        params["aug_remove_prob"] = self.aug_remove_prob
+        self.aug_remove_prob = 0
+        def fs():
+            return 1
+        self.frame_subsampling = fs
+        return params
+
+    def enable_random_transforms(self, parameters):
+        super().enable_random_transforms(parameters)
+        if "frame_subsampling" in parameters:
+            self.frame_subsampling = parameters["frame_subsampling"]
+        if "aug_remove_prob" in parameters:
+            self.aug_remove_prob = parameters["aug_remove_prob"]
 
     def _get_batch_by_channel(self, index_array, perform_augmentation, input_only=False, perform_elasticdeform=True, perform_tiling=True, **kwargs):
         if "n_frames" not in kwargs:
             if self.aug_remove_prob>0 and random() < self.aug_remove_prob:
                 kwargs.update({"n_frames":0}) # flag aug remove
         if "frame_subsampling" not in kwargs:
             kwargs.update({"frame_subsampling":self.frame_subsampling()})
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.3.8/dataset_iterator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
-Name: dataset-iterator
-Version: 0.3.6
-Summary: data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator
+Name: dataset_iterator
+Version: 0.3.8
+Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
+Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.9.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
-License: UNKNOWN
-Download-URL: https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.4.tar.gz
 Keywords: Iterator,Dataset,Image,Numpy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: h5py>=2.9
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: scikit-image
+Requires-Dist: tensorflow
+Requires-Dist: keras
 
 # Dataset Iterator
 This repo contains keras iterator classes for multi-channel (time-lapse) images contained in dataset files such as hdf5.
 
 ## Dataset structure:
 One dataset file can contain several sub-datasets (dataset_name0, dataset_name1, etc...), the iterator will iterate through all of them as if they were concatenated.
 
@@ -70,9 +75,7 @@
 - There is currently an implementation of DatasetIO for .h5 files (`H5pyIO`), as well as dataset composed of multiple images files supported by PILLOW (`MultipleFileIO`).
 - one can also concatenate datasets from different files:
   - if a dataset is split into several files that contain the same channels: use `ConcatenateDatasetIO`
   - if a dataset contains channels in different files, use: `MultipleDatasetIO`
 
 # Demo
 See this notebook for a demo: [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1J-UPivwyNTpyLhOMfzhfG0pIl6gDD9I5)
-
-
```

### Comparing `dataset_iterator-0.3.6/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.3.8/dataset_iterator.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 setup.py
 dataset_iterator/__init__.py
 dataset_iterator/concat_iterator.py
+dataset_iterator/hard_sample_mining.py
 dataset_iterator/helpers.py
 dataset_iterator/image_data_generator.py
 dataset_iterator/index_array_iterator.py
 dataset_iterator/multichannel_iterator.py
 dataset_iterator/pre_processing.py
 dataset_iterator/tile_utils.py
 dataset_iterator/tracking_iterator.py
```

### Comparing `dataset_iterator-0.3.6/setup.py` & `dataset_iterator-0.3.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.3.6",
+    version="0.3.8",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
-    description="data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files. Based on tensorflow.keras.preprocessing.image.Iterator",
+    description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url = 'https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.4.tar.gz',
-    keywords = ['Iterator', 'Dataset', 'Image', 'Numpy'],
+    download_url='https://files.pythonhosted.org/packages/b3/1c/6383e70b8d6e409fe1e3a774d659ff0fc7fa7933a88dd199a6e48319df8b/dataset_iterator-0.3.9.tar.gz',
+    keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

