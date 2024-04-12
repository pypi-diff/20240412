# Comparing `tmp/tb1_parser-1.0.1.tar.gz` & `tmp/tb1_parser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-1.0.1.tar", last modified: Fri Apr 12 15:43:14 2024, max compression
+gzip compressed data, was "tb1_parser-1.0.2.tar", last modified: Fri Apr 12 16:08:51 2024, max compression
```

## Comparing `tb1_parser-1.0.1.tar` & `tb1_parser-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.837742 tb1_parser-1.0.1/
--rw-rw-rw-   0        0        0      272 2024-04-12 15:43:14.837742 tb1_parser-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 15:43:14.839744 tb1_parser-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-12 15:31:33.000000 tb1_parser-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.826740 tb1_parser-1.0.1/tb1_parser/
--rw-rw-rw-   0        0        0      157 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5806 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2127 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2213 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     6197 2024-04-12 12:47:47.000000 tb1_parser-1.0.1/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4454 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.1/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0     1625 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.836743 tb1_parser-1.0.1/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.683119 tb1_parser-1.0.2/
+-rw-rw-rw-   0        0        0      272 2024-04-12 16:08:51.682121 tb1_parser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:08:51.684123 tb1_parser-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      393 2024-04-12 16:08:48.000000 tb1_parser-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.671118 tb1_parser-1.0.2/tb1_parser/
+-rw-rw-rw-   0        0        0      311 2024-04-12 15:56:18.000000 tb1_parser-1.0.2/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2127 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2213 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     6197 2024-04-12 16:07:03.000000 tb1_parser-1.0.2/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4454 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.2/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.2/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0     1625 2024-04-12 15:31:09.000000 tb1_parser-1.0.2/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:08:51.681120 tb1_parser-1.0.2/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 16:08:51.000000 tb1_parser-1.0.2/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-1.0.1/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-1.0.2/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/_di_sheet_parser.py` & `tb1_parser-1.0.2/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/_do_sheet_parser.py` & `tb1_parser-1.0.2/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/_regex_lib.py` & `tb1_parser-1.0.2/tb1_parser/_regex_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,10 +133,10 @@
             'Давление': 'P',
             'Перепад давления': 'dP',
             'Ток': 'I',
             'Напряжение': 'U',
             'Уровень': 'L'
         },
         # 'find_plc_module': r'^\w{2}\-[a-z0-9-]+\,?\s+?\(?(\w(\d+).?(\d+))\)?$'
-        'find_plc_module': r'([IOAD]+.?\d+\D\d+)\s{0,}\(?(\D?\d+\-\d+)\)?'
+        'find_plc_module': r'([IOAD]+.?\d+\D+\d+)\D{0,}\(?(\w\d+\-\d+)\)?'
     }
 }
```

### Comparing `tb1_parser-1.0.1/tb1_parser/_sheet_parser.py` & `tb1_parser-1.0.2/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/_tb1_file_reader.py` & `tb1_parser-1.0.2/tb1_parser/_tb1_file_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-1.0.2/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser/tb1_parser.py` & `tb1_parser-1.0.2/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.1/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-1.0.2/tb1_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

