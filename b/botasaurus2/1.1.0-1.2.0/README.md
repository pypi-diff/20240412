# Comparing `tmp/botasaurus2-1.1.0.tar.gz` & `tmp/botasaurus2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.1.0.tar", max compression
+gzip compressed data, was "botasaurus2-1.2.0.tar", max compression
```

## Comparing `botasaurus2-1.1.0.tar` & `botasaurus2-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.1.0/README.md
--rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.1.0/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.1.0/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      834 2024-04-11 20:48:02.907490 botasaurus2-1.1.0/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.1.0/botasaurus/constants.py
--rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    38763 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.1.0/botasaurus/output.py
--rw-r--r--   0        0        0     4720 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.1.0/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.1.0/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.1.0/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.2.0/README.md
+-rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.2.0/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.2.0/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.2.0/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.2.0/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.2.0/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.2.0/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.2.0/botasaurus/constants.py
+-rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.2.0/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.2.0/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    38906 2024-04-12 14:01:48.615321 botasaurus2-1.2.0/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.2.0/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.2.0/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.2.0/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.2.0/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.2.0/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.2.0/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.2.0/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.2.0/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-12 14:06:05.851363 botasaurus2-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.2.0/PKG-INFO
```

### Comparing `botasaurus2-1.1.0/LICENSE` & `botasaurus2-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/README.md` & `botasaurus2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/__init__.py` & `botasaurus2-1.2.0/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/accept_google_cookies.py` & `botasaurus2-1.2.0/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/anti_detect_driver.py` & `botasaurus2-1.2.0/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/anti_detect_requests.py` & `botasaurus2-1.2.0/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/base_data.py` & `botasaurus2-1.2.0/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/beep_utils.py` & `botasaurus2-1.2.0/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/botasaurus_storage.py` & `botasaurus2-1.2.0/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/bt.py` & `botasaurus2-1.2.0/botasaurus/bt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .user_generator import generate_user, generate_users, Gender, Country
 from .calc_max_parallel_browsers import calc_max_parallel_browsers, BrowserResourceConfig
 from .creators import create_driver, create_requests
 from .local_storage import LocalStorageClass
 from .opponent import Opponent
 from .output import read_json, write_json, read_temp_json, write_temp_json,  read_csv, write_csv,   read_html,write_html,  read_file,write_file, file_exists,save_image
-from .profile import Profile
+from .profile import ProfileClass
 from .temp_mail import TempMail
 from .user_agent import UserAgent
 from .wait import Wait
 from .window_size import WindowSize
 from .formats import Formats
 from .beep_utils import prompt
 from .utils import remove_nones
 
 # TODO: track where/when calls to _LocalStorage aliased as LocalStorageClass are needed
 # LocalStorage = LocalStorageClass()
+# TODO: track where/when calls to _Profile aliased as ProfileClass are needed
+# Profile = ProfileClass()
```

### Comparing `botasaurus2-1.1.0/botasaurus/cache.py` & `botasaurus2-1.2.0/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.2.0/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/captcha.py` & `botasaurus2-1.2.0/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/check_and_download_driver.py` & `botasaurus2-1.2.0/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/cl.py` & `botasaurus2-1.2.0/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/close.py` & `botasaurus2-1.2.0/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/create_driver_utils.py` & `botasaurus2-1.2.0/botasaurus/create_driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/create_stealth_driver.py` & `botasaurus2-1.2.0/botasaurus/create_stealth_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/creators.py` & `botasaurus2-1.2.0/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/decorator_helpers.py` & `botasaurus2-1.2.0/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/decorators.py` & `botasaurus2-1.2.0/botasaurus/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from .beep_utils import beep_input
 from .decorators_utils import (
     create_directories_if_not_exists,
     create_directory_if_not_exists,
 )
 # from .local_storage import LocalStorage
 from .local_storage import LocalStorageClass
-from .profile import Profile
+from .profile import ProfileClass
 from .usage import Usage
 from .list_utils import flatten
 
 
 class RetryException(Exception):
     pass
 
@@ -432,15 +432,17 @@
             create_error_logs = kwargs.get("create_error_logs", create_error_logs)
 
             raise_exception = kwargs.get("raise_exception", raise_exception)
             create_driver = kwargs.get("create_driver", create_driver)
             capabilities = kwargs.get("capabilities", capabilities)
             local_storage_dir = kwargs.get("local_storage_dir", local_storage_dir)
 
-            LocalStorageClass(local_storage_dir)
+            local_storage = LocalStorageClass(local_storage_dir)
+            profile = ProfileClass(local_storage_dir)
+            Profile = profile  # TODO: alter thourghout this module
             fn_name = func.__name__
 
             if cache:
                 _create_cache_directory_if_not_exists(func)
 
             # # Pool to hold reusable drivers
             _driver_pool = wrapper_browser._driver_pool if keep_drivers_alive else []
```

### Comparing `botasaurus2-1.1.0/botasaurus/download_driver.py` & `botasaurus2-1.2.0/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/get_chrome_version.py` & `botasaurus2-1.2.0/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/got_adapter.py` & `botasaurus2-1.2.0/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/ip_utils.py` & `botasaurus2-1.2.0/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/list_utils.py` & `botasaurus2-1.2.0/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/local_storage.py` & `botasaurus2-1.2.0/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/local_storage_driver.py` & `botasaurus2-1.2.0/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/output.py` & `botasaurus2-1.2.0/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/profile.py` & `botasaurus2-1.2.0/botasaurus/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 import json
 import os
 import random as random_module
+from pathlib import Path
 
 from .utils import datetime_to_str, relative_path, str_to_datetime
 
 class ProfilePyStorageException(Exception):
     pass
 
 class BasicStorageBackend:
@@ -21,19 +22,22 @@
     def remove_item(self, item: str) -> None:
         self.raise_dummy_exception()
 
     def clear(self) -> None:
         self.raise_dummy_exception()
 
 class JSONStorageBackend(BasicStorageBackend):
-    def __init__(self) -> None:
+    def __init__(self, base_dir: str = None) -> None:
+        self.base_dir = base_dir
         self.refresh()
 
     def refresh(self):
         self.json_path = relative_path( "profiles.json", 0)
+        if self.base_dir is not None:
+            self.json_path = self.base_dir / Path("profiles.json")
         self.json_data = {}
 
         if not os.path.isfile(self.json_path):
             self.commit_to_disk()
 
         with open(self.json_path, "r") as json_file:
             self.json_data = json.load(json_file)
@@ -67,16 +71,16 @@
     def clear(self) -> None:
         if os.path.isfile(self.json_path):
             os.remove(self.json_path)
         self.json_data = {}
         self.commit_to_disk()
     
 class _Profile:
-    def __init__(self) -> None:
-        self.storage_backend_instance = JSONStorageBackend()
+    def __init__(self, base_dir: str = None) -> None:
+        self.storage_backend_instance = JSONStorageBackend(base_dir)
 
     profile = None
     def refresh(self) -> None:
         self.storage_backend_instance.refresh()
 
     def check_profile(self) -> None:
         if self.profile is None:
@@ -145,15 +149,19 @@
     def set_profile(self, profile):
         self.check_profile()
         if type(profile) is dict:
             self.storage_backend_instance.set_item(self.profile, profile)
         else: 
             raise Exception("Profile is not a dictionary.")
 
-Profile = _Profile()
+# Profile = _Profile()
+
+
+ProfileClass = _Profile
+
 
 if __name__ == "__main__":
     t = _Profile()
     
     print(t.get_item("a"))
     print(t.set_item("a" ,"ss"))
     print(t.remove_item("a"))
```

### Comparing `botasaurus2-1.1.0/botasaurus/sitemap.py` & `botasaurus2-1.2.0/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/str_utils.py` & `botasaurus2-1.2.0/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/temp_mail.py` & `botasaurus2-1.2.0/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/user_agent.py` & `botasaurus2-1.2.0/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/user_generator.py` & `botasaurus2-1.2.0/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/utils.py` & `botasaurus2-1.2.0/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/botasaurus/window_size.py` & `botasaurus2-1.2.0/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.1.0/pyproject.toml` & `botasaurus2-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.1.0"
+version = "1.2.0"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.1.0/PKG-INFO` & `botasaurus2-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.1.0
+Version: 1.2.0
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.1.0 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.2.0 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

