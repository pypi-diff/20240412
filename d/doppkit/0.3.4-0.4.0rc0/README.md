# Comparing `tmp/doppkit-0.3.4.tar.gz` & `tmp/doppkit-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.3.4.tar", last modified: Fri Feb 23 15:19:41 2024, max compression
+gzip compressed data, was "doppkit-0.4.0rc0.tar", last modified: Fri Apr 12 16:10:51 2024, max compression
```

## Comparing `doppkit-0.3.4.tar` & `doppkit-0.4.0rc0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.820289 doppkit-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 15:19:25.000000 doppkit-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-02-23 15:19:41.820289 doppkit-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-23 15:19:25.000000 doppkit-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.820289 doppkit-0.3.4/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-23 15:19:41.000000 doppkit-0.3.4/doppkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-23 15:19:25.000000 doppkit-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 15:19:41.820289 doppkit-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.812289 doppkit-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.816290 doppkit-0.3.4/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.816290 doppkit-0.3.4/src/doppkit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/cli/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.816290 doppkit-0.3.4/src/doppkit/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/ExportView.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/SettingsDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:41.816290 doppkit-0.3.4/src/doppkit/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-02-23 15:19:25.000000 doppkit-0.3.4/src/doppkit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 16:10:51.000000 doppkit-0.4.0rc0/doppkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.779296 doppkit-0.4.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.783296 doppkit-0.4.0rc0/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.783296 doppkit-0.4.0rc0/src/doppkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/src/doppkit/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/ExportView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/SettingsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/UploadView.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:51.787296 doppkit-0.4.0rc0/src/doppkit/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22525 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 16:10:36.000000 doppkit-0.4.0rc0/src/doppkit/util.py
```

### Comparing `doppkit-0.3.4/LICENSE` & `doppkit-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/PKG-INFO` & `doppkit-0.4.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.3.4
+Version: 0.4.0rc0
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.3.4/README.md` & `doppkit-0.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/doppkit.egg-info/PKG-INFO` & `doppkit-0.4.0rc0/doppkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.3.4
+Version: 0.4.0rc0
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.3.4/doppkit.egg-info/SOURCES.txt` & `doppkit-0.4.0rc0/doppkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 doppkit.egg-info/entry_points.txt
 doppkit.egg-info/requires.txt
 doppkit.egg-info/top_level.txt
 src/doppkit/__init__.py
 src/doppkit/app.py
 src/doppkit/cache.py
 src/doppkit/grid.py
+src/doppkit/upload.py
 src/doppkit/util.py
 src/doppkit/cli/__init__.py
 src/doppkit/cli/__main__.py
 src/doppkit/cli/cache.py
 src/doppkit/cli/list.py
 src/doppkit/cli/sync.py
 src/doppkit/gui/ExportView.py
 src/doppkit/gui/LogWidget.py
 src/doppkit/gui/MenuBar.py
 src/doppkit/gui/SettingsDialog.py
+src/doppkit/gui/UploadView.py
 src/doppkit/gui/__init__.py
 src/doppkit/gui/__main__.py
 src/doppkit/gui/cache.py
 src/doppkit/gui/window.py
 src/doppkit/gui/resources/__init__.py
```

### Comparing `doppkit-0.3.4/pyproject.toml` & `doppkit-0.4.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/app.py` & `doppkit-0.4.0rc0/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/cache.py` & `doppkit-0.4.0rc0/src/doppkit/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     name: str = ""
     save_path: str = "."
     total: int = 1
 
 
 class Progress(Protocol):
 
-    def update(self, name: str, url: str, completed: int) -> None:
+    def update(self, name: str, source: str, completed: int) -> None:
         ...
 
-    def create_task(self, name: str, url: str, total: int) -> None:
+    def create_task(self, name: str, source: str, total: int) -> None:
         ...
     
-    def complete_task(self, name: str, url: str) -> None:
+    def complete_task(self, name: str, source: str) -> None:
         ...
 
 
 
 
 class Content:
     def __init__(
```

### Comparing `doppkit-0.3.4/src/doppkit/cli/__main__.py` & `doppkit-0.4.0rc0/src/doppkit/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/cli/cache.py` & `doppkit-0.4.0rc0/src/doppkit/cli/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 class RichProgress:
     
     def __init__(self, context_manager: Progress):
         self.context_manager = context_manager
         self.tasks: dict[str, TaskID] = {}
 
-    def create_task(self, name: str, url: str, total: int):
+    def create_task(self, name: str, source: str, total: int):
         self.tasks[name] = self.context_manager.add_task(name, total=total)
 
-    def update(self, name: str, url: str, completed: int):
+    def update(self, name: str, source: str, completed: int):
         task = self.tasks[name]
         self.context_manager.update(task, completed=completed)
     
-    def complete_task(self, name: str, url: str):
+    def complete_task(self, name: str, source: str):
         task = self.tasks.pop(name)
         self.context_manager.update(task, visible=False)
 
 
 async def cache(app: 'Application', urls: Iterable['DownloadUrl'], headers) -> Iterable[Union[Exception, 'Content']]:
 
     text_column = TextColumn("{task.description}", table_column=Column(ratio=1))
```

### Comparing `doppkit-0.3.4/src/doppkit/cli/list.py` & `doppkit-0.4.0rc0/src/doppkit/cli/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/cli/sync.py` & `doppkit-0.4.0rc0/src/doppkit/cli/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/grid.py` & `doppkit-0.4.0rc0/src/doppkit/grid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 __all__ = ["Grid", "Exportfile", "Export", "AOI"]
 
 import itertools
 import json
 import warnings
 import logging
+import pathlib
+import math
 
 import httpx
-from typing import Optional, Iterable, TypedDict, Union
+from typing import Optional, Iterable, TypedDict, Union, TYPE_CHECKING
 
-from .cache import cache, DownloadUrl
+from .cache import cache, DownloadUrl, Progress
+from .upload import upload
+
+if TYPE_CHECKING:
+    from .upload import ETagDict
 
 logger = logging.getLogger(__name__)
 
 API_VERSION = "v4"
+MULTIPART_BYTES_PER_CHUNK = 10_000_000  # ~ 6mb
 
 aoi_endpoint_ext = f"/api/{API_VERSION}/aois"
 export_endpoint_ext = f"/api/{API_VERSION}/exports"
 task_endpoint_ext = f"/api/{API_VERSION}/tasks"
+upload_endpoint_ext = f"/api/{API_VERSION}/upload"
 
 
 class ExportStarted(TypedDict):
     export_id: str
     task_id: str
 
 
@@ -163,14 +171,87 @@
         else:
             if "error" in response:
                 logger.error(f"GRiD returned the following error: {response['error']}")
                 raise RuntimeError(response['error'])
         return response["aois"]
 
 
+    async def upload_asset(
+            self,
+            filepath: pathlib.Path,
+            bytes_per_chunk=MULTIPART_BYTES_PER_CHUNK,
+            progress: Optional[Progress]=None
+    ):
+        logger.info(f"Starting upload of {filepath}")
+        source_size = filepath.stat().st_size
+        chunks_count = int(math.ceil(source_size / float(bytes_per_chunk)))
+
+        key = f"test-ogi/upload/{filepath.name}"
+        upload_endpoint_url = f"{self.args.url}{upload_endpoint_ext}"
+
+        headers = {"Authorization": f"Bearer {self.args.token}"}
+        async with httpx.AsyncClient(verify=not self.args.disable_ssl_verification) as client:
+            params = {"key": key}
+            response_upload_id = await client.get(
+                f"{upload_endpoint_url}/open/",
+                params=params,
+                headers=headers
+            )
+            logger.debug(f"Upload open call returned {response_upload_id}")
+
+            try:
+                upload_id = response_upload_id.json()["upload_id"]
+            except KeyError as e:
+                if "error" in response_upload_id.json():
+                    raise ConnectionError(response_upload_id.json()["error"]) from e
+                else:
+                    raise ConnectionError(response_upload_id.json()) from e
+
+            params.update(upload_id=upload_id, nparts=str(chunks_count))
+            response_urls = await client.get(
+                f"{upload_endpoint_url}/get_urls/",
+                params=params,
+                headers=headers
+            )
+
+            # want to make sure URLs are in order of part
+            urls = [
+                part['url'] 
+                for part in sorted(
+                    response_urls.json()["parts"],
+                    key=lambda part: part['part']
+                )
+            ]
+
+            part_info = await upload(
+                app=self.args,
+                filepath=filepath,
+                urls=urls,
+                bytes_per_chunk=bytes_per_chunk,
+                auth_header=headers,
+                progress=progress
+            )
+
+            data = {
+                "upload_id": upload_id,
+                "key": key,
+                "upload_info": part_info
+            }
+
+            response_finish = await client.put(
+                f"{upload_endpoint_url}/close/",
+                json=data,
+                headers=headers
+            )
+            logger.debug(f"Upload close call returned {response_finish}")
+            logger.info(f"Finished upload of {filepath}")
+
+        return None
+
+
     async def make_exports(
             self,
             aoi: AOI,
             name: str,
             intersect_types:Optional[Iterable[str]]=None
     ) -> list[ExportStarted]:
         """
@@ -196,15 +277,15 @@
                 product_ids.extend([entry["id"] for entry in aoi["mesh_intersects"]])
             elif intersection == "pointcloud":
                 product_ids.extend([entry["id"] for entry in aoi["pointcloud_intersects"]])
             elif intersection == "vector":
                 product_ids.extend([entry["id"] for entry in aoi["vector_intersects"]])
             else:
                 warnings.warn(
-                    f"Unknown intersect type {intersection}, needs to be one of "
+                    f"Unknown intersect type {intersection}, needs to be one of " +
                     "raster, mesh, pointcloud, or vector.  Ignoring.",
                     stacklevel=2
                 )
         export_endpoint = f"{self.args.url}{export_endpoint_ext}"
 
         # https://pro.arcgis.com/en/pro-app/2.9/arcpy/classes/spatialreference.htm
         # make sure to provide a way to pass in hsrs and vsrs info from arcgis pro
@@ -282,15 +363,15 @@
                 logger.error(f"Doppkit cache function returned unexpected type: {type(export_files[0])}")
                 raise TypeError(
                     f"Cache Function returned unknown type {type(export_files[0])}"
                 ) from e
         else:
             if "error" in response:
                 logger.warning(
-                    f"Attempting to access {export_id=} resulted in the following error "
+                    f"Attempting to access {export_id=} resulted in the following error " +
                     f"from GRiD: {response['error']}"
                 )
                 return []
 
         exports = []
         for f in export_files:
             j = json.loads(f.data)
```

### Comparing `doppkit-0.3.4/src/doppkit/gui/ExportView.py` & `doppkit-0.4.0rc0/src/doppkit/gui/ExportView.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/gui/LogWidget.py` & `doppkit-0.4.0rc0/src/doppkit/gui/LogWidget.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/gui/SettingsDialog.py` & `doppkit-0.4.0rc0/src/doppkit/gui/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/gui/__main__.py` & `doppkit-0.4.0rc0/src/doppkit/gui/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     return True
 
 
 def main():
     app = Application(
         token=None,
         url="https://grid.nga.mil/grid",
-        # log_level=logging.DEBUG,  # override for custom messaging
+        log_level=logging.DEBUG,  # override for custom messaging
         threads=5,
         run_method="GUI",
         progress=True,
         override=False
     )
     # https://github.com/CabbageDevelopment/qasync/issues/68
     # the easy way breaks with Python 3.11, so we do the plumbing ourselves to work around it
```

### Comparing `doppkit-0.3.4/src/doppkit/gui/cache.py` & `doppkit-0.4.0rc0/src/doppkit/gui/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.3.4/src/doppkit/gui/window.py` & `doppkit-0.4.0rc0/src/doppkit/gui/window.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,94 +12,160 @@
 import time
 from urllib.parse import urlparse
 
 import qasync
 
 
 from .ExportView import ExportModel, ExportDelegate
+from .UploadView import UploadModel, UploadItem, UploadDelegate
 from .LogWidget import LoggingDialog
 from .MenuBar import MenuBar
 
 logger = logging.getLogger("doppkit")
 
 
 class ExportFileProgress(NamedTuple):
     url: str
     export_id: int
     current: int = 0
     total: int = 1
     is_complete: bool = False
 
 
-class QtProgress(QtCore.QObject):
+class UploadFileProgress(NamedTuple):
+    path: str
+    current: int = 0
+    total: int = 1
+    is_complete: bool = False
+
+class QtUploadProgress(QtCore.QObject):
+
+    taskCompleted = QtCore.Signal(object)
+    taskAdded = QtCore.Signal(object)
+    taskUpdated = QtCore.Signal(object)
+
+
+    def __init__(self):
+        super().__init__()
+
+        # key is filepath
+        self.upload_progress: dict[str, UploadProgressTracking] = {}
+
+    def create_task(self, name: str, source: str, total: int):
+        """
+        Method adds a task to track the download progress
+
+        Parameters
+        ----------
+        name
+            The name of the file being downloaded
+        source
+            The filepath to file being uploaded
+        total
+            The total size of the file in bytes
+
+        Returns
+        -------
+            None
+        """
+        self.upload_progress[source] = UploadProgressTracking(
+            source,
+            current=0,
+            total=total
+        )
+
+
+    def update(self, name: str, source: str, completed: int) -> None:
+        old_progress = self.upload_progress[source]
+        new_progress = UploadProgressTracking(
+            source,
+            current=completed,
+            total=old_progress.total
+        )
+        self.upload_progress[source] = new_progress
+        self.taskUpdated.emit(new_progress)
+
+    def complete_task(self, name: str, source: str) -> None:
+        old_progress = self.upload_progress[source]
+        self.update(
+            name,
+            source,
+            completed=old_progress.total
+        )
+        new_progress = self.upload_progress[source]
+        self.taskCompleted.emit(new_progress)
+
+
+
+class QtExportProgress(QtCore.QObject):
 
     taskCompleted = QtCore.Signal(object)
     taskAdded = QtCore.Signal(object)
     taskUpdated = QtCore.Signal(object)
 
     def __init__(self):
         super().__init__()
         # key is the export PK
-        self.export_progress: dict[int, ProgressTracking] = {}
+        self.export_progress: dict[int, ExportProgressTracking] = {}
 
         # key is AOI PK
-        self.aois: dict[int, list[ProgressTracking]] = defaultdict(list)
+        self.aois: dict[int, list[ExportProgressTracking]] = defaultdict(list)
 
         self.urls_to_export_id: dict[str, list[int]] = defaultdict(list)
 
         self.export_files: dict[int, dict[str, ExportFileProgress]] = defaultdict(dict)
 
-    def create_task(self, name: str, url: str, total: int):
+    def create_task(self, name: str, source: str, total: int):
         """
         Method adds a task to track the download progress
 
         Parameters
         ----------
         name
             The name of the file being downloaded
-        url
+        source
             The URL to contents of the file are being downloaded from
         total
             The total size of the file in bytes
 
         Returns
         -------
             None
         """
 
-        export_ids = self.urls_to_export_id[url]
+        export_ids = self.urls_to_export_id[source]
         for export_id in export_ids:
-            self.export_files[export_id][url] = ExportFileProgress(
-                url,
+            self.export_files[export_id][source] = ExportFileProgress(
+                source,
                 export_id=export_id,
                 total=total
             )
 
-    def update(self, name: str, url: str, completed: int) -> None:
-        export_ids = self.urls_to_export_id[url]
+    def update(self, name: str, source: str, completed: int) -> None:
+        export_ids = self.urls_to_export_id[source]
         for export_id in export_ids:
-            old_progress = self.export_files[export_id][url]
-            self.export_files[export_id][url] = ExportFileProgress(
-                url,
+            old_progress = self.export_files[export_id][source]
+            self.export_files[export_id][source] = ExportFileProgress(
+                source,
                 export_id=export_id,
                 current=completed,
                 total=old_progress.total,
                 is_complete=completed >= old_progress.total
             )
             export_progress = self.export_progress[export_id]
             export_downloaded = sum(file_progress.current for file_progress in self.export_files[export_id].values())
             export_progress.update(export_downloaded)
             self.taskUpdated.emit(export_progress)
 
-    def complete_task(self, name: str, url: str) -> None:
-        export_ids = self.urls_to_export_id[url]
+    def complete_task(self, name: str, source: str) -> None:
+        export_ids = self.urls_to_export_id[source]
 
         for export_id in export_ids:
-            old_progress = self.export_files[export_id][url]
-            self.update(name, url, old_progress.total)
+            old_progress = self.export_files[export_id][source]
+            self.update(name, source, old_progress.total)
             export_progress = self.export_progress[export_id]
             if all(export_file.is_complete for export_file in self.export_files[export_id].values()):
                 export_progress.is_complete = True
                 self.taskCompleted.emit(export_progress)
 
     def update_export_progress(self):
         pass
@@ -143,15 +209,15 @@
 
         self.setGeometry(300, 300, 300, 220)
         self.setWindowTitle(f"doppkit - {__version__}")
         self.doppkit = doppkit_application
         self.AOI_ids: list[int] = []
         self.AOIs: list[AOI] = []  # populated from GRiD
 
-        self.progressTracker = QtProgress()
+        self.exportProgressTracker = QtExportProgress()
 
         # Download Progress Viewer
         self.exportView = None
 
         # Log Viewer
         self.logView = LoggingDialog()
 
@@ -277,31 +343,34 @@
         if ssl_white_list is None:
             # setting default URLs to skip
             ssl_white_list = ["https://grid.nga.smil.mil", "https://grid.nga.ic.gov"]
             settings.setValue("grid/ssl_url_white_list", ssl_white_list)
 
         # populate fields with previously stored values or defaults otherwise
         tokenLineEdit.setText(settings.value("grid/token"))
+        self.doppkit.token = settings.value("grid/token")
 
         urlLineComboBox.setEditText(str(settings.value("grid/url", "https://grid.nga.mil/grid")))
         
         downloadLineEdit.setText(
             str(
                 settings.value(
                     "grid/download",
                     QtCore.QStandardPaths.standardLocations(
                         QtCore.QStandardPaths.StandardLocation.DownloadLocation
                     )[0]
                 )
             )
         )
 
-        self.progressInterconnect = QtProgress()
+        self.progressInterconnect = QtExportProgress()
+        self.uploadProgressInterconnect = QtUploadProgress()
         self.show()
 
+
     def closeEvent(self, evt: QtGui.QCloseEvent) -> None:
         settings = QtCore.QSettings()
         settings.beginGroup("MainWindow")
         settings.setValue("geometry", self.saveGeometry())
         settings.endGroup()
 
     def showDownloadDialog(self, checked:bool = False):
@@ -340,14 +409,47 @@
 
     def tokenChanged(self) -> None:
         self.doppkit.token = self.sender().text().strip()
         setting = QtCore.QSettings()
         setting.setValue("grid/token", self.doppkit.token)
 
     @qasync.asyncSlot()
+    async def uploadFiles(self, files: list[str]):
+
+        items = [
+            UploadItem(filepath, self.uploadProgressInterconnect)
+            for filepath in files
+        ]
+
+        api = Grid(self.doppkit)
+        model = UploadModel()
+        model.load(items, self.uploadProgressInterconnect)
+
+        self.uploadView = QtWidgets.QListView()
+        self.uploadView.setSelectionMode(
+            QtWidgets.QAbstractItemView.SelectionMode.NoSelection
+        )
+        self.uploadView.setWordWrap(False)
+
+        self.uploadView.setModel(model)
+        self.uploadView.setTextElideMode(QtCore.Qt.TextElideMode.ElideMiddle)
+        self.uploadView.setUniformItemSizes(True)
+        self.uploadView.setModel(model)
+        self.uploadView.setItemDelegateForColumn(0, UploadDelegate())
+        self.uploadView.show()
+
+        for file_ in files:
+            await api.upload_asset(
+                pathlib.Path(file_),
+                progress=self.uploadProgressInterconnect
+            )
+
+        logger.debug("Uploads Finished")
+
+    @qasync.asyncSlot()
     async def listExports(self):
         self.buttonList.setEnabled(False)
         # TODO: this should accept a list of AOIs
 
         # need to determine if we should skip SSL verification...
         # first, is SSL verification enabled?
         settings = QtCore.QSettings()
@@ -435,15 +537,15 @@
                         logger.debug(f"File already exists, skipping {filename}")
                     else:
                         urls.append(
                             download_file
                         )
                         download_size += download_file.total
                         self.progressInterconnect.urls_to_export_id[download_file.url].append(export["id"])
-                progress_tracker = ProgressTracking(
+                progress_tracker = ExportProgressTracking(
                     export["id"],
                     export_name=export["name"],
                     aoi_id=aoi["id"],
                     aoi_name=aoi["name"],
                     current=0,
                     total=download_size   # export["complete_size"] is inaccurate for the time being...
                 )
@@ -452,16 +554,62 @@
 
         try:
             _ = await cache(self.doppkit, urls, {}, progress=self.progressInterconnect)
             logger.info("Download AOI Exports Complete")
         finally:
             self.buttonDownload.setEnabled(True)
 
+
+@dataclass
+class UploadProgressTracking:
+    path: str
+    current: int
+    total: int
+    elapsed: float = time.perf_counter()
+    rate: float = 0.0
+    is_complete: bool = False
+    rate_update_timer = time.perf_counter()
+
+    def ratio(self) -> float:
+        try:
+            ratio = self.current / self.total
+        except ZeroDivisionError:
+            ratio = 0.0
+        else:
+            if math.floor(100 * ratio) > 100:
+                logger.warning(
+                    f"Completed download ratio for {os.path.basename(self.path)} calculated " +
+                    f"to be {self.current=}/{self.total=}={ratio} (> 1.0), " +
+                    "likely incorrect..."
+                )
+                return 1.0
+        return ratio
+
+    def percentage(self) -> int:
+        return math.floor(100 * self.ratio())
+
+    def int32_progress(self):
+        return math.floor(((2 ** 32 - 1) // 2) * self.ratio())
+
+    def update(self, current: int) -> None:
+        old_current = self.current
+        self.current = current
+        diff = current - old_current
+        now = time.perf_counter()
+        duration = now - self.elapsed
+        self.rate = diff / duration
+        if now - self.rate_update_timer > 1.0:
+            # self.update_download_rate()
+            self.rate_update_timer = now
+        self.elapsed = now
+
+
+
 @dataclass
-class ProgressTracking:
+class ExportProgressTracking:
     export_id: int
     export_name: str
     aoi_id: int
     aoi_name: str
     current: int
     total: int
     elapsed: float = time.perf_counter()
@@ -473,16 +621,16 @@
         try:
             ratio = self.current / self.total
         except ZeroDivisionError:
             ratio = 0.0
         else:
             if math.floor(100 * ratio) > 100:
                 logger.warning(
-                    f"Completed download ratio for {self.export_name} calculated "
-                    f"to be {self.current=}/{self.total=}={ratio} (> 1.0), "
+                    f"Completed download ratio for {self.export_name} calculated " +
+                    f"to be {self.current=}/{self.total=}={ratio} (> 1.0), " +
                     "likely incorrect..."
                 )
                 return 1.0
         return ratio
 
     def percentage(self) -> int:
         return math.floor(100 * self.ratio())
```

### Comparing `doppkit-0.3.4/src/doppkit/util.py` & `doppkit-0.4.0rc0/src/doppkit/util.py`

 * *Files identical despite different names*

