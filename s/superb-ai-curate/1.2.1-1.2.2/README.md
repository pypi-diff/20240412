# Comparing `tmp/superb_ai_curate-1.2.1.tar.gz` & `tmp/superb_ai_curate-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb_ai_curate-1.2.1.tar", max compression
+gzip compressed data, was "superb_ai_curate-1.2.2.tar", max compression
```

## Comparing `superb_ai_curate-1.2.1.tar` & `superb_ai_curate-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1083 2023-10-25 02:33:11.990425 superb_ai_curate-1.2.1/LICENSE
--rw-r--r--   0        0        0     3309 2023-10-25 02:33:11.990493 superb_ai_curate-1.2.1/README.md
--rw-r--r--   0        0        0     3244 2024-03-19 07:28:03.017107 superb_ai_curate-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      430 2023-10-31 07:38:13.527407 superb_ai_curate-1.2.1/spb_curate/__init__.py
--rw-r--r--   0        0        0      172 2023-10-31 07:38:13.527493 superb_ai_curate-1.2.1/spb_curate/abstract/__init__.py
--rw-r--r--   0        0        0      164 2023-10-31 07:38:13.527572 superb_ai_curate-1.2.1/spb_curate/abstract/api/__init__.py
--rw-r--r--   0        0        0    10126 2023-10-25 02:33:11.991765 superb_ai_curate-1.2.1/spb_curate/abstract/api/resource.py
--rw-r--r--   0        0        0     8270 2023-10-25 02:33:11.991855 superb_ai_curate-1.2.1/spb_curate/abstract/superb_ai_object.py
--rw-r--r--   0        0        0     9349 2024-03-15 02:23:20.097160 superb_ai_curate-1.2.1/spb_curate/api_requestor.py
--rw-r--r--   0        0        0     1932 2023-10-25 02:33:11.992010 superb_ai_curate-1.2.1/spb_curate/config.py
--rw-r--r--   0        0        0      139 2023-10-31 07:38:13.527835 superb_ai_curate-1.2.1/spb_curate/curate/__init__.py
--rw-r--r--   0        0        0      125 2023-10-31 07:38:13.528111 superb_ai_curate-1.2.1/spb_curate/curate/api/__init__.py
--rw-r--r--   0        0        0      378 2023-10-31 07:38:13.528165 superb_ai_curate-1.2.1/spb_curate/curate/api/abstract.py
--rw-r--r--   0        0        0   108420 2024-03-19 05:38:12.023369 superb_ai_curate-1.2.1/spb_curate/curate/api/curate.py
--rw-r--r--   0        0        0      618 2023-10-31 07:38:13.528770 superb_ai_curate-1.2.1/spb_curate/curate/api/enums.py
--rw-r--r--   0        0        0    10696 2023-10-31 07:38:13.528988 superb_ai_curate-1.2.1/spb_curate/curate/api/job.py
--rw-r--r--   0        0        0    25391 2023-10-31 07:38:13.529297 superb_ai_curate-1.2.1/spb_curate/curate/api/model_diagnosis.py
--rw-r--r--   0        0        0       70 2023-10-31 07:38:13.529377 superb_ai_curate-1.2.1/spb_curate/curate/api/settings.py
--rw-r--r--   0        0        0      300 2023-10-25 02:33:11.992298 superb_ai_curate-1.2.1/spb_curate/curate/model/__init__.py
--rw-r--r--   0        0        0    24433 2023-10-25 02:33:11.992398 superb_ai_curate-1.2.1/spb_curate/curate/model/annotation_types.py
--rw-r--r--   0        0        0     2162 2023-10-25 02:33:11.992458 superb_ai_curate-1.2.1/spb_curate/error.py
--rw-r--r--   0        0        0     4820 2024-03-19 07:28:03.017635 superb_ai_curate-1.2.1/spb_curate/http_client.py
--rw-r--r--   0        0        0      287 2023-10-25 02:33:11.992561 superb_ai_curate-1.2.1/spb_curate/object_mapping.py
--rw-r--r--   0        0        0      730 2024-03-19 07:28:03.017993 superb_ai_curate-1.2.1/spb_curate/superb_ai_response.py
--rw-r--r--   0        0        0     5347 2023-10-25 02:33:11.992686 superb_ai_curate-1.2.1/spb_curate/util.py
--rw-r--r--   0        0        0      166 2023-10-25 02:33:11.992735 superb_ai_curate-1.2.1/spb_curate/version.py
--rw-r--r--   0        0        0     4505 1970-01-01 00:00:00.000000 superb_ai_curate-1.2.1/setup.py
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 superb_ai_curate-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-15 06:27:16.156321 superb_ai_curate-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3309 2023-09-19 05:20:56.054403 superb_ai_curate-1.2.2/README.md
+-rw-r--r--   0        0        0     3244 2024-04-12 05:01:59.826062 superb_ai_curate-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      430 2024-04-11 13:01:44.645615 superb_ai_curate-1.2.2/spb_curate/__init__.py
+-rw-r--r--   0        0        0      172 2023-11-14 10:01:04.037123 superb_ai_curate-1.2.2/spb_curate/abstract/__init__.py
+-rw-r--r--   0        0        0      164 2023-11-14 10:01:04.037271 superb_ai_curate-1.2.2/spb_curate/abstract/api/__init__.py
+-rw-r--r--   0        0        0    10126 2023-09-19 05:20:56.055153 superb_ai_curate-1.2.2/spb_curate/abstract/api/resource.py
+-rw-r--r--   0        0        0     8270 2023-09-19 05:20:56.055472 superb_ai_curate-1.2.2/spb_curate/abstract/superb_ai_object.py
+-rw-r--r--   0        0        0     9349 2023-06-15 06:27:16.158041 superb_ai_curate-1.2.2/spb_curate/api_requestor.py
+-rw-r--r--   0        0        0     1932 2023-06-15 06:27:16.158123 superb_ai_curate-1.2.2/spb_curate/config.py
+-rw-r--r--   0        0        0      139 2023-11-14 10:01:04.037385 superb_ai_curate-1.2.2/spb_curate/curate/__init__.py
+-rw-r--r--   0        0        0      125 2023-11-14 10:01:04.037496 superb_ai_curate-1.2.2/spb_curate/curate/api/__init__.py
+-rw-r--r--   0        0        0      378 2023-11-14 10:01:04.037568 superb_ai_curate-1.2.2/spb_curate/curate/api/abstract.py
+-rw-r--r--   0        0        0   108488 2024-04-12 05:01:59.826544 superb_ai_curate-1.2.2/spb_curate/curate/api/curate.py
+-rw-r--r--   0        0        0      618 2023-11-14 10:01:04.038109 superb_ai_curate-1.2.2/spb_curate/curate/api/enums.py
+-rw-r--r--   0        0        0    10696 2023-11-14 10:01:04.038389 superb_ai_curate-1.2.2/spb_curate/curate/api/job.py
+-rw-r--r--   0        0        0    25391 2023-11-14 10:01:04.038566 superb_ai_curate-1.2.2/spb_curate/curate/api/model_diagnosis.py
+-rw-r--r--   0        0        0       70 2023-11-14 10:01:04.038647 superb_ai_curate-1.2.2/spb_curate/curate/api/settings.py
+-rw-r--r--   0        0        0      300 2023-06-15 06:27:16.158508 superb_ai_curate-1.2.2/spb_curate/curate/model/__init__.py
+-rw-r--r--   0        0        0    24433 2023-06-15 06:27:16.158644 superb_ai_curate-1.2.2/spb_curate/curate/model/annotation_types.py
+-rw-r--r--   0        0        0     2162 2023-06-15 06:27:16.158744 superb_ai_curate-1.2.2/spb_curate/error.py
+-rw-r--r--   0        0        0     4820 2024-04-03 05:52:51.356901 superb_ai_curate-1.2.2/spb_curate/http_client.py
+-rw-r--r--   0        0        0      287 2023-06-15 06:27:16.158905 superb_ai_curate-1.2.2/spb_curate/object_mapping.py
+-rw-r--r--   0        0        0      730 2024-04-03 05:52:51.357334 superb_ai_curate-1.2.2/spb_curate/superb_ai_response.py
+-rw-r--r--   0        0        0     5347 2023-06-15 06:27:16.159080 superb_ai_curate-1.2.2/spb_curate/util.py
+-rw-r--r--   0        0        0      166 2023-06-15 06:27:16.159147 superb_ai_curate-1.2.2/spb_curate/version.py
+-rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 superb_ai_curate-1.2.2/PKG-INFO
```

### Comparing `superb_ai_curate-1.2.1/LICENSE` & `superb_ai_curate-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/README.md` & `superb_ai_curate-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/pyproject.toml` & `superb_ai_curate-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # /pyproject.toml
 [project]
 description = "The official Superb AI Curate client for Python"
 name = "superb-ai-curate"
-version = "1.2.1"
+version = "1.2.2"
 
 [[project.authors]]
 name = "Superb AI"
 email = "support@superb-ai.com"
 
 [tool.poetry]
 name = "superb-ai-curate"
-version = "1.2.1"
+version = "1.2.2"
 license = "MIT"
 description = "The official Superb AI Curate client for Python"
 authors = ["Superb AI <support@superb-ai.com>"]
 homepage = "https://superb-ai.com/"
 repository = "https://github.com/Superb-AI-Suite/superb-ai-curate-python"
 documentation = "https://docs.superb-ai.com/reference/introduction-curate-sdk"
 readme = "README.md"
```

### Comparing `superb_ai_curate-1.2.1/spb_curate/abstract/api/resource.py` & `superb_ai_curate-1.2.2/spb_curate/abstract/api/resource.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/abstract/superb_ai_object.py` & `superb_ai_curate-1.2.2/spb_curate/abstract/superb_ai_object.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/api_requestor.py` & `superb_ai_curate-1.2.2/spb_curate/api_requestor.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/config.py` & `superb_ai_curate-1.2.2/spb_curate/config.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/curate/api/curate.py` & `superb_ai_curate-1.2.2/spb_curate/curate/api/curate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2994,19 +2994,20 @@
         if query is not None:
             job = Job.create(
                 access_key=access_key,
                 team_name=team_name,
                 job_type=JobType.UPDATE_SLICE_BY_QUERY,
                 param={
                     "dataset_id": self.dataset_id,
-                    "images": {
+                    "image_filters": {
                         "slice": None,
                         "query": query,
                     },
-                    "slices": {"add": [self.id], "remove": []},
+                    "slice_id": self.id,
+                    "remove": False,
                 },
             )
         else:
             images = [] if not images else images
             image_ids = [] if not image_ids else image_ids
             image_keys = [] if not image_keys else image_keys
 
@@ -3032,15 +3033,16 @@
                 team_name=team_name,
                 job_type=JobType.UPDATE_SLICE,
                 param={
                     "dataset_id": self.dataset_id,
                     "images": {
                         "param_id": uploaded_param["id"],
                     },
-                    "slices": {"add": [self.id], "remove": []},
+                    "slice_id": self.id,
+                    "remove": False,
                 },
             )
 
         if not asynchronous:
             job.wait_until_complete()
 
         return job
@@ -3095,19 +3097,20 @@
         if query is not None:
             job = Job.create(
                 access_key=access_key,
                 team_name=team_name,
                 job_type=JobType.UPDATE_SLICE_BY_QUERY,
                 param={
                     "dataset_id": self.dataset_id,
-                    "images": {
+                    "image_filters": {
                         "slice": None,
                         "query": query,
                     },
-                    "slices": {"add": [], "remove": [self.id]},
+                    "slice_id": self.id,
+                    "remove": True,
                 },
             )
         else:
             images = [] if not images else images
             image_ids = [] if not image_ids else image_ids
             image_keys = [] if not image_keys else image_keys
 
@@ -3131,15 +3134,16 @@
             job = Job.create(
                 access_key=access_key,
                 team_name=team_name,
                 job_type=JobType.UPDATE_SLICE,
                 param={
                     "dataset_id": self.dataset_id,
                     "images": {"param_id": uploaded_param["id"]},
-                    "slices": {"add": [], "remove": [self.id]},
+                    "slice_id": self.id,
+                    "remove": True,
                 },
             )
 
         if not asynchronous:
             job.wait_until_complete()
 
         return job
```

### Comparing `superb_ai_curate-1.2.1/spb_curate/curate/api/enums.py` & `superb_ai_curate-1.2.2/spb_curate/curate/api/enums.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/curate/api/job.py` & `superb_ai_curate-1.2.2/spb_curate/curate/api/job.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/curate/api/model_diagnosis.py` & `superb_ai_curate-1.2.2/spb_curate/curate/api/model_diagnosis.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/curate/model/annotation_types.py` & `superb_ai_curate-1.2.2/spb_curate/curate/model/annotation_types.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/error.py` & `superb_ai_curate-1.2.2/spb_curate/error.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/http_client.py` & `superb_ai_curate-1.2.2/spb_curate/http_client.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/superb_ai_response.py` & `superb_ai_curate-1.2.2/spb_curate/superb_ai_response.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/spb_curate/util.py` & `superb_ai_curate-1.2.2/spb_curate/util.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.1/PKG-INFO` & `superb_ai_curate-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superb-ai-curate
-Version: 1.2.1
+Version: 1.2.2
 Summary: The official Superb AI Curate client for Python
 Home-page: https://superb-ai.com/
 License: MIT
 Keywords: superb ai,superbapi,tasks,categorization,annotation,labeling,dataops,mlops,curation
 Author: Superb AI
 Author-email: support@superb-ai.com
 Requires-Python: >=3.7,<4.0
@@ -16,34 +16,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: dev
 Provides-Extra: docs
-Requires-Dist: Sphinx; extra == "docs"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: coveralls; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: Sphinx ; extra == "docs"
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: coveralls ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: requests (>=2.20.0,<3.0.0)
-Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0); extra == "docs"
-Requires-Dist: sphinx-pyproject; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx-pyproject ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon ; extra == "docs"
 Project-URL: Documentation, https://docs.superb-ai.com/reference/introduction-curate-sdk
 Project-URL: Repository, https://github.com/Superb-AI-Suite/superb-ai-curate-python
 Description-Content-Type: text/markdown
 
 # `superb-ai-curate`
 
 [![Coverage Status](https://coveralls.io/repos/github/Superb-AI-Suite/superb-ai-curate-python/badge.svg?branch=main)](https://coveralls.io/github/Superb-AI-Suite/superb-ai-curate-python?branch=main)
```

