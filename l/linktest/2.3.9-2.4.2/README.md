# Comparing `tmp/linktest-2.3.9.tar.gz` & `tmp/linktest-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.3.9.tar", last modified: Thu Apr 11 08:18:30 2024, max compression
+gzip compressed data, was "linktest-2.4.2.tar", last modified: Fri Apr 12 14:38:50 2024, max compression
```

## Comparing `linktest-2.3.9.tar` & `linktest-2.4.2.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.535325 linktest-2.3.9/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-11 08:18:30.534953 linktest-2.3.9/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.532401 linktest-2.3.9/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-11 08:12:00.000000 linktest-2.3.9/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15820 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33851 2024-04-11 08:08:56.000000 linktest-2.3.9/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-10 09:42:36.000000 linktest-2.3.9/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104520 2024-04-11 07:37:54.000000 linktest-2.3.9/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7733 2024-04-11 08:10:09.000000 linktest-2.3.9/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-11 08:12:10.000000 linktest-2.3.9/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10727 2024-04-11 08:11:02.000000 linktest-2.3.9/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-09 14:22:43.000000 linktest-2.3.9/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-11 08:18:30.534533 linktest-2.3.9/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1241 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-11 08:18:30.000000 linktest-2.3.9/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-11 08:18:30.535388 linktest-2.3.9/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-11 08:18:24.000000 linktest-2.3.9/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.549996 linktest-2.4.2/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-12 14:38:50.549702 linktest-2.4.2/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.545276 linktest-2.4.2/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-12 14:34:03.000000 linktest-2.4.2/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-12 14:31:48.000000 linktest-2.4.2/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15915 2024-04-12 14:31:42.000000 linktest-2.4.2/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3825 2024-04-12 13:57:12.000000 linktest-2.4.2/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37292 2024-04-12 14:18:40.000000 linktest-2.4.2/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10265 2024-04-09 02:55:29.000000 linktest-2.4.2/linktest/logged_requests copy.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104608 2024-04-12 14:31:34.000000 linktest-2.4.2/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7937 2024-04-12 10:48:42.000000 linktest-2.4.2/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-12 14:34:03.000000 linktest-2.4.2/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-12 14:31:12.000000 linktest-2.4.2/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11563 2024-04-12 02:12:43.000000 linktest-2.4.2/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.549418 linktest-2.4.2/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1304 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-12 14:38:50.550092 linktest-2.4.2/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-12 14:38:44.000000 linktest-2.4.2/setup.py
```

### Comparing `linktest-2.3.9/linktest/appium_utils.py` & `linktest-2.4.2/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/auto_generate_testcase_list.py` & `linktest-2.4.2/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.4.2/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/base_testcase.py` & `linktest-2.4.2/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/clean_data.py` & `linktest-2.4.2/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/conver_xml_into_db.py` & `linktest-2.4.2/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/database_helper.py` & `linktest-2.4.2/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/date_utilities.py` & `linktest-2.4.2/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/doctor.py` & `linktest-2.4.2/linktest/doctor.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 #  16.customized_android_capabilities
 #  17.android_implicitly_wait
 #  18.DEVICE_ID_NAME_DICT
 #  19.ANDROID_TESTCASE_ACCOUNT
 #  20.# SaveScreenshotForPassedTestCaseFlag
 #  21. Configuration for Browser option ( update follow your business)
 #  22. generate_xunit_result (default value is False)
+#  23. auto_download_chromedriver (default value is False)
 
 import logging
 
 # ------ testcase's log setting ------
 - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
 - LOG_LEVEL = logging.DEBUG # default value is DEBUG
 - LOG_TO_FILE = True # default value is True
@@ -79,14 +80,16 @@
 
 # SaveScreenshotForPassedTestCaseFlag default value if False
 SaveScreenshotForPassedTestCaseFlag = False
 
 # set the webdriver's implicitly_wait default value: 60
 implicitly_wait = 60
 
+auto_download_chromedriver = False
+
 # configure for Database
 if ENVIRONMENT == Environment.UAT:
     DATABASE = {
         "Server": "uat-server",
         "User": "uat-user",
         "Password": "uat-password"
     }
```

### Comparing `linktest-2.3.9/linktest/framework_log.py` & `linktest-2.4.2/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/get_adb_devices.py` & `linktest-2.4.2/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/get_ios_devices_list.py` & `linktest-2.4.2/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/get_platform_info.py` & `linktest-2.4.2/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/get_project_info.py` & `linktest-2.4.2/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/html_report.py` & `linktest-2.4.2/linktest/html_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,27 @@
                 a:hover{
                     text-decoration:underline;
                     background-color:#8E8E8E;
                 }
             </style>
             """
 
+            collapsible_js = """
+            <script>
+                function toggleVisibility(id) {
+                    var element = document.getElementById(id);
+                    if (element.style.display === 'block' || element.style.display === '') {
+                        element.style.display = 'none';
+                    } else {
+                        element.style.removeProperty('display');
+                    }
+                }
+            </script>
+            """
+
             # java script code for filter function
             java_script_code_for_filter = """
             <script type="text/javascript">
 
                 function changeTag(){
                     var my_select = document.getElementById("testcase_tag");
                     if (my_select.value == "tests"){
@@ -168,14 +181,16 @@
                         document.getElementById("num_pass").innerHTML=num_passed_case;
                     }
                 }
 
             </script>
             """
 
+            java_script_code_for_filter += collapsible_js
+
             java_script_copy_failed_testcases = """
             <script>
                 function copyFailedTestCase(){
                     document.getElementById("failed_testcase_names").style.display="none";
                     
                     document.getElementById("copy_status_info").innerHTML = "<font color=#DC3912>Copied</font>";
                     
@@ -200,14 +215,19 @@
                 
                 <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
                 <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa" crossorigin="anonymous"></script>
                 <script type="text/javascript" src="https://cdn.jsdelivr.net/clipboard.js/1.5.12/clipboard.min.js"></script>
                 <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/echarts@5.0.2/dist/echarts.min.js"></script>
                 
                 <style>
+                .screenshot-img {
+                    width: 100%%; /* Ensure it takes the full width of its parent */
+                    max-width: none; /* Remove any max-width restrictions */
+                }
+    
                 .tooltip-inner {
                   max-width: 280px;
                   color: whitesmoke;
                   text-align: right;
                   text-decoration: none;
                   background-color: darkcyan;
                   border-radius: 4px;
@@ -404,15 +424,19 @@
                         failed_cases_dict[module_name] = tc
                     od = collections.OrderedDict(sorted(failed_cases_dict.items()))
                     for k in od.keys():
                         sorted_failed_cases.append(od[k])
                 else:
                     sorted_failed_cases = failed_cases
 
-                for failed_testcase in sorted_failed_cases:
+                for index, failed_testcase in enumerate(sorted_failed_cases):
+                    screenshot_exists = isinstance(failed_testcase, UITestCase) and getattr(failed_testcase,
+                                                                                            'screenshot', None)
+                    screenshot_id = f"screenshot_{index}"
+
                     module_name = failed_testcase.__module__.replace(".", "_") + os.sep + failed_testcase.__class__.__name__
                     module_name_display = failed_testcase.__module__.replace("tests.", "&#x0009;")
                     module_name_display += os.sep + failed_testcase.__class__.__name__
                     report_file_handler.write(
                         "<tr class='all_failed_case' name=%s>" % failed_testcase.testcase_filter_tag)
 
                     report_file_handler.write(
@@ -421,15 +445,15 @@
                         "<a title='View the description of the test case' href='https://testcenter.linktest.com/testlink/linkto.php?tprojectPrefix=ET&item=testcase&id=ET-%s'><font color='#333'>" % getattr(
                             failed_testcase, "testcase_id", "None"))
                     report_file_handler.write("%s" % ('-' if getattr(
                             failed_testcase, "testcase_id", "None") == None else getattr(failed_testcase, "testcase_id")))
                     report_file_handler.write("</font></a></td>")
 
                     testcase_information = """
-                        <td width='710'style='word-break:break-all'>
+                        <td width='710' style='word-break:break-all'>
                         <a  href='%s'>
                             <font color='#333'>
                                 %s
                             </font>
                         </a>
                         """ % (
                         module_name,
@@ -443,39 +467,49 @@
                             " <a title='%s'> (" % 'Please see the execution logs for more details' + failed_testcase.exception_info + ") </a>")
                     except BaseException:
                         print(traceback.format_exc())
 
                     if failed_testcase.rerun_tag == 0:
                         try:
                             report_file_handler.write(
-                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> Log</font></a>" %
+                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> Text Log</font></a>" %
                                 failed_testcase.log_file_path)
+                            report_file_handler.write(
+                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML Log</font></a>" %
+                                failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                         try:
                             if isinstance(failed_testcase, UITestCase):
-                                if failed_testcase.screenshot_index > 0:
-                                    for index in range(failed_testcase.screenshot_index):
+                                if failed_testcase.linktest_screenshot_index > 0:
+                                    for index in range(failed_testcase.linktest_screenshot_index):
                                         report_file_handler.write(
                                             "<a title='Screenshot%s' href='%s'> <font color='green'> - Screenshot_%s</font> </a>" %
                                             (index + 1, "./" + failed_testcase.__module__.replace(".", "_") +
                                              os.sep + failed_testcase.logger.name + os.sep + failed_testcase.logger.name +
                                              "_" + str(index + 1) + "_screenshot.png", index + 1))
                                 report_file_handler.write(
                                     "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='click to see the Screenshot' href='%s'> <font color='#DC3912'> - Screenshot</font> </a>" %
                                     failed_testcase.screenshot)
+
+                            if screenshot_exists:
+                                report_file_handler.write(
+                                    f" <button onclick='toggleVisibility(\"{screenshot_id}\")'>Toggle Screenshots</button>")
                         except BaseException:
                             print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
                         try:
                             report_file_handler.write(
-                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed ReRun Log' href='%s'> <font color='#DC3912'> | ReRun_Log</font> </a>" %
-                                failed_testcase.log_file_path)
+                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed ReRun Log' href='%s'> <font color='#DC3912'> | Text ReRun_Log</font> </a>" %
+                                failed_testcaselog_file_path)
+                            report_file_handler.write(
+                                "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed ReRun Log' href='%s'> <font color='#DC3912'> | HTML ReRun_Log</font> </a>" %
+                                failed_testcaselog_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                         try:
                             if isinstance(failed_testcase, UITestCase):
                                 report_file_handler.write(
                                     "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='Click to see the ReRun_Screenshot' href='%s'> <font color='#DC3912'> - ReRun_Screenshot</font> </a>" %
@@ -488,14 +522,24 @@
                     report_file_handler.write("<td width='150' align='center' >")
                     report_file_handler.write("<font>")
                     if not hasattr(failed_testcase, "execution_time"):
                         failed_testcase.execution_time = ""
                     report_file_handler.write("%s" % failed_testcase.execution_time)
                     report_file_handler.write("</font>")
                     report_file_handler.write("</td></tr>")
+
+                # Adding the screenshots section
+                if screenshot_exists:
+                    report_file_handler.write(f"<tr id='screenshot_0' style='display: none;'>")
+                    report_file_handler.write(f"<td width='125' align='center' style='word-break:break-all;no-wrap:no-wrap'>TestName_1_Screenshot</td>")
+                    report_file_handler.write(f"<td width='710' align='center' style='word-break:break-all;no-wrap:no-wrap'>")
+                    report_file_handler.write(
+                        f"<img src='{failed_testcase.screenshot}' alt='Screenshot' style='width:100%; height:auto;'>")
+                    report_file_handler.write("</td><td></td></tr>")
+
                 report_file_handler.write("</table></td></tr></table>")
 
             if len(passed_cases) > 0:
                 passed_testcase_table = """
                 <table align='center'>
                 <tr><td>
 
@@ -552,23 +596,26 @@
                         report_file_handler.write("<font color='orange'> -- Miss Attribute</font>")
 
                     report_file_handler.write("</font>")
                     report_file_handler.write("</font></a>")
 
                     try:
                         report_file_handler.write(
-                            "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp;&nbsp;Log</font> </a>" %
+                            "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp;&nbsp; Text Log</font> </a>" %
                             passed_testcase.log_file_path)
+                        report_file_handler.write(
+                            "<a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp;&nbsp; HTML Log</font> </a>" %
+                            passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if isinstance(passed_testcase, UITestCase):
-                            if getattr(passed_testcase, 'screenshot_index', 0):
-                                for index in range(passed_testcase.screenshot_index):
+                            if getattr(passed_testcase, 'linktest_screenshot_index', 0):
+                                for index in range(passed_testcase.linktest_screenshot_index):
                                     report_file_handler.write(
                                         "<a title='Screenshot%s' href='%s'> <font color='green'> - Screenshot_%s</font> </a>" %
                                         (index + 1, "./" + passed_testcase.__module__.replace(".", "_") +
                                          os.sep + passed_testcase.logger.name + os.sep + passed_testcase.logger.name +
                                          "_" + str(index+1) + "_screenshot.png", index + 1))
                             report_file_handler.write(
                                 "<a title='Screenshot' href='%s'> <font color='green'> - Screenshot</font> </a>" %
@@ -576,16 +623,19 @@
                     except BaseException:
                         traceback.print_exc()
                         print(traceback.format_exc())
 
                     try:
                         if passed_testcase.rerun_tag == 1:
                             report_file_handler.write(
-                                "<a title='ReRun_Log' href='%s'> <font color='green'> | ReRun_Log</font> </a>" %
+                                "<a title='ReRun_Log' href='%s'> <font color='green'> | Text ReRun_Log</font> </a>" %
                                 passed_testcase.log_file_path)
+                            report_file_handler.write(
+                                "<a title='ReRun_Log' href='%s'> <font color='green'> | HTML ReRun_Log</font> </a>" %
+                                passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if isinstance(passed_testcase, UITestCase):
                             if passed_testcase.rerun_tag == 1:
                                 report_file_handler.write(
```

### Comparing `linktest-2.3.9/linktest/logged_requests.py` & `linktest-2.4.2/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/main.py` & `linktest-2.4.2/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
     - DEBUG_RUN (keeps the browser active after execution is done; default value is False)
     - Show_All_Chrome_Driver_Logs (determines whether to show all webdriver logs; default value is False)
     - QUEUE_SIZE (setting queue_size to 8, for example, means that a maximum of 8 test cases can be executed concurrently)
     - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard)
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
     - auto_log_request (default value is True; automatically logs request actions)
+    - auto_download_chromedriver (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
 
     # ------ Configuration Related to the TestCase's Log ------
     - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
     - LOG_LEVEL = logging.DEBUG # default value is DEBUG
     - LOG_TO_FILE = True # default value is True
     - LOG_TO_CONSOLE = True # default value is True
 
@@ -432,14 +433,15 @@
     from . import doctor
 
     doctor.doctor_check()
 except BaseException:
     traceback.print_exc()
 
 from . import html_report
+from . import generate_html_log
 from . import run_testcase_thread
 from . import timeout_thread
 from . import testcase_timeout_exception
 from . import auto_generate_testcase_list_from_csv
 from . import auto_generate_testcase_list
 from . import xml_report
 from . import doctor
@@ -683,18 +685,14 @@
                     executing_testcase.logger = logger_rerun
                     executing_testcase.requests = LoggedRequests(logger_rerun)
 
 
                     executing_testcase.logfile_full_name = logfile_full_name_rerun
                     executing_testcase.log_file_path = logfile_full_name_rerun.replace(project_info.output_folder, ".")
 
-                executing_testcase.logger.info(
-                    "======== Execution Log for TestCase: {TestCaseName} ========".format(
-                        TestCaseName=testcase.__name__) + os.linesep)
-
                 executing_testcase.logger.info("- Test Host Operating System: %s" % PLATFORM_INFO + os.linesep)
                 executing_testcase.logger.info(
                     "- Test Execution Environment: %s " % settings.ENVIRONMENT.upper() + os.linesep)
 
                 # if IOS testcase run then should start appium first
                 if issubclass(testcase, ios_testcase.IOSTestCase) or issubclass(testcase,
                                                                                 android_testcase.AndroidTestCase):
@@ -926,15 +924,15 @@
 
                 if issubclass(testcase, ui_testcase.UITestCase):
 
                     try:
                         # save the current URL and all the browser's related information when got error.
                         executing_testcase.logger.error(
                             "---------------- Error URL & Browser Info Start --------------" +
-                            testcase.browser.current_url + os.linesep)
+                            executing_testcase.browser.current_url() + os.linesep)
                         executing_testcase.logger.error(testcase.browser.__dict__)
                         executing_testcase.logger.error(
                             "---------------- Error URL & Browser Info End --------------" + os.linesep)
                     except:
                         traceback.print_exc()
 
                 executing_testcase.logger.error(traceback_info)
@@ -1180,14 +1178,15 @@
                                                 webdriver.quit()
                                     elif isinstance(webdriver, WebDriver):
                                         if close_browser_after_done_flag:
                                             webdriver.delete_all_cookies()
                                             webdriver.quit()
                                 except BaseException:
                                     traceback.print_exc()
+                                
 
                         if issubclass(testcase, ios_testcase.IOSTestCase):
                             # set executing_ios_testcase_flag as False after this ios testcase execution done
                             TestCaseExecutor.executing_ios_testcase_flag = False  # todo
                             kill_process_by_name("Simulator")
 
                         if issubclass(testcase, android_testcase.AndroidTestCase):
@@ -1204,14 +1203,16 @@
                             setattr(TestCaseExecutor, device_name, False)
 
                         if getattr(settings, 'LOG_TO_FILE', False):
                             with open(executing_testcase.logfile_full_name, "r", encoding="utf-8", errors="ignore") as logfile_full_name:
                                 execution_log = logfile_full_name.read()
                                 executing_testcase.execution_log = execution_log
                     finally:
+                        generate_html_log.generate_html_log(executing_testcase)
+
                         if os.sep + "jenkins" + os.sep + "workspace" + os.sep in project_info.project_path:
                             TestCaseExecutor.jenkins_job_name = \
                                 project_info.project_path.split(os.sep + "jenkins" + os.sep + "workspace" + os.sep)[
                                     1].split(os.sep)[0]
 
                 try:
                     print(" - (Passed:%s | Failed:%s | Remaining:%s | Total:%s) - Testcase execution for '%s' has completed." % (
```

### Comparing `linktest-2.3.9/linktest/memory_usage.py` & `linktest-2.4.2/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/re_func.py` & `linktest-2.4.2/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/run.py` & `linktest-2.4.2/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/run_testcase_thread.py` & `linktest-2.4.2/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/scp_report_to_specified_path.py` & `linktest-2.4.2/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/selenium_helper.py` & `linktest-2.4.2/linktest/selenium_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,22 @@
     if hasattr(settings, "run_by_github_action") and settings.run_by_github_action is True:
         pass
     else:
         # Check if the current version of chromedriver exists
         # and if it doesn't exist, download it automatically,
         # then add chromedriver to path
 
-        import chromedriver_autoinstaller
-        chromedriver_autoinstaller.install()
+        try:
+            from settings import auto_download_chromedriver
+        except ImportError:
+            auto_download_chromedriver = False
+
+        if auto_download_chromedriver is True:
+            import chromedriver_autoinstaller
+            chromedriver_autoinstaller.install()
 except BaseException:
     traceback.print_exc()
 
 
 from . import get_project_info
```

### Comparing `linktest-2.3.9/linktest/timeout_thread.py` & `linktest-2.4.2/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/ui_testcase.py` & `linktest-2.4.2/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/update_config.py` & `linktest-2.4.2/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest/webdriver_wrapper.py` & `linktest-2.4.2/linktest/webdriver_wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,31 +71,31 @@
         self.logger.info(msg)
 
     def send_keys(self, *value):
         self._log_action("send_keys", *value)
         self.element.send_keys(*value)
 
     def click(self):
-        self._log_action("click")
+        self.logger.info(f"- WebElementWrapper Action: 'click'")
         self.element.click()
 
     def clear(self):
-        self._log_action("clear")
+        self.logger.info(f"- WebElementWrapper Action: 'clear'")
         self.element.clear()
 
     def tag_name(self) -> str:
-        self._log_action("tag_name")
+        self.logger.info(f"- WebElementWrapper Action: 'tag_name'")
         return self.element.tag_name
 
     def submit(self):
-        self._log_action("submit")
+        self.logger.info(f"- WebElementWrapper Action: 'submit'")
         self.element.submit()
 
     def text(self) -> str:
-        self._log_action("text")
+        self.logger.info(f"- WebElementWrapper Action: 'text'")
         return self.element.text
 
     def get_property(self, name) -> Union[str, bool, WebElement, dict]:
         self._log_action("get_property", name)
         return self.element.get_property(name)
 
     def get_dom_attribute(self, name) -> str:
@@ -103,43 +103,43 @@
         return self.element.get_attribute(name)
 
     def get_attribute(self, name) -> Union[str, None]:
         self._log_action("get_attribute", name)
         return self.element.get_attribute(name)
 
     def is_selected(self) -> bool:
-        self._log_action("is_selected")
+        self.logger.info(f"- WebElementWrapper Action: 'is_selected'")
         return self.element.is_selected()
 
     def is_enabled(self) -> bool:
-        self._log_action("is_enabled")
+        self.logger.info(f"- WebElementWrapper Action: 'is_enabled'")
         return self.element.is_enabled()
 
     def is_displayed(self) -> bool:
-        self._log_action("is_displayed")
+        self.logger.info(f"- WebElementWrapper Action: 'is_displayed'")
         return self.element.is_displayed()
 
     def location_once_scrolled_into_view(self) -> dict:
         self._log_action("location_once_scrolled_into_view")
         return self.element.location_once_scrolled_into_view
 
     def size(self) -> dict:
-        self._log_action("size")
+        self.logger.info(f"- WebElementWrapper Action: 'size'")
         return self.element.size
 
     def value_of_css_property(self, property_name) -> str:
         self._log_action("value_of_css_property", property_name)
         return self.element.value_of_css_property(property_name)
 
     def location(self) -> dict:
-        self._log_action("location")
+        self.logger.info(f"- WebElementWrapper Action: 'location'")
         return self.element.location
 
     def rect(self) -> dict:
-        self._log_action("rect")
+        self.logger.info(f"- WebElementWrapper Action: 'rect'")
         return self.element.rect
 
     def screenshot_as_base64(self) -> str:
         self._log_action("screenshot_as_base64")
         return self.element.screenshot_as_base64
 
     def screenshot_as_png(self) -> bytes:
@@ -147,19 +147,19 @@
         return self.element.screenshot_as_png
 
     def screenshot(self, filename) -> bool:
         self._log_action("screenshot", filename)
         return self.element.screenshot(filename)
 
     def parent(self):
-        self._log_action("parent")
+        self.logger.info(f"- WebElementWrapper Action: 'parent'")
         return self.element.parent
 
     def id(self) -> str:
-        self._log_action("id")
+        self.logger.info(f"- WebElementWrapper Action: 'id'")
         return self.element.id
 
     def find_element(self, by=By.ID, value=None) -> WebElement:
         self._log_action("find_element", by, value)
         return self.element.find_element(by, value)
 
     def find_elements(self, by=By.ID, value=None) -> List[WebElement]:
@@ -205,95 +205,95 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         self._log_action("execute_async_script", script, *args)
         return super().execute_async_script(script, *args)
 
     def title(self) -> str:
-        self._log_action("title")
+        self.logger.info(f"- WebDriver Action: 'title'")
         return super().title
 
     # def create_web_element(self, element_id: str) -> WebElement:
     #     self._log_action("create_web_element", element_id)
     #     return super().create_web_element(element_id)
 
     def start_session(self, capabilities: dict) -> None:
         self._log_action("start_session", capabilities)
         super().start_session(capabilities)
 
     def current_url(self) -> str:
-        self._log_action("current_url")
+        self.logger.info(f"- WebDriver Action: 'current_url'")
         return super().current_url
 
     def page_source(self) -> str:
-        self._log_action("page_source")
+        self.logger.info(f"- WebDriver Action: 'page_source'")
         return super().page_source
 
     def close(self) -> None:
-        self._log_action("close")
+        self.logger.info(f"- WebDriver Action: 'close'")
         super().close()
 
     def quit(self) -> None:
-        self._log_action("quit")
+        self.logger.info(f"- WebDriver Action: 'quit'")
         super().quit()
 
     def current_window_handle(self) -> str:
-        self._log_action("current_window_handle")
+        self.logger.info(f"- WebDriver Action: 'current_window_handle'")
         return super().current_window_handle
 
     def window_handles(self) -> List[str]:
         self._log_action("window_handles")
         return super().window_handles
 
     def maximize_window(self) -> None:
-        self._log_action("maximize_window")
+        self.logger.info(f"- WebDriver Action: 'maximize_window'")
         super().maximize_window()
 
     def fullscreen_window(self) -> None:
-        self._log_action("fullscreen_window")
+        self.logger.info(f"- WebDriver Action: 'fullscreen_window'")
         super().fullscreen_window()
 
     def minimize_window(self) -> None:
-        self._log_action("minimize_window")
+        self.logger.info(f"- WebDriver Action: 'minimize_window'")
         super().minimize_window()
 
     def get_cookie(self, name) -> typing.Optional[typing.Dict]:
         self._log_action("get_cookie", name)
         return super().get_cookie(name)
 
     def refresh(self) -> None:
-        self._log_action("refresh")
+        self.logger.info(f"- WebDriver Action: 'refresh'")
         super().refresh()
 
     def forward(self) -> None:
-        self._log_action("forward")
+        self.logger.info(f"- WebDriver Action: 'forward'")
         super().forward()
 
     def back(self) -> None:
-        self._log_action("back")
+        self.logger.info(f"- WebDriver Action: 'back'")
         super().back()
 
     def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
         self._log_action("print_page", print_options)
         return super().print_page(print_options)
 
     def get_cookies(self) -> List[dict]:
-        self._log_action("get_cookies")
+        self.logger.info(f"- WebDriver Action: 'get_cookies'")
         return super().get_cookies()
 
     def add_cookie(self, cookie_dict) -> None:
         self._log_action("add_cookie", cookie_dict)
         super().add_cookie(cookie_dict)
 
     def delete_cookie(self, name) -> None:
         self._log_action("delete_cookie", name)
         super().delete_cookie(name)
 
     def delete_all_cookies(self) -> None:
-        self._log_action("delete_all_cookies")
+        self.logger.info(f"- WebDriver Action: 'delete_all_cookies'")
         super().delete_all_cookies()
 
     def implicitly_wait(self, time_to_wait: float) -> None:
         self._log_action("implicitly_wait", time_to_wait)
         super().implicitly_wait(time_to_wait)
 
     def set_script_timeout(self, time_to_wait: float) -> None:
@@ -302,18 +302,18 @@
 
     def set_page_load_timeout(self, time_to_wait: float) -> None:
         self._log_action("set_page_load_timeout", time_to_wait)
         super().set_page_load_timeout(time_to_wait)
 
     def save_screenshot(self, filename=None) -> bool:
         if filename is None:
-            if not getattr(self.ui_testcase, 'screenshot_index', False):
-                setattr(self.ui_testcase, 'screenshot_index', 1)
+            if not getattr(self.ui_testcase, 'linktest_screenshot_index', False):
+                setattr(self.ui_testcase, 'linktest_screenshot_index', 1)
             else:
-                self.ui_testcase.screenshot_index += 1
+                self.ui_testcase.linktest_screenshot_index += 1
 
-            filename = self.ui_testcase.full_tc_folder + os.sep + self.logger.name + "_" + str(self.ui_testcase.screenshot_index) + "_screenshot.png"
-
-        self._log_action("save_screenshot", filename)
+            filename = self.ui_testcase.full_tc_folder + os.sep + self.logger.name + "_" + str(self.ui_testcase.linktest_screenshot_index) + "_screenshot.png"
+            self.logger.info("linktest_screenshot_filename: " + filename)
+        # self._log_action("save_screenshot", filename)
         return super().save_screenshot(filename)
 
     # todo 可以继续在此处添加其他 WebDriver 方法的日志记录功能
```

### Comparing `linktest-2.3.9/linktest/xml_report.py` & `linktest-2.4.2/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.3.9/linktest.egg-info/SOURCES.txt` & `linktest-2.4.2/linktest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 linktest/clean_data.py
 linktest/conver_xml_into_db.py
 linktest/database_helper.py
 linktest/date_utilities.py
 linktest/detect_delimiter.py
 linktest/doctor.py
 linktest/framework_log.py
+linktest/generate_html_log.py
 linktest/get_adb_devices.py
 linktest/get_ios_devices_list.py
 linktest/get_platform_info.py
 linktest/get_project_info.py
 linktest/html_report.py
 linktest/ios_testcase.py
 linktest/linktest_setup.py
+linktest/logged_requests copy.py
 linktest/logged_requests.py
 linktest/main.py
 linktest/memory_usage.py
 linktest/re_func.py
 linktest/run.py
 linktest/run_testcase_thread.py
 linktest/scp_report_to_specified_path.py
```

