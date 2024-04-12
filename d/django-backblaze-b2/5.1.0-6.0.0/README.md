# Comparing `tmp/django_backblaze_b2-5.1.0.tar.gz` & `tmp/django_backblaze_b2-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-5.1.0.tar", max compression
+gzip compressed data, was "django_backblaze_b2-6.0.0.tar", max compression
```

## Comparing `django_backblaze_b2-5.1.0.tar` & `django_backblaze_b2-6.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-5.1.0/LICENSE
--rw-r--r--   0        0        0     8601 2023-12-26 01:12:14.843342 django_backblaze_b2-5.1.0/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-5.1.0/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-5.1.0/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2609 2024-01-15 10:06:54.551992 django_backblaze_b2-5.1.0/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     7933 2023-12-26 01:12:14.843664 django_backblaze_b2-5.1.0/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     2604 2024-01-15 10:06:54.552160 django_backblaze_b2-5.1.0/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-5.1.0/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    13851 2024-01-15 10:30:36.902989 django_backblaze_b2-5.1.0/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     6942 2024-01-15 10:06:54.552583 django_backblaze_b2-5.1.0/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      358 2023-12-07 08:45:21.614957 django_backblaze_b2-5.1.0/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-5.1.0/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     2074 2024-01-15 10:30:39.145056 django_backblaze_b2-5.1.0/pyproject.toml
--rw-r--r--   0        0        0    10228 1970-01-01 00:00:00.000000 django_backblaze_b2-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-6.0.0/LICENSE
+-rw-r--r--   0        0        0     8601 2023-12-26 01:12:14.843342 django_backblaze_b2-6.0.0/README.md
+-rw-r--r--   0        0        0      264 2024-04-12 07:47:07.915791 django_backblaze_b2-6.0.0/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-6.0.0/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2609 2024-01-15 10:06:54.551992 django_backblaze_b2-6.0.0/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7897 2024-04-12 07:37:57.501120 django_backblaze_b2-6.0.0/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     2604 2024-01-15 10:06:54.552160 django_backblaze_b2-6.0.0/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-6.0.0/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    13739 2024-04-12 07:37:57.501525 django_backblaze_b2-6.0.0/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     6942 2024-01-15 10:06:54.552583 django_backblaze_b2-6.0.0/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      358 2023-12-07 08:45:21.614957 django_backblaze_b2-6.0.0/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-6.0.0/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     2160 2024-04-12 07:47:07.916260 django_backblaze_b2-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10234 1970-01-01 00:00:00.000000 django_backblaze_b2-6.0.0/PKG-INFO
```

### Comparing `django_backblaze_b2-5.1.0/LICENSE` & `django_backblaze_b2-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/README.md` & `django_backblaze_b2-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/_decorators.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/b2_file.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/cache_account_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import threading
 from functools import wraps
 from hashlib import sha3_224 as hash
 from typing import Iterable, List, Optional, Tuple
 
-from b2sdk.account_info.exception import MissingAccountData
-from b2sdk.account_info.upload_url_pool import UrlPoolAccountInfo
+from b2sdk.v2 import UrlPoolAccountInfo
+from b2sdk.v2.exception import MissingAccountData
 from django.core.cache import InvalidCacheBackendError, caches
 from django.core.exceptions import ImproperlyConfigured
 
 logger = logging.getLogger("django-backblaze-b2")
 
 
 class StoredBucketInfo:
```

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/options.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/options.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/storage.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from datetime import datetime
 from hashlib import sha3_224 as hash
 from logging import getLogger
 from typing import IO, Any, Callable, Dict, List, Optional, Tuple, cast
 
-from b2sdk.account_info import InMemoryAccountInfo
-from b2sdk.account_info.sqlite_account_info import SqliteAccountInfo
-from b2sdk.cache import AuthInfoCache
-from b2sdk.exception import FileOrBucketNotFound, NonExistentBucket
-from b2sdk.v2 import AbstractAccountInfo, B2Api, Bucket
+from b2sdk.v2 import AbstractAccountInfo, AuthInfoCache, B2Api, Bucket, InMemoryAccountInfo, SqliteAccountInfo
+from b2sdk.v2.exception import FileNotPresent, NonExistentBucket
 from django.core.cache.backends.base import BaseCache
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.base import File
 from django.core.files.storage import Storage
 from django.utils.deconstruct import deconstructible
 from typing_extensions import NotRequired, TypedDict, TypeVar, Unpack
 
@@ -216,15 +213,15 @@
 
                 def load_info():
                     logger.debug(f"file info cache miss for {name}")
                     return self.bucket.get_file_info_by_name(name).as_dict()
 
                 return self._cache.get_or_set(key=cache_key, default=load_info, timeout=timeout_in_seconds)
             return self.bucket.get_file_info_by_name(name).as_dict()
-        except FileOrBucketNotFound:
+        except FileNotPresent:
             return None
 
     def _file_cache_key(self, name: str) -> str:
         return hash(f"{self.bucket.name}__{name}".encode()).hexdigest()
 
     @property
     def _cache(self) -> Optional[BaseCache]:
```

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/storages.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/storages.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/django_backblaze_b2/views.py` & `django_backblaze_b2-6.0.0/django_backblaze_b2/views.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-5.1.0/pyproject.toml` & `django_backblaze_b2-6.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-backblaze-b2"
-version = "5.1.0"
+version = "6.0.0"
 description = "A Django app to use backblaze b2 as storage."
 authors = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 maintainers = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/ehossack/django-backblaze-b2/"
 repository = "https://github.com/ehossack/django-backblaze-b2/"
@@ -31,37 +31,40 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-b2sdk = ">=1.23.0"
+b2sdk = ">=2.0.0,<3.0.0"
 django = ">=3.2"
 typing-extensions = "^4.0.1"
 
 [tool.poetry.group.dev.dependencies]
 django-stubs = "^4.2.7"
-pytest = "^7.4"
+pytest = ">=7.4,<9.0"
 mypy = ">=0.8"
-pytest-cov = "^4.1"
+pytest-cov = ">=4.1,<6.0"
 pytest-django = "^4.5"
 pytest-pythonpath = "^0.7"
 docutils = "^0.20"
 toml = "^0.10.2"
-ruff = "^0.1.7"
+ruff = ">=0.1.7,<0.4.0"
+types-toml = "^0.10.8.20240310"
 
 [build-system]
 requires = ["poetry>=1.5.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.ruff]
 exclude = [".git", "__pycache__", ".mypy_stubs"]
-ignore = []
 line-length = 120
+
+[tool.ruff.lint]
+ignore = []
 select = ["C9", "E", "F", "I", "N", "W"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 10
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/test_project/django_project/settings.py" = ["F841"]
```

### Comparing `django_backblaze_b2-5.1.0/PKG-INFO` & `django_backblaze_b2-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backblaze-b2
-Version: 5.1.0
+Version: 6.0.0
 Summary: A Django app to use backblaze b2 as storage.
 Home-page: https://github.com/ehossack/django-backblaze-b2/
 License: BSD-2-Clause
 Keywords: django,storage,backblaze,b2,cloud
 Author: Etienne H
 Author-email: django_backblaze_b2@internet-e-mail.com
 Maintainer: Etienne H
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: b2sdk (>=1.23.0)
+Requires-Dist: b2sdk (>=2.0.0,<3.0.0)
 Requires-Dist: django (>=3.2)
 Requires-Dist: typing-extensions (>=4.0.1,<5.0.0)
 Project-URL: Repository, https://github.com/ehossack/django-backblaze-b2/
 Description-Content-Type: text/markdown
 
 # django-backblaze-b2
```

