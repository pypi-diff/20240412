# Comparing `tmp/systemd-watchdog-thread-1.0.tar.gz` & `tmp/systemd_watchdog_thread-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemd-watchdog-thread-1.0.tar", last modified: Sat Nov 18 13:34:17 2023, max compression
+gzip compressed data, was "systemd_watchdog_thread-1.1.tar", last modified: Fri Apr 12 21:36:41 2024, max compression
```

## Comparing `systemd-watchdog-thread-1.0.tar` & `systemd_watchdog_thread-1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1063 2023-10-12 18:33:56.000000 systemd-watchdog-thread-1.0/LICENSE
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1189 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/PKG-INFO
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      601 2023-11-18 12:59:29.000000 systemd-watchdog-thread-1.0/README.md
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      462 2023-11-18 13:33:55.000000 systemd-watchdog-thread-1.0/pyproject.toml
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      377 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/setup.cfg
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-11-18 13:34:17.158925 systemd-watchdog-thread-1.0/src/
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      213 2023-11-18 13:32:16.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread/__init__.py
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1870 2023-11-18 12:33:51.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread/watchdogthread.py
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1189 2023-11-18 13:34:17.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/PKG-INFO
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      404 2023-11-18 13:34:17.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/SOURCES.txt
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)        1 2023-11-18 13:34:17.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/dependency_links.txt
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)        9 2023-11-18 13:34:17.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/requires.txt
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)       24 2023-11-18 13:34:17.000000 systemd-watchdog-thread-1.0/src/systemd_watchdog_thread.egg-info/top_level.txt
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-11-18 13:34:17.162925 systemd-watchdog-thread-1.0/tests/
--rwxr-xr-x   0 gweatherby (16342) uconn_health (30059)     1210 2023-11-18 13:33:29.000000 systemd-watchdog-thread-1.0/tests/testnotifier.py
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2024-04-12 21:36:41.403392 systemd_watchdog_thread-1.1/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1063 2023-10-12 18:33:56.000000 systemd_watchdog_thread-1.1/LICENSE
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     2499 2024-04-12 21:36:41.403392 systemd_watchdog_thread-1.1/PKG-INFO
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      736 2024-04-12 21:34:58.000000 systemd_watchdog_thread-1.1/README.md
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      540 2024-04-12 21:36:10.000000 systemd_watchdog_thread-1.1/pyproject.toml
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      244 2024-04-12 21:36:41.403392 systemd_watchdog_thread-1.1/setup.cfg
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2024-04-12 21:36:41.399392 systemd_watchdog_thread-1.1/src/
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2024-04-12 21:36:41.399392 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      227 2024-04-12 21:29:10.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread/__init__.py
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1971 2024-04-12 21:28:37.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread/watchdogthread.py
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2024-04-12 21:36:41.403392 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     2499 2024-04-12 21:36:41.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/PKG-INFO
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      426 2024-04-12 21:36:41.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/SOURCES.txt
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)        1 2024-04-12 21:36:41.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/dependency_links.txt
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)        9 2024-04-12 21:36:41.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/requires.txt
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)       24 2024-04-12 21:36:41.000000 systemd_watchdog_thread-1.1/src/systemd_watchdog_thread.egg-info/top_level.txt
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2024-04-12 21:36:41.403392 systemd_watchdog_thread-1.1/tests/
+-rwxr-xr-x   0 gweatherby (16342) uconn_health (30059)      808 2024-04-12 21:32:04.000000 systemd_watchdog_thread-1.1/tests/testfunction.py
+-rwxr-xr-x   0 gweatherby (16342) uconn_health (30059)     1210 2023-11-18 13:33:29.000000 systemd_watchdog_thread-1.1/tests/testnotifier.py
```

### Comparing `systemd-watchdog-thread-1.0/LICENSE` & `systemd_watchdog_thread-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systemd-watchdog-thread-1.0/README.md` & `systemd_watchdog_thread-1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,13 +6,21 @@
 environment variable.
 
 It runs as a daemon [thread](https://docs.python.org/3/library/threading.html#thread-objects),
 so it will exit when the main program exits.
 
 ## usage
 
+    from systemd_watchdog_thread import WatchdogThread
+
     wdt = WatchdogThread()
     t = wdt.run()
 
+or
+
+    from systemd_watchdog_thread import run_watchdog 
+
+    run_watchdog()
+
 ## testing
 *finish()* may be called to stop sending READY messages. This is provided to test
 the systemd watchdog functionality.
```

### Comparing `systemd-watchdog-thread-1.0/src/systemd_watchdog_thread/watchdogthread.py` & `systemd_watchdog_thread-1.1/src/systemd_watchdog_thread/watchdogthread.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,7 +50,12 @@
             self.notify_dog()
             try:
                 if self.flag.acquire(blocking=True, timeout=self.wd_timeout):
                     wdt_logger.info("Thread exiting")
                     return
             except:
                 wdt_logger.exception(f"{self.wd_timeout} sleep")
+
+def run_watchdog():
+    """Launch watchdog daemon thread"""
+    wdt = WatchdogThread()
+    wdt.run()
```

### Comparing `systemd-watchdog-thread-1.0/tests/testnotifier.py` & `systemd_watchdog_thread-1.1/tests/testnotifier.py`

 * *Files identical despite different names*

