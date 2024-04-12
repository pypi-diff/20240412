# Comparing `tmp/BetheFluid-0.4.tar.gz` & `tmp/BetheFluid-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BetheFluid-0.4.tar", last modified: Fri Apr 12 15:14:29 2024, max compression
+gzip compressed data, was "BetheFluid-0.5.tar", last modified: Fri Apr 12 15:36:25 2024, max compression
```

## Comparing `BetheFluid-0.4.tar` & `BetheFluid-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:14:29.463537 BetheFluid-0.4/
-drwxrwxrwx   0        0        0        0 2024-04-12 15:14:29.444080 BetheFluid-0.4/BetheFluid/
--rw-rw-rw-   0        0        0      242 2024-04-09 16:26:34.000000 BetheFluid-0.4/BetheFluid/__init__.py
--rw-rw-rw-   0        0        0     1999 2024-04-12 15:13:30.000000 BetheFluid-0.4/BetheFluid/calc.py
--rw-rw-rw-   0        0        0     6166 2024-04-12 14:39:26.000000 BetheFluid-0.4/BetheFluid/observable.py
--rw-rw-rw-   0        0        0    13466 2024-04-12 15:06:52.000000 BetheFluid-0.4/BetheFluid/solver.py
--rw-rw-rw-   0        0        0     1880 2024-04-12 15:13:30.000000 BetheFluid-0.4/BetheFluid/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:14:29.454774 BetheFluid-0.4/BetheFluid.egg-info/
--rw-rw-rw-   0        0        0      141 2024-04-12 15:14:29.000000 BetheFluid-0.4/BetheFluid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-04-12 15:14:29.000000 BetheFluid-0.4/BetheFluid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:14:29.000000 BetheFluid-0.4/BetheFluid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-04 15:05:54.000000 BetheFluid-0.4/BetheFluid.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-04-12 15:14:29.000000 BetheFluid-0.4/BetheFluid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 15:14:29.000000 BetheFluid-0.4/BetheFluid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      141 2024-04-12 15:14:29.462525 BetheFluid-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-12 15:14:29.463537 BetheFluid-0.4/setup.cfg
--rw-rw-rw-   0        0        0      369 2024-04-09 16:08:08.000000 BetheFluid-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:14:29.461236 BetheFluid-0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-02-07 18:49:41.000000 BetheFluid-0.4/tests/test_calc_energy.py
--rw-rw-rw-   0        0        0        0 2024-02-07 18:50:05.000000 BetheFluid-0.4/tests/test_calc_entropy.py
--rw-rw-rw-   0        0        0        0 2024-02-07 18:18:13.000000 BetheFluid-0.4/tests/test_diffusion_operator.py
--rw-rw-rw-   0        0        0        0 2024-02-07 18:18:58.000000 BetheFluid-0.4/tests/test_solver.py
--rw-rw-rw-   0        0        0      782 2024-04-09 16:00:57.000000 BetheFluid-0.4/tests/test_velocity_Lieb_Liniger.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:36:25.829430 BetheFluid-0.5/
+drwxrwxrwx   0        0        0        0 2024-04-12 15:36:25.810423 BetheFluid-0.5/BetheFluid/
+-rw-rw-rw-   0        0        0      242 2024-04-09 16:26:34.000000 BetheFluid-0.5/BetheFluid/__init__.py
+-rw-rw-rw-   0        0        0     1999 2024-04-12 15:13:30.000000 BetheFluid-0.5/BetheFluid/calc.py
+-rw-rw-rw-   0        0        0     6166 2024-04-12 14:39:26.000000 BetheFluid-0.5/BetheFluid/observable.py
+-rw-rw-rw-   0        0        0    13466 2024-04-12 15:06:52.000000 BetheFluid-0.5/BetheFluid/solver.py
+-rw-rw-rw-   0        0        0     1880 2024-04-12 15:13:30.000000 BetheFluid-0.5/BetheFluid/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:36:25.821491 BetheFluid-0.5/BetheFluid.egg-info/
+-rw-rw-rw-   0        0        0      141 2024-04-12 15:36:25.000000 BetheFluid-0.5/BetheFluid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-12 15:36:25.000000 BetheFluid-0.5/BetheFluid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:36:25.000000 BetheFluid-0.5/BetheFluid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-12-04 15:05:54.000000 BetheFluid-0.5/BetheFluid.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2024-04-12 15:36:25.000000 BetheFluid-0.5/BetheFluid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 15:36:25.000000 BetheFluid-0.5/BetheFluid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      141 2024-04-12 15:36:25.829245 BetheFluid-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:36:25.829430 BetheFluid-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      369 2024-04-12 15:35:56.000000 BetheFluid-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:36:25.827235 BetheFluid-0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-07 18:49:41.000000 BetheFluid-0.5/tests/test_calc_energy.py
+-rw-rw-rw-   0        0        0        0 2024-02-07 18:50:05.000000 BetheFluid-0.5/tests/test_calc_entropy.py
+-rw-rw-rw-   0        0        0        0 2024-02-07 18:18:13.000000 BetheFluid-0.5/tests/test_diffusion_operator.py
+-rw-rw-rw-   0        0        0        0 2024-02-07 18:18:58.000000 BetheFluid-0.5/tests/test_solver.py
+-rw-rw-rw-   0        0        0      782 2024-04-09 16:00:57.000000 BetheFluid-0.5/tests/test_velocity_Lieb_Liniger.py
```

### Comparing `BetheFluid-0.4/BetheFluid/calc.py` & `BetheFluid-0.5/BetheFluid/calc.py`

 * *Files identical despite different names*

### Comparing `BetheFluid-0.4/BetheFluid/observable.py` & `BetheFluid-0.5/BetheFluid/observable.py`

 * *Files identical despite different names*

### Comparing `BetheFluid-0.4/BetheFluid/solver.py` & `BetheFluid-0.5/BetheFluid/solver.py`

 * *Files identical despite different names*

### Comparing `BetheFluid-0.4/BetheFluid/utils.py` & `BetheFluid-0.5/BetheFluid/utils.py`

 * *Files identical despite different names*

### Comparing `BetheFluid-0.4/tests/test_velocity_Lieb_Liniger.py` & `BetheFluid-0.5/tests/test_velocity_Lieb_Liniger.py`

 * *Files identical despite different names*

