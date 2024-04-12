# Comparing `tmp/tb1_parser-1.0.2.tar.gz` & `tmp/tb1_parser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-1.0.2.tar", last modified: Fri Apr 12 16:08:51 2024, max compression
+gzip compressed data, was "tb1_parser-1.0.3.tar", last modified: Fri Apr 12 16:18:56 2024, max compression
```

## Comparing `tb1_parser-1.0.2.tar` & `tb1_parser-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.683119 tb1_parser-1.0.2/
--rw-rw-rw-   0        0        0      272 2024-04-12 16:08:51.682121 tb1_parser-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 16:08:51.684123 tb1_parser-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-12 16:08:48.000000 tb1_parser-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.671118 tb1_parser-1.0.2/tb1_parser/
--rw-rw-rw-   0        0        0      311 2024-04-12 15:56:18.000000 tb1_parser-1.0.2/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2127 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2213 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     6197 2024-04-12 16:07:03.000000 tb1_parser-1.0.2/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4454 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.2/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0     1625 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.681120 tb1_parser-1.0.2/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:18:56.056645 tb1_parser-1.0.3/
+-rw-rw-rw-   0        0        0      272 2024-04-12 16:18:56.055624 tb1_parser-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:18:56.057641 tb1_parser-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      393 2024-04-12 16:16:40.000000 tb1_parser-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:18:56.045564 tb1_parser-1.0.3/tb1_parser/
+-rw-rw-rw-   0        0        0      269 2024-04-12 16:17:57.000000 tb1_parser-1.0.3/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2127 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2213 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     6197 2024-04-12 16:07:03.000000 tb1_parser-1.0.3/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4454 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.3/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.3/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.3/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      540 2024-04-12 16:18:19.000000 tb1_parser-1.0.3/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-12 16:18:08.000000 tb1_parser-1.0.3/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      353 2024-04-12 16:18:02.000000 tb1_parser-1.0.3/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0      609 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/signal.py
+-rw-rw-rw-   0        0        0       74 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1625 2024-04-12 15:31:09.000000 tb1_parser-1.0.3/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:18:56.055624 tb1_parser-1.0.3/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 16:18:55.000000 tb1_parser-1.0.3/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-1.0.2/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-1.0.3/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_di_sheet_parser.py` & `tb1_parser-1.0.3/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_do_sheet_parser.py` & `tb1_parser-1.0.3/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_regex_lib.py` & `tb1_parser-1.0.3/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_sheet_parser.py` & `tb1_parser-1.0.3/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_tb1_file_reader.py` & `tb1_parser-1.0.3/tb1_parser/_tb1_file_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-1.0.3/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser/tb1_parser.py` & `tb1_parser-1.0.3/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.2/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-1.0.3/tb1_parser.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 tb1_parser/_di_sheet_parser.py
 tb1_parser/_do_sheet_parser.py
 tb1_parser/_regex_lib.py
 tb1_parser/_sheet_parser.py
 tb1_parser/_tb1_file_reader.py
 tb1_parser/_tb1_readed_sheets_collection.py
 tb1_parser/_tb1_sheet_reader.py
+tb1_parser/ai_signal.py
+tb1_parser/di_signal.py
+tb1_parser/do_signal.py
+tb1_parser/parsed_tb1_collection.py
+tb1_parser/signal.py
+tb1_parser/signals_collection.py
 tb1_parser/tb1_parser.py
 tb1_parser.egg-info/PKG-INFO
 tb1_parser.egg-info/SOURCES.txt
 tb1_parser.egg-info/dependency_links.txt
 tb1_parser.egg-info/not-zip-safe
 tb1_parser.egg-info/requires.txt
 tb1_parser.egg-info/top_level.txt
```

