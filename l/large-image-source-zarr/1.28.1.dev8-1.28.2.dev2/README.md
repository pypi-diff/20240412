# Comparing `tmp/large-image-source-zarr-1.28.1.dev8.tar.gz` & `tmp/large-image-source-zarr-1.28.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-zarr-1.28.1.dev8.tar", last modified: Wed Apr 10 16:17:19 2024, max compression
+gzip compressed data, was "large-image-source-zarr-1.28.2.dev2.tar", last modified: Fri Apr 12 15:26:30 2024, max compression
```

## Comparing `large-image-source-zarr-1.28.1.dev8.tar` & `large-image-source-zarr-1.28.2.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-10 16:17:18.000000 large-image-source-zarr-1.28.1.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-10 16:17:18.000000 large-image-source-zarr-1.28.1.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.125867 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    34406 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-10 16:17:19.000000 large-image-source-zarr-1.28.1.dev8/large_image_source_zarr.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 16:17:19.129867 large-image-source-zarr-1.28.1.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2024-04-10 16:11:56.000000 large-image-source-zarr-1.28.1.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34406 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      342 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      123 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-12 15:26:30.000000 large-image-source-zarr-1.28.2.dev2/large_image_source_zarr.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 15:26:30.322804 large-image-source-zarr-1.28.2.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2705 2024-04-12 15:20:51.000000 large-image-source-zarr-1.28.2.dev2/setup.py
```

### Comparing `large-image-source-zarr-1.28.1.dev8/LICENSE` & `large-image-source-zarr-1.28.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.1.dev8/README.rst` & `large-image-source-zarr-1.28.2.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-zarr-1.28.1.dev8/large_image_source_zarr/__init__.py` & `large-image-source-zarr-1.28.2.dev2/large_image_source_zarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -769,15 +769,15 @@
             else:
                 raise TileSourceError('Output path exists (%s).' % str(path))
 
         suffix = Path(path).suffix
         source = self
 
         if self.crop:
-            top, left, height, width = self.crop
+            left, top, width, height = self.crop
             source = new()
             source._zarr.attrs.update(self._zarr.attrs)
             for frame in self.getMetadata().get('frames', [{'Index': 0}]):
                 frame_position = {
                     k.replace('Index', '').lower(): v
                     for k, v in frame.items()
                     if k.replace('Index', '').lower() in self._axes
```

### Comparing `large-image-source-zarr-1.28.1.dev8/setup.py` & `large-image-source-zarr-1.28.2.dev2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,17 @@
         'zarr',
         # I am uncertain why this is required, since numcodecs is required by
         # zarr; but without it some jpeg encoded data cannot be read
         'imagecodecs-numcodecs',
     ],
     extras_require={
         'girder': f'girder-large-image{limit_version}',
+        'all': [
+            'large-image-converter',
+        ],
     },
     keywords='large_image, tile source',
     packages=find_packages(exclude=['test', 'test.*']),
     url='https://github.com/girder/large_image',
     python_requires='>=3.6',
     entry_points={
         'large_image.source': [
```

