# Comparing `tmp/titiler.extensions-0.18.0.tar.gz` & `tmp/titiler.extensions-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.extensions-0.18.0.tar", last modified: Fri Mar 22 17:58:28 2024, max compression
+gzip compressed data, was "titiler.extensions-0.18.1.tar", last modified: Fri Apr 12 16:38:00 2024, max compression
```

## Comparing `titiler.extensions-0.18.0.tar` & `titiler.extensions-0.18.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4704 2024-03-22 17:57:55.235572 titiler.extensions-0.18.0/README.md
--rw-r--r--   0        0        0     1762 2024-03-22 17:57:55.235572 titiler.extensions-0.18.0/pyproject.toml
--rw-r--r--   0        0        0      244 2024-03-22 17:57:55.247572 titiler.extensions-0.18.0/titiler/extensions/__init__.py
--rw-r--r--   0        0        0     1236 2024-03-22 17:57:55.247572 titiler.extensions-0.18.0/titiler/extensions/cogeo.py
--rw-r--r--   0        0        0        0 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/py.typed
--rw-r--r--   0        0        0     6098 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/stac.py
--rw-r--r--   0        0        0    29418 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/templates/cog_viewer.html
--rw-r--r--   0        0        0    33936 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/templates/stac_viewer.html
--rw-r--r--   0        0        0     2471 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.0.0.xml
--rw-r--r--   0        0        0     3069 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.1.1.xml
--rw-r--r--   0        0        0     3820 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.3.0.xml
--rw-r--r--   0        0        0     2340 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/viewer.py
--rw-r--r--   0        0        0    23213 2024-03-22 17:57:55.251572 titiler.extensions-0.18.0/titiler/extensions/wms.py
--rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 titiler.extensions-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0     4704 2024-04-12 16:37:28.709344 titiler.extensions-0.18.1/README.md
+-rw-r--r--   0        0        0     1762 2024-04-12 16:37:28.709344 titiler.extensions-0.18.1/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/__init__.py
+-rw-r--r--   0        0        0     1236 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/cogeo.py
+-rw-r--r--   0        0        0        0 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/py.typed
+-rw-r--r--   0        0        0     6098 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/stac.py
+-rw-r--r--   0        0        0    29418 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/templates/cog_viewer.html
+-rw-r--r--   0        0        0    33936 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/templates/stac_viewer.html
+-rw-r--r--   0        0        0     2471 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.0.0.xml
+-rw-r--r--   0        0        0     3069 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.1.1.xml
+-rw-r--r--   0        0        0     3820 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.3.0.xml
+-rw-r--r--   0        0        0     2340 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/viewer.py
+-rw-r--r--   0        0        0    23213 2024-04-12 16:37:28.725344 titiler.extensions-0.18.1/titiler/extensions/wms.py
+-rw-r--r--   0        0        0     5931 1970-01-01 00:00:00.000000 titiler.extensions-0.18.1/PKG-INFO
```

### Comparing `titiler.extensions-0.18.0/README.md` & `titiler.extensions-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/pyproject.toml` & `titiler.extensions-0.18.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = []
 dependencies = [
-    "titiler.core==0.18.0",
+    "titiler.core==0.18.1",
 ]
-version = "0.18.0"
+version = "0.18.1"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 test = [
     "pytest",
```

### Comparing `titiler.extensions-0.18.0/titiler/extensions/cogeo.py` & `titiler.extensions-0.18.1/titiler/extensions/cogeo.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/stac.py` & `titiler.extensions-0.18.1/titiler/extensions/stac.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/templates/cog_viewer.html` & `titiler.extensions-0.18.1/titiler/extensions/templates/cog_viewer.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/templates/stac_viewer.html` & `titiler.extensions-0.18.1/titiler/extensions/templates/stac_viewer.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.0.0.xml` & `titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.1.1.xml` & `titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/templates/wms_1.3.0.xml` & `titiler.extensions-0.18.1/titiler/extensions/templates/wms_1.3.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/viewer.py` & `titiler.extensions-0.18.1/titiler/extensions/viewer.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/titiler/extensions/wms.py` & `titiler.extensions-0.18.1/titiler/extensions/wms.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.18.0/PKG-INFO` & `titiler.extensions-0.18.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.extensions
-Version: 0.18.0
+Version: 0.18.1
 Summary: Extensions for TiTiler Factories.
 License: MIT
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,GDAL,Rasterio,OGC
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

