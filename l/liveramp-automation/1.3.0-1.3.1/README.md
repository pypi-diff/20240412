# Comparing `tmp/liveramp_automation-1.3.0.tar.gz` & `tmp/liveramp_automation-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.3.0.tar", last modified: Wed Apr  3 03:15:10 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.1.tar", last modified: Fri Apr 12 01:22:43 2024, max compression
```

## Comparing `liveramp_automation-1.3.0.tar` & `liveramp_automation-1.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.598365 liveramp_automation-1.3.0/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.0/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-04-03 03:15:10.598045 liveramp_automation-1.3.0/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.0/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.582516 liveramp_automation-1.3.0/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.0/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-03 03:14:50.000000 liveramp_automation-1.3.0/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.586190 liveramp_automation-1.3.0/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8133 2024-02-28 01:54:10.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-03 03:14:23.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     9622 2024-03-20 08:56:22.000000 liveramp_automation-1.3.0/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.590503 liveramp_automation-1.3.0/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.0/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.0/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4960 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.0/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.0/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.0/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.0/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.0/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.0/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.597522 liveramp_automation-1.3.0/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2881 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      415 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-03 03:15:10.000000 liveramp_automation-1.3.0/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-03 03:15:10.598416 liveramp_automation-1.3.0/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1413 2024-03-11 02:37:57.000000 liveramp_automation-1.3.0/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.590866 liveramp_automation-1.3.0/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.0/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.593348 liveramp_automation-1.3.0/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.0/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.0/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.0/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.0/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.0/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.0/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-03 03:15:10.596951 liveramp_automation-1.3.0/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.0/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.0/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.0/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.0/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.0/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.086596 liveramp_automation-1.3.1/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.1/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2906 2024-04-12 01:22:43.086268 liveramp_automation-1.3.1/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.1/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.068800 liveramp_automation-1.3.1/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.1/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-12 01:22:24.000000 liveramp_automation-1.3.1/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.072868 liveramp_automation-1.3.1/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8133 2024-02-28 01:54:10.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-03 03:14:23.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     9622 2024-03-20 08:56:22.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.077639 liveramp_automation-1.3.1/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.1/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.1/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4960 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.1/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.1/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.1/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.1/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.1/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.1/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.085735 liveramp_automation-1.3.1/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2906 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      425 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-12 01:22:43.086662 liveramp_automation-1.3.1/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1434 2024-04-12 01:22:13.000000 liveramp_automation-1.3.1/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.078025 liveramp_automation-1.3.1/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.1/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.080515 liveramp_automation-1.3.1/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.1/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.1/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.1/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.1/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.1/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.1/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.085087 liveramp_automation-1.3.1/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.1/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.1/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.1/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.3.0/LICENSE` & `liveramp_automation-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/PKG-INFO` & `liveramp_automation-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.3.0
+Version: 1.3.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
@@ -30,14 +30,15 @@
 Requires-Dist: pytest-json
 Requires-Dist: pytest-json-report
 Requires-Dist: pytest-playwright==0.4.3
 Requires-Dist: pytest-xdist==3.5.0
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: retrying
+Requires-Dist: snowflake
 Requires-Dist: selenium==4.16.0
 
 # liveramp-automation
 an automation framework helps you quickly author scripts for any automation testing
```

### Comparing `liveramp_automation-1.3.0/README.md` & `liveramp_automation-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.1/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.1/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.1/liveramp_automation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.3.0
+Version: 1.3.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
@@ -30,14 +30,15 @@
 Requires-Dist: pytest-json
 Requires-Dist: pytest-json-report
 Requires-Dist: pytest-playwright==0.4.3
 Requires-Dist: pytest-xdist==3.5.0
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: retrying
+Requires-Dist: snowflake
 Requires-Dist: selenium==4.16.0
 
 # liveramp-automation
 an automation framework helps you quickly author scripts for any automation testing
```

### Comparing `liveramp_automation-1.3.0/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.1/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/setup.py` & `liveramp_automation-1.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,10 +44,11 @@
         'pytest-json',
         'pytest-json-report',
         'pytest-playwright==0.4.3',
         'pytest-xdist==3.5.0',
         'PyYAML',
         'requests',
         'retrying',
+        'snowflake',
         'selenium==4.16.0',
     ],
 )
```

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_file.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.1/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_log.py` & `liveramp_automation-1.3.1/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.1/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.1/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.1/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_request.py` & `liveramp_automation-1.3.1/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.1/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.1/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.0/tests/test_utils/test_version.py` & `liveramp_automation-1.3.1/tests/test_utils/test_version.py`

 * *Files identical despite different names*

