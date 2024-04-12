# Comparing `tmp/SMjournal-0.0.5.tar.gz` & `tmp/SMjournal-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjournal-0.0.5.tar", last modified: Fri Apr 12 15:13:39 2024, max compression
+gzip compressed data, was "SMjournal-0.0.6.tar", last modified: Fri Apr 12 15:20:54 2024, max compression
```

## Comparing `SMjournal-0.0.5.tar` & `SMjournal-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:13:39.240179 SMjournal-0.0.5/
--rw-rw-r--   0 agus      (1000) agus      (1000)     1077 2024-04-11 13:57:24.000000 SMjournal-0.0.5/LICENSE
--rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:13:39.240179 SMjournal-0.0.5/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)        0 2024-04-11 13:57:24.000000 SMjournal-0.0.5/README.md
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:13:39.236179 SMjournal-0.0.5/SMjournal/
--rw-rw-r--   0 agus      (1000) agus      (1000)      124 2024-04-11 13:57:24.000000 SMjournal-0.0.5/SMjournal/__init__.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4909 2024-04-12 14:56:15.000000 SMjournal-0.0.5/SMjournal/collinearity.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4690 2024-04-11 13:57:24.000000 SMjournal-0.0.5/SMjournal/data.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     1512 2024-04-11 13:57:24.000000 SMjournal-0.0.5/SMjournal/low_level.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4434 2024-04-11 13:57:24.000000 SMjournal-0.0.5/SMjournal/meta_reg.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     2928 2024-04-11 13:57:24.000000 SMjournal-0.0.5/SMjournal/potentiality.py
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:13:39.240179 SMjournal-0.0.5/SMjournal.egg-info/
--rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:13:39.000000 SMjournal-0.0.5/SMjournal.egg-info/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)      343 2024-04-12 15:13:39.000000 SMjournal-0.0.5/SMjournal.egg-info/SOURCES.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)        1 2024-04-12 15:13:39.000000 SMjournal-0.0.5/SMjournal.egg-info/dependency_links.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       88 2024-04-12 15:13:39.000000 SMjournal-0.0.5/SMjournal.egg-info/requires.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       10 2024-04-12 15:13:39.000000 SMjournal-0.0.5/SMjournal.egg-info/top_level.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)      106 2024-04-11 13:57:24.000000 SMjournal-0.0.5/pyproject.toml
--rw-rw-r--   0 agus      (1000) agus      (1000)      633 2024-04-12 15:13:39.240179 SMjournal-0.0.5/setup.cfg
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:20:54.074936 SMjournal-0.0.6/
+-rw-rw-r--   0 agus      (1000) agus      (1000)     1077 2024-04-11 13:57:24.000000 SMjournal-0.0.6/LICENSE
+-rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:20:54.074936 SMjournal-0.0.6/PKG-INFO
+-rw-rw-r--   0 agus      (1000) agus      (1000)        0 2024-04-11 13:57:24.000000 SMjournal-0.0.6/README.md
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:20:54.066936 SMjournal-0.0.6/SMjournal/
+-rw-rw-r--   0 agus      (1000) agus      (1000)      124 2024-04-11 13:57:24.000000 SMjournal-0.0.6/SMjournal/__init__.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4904 2024-04-12 15:19:53.000000 SMjournal-0.0.6/SMjournal/collinearity.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4690 2024-04-11 13:57:24.000000 SMjournal-0.0.6/SMjournal/data.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     1512 2024-04-11 13:57:24.000000 SMjournal-0.0.6/SMjournal/low_level.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4434 2024-04-11 13:57:24.000000 SMjournal-0.0.6/SMjournal/meta_reg.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     2928 2024-04-11 13:57:24.000000 SMjournal-0.0.6/SMjournal/potentiality.py
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:20:54.070936 SMjournal-0.0.6/SMjournal.egg-info/
+-rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:20:54.000000 SMjournal-0.0.6/SMjournal.egg-info/PKG-INFO
+-rw-rw-r--   0 agus      (1000) agus      (1000)      343 2024-04-12 15:20:54.000000 SMjournal-0.0.6/SMjournal.egg-info/SOURCES.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)        1 2024-04-12 15:20:54.000000 SMjournal-0.0.6/SMjournal.egg-info/dependency_links.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)       88 2024-04-12 15:20:54.000000 SMjournal-0.0.6/SMjournal.egg-info/requires.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)       10 2024-04-12 15:20:54.000000 SMjournal-0.0.6/SMjournal.egg-info/top_level.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)      106 2024-04-11 13:57:24.000000 SMjournal-0.0.6/pyproject.toml
+-rw-rw-r--   0 agus      (1000) agus      (1000)      633 2024-04-12 15:20:54.074936 SMjournal-0.0.6/setup.cfg
```

### Comparing `SMjournal-0.0.5/LICENSE` & `SMjournal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.5/PKG-INFO` & `SMjournal-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.5/SMjournal/collinearity.py` & `SMjournal-0.0.6/SMjournal/collinearity.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
   for i in range(len(corr_numpy)):
     value=corr_numpy[i,indices[i]]
     if value>filter or value<-filter:
       finalIndices.append(i)
   finalIndices
   finalCorr=correlation.iloc[finalIndices,finalIndices]
 
-  corrplot.figure(figsize=(10,7))
+  plt.figure(figsize=(10,7))
 
   # Generate a mask to onlyshow the bottom triangle
   mask = np.triu(np.ones_like(finalCorr, dtype=bool))
 
   # generate heatmap
   corrplot=sns.heatmap(finalCorr, annot=True, mask=mask, vmin=-1, vmax=1,cmap="rocket_r")
   corrplot.title('Correlation Coefficient Of Predictors')
```

### Comparing `SMjournal-0.0.5/SMjournal/data.py` & `SMjournal-0.0.6/SMjournal/data.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.5/SMjournal/low_level.py` & `SMjournal-0.0.6/SMjournal/low_level.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.5/SMjournal/meta_reg.py` & `SMjournal-0.0.6/SMjournal/meta_reg.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.5/SMjournal/potentiality.py` & `SMjournal-0.0.6/SMjournal/potentiality.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.5/SMjournal.egg-info/PKG-INFO` & `SMjournal-0.0.6/SMjournal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
