# Comparing `tmp/ndbioimage-2024.4.5.tar.gz` & `tmp/ndbioimage-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.5.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.6.tar", max compression
```

## Comparing `ndbioimage-2024.4.5.tar` & `ndbioimage-2024.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.5/LICENSE
--rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.5/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.5/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    54071 2024-04-12 13:42:57.566891 ndbioimage-2024.4.5/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.5/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.5/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.5/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    29149 2024-04-12 14:01:22.722103 ndbioimage-2024.4.5/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.5/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.5/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.5/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.5/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.5/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.5/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1246 2024-04-12 13:36:02.623186 ndbioimage-2024.4.5/pyproject.toml
--rw-r--r--   0        0        0     4066 1970-01-01 00:00:00.000000 ndbioimage-2024.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.6/LICENSE
+-rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.6/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.6/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54071 2024-04-12 13:42:57.566891 ndbioimage-2024.4.6/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.6/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.6/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.6/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    29149 2024-04-12 14:01:22.722103 ndbioimage-2024.4.6/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.6/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.6/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.6/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.6/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.6/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.6/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1241 2024-04-12 15:38:36.426189 ndbioimage-2024.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 ndbioimage-2024.4.6/PKG-INFO
```

### Comparing `ndbioimage-2024.4.5/LICENSE` & `ndbioimage-2024.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/README.md` & `ndbioimage-2024.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/.DS_Store` & `ndbioimage-2024.4.6/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/__init__.py` & `ndbioimage-2024.4.6/ndbioimage/__init__.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/jvm.py` & `ndbioimage-2024.4.6/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.6/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/ndbioimage/transforms.py` & `ndbioimage-2024.4.6/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.5/pyproject.toml` & `ndbioimage-2024.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.5"
+version = "2024.4.6"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
 exclude = ["ndbioimage/jars"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 numpy = "*"
 pandas = "*"
 tifffile = "*"
 czifile = "2019.7.2"
 tiffwrite = "*"
 ome-types = "^0.4.0"
 pint = "*"
@@ -31,15 +31,15 @@
 ]
 scikit-image = "*"
 imagecodecs = "*"
 xsdata = "^23"  # until pydantic is up-to-date
 pytest = { version = "*", optional = true }
 
 [tool.poetry.extras]
-test = ["pytest-xdist"]
+test = ["pytest"]
 
 [tool.poetry.scripts]
 ndbioimage = "ndbioimage:main"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore:::(colorcet)"]
```

### Comparing `ndbioimage-2024.4.5/PKG-INFO` & `ndbioimage-2024.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: test
 Requires-Dist: JPype1
 Requires-Dist: SimpleITK-SimpleElastix ; platform_machine == "aarch64" and python_version >= "3.12"
 Requires-Dist: SimpleITK-SimpleElastix ; python_version < "3.12"
@@ -24,15 +22,15 @@
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
 Requires-Dist: numpy
 Requires-Dist: ome-types (>=0.4.0,<0.5.0)
 Requires-Dist: pandas
 Requires-Dist: parfor (>=2024.3.0)
 Requires-Dist: pint
-Requires-Dist: pytest
+Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pyyaml
 Requires-Dist: scikit-image
 Requires-Dist: tifffile
 Requires-Dist: tiffwrite
 Requires-Dist: tqdm
 Requires-Dist: xsdata (>=23,<24)
 Project-URL: Repository, https://github.com/wimpomp/ndbioimage
```

