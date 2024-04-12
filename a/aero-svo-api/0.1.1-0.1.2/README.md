# Comparing `tmp/aero-svo-api-0.1.1.tar.gz` & `tmp/aero-svo-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aero-svo-api-0.1.1.tar", last modified: Wed Mar 13 09:31:02 2024, max compression
+gzip compressed data, was "aero-svo-api-0.1.2.tar", last modified: Fri Apr 12 14:29:32 2024, max compression
```

## Comparing `aero-svo-api-0.1.1.tar` & `aero-svo-api-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 09:31:02.994559 aero-svo-api-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-12-19 10:48:38.000000 aero-svo-api-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2734 2024-03-13 09:31:02.992557 aero-svo-api-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      727 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/README.md
--rw-rw-rw-   0        0        0      949 2024-03-13 09:24:18.000000 aero-svo-api-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       33 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 09:31:02.994559 aero-svo-api-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-13 09:31:02.959596 aero-svo-api-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 09:31:02.974569 aero-svo-api-0.1.1/src/aero_svo_api/
--rw-rw-rw-   0        0        0       81 2024-03-13 09:24:58.000000 aero-svo-api-0.1.1/src/aero_svo_api/__init__.py
--rw-rw-rw-   0        0        0     2719 2024-03-13 09:00:37.000000 aero-svo-api-0.1.1/src/aero_svo_api/api.py
--rw-rw-rw-   0        0        0     5118 2024-03-13 09:00:37.000000 aero-svo-api-0.1.1/src/aero_svo_api/models.py
--rw-rw-rw-   0        0        0      372 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/src/aero_svo_api/urls.py
--rw-rw-rw-   0        0        0      143 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/src/aero_svo_api/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:31:02.991559 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/
--rw-rw-rw-   0        0        0     2734 2024-03-13 09:31:02.000000 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-03-13 09:31:02.000000 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 09:31:02.000000 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-03-13 09:31:02.000000 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-13 09:31:02.000000 aero-svo-api-0.1.1/src/aero_svo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-13 09:31:02.989575 aero-svo-api-0.1.1/tests/
--rw-rw-rw-   0        0        0     3211 2024-03-13 09:00:37.000000 aero-svo-api-0.1.1/tests/test_api.py
--rw-rw-rw-   0        0        0     1079 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/tests/test_models.py
--rw-rw-rw-   0        0        0      370 2024-03-13 08:31:50.000000 aero-svo-api-0.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.259559 aero-svo-api-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2023-12-19 10:48:38.000000 aero-svo-api-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2734 2024-04-12 14:29:32.257565 aero-svo-api-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/README.md
+-rw-rw-rw-   0        0        0      949 2024-03-13 09:24:18.000000 aero-svo-api-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       33 2024-03-29 11:09:09.000000 aero-svo-api-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:29:32.259559 aero-svo-api-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.213559 aero-svo-api-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.231559 aero-svo-api-0.1.2/src/aero_svo_api/
+-rw-rw-rw-   0        0        0       81 2024-04-12 14:13:15.000000 aero-svo-api-0.1.2/src/aero_svo_api/__init__.py
+-rw-rw-rw-   0        0        0     2719 2024-03-13 09:00:37.000000 aero-svo-api-0.1.2/src/aero_svo_api/api.py
+-rw-rw-rw-   0        0        0     5150 2024-04-12 14:05:36.000000 aero-svo-api-0.1.2/src/aero_svo_api/models.py
+-rw-rw-rw-   0        0        0      372 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/src/aero_svo_api/urls.py
+-rw-rw-rw-   0        0        0      143 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/src/aero_svo_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.256559 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/
+-rw-rw-rw-   0        0        0     2734 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 14:29:32.000000 aero-svo-api-0.1.2/src/aero_svo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 14:29:32.253559 aero-svo-api-0.1.2/tests/
+-rw-rw-rw-   0        0        0     3211 2024-03-13 09:00:37.000000 aero-svo-api-0.1.2/tests/test_api.py
+-rw-rw-rw-   0        0        0     1079 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/tests/test_models.py
+-rw-rw-rw-   0        0        0      370 2024-03-13 08:31:50.000000 aero-svo-api-0.1.2/tests/test_utils.py
```

### Comparing `aero-svo-api-0.1.1/LICENSE` & `aero-svo-api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.1/PKG-INFO` & `aero-svo-api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aero-svo-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unoficial api wrapper for Sheremetyevo International Airport
 Author-email: Nikita Bulavinov <jktujgxtu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nikita Bulavinov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aero-svo-api-0.1.1/README.md` & `aero-svo-api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.1/pyproject.toml` & `aero-svo-api-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.1/src/aero_svo_api/api.py` & `aero-svo-api-0.1.2/src/aero_svo_api/api.py`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.1/src/aero_svo_api/models.py` & `aero-svo-api-0.1.2/src/aero_svo_api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     mar3: Airport | None = None
     mar4: Airport | None = None
     mar5: Airport | None = None
     aircraft: Aircraft
     main_id: int | None = Field(None, alias='main_flight')
     way_time: int
     # check-in
+    chin_id: str | None = None
     chin_start: datetime | None = Field(None, alias='t_chin_start')
     chin_end: datetime | None = Field(None, alias='t_chin_finish')
     chin_start_et: datetime | None = Field(None, alias='estimated_chin_start')
     chin_end_et: datetime | None = Field(None, alias='estimated_chin_finish')
     # boarding
     boarding_start: datetime | None = Field(None, alias='t_boarding_start')
     boarding_end: datetime | None = Field(None, alias='t_boarding_finish')
```

### Comparing `aero-svo-api-0.1.1/src/aero_svo_api.egg-info/PKG-INFO` & `aero-svo-api-0.1.2/src/aero_svo_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aero-svo-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Unoficial api wrapper for Sheremetyevo International Airport
 Author-email: Nikita Bulavinov <jktujgxtu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Nikita Bulavinov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aero-svo-api-0.1.1/tests/test_api.py` & `aero-svo-api-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `aero-svo-api-0.1.1/tests/test_models.py` & `aero-svo-api-0.1.2/tests/test_models.py`

 * *Files identical despite different names*

