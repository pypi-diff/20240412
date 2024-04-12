# Comparing `tmp/datav-0.1.5.tar.gz` & `tmp/datav-0.2.0.tar.gz`

## Comparing `datav-0.1.5.tar` & `datav-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 datav-0.1.5/CHANGELOG
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 datav-0.1.5/requirements-dev.lock
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 datav-0.1.5/requirements.lock
--rw-r--r--   0        0        0  1132280 2020-02-02 00:00:00.000000 datav-0.1.5/research_site.png
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 datav-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 datav-0.1.5/.github/workflows/qa.yml
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 datav-0.1.5/examples/alaer.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 datav-0.1.5/src/datav/__init__.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 datav-0.1.5/src/datav/downloader.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 datav-0.1.5/src/datav/feature.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 datav-0.1.5/.gitignore
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 datav-0.1.5/LICENSE
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 datav-0.1.5/README.md
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 datav-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 datav-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 datav-0.2.0/.Rprofile
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 datav-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 datav-0.2.0/CHANGELOG
+-rw-r--r--   0        0        0   322188 2020-02-02 00:00:00.000000 datav-0.2.0/ancestry1.pdf
+-rw-r--r--   0        0        0    11072 2020-02-02 00:00:00.000000 datav-0.2.0/renv.lock
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 datav-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 datav-0.2.0/requirements.lock
+-rw-r--r--   0        0        0  1132280 2020-02-02 00:00:00.000000 datav-0.2.0/research_site.png
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 datav-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 datav-0.2.0/.github/workflows/qa.yml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 datav-0.2.0/examples/alaer.py
+-rw-r--r--   0        0        0   241655 2020-02-02 00:00:00.000000 datav-0.2.0/examples/tess3r.ipynb
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 datav-0.2.0/renv/.gitignore
+-rw-r--r--   0        0        0    27992 2020-02-02 00:00:00.000000 datav-0.2.0/renv/activate.R
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 datav-0.2.0/renv/settings.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 datav-0.2.0/src/datav/__init__.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 datav-0.2.0/src/datav/downloader.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 datav-0.2.0/src/datav/feature.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 datav-0.2.0/src/datav/plot.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 datav-0.2.0/.gitignore
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 datav-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 datav-0.2.0/README.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 datav-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13658 2020-02-02 00:00:00.000000 datav-0.2.0/PKG-INFO
```

### Comparing `datav-0.1.5/CHANGELOG` & `datav-0.2.0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/research_site.png` & `datav-0.2.0/research_site.png`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/.github/workflows/python-publish.yml` & `datav-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/.github/workflows/qa.yml` & `datav-0.2.0/.github/workflows/qa.yml`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/examples/alaer.py` & `datav-0.2.0/examples/alaer.py`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/src/datav/downloader.py` & `datav-0.2.0/src/datav/downloader.py`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/src/datav/feature.py` & `datav-0.2.0/src/datav/feature.py`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/LICENSE` & `datav-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/README.md` & `datav-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datav-0.1.5/pyproject.toml` & `datav-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [project]
 name = "datav"
-version = "0.1.5"
+version = "0.2.0"
 description = "Data visualization tools for Python."
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [{ name = "Tang Ziya", email = "tcztzy@gmail.com" }]
 dependencies = [
     "cartopy>=0.22",
+    "scikit-learn>=1.4.2",
+    "geopandas>=0.14.3",
+    "xarray>=2024.3.0",
+    "matplotlib>=3.8.4",
+    "numpy>=1.26.4",
 ]
 classifiers = [
     "Framework :: Matplotlib",
     "Natural Language :: Chinese (Simplified)",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: Free For Educational Use",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [build-system]
@@ -30,14 +34,16 @@
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pytest>=7.4.0",
     "pytest-cov>=4.1.0",
     "ruff>=0.0.280",
+    "rpy2>=3.5.16",
+    "ipykernel>=6.29.4",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --cov=src"
 testpaths = [
     "src",
 ]
```

### Comparing `datav-0.1.5/PKG-INFO` & `datav-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: datav
-Version: 0.1.5
+Version: 0.2.0
 Summary: Data visualization tools for Python.
 Author-email: Tang Ziya <tcztzy@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -172,21 +172,25 @@
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free For Educational Use
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: cartopy>=0.22
+Requires-Dist: geopandas>=0.14.3
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: xarray>=2024.3.0
 Description-Content-Type: text/markdown
 
 DataV
 -----
 ![PyPI](https://img.shields.io/pypi/v/datav)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datav)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/datav)
```

