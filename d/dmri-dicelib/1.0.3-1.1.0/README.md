# Comparing `tmp/dmri-dicelib-1.0.3.tar.gz` & `tmp/dmri-dicelib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmri-dicelib-1.0.3.tar", last modified: Wed Nov  1 14:29:02 2023, max compression
+gzip compressed data, was "dmri-dicelib-1.1.0.tar", last modified: Fri Apr 12 14:11:46 2024, max compression
```

## Comparing `dmri-dicelib-1.0.3.tar` & `dmri-dicelib-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.819620 dmri-dicelib-1.0.3/
--rw-rw-rw-   0        0        0     4495 2023-10-16 14:55:58.000000 dmri-dicelib-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       47 2023-10-17 10:21:56.000000 dmri-dicelib-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1988 2023-11-01 14:29:02.819620 dmri-dicelib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.677155 dmri-dicelib-1.0.3/bin/
--rw-rw-rw-   0        0        0     2366 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_image_extract.py
--rw-rw-rw-   0        0        0     3722 2023-10-16 14:52:01.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_assign.py
--rw-rw-rw-   0        0        0     4262 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_cluster.py
--rw-rw-rw-   0        0        0     3993 2023-10-16 14:52:01.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_compress.py
--rw-rw-rw-   0        0        0     3779 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_convert.py
--rw-rw-rw-   0        0        0     3709 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_filter.py
--rw-rw-rw-   0        0        0     1715 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_indices.py
--rw-rw-rw-   0        0        0      905 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_info.py
--rw-rw-rw-   0        0        0     3464 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_join.py
--rw-rw-rw-   0        0        0     1878 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_lengths.py
--rw-rw-rw-   0        0        0     1785 2023-10-16 14:52:01.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_sanitize.py
--rw-rw-rw-   0        0        0     2414 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_smooth.py
--rw-rw-rw-   0        0        0     2537 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_split.py
--rw-rw-rw-   0        0        0     4043 2023-10-16 14:52:01.000000 dmri-dicelib-1.0.3/bin/dice_tractogram_tsf.py
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.771818 dmri-dicelib-1.0.3/dicelib/
--rw-rw-rw-   0        0        0    10541 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/Tsf.pyx
--rw-rw-rw-   0        0        0      321 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/__init__.py
--rw-rw-rw-   0        0        0    30049 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/clustering.pyx
--rw-rw-rw-   0        0        0    11898 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/connectivity.pyx
--rw-rw-rw-   0        0        0     3226 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/image.pyx
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.787445 dmri-dicelib-1.0.3/dicelib/include/
--rw-rw-rw-   0        0        0     7506 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/include/Catmull.h
--rw-rw-rw-   0        0        0     2645 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/include/Vector.h
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.803967 dmri-dicelib-1.0.3/dicelib/include/psimpl_v7_src/
--rw-rw-rw-   0        0        0    85996 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/include/psimpl_v7_src/psimpl.h
--rw-rw-rw-   0        0        0      929 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/info.py
--rw-rw-rw-   0        0        0     1399 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/lazytractogram.pxd
--rw-rw-rw-   0        0        0    17393 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/lazytractogram.pyx
--rw-rw-rw-   0        0        0     5816 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/smoothing.pyx
--rw-rw-rw-   0        0        0     3484 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/split_cluster.pyx
--rw-rw-rw-   0        0        0     2646 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/streamline.hpp
--rw-rw-rw-   0        0        0     7563 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/streamline.pyx
--rw-rw-rw-   0        0        0    52078 2023-10-17 10:20:39.000000 dmri-dicelib-1.0.3/dicelib/tractogram.pyx
--rw-rw-rw-   0        0        0    12473 2023-10-31 11:02:30.000000 dmri-dicelib-1.0.3/dicelib/ui.py
-drwxrwxrwx   0        0        0        0 2023-11-01 14:29:02.819620 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/
--rw-rw-rw-   0        0        0     1988 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1086 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       63 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-01 14:29:02.000000 dmri-dicelib-1.0.3/dmri_dicelib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1453 2023-11-01 14:29:02.819620 dmri-dicelib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3963 2023-10-16 14:51:34.000000 dmri-dicelib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.109386 dmri-dicelib-1.1.0/
+-rw-rw-rw-   0        0        0     4495 2023-10-16 14:55:58.000000 dmri-dicelib-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2024-04-12 13:58:44.000000 dmri-dicelib-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7276 2024-04-12 14:11:46.108383 dmri-dicelib-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-10-16 14:51:34.000000 dmri-dicelib-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.064267 dmri-dicelib-1.1.0/dicelib/
+-rw-rw-rw-   0        0        0      316 2024-04-12 13:58:44.000000 dmri-dicelib-1.1.0/dicelib/__init__.py
+-rw-rw-rw-   0        0        0    41361 2024-04-11 15:37:10.000000 dmri-dicelib-1.1.0/dicelib/clustering.pyx
+-rw-rw-rw-   0        0        0      377 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/connectivity.pxd
+-rw-rw-rw-   0        0        0    38211 2024-04-11 09:22:23.000000 dmri-dicelib-1.1.0/dicelib/connectivity.pyx
+-rw-rw-rw-   0        0        0     3667 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/image.pyx
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.067275 dmri-dicelib-1.1.0/dicelib/include/
+-rw-rw-rw-   0        0        0     7506 2024-02-14 16:11:18.000000 dmri-dicelib-1.1.0/dicelib/include/Catmull.h
+-rw-rw-rw-   0        0        0     2645 2024-02-14 16:11:18.000000 dmri-dicelib-1.1.0/dicelib/include/Vector.h
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.067275 dmri-dicelib-1.1.0/dicelib/include/psimpl_v7_src/
+-rw-rw-rw-   0        0        0    85996 2024-02-14 16:11:18.000000 dmri-dicelib-1.1.0/dicelib/include/psimpl_v7_src/psimpl.h
+-rw-rw-rw-   0        0        0     4912 2024-04-11 11:44:12.000000 dmri-dicelib-1.1.0/dicelib/include/streamline_utils.hpp
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.071288 dmri-dicelib-1.1.0/dicelib/scripts/
+-rw-rw-rw-   0        0        0     2678 2024-04-12 13:10:52.000000 dmri-dicelib-1.1.0/dicelib/scripts/dice_connectome.py
+-rw-rw-rw-   0        0        0     1040 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/scripts/dice_image.py
+-rw-rw-rw-   0        0        0    23661 2024-04-12 13:58:53.000000 dmri-dicelib-1.1.0/dicelib/scripts/dice_tractogram.py
+-rw-rw-rw-   0        0        0      318 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/streamline.pxd
+-rw-rw-rw-   0        0        0    21075 2024-04-12 13:58:53.000000 dmri-dicelib-1.1.0/dicelib/streamline.pyx
+-rw-rw-rw-   0        0        0     1359 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/tractogram.pxd
+-rw-rw-rw-   0        0        0   119686 2024-04-12 13:58:53.000000 dmri-dicelib-1.1.0/dicelib/tractogram.pyx
+-rw-rw-rw-   0        0        0    10453 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/dicelib/tsf.pyx
+-rw-rw-rw-   0        0        0    50657 2024-04-11 15:37:10.000000 dmri-dicelib-1.1.0/dicelib/ui.py
+-rw-rw-rw-   0        0        0     5333 2024-04-12 13:58:44.000000 dmri-dicelib-1.1.0/dicelib/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:11:46.107380 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/
+-rw-rw-rw-   0        0        0     7276 2024-04-12 14:11:45.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-04-12 14:11:46.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:11:45.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1442 2024-04-12 14:11:45.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2024-04-12 14:11:45.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 14:11:45.000000 dmri-dicelib-1.1.0/dmri_dicelib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3192 2024-04-10 09:53:34.000000 dmri-dicelib-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:11:46.110388 dmri-dicelib-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3152 2024-04-09 08:21:40.000000 dmri-dicelib-1.1.0/setup.py
```

### Comparing `dmri-dicelib-1.0.3/LICENSE` & `dmri-dicelib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmri-dicelib-1.0.3/README.md` & `dmri-dicelib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dmri-dicelib-1.0.3/dicelib/Tsf.pyx` & `dmri-dicelib-1.1.0/dicelib/tsf.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!python
 # cython: language_level=3, c_string_type=str, c_string_encoding=ascii, boundscheck=False, wraparound=False, profile=False, nonecheck=False, cdivision=True, initializedcheck=False, binding=False
-cimport cython
-import numpy as np
-cimport numpy as np
-from libc.stdio cimport fopen, fclose, FILE, fseek, SEEK_END, SEEK_SET
-from libc.stdio cimport fgets, fread, fwrite
-from libc.stdlib cimport malloc, free
-from libc.string cimport strlen, strncmp, strchr
-from libcpp.string cimport string
-from libc.math cimport isnan, isinf, NAN
+
+from dicelib.tractogram import LazyTractogram
+
 import os
-from dicelib.lazytractogram import LazyTractogram
 import time
 
+from libc.math cimport isinf, isnan, NAN
+from libc.stdio cimport fclose, fgets, FILE, fopen, fread, fseek, fwrite, SEEK_END, SEEK_SET
+from libc.stdlib cimport free, malloc
+from libc.string cimport strchr, strlen, strncmp 
+from libcpp.string cimport string
+
 cdef float[1] NAN1 = {NAN}
 
 cdef class Tsf:
     """Class to read/write tsf files for visualization.
 
     A file can be opened in three different modalities:
     - 'r': reading
```

### Comparing `dmri-dicelib-1.0.3/dicelib/include/Catmull.h` & `dmri-dicelib-1.1.0/dicelib/include/Catmull.h`

 * *Files identical despite different names*

### Comparing `dmri-dicelib-1.0.3/dicelib/include/Vector.h` & `dmri-dicelib-1.1.0/dicelib/include/Vector.h`

 * *Files identical despite different names*

### Comparing `dmri-dicelib-1.0.3/dicelib/include/psimpl_v7_src/psimpl.h` & `dmri-dicelib-1.1.0/dicelib/include/psimpl_v7_src/psimpl.h`

 * *Files identical despite different names*

### Comparing `dmri-dicelib-1.0.3/dicelib/lazytractogram.pxd` & `dmri-dicelib-1.1.0/dicelib/tractogram.pxd`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-#!python
 # cython: boundscheck=False, wraparound=False, profile=False, language_level=3
 
-
-from libc.stdio cimport fopen, fclose, FILE#, fseek, SEEK_END, SEEK_SET
+from libc.stdio cimport fclose, FILE, fopen
 
 cdef class LazyTractogram:
     cdef readonly   str                             filename
     cdef readonly   str                             suffix
     cdef readonly   dict                            header
     cdef readonly   str                             mode
     cdef readonly   bint                            is_open
```

### Comparing `dmri-dicelib-1.0.3/setup.py` & `dmri-dicelib-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,32 +5,25 @@
 from shutil import rmtree
 
 # name of the package
 package_name = 'dicelib'
 
 
 def get_extensions():
-    lazytractogram = Extension(
-        name=f'{package_name}.lazytractogram',
-        sources=[f'{package_name}/lazytractogram.pyx'],
-        include_dirs=[get_include()],
-        extra_compile_args=['-w', '-std=c++11', '-g0'],
-        language='c++'
-    )
     image = Extension(
         name=f'{package_name}.image',
         sources=[f'{package_name}/image.pyx'],
         include_dirs=[get_include()],
         extra_compile_args=['-w', '-std=c++11', '-g0'],
         language='c++'
     )
     streamline = Extension(
         name=f'{package_name}.streamline',
         sources=[f'{package_name}/streamline.pyx'],
-        include_dirs=[get_include()],
+        include_dirs=[get_include(), f'{package_name}/include'],
         extra_compile_args=['-w', '-std=c++11', '-g0'],
         language='c++'
     )
     tractogram = Extension(
         name=f'{package_name}.tractogram',
         sources=[f'{package_name}/tractogram.pyx'],
         include_dirs=[get_include()],
@@ -46,36 +39,23 @@
     connectivity = Extension(
         name=f'{package_name}.connectivity',
         sources=['dicelib/connectivity.pyx'],
         include_dirs=[get_include()],
         extra_compile_args=['-w', '-std=c++11'],
         language='c++',
     )
-    split_cluster = Extension(
-        name=f'{package_name}.split_cluster',
-        sources=[f'{package_name}/split_cluster.pyx'],
-        include_dirs=[get_include()],
-        extra_compile_args=['-w', '-std=c++11'],
-        language='c++',
-    )
     tsf = Extension(
         name=f'{package_name}.tsf',
-        sources=[f'{package_name}/Tsf.pyx'],
+        sources=[f'{package_name}/tsf.pyx'],
         include_dirs=[get_include()],
         extra_compile_args=['-w', '-std=c++11'],
         language='c++',
     )
-    smoothing = Extension(
-        name=f'{package_name}.smoothing',
-        sources=[f'{package_name}/smoothing.pyx'],
-        include_dirs=[get_include()],
-        extra_compile_args=['-w', '-std=c++11'],
-        language='c++',
-    )
-    return [ lazytractogram, image, streamline, tractogram, clustering, split_cluster, connectivity, tsf, smoothing ]
+
+    return [image, streamline, tractogram, clustering, connectivity, tsf]
 
 
 class CustomBuildExtCommand(build_ext):
     """build_ext command to use when numpy headers are needed"""
 
     def run(self):
         # Now that the requirements are installed, get everything from numpy
@@ -109,10 +89,9 @@
         rmtree('./build', ignore_errors=True)
 
 setup(
     cmdclass={
         'build_ext': CustomBuildExtCommand,
         'clean': CleanCommand
     },
-    ext_modules=get_extensions(),
-    scripts=glob('bin/*.py')
+    ext_modules=get_extensions()
 )
```

