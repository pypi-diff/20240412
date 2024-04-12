# Comparing `tmp/pyshared-1.5.3-py3-none-any.whl.zip` & `tmp/pyshared-1.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 11345 bytes, number of entries: 15
--rw-r--r--  2.0 unx      755 b- defN 24-Apr-04 12:51 pyshared/__init__.py
+Zip file size: 12256 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      781 b- defN 24-Apr-12 00:41 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
 -rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
--rw-r--r--  2.0 unx      914 b- defN 24-Mar-31 21:30 pyshared/pytest.py
+-rw-r--r--  2.0 unx      936 b- defN 24-Apr-12 00:40 pyshared/pytest.py
 -rw-r--r--  2.0 unx     4929 b- defN 24-Apr-03 16:29 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-05 23:00 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6742 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-05 23:01 pyshared-1.5.3.dist-info/RECORD
-15 files, 22931 bytes uncompressed, 9485 bytes compressed:  58.6%
+-rw-r--r--  2.0 unx     2793 b- defN 24-Apr-12 01:03 pyshared/test.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-12 01:13 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6829 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/RECORD
+16 files, 25932 bytes uncompressed, 10288 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -21,26 +21,29 @@
 
 Filename: pyshared/shell.py
 Comment: 
 
 Filename: pyshared/terminal.py
 Comment: 
 
+Filename: pyshared/test.py
+Comment: 
+
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.3.dist-info/LICENSE
+Filename: pyshared-1.5.4.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.3.dist-info/METADATA
+Filename: pyshared-1.5.4.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.3.dist-info/WHEEL
+Filename: pyshared-1.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.3.dist-info/top_level.txt
+Filename: pyshared-1.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.3.dist-info/RECORD
+Filename: pyshared-1.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/__init__.py

```diff
@@ -26,7 +26,8 @@
 from .crypto import is_jwt
 from .env import typed_evar
 from .exceptions import NotPrintableError
 from .python import default_repr, ranstr, safe_repr, truncstr
 from .shell import runcmd
 from .terminal import get_terminal_width, print_columns, print_middle
 from .pytest import multiscope_fixture
+from .test import RanData
```

## pyshared/pytest.py

```diff
@@ -1,9 +1,11 @@
 import pytest as pt
 import inspect
+import random as ran
+
 from typing import Callable as Call
 
 _SCOPES = ['function', 'module', 'session']
 
 
 def multiscope_fixture(func: Call):
     """Decorator to create a fixture for each scope (function, module, session)
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.3'
+__version__ = '1.5.4'
```

## Comparing `pyshared-1.5.3.dist-info/LICENSE` & `pyshared-1.5.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.3.dist-info/METADATA` & `pyshared-1.5.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -147,14 +147,18 @@
 
 Terminal utilities for improved user interaction.
 
 - `get_terminal_width`: Safely retrieves the terminal width, defaulting to 80 columns on failure.
 - `print_middle`: Centers text within left/right padding based on terminal width.
 - `print_columns`: Arranges a list of strings into guestimated $x length strings based on what is approximately optimal for the contents/terminal width.
 
+### `tests.py`
+
+- `RanData`: A class for generating random data for testing purposes.
+
 ## Test Coverage
 
 100% lol
 
 ```
 ---------- coverage: platform darwin, python 3.9.18-final-0 ----------
 Name                     Stmts   Miss  Cover   Missing
```

## Comparing `pyshared-1.5.3.dist-info/RECORD` & `pyshared-1.5.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-pyshared/__init__.py,sha256=VqZmVO93-BblrWX_K3Wpj5oNkaGDRAwp7W7x-KUFCog,755
+pyshared/__init__.py,sha256=8TrznKzkmm9mjpR6joySUECAwvMGDK0pjCldF9PQfWo,781
 pyshared/consts.py,sha256=vfUhhaxsFGp-DnTP_iJ-ZFT_w_be6frq9VabkLzejuA,124
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
 pyshared/env.py,sha256=sJM9SVUIKVq9n7ugpC81zRhvAlNPur_Q8qUiCasglXQ,2029
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
-pyshared/pytest.py,sha256=Sr62vEHhsVtdD6g5oUtpvW07ciYkVhjnCmMCSK_LLnA,914
+pyshared/pytest.py,sha256=3coYUTNfSHB7-pQIPlIOWwOjbtjgBoX5uEc90DfH188,936
 pyshared/python.py,sha256=2AsqfdwMGv-ZwXvlaKvaPKmXwq69yFSwKIzQfMblD_E,4929
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
-pyshared/version.py,sha256=mvQ7nJwcwEkbyD9OYSTfEPdWnrUwfgEf6kkbYY_zLqU,22
-pyshared-1.5.3.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.5.3.dist-info/METADATA,sha256=LmMfT2GjBVHI6ymjT8S9mRl3YwD2vfFJzH5yepCsSsM,6742
-pyshared-1.5.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.5.3.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.5.3.dist-info/RECORD,,
+pyshared/test.py,sha256=j7mug9uYsYHq0R6NjrjvJQSIWlOEcKCRTASjejcSJxE,2793
+pyshared/version.py,sha256=J1aSCJ_LeXu9eC8GJfi0qc4dCnumcuDr3J7ga_AZg8g,22
+pyshared-1.5.4.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.4.dist-info/METADATA,sha256=FptX90LNHGBSO2sIL51ggGISuHKZberqBEpbgN7n4wg,6829
+pyshared-1.5.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.4.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.4.dist-info/RECORD,,
```

