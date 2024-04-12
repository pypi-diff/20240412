# Comparing `tmp/sparrow-cvat-1.1.0.dev1694542729.tar.gz` & `tmp/sparrow-cvat-1.1.0.dev1694543918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow-cvat-1.1.0.dev1694542729.tar", last modified: Tue Sep 12 18:19:01 2023, max compression
+gzip compressed data, was "sparrow-cvat-1.1.0.dev1694543918.tar", last modified: Tue Sep 12 18:38:50 2023, max compression
```

## Comparing `sparrow-cvat-1.1.0.dev1694542729.tar` & `sparrow-cvat-1.1.0.dev1694543918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:19:01.359212 sparrow-cvat-1.1.0.dev1694542729/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-09-12 18:19:01.359212 sparrow-cvat-1.1.0.dev1694542729/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-09-12 18:19:01.359212 sparrow-cvat-1.1.0.dev1694542729/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:19:01.355212 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-12 18:18:11.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:19:01.355212 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-12 18:19:01.000000 sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:38:50.730992 sparrow-cvat-1.1.0.dev1694543918/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-09-12 18:38:50.730992 sparrow-cvat-1.1.0.dev1694543918/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-09-12 18:38:50.730992 sparrow-cvat-1.1.0.dev1694543918/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:38:50.726992 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-12 18:37:54.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 18:38:50.726992 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-12 18:38:50.000000 sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/top_level.txt
```

### Comparing `sparrow-cvat-1.1.0.dev1694542729/LICENSE` & `sparrow-cvat-1.1.0.dev1694543918/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-1.1.0.dev1694542729/PKG-INFO` & `sparrow-cvat-1.1.0.dev1694543918/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-cvat
-Version: 1.1.0.dev1694542729
+Version: 1.1.0.dev1694543918
 Author: Sparrow Computing
 Author-email: ben@sparrow.dev
 License-File: LICENSE
 Requires-Dist: cvat-sdk==2.5.0
 Requires-Dist: fire
 Requires-Dist: pillow
 Requires-Dist: requests
```

### Comparing `sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/__main__.py` & `sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/api.py` & `sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/api.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat/tasks.py` & `sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
 
 def list_tasks(project_id: int) -> list[int]:
     """List all tasks in a project."""
     response = CVAT.get(f"tasks?project_id={project_id}")
     tasks = [task["id"] for task in response["results"]]
     while response["next"]:
-        response = CVAT.get(response["next"])
+        _, path = response["next"].split("api/")
+        response = CVAT.get(path)
         tasks.extend([task["id"] for task in response["results"]])
     return tasks
 
 
 def download_annotations(
     task_id: int,
     output_path: Optional[Union[str, Path]] = None,
```

### Comparing `sparrow-cvat-1.1.0.dev1694542729/sparrow_cvat.egg-info/PKG-INFO` & `sparrow-cvat-1.1.0.dev1694543918/sparrow_cvat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-cvat
-Version: 1.1.0.dev1694542729
+Version: 1.1.0.dev1694543918
 Author: Sparrow Computing
 Author-email: ben@sparrow.dev
 License-File: LICENSE
 Requires-Dist: cvat-sdk==2.5.0
 Requires-Dist: fire
 Requires-Dist: pillow
 Requires-Dist: requests
```

