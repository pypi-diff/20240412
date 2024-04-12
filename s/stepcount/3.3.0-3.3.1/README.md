# Comparing `tmp/stepcount-3.3.0.tar.gz` & `tmp/stepcount-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.3.0.tar", last modified: Thu Mar 14 20:03:09 2024, max compression
+gzip compressed data, was "stepcount-3.3.1.tar", last modified: Fri Apr 12 12:25:55 2024, max compression
```

## Comparing `stepcount-3.3.0.tar` & `stepcount-3.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:03:09.857207 stepcount-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-03-14 20:03:00.000000 stepcount-3.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-14 20:03:09.857207 stepcount-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-03-14 20:03:00.000000 stepcount-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-14 20:03:00.000000 stepcount-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 20:03:09.857207 stepcount-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-14 20:03:00.000000 stepcount-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:03:09.853207 stepcount-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:03:09.857207 stepcount-3.3.0/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-14 20:03:09.857207 stepcount-3.3.0/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23294 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17621 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:03:09.857207 stepcount-3.3.0/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-03-14 20:03:00.000000 stepcount-3.3.0/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 20:03:09.857207 stepcount-3.3.0/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-14 20:03:09.000000 stepcount-3.3.0/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-03-14 20:03:00.000000 stepcount-3.3.0/versioneer.py
+drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.123067 stepcount-3.3.1/
+-rw-r--r--   0 miko      (1000) miko      (1000)     8026 2024-04-12 12:18:04.000000 stepcount-3.3.1/LICENSE.md
+-rw-r--r--   0 miko      (1000) miko      (1000)     8200 2024-04-12 12:25:55.123067 stepcount-3.3.1/PKG-INFO
+-rw-r--r--   0 miko      (1000) miko      (1000)     6395 2024-04-12 12:18:04.000000 stepcount-3.3.1/README.md
+-rw-r--r--   0 miko      (1000) miko      (1000)     6814 2024-04-12 12:18:04.000000 stepcount-3.3.1/pyproject.toml
+-rw-r--r--   0 miko      (1000) miko      (1000)       38 2024-04-12 12:25:55.123067 stepcount-3.3.1/setup.cfg
+-rw-r--r--   0 miko      (1000) miko      (1000)     2912 2024-04-12 12:18:04.000000 stepcount-3.3.1/setup.py
+drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/
+drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.123067 stepcount-3.3.1/src/stepcount/
+-rw-r--r--   0 miko      (1000) miko      (1000)      580 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/__init__.py
+-rw-r--r--   0 miko      (1000) miko      (1000)      497 2024-04-12 12:25:55.123067 stepcount-3.3.1/src/stepcount/_version.py
+-rw-r--r--   0 miko      (1000) miko      (1000)     5345 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/features.py
+-rw-r--r--   0 miko      (1000) miko      (1000)     9731 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/hmm_utils.py
+-rw-r--r--   0 miko      (1000) miko      (1000)    23294 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/models.py
+-rw-r--r--   0 miko      (1000) miko      (1000)    11941 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/sslmodel.py
+-rw-r--r--   0 miko      (1000) miko      (1000)    17801 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/stepcount.py
+drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/stepcount/utils/
+-rw-r--r--   0 miko      (1000) miko      (1000)      124 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/__init__.py
+-rw-r--r--   0 miko      (1000) miko      (1000)     1346 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 miko      (1000) miko      (1000)     2807 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/stepcount.egg-info/
+-rw-r--r--   0 miko      (1000) miko      (1000)     8200 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 miko      (1000) miko      (1000)      576 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 miko      (1000) miko      (1000)        1 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 miko      (1000) miko      (1000)      189 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 miko      (1000) miko      (1000)      385 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 miko      (1000) miko      (1000)       10 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 miko      (1000) miko      (1000)    83607 2024-04-12 12:18:04.000000 stepcount-3.3.1/versioneer.py
```

### Comparing `stepcount-3.3.0/LICENSE.md` & `stepcount-3.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/PKG-INFO` & `stepcount-3.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: stepcount
-Version: 3.3.0
-Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
-Home-page: https://github.com/OxWearables/stepcount
-Download-URL: https://github.com/OxWearables/stepcount
-Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
-Maintainer: Shing Chan
-Maintainer-email: shing.chan@ndph.ox.ac.uk
-License: See LICENSE file.
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
 ## Install
@@ -164,15 +143,15 @@
 2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
 2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
 ...
 ```
 
 then use:
 ```console
-$ stepcount my-file.csv --txyz 'HEADER_TIMESTAMP,X,Y,Z'
+$ stepcount my-file.csv --txyz HEADER_TIMESTAMP,X,Y,Z
 ```
 
 
 ### Processing multiple files
 #### Windows
 To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
```

### Comparing `stepcount-3.3.0/pyproject.toml` & `stepcount-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/setup.py` & `stepcount-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/__init__.py` & `stepcount-3.3.1/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/features.py` & `stepcount-3.3.1/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/hmm_utils.py` & `stepcount-3.3.1/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/models.py` & `stepcount-3.3.1/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/sslmodel.py` & `stepcount-3.3.1/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/stepcount.py` & `stepcount-3.3.1/src/stepcount/stepcount.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,21 +158,30 @@
 
     def _sum(x):
         x = x.to_numpy()
         if skipna:
             return np.nansum(x)
         return np.sum(x)
 
+    def _max(x, n=1):
+        if skipna:
+            return x.nlargest(n, keep='all').mean()
+        elif x.isna().any():
+            return np.nan
+
     # there's a bug with .resample().sum(skipna)
     # https://github.com/pandas-dev/pandas/issues/29382
 
     # steps
     total = np.round(Y.agg(_sum))  # total steps
     hourly = Y.resample('H').agg(_sum).round().rename('Steps')  # steps, hourly
     daily = Y.resample('D').agg(_sum).round().rename('Steps')  # steps, daily
+    minutely = Y.resample('T').agg(_sum).round().rename('Steps')  # steps, minutely
+
+    # steps, daily stats
     if not adjust_estimates:
         daily_avg = np.round(daily.mean())
         daily_med = np.round(daily.median())
         daily_min = np.round(daily.min())
         daily_max = np.round(daily.max())
     else:
         weekdaily = daily.groupby(daily.index.weekday).mean()
@@ -182,33 +191,31 @@
         daily_max = np.round(weekdaily.max())
 
     # walking
     dt = pd.Timedelta(infer_freq(Y.index)).seconds
     W = Y.mask(~Y.isna(), Y >= steptol)
     total_walk = np.round(W.agg(_sum) * dt / 60)
     daily_walk = (W.resample('D').agg(_sum) * dt / 60).round().rename('Walk(mins)')
+
+    # walking, daily stats
     if not adjust_estimates:
         daily_walk_avg = np.round(daily_walk.mean())
         daily_walk_med = np.round(daily_walk.median())
         daily_walk_min = np.round(daily_walk.min())
         daily_walk_max = np.round(daily_walk.max())
     else:
         weekdaily_walk = daily_walk.groupby(daily_walk.index.weekday).mean()
         daily_walk_avg = np.round(weekdaily_walk.mean())
         daily_walk_med = np.round(weekdaily_walk.median())
         daily_walk_min = np.round(weekdaily_walk.min())
         daily_walk_max = np.round(weekdaily_walk.max())
 
-    def _max(x, n=1):
-        return x.nlargest(n, keep='all').mean()
-
     # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
-    cadence = Y.resample('min').sum()
-    daily_cadence_peak1 = cadence.resample('D').agg(_max, n=1)
-    daily_cadence_peak30 = cadence.resample('D').agg(_max, n=30)
+    daily_cadence_peak1 = minutely.resample('D').agg(_max, n=1)
+    daily_cadence_peak30 = minutely.resample('D').agg(_max, n=30)
     if not adjust_estimates:
         cadence_peak1 = np.round(daily_cadence_peak1.mean())
         cadence_peak30 = np.round(daily_cadence_peak30.mean())
     else:
         weekdaily_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).mean()
         weekdaily_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).mean()
         cadence_peak1 = np.round(weekdaily_cadence_peak1.mean())
```

### Comparing `stepcount-3.3.0/src/stepcount/utils/collate_outputs.py` & `stepcount-3.3.1/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount/utils/generate_commands.py` & `stepcount-3.3.1/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.3.0
+Version: 3.3.1
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: actipy>=3.0.5
+Requires-Dist: numpy==1.24.*
+Requires-Dist: scipy==1.10.*
+Requires-Dist: pandas==2.0.*
+Requires-Dist: tqdm==4.64.*
+Requires-Dist: joblib==1.2.*
+Requires-Dist: scikit-learn==1.1.1
+Requires-Dist: imbalanced-learn==0.9.1
+Requires-Dist: hmmlearn==0.3.*
+Requires-Dist: torch==1.13.*
+Requires-Dist: torchvision==0.14.*
+Requires-Dist: transforms3d==0.4.*
 Provides-Extra: dev
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: autopep8; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
+Requires-Dist: ipdb; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: tomli; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE.md
+Requires-Dist: sphinx>=4.2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=1.0; extra == "docs"
+Requires-Dist: readthedocs-sphinx-search>=0.1; extra == "docs"
+Requires-Dist: sphinxcontrib-programoutput>=0.17; extra == "docs"
+Requires-Dist: docutils<0.18; extra == "docs"
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
@@ -164,15 +189,15 @@
 2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
 2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
 ...
 ```
 
 then use:
 ```console
-$ stepcount my-file.csv --txyz 'HEADER_TIMESTAMP,X,Y,Z'
+$ stepcount my-file.csv --txyz HEADER_TIMESTAMP,X,Y,Z
 ```
 
 
 ### Processing multiple files
 #### Windows
 To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
```

### Comparing `stepcount-3.3.0/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.3.1/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.0/versioneer.py` & `stepcount-3.3.1/versioneer.py`

 * *Files identical despite different names*

