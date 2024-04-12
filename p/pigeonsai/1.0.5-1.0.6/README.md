# Comparing `tmp/pigeonsai-1.0.5.tar.gz` & `tmp/pigeonsai-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-1.0.5.tar", last modified: Wed Apr 10 17:15:02 2024, max compression
+gzip compressed data, was "pigeonsai-1.0.6.tar", last modified: Fri Apr 12 00:54:31 2024, max compression
```

## Comparing `pigeonsai-1.0.5.tar` & `pigeonsai-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/
--rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      374 2024-04-10 17:12:16.000000 pigeonsai-1.0.5/README.md
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/setup.cfg
--rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-04-10 17:14:41.000000 pigeonsai-1.0.5/setup.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/
--rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.5/src/pigeonsai/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.5/src/pigeonsai/_client.py
--rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.5/src/pigeonsai/_constants.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.5/src/pigeonsai/_exceptions.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/_utils/
--rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.5/src/pigeonsai/_utils/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.5/src/pigeonsai/_utils/_utils.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai/resources/
--rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.5/src/pigeonsai/resources/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.5/src/pigeonsai/resources/anomaly_detector.py
--rw-r--r--   0 bs        (1000) bs        (1000)    10791 2024-04-10 16:56:58.000000 pigeonsai-1.0.5/src/pigeonsai/resources/data_connector.py
--rw-r--r--   0 bs        (1000) bs        (1000)    10436 2024-04-06 23:41:09.000000 pigeonsai-1.0.5/src/pigeonsai/resources/recommender.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-10 17:15:02.924447 pigeonsai-1.0.5/src/pigeonsai.egg-info/
--rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-10 17:15:02.000000 pigeonsai-1.0.5/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      374 2024-04-10 17:12:16.000000 pigeonsai-1.0.6/README.md
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/setup.cfg
+-rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-04-12 00:54:09.000000 pigeonsai-1.0.6/setup.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.791464 pigeonsai-1.0.6/src/
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/
+-rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.6/src/pigeonsai/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.6/src/pigeonsai/_client.py
+-rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.6/src/pigeonsai/_constants.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.6/src/pigeonsai/_exceptions.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/_utils/
+-rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.6/src/pigeonsai/_utils/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.6/src/pigeonsai/_utils/_utils.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai/resources/
+-rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.6/src/pigeonsai/resources/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.6/src/pigeonsai/resources/anomaly_detector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    10791 2024-04-10 16:56:58.000000 pigeonsai-1.0.6/src/pigeonsai/resources/data_connector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)    10537 2024-04-11 21:01:33.000000 pigeonsai-1.0.6/src/pigeonsai/resources/recommender.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-12 00:54:31.801464 pigeonsai-1.0.6/src/pigeonsai.egg-info/
+-rw-r--r--   0 bs        (1000) bs        (1000)     1882 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-12 00:54:31.000000 pigeonsai-1.0.6/src/pigeonsai.egg-info/top_level.txt
```

### Comparing `pigeonsai-1.0.5/PKG-INFO` & `pigeonsai-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.5
+Version: 1.0.6
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.5/setup.py` & `pigeonsai-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="1.0.5",
+    version="1.0.6",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-1.0.5/src/pigeonsai/_client.py` & `pigeonsai-1.0.6/src/pigeonsai/_client.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.5/src/pigeonsai/_exceptions.py` & `pigeonsai-1.0.6/src/pigeonsai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.5/src/pigeonsai/resources/data_connector.py` & `pigeonsai-1.0.6/src/pigeonsai/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.5/src/pigeonsai/resources/recommender.py` & `pigeonsai-1.0.6/src/pigeonsai/resources/recommender.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,15 @@
         learn_rate: Optional[str] = None,
         beta: Optional[str] = None,
         verbose: Optional[str] = None,
         train_prop: Optional[str] = None,
         random_seed: Optional[str] = None,
         latent_dims: Optional[str] = None,
         hidden_dims: Optional[str] = None,
+        eval_user_percent: Optional[str] = None,
         recall_at_k: Optional[str] = None,
         eval_iterations: Optional[str] = None,
         act_fn: Optional[str] = None,
         likelihood: Optional[str] = None,
         data_subset_percent: Optional[str] = None,
     ):
         kwargs = {
@@ -253,14 +254,15 @@
             'learn_rate': learn_rate,
             'beta': beta,
             'verbose': verbose,
             'train_prop': train_prop,
             'random_seed': random_seed,
             'latent_dims': latent_dims,
             'hidden_dims': hidden_dims,
+            'eval_user_percent': eval_user_percent,
             'recall_at_k': recall_at_k,
             'eval_iterations': eval_iterations,
             'act_fn': act_fn,
             'likelihood': likelihood,
             'data_subset_percent': data_subset_percent,
         }
```

### Comparing `pigeonsai-1.0.5/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-1.0.6/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.5
+Version: 1.0.6
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.5/src/pigeonsai.egg-info/SOURCES.txt` & `pigeonsai-1.0.6/src/pigeonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

