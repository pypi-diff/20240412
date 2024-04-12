# Comparing `tmp/FreeBack-0.1.3.tar.gz` & `tmp/FreeBack-3.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-0.1.3.tar", last modified: Fri Apr 12 00:32:47 2024, max compression
+gzip compressed data, was "FreeBack-3.0.0b0.tar", last modified: Fri Apr 12 01:46:35 2024, max compression
```

## Comparing `FreeBack-0.1.3.tar` & `FreeBack-3.0.0b0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:32:47.133150 FreeBack-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-12 00:32:47.127149 FreeBack-0.1.3/FreeBack/
--rw-rw-rw-   0        0        0       77 2024-04-11 06:17:47.000000 FreeBack-0.1.3/FreeBack/__init__.py
--rw-rw-rw-   0        0        0    39318 2024-04-09 06:54:26.000000 FreeBack-0.1.3/FreeBack/alpha.py
--rw-rw-rw-   0        0        0    33890 2024-04-11 00:53:14.000000 FreeBack-0.1.3/FreeBack/barbybar.py
--rw-rw-rw-   0        0        0    12401 2024-04-11 06:17:47.000000 FreeBack-0.1.3/FreeBack/display.py
--rw-rw-rw-   0        0        0    10145 2024-03-01 16:35:30.000000 FreeBack-0.1.3/FreeBack/event.py
--rw-rw-rw-   0        0        0    15629 2024-04-10 06:43:08.000000 FreeBack-0.1.3/FreeBack/my_pd.py
--rw-rw-rw-   0        0        0    35542 2024-04-11 06:17:47.000000 FreeBack-0.1.3/FreeBack/post.py
--rw-rw-rw-   0        0        0      460 2024-04-08 05:39:48.000000 FreeBack-0.1.3/FreeBack/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:32:47.132150 FreeBack-0.1.3/FreeBack.egg-info/
--rw-rw-rw-   0        0        0      258 2024-04-12 00:32:47.000000 FreeBack-0.1.3/FreeBack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-12 00:32:47.000000 FreeBack-0.1.3/FreeBack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:32:47.000000 FreeBack-0.1.3/FreeBack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 00:32:47.000000 FreeBack-0.1.3/FreeBack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-11 06:54:53.000000 FreeBack-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      258 2024-04-12 00:32:47.132150 FreeBack-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-04-11 06:54:48.000000 FreeBack-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 00:32:47.134151 FreeBack-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      525 2024-04-12 00:29:43.000000 FreeBack-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.628241 FreeBack-3.0.0b0/
+drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.621129 FreeBack-3.0.0b0/FreeBack/
+-rw-rw-rw-   0        0        0       77 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/__init__.py
+-rw-rw-rw-   0        0        0    39318 2024-04-09 06:54:26.000000 FreeBack-3.0.0b0/FreeBack/alpha.py
+-rw-rw-rw-   0        0        0    33890 2024-04-11 00:53:14.000000 FreeBack-3.0.0b0/FreeBack/barbybar.py
+-rw-rw-rw-   0        0        0    12401 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/display.py
+-rw-rw-rw-   0        0        0    10145 2024-03-01 16:35:30.000000 FreeBack-3.0.0b0/FreeBack/event.py
+-rw-rw-rw-   0        0        0    15629 2024-04-10 06:43:08.000000 FreeBack-3.0.0b0/FreeBack/my_pd.py
+-rw-rw-rw-   0        0        0    35542 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/post.py
+drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.627232 FreeBack-3.0.0b0/FreeBack.egg-info/
+-rw-rw-rw-   0        0        0     1182 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2024-04-12 01:34:50.000000 FreeBack-3.0.0b0/LICENSE
+-rw-rw-rw-   0        0        0     1182 2024-04-12 01:46:35.627232 FreeBack-3.0.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-04-11 06:54:48.000000 FreeBack-3.0.0b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 01:46:35.628241 FreeBack-3.0.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-12 01:43:09.000000 FreeBack-3.0.0b0/setup.py
```

### Comparing `FreeBack-0.1.3/FreeBack/alpha.py` & `FreeBack-3.0.0b0/FreeBack/alpha.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/FreeBack/barbybar.py` & `FreeBack-3.0.0b0/FreeBack/barbybar.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/FreeBack/display.py` & `FreeBack-3.0.0b0/FreeBack/display.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/FreeBack/event.py` & `FreeBack-3.0.0b0/FreeBack/event.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/FreeBack/my_pd.py` & `FreeBack-3.0.0b0/FreeBack/my_pd.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/FreeBack/post.py` & `FreeBack-3.0.0b0/FreeBack/post.py`

 * *Files identical despite different names*

### Comparing `FreeBack-0.1.3/README.md` & `FreeBack-3.0.0b0/README.md`

 * *Files identical despite different names*

