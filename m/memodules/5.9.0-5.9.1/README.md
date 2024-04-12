# Comparing `tmp/memodules-5.9.0.tar.gz` & `tmp/memodules-5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memodules-5.9.0.tar", last modified: Thu Apr 11 02:20:16 2024, max compression
+gzip compressed data, was "memodules-5.9.1.tar", last modified: Thu Apr 11 08:00:21 2024, max compression
```

## Comparing `memodules-5.9.0.tar` & `memodules-5.9.1.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.984761 memodules-5.9.0/
--rw-rw-rw-   0        0        0      449 2024-04-11 02:20:16.981771 memodules-5.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.786421 memodules-5.9.0/memodules/
--rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.9.0/memodules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.811338 memodules-5.9.0/memodules/alphabet_to_integer/
--rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.9.0/memodules/alphabet_to_integer/AlphabetToInteger.py
--rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.9.0/memodules/alphabet_to_integer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.815325 memodules-5.9.0/memodules/builtins/
--rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.9.0/memodules/builtins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.824295 memodules-5.9.0/memodules/builtins/tkinter/
--rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.9.0/memodules/builtins/tkinter/Event.py
--rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.9.0/memodules/builtins/tkinter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.831272 memodules-5.9.0/memodules/builtins/tkinter/ttk/
--rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.9.0/memodules/builtins/tkinter/ttk/Event.py
--rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.9.0/memodules/builtins/tkinter/ttk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.838249 memodules-5.9.0/memodules/cr_exchange_lib/
--rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.9.0/memodules/cr_exchange_lib/__init__.py
--rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.9.0/memodules/cr_exchange_lib/crExchangeLib.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.845225 memodules-5.9.0/memodules/cslapp/
--rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.9.0/memodules/cslapp/__init__.py
--rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.9.0/memodules/cslapp/calc_source.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.853199 memodules-5.9.0/memodules/debug_tools/
--rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.9.0/memodules/debug_tools/__init__.py
--rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.9.0/memodules/debug_tools/access_viewer.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.866156 memodules-5.9.0/memodules/decorators/
--rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.9.0/memodules/decorators/PushHF.py
--rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.9.0/memodules/decorators/__init__.py
--rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.9.0/memodules/decorators/debug_dec.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.874129 memodules-5.9.0/memodules/directory/
--rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.9.0/memodules/directory/__init__.py
--rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.9.0/memodules/directory/structure.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.880109 memodules-5.9.0/memodules/e_typing/
--rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.9.0/memodules/e_typing/__init__.py
--rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.9.0/memodules/e_typing/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.888083 memodules-5.9.0/memodules/error_lib/
--rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.9.0/memodules/error_lib/ErrorLib.py
--rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.9.0/memodules/error_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.900043 memodules-5.9.0/memodules/inicon/
--rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.9.0/memodules/inicon/__init__.py
--rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.9.0/memodules/inicon/inicon.py
--rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.9.0/memodules/inicon/inicon.pyi
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.904030 memodules-5.9.0/memodules/judgment/
--rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.9.0/memodules/judgment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.945891 memodules-5.9.0/memodules/log/
--rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.9.0/memodules/log/Dlog.py
--rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.9.0/memodules/log/Dlog.pyi
--rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.9.0/memodules/log/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.9.0/memodules/log/cprint.py
--rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.9.0/memodules/log/cprint.pyi
--rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.9.0/memodules/log/log.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.964827 memodules-5.9.0/memodules/sandbox/
--rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.9.0/memodules/sandbox/__init__.py
--rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.9.0/memodules/sandbox/sqlalchemy.py
--rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.9.0/memodules/sandbox/sqlalchemy.pyi
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.968814 memodules-5.9.0/memodules/sql_pack/
--rw-rw-rw-   0        0        0      724 2024-04-11 02:18:35.000000 memodules-5.9.0/memodules/sql_pack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.979778 memodules-5.9.0/memodules/xl_for_python/
--rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.9.0/memodules/xl_for_python/Python_xlTypeLib_Addin.py
--rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.9.0/memodules/xl_for_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 02:20:16.801372 memodules-5.9.0/memodules.egg-info/
--rw-rw-rw-   0        0        0      449 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1417 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 02:20:16.000000 memodules-5.9.0/memodules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 02:20:16.984761 memodules-5.9.0/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-04-11 02:20:08.000000 memodules-5.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:21.051300 memodules-5.9.1/
+-rw-rw-rw-   0        0        0      449 2024-04-11 08:00:21.049304 memodules-5.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.883094 memodules-5.9.1/memodules/
+-rw-rw-rw-   0        0        0       57 2023-11-22 03:59:37.000000 memodules-5.9.1/memodules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.903636 memodules-5.9.1/memodules/alphabet_to_integer/
+-rw-rw-rw-   0        0        0     2966 2023-07-03 08:02:29.000000 memodules-5.9.1/memodules/alphabet_to_integer/AlphabetToInteger.py
+-rw-rw-rw-   0        0        0       34 2023-07-10 05:00:24.000000 memodules-5.9.1/memodules/alphabet_to_integer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.906636 memodules-5.9.1/memodules/builtins/
+-rw-rw-rw-   0        0        0       48 2024-02-27 00:52:47.000000 memodules-5.9.1/memodules/builtins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.913305 memodules-5.9.1/memodules/builtins/tkinter/
+-rw-rw-rw-   0        0        0      779 2024-03-26 05:19:27.000000 memodules-5.9.1/memodules/builtins/tkinter/Event.py
+-rw-rw-rw-   0        0        0       87 2024-03-26 05:19:42.000000 memodules-5.9.1/memodules/builtins/tkinter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.920871 memodules-5.9.1/memodules/builtins/tkinter/ttk/
+-rw-rw-rw-   0        0        0      646 2024-03-26 05:18:53.000000 memodules-5.9.1/memodules/builtins/tkinter/ttk/Event.py
+-rw-rw-rw-   0        0        0       65 2024-03-26 05:19:07.000000 memodules-5.9.1/memodules/builtins/tkinter/ttk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.927859 memodules-5.9.1/memodules/cr_exchange_lib/
+-rw-rw-rw-   0        0        0       30 2023-07-10 05:00:52.000000 memodules-5.9.1/memodules/cr_exchange_lib/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-03 07:34:40.000000 memodules-5.9.1/memodules/cr_exchange_lib/crExchangeLib.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.933450 memodules-5.9.1/memodules/cslapp/
+-rw-rw-rw-   0        0        0        2 2023-10-31 06:11:53.000000 memodules-5.9.1/memodules/cslapp/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-10-31 04:58:15.000000 memodules-5.9.1/memodules/cslapp/calc_source.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.940556 memodules-5.9.1/memodules/debug_tools/
+-rw-rw-rw-   0        0        0       87 2024-03-21 06:14:08.000000 memodules-5.9.1/memodules/debug_tools/__init__.py
+-rw-rw-rw-   0        0        0     2779 2024-03-21 06:12:58.000000 memodules-5.9.1/memodules/debug_tools/access_viewer.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.951790 memodules-5.9.1/memodules/decorators/
+-rw-rw-rw-   0        0        0       70 2023-09-20 07:29:16.000000 memodules-5.9.1/memodules/decorators/PushHF.py
+-rw-rw-rw-   0        0        0       83 2023-09-13 06:58:38.000000 memodules-5.9.1/memodules/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2571 2023-09-13 05:52:15.000000 memodules-5.9.1/memodules/decorators/debug_dec.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.958767 memodules-5.9.1/memodules/directory/
+-rw-rw-rw-   0        0        0       80 2023-11-27 04:09:01.000000 memodules-5.9.1/memodules/directory/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-11-27 04:07:08.000000 memodules-5.9.1/memodules/directory/structure.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.964457 memodules-5.9.1/memodules/e_typing/
+-rw-rw-rw-   0        0        0     3490 2023-12-13 00:21:50.000000 memodules-5.9.1/memodules/e_typing/__init__.py
+-rw-rw-rw-   0        0        0     2342 2023-11-28 05:57:33.000000 memodules-5.9.1/memodules/e_typing/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.971937 memodules-5.9.1/memodules/error_lib/
+-rw-rw-rw-   0        0        0      261 2023-07-03 08:01:32.000000 memodules-5.9.1/memodules/error_lib/ErrorLib.py
+-rw-rw-rw-   0        0        0       25 2023-07-10 05:01:07.000000 memodules-5.9.1/memodules/error_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.977918 memodules-5.9.1/memodules/importer/
+-rw-rw-rw-   0        0        0      249 2024-04-11 05:41:26.000000 memodules-5.9.1/memodules/importer/__init__.py
+-rw-rw-rw-   0        0        0      249 2024-04-11 05:33:20.000000 memodules-5.9.1/memodules/importer/__init__.pyi
+-rw-rw-rw-   0        0        0     1418 2024-04-11 06:03:35.000000 memodules-5.9.1/memodules/importer/sqlalchemy.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.989829 memodules-5.9.1/memodules/inicon/
+-rw-rw-rw-   0        0        0      137 2023-11-21 06:53:02.000000 memodules-5.9.1/memodules/inicon/__init__.py
+-rw-rw-rw-   0        0        0     9024 2023-11-21 06:49:32.000000 memodules-5.9.1/memodules/inicon/inicon.py
+-rw-rw-rw-   0        0        0     7970 2023-11-21 06:52:14.000000 memodules-5.9.1/memodules/inicon/inicon.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.993545 memodules-5.9.1/memodules/judgment/
+-rw-rw-rw-   0        0        0      282 2023-11-22 05:58:18.000000 memodules-5.9.1/memodules/judgment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:21.022476 memodules-5.9.1/memodules/log/
+-rw-rw-rw-   0        0        0     4296 2023-12-18 00:57:53.000000 memodules-5.9.1/memodules/log/Dlog.py
+-rw-rw-rw-   0        0        0     1675 2023-12-18 00:57:13.000000 memodules-5.9.1/memodules/log/Dlog.pyi
+-rw-rw-rw-   0        0        0      184 2023-12-13 01:08:14.000000 memodules-5.9.1/memodules/log/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-12-18 07:07:23.000000 memodules-5.9.1/memodules/log/cprint.py
+-rw-rw-rw-   0        0        0     3199 2023-12-13 01:54:07.000000 memodules-5.9.1/memodules/log/cprint.pyi
+-rw-rw-rw-   0        0        0     5385 2023-07-10 23:31:34.000000 memodules-5.9.1/memodules/log/log.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:21.032384 memodules-5.9.1/memodules/sandbox/
+-rw-rw-rw-   0        0        0      168 2024-03-19 04:41:58.000000 memodules-5.9.1/memodules/sandbox/__init__.py
+-rw-rw-rw-   0        0        0     1046 2024-03-19 05:22:08.000000 memodules-5.9.1/memodules/sandbox/sqlalchemy.py
+-rw-rw-rw-   0        0        0     3078 2024-03-19 07:45:47.000000 memodules-5.9.1/memodules/sandbox/sqlalchemy.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:21.037375 memodules-5.9.1/memodules/sql_pack/
+-rw-rw-rw-   0        0        0     1477 2024-04-11 07:55:31.000000 memodules-5.9.1/memodules/sql_pack/__init__.py
+-rw-rw-rw-   0        0        0     1976 2024-04-11 07:58:30.000000 memodules-5.9.1/memodules/sql_pack/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:21.046247 memodules-5.9.1/memodules/xl_for_python/
+-rw-rw-rw-   0        0        0     2899 2023-07-10 23:30:28.000000 memodules-5.9.1/memodules/xl_for_python/Python_xlTypeLib_Addin.py
+-rw-rw-rw-   0        0        0       39 2023-07-10 05:01:49.000000 memodules-5.9.1/memodules/xl_for_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:00:20.894616 memodules-5.9.1/memodules.egg-info/
+-rw-rw-rw-   0        0        0      449 2024-04-11 08:00:20.000000 memodules-5.9.1/memodules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2024-04-11 08:00:20.000000 memodules-5.9.1/memodules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 08:00:20.000000 memodules-5.9.1/memodules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 08:00:20.000000 memodules-5.9.1/memodules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 08:00:21.051300 memodules-5.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-11 08:00:06.000000 memodules-5.9.1/setup.py
```

### Comparing `memodules-5.9.0/memodules/alphabet_to_integer/AlphabetToInteger.py` & `memodules-5.9.1/memodules/alphabet_to_integer/AlphabetToInteger.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/builtins/tkinter/Event.py` & `memodules-5.9.1/memodules/builtins/tkinter/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/builtins/tkinter/ttk/Event.py` & `memodules-5.9.1/memodules/builtins/tkinter/ttk/Event.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/cr_exchange_lib/crExchangeLib.py` & `memodules-5.9.1/memodules/cr_exchange_lib/crExchangeLib.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/cslapp/calc_source.py` & `memodules-5.9.1/memodules/cslapp/calc_source.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/debug_tools/access_viewer.py` & `memodules-5.9.1/memodules/debug_tools/access_viewer.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/decorators/debug_dec.py` & `memodules-5.9.1/memodules/decorators/debug_dec.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/e_typing/__init__.py` & `memodules-5.9.1/memodules/e_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/e_typing/__init__.pyi` & `memodules-5.9.1/memodules/e_typing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/inicon/inicon.py` & `memodules-5.9.1/memodules/inicon/inicon.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/inicon/inicon.pyi` & `memodules-5.9.1/memodules/inicon/inicon.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/log/Dlog.py` & `memodules-5.9.1/memodules/log/Dlog.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/log/Dlog.pyi` & `memodules-5.9.1/memodules/log/Dlog.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/log/cprint.py` & `memodules-5.9.1/memodules/log/cprint.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/log/cprint.pyi` & `memodules-5.9.1/memodules/log/cprint.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/log/log.py` & `memodules-5.9.1/memodules/log/log.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/sandbox/sqlalchemy.py` & `memodules-5.9.1/memodules/sandbox/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/sandbox/sqlalchemy.pyi` & `memodules-5.9.1/memodules/sandbox/sqlalchemy.pyi`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules/xl_for_python/Python_xlTypeLib_Addin.py` & `memodules-5.9.1/memodules/xl_for_python/Python_xlTypeLib_Addin.py`

 * *Files identical despite different names*

### Comparing `memodules-5.9.0/memodules.egg-info/SOURCES.txt` & `memodules-5.9.1/memodules.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,27 @@
 memodules/decorators/debug_dec.py
 memodules/directory/__init__.py
 memodules/directory/structure.py
 memodules/e_typing/__init__.py
 memodules/e_typing/__init__.pyi
 memodules/error_lib/ErrorLib.py
 memodules/error_lib/__init__.py
+memodules/importer/__init__.py
+memodules/importer/__init__.pyi
+memodules/importer/sqlalchemy.py
 memodules/inicon/__init__.py
 memodules/inicon/inicon.py
 memodules/inicon/inicon.pyi
 memodules/judgment/__init__.py
 memodules/log/Dlog.py
 memodules/log/Dlog.pyi
 memodules/log/__init__.py
 memodules/log/cprint.py
 memodules/log/cprint.pyi
 memodules/log/log.py
 memodules/sandbox/__init__.py
 memodules/sandbox/sqlalchemy.py
 memodules/sandbox/sqlalchemy.pyi
 memodules/sql_pack/__init__.py
+memodules/sql_pack/__init__.pyi
 memodules/xl_for_python/Python_xlTypeLib_Addin.py
 memodules/xl_for_python/__init__.py
```

### Comparing `memodules-5.9.0/setup.py` & `memodules-5.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='memodules',
-    version='5.9.0',
+    version='5.9.1',
     author='mie31',
     author_email='mie.mey.master@icloud.com',
     description='local use functions',
     long_description="We do not consider the use of it by third parties.",
     long_description_content_type="text/plain",
     license="MIT",
     keywords='No redistribution!',
```

