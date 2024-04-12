# Comparing `tmp/botasaurus2-1.0.0.tar.gz` & `tmp/botasaurus2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.0.0.tar", max compression
+gzip compressed data, was "botasaurus2-1.1.0.tar", max compression
```

## Comparing `botasaurus2-1.0.0.tar` & `botasaurus2-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.0.0/README.md
--rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.0.0/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.0.0/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      703 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.0.0/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.0.0/botasaurus/constants.py
--rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    38391 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.0.0/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3070 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.0.0/botasaurus/output.py
--rw-r--r--   0        0        0     4720 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.0.0/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.0.0/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.0.0/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.0.0/botasaurus/window_size.py
--rw-r--r--   0        0        0      826 2024-04-11 18:18:56.172069 botasaurus2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.1.0/README.md
+-rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.1.0/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57045 2024-03-20 15:48:31.569396 botasaurus2-1.1.0/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      834 2024-04-11 20:48:02.907490 botasaurus2-1.1.0/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.1.0/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.1.0/botasaurus/constants.py
+-rw-r--r--   0        0        0    15195 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    38763 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.1.0/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.1.0/botasaurus/output.py
+-rw-r--r--   0        0        0     4720 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.1.0/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.1.0/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.1.0/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.1.0/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-11 20:48:02.911490 botasaurus2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.1.0/PKG-INFO
```

### Comparing `botasaurus2-1.0.0/LICENSE` & `botasaurus2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/README.md` & `botasaurus2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/__init__.py` & `botasaurus2-1.1.0/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/accept_google_cookies.py` & `botasaurus2-1.1.0/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/anti_detect_driver.py` & `botasaurus2-1.1.0/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/anti_detect_requests.py` & `botasaurus2-1.1.0/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/base_data.py` & `botasaurus2-1.1.0/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/beep_utils.py` & `botasaurus2-1.1.0/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/botasaurus_storage.py` & `botasaurus2-1.1.0/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/bt.py` & `botasaurus2-1.1.0/botasaurus/bt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from .user_generator import generate_user, generate_users, Gender, Country
 from .calc_max_parallel_browsers import calc_max_parallel_browsers, BrowserResourceConfig
 from .creators import create_driver, create_requests
-from .local_storage import LocalStorage
+from .local_storage import LocalStorageClass
 from .opponent import Opponent
 from .output import read_json, write_json, read_temp_json, write_temp_json,  read_csv, write_csv,   read_html,write_html,  read_file,write_file, file_exists,save_image
 from .profile import Profile
 from .temp_mail import TempMail
 from .user_agent import UserAgent
 from .wait import Wait
 from .window_size import WindowSize
 from .formats import Formats
 from .beep_utils import prompt
-from .utils import remove_nones 
+from .utils import remove_nones
+
+# TODO: track where/when calls to _LocalStorage aliased as LocalStorageClass are needed
+# LocalStorage = LocalStorageClass()
```

### Comparing `botasaurus2-1.0.0/botasaurus/cache.py` & `botasaurus2-1.1.0/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.1.0/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/captcha.py` & `botasaurus2-1.1.0/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/check_and_download_driver.py` & `botasaurus2-1.1.0/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/cl.py` & `botasaurus2-1.1.0/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/close.py` & `botasaurus2-1.1.0/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/create_driver_utils.py` & `botasaurus2-1.1.0/botasaurus/create_driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/create_stealth_driver.py` & `botasaurus2-1.1.0/botasaurus/create_stealth_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/creators.py` & `botasaurus2-1.1.0/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/decorator_helpers.py` & `botasaurus2-1.1.0/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/decorators.py` & `botasaurus2-1.1.0/botasaurus/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from threading import Thread
 from traceback import print_exc, format_exc
 from typing import Any, Callable, Optional, Union, List
 import os
 import sys
 from datetime import datetime
 from time import sleep
+from pathlib import Path
 from .exceptions import CloudflareDetection
 
 from .check_and_download_driver import check_and_download_driver
 
 from .utils import is_errors_instance, write_file
 
 from .formats import Formats
@@ -43,15 +44,16 @@
 
 from .anti_detect_driver import AntiDetectDriver
 from .beep_utils import beep_input
 from .decorators_utils import (
     create_directories_if_not_exists,
     create_directory_if_not_exists,
 )
-from .local_storage import LocalStorage
+# from .local_storage import LocalStorage
+from .local_storage import LocalStorageClass
 from .profile import Profile
 from .usage import Usage
 from .list_utils import flatten
 
 
 class RetryException(Exception):
     pass
@@ -335,14 +337,15 @@
     output_formats: Optional[List[str]] = None,
     raise_exception: bool = False,
     must_raise_exceptions: Optional[List[Any]] = None,
     max_retry: Optional[int] = None,
     retry_wait: Optional[int] = None,
     create_error_logs: bool = True,
     create_driver: Optional[Callable] = None,
+    local_storage_dir: Union[str, Path] = None
 ) -> Callable:
     def decorator_browser(func: Callable) -> Callable:
         if not hasattr(func, '_scraper_type'):
             func._scraper_type = "browser"
 
         def close_driver(driver: AntiDetectDriver):
             if tiny_profile:
@@ -393,14 +396,15 @@
 
             nonlocal parallel, data, cache, block_resources, block_images, window_size, metadata, add_arguments, extensions
             nonlocal tiny_profile, is_eager, lang, headless, beep
             nonlocal close_on_crash, async_queue, run_async, profile
             nonlocal proxy, user_agent, reuse_driver, keep_drivers_alive, raise_exception, must_raise_exceptions
 
             nonlocal output, output_formats, max_retry, retry_wait, create_driver, create_error_logs
+            nonlocal capabilities, local_storage_dir
 
             parallel = kwargs.get("parallel", parallel)
             data = kwargs.get("data", data)
             cache = kwargs.get("cache", cache)
             block_images = kwargs.get("block_images", block_images)
             block_resources = kwargs.get("block_resources", block_resources)
             add_arguments = kwargs.get("add_arguments", add_arguments)
@@ -425,15 +429,18 @@
             output_formats = kwargs.get("output_formats", output_formats)
             max_retry = kwargs.get("max_retry", max_retry)
             retry_wait = kwargs.get("retry_wait", retry_wait)
             create_error_logs = kwargs.get("create_error_logs", create_error_logs)
 
             raise_exception = kwargs.get("raise_exception", raise_exception)
             create_driver = kwargs.get("create_driver", create_driver)
+            capabilities = kwargs.get("capabilities", capabilities)
+            local_storage_dir = kwargs.get("local_storage_dir", local_storage_dir)
 
+            LocalStorageClass(local_storage_dir)
             fn_name = func.__name__
 
             if cache:
                 _create_cache_directory_if_not_exists(func)
 
             # # Pool to hold reusable drivers
             _driver_pool = wrapper_browser._driver_pool if keep_drivers_alive else []
```

### Comparing `botasaurus2-1.0.0/botasaurus/download_driver.py` & `botasaurus2-1.1.0/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/get_chrome_version.py` & `botasaurus2-1.1.0/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/got_adapter.py` & `botasaurus2-1.1.0/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/ip_utils.py` & `botasaurus2-1.1.0/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/list_utils.py` & `botasaurus2-1.1.0/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/local_storage.py` & `botasaurus2-1.1.0/botasaurus/local_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import json
+from pathlib import Path
 
 from .utils import relative_path
 
 
 class localStoragePyStorageException(Exception):
     pass
 
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
         self.json_path = relative_path( "local_storage.json", 0)
+        if self.base_dir is not None:
+            self.json_path = self.base_dir / Path("local_storage.json")
         self.json_data = {}
 
         if not os.path.isfile(self.json_path):
             self.commit_to_disk()
 
         with open(self.json_path, "r") as json_file:
             self.json_data = json.load(json_file)
@@ -76,16 +80,16 @@
     def clear(self) -> None:
         if os.path.isfile(self.json_path):
             os.remove(self.json_path)
         self.json_data = {}
         self.commit_to_disk()
     
 class _LocalStorage:
-    def __init__(self) -> None:
-        self.storage_backend_instance = JSONStorageBackend()
+    def __init__(self, base_dir: str = None) -> None:
+        self.storage_backend_instance = JSONStorageBackend(base_dir)
 
     def refresh(self) -> None:
         self.storage_backend_instance.refresh()
     
     def get_item(self, item: str, default = None) -> any:
         return self.storage_backend_instance.get_item(item, default)
 
@@ -101,15 +105,16 @@
     def items(self):
         return self.storage_backend_instance.items()
 
 
     # def get_new_number(self):
     #     return self.storage_backend_instance.get_new_number()
 
-LocalStorage = _LocalStorage()
+# LocalStorage = _LocalStorage()
+LocalStorageClass = _LocalStorage
 
 if __name__ == "__main__":
     t = _LocalStorage()
     
     print(t.get_item("a"))
     print(t.set_item("a" ,"ss"))
     print(t.remove_item("a"))
```

### Comparing `botasaurus2-1.0.0/botasaurus/local_storage_driver.py` & `botasaurus2-1.1.0/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/output.py` & `botasaurus2-1.1.0/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/profile.py` & `botasaurus2-1.1.0/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/sitemap.py` & `botasaurus2-1.1.0/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/str_utils.py` & `botasaurus2-1.1.0/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/temp_mail.py` & `botasaurus2-1.1.0/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/user_agent.py` & `botasaurus2-1.1.0/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/user_generator.py` & `botasaurus2-1.1.0/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/utils.py` & `botasaurus2-1.1.0/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/botasaurus/window_size.py` & `botasaurus2-1.1.0/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.0.0/pyproject.toml` & `botasaurus2-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.0.0"
+version = "1.1.0"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
@@ -23,11 +23,12 @@
 lxml = "^5.1.0"
 aigents = "^0.5.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "^7.0.0"
+ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `botasaurus2-1.0.0/PKG-INFO` & `botasaurus2-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.0.0
+Version: 1.1.0
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
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.0.0 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.1.0 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

