# Comparing `tmp/arcsecond-3.0.3.tar.gz` & `tmp/arcsecond-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcsecond-3.0.3.tar", last modified: Mon Apr  8 12:34:40 2024, max compression
+gzip compressed data, was "arcsecond-3.1.0.tar", last modified: Fri Apr 12 06:14:13 2024, max compression
```

## Comparing `arcsecond-3.0.3.tar` & `arcsecond-3.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.645067 arcsecond-3.0.3/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.0.3/LICENSE
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-08 12:34:40.644999 arcsecond-3.0.3/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.0.3/README.md
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.638539 arcsecond-3.0.3/arcsecond/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      269 2024-04-08 12:34:16.000000 arcsecond-3.0.3/arcsecond/__init__.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.640847 arcsecond-3.0.3/arcsecond/api/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.0.3/arcsecond/api/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4643 2024-04-08 12:33:03.000000 arcsecond-3.0.3/arcsecond/api/config.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.0.3/arcsecond/api/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4198 2024-03-31 12:57:46.000000 arcsecond-3.0.3/arcsecond/api/endpoint.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-03-31 13:03:41.000000 arcsecond-3.0.3/arcsecond/api/main.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     6312 2024-03-31 14:44:54.000000 arcsecond-3.0.3/arcsecond/cli.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      149 2024-03-31 12:00:33.000000 arcsecond-3.0.3/arcsecond/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.0.3/arcsecond/options.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.643275 arcsecond-3.0.3/arcsecond/uploader/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2024-03-21 21:27:31.000000 arcsecond-3.0.3/arcsecond/uploader/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1377 2024-03-31 07:22:21.000000 arcsecond-3.0.3/arcsecond/uploader/constants.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4060 2024-03-31 13:08:01.000000 arcsecond-3.0.3/arcsecond/uploader/context.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2453 2024-03-31 13:04:03.000000 arcsecond-3.0.3/arcsecond/uploader/errors.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1060 2024-03-31 14:43:40.000000 arcsecond-3.0.3/arcsecond/uploader/logger.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     4725 2024-03-31 07:26:36.000000 arcsecond-3.0.3/arcsecond/uploader/uploader.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     2801 2024-03-31 07:23:32.000000 arcsecond-3.0.3/arcsecond/uploader/utils.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     3477 2024-03-31 14:44:07.000000 arcsecond-3.0.3/arcsecond/uploader/walker.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.639710 arcsecond-3.0.3/arcsecond.egg-info/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/PKG-INFO
--rw-r--r--   0 onekiloparsec   (501) staff       (20)      877 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/SOURCES.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/dependency_links.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/entry_points.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/not-zip-safe
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/requires.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-04-08 12:34:40.000000 arcsecond-3.0.3/arcsecond.egg-info/top_level.txt
--rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-04-08 12:34:40.645298 arcsecond-3.0.3/setup.cfg
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1621 2024-03-24 20:33:09.000000 arcsecond-3.0.3/setup.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.636900 arcsecond-3.0.3/tests/
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.643977 arcsecond-3.0.3/tests/cli/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.3/tests/cli/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.0.3/tests/cli/test_cli_options.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.0.3/tests/cli/test_config.py
-drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-08 12:34:40.644655 arcsecond-3.0.3/tests/module/
--rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.0.3/tests/module/__init__.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.0.3/tests/module/test_arcsecond_root.py
--rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.0.3/tests/module/test_login.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.617282 arcsecond-3.1.0/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1072 2018-07-30 07:31:57.000000 arcsecond-3.1.0/LICENSE
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-12 06:14:13.617219 arcsecond-3.1.0/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1029 2024-03-31 14:10:14.000000 arcsecond-3.1.0/README.md
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.611600 arcsecond-3.1.0/arcsecond/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      269 2024-04-12 06:13:35.000000 arcsecond-3.1.0/arcsecond/__init__.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.613875 arcsecond-3.1.0/arcsecond/api/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      203 2024-03-31 12:00:54.000000 arcsecond-3.1.0/arcsecond/api/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4643 2024-04-08 12:33:03.000000 arcsecond-3.1.0/arcsecond/api/config.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      304 2024-03-31 14:42:08.000000 arcsecond-3.1.0/arcsecond/api/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4271 2024-04-12 06:06:33.000000 arcsecond-3.1.0/arcsecond/api/endpoint.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2443 2024-04-12 06:01:52.000000 arcsecond-3.1.0/arcsecond/api/main.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     6312 2024-03-31 14:44:54.000000 arcsecond-3.1.0/arcsecond/cli.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      190 2024-04-11 12:35:40.000000 arcsecond-3.1.0/arcsecond/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2277 2024-03-31 14:34:46.000000 arcsecond-3.1.0/arcsecond/options.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.615688 arcsecond-3.1.0/arcsecond/uploader/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2024-03-21 21:27:31.000000 arcsecond-3.1.0/arcsecond/uploader/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1401 2024-04-11 12:56:04.000000 arcsecond-3.1.0/arcsecond/uploader/constants.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4060 2024-04-11 12:33:52.000000 arcsecond-3.1.0/arcsecond/uploader/context.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2508 2024-04-11 10:17:13.000000 arcsecond-3.1.0/arcsecond/uploader/errors.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1061 2024-04-12 06:11:19.000000 arcsecond-3.1.0/arcsecond/uploader/logger.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     5481 2024-04-12 06:04:34.000000 arcsecond-3.1.0/arcsecond/uploader/uploader.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     2801 2024-03-31 07:23:32.000000 arcsecond-3.1.0/arcsecond/uploader/utils.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     4079 2024-04-12 06:12:47.000000 arcsecond-3.1.0/arcsecond/uploader/walker.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.612774 arcsecond-3.1.0/arcsecond.egg-info/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1900 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/PKG-INFO
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)      877 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/SOURCES.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/dependency_links.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       49 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/entry_points.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        1 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/not-zip-safe
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       55 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/requires.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       16 2024-04-12 06:14:13.000000 arcsecond-3.1.0/arcsecond.egg-info/top_level.txt
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)       61 2024-04-12 06:14:13.617480 arcsecond-3.1.0/setup.cfg
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1621 2024-03-24 20:33:09.000000 arcsecond-3.1.0/setup.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.610148 arcsecond-3.1.0/tests/
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.616253 arcsecond-3.1.0/tests/cli/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.1.0/tests/cli/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1551 2024-03-31 12:07:38.000000 arcsecond-3.1.0/tests/cli/test_cli_options.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1383 2024-03-29 18:20:59.000000 arcsecond-3.1.0/tests/cli/test_config.py
+drwxr-xr-x   0 onekiloparsec   (501) staff       (20)        0 2024-04-12 06:14:13.616892 arcsecond-3.1.0/tests/module/
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)        0 2020-04-01 16:34:29.000000 arcsecond-3.1.0/tests/module/__init__.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1133 2024-03-29 09:03:34.000000 arcsecond-3.1.0/tests/module/test_arcsecond_root.py
+-rw-r--r--   0 onekiloparsec   (501) staff       (20)     1092 2024-03-29 18:42:28.000000 arcsecond-3.1.0/tests/module/test_login.py
```

### Comparing `arcsecond-3.0.3/LICENSE` & `arcsecond-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/PKG-INFO` & `arcsecond-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.0.3
+Version: 3.1.0
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.0.3/README.md` & `arcsecond-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/api/config.py` & `arcsecond-3.1.0/arcsecond/api/config.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/api/endpoint.py` & `arcsecond-3.1.0/arcsecond/api/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,17 @@
         if isinstance(response, dict):
             # Responses of standard JSON payload requests are dict
             return response, None
         elif response is not None:
             if 200 <= response.status_code < 300:
                 return response.json() if response.text else {}, None
             else:
-                return None, response.text
+                return None, ArcsecondError(response.text, response.status_code)
         else:
-            return None, ArcsecondError()
+            return None, ArcsecondError(response.text, response.status_code)
 
     def _check_and_set_auth_key(self, headers, url):
         # No token header for login and register
         if API_AUTH_PATH_VERIFY in url or API_AUTH_PATH_VERIFY_PORTAL in url or 'Authorization' in headers.keys():
             return headers
 
         if self.__config.verbose:
```

### Comparing `arcsecond-3.0.3/arcsecond/api/main.py` & `arcsecond-3.1.0/arcsecond/api/main.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/cli.py` & `arcsecond-3.1.0/arcsecond/cli.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/options.py` & `arcsecond-3.1.0/arcsecond/options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/uploader/constants.py` & `arcsecond-3.1.0/arcsecond/uploader/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 class Status(Enum):
     NEW = 'New'
     PREPARING = 'Preparing'
     UPLOADING = 'Uploading'
     FINISHING = 'Finishing'
     OK = 'OK'
+    SKIPPED = 'Skipped'
     ERROR = 'Error'
 
 
 class Substatus(Enum):
     PENDING = 'pending'
     CHECKING = 'checking remote file...'
     UPLOADING = 'uploading...'
```

### Comparing `arcsecond-3.0.3/arcsecond/uploader/context.py` & `arcsecond-3.1.0/arcsecond/uploader/context.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 
 import click
 
-from arcsecond.api.constants import API_AUTH_PATH_VERIFY_PORTAL
 from arcsecond import ArcsecondAPI, ArcsecondConfig, ArcsecondAPIEndpoint
+from arcsecond.api.constants import API_AUTH_PATH_VERIFY_PORTAL
 from .errors import (
     UnknownOrganisationError,
     InvalidAstronomerError,
     InvalidWatchOptionsError,
     InvalidOrganisationDatasetError,
     InvalidDatasetError,
     InvalidOrgMembershipError
```

### Comparing `arcsecond-3.0.3/arcsecond/uploader/errors.py` & `arcsecond-3.1.0/arcsecond/uploader/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from arcsecond.errors import ArcsecondError
 
 
-class UploadRemoteFileCheckError(ArcsecondError):
+class UploadRemoteFileError(ArcsecondError):
+    pass
+
+
+class UploadRemoteFileTagsError(ArcsecondError):
     pass
 
 
 class UploadRemoteDatasetCheckError(ArcsecondError):
     pass
```

### Comparing `arcsecond-3.0.3/arcsecond/uploader/logger.py` & `arcsecond-3.1.0/arcsecond/uploader/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from datetime import datetime
 from logging import DEBUG, FileHandler, Formatter, INFO, Logger, StreamHandler, getLogger
 from pathlib import Path
 
 
 def get_oort_logger(debug=False) -> Logger:
-    suffix = '-tests' if os.environ.get('OORT_TESTS') == '1' else ''
+    suffix = ' (test)' if os.environ.get('OORT_TESTS') == '1' else ''
     logger = getLogger('arcsecond' + suffix)
     logger.setLevel(DEBUG if debug else INFO)
 
     if len(logger.handlers) == 0:
         formatter = Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
         if os.environ.get('OORT_TESTS') != '1':
```

### Comparing `arcsecond-3.0.3/arcsecond/uploader/uploader.py` & `arcsecond-3.1.0/arcsecond/uploader/uploader.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 from arcsecond import ArcsecondAPI
 from arcsecond import __version__
 from .constants import Status, Substatus
 from .context import Context
-from .errors import UploadRemoteDatasetCheckError, UploadRemoteFileCheckError
+from .errors import UploadRemoteDatasetCheckError, UploadRemoteFileError, UploadRemoteFileTagsError
 from .logger import get_oort_logger
 
 
 class FileUploader(object):
     def __init__(self, context: Context, root_path: Path, file_path: Path, display_progress: bool = False):
         self._context = context
         self._root_path = root_path
@@ -26,87 +26,104 @@
         self._is_test_context = bool(os.environ.get('OORT_TESTS') == '1')
         self._status = [Status.NEW, Substatus.PENDING, None]
 
         self._api = ArcsecondAPI(self._context.config, self._context.organisation_subdomain)
 
     @property
     def log_prefix(self) -> str:
-        return f'[FileUploader: {str(self._file_path.relative_to(self._root_path))}]'
+        return f'[{str(self._file_path.relative_to(self._root_path))}]'
+
+    @property
+    def _file_size(self) -> int:
+        return self._file_path.stat().st_size
 
     def _prepare_dataset(self):
+        self._logger.info(f'{self.log_prefix} Preparing Dataset...')
+        self._status = [Status.PREPARING, Substatus.CHECKING, None]
+
         if self._context.dataset_uuid:
             response, error = self._api.datasets.read(self._context.dataset_uuid)
             if error:
                 raise UploadRemoteDatasetCheckError(str(error))
             self._context.update_dataset(response)
+            self._logger.info(f'{self.log_prefix} Dataset preparation done.')
 
         elif self._context.dataset_name:
             # Dataset UUID is empty, and CLI validators have already checked this dataset doesn't exist.
             # Simply create dataset.
             response, error = self._api.datasets.create({'name': self._context.dataset_name})
             if error:
                 raise UploadRemoteDatasetCheckError(str(error))
             self._context.update_dataset(response)
+            self._logger.info(f'{self.log_prefix} Dataset preparation done.')
 
         else:
             raise UploadRemoteDatasetCheckError('No dataset specified.')
 
-    def _perform_upload(self):
-        self._started = datetime.now()
-        file_size = self._file_path.stat().st_size
-        self._logger.info(f'{self.log_prefix} Starting upload to Arcsecond ({file_size} bytes)')
-
+    def __get_upload_data(self):
         e = MultipartEncoder(
             fields={'dataset': self._context.dataset_uuid,
                     'file': (self._file_path.name, open(self._file_path, 'rb'))}
         )
 
         def percent_printer(monitor):
             bar_length = 40
             self.__bytes_read = monitor.bytes_read
-            fraction = min(float(monitor.bytes_read) / float(file_size), 1.0)
+            fraction = min(float(monitor.bytes_read) / float(self._file_size), 1.0)
             hashes = '#' * int(round(fraction * bar_length))
             spaces = ' ' * (bar_length - len(hashes))
             print(f'[{hashes}{spaces}] {(fraction * 100):.1f}%', end='\r')
 
         m = MultipartEncoderMonitor(e, percent_printer)
 
-        self._datafile, error = self._api.datafiles.create(data=m, headers={"Content-Type": m.content_type})
-        if error:
-            self._status = [Status.ERROR, Substatus.ERROR, None]
-            raise UploadRemoteFileCheckError(str(error))
+        return m
+
+    def _perform_upload(self):
+        self._logger.info(f'{self.log_prefix} Start uploading...')
+        self._status = [Status.UPLOADING, Substatus.UPLOADING, None]
 
-        ended = datetime.now()
-        duration = (ended - self._started).total_seconds()
-        self._logger.info(f'{self.log_prefix} Uploaded finished in {duration} seconds.')
+        self._started = datetime.now()
+        self._logger.info(f'{self.log_prefix} Starting upload to Arcsecond ({self._file_size} bytes)')
+
+        data = self.__get_upload_data()
+        self._datafile, error = self._api.datafiles.create(data=data, headers={"Content-Type": data.content_type})
+        if not error:
+            seconds = (datetime.now() - self._started).total_seconds()
+            self._logger.info(f'{self.log_prefix} Upload duration is {seconds} seconds.')
+            return
+
+        if 'already exists in dataset' in str(error):  # VERY WEAK!!! But solution with HTTP 409 isn't nice either.
+            self._status = [Status.SKIPPED, Substatus.ALREADY_SYNCED, None]
+        else:
+            self._status = [Status.ERROR, Substatus.ERROR, None]
+            raise UploadRemoteFileError(f"{str(error.status)} - {str(error)}")
 
     def _update_tags(self):
+        self._logger.info(f'{self.log_prefix} Updating file tags....')
+        self._status = [Status.FINISHING, Substatus.TAGGING, None]
+
         tag_root = f'oort|root|{str(self._root_path)}'
         tag_origin = f'oort|origin|{socket.gethostname()}'
         tag_uploader = f'oort|uploader|{self._context.config.username}'
         tag_oort = f'oort|version|{__version__}'
 
         # Tags being a list, they cannot be part of the MultipartEncoder.fields because they will
         # be interpreted as a file field tuple/list.
         tags = [tag_root, tag_origin, tag_uploader, tag_oort]
         response, error = self._api.datafiles.update(self._datafile.get('pk'), json={'tags': tags})
         if error:
             self._status = [Status.ERROR, Substatus.ERROR, None]
-            raise UploadRemoteFileCheckError(str(error))
+            raise UploadRemoteFileTagsError(str(error))
+        else:
+            self._status = [Status.OK, Substatus.DONE, None]
 
     def upload_file(self):
-        self._status = [Status.PREPARING, Substatus.CHECKING, None]
-        self._logger.info(f'{self.log_prefix} Preparing Dataset...')
-        self._prepare_dataset()
-        self._logger.info(f'{self.log_prefix} Dataset preparation done.')
-
-        self._status = [Status.UPLOADING, Substatus.UPLOADING, None]
         self._logger.info(f'{self.log_prefix} Opening upload sequence.')
+        self._prepare_dataset()
         self._perform_upload()
+        if self._status[0] == Status.SKIPPED:
+            self._logger.info(f'{self.log_prefix} Upload skipped.')
+        else:
+            self._logger.info(f'{self.log_prefix} Upload done.')
+            self._update_tags()
         self._logger.info(f'{self.log_prefix} Closing upload sequence.')
-
-        self._status = [Status.FINISHING, Substatus.TAGGING, None]
-        self._logger.info(f'{self.log_prefix} Updating file tags....')
-        self._update_tags()
-
-        self._status = [Status.OK, Substatus.DONE, None]
         return self._status
```

### Comparing `arcsecond-3.0.3/arcsecond/uploader/utils.py` & `arcsecond-3.1.0/arcsecond/uploader/utils.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/arcsecond/uploader/walker.py` & `arcsecond-3.1.0/arcsecond/uploader/walker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import time
+from collections import Counter
 from pathlib import Path
 
 import click
 
 from .constants import Status
 from .context import Context
 from .logger import get_oort_logger
 from .uploader import FileUploader
 from .utils import is_file_hidden
 
 
+def __get_duplicates(values):
+    dups = Counter(values) - Counter(set(values))
+    return list(dups.keys())
+
+
 def __walk_first_pass(context: Context, root_path: Path):
     logger = get_oort_logger()
     log_prefix = '[Walker - 1/2]'
     logger.info(f"{log_prefix} Making a first pass to collect info on files...")
     if context.config.api_name != 'dev':
         # For user experience, and let him/her read the above message.
         time.sleep(3)
@@ -24,72 +30,84 @@
     file_paths = []
     for file_path in root_path.glob('**/*'):
         # Skipping both hidden files and hidden directories.
         if is_file_hidden(file_path) or not file_path.is_file():
             continue
 
         index += 1
-        click.echo(f"\n{log_prefix} File {index} / {total_file_count} ({index / total_file_count * 100:.2f}%)")
+        msg = f"{log_prefix} File {index} / {total_file_count} ({index / total_file_count * 100:.2f}%) "
+        msg += f"{file_path.name}"
+        click.echo(msg)
         file_paths.append(file_path)
 
     logger.info(f"{log_prefix} Finished collecting file info inside folder {str(root_path)}.")
     return file_paths
 
 
 def __walk_second_pass(context: Context, root_path: Path, file_paths: list):
     logger = get_oort_logger()
     log_prefix = '[Walker - 2/2]'
     logger.info(f"{log_prefix} Starting second pass to upload files...")
     if context.config.api_name != 'dev':
         time.sleep(3)
 
-    failed_uploads = []
-    success_uploads = []
+    uploads = {'succeeded': [], 'skipped': [], 'failed': []}
     total_file_count = len(file_paths)
 
     index = 0
     for file_path in file_paths:
         index += 1
         click.echo(f"\n{log_prefix} File {index} / {total_file_count} ({index / total_file_count * 100:.2f}%)\n")
 
         uploader = FileUploader(context, root_path, file_path, display_progress=True)
         status, substatus, error = uploader.upload_file()
         if status == Status.OK:
-            success_uploads.append(str(file_path))
+            uploads['succeeded'].append(str(file_path))
+        elif status == Status.SKIPPED:
+            uploads['skipped'].append((str(file_path), substatus, error))
         else:
-            failed_uploads.append((str(file_path), substatus, error))
+            uploads['failed'].append((str(file_path), substatus, error))
 
     msg = f"{log_prefix}\n\nFinished upload walk inside folder {root_path} "
     logger.info(msg)
 
-    return success_uploads, failed_uploads
+    return uploads
 
 
 def walk(context: Context, folder_string: str):
     logger = get_oort_logger()
     log_prefix = '[Walker]'
     root_path = Path(folder_string).resolve()
     if root_path.is_file():  # Just in case we pass a file...
         root_path = root_path.parent
 
-    logger.info(f"{log_prefix} Starting upload walk through {root_path} and its subfolders...")
+    logger.info(f"{log_prefix} Starting to walk through {root_path} and its subfolders...")
 
     file_paths = __walk_first_pass(context, root_path)
-    if len(file_paths) > 0:
-        success_uploads, failed_uploads = __walk_second_pass(context, root_path, file_paths)
-        msg = f"{log_prefix} {len(success_uploads)} successful uploads and {len(failed_uploads)} failed.\n\n"
+    if len(file_paths) == 0:
+        msg = f"{log_prefix} No file paths to upload. Exiting.\n\n"
         logger.info(msg)
+        return
 
-        if len(failed_uploads) > 0:
-            logger.error(f'{log_prefix} Here are the failed uploads:')
-            for path, substatus, error in failed_uploads:
-                logger.error(f'{path} ({substatus}) {error}')
-    else:
-        msg = f"{log_prefix} No new file paths to upload.\n\n"
-        logger.info(msg)
+    all_local_filenames = [path.name for path in file_paths]
+    duplicates = __get_duplicates(all_local_filenames)
+    if len(duplicates) > 0:
+        msg = f"{log_prefix} The following files have duplicate names (not allowed in the same dataset): "
+        msg += f"{', '.join(duplicates)}"
+        logger.error(msg)
+        logger.error(f"Exiting.")
+        return
+
+    uploads = __walk_second_pass(context, root_path, file_paths)
+    msg = f"{log_prefix} uploads succeeded: {len(uploads['succeeded'])}, "
+    msg += f"skipped: {len(uploads['skipped'])}, failed:{len(uploads['failed'])} failed.\n"
+    logger.info(msg)
 
-# if __name__ == '__main__':
-#     root_path = sys.argv[1]
-#     username, upload_key, subdomain, role, telescope, debug_str = sys.argv[2].split(",")
-#     debug = (debug_str == 'True')
-#     identity = Identity(username, upload_key, subdomain, role, telescope, debug)
-#     walk(root_path, identity, debug)
+    if len(uploads['skipped']) > 0:
+        logger.error(f'{log_prefix} Here are the skipped uploads:')
+        for path, substatus, error in uploads['skipped']:
+            logger.warning(f'{path} ({substatus})')
+
+    if len(uploads['failed']) > 0:
+        logger.error(f'{log_prefix} Here are the failed uploads:')
+        for path, substatus, error in uploads['failed']:
+            logger.error(f'{path} ({substatus}) {error}')
```

### Comparing `arcsecond-3.0.3/arcsecond.egg-info/PKG-INFO` & `arcsecond-3.1.0/arcsecond.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcsecond
-Version: 3.0.3
+Version: 3.1.0
 Summary:  CLI for arcsecond.io
 Home-page: https://github.com/arcsecond-io/cli
 Author: Cedric Foellmi
 Author-email: cedric@arcsecond.io
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arcsecond-3.0.3/arcsecond.egg-info/SOURCES.txt` & `arcsecond-3.1.0/arcsecond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/setup.py` & `arcsecond-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/tests/cli/test_cli_options.py` & `arcsecond-3.1.0/tests/cli/test_cli_options.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/tests/cli/test_config.py` & `arcsecond-3.1.0/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/tests/module/test_arcsecond_root.py` & `arcsecond-3.1.0/tests/module/test_arcsecond_root.py`

 * *Files identical despite different names*

### Comparing `arcsecond-3.0.3/tests/module/test_login.py` & `arcsecond-3.1.0/tests/module/test_login.py`

 * *Files identical despite different names*

