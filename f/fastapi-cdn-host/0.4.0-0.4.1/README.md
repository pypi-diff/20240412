# Comparing `tmp/fastapi_cdn_host-0.4.0.tar.gz` & `tmp/fastapi_cdn_host-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cdn_host-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_cdn_host-0.4.1.tar", max compression
```

## Comparing `fastapi_cdn_host-0.4.0.tar` & `fastapi_cdn_host-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.0/LICENSE
--rw-r--r--   0        0        0     2466 2023-12-29 15:22:24.861442 fastapi_cdn_host-0.4.0/README.md
--rw-r--r--   0        0        0      305 2023-12-16 08:55:13.797819 fastapi_cdn_host-0.4.0/fastapi_cdn_host/__init__.py
--rw-r--r--   0        0        0    15385 2024-01-10 09:12:03.170240 fastapi_cdn_host-0.4.0/fastapi_cdn_host/client.py
--rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.0/fastapi_cdn_host/py.typed
--rw-r--r--   0        0        0      882 2024-01-10 09:13:36.033696 fastapi_cdn_host-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2466 2023-12-29 15:22:24.861442 fastapi_cdn_host-0.4.1/README.md
+-rw-r--r--   0        0        0      356 2024-04-11 07:19:56.277789 fastapi_cdn_host-0.4.1/fastapi_cdn_host/__init__.py
+-rw-r--r--   0        0        0    18466 2024-04-11 07:19:56.278335 fastapi_cdn_host-0.4.1/fastapi_cdn_host/client.py
+-rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.1/fastapi_cdn_host/py.typed
+-rw-r--r--   0        0        0      980 2024-04-11 09:10:18.051455 fastapi_cdn_host-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.1/PKG-INFO
```

### Comparing `fastapi_cdn_host-0.4.0/LICENSE` & `fastapi_cdn_host-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.0/README.md` & `fastapi_cdn_host-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.0/fastapi_cdn_host/client.py` & `fastapi_cdn_host-0.4.1/fastapi_cdn_host/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
+import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import anyio
 import httpx
 from fastapi import FastAPI, Request
+from fastapi.datastructures import URL
 from fastapi.openapi.docs import get_redoc_html, get_swagger_ui_html
 from fastapi.responses import HTMLResponse
 from fastapi.routing import APIRoute, Mount
 from fastapi.staticfiles import StaticFiles
 from typing_extensions import Annotated  # type: ignore[attr-defined]
 
 logger = logging.getLogger("fastapi-cdn-host")
@@ -27,24 +29,87 @@
 CdnHostInfoType = Union[
     Annotated[CdnDomainType, f"Will use DEFAULT_ASSET_PATH: {DEFAULT_ASSET_PATH}"],
     Tuple[CdnDomainType, Annotated[str, "In case of swagger/redoc has the same path"]],
     StrictCdnHostInfoType,
 ]
 
 
+class CdnHostItem:
+    """For cdn host url parse
+
+    Usage::
+        >>> CdnHostItem('https://raw.githubusercontent.com/swagger-api/swagger-ui/v5.14.0/dist/swagger-ui.css').export()
+        ('https://raw.githubusercontent.com/swagger-api/swagger-ui', ("/v{version}/dist/", ""))
+    """
+
+    def __init__(self, swagger_ui: str, redoc: Union[str, None] = "") -> None:
+        self.swagger_ui = swagger_ui
+        self.redoc = redoc
+
+    @staticmethod
+    def remove_filename(url: str) -> str:
+        """Remove last part of url if '.' in it
+
+        Usage::
+            >>> remove_filename('http://localhost:8000/a/b/c.js')
+            'http://localhost:8000/a/b/'
+            >>> remove_filename('http://localhost:8000/a/b')
+            'http://localhost:8000/a/b/'
+        """
+        sep = "://"
+        ps = url.split(sep)
+        path = ps[-1]
+        if not path.endswith("/"):
+            parts = path.split("/")
+            if "." in parts[-1]:
+                parts[-1] = ""
+            else:
+                parts.append("")
+            ps[-1] = "/".join(parts)
+        return sep.join(ps)
+
+    def export(self) -> StrictCdnHostInfoType:
+        url = URL(self.remove_filename(self.swagger_ui))
+        if not (scheme := url.scheme) or not (hostname := url.hostname):
+            raise ValueError(f"Invalid ({url!r}) -- missing scheme or hostname")
+        parts = url.path.split("/")
+        for index, value in enumerate(parts):
+            if re.match(r"swagger-ui\b", value):
+                break
+        host = cast(str, scheme) + "://" + cast(str, hostname) + "/".join(parts[:index])
+        swagger_path = re.sub(
+            r"\d+\.\d+\.\d+", "{version}", "/".join([""] + parts[index:])
+        )
+        if self.redoc is None:
+            redoc_path = DEFAULT_ASSET_PATH[-1]
+        else:
+            if (redoc_path := self.redoc) and not redoc_path.endswith("/"):
+                redoc_path = self.remove_filename(redoc_path)
+        return (host, (swagger_path, redoc_path))
+
+
 class CdnHostEnum(Enum):
     jsdelivr: CdnHostInfoType = "https://cdn.jsdelivr.net/npm"
     unpkg: CdnHostInfoType = "https://unpkg.com"
     cdnjs: CdnHostInfoType = "https://cdnjs.cloudflare.com/ajax/libs", NORMAL_ASSET_PATH
     bootcdn: CdnHostInfoType = "https://cdn.bootcdn.net/ajax/libs", NORMAL_ASSET_PATH
     qiniu: CdnHostInfoType = "https://cdn.staticfile.org", NORMAL_ASSET_PATH
 
     @classmethod
-    def extend(cls, *host: StrictCdnHostInfoType) -> List[CdnHostInfoType]:
-        return [*host, *cls]
+    def extend(
+        cls, *host: Union[StrictCdnHostInfoType, CdnHostItem]
+    ) -> List[CdnHostInfoType]:
+        host_infos: List[StrictCdnHostInfoType] = []
+        for i in host:
+            if isinstance(i, CdnHostItem):
+                j = i.export()
+                host_infos.append(j)
+            else:
+                host_infos.append(i)
+        return [*host_infos, *cls]
 
 
 @dataclass
 class AssetUrl:
     css: Annotated[str, "URL of swagger-ui.css"]
     js: Annotated[str, "URL of swagger-ui-bundle.js"]
     redoc: Annotated[str, "URL of redoc.standalone.js"]
@@ -70,28 +135,44 @@
                 results[index] = r.content
 
     @classmethod
     async def find_fastest_host(
         cls, urls: List[str], total_seconds=5, loop_interval=0.1
     ) -> str:
         results = [None] * len(urls)
-        async with anyio.create_task_group() as tg:
-            async with httpx.AsyncClient(timeout=total_seconds) as client:
+        async with httpx.AsyncClient(timeout=total_seconds) as client:
+            async with anyio.create_task_group() as tg:
                 for i, url in enumerate(urls):
                     tg.start_soon(cls.fetch, client, url, results, i)
                 for _ in range(int(total_seconds / loop_interval) + 1):
                     if any(r is not None for r in results):
                         tg.cancel_scope.cancel()
                         break
                     await anyio.sleep(loop_interval)
         for url, res in zip(urls, results):
             if res is not None:
                 return url
         return urls[0]
 
+    @classmethod
+    async def get_fast_hosts(
+        cls, urls: List[str], wait_seconds=0.8, total_seconds=5
+    ) -> List[str]:
+        results = [None] * len(urls)
+        async with httpx.AsyncClient(timeout=total_seconds) as client:
+            async with anyio.create_task_group() as tg:
+                for i, url in enumerate(urls):
+                    tg.start_soon(cls.fetch, client, url, results, i)
+                for _ in range(int(total_seconds / wait_seconds)):
+                    await anyio.sleep(wait_seconds)
+                    if any(r is not None for r in results):
+                        tg.cancel_scope.cancel()
+                        break
+        return [url for url, res in zip(urls, results) if res is not None]
+
 
 class CdnHostBuilder:
     swagger_ui_version = "5.9.0"  # to be optimize: auto get version from fastapi
     swagger_files = {"css": "swagger-ui.css", "js": "swagger-ui-bundle.js"}
     redoc_file = "redoc.standalone.js"
 
     def __init__(self, app=None, docs_cdn_host=None, favicon_url=None) -> None:
```

### Comparing `fastapi_cdn_host-0.4.0/pyproject.toml` & `fastapi_cdn_host-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 [tool.poetry]
 name = "fastapi-cdn-host"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {version = ">=0.100"}
 httpx = {version = ">=0.23"}
 
 
 [tool.poetry.group.dev.dependencies]
 fast-tort-cli = {extras = ["all"], version="*", python=">=3.11"}
+asyncur = {version=">=0.4.2", python=">=3.11"}
 uvicorn = {extras = ["standard"], version = "*"}
 isort = "*"
 black = "*"
 ruff = "*"
 mypy = "*"
 pytest = "*"
-bandit = "^1.7.5"
+coverage = "*"
+bandit = "^1.7.8"
+starlette = "*"
+pydantic = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile="black"
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 explicit_package_bases = true
 check_untyped_defs = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "test_*.py" = ["E501"]
 
 [tool.coverage.run]
 branch = true
 parallel=true
 source = ["fastapi_cdn_host"]
 [tool.coverage.report]
```

### Comparing `fastapi_cdn_host-0.4.0/PKG-INFO` & `fastapi_cdn_host-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cdn-host
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

