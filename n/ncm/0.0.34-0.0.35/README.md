# Comparing `tmp/ncm-0.0.34.tar.gz` & `tmp/ncm-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.34.tar", last modified: Wed Apr 10 19:46:00 2024, max compression
+gzip compressed data, was "ncm-0.0.35.tar", last modified: Fri Apr 12 21:14:26 2024, max compression
```

## Comparing `ncm-0.0.34.tar` & `ncm-0.0.35.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.207752 ncm-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 19:45:46.000000 ncm-0.0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-10 19:46:00.203752 ncm-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-10 19:45:46.000000 ncm-0.0.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.203752 ncm-0.0.34/ncm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:45:46.000000 ncm-0.0.34/ncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148216 2024-04-10 19:45:46.000000 ncm-0.0.34/ncm/ncm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:46:00.203752 ncm-0.0.34/ncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 19:46:00.000000 ncm-0.0.34/ncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:46:00.207752 ncm-0.0.34/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-04-10 19:45:46.000000 ncm-0.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 21:14:14.000000 ncm-0.0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 21:14:25.995735 ncm-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 21:14:14.000000 ncm-0.0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/ncm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:14.000000 ncm-0.0.35/ncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148323 2024-04-12 21:14:14.000000 ncm-0.0.35/ncm/ncm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/ncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:14:25.995735 ncm-0.0.35/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-04-12 21:14:23.000000 ncm-0.0.35/setup.py
```

### Comparing `ncm-0.0.34/LICENSE` & `ncm-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.34/PKG-INFO` & `ncm-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.34
+Version: 0.0.35
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.34/README.md` & `ncm-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.34/ncm/ncm.py` & `ncm-0.0.35/ncm/ncm.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     You can also return the full list of records in a single array without
     the need for paging by passing limit='all':
        n.get_accounts(limit='all')
 
     It also has native support for handling any number of "__in" filters
     beyond Cradlepoint's limit of 100. The script automatically chunks
     the list into groups of 100 and combines the results into a single array
+
 """
 
 from requests import Session
 from requests.adapters import HTTPAdapter
 from http import HTTPStatus
 from urllib3.util.retry import Retry
 from datetime import datetime, timedelta
@@ -151,14 +152,15 @@
                  api_keys=None,
                  log_events=True,
                  logger=None,
                  retries=5,
                  retry_backoff_factor=2,
                  retry_on=None,
                  base_url=None):
+        self.v2 = self # for backwards compatibility
         base_url = base_url or os.environ.get("CP_BASE_URL", "https://www.cradlepointecm.com/api/v2")
         super().__init__(log_events=log_events, logger=logger, retries=retries, retry_backoff_factor=retry_backoff_factor, retry_on=retry_on, base_url=base_url)
         if api_keys:
             if self.__validate_api_keys(api_keys):
                 self.session.headers.update(api_keys)
         self.session.headers.update({
             'Content-Type': 'application/json'
@@ -2117,14 +2119,15 @@
         :param retry_backoff_factor: backoff time multiplier for retries.
           Optional.
         :param retry_on: types of errors on which automatic retry will occur.
           Optional.
         :param base_url: # base url for calls. Configurable for testing.
           Optional.
         """
+        self.v3 = self # For backwards compatibility
         base_url = base_url or os.environ.get("CP_BASE_URL_V3", "https://api.cradlepointecm.com/api/v3")
         super().__init__(log_events, logger, retries, retry_backoff_factor, retry_on, base_url)
         if api_key:
             token = {'Authorization': f'Bearer {api_key}'}
             self.session.headers.update(token)
         self.session.headers.update({
             'Content-Type': 'application/vnd.api+json',
```

### Comparing `ncm-0.0.34/ncm.egg-info/PKG-INFO` & `ncm-0.0.35/ncm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.34
+Version: 0.0.35
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.34/setup.py` & `ncm-0.0.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.34",
+    version="0.0.35",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

