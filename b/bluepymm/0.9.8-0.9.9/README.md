# Comparing `tmp/bluepymm-0.9.8.tar.gz` & `tmp/bluepymm-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepymm-0.9.8.tar", last modified: Mon Jan 15 08:36:04 2024, max compression
+gzip compressed data, was "bluepymm-0.9.9.tar", last modified: Thu Mar 21 11:58:19 2024, max compression
```

## Comparing `bluepymm-0.9.8.tar` & `bluepymm-0.9.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-15 08:36:00.000000 bluepymm-0.9.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-01-15 08:36:00.000000 bluepymm-0.9.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-01-15 08:36:00.000000 bluepymm-0.9.8/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-15 08:36:00.000000 bluepymm-0.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-15 08:36:00.000000 bluepymm-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-15 08:36:04.693347 bluepymm-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-01-15 08:36:00.000000 bluepymm-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.697347 bluepymm-0.9.8/bluepymm/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-15 08:36:04.697347 bluepymm-0.9.8/bluepymm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/legacy/create_hoc_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/prepare_combos/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/prepare_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16419 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/prepare_combos/create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/prepare_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/prepare_combos/parse_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/prepare_combos/prepare_emodel_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/run_combos/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/run_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/run_combos/calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/run_combos/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/select_combos/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/megate_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/select_combos/table_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6660 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/templates/cell_template_neurodamus.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/templates/cell_template_neurodamus_sbo.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (127)     4762 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/templates/cell_template_neuron.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm/validate_output/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/validate_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-01-15 08:36:00.000000 bluepymm-0.9.8/bluepymm/validate_output/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:36:04.693347 bluepymm-0.9.8/bluepymm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-15 08:36:04.000000 bluepymm-0.9.8/bluepymm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-15 08:36:04.697347 bluepymm-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-15 08:36:00.000000 bluepymm-0.9.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    69513 2024-01-15 08:36:00.000000 bluepymm-0.9.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-21 11:58:14.000000 bluepymm-0.9.9/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-03-21 11:58:14.000000 bluepymm-0.9.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-21 11:58:14.000000 bluepymm-0.9.9/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-21 11:58:14.000000 bluepymm-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-21 11:58:14.000000 bluepymm-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-21 11:58:19.427771 bluepymm-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-21 11:58:14.000000 bluepymm-0.9.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/legacy/create_hoc_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/prepare_combos/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/prepare_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16419 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/prepare_combos/create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/prepare_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/prepare_combos/parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/prepare_combos/prepare_emodel_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/run_combos/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/run_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/run_combos/calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/run_combos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/select_combos/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/select_combos/table_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6759 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/templates/cell_template_neurodamus.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/templates/cell_template_neurodamus_sbo.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4902 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/templates/cell_template_neuron.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.427771 bluepymm-0.9.9/bluepymm/validate_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/validate_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-21 11:58:14.000000 bluepymm-0.9.9/bluepymm/validate_output/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:58:19.423771 bluepymm-0.9.9/bluepymm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 11:58:19.000000 bluepymm-0.9.9/bluepymm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-21 11:58:19.427771 bluepymm-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-21 11:58:14.000000 bluepymm-0.9.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69513 2024-03-21 11:58:14.000000 bluepymm-0.9.9/versioneer.py
```

### Comparing `bluepymm-0.9.8/COPYING` & `bluepymm-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/COPYING.lesser` & `bluepymm-0.9.9/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/LICENSE.txt` & `bluepymm-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/PKG-INFO` & `bluepymm-0.9.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.9.8
+Version: 0.9.9
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.9.8/README.rst` & `bluepymm-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/__init__.py` & `bluepymm-0.9.9/bluepymm/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/legacy/__init__.py` & `bluepymm-0.9.9/bluepymm/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/legacy/create_hoc_files.py` & `bluepymm-0.9.9/bluepymm/legacy/create_hoc_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/main.py` & `bluepymm-0.9.9/bluepymm/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/prepare_combos/__init__.py` & `bluepymm-0.9.9/bluepymm/prepare_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/prepare_combos/create_mm_sqlite.py` & `bluepymm-0.9.9/bluepymm/prepare_combos/create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/prepare_combos/main.py` & `bluepymm-0.9.9/bluepymm/prepare_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/prepare_combos/parse_files.py` & `bluepymm-0.9.9/bluepymm/prepare_combos/parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/prepare_combos/prepare_emodel_dirs.py` & `bluepymm-0.9.9/bluepymm/prepare_combos/prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/run_combos/__init__.py` & `bluepymm-0.9.9/bluepymm/run_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/run_combos/calculate_scores.py` & `bluepymm-0.9.9/bluepymm/run_combos/calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/run_combos/main.py` & `bluepymm-0.9.9/bluepymm/run_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/__init__.py` & `bluepymm-0.9.9/bluepymm/select_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/main.py` & `bluepymm-0.9.9/bluepymm/select_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/megate_output.py` & `bluepymm-0.9.9/bluepymm/select_combos/megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/process_megate_config.py` & `bluepymm-0.9.9/bluepymm/select_combos/process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/reporting.py` & `bluepymm-0.9.9/bluepymm/select_combos/reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/sqlite_io.py` & `bluepymm-0.9.9/bluepymm/select_combos/sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/select_combos/table_processing.py` & `bluepymm-0.9.9/bluepymm/select_combos/table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/templates/cell_template_neurodamus.jinja2` & `bluepymm-0.9.9/bluepymm/templates/cell_template_neurodamus.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,16 @@
 
   sl = $o1
   mech = $s2
   distfunc = $s3
   this.soma[0] distance(0, 0.5)
   sprint(distfunc, "%%s %s(%%f) = %s", mech, distfunc)
   forsec sl for(x, 0) {
-    sprint(stmp, distfunc, secname(), x, distance(x))
+    // use distance(x) twice for the step distribution case, e.g. for calcium hotspot
+    sprint(stmp, distfunc, secname(), x, distance(x), distance(x))
     execute(stmp)
   }
 }
 
 proc geom_nseg() {
   this.geom_nsec() //To count all sections
   //TODO: geom_nseg_fixed depends on segCounts which is calculated by
```

### Comparing `bluepymm-0.9.8/bluepymm/templates/cell_template_neurodamus_sbo.jinja2` & `bluepymm-0.9.9/bluepymm/templates/cell_template_neurodamus_sbo.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -134,24 +134,35 @@
     }
 }
 
 func getThreshold() { return 0.0 }
 
 proc load_morphology(/* morphology_dir, morphology_name */) {localobj morph, import, sf, extension, commands, pyobj
   strdef morph_path
-  sprint(morph_path, "%s/%s", $s1, $s2)  sf = new StringFunctions()
-  extension = new String()  sscanf(morph_path, "%s", extension.s)
+  sprint(morph_path, "%s/%s", $s1, $s2)
+  sf = new StringFunctions()
+  extension = new String()
+  sscanf(morph_path, "%s", extension.s)
 
-  // TODO fix the `-3` here.
   sf.right(extension.s, sf.len(extension.s)-3)
   
-  if( strcmp(extension.s, ".asc") == 0 ) {
+  if( strcmp(extension.s, "asc") == 0 ) {
      morph = new Import3d_Neurolucida3()
-  } else if( strcmp(extension.s, ".swc" ) == 0) {
+     morph.quiet = 1
+     morph.input(morph_path)
+
+     import = new Import3d_GUI(morph, 0)
+     import.instantiate(this)
+  } else if( strcmp(extension.s, "swc" ) == 0) {
      morph = new Import3d_SWC_read()
+     morph.quiet = 1
+     morph.input(morph_path)
+
+     import = new Import3d_GUI(morph, 0)
+     import.instantiate(this)
   } else if( strcmp(extension.s, ".h5") == 0 ) {
     if(nrnpython ("from morphio_wrapper import MorphIOWrapper") == 1) {
         pyobj = new PythonObject()
         commands = pyobj.MorphIOWrapper(morph_path).morph_as_hoc()
         for i = 0, pyobj.len(commands) - 1 {
             execute(commands._[i], this)
         }
@@ -177,15 +188,16 @@
 
   sl = $o1
   mech = $s2
   distfunc = $s3
   this.soma[0] distance(0, 0.5)
   sprint(distfunc, "%%s %s(%%f) = %s", mech, distfunc)
   forsec sl for(x, 0) {
-    sprint(stmp, distfunc, secname(), x, distance(x))
+    // use distance(x) twice for the step distribution case, e.g. for calcium hotspot
+    sprint(stmp, distfunc, secname(), x, distance(x), distance(x))
     execute(stmp)
   }
 }
 
 proc geom_nseg() {
   this.geom_nsec() //To count all sections
   //TODO: geom_nseg_fixed depends on segCounts which is calculated by
```

### Comparing `bluepymm-0.9.8/bluepymm/templates/cell_template_neuron.jinja2` & `bluepymm-0.9.9/bluepymm/templates/cell_template_neuron.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
   create soma[1], dend[1], apic[1], axon[1], myelin[1]
 
   objref this, CellRef, segCounts
 
   public all, somatic, apical, axonal, basal, myelinated, APC
   objref all, somatic, apical, axonal, basal, myelinated, APC
 
+obfunc getCell(){
+        return this
+}
+
 proc init(/* args: morphology_dir, morphology_name */) {
   all = new SectionList()
   apical = new SectionList()
   axonal = new SectionList()
   basal = new SectionList()
   somatic = new SectionList()
   myelinated = new SectionList()
@@ -108,15 +112,16 @@
 
   sl = $o1
   mech = $s2
   distfunc = $s3
   this.soma[0] distance(0, 0.5)
   sprint(distfunc, "%%s %s(%%f) = %s", mech, distfunc)
   forsec sl for(x, 0) {
-    sprint(stmp, distfunc, secname(), x, distance(x))
+    // use distance(x) twice for the step distribution case, e.g. for calcium hotspot
+    sprint(stmp, distfunc, secname(), x, distance(x), distance(x))
     execute(stmp)
   }
 }
 
 proc geom_nseg() {
   this.geom_nsec() //To count all sections
   //TODO: geom_nseg_fixed depends on segCounts which is calculated by
```

### Comparing `bluepymm-0.9.8/bluepymm/tools.py` & `bluepymm-0.9.9/bluepymm/tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm/validate_output/main.py` & `bluepymm-0.9.9/bluepymm/validate_output/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/bluepymm.egg-info/PKG-INFO` & `bluepymm-0.9.9/bluepymm.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.9.8
+Version: 0.9.9
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.9.8/bluepymm.egg-info/SOURCES.txt` & `bluepymm-0.9.9/bluepymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/setup.py` & `bluepymm-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.9.8/versioneer.py` & `bluepymm-0.9.9/versioneer.py`

 * *Files identical despite different names*

