# Comparing `tmp/PheTK-0.1.37.tar.gz` & `tmp/PheTK-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PheTK-0.1.37.tar", last modified: Thu Apr  4 21:00:41 2024, max compression
+gzip compressed data, was "PheTK-0.1.38.tar", last modified: Fri Apr 12 02:58:35 2024, max compression
```

## Comparing `PheTK-0.1.37.tar` & `PheTK-0.1.38.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:41.016559 PheTK-0.1.37/
--rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.37/LICENSE
--rw-r--r--   0 trantac  (1207383791) 1360859114      218 2024-04-04 21:00:41.016392 PheTK-0.1.37/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114    15638 2024-04-04 19:53:54.000000 PheTK-0.1.37/README.md
--rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-04-04 21:00:41.016617 PheTK-0.1.37/setup.cfg
--rw-r--r--   0 trantac  (1207383791) 1360859114      693 2024-04-04 21:00:34.000000 PheTK-0.1.37/setup.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.977319 PheTK-0.1.37/src/
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.982748 PheTK-0.1.37/src/PheTK/
--rw-r--r--   0 trantac  (1207383791) 1360859114    16572 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/Cohort.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/Demo.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/PheWAS.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/Phecode.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/Plot.py
--rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/__init__.py
--rw-r--r--   0 trantac  (1207383791) 1360859114      394 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/_paths.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-04-04 19:02:44.000000 PheTK-0.1.37/src/PheTK/_queries.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.37/src/PheTK/_utils.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:41.010802 PheTK-0.1.37/src/PheTK/phecode/
--rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/phecode/phecode12.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/phecode/phecodeX.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/phecode/phecodeX_WHO.csv
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.984976 PheTK-0.1.37/src/PheTK.egg-info/
--rw-r--r--   0 trantac  (1207383791) 1360859114      218 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/SOURCES.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/dependency_links.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114      115 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/requires.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/top_level.txt
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-12 02:58:35.743464 PheTK-0.1.38/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.38/LICENSE
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16795 2024-04-12 02:58:35.743183 PheTK-0.1.38/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16513 2024-04-12 02:57:43.000000 PheTK-0.1.38/README.md
+-rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-04-12 02:58:35.743531 PheTK-0.1.38/setup.cfg
+-rw-r--r--   0 trantac  (1207383791) 1360859114      934 2024-04-12 02:57:43.000000 PheTK-0.1.38/setup.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-12 02:58:35.689854 PheTK-0.1.38/src/
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-12 02:58:35.702406 PheTK-0.1.38/src/PheTK/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16572 2024-03-25 02:28:39.000000 PheTK-0.1.38/src/PheTK/Cohort.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.38/src/PheTK/Demo.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-04-12 00:30:56.000000 PheTK-0.1.38/src/PheTK/PheWAS.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-04-12 00:30:56.000000 PheTK-0.1.38/src/PheTK/Phecode.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-04-12 00:30:56.000000 PheTK-0.1.38/src/PheTK/Plot.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.38/src/PheTK/__init__.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114      526 2024-04-12 02:27:18.000000 PheTK-0.1.38/src/PheTK/_paths.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-04-12 00:30:56.000000 PheTK-0.1.38/src/PheTK/_queries.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.38/src/PheTK/_utils.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-12 02:58:35.737824 PheTK-0.1.38/src/PheTK/phecode/
+-rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.38/src/PheTK/phecode/phecode12.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.38/src/PheTK/phecode/phecodeX.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.38/src/PheTK/phecode/phecodeX_WHO.csv
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-12 02:58:35.708742 PheTK-0.1.38/src/PheTK.egg-info/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16795 2024-04-12 02:58:35.000000 PheTK-0.1.38/src/PheTK.egg-info/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-04-12 02:58:35.000000 PheTK-0.1.38/src/PheTK.egg-info/SOURCES.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-04-12 02:58:35.000000 PheTK-0.1.38/src/PheTK.egg-info/dependency_links.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114      115 2024-04-12 02:58:35.000000 PheTK-0.1.38/src/PheTK.egg-info/requires.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-04-12 02:58:35.000000 PheTK-0.1.38/src/PheTK.egg-info/top_level.txt
```

### Comparing `PheTK-0.1.37/LICENSE` & `PheTK-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/README.md` & `PheTK-0.1.38/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
 Current version: 0.1.37
 
 ## Changelog:
 
+___version 0.1.38 (11 Apr 2024):___
+- Updated default _All of Us_ ACAF matrix table file path used by .by_genotype() method in Cohort module
+as it was updated by _All of Us_.
+- Updated README to add some minimum VM configuration suggestions.
+
 ___version 0.1.37 (04 Apr 2024):___
 - Removed SNOMED codes from SQL query (_ehr_dx_code_query_) generating _ehr_length_, _dx_code_occurrence_count_, 
 _dx_condition_count_, and _age_at_last_event_ covariates in _.add_covariates()_ method in Cohort module.
   - This was to make it consistent with ICD event query for phecode mapping, 
     i.e., only ICD9CM and ICD10CM would be used as vocabulary_id for these queries.
   - For _All of Us_ users, this change should affect less than 2% of covariate data previously generated 
   by _.add_covariates()_ method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
@@ -33,20 +38,29 @@
 To check current installed version:
 ```
 pip show PheTK | grep Version
 ```
 
 ## 2. SYSTEM REQUIREMENTS
 PheTK was developed for efficient processing of large data while being resource friendly. 
-It was tested on different platforms from laptops to different cloud environments. 
-The lowest test configuration to date was a 4CPU 15GB RAM standard VM on the _All of Us_ researcher workbench 
-for PheWAS of a 200,000+ cohort and 18 covariates. 
+It was tested on different platforms from laptops to different cloud environments.
+
+Here are some minimum VM configuration suggestions for _All of Us_ users:
+- Cohort module: default General Analysis (4 CPUs, 15GB RAM) or Hail Genomic Analysis 
+(main VM and 2 workers of 4 CPUs, 15GB RAM each) VMs should work. 
+Hail Genomic Analysis is only needed for .by_genotype() method.
+- Phecode module: a minimum of 8 CPUs, 30GB RAM standard VM should work for current v7 data.
+This might require more RAM depending on user custom workflow or data - 
+usually Jupyter Python kernel would die at if there is not enough memory.
+- PheWAS module: default General Analysis VM (4 CPUs, 15GB RAM) should work. 
+However, more CPUs would speed up analysis and using low configurations do not necessarily save computing cost
+since total runtime would be longer.
+- Plot module: default General Analysis VM (4 CPUs, 15GB RAM) should work.
 
-Since every platform and every study is different, users could try different available machine configurations
-to achieve optimal performance and cost-effectiveness.
+In practice, users could try different available machine configurations to achieve optimal performance and cost-effectiveness.
 
 ## 3. 1-MINUTE PHEWAS DEMO
 
 User can run the quick 1-minute PheWAS demo with the following command in a terminal:
 
 ```
 python3 -m PheTK.Demo
```

### Comparing `PheTK-0.1.37/setup.py` & `PheTK-0.1.38/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from setuptools import setup, find_packages
 
+# Read contents of the README.md file
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='PheTK',
-    version='0.1.37',
+    version='0.1.38',
+    python_requires='>=3.7',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={
         '': ['*.*'],
         'PheTK': ['phecode/*'],
     },
     url='https://github.com/nhgritctran/PheTK',
     license='GPL-3.0',
     author='Tam Tran',
     author_email='PheTK@mail.nih.gov',
     description='The Phenotype Toolkit',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     install_requires=[
         "adjusttext",
         "connectorx",
         "google-cloud-bigquery",
         "hail",
         "lifelines",
         "matplotlib",
```

### Comparing `PheTK-0.1.37/src/PheTK/Cohort.py` & `PheTK-0.1.38/src/PheTK/Cohort.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/Demo.py` & `PheTK-0.1.38/src/PheTK/Demo.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/PheWAS.py` & `PheTK-0.1.38/src/PheTK/PheWAS.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/Phecode.py` & `PheTK-0.1.38/src/PheTK/Phecode.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/Plot.py` & `PheTK-0.1.38/src/PheTK/Plot.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/_queries.py` & `PheTK-0.1.38/src/PheTK/_queries.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/_utils.py` & `PheTK-0.1.38/src/PheTK/_utils.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/phecode/phecode12.csv` & `PheTK-0.1.38/src/PheTK/phecode/phecode12.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/phecode/phecodeX.csv` & `PheTK-0.1.38/src/PheTK/phecode/phecodeX.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.37/src/PheTK/phecode/phecodeX_WHO.csv` & `PheTK-0.1.38/src/PheTK/phecode/phecodeX_WHO.csv`

 * *Files identical despite different names*

