# Comparing `tmp/flask-paginate-2024.3.28.tar.gz` & `tmp/flask-paginate-2024.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-paginate-2024.3.28.tar", last modified: Thu Mar 28 14:00:28 2024, max compression
+gzip compressed data, was "flask-paginate-2024.4.12.tar", last modified: Fri Apr 12 02:17:19 2024, max compression
```

## Comparing `flask-paginate-2024.3.28.tar` & `flask-paginate-2024.4.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:00:28.464820 flask-paginate-2024.3.28/
--rw-rw-rw-   0        0        0     1449 2022-04-02 02:06:49.000000 flask-paginate-2024.3.28/LICENSE
--rw-rw-rw-   0        0        0       85 2022-04-02 02:06:49.000000 flask-paginate-2024.3.28/MANIFEST.in
--rw-rw-rw-   0        0        0     1336 2024-03-28 14:00:28.463760 flask-paginate-2024.3.28/PKG-INFO
--rw-rw-rw-   0        0        0     1065 2022-04-02 02:06:49.000000 flask-paginate-2024.3.28/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 14:00:28.436844 flask-paginate-2024.3.28/flask_paginate/
--rw-rw-rw-   0        0        0    24825 2024-03-28 13:57:00.000000 flask-paginate-2024.3.28/flask_paginate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:00:28.461719 flask-paginate-2024.3.28/flask_paginate.egg-info/
--rw-rw-rw-   0        0        0     1336 2024-03-28 14:00:28.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-28 14:00:28.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:00:28.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-08 02:34:46.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2024-03-28 14:00:28.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-28 14:00:28.000000 flask-paginate-2024.3.28/flask_paginate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2024-03-28 14:00:28.466869 flask-paginate-2024.3.28/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-10-23 03:31:36.000000 flask-paginate-2024.3.28/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:00:28.457632 flask-paginate-2024.3.28/tests/
--rw-rw-rw-   0        0        0     5617 2022-04-02 02:06:49.000000 flask-paginate-2024.3.28/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:17:19.952913 flask-paginate-2024.4.12/
+-rw-rw-rw-   0        0        0     1449 2022-04-02 02:06:49.000000 flask-paginate-2024.4.12/LICENSE
+-rw-rw-rw-   0        0        0       85 2022-04-02 02:06:49.000000 flask-paginate-2024.4.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     1336 2024-04-12 02:17:19.952913 flask-paginate-2024.4.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2022-04-02 02:06:49.000000 flask-paginate-2024.4.12/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 02:17:19.930926 flask-paginate-2024.4.12/flask_paginate/
+-rw-rw-rw-   0        0        0    24831 2024-04-12 02:16:13.000000 flask-paginate-2024.4.12/flask_paginate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:17:19.950912 flask-paginate-2024.4.12/flask_paginate.egg-info/
+-rw-rw-rw-   0        0        0     1336 2024-04-12 02:17:19.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-12 02:17:19.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 02:17:19.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-08 02:34:46.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2024-04-12 02:17:19.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 02:17:19.000000 flask-paginate-2024.4.12/flask_paginate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2024-04-12 02:17:19.954913 flask-paginate-2024.4.12/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-10-23 03:31:36.000000 flask-paginate-2024.4.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 02:17:19.948409 flask-paginate-2024.4.12/tests/
+-rw-rw-rw-   0        0        0     5617 2022-04-02 02:06:49.000000 flask-paginate-2024.4.12/tests/tests.py
```

### Comparing `flask-paginate-2024.3.28/LICENSE` & `flask-paginate-2024.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-paginate-2024.3.28/PKG-INFO` & `flask-paginate-2024.4.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-paginate
-Version: 2024.3.28
+Version: 2024.4.12
 Summary: Simple paginate support for flask
 Home-page: https://github.com/lixxu/flask-paginate
 Author: Lix Xu
 Author-email: xuzenglin@gmail.com
 License: BSD-3-Clause
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `flask-paginate-2024.3.28/README.md` & `flask-paginate-2024.4.12/README.md`

 * *Files identical despite different names*

### Comparing `flask-paginate-2024.3.28/flask_paginate/__init__.py` & `flask-paginate-2024.4.12/flask_paginate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 from __future__ import unicode_literals
 
 import sys
 
 from flask import current_app, request, url_for
 from markupsafe import Markup
 
-__version__ = "2024.03.28"
+__version__ = "2024.04.12"
 
 PY2 = sys.version_info[0] == 2
 
 # previous link
 _bs = '<li class="previous"><a href="{0}"{2}>{1}</a></li>'
 _bs33 = '<li><a href="{0}" aria-label="Previous"{2}>\
 <span aria-hidden="true">{1}</span></a></li>'
 _bs4 = '<li class="page-item">\
 <a class="page-link" href="{0}" aria-label="Previous"{2}>\
 <span aria-hidden="true">{1}</span>\
 <span class="sr-only">Previous</span></a></li>'
 _bs5 = '<li class="page-item">\
 <a class="page-link" href="{0}" aria-label="Previous"{2}>\
 <span aria-hidden="true">{1}</span></a></li>'
-_bulma = '<a class="pagination-previous" href={0} aria-label="Previous"{2}>{1}</a>'
+_bulma = '<a class="pagination-previous" href="{0}" aria-label="Previous"{2}>{1}</a>'
 _materialize = '<li class="waves-effect"><a href="{0}"{1}>\
 <i class="material-icons">chevron_left</i></a></li>'
 
 PREV_PAGES = dict(
     bootstrap=_bs,
     bootstrap2=_bs,
     bootstrap3=_bs,
@@ -57,15 +57,15 @@
 _bs4 = '<li class="page-item">\
 <a class="page-link" href="{0}" aria-label="Next"{2}>\
 <span aria-hidden="true">{1}</span>\
 <span class="sr-only">Next</span></a></li>'
 _bs5 = '<li class="page-item">\
 <a class="page-link" href="{0}" aria-label="Next"{2}>\
 <span aria-hidden="true">{1}</span></a></li>'
-_bulma = '<a class="pagination-next" href={0} aria-label="Next"{2}>{1}</a>'
+_bulma = '<a class="pagination-next" href="{0}" aria-label="Next"{2}>{1}</a>'
 _materialize = '<li class="waves-effect"><a href="{0}"{1}>\
 <i class="material-icons">chevron_right</i></a></li>'
 NEXT_PAGES = dict(
     bootstrap=_bs,
     bootstrap2=_bs,
     bootstrap3=_bs,
     bootstrap3_3=_bs33,
@@ -102,15 +102,15 @@
 )
 
 # normal link
 LINK = '<li><a href="{0}">{1}</a></li>'
 SEMANTIC_LINK = '<a class="item" href="{0}">{1}</a>'
 BS4_LINK = '<li class="page-item"><a class="page-link" href="{0}">{1}</a></li>'
 BS5_LINK = '<li class="page-item"><a class="page-link" href="{0}">{1}</a></li>'
-BULMA_LINK = '<li><a class="pagination-link" href={0}>{1}</a></li>'
+BULMA_LINK = '<li><a class="pagination-link" href="{0}">{1}</a></li>'
 MATERIALIZE_LINK = '<li><a class="waves-effect" href="{0}">{1}</a></li>'
 
 # disabled link
 _bs = '<li class="disabled"><a>...</a></li>'
 _bs33 = '<li class="disabled"><span>\
 <span aria-hidden="true">...</span></span></li>'
 _bs4 = '<li class="page-item disabled"><span class="page-link">...</span></li>'
```

### Comparing `flask-paginate-2024.3.28/flask_paginate.egg-info/PKG-INFO` & `flask-paginate-2024.4.12/flask_paginate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-paginate
-Version: 2024.3.28
+Version: 2024.4.12
 Summary: Simple paginate support for flask
 Home-page: https://github.com/lixxu/flask-paginate
 Author: Lix Xu
 Author-email: xuzenglin@gmail.com
 License: BSD-3-Clause
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `flask-paginate-2024.3.28/setup.py` & `flask-paginate-2024.4.12/setup.py`

 * *Files identical despite different names*

### Comparing `flask-paginate-2024.3.28/tests/tests.py` & `flask-paginate-2024.4.12/tests/tests.py`

 * *Files identical despite different names*

