# Comparing `tmp/stacci-0.9.4.tar.gz` & `tmp/stacci-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stacci-0.9.4.tar", max compression
+gzip compressed data, was "stacci-0.9.5.tar", max compression
```

## Comparing `stacci-0.9.4.tar` & `stacci-0.9.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6004 2024-03-29 08:44:39.782535 stacci-0.9.4/README.md
--rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.4/STACCI/__init__.py
--rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/ccci.py
--rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.4/STACCI/data_handler.py
--rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.4/STACCI/model.py
--rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.4/STACCI/pipeline.py
--rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/pl.py
--rw-r--r--   0        0        0     5219 2024-03-15 15:22:41.667792 stacci-0.9.4/STACCI/tl.py
--rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.4/STACCI/trainer.py
--rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.4/STACCI/utils.py
--rw-r--r--   0        0        0      773 2024-04-10 12:58:04.110833 stacci-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     7396 1970-01-01 00:00:00.000000 stacci-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     6538 2024-04-12 08:06:34.968381 stacci-0.9.5/README.md
+-rw-r--r--   0        0        0      166 2024-03-15 15:29:04.555776 stacci-0.9.5/STACCI/__init__.py
+-rw-r--r--   0        0        0    39940 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/ccci.py
+-rw-r--r--   0        0        0    10212 2024-03-15 16:51:31.767571 stacci-0.9.5/STACCI/data_handler.py
+-rw-r--r--   0        0        0     6378 2024-03-15 16:45:15.675586 stacci-0.9.5/STACCI/model.py
+-rw-r--r--   0        0        0     6734 2024-03-29 08:19:04.442599 stacci-0.9.5/STACCI/pipeline.py
+-rw-r--r--   0        0        0    65268 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/pl.py
+-rw-r--r--   0        0        0     5219 2024-03-15 15:22:41.667792 stacci-0.9.5/STACCI/tl.py
+-rw-r--r--   0        0        0     3765 2024-03-15 16:46:00.507584 stacci-0.9.5/STACCI/trainer.py
+-rw-r--r--   0        0        0    32812 2024-03-29 08:35:18.818558 stacci-0.9.5/STACCI/utils.py
+-rw-r--r--   0        0        0      773 2024-04-12 07:48:02.180427 stacci-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     7930 1970-01-01 00:00:00.000000 stacci-0.9.5/PKG-INFO
```

### Comparing `stacci-0.9.4/README.md` & `stacci-0.9.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# STACCI for STCase
-# Installation Instructions
+[![Stars](https://img.shields.io/github/stars/Lzcstan/STCase?logo=GitHub&color=yellow)](https://github.com/Lzcstan/STCase) [![PyPI](https://img.shields.io/pypi/v/STACCI.svg)](https://pypi.org/project/STACCI)
+# STACCI for STCase (**S**patial **T**ranscriptomics cell-cell **C**ommunication **a**nd **s**ubtype **e**xploration)
+STACCI (**S**patial **T**ranscriptomics **A**nalysis for **C**ell-**C**ell **I**nteractions)
+
+## Installation Instructions
 
 1. Clone the repository to your local machine and enter the repository in the command line interface.
 2. Use conda to create a new environment according to environment.yml
 
    `conda env create -f environment.yml`
 
    The purpose of this step is to install python, cudatoolkit and cudnn, where the versions of cudatoolkit and cudnn must correspond. The version in the .yml file is applicable to hosts with cuda ≥ 11.3. For servers with cuda lower than this version, consider upgrading cuda or finding the corresponding cudatoolkit version and cudnn version.
@@ -65,15 +68,15 @@
    Enter `R` in bash to enter the command line interactive interface and install `mclust` with this command:
    `install.packages("mclust")`
    During the installation process, select CRAN mirror: China (Beijing 3) [https].
 
    After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `ctrl+d` to exit R.
 5. `pip install STACCI`
 
-# Usage Instructions
+## Usage Instructions
 
 After creating a new environment according to the installation instructions and installing the corresponding dependencies, place the .h5ad file of the dataset in the specified file structure, specifically, the desired file structure of the dataset is as follows:
 
 ```bash
 {root}
 └── {dataset_path}
     └── {dataset}
@@ -111,7 +114,10 @@
 │   ├── trainer.py
 │   └── utils.py
 └── tests/
     └── datasets/
         └── 10xv4_n0_v3/
             └── 10xv4_n0_v3_stringent_self.h5ad
 ```
+
+## Tutorial
+A consice read-the-doc tutorial can be found in [this website](https://stcase.readthedocs.io/en/latest/) (in progress).
```

### Comparing `stacci-0.9.4/STACCI/ccci.py` & `stacci-0.9.5/STACCI/ccci.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/data_handler.py` & `stacci-0.9.5/STACCI/data_handler.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/model.py` & `stacci-0.9.5/STACCI/model.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/pipeline.py` & `stacci-0.9.5/STACCI/pipeline.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/pl.py` & `stacci-0.9.5/STACCI/pl.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/tl.py` & `stacci-0.9.5/STACCI/tl.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/trainer.py` & `stacci-0.9.5/STACCI/trainer.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/STACCI/utils.py` & `stacci-0.9.5/STACCI/utils.py`

 * *Files identical despite different names*

### Comparing `stacci-0.9.4/pyproject.toml` & `stacci-0.9.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "STACCI"
-version = "0.9.4"
+version = "0.9.5"
 description = "STACCI for STCase"
 authors = ["Lzcstan <lzcstan@outlook.com>"]
 readme = "README.md"
 packages = [
   { include = "STACCI", from = "." },
 ]
```

### Comparing `stacci-0.9.4/PKG-INFO` & `stacci-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: STACCI
-Version: 0.9.4
+Version: 0.9.5
 Summary: STACCI for STCase
 Author: Lzcstan
 Author-email: lzcstan@outlook.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -39,16 +39,19 @@
 Requires-Dist: torch-geometric
 Requires-Dist: torch-scatter
 Requires-Dist: torch-sparse
 Requires-Dist: torch-spline-conv
 Project-URL: repository, https://github.com/Lzcstan/STACCI
 Description-Content-Type: text/markdown
 
-# STACCI for STCase
-# Installation Instructions
+[![Stars](https://img.shields.io/github/stars/Lzcstan/STCase?logo=GitHub&color=yellow)](https://github.com/Lzcstan/STCase) [![PyPI](https://img.shields.io/pypi/v/STACCI.svg)](https://pypi.org/project/STACCI)
+# STACCI for STCase (**S**patial **T**ranscriptomics cell-cell **C**ommunication **a**nd **s**ubtype **e**xploration)
+STACCI (**S**patial **T**ranscriptomics **A**nalysis for **C**ell-**C**ell **I**nteractions)
+
+## Installation Instructions
 
 1. Clone the repository to your local machine and enter the repository in the command line interface.
 2. Use conda to create a new environment according to environment.yml
 
    `conda env create -f environment.yml`
 
    The purpose of this step is to install python, cudatoolkit and cudnn, where the versions of cudatoolkit and cudnn must correspond. The version in the .yml file is applicable to hosts with cuda ≥ 11.3. For servers with cuda lower than this version, consider upgrading cuda or finding the corresponding cudatoolkit version and cudnn version.
@@ -110,15 +113,15 @@
    Enter `R` in bash to enter the command line interactive interface and install `mclust` with this command:
    `install.packages("mclust")`
    During the installation process, select CRAN mirror: China (Beijing 3) [https].
 
    After the installation is done, enter the command `library(mclust)` to load. If the `mclust` logo is displayed, it means the installation is successful. You can press `ctrl+d` to exit R.
 5. `pip install STACCI`
 
-# Usage Instructions
+## Usage Instructions
 
 After creating a new environment according to the installation instructions and installing the corresponding dependencies, place the .h5ad file of the dataset in the specified file structure, specifically, the desired file structure of the dataset is as follows:
 
 ```bash
 {root}
 └── {dataset_path}
     └── {dataset}
@@ -157,7 +160,9 @@
 │   └── utils.py
 └── tests/
     └── datasets/
         └── 10xv4_n0_v3/
             └── 10xv4_n0_v3_stringent_self.h5ad
 ```
 
+## Tutorial
+A consice read-the-doc tutorial can be found in [this website](https://stcase.readthedocs.io/en/latest/) (in progress).
```

