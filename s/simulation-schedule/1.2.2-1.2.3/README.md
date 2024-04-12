# Comparing `tmp/simulation-schedule-1.2.2.tar.gz` & `tmp/simulation-schedule-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation-schedule-1.2.2.tar", last modified: Tue Apr  9 17:29:36 2024, max compression
+gzip compressed data, was "simulation-schedule-1.2.3.tar", last modified: Fri Apr 12 13:48:25 2024, max compression
```

## Comparing `simulation-schedule-1.2.2.tar` & `simulation-schedule-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.887441 simulation-schedule-1.2.2/
--rw-r--r--   0 ruben      (501) staff       (20)     2012 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/AUTHORS.rst
--rw-r--r--   0 ruben      (501) staff       (20)     6542 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/HISTORY.rst
--rw-r--r--   0 ruben      (501) staff       (20)     1099 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/LICENSE.txt
--rw-r--r--   0 ruben      (501) staff       (20)      147 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/MANIFEST.in
--rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-09 17:29:36.887382 simulation-schedule-1.2.2/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)     2288 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/README.rst
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.886548 simulation-schedule-1.2.2/schedule/
--rw-r--r--   0 ruben      (501) staff       (20)    33413 2024-04-09 16:02:23.000000 simulation-schedule-1.2.2/schedule/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)        0 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/schedule/py.typed
--rw-r--r--   0 ruben      (501) staff       (20)       93 2024-04-09 17:29:36.887619 simulation-schedule-1.2.2/setup.cfg
--rw-r--r--   0 ruben      (501) staff       (20)     1599 2024-04-09 17:29:10.000000 simulation-schedule-1.2.2/setup.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-09 17:29:36.887163 simulation-schedule-1.2.2/simulation_schedule.egg-info/
--rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      305 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/SOURCES.txt
--rw-r--r--   0 ruben      (501) staff       (20)        1 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/dependency_links.txt
--rw-r--r--   0 ruben      (501) staff       (20)        9 2024-04-09 17:29:36.000000 simulation-schedule-1.2.2/simulation_schedule.egg-info/top_level.txt
--rw-r--r--   0 ruben      (501) staff       (20)    46579 2024-04-09 16:00:45.000000 simulation-schedule-1.2.2/test_schedule.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423910 simulation-schedule-1.2.3/
+-rw-r--r--   0 ruben      (501) staff       (20)     2012 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/AUTHORS.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     6542 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/HISTORY.rst
+-rw-r--r--   0 ruben      (501) staff       (20)     1099 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/LICENSE.txt
+-rw-r--r--   0 ruben      (501) staff       (20)      147 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-12 13:48:25.423849 simulation-schedule-1.2.3/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)     2288 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/README.rst
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423129 simulation-schedule-1.2.3/schedule/
+-rw-r--r--   0 ruben      (501) staff       (20)    33428 2024-04-12 13:47:40.000000 simulation-schedule-1.2.3/schedule/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/schedule/py.typed
+-rw-r--r--   0 ruben      (501) staff       (20)       93 2024-04-12 13:48:25.424091 simulation-schedule-1.2.3/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)     1599 2024-04-12 13:48:14.000000 simulation-schedule-1.2.3/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2024-04-12 13:48:25.423667 simulation-schedule-1.2.3/simulation_schedule.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     3352 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      305 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        9 2024-04-12 13:48:25.000000 simulation-schedule-1.2.3/simulation_schedule.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)    46579 2024-04-09 16:00:45.000000 simulation-schedule-1.2.3/test_schedule.py
```

### Comparing `simulation-schedule-1.2.2/AUTHORS.rst` & `simulation-schedule-1.2.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.2/HISTORY.rst` & `simulation-schedule-1.2.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.2/LICENSE.txt` & `simulation-schedule-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.2/PKG-INFO` & `simulation-schedule-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.2
+Version: 1.2.3
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.2
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.3
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simulation-schedule-1.2.2/README.rst` & `simulation-schedule-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `simulation-schedule-1.2.2/schedule/__init__.py` & `simulation-schedule-1.2.3/schedule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
     @property
     def timestamp(self) -> datetime.datetime:
         """
         :return: The current time in the scheduler's timezone
         """
         if self.is_realtime:
-            return datetime.datetime.now()
+            return datetime.datetime.now(tz=datetime.UTC)
         else:
             return self._timestamp
 
     @timestamp.setter
     def timestamp(self, timestamp) -> None:
         """
         Set the current time in the scheduler's timezone.
```

### Comparing `simulation-schedule-1.2.2/setup.py` & `simulation-schedule-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 from setuptools import setup
 
 
-SCHEDULE_VERSION = "1.2.2"
+SCHEDULE_VERSION = "1.2.3"
 SCHEDULE_DOWNLOAD_URL = "https://github.com/dbader/schedule/tarball/" + SCHEDULE_VERSION
 
 
 def read_file(filename):
     """
     Read a utf8 encoded text file and return its contents.
     """
```

### Comparing `simulation-schedule-1.2.2/simulation_schedule.egg-info/PKG-INFO` & `simulation-schedule-1.2.3/simulation_schedule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simulation-schedule
-Version: 1.2.2
+Version: 1.2.3
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
-Download-URL: https://github.com/dbader/schedule/tarball/1.2.2
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.3
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simulation-schedule-1.2.2/test_schedule.py` & `simulation-schedule-1.2.3/test_schedule.py`

 * *Files identical despite different names*

