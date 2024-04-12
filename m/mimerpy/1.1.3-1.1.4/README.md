# Comparing `tmp/mimerpy-1.1.3.tar.gz` & `tmp/mimerpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimerpy-1.1.3.tar", last modified: Thu Mar 23 10:53:14 2023, max compression
+gzip compressed data, was "dist/mimerpy-1.1.4.tar", last modified: Fri Apr 12 12:39:30 2024, max compression
```

## Comparing `mimerpy-1.1.3.tar` & `mimerpy-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 10:53:14.110503 mimerpy-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-03-23 10:48:55.000000 mimerpy-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2023-03-23 10:48:55.000000 mimerpy-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2311 2023-03-23 10:53:14.110503 mimerpy-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2023-03-23 10:48:55.000000 mimerpy-1.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-23 10:53:14.079253 mimerpy-1.1.3/mimerpy/
--rw-rw-rw-   0        0        0     6779 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/__init__.py
--rw-rw-rw-   0        0        0     3398 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/__main__.py
--rw-rw-rw-   0        0        0     8838 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/connectionPy.py
--rw-rw-rw-   0        0        0    33334 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/cursorPy.py
--rw-rw-rw-   0        0        0     3729 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/mimPyExceptionHandler.py
--rw-rw-rw-   0        0        0     3865 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/mimPyExceptions.py
--rw-rw-rw-   0        0        0    12179 2023-03-23 10:48:55.000000 mimerpy-1.1.3/mimerpy/pool.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:53:14.079253 mimerpy-1.1.3/mimerpy.egg-info/
--rw-rw-rw-   0        0        0     2311 2023-03-23 10:53:13.000000 mimerpy-1.1.3/mimerpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-03-23 10:53:13.000000 mimerpy-1.1.3/mimerpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 10:53:13.000000 mimerpy-1.1.3/mimerpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-23 10:53:13.000000 mimerpy-1.1.3/mimerpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 10:53:14.110503 mimerpy-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     4526 2023-03-23 10:48:55.000000 mimerpy-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 10:53:14.094877 mimerpy-1.1.3/src/
--rw-rw-rw-   0        0        0    62554 2023-03-23 10:48:55.000000 mimerpy-1.1.3/src/mimerapi.c
-drwxrwxrwx   0        0        0        0 2023-03-23 10:53:14.094877 mimerpy-1.1.3/tests/
--rw-rw-rw-   0        0        0    17445 2023-03-23 10:48:55.000000 mimerpy-1.1.3/tests/testConnection.py
--rw-rw-rw-   0        0        0    89573 2023-03-23 10:48:55.000000 mimerpy-1.1.3/tests/testCursor.py
--rw-rw-rw-   0        0        0    11472 2023-03-23 10:48:55.000000 mimerpy-1.1.3/tests/testMimerPool.py
--rw-rw-rw-   0        0        0    12409 2023-03-23 10:48:55.000000 mimerpy-1.1.3/tests/testMonkey.py
--rw-rw-rw-   0        0        0    58971 2023-03-23 10:48:55.000000 mimerpy-1.1.3/tests/testScrollCursor.py
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1072 2020-08-26 08:46:06.000000 mimerpy-1.1.4/LICENSE.txt
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/tests/
+-rw-r--r--   0 fral      (1000) fral      (1000)        0 2019-03-20 10:04:22.000000 mimerpy-1.1.4/tests/__init__.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    11200 2021-04-16 07:53:51.000000 mimerpy-1.1.4/tests/testMimerPool.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    12060 2021-04-16 07:53:51.000000 mimerpy-1.1.4/tests/testMonkey.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    87612 2021-06-02 23:16:00.000000 mimerpy-1.1.4/tests/testCursor.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     3391 2021-06-02 23:16:00.000000 mimerpy-1.1.4/tests/db_config.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    16969 2021-04-16 07:53:51.000000 mimerpy-1.1.4/tests/testConnection.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    57713 2021-04-16 07:53:51.000000 mimerpy-1.1.4/tests/testScrollCursor.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1369 2021-04-16 07:53:51.000000 mimerpy-1.1.4/tests/dropdb.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     2530 2024-04-12 12:39:30.000000 mimerpy-1.1.4/PKG-INFO
+-rw-rw-r--   0 fral      (1000) fral      (1000)     4405 2024-04-12 11:29:52.000000 mimerpy-1.1.4/setup.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1352 2021-04-16 07:53:51.000000 mimerpy-1.1.4/README.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)       38 2024-04-12 12:39:30.000000 mimerpy-1.1.4/setup.cfg
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy/
+-rw-rw-r--   0 fral      (1000) fral      (1000)     6593 2021-04-16 07:53:51.000000 mimerpy-1.1.4/mimerpy/__init__.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     3635 2021-05-05 21:42:14.000000 mimerpy-1.1.4/mimerpy/mimPyExceptionHandler.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    32495 2021-06-02 23:16:00.000000 mimerpy-1.1.4/mimerpy/cursorPy.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     3740 2021-05-05 21:42:14.000000 mimerpy-1.1.4/mimerpy/mimPyExceptions.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     3317 2021-04-16 07:53:51.000000 mimerpy-1.1.4/mimerpy/__main__.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)    11868 2024-04-12 11:29:52.000000 mimerpy-1.1.4/mimerpy/pool.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     8693 2024-04-12 11:29:52.000000 mimerpy-1.1.4/mimerpy/connectionPy.py
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/scripts/
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1009 2021-04-16 07:53:51.000000 mimerpy-1.1.4/scripts/windowsAutoRelease.bat
+-rw-rw-r--   0 fral      (1000) fral      (1000)      716 2021-04-16 07:53:51.000000 mimerpy-1.1.4/scripts/ubuntuAutoRelease.sh
+-rw-rw-r--   0 fral      (1000) fral      (1000)      957 2021-04-16 07:53:51.000000 mimerpy-1.1.4/scripts/ebuild.sh
+-rw-rw-r--   0 fral      (1000) fral      (1000)       39 2021-04-16 07:53:51.000000 mimerpy-1.1.4/.gitattributes
+-rw-rw-r--   0 fral      (1000) fral      (1000)      159 2021-04-16 07:53:51.000000 mimerpy-1.1.4/.gitignore
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/src/
+-rw-rw-r--   0 fral      (1000) fral      (1000)    60632 2021-04-16 07:53:51.000000 mimerpy-1.1.4/src/mimerapi.c
+-rw-r--r--   0 fral      (1000) fral      (1000)       59 2019-03-20 10:04:22.000000 mimerpy-1.1.4/MANIFEST.in
+-rw-r--r--   0 fral      (1000) fral      (1000)        0 2019-03-20 10:04:22.000000 mimerpy-1.1.4/setupinfo.py
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy.egg-info/
+-rw-rw-r--   0 fral      (1000) fral      (1000)       17 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy.egg-info/top_level.txt
+-rw-rw-r--   0 fral      (1000) fral      (1000)     2530 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy.egg-info/PKG-INFO
+-rw-rw-r--   0 fral      (1000) fral      (1000)        1 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1064 2024-04-12 12:39:30.000000 mimerpy-1.1.4/mimerpy.egg-info/SOURCES.txt
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/doc/
+-rw-rw-r--   0 fral      (1000) fral      (1000)    18790 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/mimerpy.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)      871 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/releasenotes.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)      678 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/dbtest.py
+-rw-rw-r--   0 fral      (1000) fral      (1000)     5061 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/gettingstarted.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)    15719 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/datatypes.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1293 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/index.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)    11780 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/conf.py
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/doc/_static/
+-rw-rw-r--   0 fral      (1000) fral      (1000)      469 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/_static/style.css
+-rw-rw-r--   0 fral      (1000) fral      (1000)     2346 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/installationguide.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1656 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/introduction.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     7716 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/userguide.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     8298 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/Makefile
+-rw-rw-r--   0 fral      (1000) fral      (1000)    12243 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/codeexamples.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1623 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/legalnotice.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)     5335 2024-04-12 11:29:52.000000 mimerpy-1.1.4/doc/exceptions.rst
+-rw-rw-r--   0 fral      (1000) fral      (1000)        9 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/.gitignore
+-rw-rw-r--   0 fral      (1000) fral      (1000)      811 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/make_for_windows.bat
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/doc/images/
+-rw-rw-r--   0 fral      (1000) fral      (1000)     1191 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/images/mimerhd32x32.png
+-rw-rw-r--   0 fral      (1000) fral      (1000)     5430 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/images/mimerhd32x32.ico
+-rw-rw-r--   0 fral      (1000) fral      (1000)     2200 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/images/mimerhd.png
+-rw-rw-r--   0 fral      (1000) fral      (1000)      243 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/README.txt
+drwxrwxr-x   0 fral      (1000) fral      (1000)        0 2024-04-12 12:39:30.000000 mimerpy-1.1.4/doc/_templates/
+-rw-rw-r--   0 fral      (1000) fral      (1000)      156 2021-04-16 07:53:51.000000 mimerpy-1.1.4/doc/_templates/layout.html
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mimerpy-1.1.3/LICENSE.txt` & `mimerpy-1.1.4/LICENSE.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 Mimer Information Technology
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 Mimer Information Technology
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mimerpy-1.1.3/PKG-INFO` & `mimerpy-1.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: mimerpy
-Version: 1.1.3
-Summary: Python database interface for Mimer SQL
-Home-page: https://developer.mimer.com/mimerpy
-Author: Erik Gunne & Magdalena Bostrom
-Author-email: mimerpy@mimer.com
-Maintainer: Mimer Information Technology AB
-Maintainer-email: mimerpy@mimer.com
-License: MIT
-Keywords: Mimer MimerSQL Database SQL PEP249
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-MimerPy: Python database interface for Mimer SQL
-==================================================
-MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
-`PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
-implemented on top of a Cpython wrapper of the native Mimer API interface.
-
-Requirements:
-
-* A Mimer SQL version 11 or later installation on the client side
-* A Mimer SQL version 11 or later database server
-* MimerPy is currently supported on Linux, and Windows.
-* Python 3.5 or later
-
-The source code for MimerPy resides on GitHub_. Installable packages
-can be found on PyPi_. To install, use the command:
-
-.. code-block:: console
-
-    python3 -m pip install mimerpy
-
-The source for the MimerPy manual is stored together with the source
-in the doc/ directory. We recommend reading it on the
-Mimer Information Technology `documentation site`_.
-
-The `home page`_ for the project can be found on the Mimer Information Technology developer site.
-
-
-.. _Python: http://www.python.org/
-.. _PEP 249: https://www.python.org/dev/peps/pep-0249/
-.. _MimerSQL: https://www.mimer.com
-.. _GitHub: https://github.com/mimersql/MimerPy
-.. _PyPi: https://pypi.org/project/mimerpy/
-.. _documentation site: https://developer.mimer.com/documentation
-.. _home page: https://developer.mimer.com/mimerpy
+Metadata-Version: 2.1
+Name: mimerpy
+Version: 1.1.4
+Summary: Python database interface for Mimer SQL
+Home-page: https://developer.mimer.com/mimerpy
+Author: Erik Gunne & Magdalena Bostrom
+Author-email: mimerpy@mimer.com
+Maintainer: Mimer Information Technology AB
+Maintainer-email: mimerpy@mimer.com
+License: MIT
+Description: MimerPy: Python database interface for Mimer SQL
+        ==================================================
+        MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
+        `PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
+        implemented on top of a Cpython wrapper of the native Mimer API interface.
+        
+        Requirements:
+        
+        * A Mimer SQL version 11 or later installation on the client side
+        * A Mimer SQL version 11 or later database server
+        * MimerPy is currently supported on Linux, and Windows.
+        * Python 3.5 or later
+        
+        The source code for MimerPy resides on GitHub_. Installable packages
+        can be found on PyPi_. To install, use the command:
+        
+        .. code-block:: console
+        
+            python3 -m pip install mimerpy
+        
+        The source for the MimerPy manual is stored together with the source
+        in the doc/ directory. We recommend reading it on the
+        Mimer Information Technology `documentation site`_.
+        
+        The `home page`_ for the project can be found on the Mimer Information Technology developer site.
+        
+        
+        .. _Python: http://www.python.org/
+        .. _PEP 249: https://www.python.org/dev/peps/pep-0249/
+        .. _MimerSQL: https://www.mimer.com
+        .. _GitHub: https://github.com/mimersql/MimerPy
+        .. _PyPi: https://pypi.org/project/mimerpy/
+        .. _documentation site: https://developer.mimer.com/documentation
+        .. _home page: https://developer.mimer.com/mimerpy
+        
+Keywords: Mimer MimerSQL Database SQL PEP249
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
```

### Comparing `mimerpy-1.1.3/README.rst` & `mimerpy-1.1.4/README.rst`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-MimerPy: Python database interface for Mimer SQL
-==================================================
-MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
-`PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
-implemented on top of a Cpython wrapper of the native Mimer API interface.
-
-Requirements:
-
-* A Mimer SQL version 11 or later installation on the client side
-* A Mimer SQL version 11 or later database server
-* MimerPy is currently supported on Linux, and Windows.
-* Python 3.5 or later
-
-The source code for MimerPy resides on GitHub_. Installable packages
-can be found on PyPi_. To install, use the command:
-
-.. code-block:: console
-
-    python3 -m pip install mimerpy
-
-The source for the MimerPy manual is stored together with the source
-in the doc/ directory. We recommend reading it on the
-Mimer Information Technology `documentation site`_.
-
-The `home page`_ for the project can be found on the Mimer Information Technology developer site.
-
-
-.. _Python: http://www.python.org/
-.. _PEP 249: https://www.python.org/dev/peps/pep-0249/
-.. _MimerSQL: https://www.mimer.com
-.. _GitHub: https://github.com/mimersql/MimerPy
-.. _PyPi: https://pypi.org/project/mimerpy/
-.. _documentation site: https://developer.mimer.com/documentation
-.. _home page: https://developer.mimer.com/mimerpy
+MimerPy: Python database interface for Mimer SQL
+==================================================
+MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
+`PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
+implemented on top of a Cpython wrapper of the native Mimer API interface.
+
+Requirements:
+
+* A Mimer SQL version 11 or later installation on the client side
+* A Mimer SQL version 11 or later database server
+* MimerPy is currently supported on Linux, and Windows.
+* Python 3.5 or later
+
+The source code for MimerPy resides on GitHub_. Installable packages
+can be found on PyPi_. To install, use the command:
+
+.. code-block:: console
+
+    python3 -m pip install mimerpy
+
+The source for the MimerPy manual is stored together with the source
+in the doc/ directory. We recommend reading it on the
+Mimer Information Technology `documentation site`_.
+
+The `home page`_ for the project can be found on the Mimer Information Technology developer site.
+
+
+.. _Python: http://www.python.org/
+.. _PEP 249: https://www.python.org/dev/peps/pep-0249/
+.. _MimerSQL: https://www.mimer.com
+.. _GitHub: https://github.com/mimersql/MimerPy
+.. _PyPi: https://pypi.org/project/mimerpy/
+.. _documentation site: https://developer.mimer.com/documentation
+.. _home page: https://developer.mimer.com/mimerpy
```

### Comparing `mimerpy-1.1.3/mimerpy/__init__.py` & `mimerpy-1.1.4/mimerpy/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-from platform import system
-from sys import version_info
-plat = system()
-if plat == 'Windows' and version_info[0] == 3 and version_info[1] >= 8:
-    from os import add_dll_directory
-    from winreg import HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY, ConnectRegistry, OpenKeyEx, QueryValueEx, CloseKey, EnumKey, OpenKeyEx
-    root = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
-    mimer_key = OpenKeyEx(root, r"SOFTWARE\Mimer\Mimer SQL", 0,  KEY_READ | KEY_WOW64_64KEY)
-    index = 0
-    while True:
-        try:
-            key = EnumKey(mimer_key,index)
-            if key != "License" and key != "SQLHosts":
-                version = key
-                break
-            index = index + 1
-        except OSError:
-            break
-    inner_key = OpenKeyEx(mimer_key, version)
-    path = QueryValueEx(inner_key, 'PathName')[0]
-    CloseKey(inner_key)
-    CloseKey(root)
-    add_dll_directory(path)
-
-import mimerpy
-from pkg_resources import get_distribution, DistributionNotFound
-
-#
-#  Set version number from tag in git
-#
-try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
-    # Package is not installed
-    pass
-
-
-#
-# Set globals in mimerpy module and version in mimerapi module
-#
-import mimerapi
-import re
-
-apilevel = '2.0'
-threadsafety = '1'
-paramstyle = 'qmark'
-_v = re.findall(r'^\d+\.\d+\.\d+$', __version__)
-version = _v[0] if len(_v) else ''
-version_info = tuple([int(x) for x in version.split(".")]) if len(version) else ()
-mimerapi.__version__ = mimerapi.mimerAPIVersion().rstrip()
-
-
-#
-#  Check MimerAPI required version and set function level
-#
-from mimerpy.mimPyExceptions import *
-from mimerpy.mimPyExceptionHandler import mimerpy_error
-
-(_a, _b, _c, _d) = re.findall(r'^(\d+)\.(\d+)\.(\d)+(.)',
-                              mimerapi.__version__)[0]
-mimerapi._version_tuple = (int(_a), int(_b), int(_c), _d)
-if mimerapi._version_tuple < (11, 0, 5, 'A'):
-    raise NotSupportedError((-25101, mimerpy_error[-25101]))
-elif mimerapi._version_tuple < (11, 0, 5, 'B'):
-    # First supported version
-    mimerapi._level = 1
-else:
-    # String access to DECIMAL(p,s) and FLOAT(p). Map to Python decimal
-    mimerapi._level = 2
-
-
-from mimerpy.connectionPy import Connection
-
-def connect(dsn='', user='', password='',
-            autocommit=False, errorhandler=None):
-    """
-    Create a database connection.
-
-    dsn         Data source name.
-                If empty, the environment variable MIMER_DATABASE is consulted.
-                If that variable is unavailable, the default database as
-                specified in /etc/sqlhosts (UNIX) or in the Mimer Administrator
-                (Windows) is used.
-
-    user        Name of the ident to use.
-                If empty, the database server will perform an OS_USER login
-                using the OS-level username. This does not work if the database
-                server is remote.
-
-    password    Password to chosen ident.
-                Leave this empty if performing an OS_USER login.
-
-    autocommit  Autocommit mode.
-                The default behaviour according to PEP-0249 is False, meaning
-                that all transactions have to be explicitly committed.
-                If autocommit is enabled, each statement is committed
-                automatically when executed.
-
-    errorhandler A handler for errors according to the Optional Error Handling
-                Extension described in PEP-0249.
-    """
-    return Connection(dsn, user, password, autocommit, errorhandler)
-
-#
-#  Tracing and logging
-#
-import functools
-import logging
-from mimerpy.cursorPy import _define_funcs
-
-def _tracefunc(func, prefix, logger):
-    @functools.wraps(func)
-    def tracer(*args, **kwargs):
-        r_args = [repr(a) for a in args]
-        r_kwargs = ["%s=%s" % (k, repr(v)) for k, v in kwargs.items()]
-        signature = ", ".join(r_args + r_kwargs)
-        logger.info("%sCall %s(%s)"
-                    % (prefix, func.__name__, signature))
-        try:
-            value = func(*args, **kwargs)
-            logger.info("%sRet: %s" % (prefix, repr(value)))
-            return value
-        except Exception as e:
-            logger.info("EXCEPTION: %s" % repr(e))
-            raise e
-    return tracer
-
-def _alterfuncs(d, prefix, logger):
-    for fn in dir(d):
-        f = d.__getattribute__(fn)
-        if fn[0] != '_' and fn[0] >= 'a' and callable(f):
-            setattr(d, fn, _tracefunc(f, prefix, logger))
-
-def _apitrace(prefix=''):
-    logger = logging.getLogger("MimerAPI")
-    logger.setLevel(logging.INFO)
-    _alterfuncs(mimerapi, prefix, logger)
-    _define_funcs()
-
-def _altermeths(d, prefix, logger):
-    for fn in dir(d):
-        if fn[0] != '_' and fn[0] >= 'a':
-            try:
-                f = d.__getattribute__(d, fn)
-                if callable(f):
-                    setattr(d, fn, _tracefunc(f, prefix, logger))
-            except AttributeError:
-                pass
-
-def _pytrace(prefix=''):
-    logger = logging.getLogger("MimerPy")
-    logger.setLevel(logging.INFO)
-    _alterfuncs(mimerpy, prefix, logger)
-    _altermeths(mimerpy.connectionPy.Connection, prefix, logger)
-    _altermeths(mimerpy.cursorPy.Cursor, prefix, logger)
-    _altermeths(mimerpy.cursorPy.ScrollCursor, prefix, logger)
-
-def _trace(things=255, prefix='', setLogLevel=True):
-    if setLogLevel:
-        logging.basicConfig(level=logging.INFO)
-    if things & 1:
-        _pytrace(prefix)
-    if things & 2:
-        _apitrace(prefix)
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+from platform import system
+from sys import version_info
+plat = system()
+if plat == 'Windows' and version_info[0] == 3 and version_info[1] >= 8:
+    from os import add_dll_directory
+    from winreg import HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY, ConnectRegistry, OpenKeyEx, QueryValueEx, CloseKey, EnumKey, OpenKeyEx
+    root = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
+    mimer_key = OpenKeyEx(root, r"SOFTWARE\Mimer\Mimer SQL", 0,  KEY_READ | KEY_WOW64_64KEY)
+    index = 0
+    while True:
+        try:
+            key = EnumKey(mimer_key,index)
+            if key != "License" and key != "SQLHosts":
+                version = key
+                break
+            index = index + 1
+        except OSError:
+            break
+    inner_key = OpenKeyEx(mimer_key, version)
+    path = QueryValueEx(inner_key, 'PathName')[0]
+    CloseKey(inner_key)
+    CloseKey(root)
+    add_dll_directory(path)
+
+import mimerpy
+from pkg_resources import get_distribution, DistributionNotFound
+
+#
+#  Set version number from tag in git
+#
+try:
+    __version__ = get_distribution(__name__).version
+except DistributionNotFound:
+    # Package is not installed
+    pass
+
+
+#
+# Set globals in mimerpy module and version in mimerapi module
+#
+import mimerapi
+import re
+
+apilevel = '2.0'
+threadsafety = '1'
+paramstyle = 'qmark'
+_v = re.findall(r'^\d+\.\d+\.\d+$', __version__)
+version = _v[0] if len(_v) else ''
+version_info = tuple([int(x) for x in version.split(".")]) if len(version) else ()
+mimerapi.__version__ = mimerapi.mimerAPIVersion().rstrip()
+
+
+#
+#  Check MimerAPI required version and set function level
+#
+from mimerpy.mimPyExceptions import *
+from mimerpy.mimPyExceptionHandler import mimerpy_error
+
+(_a, _b, _c, _d) = re.findall(r'^(\d+)\.(\d+)\.(\d)+(.)',
+                              mimerapi.__version__)[0]
+mimerapi._version_tuple = (int(_a), int(_b), int(_c), _d)
+if mimerapi._version_tuple < (11, 0, 5, 'A'):
+    raise NotSupportedError((-25101, mimerpy_error[-25101]))
+elif mimerapi._version_tuple < (11, 0, 5, 'B'):
+    # First supported version
+    mimerapi._level = 1
+else:
+    # String access to DECIMAL(p,s) and FLOAT(p). Map to Python decimal
+    mimerapi._level = 2
+
+
+from mimerpy.connectionPy import Connection
+
+def connect(dsn='', user='', password='',
+            autocommit=False, errorhandler=None):
+    """
+    Create a database connection.
+
+    dsn         Data source name.
+                If empty, the environment variable MIMER_DATABASE is consulted.
+                If that variable is unavailable, the default database as
+                specified in /etc/sqlhosts (UNIX) or in the Mimer Administrator
+                (Windows) is used.
+
+    user        Name of the ident to use.
+                If empty, the database server will perform an OS_USER login
+                using the OS-level username. This does not work if the database
+                server is remote.
+
+    password    Password to chosen ident.
+                Leave this empty if performing an OS_USER login.
+
+    autocommit  Autocommit mode.
+                The default behaviour according to PEP-0249 is False, meaning
+                that all transactions have to be explicitly committed.
+                If autocommit is enabled, each statement is committed
+                automatically when executed.
+
+    errorhandler A handler for errors according to the Optional Error Handling
+                Extension described in PEP-0249.
+    """
+    return Connection(dsn, user, password, autocommit, errorhandler)
+
+#
+#  Tracing and logging
+#
+import functools
+import logging
+from mimerpy.cursorPy import _define_funcs
+
+def _tracefunc(func, prefix, logger):
+    @functools.wraps(func)
+    def tracer(*args, **kwargs):
+        r_args = [repr(a) for a in args]
+        r_kwargs = ["%s=%s" % (k, repr(v)) for k, v in kwargs.items()]
+        signature = ", ".join(r_args + r_kwargs)
+        logger.info("%sCall %s(%s)"
+                    % (prefix, func.__name__, signature))
+        try:
+            value = func(*args, **kwargs)
+            logger.info("%sRet: %s" % (prefix, repr(value)))
+            return value
+        except Exception as e:
+            logger.info("EXCEPTION: %s" % repr(e))
+            raise e
+    return tracer
+
+def _alterfuncs(d, prefix, logger):
+    for fn in dir(d):
+        f = d.__getattribute__(fn)
+        if fn[0] != '_' and fn[0] >= 'a' and callable(f):
+            setattr(d, fn, _tracefunc(f, prefix, logger))
+
+def _apitrace(prefix=''):
+    logger = logging.getLogger("MimerAPI")
+    logger.setLevel(logging.INFO)
+    _alterfuncs(mimerapi, prefix, logger)
+    _define_funcs()
+
+def _altermeths(d, prefix, logger):
+    for fn in dir(d):
+        if fn[0] != '_' and fn[0] >= 'a':
+            try:
+                f = d.__getattribute__(d, fn)
+                if callable(f):
+                    setattr(d, fn, _tracefunc(f, prefix, logger))
+            except AttributeError:
+                pass
+
+def _pytrace(prefix=''):
+    logger = logging.getLogger("MimerPy")
+    logger.setLevel(logging.INFO)
+    _alterfuncs(mimerpy, prefix, logger)
+    _altermeths(mimerpy.connectionPy.Connection, prefix, logger)
+    _altermeths(mimerpy.cursorPy.Cursor, prefix, logger)
+    _altermeths(mimerpy.cursorPy.ScrollCursor, prefix, logger)
+
+def _trace(things=255, prefix='', setLogLevel=True):
+    if setLogLevel:
+        logging.basicConfig(level=logging.INFO)
+    if things & 1:
+        _pytrace(prefix)
+    if things & 2:
+        _apitrace(prefix)
```

### Comparing `mimerpy-1.1.3/mimerpy/__main__.py` & `mimerpy-1.1.4/mimerpy/__main__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import mimerpy
-import mimerapi
-import argparse
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(prog = "mimerpy", description="""
-A simple command line program for the MimerPy library. It can
-display the version number of the MimerPy library (-v switch) or
-connect to a Mimer SQL database server and execute a singe SQL
-statement (provide database, user, and password arguments and a
-SQL statement).
-""")
-    parser.add_argument("-d", "--database",
-                        help="Database to connect to")
-    parser.add_argument("-u", "--user",
-                        help="User name to use in connection")
-    parser.add_argument("-p", "--password",
-                        help="Password for the user")
-    parser.add_argument("-v", "--version",
-                        help="Display MimerPy and MimerAPI version numbers",
-                        action="store_true")
-    parser.add_argument("-t", "--tag",
-                        help=argparse.SUPPRESS, action="store_true")
-    parser.add_argument("--trace",
-                        help=argparse.SUPPRESS, action="store_true")
-    parser.add_argument("sql", default=None, nargs='?',
-                        help="A SQL command to execute")
-    args = parser.parse_args()
-
-    something = False
-
-    if args.tag:
-        something = True
-        print(mimerpy.version)
-
-    if args.version:
-        something = True
-        print("MimerPy   version %s" % mimerpy.__version__)
-        print("Mimer API version %s" % mimerapi.__version__)
-
-    if args.sql:
-        something = True
-        try:
-            if args.trace:
-                mimerpy._trace()
-            with mimerpy.connect(dsn = args.database,
-                                 user = args.user,
-                                 password = args.password,
-                                 autocommit = True) as con:
-                with con.cursor() as cur:
-                    cur.execute(args.sql)
-                    if cur.description is not None:
-                        for r in cur:
-                            print(r)
-        except Exception as e:
-            print(e)
-
-    if not something:
-        print("Use option -h to get help")
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import mimerpy
+import mimerapi
+import argparse
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(prog = "mimerpy", description="""
+A simple command line program for the MimerPy library. It can
+display the version number of the MimerPy library (-v switch) or
+connect to a Mimer SQL database server and execute a singe SQL
+statement (provide database, user, and password arguments and a
+SQL statement).
+""")
+    parser.add_argument("-d", "--database",
+                        help="Database to connect to")
+    parser.add_argument("-u", "--user",
+                        help="User name to use in connection")
+    parser.add_argument("-p", "--password",
+                        help="Password for the user")
+    parser.add_argument("-v", "--version",
+                        help="Display MimerPy and MimerAPI version numbers",
+                        action="store_true")
+    parser.add_argument("-t", "--tag",
+                        help=argparse.SUPPRESS, action="store_true")
+    parser.add_argument("--trace",
+                        help=argparse.SUPPRESS, action="store_true")
+    parser.add_argument("sql", default=None, nargs='?',
+                        help="A SQL command to execute")
+    args = parser.parse_args()
+
+    something = False
+
+    if args.tag:
+        something = True
+        print(mimerpy.version)
+
+    if args.version:
+        something = True
+        print("MimerPy   version %s" % mimerpy.__version__)
+        print("Mimer API version %s" % mimerapi.__version__)
+
+    if args.sql:
+        something = True
+        try:
+            if args.trace:
+                mimerpy._trace()
+            with mimerpy.connect(dsn = args.database,
+                                 user = args.user,
+                                 password = args.password,
+                                 autocommit = True) as con:
+                with con.cursor() as cur:
+                    cur.execute(args.sql)
+                    if cur.description is not None:
+                        for r in cur:
+                            print(r)
+        except Exception as e:
+            print(e)
+
+    if not something:
+        print("Use option -h to get help")
```

### Comparing `mimerpy-1.1.3/mimerpy/connectionPy.py` & `mimerpy-1.1.4/mimerpy/connectionPy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,270 +1,273 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import mimerapi
-import weakref
-from mimerpy.cursorPy import *
-from mimerpy.mimPyExceptionHandler import *
-import sys
-
-def defaulterrorhandler(connection, cursor, errorclass, errorvalue):
-    """
-    If cursor is not None, (errorclass, errorvalue) is appended to
-    cursor.messages; otherwise it is appended to
-    connection.messages. Then errorclass is raised with errorvalue as
-    the value.
-    You can override this with your own error handler by assigning it
-    to the instance.
-    """
-#    sys.tracebacklimit = 1
-    error = errorclass, errorvalue
-    if cursor:
-        cursor.messages.append(error)
-    else:
-        connection.messages.append(error)
-
-    raise errorclass(errorvalue)
-
-
-class Connection:
-
-    """
-
-        MimerSQL database connection
-
-        The class Connection is used to establish
-        a connection with a Mimer database.
-
-    """
-
-    def __init__(self, dsn='', user='', password='',
-                 autocommit=False, errorhandler=None):
-        """
-        Creates a database connection.
-
-        Use the mimerpy.connect() function to create a connection rather than
-        calling this function.
-        """
-        self.autocommitmode = autocommit
-        self.errorhandler = (errorhandler if errorhandler
-                             else defaulterrorhandler)
-        self.messages = []
-        self._session = None
-        self.__cursors = weakref.WeakSet()
-        self._transaction = False
-
-        dsn = dsn if dsn else ""
-        user = user if user else ""
-        password = password if password else ""
-
-        (self._session, rc) = mimerapi.mimerBeginSession8(dsn, user, password)
-        if rc:
-            if rc == 90:
-                rc = -25031     # Login failure
-            (ec, ev) = get_mimerapi_exception(rc, self._session)
-            mimerapi.mimerEndSession(self._session)
-            self._session = None
-            self.errorhandler(self, None, ec, ev)
-
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self,type, value, traceback):
-        self.__check_if_open()
-        self.close()
-
-    def __del__(self):
-        if (not self._session == None):
-            self.close()
-
-    def close(self):
-        """
-
-            Closes the database connection.
-
-            Method is used for closing a connection.
-            When using close() all cursors that are
-            using the connection are also closed.
-
-            If the auto-commit feature is turned off
-            and a connection is closed before committing
-            any changes, an implicit rollback is executed.
-            Thus, before evoking close(), commit() should
-            be used to prevent any changes being lost. However,
-            if auto-commit is turned on, an implicit rollback
-            is not performed.
-
-            When a connection has been closed using close(),
-            it is unusable and a ProgrammingError() is raised
-            if any operations are attempted on the connection.
-
-        """
-        if (not self._session == None):
-            for cur in self.__cursors:
-                cur.close()
-
-            if (self._transaction):
-                rc_value = mimerapi.mimerEndTransaction(self._session, 1)
-                self.__check_mimerapi_error(rc_value, self._session)
-                self._transaction = False
-            rc_value = mimerapi.mimerEndSession(self._session)
-            self.__check_mimerapi_error(rc_value, self._session)
-            self._session = None
-
-    def rollback(self):
-        """
-
-            Rolls back any pending transaction. Causes the database
-            to roll back to the start of any pending transaction.
-            If a connection is closed without committing any changes
-            made during the transaction, a rollback is implicitly performed.
-
-        """
-        self.__check_if_open()
-        rc_value = mimerapi.mimerEndTransaction(self._session, 1)
-        self.__check_mimerapi_error(rc_value, self._session)
-        self._transaction = False
-
-    def commit(self):
-        """Commits any pending transaction."""
-        self.__check_if_open()
-        rc_value = mimerapi.mimerEndTransaction(self._session, 0)
-        self.__check_mimerapi_error(rc_value, self._session)
-        self._transaction = False
-
-    def cursor(self, **kwargs):
-        """
-
-            Returns a new Cursor Object using the connection.
-            If scrollable is unspecified, the default cursor class
-            will be returned. If scrollable = True a scrollable
-            cursor will be returned.
-
-        """
-        self.__check_if_open()
-        kwargs2 = kwargs.copy()
-        mode = kwargs2.pop('scrollable', False)
-        if (mode):
-             curs = ScrollCursor(self, self._session)
-        else:
-             curs = Cursor(self, self._session)
-
-        self.__cursors.add(curs)
-        return curs
-
-    def execute(self, *arg):
-        """
-            Creates a cursor and executes a database operation.
-
-            arg
-                query to execute
-
-            Returns a new Cursor object using the connection and executes
-            a database operation.
-
-        """
-        self.__check_if_open()
-        curs = Cursor(self, self._session)
-        self.__cursors.add(curs)
-        curs.execute(*arg)
-        return curs
-
-    def executemany(self, *arg):
-        """
-            Creates a cursor and executes a database operation.
-
-            arg
-                query to execute and parameter sequences.
-
-            Returns a new Cursor object using the connection and executes
-            a database operation against all parameter sequences or mappings
-            found in args.
-
-        """
-        self.__check_if_open()
-        curs = Cursor(self, self._session)
-        self.__cursors.add(curs)
-        curs.executemany(*arg)
-        return curs
-
-    def autocommit(self, mode):
-        """
-
-        Turns autocommit mode on or off. Defualt is false.
-        By using this method, from this point onward changes are autocommitted.
-
-        arg
-            Boolean
-
-        """
-        if (mode):
-            self.autocommitmode = True
-            if (self._transaction):
-                self.rollback()
-        else:
-            self.autocommitmode = False
-
-    def reset(self):
-        """
-        Reset the connection. Close all cursors and do rollback if a transaction
-        is running. Reset auto commit to default.
-        """
-        if self.__cursors:
-            for cur in self.__cursors:
-                cur.close()
-        
-        if self._transaction:
-            self.rollback()
-        
-        self.autocommit(False)
-
-    def __raise_exception(self, rc):
-        self.errorhandler(self, None, get_error_class(rc),
-                          (rc, mimerpy_error[rc]))
-
-    def __check_if_open(self):
-        if (self._session == None):
-            self.__raise_exception(-25010)
-
-    def __check_mimerapi_error(self, rc, handle):
-        if rc < 0:
-            (ec, ev) = get_mimerapi_exception(rc, handle)
-            self.errorhandler(self, None, ec, ev)
-
-    def xid(self):
-        self.__raise_exception(-25001)
-
-    def tpc_begin(self):
-        self.__raise_exception(-25001)
-
-    def tpc_prepare(self):
-        self.__raise_exception(-25001)
-
-    def tpc_commit(self):
-        self.__raise_exception(-25001)
-
-    def tpc_rollback(self):
-        self.__raise_exception(-25001)
-
-    def tpc_recover(self):
-        self.__raise_exception(-25001)
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import mimerapi
+import weakref
+from mimerpy.cursorPy import *
+from mimerpy.mimPyExceptionHandler import *
+import sys
+
+def defaulterrorhandler(connection, cursor, errorclass, errorvalue):
+    """
+    If cursor is not None, (errorclass, errorvalue) is appended to
+    cursor.messages; otherwise it is appended to
+    connection.messages. Then errorclass is raised with errorvalue as
+    the value.
+    You can override this with your own error handler by assigning it
+    to the instance.
+    """
+#    sys.tracebacklimit = 1
+    error = errorclass, errorvalue
+    if cursor:
+        cursor.messages.append(error)
+    else:
+        connection.messages.append(error)
+
+    raise errorclass(errorvalue)
+
+
+class Connection:
+
+    """
+
+        MimerSQL database connection
+
+        The class Connection is used to establish
+        a connection with a Mimer database.
+
+    """
+
+    def __init__(self, dsn='', user='', password='',
+                 autocommit=False, errorhandler=None):
+        """
+        Creates a database connection.
+
+        Use the mimerpy.connect() function to create a connection rather than
+        calling this function.
+        """
+        self.autocommitmode = autocommit
+        self.errorhandler = (errorhandler if errorhandler
+                             else defaulterrorhandler)
+        self.messages = []
+        self._session = None
+        self.__cursors = weakref.WeakSet()
+        self._transaction = False
+
+        dsn = dsn if dsn else ""
+        user = user if user else ""
+        password = password if password else ""
+
+        (self._session, rc) = mimerapi.mimerBeginSession8(dsn, user, password)
+        if rc:
+            if rc == 90:
+                rc = -25031     # Login failure
+            (ec, ev) = get_mimerapi_exception(rc, self._session)
+            mimerapi.mimerEndSession(self._session)
+            self._session = None
+            self.errorhandler(self, None, ec, ev)
+
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self,type, value, traceback):
+        self.__check_if_open()
+        self.close()
+
+    def __del__(self):
+        if (not self._session == None):
+            self.close()
+
+    def close(self):
+        """
+
+            Closes the database connection.
+
+            Method is used for closing a connection.
+            When using close() all cursors that are
+            using the connection are also closed.
+
+            If the auto-commit feature is turned off
+            and a connection is closed before committing
+            any changes, an implicit rollback is executed.
+            Thus, before evoking close(), commit() should
+            be used to prevent any changes being lost. However,
+            if auto-commit is turned on, an implicit rollback
+            is not performed.
+
+            When a connection has been closed using close(),
+            it is unusable and a ProgrammingError() is raised
+            if any operations are attempted on the connection.
+
+        """
+        if (not self._session == None):
+            for cur in self.__cursors:
+                cur.close()
+
+            if (self._transaction):
+                rc_value = mimerapi.mimerEndTransaction(self._session, 1)
+                if (rc_value != -24101):
+                    self.__check_mimerapi_error(rc_value, self._session)
+                self._transaction = False
+            rc_value = mimerapi.mimerEndSession(self._session)
+            self.__check_mimerapi_error(rc_value, self._session)
+            self._session = None
+
+    def rollback(self):
+        """
+
+            Rolls back any pending transaction. Causes the database
+            to roll back to the start of any pending transaction.
+            If a connection is closed without committing any changes
+            made during the transaction, a rollback is implicitly performed.
+
+        """
+        self.__check_if_open()
+        if (self._transaction):
+            rc_value = mimerapi.mimerEndTransaction(self._session, 1)
+            self.__check_mimerapi_error(rc_value, self._session)
+        self._transaction = False
+
+    def commit(self):
+        """Commits any pending transaction."""
+        self.__check_if_open()
+        if (self._transaction):
+            rc_value = mimerapi.mimerEndTransaction(self._session, 0)
+            self.__check_mimerapi_error(rc_value, self._session)
+        self._transaction = False
+
+    def cursor(self, **kwargs):
+        """
+
+            Returns a new Cursor Object using the connection.
+            If scrollable is unspecified, the default cursor class
+            will be returned. If scrollable = True a scrollable
+            cursor will be returned.
+
+        """
+        self.__check_if_open()
+        kwargs2 = kwargs.copy()
+        mode = kwargs2.pop('scrollable', False)
+        if (mode):
+             curs = ScrollCursor(self, self._session)
+        else:
+             curs = Cursor(self, self._session)
+
+        self.__cursors.add(curs)
+        return curs
+
+    def execute(self, *arg):
+        """
+            Creates a cursor and executes a database operation.
+
+            arg
+                query to execute
+
+            Returns a new Cursor object using the connection and executes
+            a database operation.
+
+        """
+        self.__check_if_open()
+        curs = Cursor(self, self._session)
+        self.__cursors.add(curs)
+        curs.execute(*arg)
+        return curs
+
+    def executemany(self, *arg):
+        """
+            Creates a cursor and executes a database operation.
+
+            arg
+                query to execute and parameter sequences.
+
+            Returns a new Cursor object using the connection and executes
+            a database operation against all parameter sequences or mappings
+            found in args.
+
+        """
+        self.__check_if_open()
+        curs = Cursor(self, self._session)
+        self.__cursors.add(curs)
+        curs.executemany(*arg)
+        return curs
+
+    def autocommit(self, mode):
+        """
+
+        Turns autocommit mode on or off. Defualt is false.
+        By using this method, from this point onward changes are autocommitted.
+
+        arg
+            Boolean
+
+        """
+        if (mode):
+            self.autocommitmode = True
+            if (self._transaction):
+                self.rollback()
+        else:
+            self.autocommitmode = False
+
+    def reset(self):
+        """
+        Reset the connection. Close all cursors and do rollback if a transaction
+        is running. Reset auto commit to default.
+        """
+        if self.__cursors:
+            for cur in self.__cursors:
+                cur.close()
+        
+        if self._transaction:
+            self.rollback()
+        
+        self.autocommit(False)
+
+    def __raise_exception(self, rc):
+        self.errorhandler(self, None, get_error_class(rc),
+                          (rc, mimerpy_error[rc]))
+
+    def __check_if_open(self):
+        if (self._session == None):
+            self.__raise_exception(-25010)
+
+    def __check_mimerapi_error(self, rc, handle):
+        if rc < 0:
+            (ec, ev) = get_mimerapi_exception(rc, handle)
+            self.errorhandler(self, None, ec, ev)
+
+    def xid(self):
+        self.__raise_exception(-25001)
+
+    def tpc_begin(self):
+        self.__raise_exception(-25001)
+
+    def tpc_prepare(self):
+        self.__raise_exception(-25001)
+
+    def tpc_commit(self):
+        self.__raise_exception(-25001)
+
+    def tpc_rollback(self):
+        self.__raise_exception(-25001)
+
+    def tpc_recover(self):
+        self.__raise_exception(-25001)
```

### Comparing `mimerpy-1.1.3/mimerpy/cursorPy.py` & `mimerpy-1.1.4/mimerpy/cursorPy.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,839 +1,839 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-from mimerpy.mimPyExceptionHandler import *
-import mimerapi
-import collections, decimal, uuid
-from types import GeneratorType
-
-
-def _pythonSetDecimal(statement, cur_column, parameter):
-    if parameter is None:
-        rc = mimerapi.mimerSetString8(statement, cur_column, parameter)
-    else: 
-        rc = mimerapi.mimerSetString8(statement, cur_column, str(parameter))
-    return rc
-
-def _pythonSetDecimalF(statement, cur_column, parameter):
-    if mimerapi._level >= 2:
-        return _pythonSetDecimal(statement, cur_column, parameter)
-    return -25102
-
-def _pythonGetDecimal(statement, cur_column):
-    rc, val = mimerapi.mimerGetString8(statement, cur_column)
-    if rc >= 0 and val is not None:
-        val = decimal.Decimal(val)
-    return (rc, val)
-
-def _pythonGetDecimalF(statement, cur_column):
-    if mimerapi._level >= 2:
-        return _pythonGetDecimal(statement, cur_column)
-    return (-25102, None)
-
-def _pythonGetInt(statement, col):
-    if mimerapi._level >= 2:
-        rc, val = mimerapi.mimerGetString8(statement, col)
-        if rc >= 0 and val is not None:
-            return (0, int(val))
-        return (rc, None)
-    return mimerapi.mimerGetInt64(statement, col)
-
-def _pythonSetInt(statement, col, val):
-    if mimerapi._level >= 2 and val is not None:
-        return mimerapi.mimerSetString8(statement, col, str(val))
-    return mimerapi.mimerSetInt64(statement, col, val)
-
-def _pythonGetUUID(statement, col):
-    rc, val = mimerapi.mimerGetUUID(statement, col)
-    if rc >= 0 and val is not None:
-        return (0, uuid.UUID(bytes=val))
-    return (rc, None)
-
-def _pythonSetUUID(statement, col, val):
-    return mimerapi.mimerSetUUID(statement, col, val.bytes)
-
-def _define_funcs():
-    global get_funcs
-    global set_funcs
-
-    TYPEID_MASK = 0x40000000
-
-    get_funcs = {1: mimerapi.mimerGetString8,
-                 2: _pythonGetDecimal,
-                 31: _pythonGetDecimal,
-                 3: _pythonGetInt,
-                 4: _pythonGetDecimalF,
-                 6: mimerapi.mimerGetInt32,
-                 10: mimerapi.mimerGetDouble,
-                 11: mimerapi.mimerGetString8,
-                 12: mimerapi.mimerGetString8,
-                 13: mimerapi.mimerGetString8,
-                 14: mimerapi.mimerGetString8,
-                 15: mimerapi.mimerGetString8,
-                 16: mimerapi.mimerGetString8,
-                 17: mimerapi.mimerGetString8,
-                 18: mimerapi.mimerGetString8,
-                 19: mimerapi.mimerGetString8,
-                 20: mimerapi.mimerGetString8,
-                 21: mimerapi.mimerGetString8,
-                 22: mimerapi.mimerGetString8,
-                 23: mimerapi.mimerGetString8,
-                 24: mimerapi.mimerGetString8,
-                 25: mimerapi.mimerGetString8,
-                 26: mimerapi.mimerGetString8,
-                 27: mimerapi.mimerGetString8,
-                 34: mimerapi.mimerGetBinary,
-                 35: mimerapi.mimerGetBinary,
-                 39: mimerapi.mimerGetString8,
-                 40: mimerapi.mimerGetString8,
-                 42: mimerapi.mimerGetBoolean,
-                 48: mimerapi.mimerGetInt32,
-                 50: mimerapi.mimerGetInt32,
-                 52: mimerapi.mimerGetInt64,
-                 63: mimerapi.mimerGetString8,
-                 56: mimerapi.mimerGetDouble,
-                 54: mimerapi.mimerGetFloat,
-                 57: mimerapi.mimerGetBlobData,
-                 58: mimerapi.mimerGetNclobData8,
-                 59: mimerapi.mimerGetNclobData8,
-                 8104: _pythonGetUUID,
-    }
-
-    set_funcs = {1: mimerapi.mimerSetString8,
-                 2: _pythonSetDecimal,
-                 31: _pythonSetDecimal,
-                 3: _pythonSetInt,
-                 4: _pythonSetDecimalF,
-                 6: mimerapi.mimerSetInt32,
-                 10: mimerapi.mimerSetDouble,
-                 11: mimerapi.mimerSetString8,
-                 12: mimerapi.mimerSetString8,
-                 13: mimerapi.mimerSetString8,
-                 14: mimerapi.mimerSetString8,
-                 15: mimerapi.mimerSetString8,
-                 16: mimerapi.mimerSetString8,
-                 17: mimerapi.mimerSetString8,
-                 18: mimerapi.mimerSetString8,
-                 19: mimerapi.mimerSetString8,
-                 20: mimerapi.mimerSetString8,
-                 21: mimerapi.mimerSetString8,
-                 22: mimerapi.mimerSetString8,
-                 23: mimerapi.mimerSetString8,
-                 24: mimerapi.mimerSetString8,
-                 25: mimerapi.mimerSetString8,
-                 26: mimerapi.mimerSetString8,
-                 27: mimerapi.mimerSetString8,
-                 34: mimerapi.mimerSetBinary,
-                 35: mimerapi.mimerSetBinary,
-                 39: mimerapi.mimerSetString8,
-                 40: mimerapi.mimerSetString8,
-                 42: mimerapi.mimerSetBoolean,
-                 48: mimerapi.mimerSetInt32,
-                 50: mimerapi.mimerSetInt32,
-                 52: mimerapi.mimerSetInt64,
-                 63: mimerapi.mimerSetString8,
-                 56: mimerapi.mimerSetDouble,
-                 54: mimerapi.mimerSetFloat,
-                 57: mimerapi.mimerSetBlobData,
-                 58: mimerapi.mimerSetNclobData8,
-                 59: mimerapi.mimerSetNclobData8,
-                 501: mimerapi.mimerSetNull,
-                 8104: _pythonSetUUID,
-    }
-
-_define_funcs()
-
-class Cursor:
-    """
-        MimerSQL Cursor.
-
-        The class cursor is used to execute MimerSQL statements and manage data result sets.
-
-    """
-
-    def __init__(self, connection, session):
-        """
-            Creates a MimerPy cursor.
-
-            session
-                reference to MimerSession sessionhandle.
-
-        """
-        self.connection = connection
-        self.arraysize = 1
-        self.rowcount = -1
-        self.errorhandler = connection.errorhandler
-        self.messages = []
-        self.description = None
-
-        self._number_of_parameters = None
-        self._number_of_columns = None
-        self._last_query = None
-        self._DDL_rc_value = None
-        self._column_type = []
-
-        self.__session = session
-        self.__statement = None
-        self.__mimcursor = False
-
-    def __enter__(self):
-        self.__check_if_open()
-        return self
-
-    def __exit__(self, type, value, traceback):
-        self.connection.commit()
-        self.close()
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        self.__check_if_open()
-        return_value = self.fetchone()
-        if return_value == []:
-            raise StopIteration
-        return return_value
-
-    def __del__(self):
-        self.close()
-
-    def close(self):
-        """
-            Closes the cursor.
-
-            From this point onwards the cursor is unusable and a
-            ProgrammingError is raised if any operations are attempted
-            on the connection.
-
-        """
-        self.__close_statement()
-        self.__session = None
-
-    def execute(self, *arg):
-        """
-            Executes a database operation.
-
-            arg
-                query to execute
-
-            Executes a database operation.
-
-        """
-        rc_value = 0
-        self.__check_if_open()
-        self.__check_for_transaction()
-        parameter_markers = ()
-
-        # I would like to look over this at some point, the type control is not ideal - Erik 2018-10
-        if (len(arg) > 1):
-            if (isinstance(arg[1], dict)):
-                parameter_markers = arg[1]
-            elif (not isinstance(arg[1], tuple) and (not isinstance(arg[1], list))):
-                parameter_markers = [arg[1]]
-            else:
-                parameter_markers = arg[1]
-        query = arg[0]
-
-        # If same query is used twice there is not need for a new statement
-        if (query != self._last_query or self.__mimcursor):
-            self.__close_statement()
-            values = mimerapi.mimerBeginStatement8(self.__session, query, 0)
-            rc_value = values[0]
-            self._DDL_rc_value = values[0]
-
-            # -24005 indicates a DDL statement
-            if (self._DDL_rc_value != -24005):
-                self.__check_mimerapi_error(rc_value, self.__session)
-                self.__statement = values[1]
-
-        self._last_query = query
-
-        # Return value -24005 is given when a DDL query query is passed through
-        # mimerBeginStatementC.
-        if (self._DDL_rc_value == -24005):
-            self.connection.transaction = False
-            self.messages = []
-            rc_value = mimerapi.mimerExecuteStatement8(self.__session, query)
-            self.__check_mimerapi_error(rc_value, self.__session)
-        else:
-            rc_value = mimerapi.mimerParameterCount(self.__statement)
-            self.__check_mimerapi_error(rc_value, self.__statement)
-
-            # Return value of mimerParameterCount = 0 implies a query with no
-            # parameters.
-            if (rc_value > 0):
-                self._number_of_parameters = rc_value
-                try:
-
-                    if (len(parameter_markers) < self._number_of_parameters):
-                        self.__raise_exception(-25013)
-
-                    # Column number starts a 1
-                    for cur_column in range(1, self._number_of_parameters + 1):
-                        parameter_type = mimerapi.mimerParameterType(
-                            self.__statement, cur_column)
-                        self.__check_mimerapi_error(
-                            parameter_type, self.__statement)
-
-                        if (isinstance(parameter_markers, dict)):
-                            rc_value, parameter_name = mimerapi.mimerParameterName8(
-                                self.__statement, cur_column)
-                            self.__check_mimerapi_error(
-                                rc_value, self.__statement)
-                            if parameter_name in parameter_markers:
-                                parameter = parameter_markers.get(
-                                    parameter_name)
-                                if (parameter == None):
-                                    parameter_type = 501
-                                rc_value = set_funcs[parameter_type](
-                                    self.__statement, cur_column, parameter)
-                            else:
-                                # self.__raise_exception(-25012,str(parameter_name))
-                                pass  # Skipping keys in dictionary that does not match with any column
-                        else:
-                            # If the parameter marker is None, we use mimerSetNull
-                            try:
-                                if (parameter_markers[cur_column - 1] == None):
-                                    parameter_type = 501
-                            except TypeError:
-                                # End up here when invalid parameters are used
-                                self.__raise_exception(-25013)
-                            rc_value = set_funcs[parameter_type](self.__statement,
-                                                                cur_column, parameter_markers[cur_column - 1])
-                        self.__check_mimerapi_error(rc_value, self.__statement)
-
-                # Catching error for errorhandler
-                except KeyError as e:
-                    self.__raise_exception(-25020, exception=e)  # &&&& ??
-                # Catching error for errorhandler
-                except TypeError as e:
-                    # End up here when invalid parameters are used¨
-                    self.__raise_exception(-25020, exception=e)
-                # Catching error for errorhandler
-                except OverflowError as e:
-                    self.__raise_exception(-25020, exception=e)
-
-            self.__check_mimerapi_error(rc_value, self.__statement)
-            rc_value = mimerapi.mimerColumnCount(self.__statement)
-
-            # Return value of mimerColumnCount <= 0 implies a query with no
-            # result set.
-            if (rc_value <= 0):
-                self.__check_mimerapi_error(rc_value, self.__statement)
-                self.messages = []
-                rc_value = mimerapi.mimerExecute(self.__statement)
-                self.__check_mimerapi_error(rc_value, self.__statement)
-                self.rowcount = rc_value
-            else:
-                # Return value of mimerColumnCount > 0 implies a query with a
-                # result set.
-                self.rowcount = rc_value
-                self._number_of_columns = rc_value
-                rc_value = mimerapi.mimerOpenCursor(self.__statement)
-                self.__check_mimerapi_error(rc_value, self.__statement)
-                self.__mimcursor = True
-                description = collections.namedtuple('Column_description',
-                                                     'name type_code display_size internal_size precision scale null_ok')
-                self.description = ()
-                self._column_type = []
-                for cur_column in range(1, self._number_of_columns + 1):
-                    func_tuple = mimerapi.mimerColumnName8(
-                        self.__statement, cur_column)
-                    rc_value = func_tuple[0]
-                    self.__check_mimerapi_error(rc_value, self.__statement)
-                    name = func_tuple[1]
-                    rc_value = mimerapi.mimerColumnType(
-                        self.__statement, cur_column)
-                    self.__check_mimerapi_error(rc_value, self.__statement)
-                    self._column_type.append(rc_value)
-                    type_code = rc_value
-                    self.description = self.description + (description(name=name,
-                                                                       type_code=type_code,
-                                                                       display_size=None,
-                                                                       internal_size=None,
-                                                                       precision=None,
-                                                                       scale=None,
-                                                                       null_ok=None),)
-
-    def executemany(self, query, params):
-        """
-            Executes a database operation.
-
-            query
-                query with parameter markers to execute.
-
-            params
-                sequence of parameters.
-
-            Executes a database operation against all parameter sequences or mappings
-            found in params.
-
-        """
-        self.__check_if_open()
-        self.__check_for_transaction()
-        self._last_query = None
-        self.rowcount = 0
-        rc_value = 0
-        values = []
-
-        if isinstance(params, GeneratorType):
-            tmp_params = []
-            for i in params:
-                tmp_params.append(i)
-            params = tmp_params
-
-        # I would like to look over this at some point
-        # Checking for invalid parameter structure
-        if (not isinstance(params, tuple) and not isinstance(params, list)):
-            self.__raise_exception(-25013)
-        # else:
-        #    if (not isinstance(params[0], tuple) and not isinstance(params[0], dict)):
-        #        self.__raise_exception(-25013)
-
-        self.__close_statement()
-        values = mimerapi.mimerBeginStatement8(self.__session, query, 0)
-        rc_value = values[0]
-
-        self.__check_mimerapi_error(rc_value, self.__session)
-        self.__statement = values[1]
-        self.__check_mimerapi_error(rc_value, self.__statement)
-
-        rc_value = mimerapi.mimerParameterCount(self.__statement)
-        self._number_of_parameters = rc_value
-        self.__check_mimerapi_error(rc_value, self.__statement)
-
-        try:
-            for laps in range(0, len(params)):
-                cur_param = params[laps]
-
-                # Column number starts a 1
-                for cur_column in range(1, self._number_of_parameters + 1):
-                    parameter_type = mimerapi.mimerParameterType(
-                        self.__statement, cur_column)
-                    self.__check_mimerapi_error(
-                        parameter_type, self.__statement)
-
-                    if (isinstance(cur_param, dict)):
-                        rc_value, parameter_name = mimerapi.mimerParameterName8(
-                            self.__statement, cur_column)
-                        self.__check_mimerapi_error(rc_value, self.__statement)
-                        if parameter_name in cur_param:
-                            parameter = cur_param.get(parameter_name)
-                            if (parameter == None):
-                                parameter_type = 501
-                            rc_value = set_funcs[parameter_type](
-                                self.__statement, cur_column, parameter)
-                        else:
-                            #self.__raise_exception(-25012, str(parameter_name))
-                            pass  # Skipping keys in dictionary that does not match with any column
-                    else:
-                        # If the parameter marker is None, we use mimerSetNull
-                        try:
-                            if (cur_param[cur_column - 1] == None):
-                                parameter_type = 501
-                        except TypeError as e:
-                            # End up here when invalid parameters are used
-                            self.__raise_exception(-25013)
-                        rc_value = set_funcs[parameter_type](self.__statement,
-                                                             cur_column, cur_param[cur_column - 1])
-                self.messages = []
-
-                # Batching after all parameters are set
-                if (laps != len(params) - 1):
-                    rc_value = mimerapi.mimerAddBatch(self.__statement)
-                    self.__check_mimerapi_error(rc_value, self.__statement)
-                self.rowcount = self.rowcount + rc_value
-
-            rc_value = mimerapi.mimerExecute(self.__statement)
-            self.__check_mimerapi_error(rc_value, self.__statement)
-
-        # Catching error for errorhandler
-        except TypeError as e:
-            self.__raise_exception(-25020, exception=e)
-        # Catching error for errorhandler
-        except OverflowError as e:
-            self.__raise_exception(-25020, exception=e)
-
-    def fetchone(self):
-        """
-            Fetch next row of a query result set.
-
-            The row is returned as a tuple. If no more data is available,
-            None is returned. If fetchone is called and the previous call
-            to execute did not produce a result set, a ProgrammingError
-            is raised.
-
-        """
-        self.__check_if_open()
-        self.__check_for_transaction()
-
-        if (not self.__mimcursor):
-            self.__raise_exception(-25014)
-
-        rc_value = mimerapi.mimerFetch(self.__statement)
-        self.__check_mimerapi_error(rc_value, self.__statement)
-        return_tuple = ()
-
-        # Return value of mimerFetch == 100 implies end of result set
-        if (rc_value == 100):
-            return []
-
-        for cur_column in range(1, self._number_of_columns + 1):
-            func_tuple = get_funcs[self._column_type[cur_column - 1]
-                                   ](self.__statement, cur_column)
-            self.__check_mimerapi_error(func_tuple[0], self.__statement)
-
-            # Conversion from C int to Python boolean
-            if (rc_value == 42 and not func_tuple[1] == None):
-                if (func_tuple[1] == 0):
-                    return_tuple = return_tuple + (False,)
-                else:
-                    return_tuple = return_tuple + (True,)
-            else:
-                return_tuple = return_tuple + (func_tuple[1],)
-        return return_tuple
-
-    def fetchmany(self, *arg):
-        """Fetch next row of a query result set.
-
-        arg
-            sets the arraysize
-
-        The number of rows to fetch per call is specified by the parameter.
-        If it is not given, the cursor's arraysize determines the number of
-        rows to be fetched. The method should try to fetch as many rows as
-        indicated by the size parameter. If this is not possible due to the
-        specified number of rows not being available, fewer rows may be returned.
-        Arraysize is retained after each call to fetchmany.
-
-        """
-        values = []
-        return_tuple = ()
-
-        self.__check_if_open()
-        self.__check_for_transaction()
-
-        if (not self.__mimcursor):
-            self.__raise_exception(-25014)
-
-        # If arg is provided, arraysize is set
-        if (len(arg) > 0):
-            self.arraysize = arg[0]
-
-        fetch_length = self.arraysize
-        rc_value = mimerapi.mimerFetch(self.__statement)
-        fetch_value = rc_value
-
-        while (fetch_value != 100 and fetch_length > 0):
-            self.__check_mimerapi_error(fetch_value, self.__statement)
-            return_tuple = ()
-
-            # Column number starts a 1
-            for cur_column in range(1, self._number_of_columns + 1):
-                func_tuple = get_funcs[self._column_type[cur_column - 1]
-                                       ](self.__statement, cur_column)
-                self.__check_mimerapi_error(func_tuple[0], self.__statement)
-
-                # Conversion from C int to Python boolean
-                if (rc_value == 42 and not func_tuple[1] == None):
-                    if (func_tuple[1] == 0):
-                        return_tuple = return_tuple + (False,)
-                    else:
-                        return_tuple = return_tuple + (True,)
-                else:
-                    return_tuple = return_tuple + (func_tuple[1],)
-
-            values.append(return_tuple)
-            fetch_length = fetch_length - 1
-            if(fetch_length > 0):
-                fetch_value = mimerapi.mimerFetch(self.__statement)
-        return values
-
-    def fetchall(self):
-        """
-            Fetch all (remaining) row of a query result set.
-
-            The rows are returned as a list of tuples. If no more data is
-            available, an empty list is returned. If fetchall is called and
-            the previous call to execute did not produce a result set,
-            a ProgrammingError is raised.
-
-        """
-        self.__check_if_open()
-        self.__check_for_transaction()
-        if (not self.__mimcursor):
-            self.__raise_exception(-25014)
-        values = []
-        rc_value = mimerapi.mimerFetch(self.__statement)
-        fetch_value = rc_value
-
-        while (fetch_value != 100):
-            self.__check_mimerapi_error(fetch_value, self.__statement)
-            return_tuple = ()
-
-            # Column number starts a 1
-            for cur_column in range(1, self._number_of_columns + 1):
-                func_tuple = get_funcs[self._column_type[cur_column - 1]
-                                       ](self.__statement, cur_column)
-                self.__check_mimerapi_error(func_tuple[0], self.__statement)
-
-                # Conversion from C int to Python boolean
-                if (rc_value == 42 and not func_tuple[1] == None):
-                    if (func_tuple[1] == 0):
-                        return_tuple = return_tuple + (False,)
-                    else:
-                        return_tuple = return_tuple + (True,)
-                else:
-                    return_tuple = return_tuple + (func_tuple[1],)
-            values.append(return_tuple)
-            fetch_value = mimerapi.mimerFetch(self.__statement)
-        return values
-
-    def setinputsizes(self):
-        """Does nothing but required by the DB API."""
-
-    def setoutputsizes(self):
-        """Does nothing but required by the DB API."""
-
-    def next(self):
-        """
-            Returns the next row in a result set, with the same semantics
-            as fetchone. If there is no more data available in the result
-            set, a StopIteration exception is raised.
-
-        """
-        return_tuple = self.fetchone()
-        if (return_tuple):
-            return return_tuple
-        else:
-            raise StopIteration
-
-    def __close_statement(self):
-        # Private method for closing MimerStatement.
-        if (self.__statement is not None and
-                self.connection._session is not None):
-            rc_value = mimerapi.mimerEndStatement(self.__statement)
-            self.__check_mimerapi_error(rc_value, self.__statement)
-        self.__statement = None
-        self.__mimcursor = False
-
-    def __check_if_open(self):
-        if (self.__session == None):
-            self.__raise_exception(-25015)
-
-    def __check_for_transaction(self):
-        if (not self.connection._transaction and not self.connection.autocommitmode):
-            rc_value = mimerapi.mimerBeginTransaction(self.__session)
-            self.__check_mimerapi_error(rc_value, self.__session)
-            self.connection._transaction = True
-
-    def __raise_exception(self, rc, val=None, exception=None):
-        msg = mimerpy_error[rc]
-        if val is not None:
-            msg = msg % val
-        if exception is None:
-            etup = (rc, msg)
-        else:
-            etup = (rc, msg, exception)
-        self.errorhandler(None, self, get_error_class(rc), etup)
-
-    def __check_mimerapi_error(self, rc, handle):
-        if rc < 0:
-            (ec, ev) = get_mimerapi_exception(rc, handle)
-            self.errorhandler(None, self, ec, ev)
-
-    def nextset(self):
-        self.__raise_exception(-25000)
-
-    def callproc(self):
-        self.__raise_exception(-25000)
-
-
-
-class ScrollCursor(Cursor):
-    """
-        Subclass to the Cursor-class where the cursor can be scrolled to
-        new positions in the result set.
-
-    """
-
-    def __init__(self, connection, session):
-        super(ScrollCursor, self).__init__(connection, session)
-        self.__result_set = None
-        self.rownumber = None
-
-    def execute(self, *arg):
-        """
-            Executes a database operation.
-
-            arg
-                query to execute
-
-            Executes a database operation.
-
-        """
-        super(ScrollCursor, self).execute(*arg)
-
-        # If a resulet set is produced, it is fetched.
-        if (self._Cursor__mimcursor):
-            self.__result_set = super(ScrollCursor, self).fetchall()
-            self.rowcount = len(self.__result_set)
-            self.rownumber = 0
-        else:
-            self.__result_set = None
-
-    def fetchone(self):
-        """
-            Fetch next row of a query result set.
-
-            The row is returned as a tuple. If no more data is available,
-            None is returned. If fetchone is called and the previous call
-            to execute did not produce a result set, a ProgrammingError
-            is raised.
-
-        """
-        self._Cursor__check_if_open()
-        self._Cursor__check_for_transaction()
-
-        if (self.__result_set == None):
-            self._Cursor__raise_exception(-25014)
-        values = ()
-        try:
-            values = values + self.__result_set[self.rownumber]
-            self.rownumber = self.rownumber + 1
-        except IndexError:
-            return []
-        return values
-
-    def fetchmany(self, *arg):
-        """
-            Fetch next row of a query result set.
-
-            arg
-                sets the arraysize
-
-            The number of rows to fetch per call is specified by the parameter.
-            If it is not given, the cursor's arraysize determines the number of
-            rows to be fetched. The method should try to fetch as many rows as
-            indicated by the size parameter. If this is not possible due to the
-            specified number of rows not being available, fewer rows may be returned.
-            Arraysize is retained after each call to fetchmany.
-
-        """
-        self._Cursor__check_if_open()
-        self._Cursor__check_for_transaction()
-
-        if (self.__result_set == None):
-            self._Cursor__raise_exception(-25014)
-
-        if (len(arg) > 0):
-            self.arraysize = arg[0]
-
-        fetch_size = self.arraysize
-        values = []
-
-        while (fetch_size):
-            try:
-                values.append(self.__result_set[self.rownumber])
-                fetch_size = fetch_size - 1
-                self.rownumber = self.rownumber + 1
-            except IndexError:
-                break
-        return values
-
-    def fetchall(self):
-        """
-            Fetch all (remaining) row of a query result set.
-
-            The rows are returned as a list of tuples. If no more data is
-            available, an empty list is returned. If fetchall is called and
-            the previous call to execute did not produce a result set,
-            a ProgrammingError is raised.
-
-        """
-        self._Cursor__check_if_open()
-        self._Cursor__check_for_transaction()
-        values = []
-        if (self.__result_set == None):
-            self._Cursor__raise_exception(-25014)
-        if (not self.rownumber):
-            self.rownumber = len(self.__result_set)
-            return self.__result_set
-        else:
-            values = self.__result_set[self.rownumber:len(self.__result_set)]
-            self.rownumber = len(self.__result_set)
-            return values
-
-    def next(self):
-        """
-            Returns the next row in a result set, with the same semantics
-            as fetchone. If there is no more data available in the result
-            set, a StopIteration exception is raised.
-
-        """
-        self._Cursor__check_if_open()
-        self._Cursor__check_for_transaction()
-
-        if (self.__result_set == None):
-            self._Cursor__raise_exception(-25014)
-        if (self.__result_set == []):
-            return self.__result_set
-
-        values = ()
-        try:
-            values = values + self.__result_set[self.rownumber]
-            self.rownumber = self.rownumber + 1
-        except IndexError:
-            raise StopIteration
-        return values
-
-    def scroll(self, value, mode='relative'):
-        """
-            Method scrolls the cursor to a new position according to the
-            mode of the scroll.
-
-            The mode of the cursor is set to relative by default. This
-            changes the cursor’s position by value number of rows in
-            relation to the current position of the cursor. If mode is
-            set to absolute the cursor is moved value number of rows down
-            from the absolute position.
-
-            If the method is called upon and desired position in the result
-            set does not exist, an IndexError is raised.
-
-        """
-        self._Cursor__check_if_open()
-        self._Cursor__check_for_transaction()
-
-        if (mode == 'relative'):
-            new_row = self.rownumber + value
-            if (new_row >= len(self.__result_set)):
-                raise IndexError
-            else:
-                self.rownumber = new_row
-        elif (mode == 'absolute'):
-            if (value >= len(self.__result_set)):
-                raise IndexError
-            else:
-                self.rownumber = value
-        else:
-            self._Cursor__raise_exception(-25016)
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+from mimerpy.mimPyExceptionHandler import *
+import mimerapi
+import collections, decimal, uuid
+from types import GeneratorType
+
+
+def _pythonSetDecimal(statement, cur_column, parameter):
+    if parameter is None:
+        rc = mimerapi.mimerSetString8(statement, cur_column, parameter)
+    else: 
+        rc = mimerapi.mimerSetString8(statement, cur_column, str(parameter))
+    return rc
+
+def _pythonSetDecimalF(statement, cur_column, parameter):
+    if mimerapi._level >= 2:
+        return _pythonSetDecimal(statement, cur_column, parameter)
+    return -25102
+
+def _pythonGetDecimal(statement, cur_column):
+    rc, val = mimerapi.mimerGetString8(statement, cur_column)
+    if rc >= 0 and val is not None:
+        val = decimal.Decimal(val)
+    return (rc, val)
+
+def _pythonGetDecimalF(statement, cur_column):
+    if mimerapi._level >= 2:
+        return _pythonGetDecimal(statement, cur_column)
+    return (-25102, None)
+
+def _pythonGetInt(statement, col):
+    if mimerapi._level >= 2:
+        rc, val = mimerapi.mimerGetString8(statement, col)
+        if rc >= 0 and val is not None:
+            return (0, int(val))
+        return (rc, None)
+    return mimerapi.mimerGetInt64(statement, col)
+
+def _pythonSetInt(statement, col, val):
+    if mimerapi._level >= 2 and val is not None:
+        return mimerapi.mimerSetString8(statement, col, str(val))
+    return mimerapi.mimerSetInt64(statement, col, val)
+
+def _pythonGetUUID(statement, col):
+    rc, val = mimerapi.mimerGetUUID(statement, col)
+    if rc >= 0 and val is not None:
+        return (0, uuid.UUID(bytes=val))
+    return (rc, None)
+
+def _pythonSetUUID(statement, col, val):
+    return mimerapi.mimerSetUUID(statement, col, val.bytes)
+
+def _define_funcs():
+    global get_funcs
+    global set_funcs
+
+    TYPEID_MASK = 0x40000000
+
+    get_funcs = {1: mimerapi.mimerGetString8,
+                 2: _pythonGetDecimal,
+                 31: _pythonGetDecimal,
+                 3: _pythonGetInt,
+                 4: _pythonGetDecimalF,
+                 6: mimerapi.mimerGetInt32,
+                 10: mimerapi.mimerGetDouble,
+                 11: mimerapi.mimerGetString8,
+                 12: mimerapi.mimerGetString8,
+                 13: mimerapi.mimerGetString8,
+                 14: mimerapi.mimerGetString8,
+                 15: mimerapi.mimerGetString8,
+                 16: mimerapi.mimerGetString8,
+                 17: mimerapi.mimerGetString8,
+                 18: mimerapi.mimerGetString8,
+                 19: mimerapi.mimerGetString8,
+                 20: mimerapi.mimerGetString8,
+                 21: mimerapi.mimerGetString8,
+                 22: mimerapi.mimerGetString8,
+                 23: mimerapi.mimerGetString8,
+                 24: mimerapi.mimerGetString8,
+                 25: mimerapi.mimerGetString8,
+                 26: mimerapi.mimerGetString8,
+                 27: mimerapi.mimerGetString8,
+                 34: mimerapi.mimerGetBinary,
+                 35: mimerapi.mimerGetBinary,
+                 39: mimerapi.mimerGetString8,
+                 40: mimerapi.mimerGetString8,
+                 42: mimerapi.mimerGetBoolean,
+                 48: mimerapi.mimerGetInt32,
+                 50: mimerapi.mimerGetInt32,
+                 52: mimerapi.mimerGetInt64,
+                 63: mimerapi.mimerGetString8,
+                 56: mimerapi.mimerGetDouble,
+                 54: mimerapi.mimerGetFloat,
+                 57: mimerapi.mimerGetBlobData,
+                 58: mimerapi.mimerGetNclobData8,
+                 59: mimerapi.mimerGetNclobData8,
+                 8104: _pythonGetUUID,
+    }
+
+    set_funcs = {1: mimerapi.mimerSetString8,
+                 2: _pythonSetDecimal,
+                 31: _pythonSetDecimal,
+                 3: _pythonSetInt,
+                 4: _pythonSetDecimalF,
+                 6: mimerapi.mimerSetInt32,
+                 10: mimerapi.mimerSetDouble,
+                 11: mimerapi.mimerSetString8,
+                 12: mimerapi.mimerSetString8,
+                 13: mimerapi.mimerSetString8,
+                 14: mimerapi.mimerSetString8,
+                 15: mimerapi.mimerSetString8,
+                 16: mimerapi.mimerSetString8,
+                 17: mimerapi.mimerSetString8,
+                 18: mimerapi.mimerSetString8,
+                 19: mimerapi.mimerSetString8,
+                 20: mimerapi.mimerSetString8,
+                 21: mimerapi.mimerSetString8,
+                 22: mimerapi.mimerSetString8,
+                 23: mimerapi.mimerSetString8,
+                 24: mimerapi.mimerSetString8,
+                 25: mimerapi.mimerSetString8,
+                 26: mimerapi.mimerSetString8,
+                 27: mimerapi.mimerSetString8,
+                 34: mimerapi.mimerSetBinary,
+                 35: mimerapi.mimerSetBinary,
+                 39: mimerapi.mimerSetString8,
+                 40: mimerapi.mimerSetString8,
+                 42: mimerapi.mimerSetBoolean,
+                 48: mimerapi.mimerSetInt32,
+                 50: mimerapi.mimerSetInt32,
+                 52: mimerapi.mimerSetInt64,
+                 63: mimerapi.mimerSetString8,
+                 56: mimerapi.mimerSetDouble,
+                 54: mimerapi.mimerSetFloat,
+                 57: mimerapi.mimerSetBlobData,
+                 58: mimerapi.mimerSetNclobData8,
+                 59: mimerapi.mimerSetNclobData8,
+                 501: mimerapi.mimerSetNull,
+                 8104: _pythonSetUUID,
+    }
+
+_define_funcs()
+
+class Cursor:
+    """
+        MimerSQL Cursor.
+
+        The class cursor is used to execute MimerSQL statements and manage data result sets.
+
+    """
+
+    def __init__(self, connection, session):
+        """
+            Creates a MimerPy cursor.
+
+            session
+                reference to MimerSession sessionhandle.
+
+        """
+        self.connection = connection
+        self.arraysize = 1
+        self.rowcount = -1
+        self.errorhandler = connection.errorhandler
+        self.messages = []
+        self.description = None
+
+        self._number_of_parameters = None
+        self._number_of_columns = None
+        self._last_query = None
+        self._DDL_rc_value = None
+        self._column_type = []
+
+        self.__session = session
+        self.__statement = None
+        self.__mimcursor = False
+
+    def __enter__(self):
+        self.__check_if_open()
+        return self
+
+    def __exit__(self, type, value, traceback):
+        self.connection.commit()
+        self.close()
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        self.__check_if_open()
+        return_value = self.fetchone()
+        if return_value == []:
+            raise StopIteration
+        return return_value
+
+    def __del__(self):
+        self.close()
+
+    def close(self):
+        """
+            Closes the cursor.
+
+            From this point onwards the cursor is unusable and a
+            ProgrammingError is raised if any operations are attempted
+            on the connection.
+
+        """
+        self.__close_statement()
+        self.__session = None
+
+    def execute(self, *arg):
+        """
+            Executes a database operation.
+
+            arg
+                query to execute
+
+            Executes a database operation.
+
+        """
+        rc_value = 0
+        self.__check_if_open()
+        self.__check_for_transaction()
+        parameter_markers = ()
+
+        # I would like to look over this at some point, the type control is not ideal - Erik 2018-10
+        if (len(arg) > 1):
+            if (isinstance(arg[1], dict)):
+                parameter_markers = arg[1]
+            elif (not isinstance(arg[1], tuple) and (not isinstance(arg[1], list))):
+                parameter_markers = [arg[1]]
+            else:
+                parameter_markers = arg[1]
+        query = arg[0]
+
+        # If same query is used twice there is not need for a new statement
+        if (query != self._last_query or self.__mimcursor):
+            self.__close_statement()
+            values = mimerapi.mimerBeginStatement8(self.__session, query, 0)
+            rc_value = values[0]
+            self._DDL_rc_value = values[0]
+
+            # -24005 indicates a DDL statement
+            if (self._DDL_rc_value != -24005):
+                self.__check_mimerapi_error(rc_value, self.__session)
+                self.__statement = values[1]
+
+        self._last_query = query
+
+        # Return value -24005 is given when a DDL query query is passed through
+        # mimerBeginStatementC.
+        if (self._DDL_rc_value == -24005):
+            self.connection.transaction = False
+            self.messages = []
+            rc_value = mimerapi.mimerExecuteStatement8(self.__session, query)
+            self.__check_mimerapi_error(rc_value, self.__session)
+        else:
+            rc_value = mimerapi.mimerParameterCount(self.__statement)
+            self.__check_mimerapi_error(rc_value, self.__statement)
+
+            # Return value of mimerParameterCount = 0 implies a query with no
+            # parameters.
+            if (rc_value > 0):
+                self._number_of_parameters = rc_value
+                try:
+
+                    if (len(parameter_markers) < self._number_of_parameters):
+                        self.__raise_exception(-25013)
+
+                    # Column number starts a 1
+                    for cur_column in range(1, self._number_of_parameters + 1):
+                        parameter_type = mimerapi.mimerParameterType(
+                            self.__statement, cur_column)
+                        self.__check_mimerapi_error(
+                            parameter_type, self.__statement)
+
+                        if (isinstance(parameter_markers, dict)):
+                            rc_value, parameter_name = mimerapi.mimerParameterName8(
+                                self.__statement, cur_column)
+                            self.__check_mimerapi_error(
+                                rc_value, self.__statement)
+                            if parameter_name in parameter_markers:
+                                parameter = parameter_markers.get(
+                                    parameter_name)
+                                if (parameter == None):
+                                    parameter_type = 501
+                                rc_value = set_funcs[parameter_type](
+                                    self.__statement, cur_column, parameter)
+                            else:
+                                # self.__raise_exception(-25012,str(parameter_name))
+                                pass  # Skipping keys in dictionary that does not match with any column
+                        else:
+                            # If the parameter marker is None, we use mimerSetNull
+                            try:
+                                if (parameter_markers[cur_column - 1] == None):
+                                    parameter_type = 501
+                            except TypeError:
+                                # End up here when invalid parameters are used
+                                self.__raise_exception(-25013)
+                            rc_value = set_funcs[parameter_type](self.__statement,
+                                                                cur_column, parameter_markers[cur_column - 1])
+                        self.__check_mimerapi_error(rc_value, self.__statement)
+
+                # Catching error for errorhandler
+                except KeyError as e:
+                    self.__raise_exception(-25020, exception=e)  # &&&& ??
+                # Catching error for errorhandler
+                except TypeError as e:
+                    # End up here when invalid parameters are used¨
+                    self.__raise_exception(-25020, exception=e)
+                # Catching error for errorhandler
+                except OverflowError as e:
+                    self.__raise_exception(-25020, exception=e)
+
+            self.__check_mimerapi_error(rc_value, self.__statement)
+            rc_value = mimerapi.mimerColumnCount(self.__statement)
+
+            # Return value of mimerColumnCount <= 0 implies a query with no
+            # result set.
+            if (rc_value <= 0):
+                self.__check_mimerapi_error(rc_value, self.__statement)
+                self.messages = []
+                rc_value = mimerapi.mimerExecute(self.__statement)
+                self.__check_mimerapi_error(rc_value, self.__statement)
+                self.rowcount = rc_value
+            else:
+                # Return value of mimerColumnCount > 0 implies a query with a
+                # result set.
+                self.rowcount = rc_value
+                self._number_of_columns = rc_value
+                rc_value = mimerapi.mimerOpenCursor(self.__statement)
+                self.__check_mimerapi_error(rc_value, self.__statement)
+                self.__mimcursor = True
+                description = collections.namedtuple('Column_description',
+                                                     'name type_code display_size internal_size precision scale null_ok')
+                self.description = ()
+                self._column_type = []
+                for cur_column in range(1, self._number_of_columns + 1):
+                    func_tuple = mimerapi.mimerColumnName8(
+                        self.__statement, cur_column)
+                    rc_value = func_tuple[0]
+                    self.__check_mimerapi_error(rc_value, self.__statement)
+                    name = func_tuple[1]
+                    rc_value = mimerapi.mimerColumnType(
+                        self.__statement, cur_column)
+                    self.__check_mimerapi_error(rc_value, self.__statement)
+                    self._column_type.append(rc_value)
+                    type_code = rc_value
+                    self.description = self.description + (description(name=name,
+                                                                       type_code=type_code,
+                                                                       display_size=None,
+                                                                       internal_size=None,
+                                                                       precision=None,
+                                                                       scale=None,
+                                                                       null_ok=None),)
+
+    def executemany(self, query, params):
+        """
+            Executes a database operation.
+
+            query
+                query with parameter markers to execute.
+
+            params
+                sequence of parameters.
+
+            Executes a database operation against all parameter sequences or mappings
+            found in params.
+
+        """
+        self.__check_if_open()
+        self.__check_for_transaction()
+        self._last_query = None
+        self.rowcount = 0
+        rc_value = 0
+        values = []
+
+        if isinstance(params, GeneratorType):
+            tmp_params = []
+            for i in params:
+                tmp_params.append(i)
+            params = tmp_params
+
+        # I would like to look over this at some point
+        # Checking for invalid parameter structure
+        if (not isinstance(params, tuple) and not isinstance(params, list)):
+            self.__raise_exception(-25013)
+        # else:
+        #    if (not isinstance(params[0], tuple) and not isinstance(params[0], dict)):
+        #        self.__raise_exception(-25013)
+
+        self.__close_statement()
+        values = mimerapi.mimerBeginStatement8(self.__session, query, 0)
+        rc_value = values[0]
+
+        self.__check_mimerapi_error(rc_value, self.__session)
+        self.__statement = values[1]
+        self.__check_mimerapi_error(rc_value, self.__statement)
+
+        rc_value = mimerapi.mimerParameterCount(self.__statement)
+        self._number_of_parameters = rc_value
+        self.__check_mimerapi_error(rc_value, self.__statement)
+
+        try:
+            for laps in range(0, len(params)):
+                cur_param = params[laps]
+
+                # Column number starts a 1
+                for cur_column in range(1, self._number_of_parameters + 1):
+                    parameter_type = mimerapi.mimerParameterType(
+                        self.__statement, cur_column)
+                    self.__check_mimerapi_error(
+                        parameter_type, self.__statement)
+
+                    if (isinstance(cur_param, dict)):
+                        rc_value, parameter_name = mimerapi.mimerParameterName8(
+                            self.__statement, cur_column)
+                        self.__check_mimerapi_error(rc_value, self.__statement)
+                        if parameter_name in cur_param:
+                            parameter = cur_param.get(parameter_name)
+                            if (parameter == None):
+                                parameter_type = 501
+                            rc_value = set_funcs[parameter_type](
+                                self.__statement, cur_column, parameter)
+                        else:
+                            #self.__raise_exception(-25012, str(parameter_name))
+                            pass  # Skipping keys in dictionary that does not match with any column
+                    else:
+                        # If the parameter marker is None, we use mimerSetNull
+                        try:
+                            if (cur_param[cur_column - 1] == None):
+                                parameter_type = 501
+                        except TypeError as e:
+                            # End up here when invalid parameters are used
+                            self.__raise_exception(-25013)
+                        rc_value = set_funcs[parameter_type](self.__statement,
+                                                             cur_column, cur_param[cur_column - 1])
+                self.messages = []
+
+                # Batching after all parameters are set
+                if (laps != len(params) - 1):
+                    rc_value = mimerapi.mimerAddBatch(self.__statement)
+                    self.__check_mimerapi_error(rc_value, self.__statement)
+                self.rowcount = self.rowcount + rc_value
+
+            rc_value = mimerapi.mimerExecute(self.__statement)
+            self.__check_mimerapi_error(rc_value, self.__statement)
+
+        # Catching error for errorhandler
+        except TypeError as e:
+            self.__raise_exception(-25020, exception=e)
+        # Catching error for errorhandler
+        except OverflowError as e:
+            self.__raise_exception(-25020, exception=e)
+
+    def fetchone(self):
+        """
+            Fetch next row of a query result set.
+
+            The row is returned as a tuple. If no more data is available,
+            None is returned. If fetchone is called and the previous call
+            to execute did not produce a result set, a ProgrammingError
+            is raised.
+
+        """
+        self.__check_if_open()
+        self.__check_for_transaction()
+
+        if (not self.__mimcursor):
+            self.__raise_exception(-25014)
+
+        rc_value = mimerapi.mimerFetch(self.__statement)
+        self.__check_mimerapi_error(rc_value, self.__statement)
+        return_tuple = ()
+
+        # Return value of mimerFetch == 100 implies end of result set
+        if (rc_value == 100):
+            return []
+
+        for cur_column in range(1, self._number_of_columns + 1):
+            func_tuple = get_funcs[self._column_type[cur_column - 1]
+                                   ](self.__statement, cur_column)
+            self.__check_mimerapi_error(func_tuple[0], self.__statement)
+
+            # Conversion from C int to Python boolean
+            if (rc_value == 42 and not func_tuple[1] == None):
+                if (func_tuple[1] == 0):
+                    return_tuple = return_tuple + (False,)
+                else:
+                    return_tuple = return_tuple + (True,)
+            else:
+                return_tuple = return_tuple + (func_tuple[1],)
+        return return_tuple
+
+    def fetchmany(self, *arg):
+        """Fetch next row of a query result set.
+
+        arg
+            sets the arraysize
+
+        The number of rows to fetch per call is specified by the parameter.
+        If it is not given, the cursor's arraysize determines the number of
+        rows to be fetched. The method should try to fetch as many rows as
+        indicated by the size parameter. If this is not possible due to the
+        specified number of rows not being available, fewer rows may be returned.
+        Arraysize is retained after each call to fetchmany.
+
+        """
+        values = []
+        return_tuple = ()
+
+        self.__check_if_open()
+        self.__check_for_transaction()
+
+        if (not self.__mimcursor):
+            self.__raise_exception(-25014)
+
+        # If arg is provided, arraysize is set
+        if (len(arg) > 0):
+            self.arraysize = arg[0]
+
+        fetch_length = self.arraysize
+        rc_value = mimerapi.mimerFetch(self.__statement)
+        fetch_value = rc_value
+
+        while (fetch_value != 100 and fetch_length > 0):
+            self.__check_mimerapi_error(fetch_value, self.__statement)
+            return_tuple = ()
+
+            # Column number starts a 1
+            for cur_column in range(1, self._number_of_columns + 1):
+                func_tuple = get_funcs[self._column_type[cur_column - 1]
+                                       ](self.__statement, cur_column)
+                self.__check_mimerapi_error(func_tuple[0], self.__statement)
+
+                # Conversion from C int to Python boolean
+                if (rc_value == 42 and not func_tuple[1] == None):
+                    if (func_tuple[1] == 0):
+                        return_tuple = return_tuple + (False,)
+                    else:
+                        return_tuple = return_tuple + (True,)
+                else:
+                    return_tuple = return_tuple + (func_tuple[1],)
+
+            values.append(return_tuple)
+            fetch_length = fetch_length - 1
+            if(fetch_length > 0):
+                fetch_value = mimerapi.mimerFetch(self.__statement)
+        return values
+
+    def fetchall(self):
+        """
+            Fetch all (remaining) row of a query result set.
+
+            The rows are returned as a list of tuples. If no more data is
+            available, an empty list is returned. If fetchall is called and
+            the previous call to execute did not produce a result set,
+            a ProgrammingError is raised.
+
+        """
+        self.__check_if_open()
+        self.__check_for_transaction()
+        if (not self.__mimcursor):
+            self.__raise_exception(-25014)
+        values = []
+        rc_value = mimerapi.mimerFetch(self.__statement)
+        fetch_value = rc_value
+
+        while (fetch_value != 100):
+            self.__check_mimerapi_error(fetch_value, self.__statement)
+            return_tuple = ()
+
+            # Column number starts a 1
+            for cur_column in range(1, self._number_of_columns + 1):
+                func_tuple = get_funcs[self._column_type[cur_column - 1]
+                                       ](self.__statement, cur_column)
+                self.__check_mimerapi_error(func_tuple[0], self.__statement)
+
+                # Conversion from C int to Python boolean
+                if (rc_value == 42 and not func_tuple[1] == None):
+                    if (func_tuple[1] == 0):
+                        return_tuple = return_tuple + (False,)
+                    else:
+                        return_tuple = return_tuple + (True,)
+                else:
+                    return_tuple = return_tuple + (func_tuple[1],)
+            values.append(return_tuple)
+            fetch_value = mimerapi.mimerFetch(self.__statement)
+        return values
+
+    def setinputsizes(self):
+        """Does nothing but required by the DB API."""
+
+    def setoutputsizes(self):
+        """Does nothing but required by the DB API."""
+
+    def next(self):
+        """
+            Returns the next row in a result set, with the same semantics
+            as fetchone. If there is no more data available in the result
+            set, a StopIteration exception is raised.
+
+        """
+        return_tuple = self.fetchone()
+        if (return_tuple):
+            return return_tuple
+        else:
+            raise StopIteration
+
+    def __close_statement(self):
+        # Private method for closing MimerStatement.
+        if (self.__statement is not None and
+                self.connection._session is not None):
+            rc_value = mimerapi.mimerEndStatement(self.__statement)
+            self.__check_mimerapi_error(rc_value, self.__statement)
+        self.__statement = None
+        self.__mimcursor = False
+
+    def __check_if_open(self):
+        if (self.__session == None):
+            self.__raise_exception(-25015)
+
+    def __check_for_transaction(self):
+        if (not self.connection._transaction and not self.connection.autocommitmode):
+            rc_value = mimerapi.mimerBeginTransaction(self.__session)
+            self.__check_mimerapi_error(rc_value, self.__session)
+            self.connection._transaction = True
+
+    def __raise_exception(self, rc, val=None, exception=None):
+        msg = mimerpy_error[rc]
+        if val is not None:
+            msg = msg % val
+        if exception is None:
+            etup = (rc, msg)
+        else:
+            etup = (rc, msg, exception)
+        self.errorhandler(None, self, get_error_class(rc), etup)
+
+    def __check_mimerapi_error(self, rc, handle):
+        if rc < 0:
+            (ec, ev) = get_mimerapi_exception(rc, handle)
+            self.errorhandler(None, self, ec, ev)
+
+    def nextset(self):
+        self.__raise_exception(-25000)
+
+    def callproc(self):
+        self.__raise_exception(-25000)
+
+
+
+class ScrollCursor(Cursor):
+    """
+        Subclass to the Cursor-class where the cursor can be scrolled to
+        new positions in the result set.
+
+    """
+
+    def __init__(self, connection, session):
+        super(ScrollCursor, self).__init__(connection, session)
+        self.__result_set = None
+        self.rownumber = None
+
+    def execute(self, *arg):
+        """
+            Executes a database operation.
+
+            arg
+                query to execute
+
+            Executes a database operation.
+
+        """
+        super(ScrollCursor, self).execute(*arg)
+
+        # If a resulet set is produced, it is fetched.
+        if (self._Cursor__mimcursor):
+            self.__result_set = super(ScrollCursor, self).fetchall()
+            self.rowcount = len(self.__result_set)
+            self.rownumber = 0
+        else:
+            self.__result_set = None
+
+    def fetchone(self):
+        """
+            Fetch next row of a query result set.
+
+            The row is returned as a tuple. If no more data is available,
+            None is returned. If fetchone is called and the previous call
+            to execute did not produce a result set, a ProgrammingError
+            is raised.
+
+        """
+        self._Cursor__check_if_open()
+        self._Cursor__check_for_transaction()
+
+        if (self.__result_set == None):
+            self._Cursor__raise_exception(-25014)
+        values = ()
+        try:
+            values = values + self.__result_set[self.rownumber]
+            self.rownumber = self.rownumber + 1
+        except IndexError:
+            return []
+        return values
+
+    def fetchmany(self, *arg):
+        """
+            Fetch next row of a query result set.
+
+            arg
+                sets the arraysize
+
+            The number of rows to fetch per call is specified by the parameter.
+            If it is not given, the cursor's arraysize determines the number of
+            rows to be fetched. The method should try to fetch as many rows as
+            indicated by the size parameter. If this is not possible due to the
+            specified number of rows not being available, fewer rows may be returned.
+            Arraysize is retained after each call to fetchmany.
+
+        """
+        self._Cursor__check_if_open()
+        self._Cursor__check_for_transaction()
+
+        if (self.__result_set == None):
+            self._Cursor__raise_exception(-25014)
+
+        if (len(arg) > 0):
+            self.arraysize = arg[0]
+
+        fetch_size = self.arraysize
+        values = []
+
+        while (fetch_size):
+            try:
+                values.append(self.__result_set[self.rownumber])
+                fetch_size = fetch_size - 1
+                self.rownumber = self.rownumber + 1
+            except IndexError:
+                break
+        return values
+
+    def fetchall(self):
+        """
+            Fetch all (remaining) row of a query result set.
+
+            The rows are returned as a list of tuples. If no more data is
+            available, an empty list is returned. If fetchall is called and
+            the previous call to execute did not produce a result set,
+            a ProgrammingError is raised.
+
+        """
+        self._Cursor__check_if_open()
+        self._Cursor__check_for_transaction()
+        values = []
+        if (self.__result_set == None):
+            self._Cursor__raise_exception(-25014)
+        if (not self.rownumber):
+            self.rownumber = len(self.__result_set)
+            return self.__result_set
+        else:
+            values = self.__result_set[self.rownumber:len(self.__result_set)]
+            self.rownumber = len(self.__result_set)
+            return values
+
+    def next(self):
+        """
+            Returns the next row in a result set, with the same semantics
+            as fetchone. If there is no more data available in the result
+            set, a StopIteration exception is raised.
+
+        """
+        self._Cursor__check_if_open()
+        self._Cursor__check_for_transaction()
+
+        if (self.__result_set == None):
+            self._Cursor__raise_exception(-25014)
+        if (self.__result_set == []):
+            return self.__result_set
+
+        values = ()
+        try:
+            values = values + self.__result_set[self.rownumber]
+            self.rownumber = self.rownumber + 1
+        except IndexError:
+            raise StopIteration
+        return values
+
+    def scroll(self, value, mode='relative'):
+        """
+            Method scrolls the cursor to a new position according to the
+            mode of the scroll.
+
+            The mode of the cursor is set to relative by default. This
+            changes the cursor’s position by value number of rows in
+            relation to the current position of the cursor. If mode is
+            set to absolute the cursor is moved value number of rows down
+            from the absolute position.
+
+            If the method is called upon and desired position in the result
+            set does not exist, an IndexError is raised.
+
+        """
+        self._Cursor__check_if_open()
+        self._Cursor__check_for_transaction()
+
+        if (mode == 'relative'):
+            new_row = self.rownumber + value
+            if (new_row >= len(self.__result_set)):
+                raise IndexError
+            else:
+                self.rownumber = new_row
+        elif (mode == 'absolute'):
+            if (value >= len(self.__result_set)):
+                raise IndexError
+            else:
+                self.rownumber = value
+        else:
+            self._Cursor__raise_exception(-25016)
```

### Comparing `mimerpy-1.1.3/mimerpy/mimPyExceptionHandler.py` & `mimerpy-1.1.4/mimerpy/mimPyExceptionHandler.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-from mimerpy.mimPyExceptions import *
-import mimerapi
-
-# When adding new MimerAPI error codes:
-#  - Use the range -25xxx
-#  - Check the dictionaries below so that the right exception is thrown
-#  - Update env/gblsym/message.sym in the Mimer trunk
-#  - Update dbl/sdb/syscat.ddi in the Mimer trunk
-#  - Tell Jarl
-
-mimerpy_error = {
-    -25000:"Unsupported method",
-    -25001:"TPC is unsupported",
-    -25010:"Connection not open",
-    -25011:"Invalid number of parameters",
-    -25012:"KeyError in parameters, key: %s does not exist in dictionary",
-    -25013:"Invalid parameter format",
-    -25014:"Previous execute did not produce a result set",
-    -25015:"Cursor not open",
-    -25016:"Illegal scroll mode",
-    -25020:"Data conversion error",
-    -25030:"Out of memory",
-    -25031:"Login failure",
-    -25101:("The operation requires Mimer API version 11.0.5A or newer. You have %s." % mimerapi.__version__),
-    -25102:("The operation requires Mimer API version 11.0.5B or newer. You have %s." % mimerapi.__version__),
-}
-
-py_error_nnnnn = {10001:TransactionAbortError,10003:TransactionAbortError,24010:DataError,24011:DataError
-}
-
-py_error_nnnnx = {2500:NotSupportedError,
-                  2501:ProgrammingError,
-                  2502:DataError,
-                  2503:OperationalError,
-                  2510:NotSupportedError,
-}
-
-py_error_nnxxx = {10:DataError, 11:OperationalError, 12:ProgrammingError,
-                  14:ProgrammingError, 16:OperationalError, 18:DatabaseError,
-                  19:InternalError, 21:IntegrityError, 23:InternalError,
-                  24:ProgrammingError,
-                  25:ProgrammingError, 26:InterfaceError,
-                  27:DataError, 28: NotSupportedError}
-
-py_error_xxxxx = InternalError
-
-def get_error_class(rc):
-    """
-    Return a suitable error class from an error number.
-    """
-    rc = -rc;
-    if rc in py_error_nnnnn:
-        return py_error_nnnnn[rc]
-    rc = rc // 10
-    if rc in py_error_nnnnx:
-        return py_error_nnnnx[rc]
-    rc = rc // 100
-    if rc in py_error_nnxxx:
-        return py_error_nnxxx[rc]
-    return py_error_xxxxx
-
-
-def get_mimerapi_exception(rc, mimerapi_handle):
-    """
-    Return (errorclass, errorvalue) from a failed MimerAPI call.
-    """
-    if -25999 <= rc <= -25000:
-        return (get_error_class(rc), (rc, mimerpy_error[rc]))
-    (rc0, _, msg) = mimerapi.mimerGetError8(mimerapi_handle)
-    if rc0:
-        msg = "Unknown error %d" % rc
-    return (get_error_class(rc), (rc, msg))
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+from mimerpy.mimPyExceptions import *
+import mimerapi
+
+# When adding new MimerAPI error codes:
+#  - Use the range -25xxx
+#  - Check the dictionaries below so that the right exception is thrown
+#  - Update env/gblsym/message.sym in the Mimer trunk
+#  - Update dbl/sdb/syscat.ddi in the Mimer trunk
+#  - Tell Jarl
+
+mimerpy_error = {
+    -25000:"Unsupported method",
+    -25001:"TPC is unsupported",
+    -25010:"Connection not open",
+    -25011:"Invalid number of parameters",
+    -25012:"KeyError in parameters, key: %s does not exist in dictionary",
+    -25013:"Invalid parameter format",
+    -25014:"Previous execute did not produce a result set",
+    -25015:"Cursor not open",
+    -25016:"Illegal scroll mode",
+    -25020:"Data conversion error",
+    -25030:"Out of memory",
+    -25031:"Login failure",
+    -25101:("The operation requires Mimer API version 11.0.5A or newer. You have %s." % mimerapi.__version__),
+    -25102:("The operation requires Mimer API version 11.0.5B or newer. You have %s." % mimerapi.__version__),
+}
+
+py_error_nnnnn = {10001:TransactionAbortError,10003:TransactionAbortError,24010:DataError,24011:DataError
+}
+
+py_error_nnnnx = {2500:NotSupportedError,
+                  2501:ProgrammingError,
+                  2502:DataError,
+                  2503:OperationalError,
+                  2510:NotSupportedError,
+}
+
+py_error_nnxxx = {10:DataError, 11:OperationalError, 12:ProgrammingError,
+                  14:ProgrammingError, 16:OperationalError, 18:DatabaseError,
+                  19:InternalError, 21:IntegrityError, 23:InternalError,
+                  24:ProgrammingError,
+                  25:ProgrammingError, 26:InterfaceError,
+                  27:DataError, 28: NotSupportedError}
+
+py_error_xxxxx = InternalError
+
+def get_error_class(rc):
+    """
+    Return a suitable error class from an error number.
+    """
+    rc = -rc;
+    if rc in py_error_nnnnn:
+        return py_error_nnnnn[rc]
+    rc = rc // 10
+    if rc in py_error_nnnnx:
+        return py_error_nnnnx[rc]
+    rc = rc // 100
+    if rc in py_error_nnxxx:
+        return py_error_nnxxx[rc]
+    return py_error_xxxxx
+
+
+def get_mimerapi_exception(rc, mimerapi_handle):
+    """
+    Return (errorclass, errorvalue) from a failed MimerAPI call.
+    """
+    if -25999 <= rc <= -25000:
+        return (get_error_class(rc), (rc, mimerpy_error[rc]))
+    (rc0, _, msg) = mimerapi.mimerGetError8(mimerapi_handle)
+    if rc0:
+        msg = "Unknown error %d" % rc
+    return (get_error_class(rc), (rc, msg))
```

### Comparing `mimerpy-1.1.3/mimerpy/mimPyExceptions.py` & `mimerpy-1.1.4/mimerpy/mimPyExceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-class Warning(Exception):
-
-    """
-        Exception raised for important warnings like data truncations
-        while inserting, etc.
-
-    """
-    def __init__(self, message):
-        self.message = message
-
-class Error(Exception):
-
-    """
-        Exception that is the base class of all other error exceptions.
-        Can be used to catch all errors with one single except statement.
-
-    """
-    def __init__(self, message):
-        self.errno = message[0]
-        self.message = message[1]
-
-    def __str__(self):
-        text = str(self.errno) + " " + self.message
-        return text
-
-class InterfaceError(Error):
-
-    """
-        Exception raised for errors that are related to the database
-        interface rather than the database itself. For example if a
-        parameter is specified in the wrong format.
-
-    """
-
-class DatabaseError(Error):
-
-    """
-        Exception raised for errors that are related to the database.
-
-    """
-
-class DataError(DatabaseError):
-
-    """
-        Exception raised for errors that are due to problems with the
-        processed data like division by zero, numeric value out of range, etc.
-
-    """
-
-class OperationalError(DatabaseError):
-
-    """
-        Exception raised for errors that are related to the database’s
-        operation and not necessarily under the control of the programmer,
-        e.g. an unexpected disconnect occurs, the data source name is not
-        found, a transaction could not be processed, a memory allocation
-        error occurred during processing, etc.
-
-    """
-
-class TransactionAbortError(OperationalError):
-
-    """
-        Exception raised for Transaction aborted. Can be due to conflict with 
-        other transaction or due to a preceding problem with databanks or 
-        resources
-
-    """
-
-class IntegrityError(DatabaseError):
-
-    """
-        Exception raised when the relational integrity of the database
-        is affected, e.g. a foreign key check fails.
-
-    """
-
-class InternalError(DatabaseError):
-
-    """
-        Exception raised when the database encounters an internal error,
-        e.g. the cursor is not valid anymore, the transaction is out of
-        sync, etc.
-
-    """
-
-class ProgrammingError(DatabaseError):
-
-    """
-        Exception raised for programming errors, e.g. table not found
-        or already exists, syntax error in the SQL statement, wrong
-        number of parameters specified, etc.
-
-    """
-
-
-class NotSupportedError(DatabaseError):
-
-    """
-        Exception raised in case a method or database API was used which
-        is not supported by the database.
-
-    """
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+class Warning(Exception):
+
+    """
+        Exception raised for important warnings like data truncations
+        while inserting, etc.
+
+    """
+    def __init__(self, message):
+        self.message = message
+
+class Error(Exception):
+
+    """
+        Exception that is the base class of all other error exceptions.
+        Can be used to catch all errors with one single except statement.
+
+    """
+    def __init__(self, message):
+        self.errno = message[0]
+        self.message = message[1]
+
+    def __str__(self):
+        text = str(self.errno) + " " + self.message
+        return text
+
+class InterfaceError(Error):
+
+    """
+        Exception raised for errors that are related to the database
+        interface rather than the database itself. For example if a
+        parameter is specified in the wrong format.
+
+    """
+
+class DatabaseError(Error):
+
+    """
+        Exception raised for errors that are related to the database.
+
+    """
+
+class DataError(DatabaseError):
+
+    """
+        Exception raised for errors that are due to problems with the
+        processed data like division by zero, numeric value out of range, etc.
+
+    """
+
+class OperationalError(DatabaseError):
+
+    """
+        Exception raised for errors that are related to the database’s
+        operation and not necessarily under the control of the programmer,
+        e.g. an unexpected disconnect occurs, the data source name is not
+        found, a transaction could not be processed, a memory allocation
+        error occurred during processing, etc.
+
+    """
+
+class TransactionAbortError(OperationalError):
+
+    """
+        Exception raised for Transaction aborted. Can be due to conflict with 
+        other transaction or due to a preceding problem with databanks or 
+        resources
+
+    """
+
+class IntegrityError(DatabaseError):
+
+    """
+        Exception raised when the relational integrity of the database
+        is affected, e.g. a foreign key check fails.
+
+    """
+
+class InternalError(DatabaseError):
+
+    """
+        Exception raised when the database encounters an internal error,
+        e.g. the cursor is not valid anymore, the transaction is out of
+        sync, etc.
+
+    """
+
+class ProgrammingError(DatabaseError):
+
+    """
+        Exception raised for programming errors, e.g. table not found
+        or already exists, syntax error in the SQL statement, wrong
+        number of parameters specified, etc.
+
+    """
+
+
+class NotSupportedError(DatabaseError):
+
+    """
+        Exception raised in case a method or database API was used which
+        is not supported by the database.
+
+    """
```

### Comparing `mimerpy-1.1.3/mimerpy.egg-info/PKG-INFO` & `mimerpy-1.1.4/mimerpy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: mimerpy
-Version: 1.1.3
-Summary: Python database interface for Mimer SQL
-Home-page: https://developer.mimer.com/mimerpy
-Author: Erik Gunne & Magdalena Bostrom
-Author-email: mimerpy@mimer.com
-Maintainer: Mimer Information Technology AB
-Maintainer-email: mimerpy@mimer.com
-License: MIT
-Keywords: Mimer MimerSQL Database SQL PEP249
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-MimerPy: Python database interface for Mimer SQL
-==================================================
-MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
-`PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
-implemented on top of a Cpython wrapper of the native Mimer API interface.
-
-Requirements:
-
-* A Mimer SQL version 11 or later installation on the client side
-* A Mimer SQL version 11 or later database server
-* MimerPy is currently supported on Linux, and Windows.
-* Python 3.5 or later
-
-The source code for MimerPy resides on GitHub_. Installable packages
-can be found on PyPi_. To install, use the command:
-
-.. code-block:: console
-
-    python3 -m pip install mimerpy
-
-The source for the MimerPy manual is stored together with the source
-in the doc/ directory. We recommend reading it on the
-Mimer Information Technology `documentation site`_.
-
-The `home page`_ for the project can be found on the Mimer Information Technology developer site.
-
-
-.. _Python: http://www.python.org/
-.. _PEP 249: https://www.python.org/dev/peps/pep-0249/
-.. _MimerSQL: https://www.mimer.com
-.. _GitHub: https://github.com/mimersql/MimerPy
-.. _PyPi: https://pypi.org/project/mimerpy/
-.. _documentation site: https://developer.mimer.com/documentation
-.. _home page: https://developer.mimer.com/mimerpy
+Metadata-Version: 2.1
+Name: mimerpy
+Version: 1.1.4
+Summary: Python database interface for Mimer SQL
+Home-page: https://developer.mimer.com/mimerpy
+Author: Erik Gunne & Magdalena Bostrom
+Author-email: mimerpy@mimer.com
+Maintainer: Mimer Information Technology AB
+Maintainer-email: mimerpy@mimer.com
+License: MIT
+Description: MimerPy: Python database interface for Mimer SQL
+        ==================================================
+        MimerPy is an adapter for Mimer SQL version 11 in Python_ which implements the
+        `PEP 249`_ specification.  It allows the user to access Mimer SQL through Python. MimerPy is
+        implemented on top of a Cpython wrapper of the native Mimer API interface.
+        
+        Requirements:
+        
+        * A Mimer SQL version 11 or later installation on the client side
+        * A Mimer SQL version 11 or later database server
+        * MimerPy is currently supported on Linux, and Windows.
+        * Python 3.5 or later
+        
+        The source code for MimerPy resides on GitHub_. Installable packages
+        can be found on PyPi_. To install, use the command:
+        
+        .. code-block:: console
+        
+            python3 -m pip install mimerpy
+        
+        The source for the MimerPy manual is stored together with the source
+        in the doc/ directory. We recommend reading it on the
+        Mimer Information Technology `documentation site`_.
+        
+        The `home page`_ for the project can be found on the Mimer Information Technology developer site.
+        
+        
+        .. _Python: http://www.python.org/
+        .. _PEP 249: https://www.python.org/dev/peps/pep-0249/
+        .. _MimerSQL: https://www.mimer.com
+        .. _GitHub: https://github.com/mimersql/MimerPy
+        .. _PyPi: https://pypi.org/project/mimerpy/
+        .. _documentation site: https://developer.mimer.com/documentation
+        .. _home page: https://developer.mimer.com/mimerpy
+        
+Keywords: Mimer MimerSQL Database SQL PEP249
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.5
+Description-Content-Type: text/x-rst
```

### Comparing `mimerpy-1.1.3/setup.py` & `mimerpy-1.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-from setuptools import setup, Extension
-from distutils.core import Extension
-import platform, os
-
-plat = platform.system()
-bits = platform.architecture()[0][0:2]
-
-incDirs = []
-libDirs = []
-libs = ['mimerapi']
-extraLinkArgs = []
-
-if plat == 'Linux':
-    pass
-elif plat == 'Darwin':
-    incDirs = ['/usr/local/include']
-    libDirs = ['/usr/local/lib']
-elif plat == 'Windows':
-    libs = ['mimapi' + bits]
-    from winreg import HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY, ConnectRegistry, OpenKeyEx, QueryValueEx, CloseKey, EnumKey, OpenKeyEx
-    root = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
-    mimer_key = OpenKeyEx(root, r"SOFTWARE\Mimer\Mimer SQL", 0,  KEY_READ | KEY_WOW64_64KEY)
-    index = 0
-    while True:
-        try:
-            key = EnumKey(mimer_key,index)
-            if key != "License" and key != "SQLHosts":
-                version = key
-                break
-            index = index + 1
-        except OSError:
-            break
-    inner_key = OpenKeyEx(mimer_key, version)
-    path = QueryValueEx(inner_key, 'PathName')[0]
-    CloseKey(inner_key)
-    CloseKey(root)
-    if bits == '64':
-        libDirs = [path + 'dev\\lib\\amd64']
-    elif bits == '32': 
-        libDirs = [path + 'dev\\lib\\x86']
-    else: 
-        raise Exception('Unsupported windows version, have to be 32 or 64 bits: ' + bits)
-    incDirs.append(path + 'dev\\include')
-elif plat == 'OpenVMS':
-    incDirs = ['MIMER$LIB']
-    libs = []
-    if bits == '64':
-        extraLinkArgs = [',MIMER$LIB:MIMER$API64/OPT']
-    else:
-        extraLinkArgs = [',MIMER$LIB:MIMER$API/OPT']
-else:
-    raise Exception('Unsupported platform: ' + plat)
-
-sources = ["src/mimerapi.c"]
-
-extensions = [
-    Extension('mimerapi',
-              include_dirs = incDirs,
-              library_dirs = libDirs,
-              libraries = libs,
-              extra_link_args = extraLinkArgs,
-              sources = sources),
-    ]
-
-setup (
-    name='mimerpy',
-    version = '1.1.3',
-    url='https://developer.mimer.com/mimerpy',
-    description='Python database interface for Mimer SQL',
-    long_description=open('README.rst').read(),
-    long_description_content_type='text/x-rst',
-    #long_description_content_type="text/markdown",
-    #download_url='www.developer.mimer.com/python/download',
-    author='Erik Gunne & Magdalena Bostrom',
-    author_email='mimerpy@mimer.com',
-    maintainer = 'Mimer Information Technology AB',
-    maintainer_email = 'mimerpy@mimer.com',
-    license='MIT',
-    classifiers=[
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    keywords='Mimer MimerSQL Database SQL PEP249',
-    ext_modules = extensions,
-    packages=['mimerpy'],
-    package_dir={'mimerpy': 'mimerpy', 'mimerpy.tests': 'tests'},
-    python_requires='>=3.5',
-    #install_requires=['Mimer>=11.0']
-    )
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+from setuptools import setup, Extension
+from distutils.core import Extension
+import platform, os
+
+plat = platform.system()
+bits = platform.architecture()[0][0:2]
+
+incDirs = []
+libDirs = []
+libs = ['mimerapi']
+extraLinkArgs = []
+
+if plat == 'Linux':
+    pass
+elif plat == 'Darwin':
+    incDirs = ['/usr/local/include']
+    libDirs = ['/usr/local/lib']
+elif plat == 'Windows':
+    libs = ['mimapi' + bits]
+    from winreg import HKEY_LOCAL_MACHINE, KEY_READ, KEY_WOW64_64KEY, ConnectRegistry, OpenKeyEx, QueryValueEx, CloseKey, EnumKey, OpenKeyEx
+    root = ConnectRegistry(None, HKEY_LOCAL_MACHINE)
+    mimer_key = OpenKeyEx(root, r"SOFTWARE\Mimer\Mimer SQL", 0,  KEY_READ | KEY_WOW64_64KEY)
+    index = 0
+    while True:
+        try:
+            key = EnumKey(mimer_key,index)
+            if key != "License" and key != "SQLHosts":
+                version = key
+                break
+            index = index + 1
+        except OSError:
+            break
+    inner_key = OpenKeyEx(mimer_key, version)
+    path = QueryValueEx(inner_key, 'PathName')[0]
+    CloseKey(inner_key)
+    CloseKey(root)
+    if bits == '64':
+        libDirs = [path + 'dev\\lib\\amd64']
+    elif bits == '32': 
+        libDirs = [path + 'dev\\lib\\x86']
+    else: 
+        raise Exception('Unsupported windows version, have to be 32 or 64 bits: ' + bits)
+    incDirs.append(path + 'dev\\include')
+elif plat == 'OpenVMS':
+    incDirs = ['MIMER$LIB']
+    libs = []
+    if bits == '64':
+        extraLinkArgs = [',MIMER$LIB:MIMER$API64/OPT']
+    else:
+        extraLinkArgs = [',MIMER$LIB:MIMER$API/OPT']
+else:
+    raise Exception('Unsupported platform: ' + plat)
+
+sources = ["src/mimerapi.c"]
+
+extensions = [
+    Extension('mimerapi',
+              include_dirs = incDirs,
+              library_dirs = libDirs,
+              libraries = libs,
+              extra_link_args = extraLinkArgs,
+              sources = sources),
+    ]
+
+setup (
+    name='mimerpy',
+    version = '1.1.4',
+    url='https://developer.mimer.com/mimerpy',
+    description='Python database interface for Mimer SQL',
+    long_description=open('README.rst').read(),
+    long_description_content_type='text/x-rst',
+    #long_description_content_type="text/markdown",
+    #download_url='www.developer.mimer.com/python/download',
+    author='Erik Gunne & Magdalena Bostrom',
+    author_email='mimerpy@mimer.com',
+    maintainer = 'Mimer Information Technology AB',
+    maintainer_email = 'mimerpy@mimer.com',
+    license='MIT',
+    classifiers=[
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+    ],
+    keywords='Mimer MimerSQL Database SQL PEP249',
+    ext_modules = extensions,
+    packages=['mimerpy'],
+    package_dir={'mimerpy': 'mimerpy', 'mimerpy.tests': 'tests'},
+    python_requires='>=3.5',
+    #install_requires=['Mimer>=11.0']
+    )
```

### Comparing `mimerpy-1.1.3/tests/testConnection.py` & `mimerpy-1.1.4/tests/testConnection.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,476 +1,476 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import mimerpy
-import unittest
-import time
-import random
-import _thread
-
-from mimerpy.mimPyExceptions import *
-import db_config
-
-class TestConnectionMethods(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(self):
-        (self.syscon, self.tstcon) = db_config.setup()
-
-    @classmethod
-    def tearDownClass(self):
-        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
-
-    def tearDown(self):
-        self.tstcon.commit()
-
-    def test_connect(self):
-        con = mimerpy.connect(**db_config.TSTUSR)
-        con.close()
-
-
-    def test_connect_many(self):
-        for a in range(100):
-            con = mimerpy.connect(**db_config.TSTUSR)
-            con.close()
-
-    # Ran with 1000 before, but with current version it is very slow
-    # Mimer now uses fancy new password encryption, this is slower than before
-    def test_connect_many_no_close(self):
-        for a in range(100):
-            con = mimerpy.connect(**db_config.TSTUSR)
-
-    def test_os_user1(self):
-        con = mimerpy.connect(db_config.DBNAME)
-        con.execute("select 1+1 from system.onerow")
-        con.close()
-
-    def test_os_user2(self):
-        con = mimerpy.connect(db_config.DBNAME, user = db_config.OSUSER)
-        con.execute("select 1+1 from system.onerow")
-        con.close()
-
-    def test_os_user3(self):
-        con = mimerpy.connect(db_config.DBNAME,
-                              user = db_config.OSUSER,
-                              password = 'wrong')
-        con.execute("select 1+1 from system.onerow")
-        con.close()
-
-    # Make sure you allow more than the user than the number_of_connections
-    # or problems occur
-    def test_condis(self):
-        mylist = []
-        number_of_connections = 20
-        for a in range(number_of_connections):
-            con = mimerpy.connect(**db_config.TSTUSR)
-            mylist.append([con, True])
-
-        for a in range(300):
-            rand = random.randint(0,number_of_connections - 1)
-            if(not mylist[rand][1]):
-                mylist.pop(rand)
-                con = mimerpy.connect(**db_config.TSTUSR)
-                mylist.append([con, True])
-            else:
-                mylist[rand][0].close()
-                mylist[rand][1] = False
-
-        for a in mylist:
-            if (a[1]):
-                a[0].close()
-
-    def test_connect_2(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = mimerpy.connect(**db_config.TSTUSR)
-        a.close()
-        b.close()
-
-    def test_connect_close(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        a.close()
-        with self.assertRaises(ProgrammingError):
-            a.commit()
-
-    def test_connect_invalid_login(self):
-        with self.assertRaises(DatabaseError):
-            wrong = db_config.TSTUSR.copy()
-            wrong['password'] = 'wrong'
-            a = mimerpy.connect(**wrong)
-
-    def test_connect_invalid_login_2(self):
-        with self.assertRaises(DatabaseError):
-            a = mimerpy.connect("self.d", "du", "där")
-
-    def test_connect_invalid_option(self):
-        with self.assertRaises(TypeError):
-            wrong = db_config.TSTUSR.copy()
-            wrong['warpspeed'] = 'extra'
-            a = mimerpy.connect(**wrong)
-
-    @unittest.skip("Connection cleanup failure")
-    def test_connect_invalid_login_3(self):
-        with self.assertRaises(IntegrityError):
-            a = mimerpy.connect()
-
-    def test_weakref(self):
-        from weakref import ref
-        import gc
-        con = mimerpy.connect(**db_config.TSTUSR)
-        w = ref(con)
-        con.close()
-        del con
-        gc.collect()
-        self.assertTrue(w() is None)
-
-    def test_connect_cursor(self):
-        con = mimerpy.connect(**db_config.TSTUSR)
-        b = con.cursor()
-        b.close()
-        con.close()
-
-    def test_connect_cursor_close(self):
-        con = mimerpy.connect(**db_config.TSTUSR)
-        b = con.cursor()
-        b.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("Hello")
-        con.close()
-
-    def test_connect_cursor_close_connection_only(self):
-        con = mimerpy.connect(**db_config.TSTUSR)
-        b = con.cursor()
-        con.close()
-
-    def test_connect_cursor_close_connection_only_2(self):
-        con = mimerpy.connect(**db_config.TSTUSR)
-        b = con.cursor()
-        con.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("Hello")
-
-    def test_multiple_cursors(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        b = a.cursor()
-        a.close()
-
-    def test_with(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-
-    def test_with_close(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-            b.execute("create table cbob2(c1 INTEGER, c2 NVARCHAR(10)) in pybank")
-        with self.assertRaises(ProgrammingError):
-            b.execute("select * from cbob2")
-
-    @unittest.skip("not yet")
-    #There is no rollback with DDL statements
-    def test_with_no_commit(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-            b.execute("create table cbob(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            with self.assertRaises(ProgrammingError):
-                b.execute("select * from cbob")
-
-
-    # &&&& Ska vi verkligen autocommitta?
-    def test_with_no_commit_insert(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-            b.execute("create table cbobc(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
-            a.commit()
-            a.execute("insert into cbobc values (?, ?)", (11, 'aaa'))
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            b.execute("select * from cbobc")
-            self.assertEqual(b.fetchall(), [])
-
-    def test_with_commit(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-            b.execute("create table cbob33(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
-            a.commit()
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            b.execute("select * from cbob33")
-
-    def test_with_commit_insert(self):
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            c = a.cursor()
-            b.execute("create table cbob373(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
-            a.commit()
-            a.execute("insert into cbob373 values (?, ?)", (11, 'aaa'))
-            a.commit()
-        with mimerpy.connect(**db_config.TSTUSR) as a:
-            b = a.cursor()
-            b.execute("select * from cbob373")
-            self.assertEqual(b.fetchall(), [(11, 'aaa')])
-
-    def test_operate_after_closed(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        a.close()
-        a.close()
-        with self.assertRaises(ProgrammingError):
-            a.execute("Kalle")
-        with self.assertRaises(ProgrammingError):
-            a.executemany("Kalle", ("Kula"))
-
-    def test_execute(self):
-        b = self.tstcon.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10))"
-                                "in pybank")
-        b.close()
-
-
-    def test_executemany(self):
-        b = self.tstcon.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))"
-                                "in pybank")
-        b = self.tstcon.executemany("insert into bob2 values (:a, :b)",
-                                    ((11, 'aaa'), (22, 'bb'),
-                                     (33, 'cc'), (44, 'dd')))
-        self.tstcon.commit()
-        b.execute("select * from bob2")
-        self.assertEqual(b.fetchall(),
-                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
-        b.close()
-
-
-    def test_executemany_simple(self):
-        b = self.tstcon.execute("create table bob2_simple(c1 INTEGER)"
-                                "in pybank")
-        b = self.tstcon.executemany("insert into bob2_simple values (:a)",
-                                    ((11,),(22,),(33,),(44,)))
-        self.tstcon.commit()
-        b.execute("select * from bob2_simple")
-        self.assertEqual(b.fetchall(),
-                         [(11,),(22,),(33,),(44,)])
-        b.close()
-
-
-    def test_executemany_no_closing(self):
-        b = self.tstcon.execute("create table bob3(c1 INTEGER, c2 NVARCHAR(10))"
-                                "in pybank")
-        b.executemany("insert into bob3 values (:a, :b)",
-                      ((11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')))
-        self.tstcon.commit()
-        b.execute("select * from bob3")
-        self.assertEqual(b.fetchall(),
-                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
-
-    def test_executemany_no_closing_dummy(self):
-        b = self.tstcon.execute("create table bob4(c1 INTEGER, c2 NVARCHAR(10))"
-                                "in pybank")
-        b = self.tstcon.executemany("insert into bob4 values (:a, :b)",
-                                    ((11, 'aaa'), (22, 'bb'),
-                                     (33, 'cc'),  (44, 'dd')))
-        self.tstcon.commit()
-        b.execute("select * from bob4")
-        self.assertEqual(b.fetchall(),
-                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
-
-    def test_commit(self):
-        b = self.tstcon.execute("create table bob5(c1 INTEGER) in pybank")
-        b.execute("insert into bob5 values (:a)", (11))
-        self.tstcon.commit()
-        b.execute("select * from bob5")
-        self.assertEqual(b.fetchone(), (11,))
-        b.close()
-
-    def test_rollback(self):
-        b = self.tstcon.execute("create table bob6(c1 INTEGER) in pybank")
-        self.tstcon.commit()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.execute("insert into bob6 values (:a)", (1133))
-        a.rollback()
-        a.close()
-
-        b = self.tstcon.execute("select * from bob6")
-        self.assertEqual(b.fetchone(), [])
-        b.close()
-
-    def test_autocommit(self):
-        b = self.tstcon.execute("create table bob66(c1 INTEGER) in pybank")
-        self.tstcon.commit()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        a.autocommit(True)
-        b = a.execute("insert into bob66 values (:a)", (1133))
-        a.close()
-
-        b = self.tstcon.execute("select * from bob66")
-        self.assertEqual(b.fetchone(), (1133,))
-        b.close()
-
-    def test_autocommit_2(self):
-        b = self.tstcon.execute("create table bobr66(c1 INTEGER) in pybank")
-        self.tstcon.commit()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        a.autocommit(False)
-        b = a.execute("insert into bobr66 values (:a)", (1133))
-        a.close()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        a.autocommit(True)
-        b = a.execute("insert into bobr66 values (:a)", (23885))
-        a.close()
-
-        b = self.tstcon.execute("select * from bobr66")
-        self.assertEqual(b.fetchone(), (23885,))
-        b.close()
-
-    def test_autocommit_3(self):
-        b = self.tstcon.execute("create table bob63(c1 INTEGER) in pybank")
-        self.tstcon.commit()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.execute("insert into bob63 values (:a)", (1133))
-        a.close()
-
-        b = self.tstcon.execute("select * from bob63")
-        self.assertEqual(b.fetchone(), [])
-        b.close()
-
-    def test_autocommit_4(self):
-        b = self.tstcon.execute("create table bob64(c1 INTEGER) in pybank")
-        self.tstcon.commit()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.execute("insert into bob64 values (:a)", (1133))
-        a.autocommit(True)
-        a.close()
-
-        b = self.tstcon.execute("select * from bob64")
-        self.assertEqual(b.fetchone(), [])
-        b.close()
-
-
-    def test_threads(self):
-
-        def thread_test(self):
-            try:
-                a = mimerpy.connect(**db_config.TSTUSR)
-                a.close()
-            except Exception as e:
-               print("Error: in thread: ", e)
-               """ """
-            try:
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-               _thread.start_new_thread( thread_test,(self,) )
-
-            except Exception as e:
-               print("Error: unable to start thread: ", e)
-               """ """
-
-
-    def test_threads_2(self):
-
-        def thread_test(self):
-            try:
-                a = mimerpy.connect(**db_config.TSTUSR)
-                cur = a.cursor()
-                cur.execute("select * from threadbob")
-                cur.fetchone()
-                a.close()
-            except Exception as e:
-               ###print("Error: in thread: ", e)
-              """ """
-
-        b = self.tstcon.execute("create table threadbob(c1 INTEGER) in pybank")
-        b.execute("insert into threadbob values (:a)", (1133))
-        self.tstcon.commit()
-        b.close()
-
-        try:
-           t1 = _thread.start_new_thread( thread_test,(self,) )
-           t2 = _thread.start_new_thread( thread_test,(self,) )
-           t3 = _thread.start_new_thread( thread_test,(self,) )
-           t4 = _thread.start_new_thread( thread_test,(self,) )
-           t5 = _thread.start_new_thread( thread_test,(self,) )
-           t6 = _thread.start_new_thread( thread_test,(self,) )
-           t7 = _thread.start_new_thread( thread_test,(self,) )
-           t8 = _thread.start_new_thread( thread_test,(self,) )
-           t9 = _thread.start_new_thread( thread_test,(self,) )
-           t10 = _thread.start_new_thread( thread_test,(self,) )
-
-        except Exception as e:
-           print("Error: unable to start thread: ", e)
-           """ """
-        # Potato, needs later fix
-        # Need to change this for a _thread.join() later
-        time.sleep(2)
-
-    def test_xid(self):
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.xid()
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.tpc_begin()
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.tpc_prepare()
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.tpc_commit()
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.tpc_rollback()
-        with self.assertRaises(NotSupportedError):
-            self.tstcon.tpc_recover()
-
-    @unittest.skip("not yet")
-    # Not working atm. cant mix ddl and dml statements in one transaction
-    # When DDL and DML statements are mixed the behavior is not super clear
-    def test_rollback_not_working(self):
-        b = self.tstcon.execute("create table bob7(c1 INTEGER) in pybank")
-        b.execute("insert into bob7 values (:a)", (1133))
-        self.tstcon.rollback()
-        b.execute("select * from bob7")
-        self.assertEqual(b.fetchone(), ())
-        b.close()
-
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.execute("select * from bob6")
-        a.close()
-
-if __name__ == '__main__':
-    unittest.main()
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import mimerpy
+import unittest
+import time
+import random
+import _thread
+
+from mimerpy.mimPyExceptions import *
+import db_config
+
+class TestConnectionMethods(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(self):
+        (self.syscon, self.tstcon) = db_config.setup()
+
+    @classmethod
+    def tearDownClass(self):
+        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
+
+    def tearDown(self):
+        self.tstcon.commit()
+
+    def test_connect(self):
+        con = mimerpy.connect(**db_config.TSTUSR)
+        con.close()
+
+
+    def test_connect_many(self):
+        for a in range(100):
+            con = mimerpy.connect(**db_config.TSTUSR)
+            con.close()
+
+    # Ran with 1000 before, but with current version it is very slow
+    # Mimer now uses fancy new password encryption, this is slower than before
+    def test_connect_many_no_close(self):
+        for a in range(100):
+            con = mimerpy.connect(**db_config.TSTUSR)
+
+    def test_os_user1(self):
+        con = mimerpy.connect(db_config.DBNAME)
+        con.execute("select 1+1 from system.onerow")
+        con.close()
+
+    def test_os_user2(self):
+        con = mimerpy.connect(db_config.DBNAME, user = db_config.OSUSER)
+        con.execute("select 1+1 from system.onerow")
+        con.close()
+
+    def test_os_user3(self):
+        con = mimerpy.connect(db_config.DBNAME,
+                              user = db_config.OSUSER,
+                              password = 'wrong')
+        con.execute("select 1+1 from system.onerow")
+        con.close()
+
+    # Make sure you allow more than the user than the number_of_connections
+    # or problems occur
+    def test_condis(self):
+        mylist = []
+        number_of_connections = 20
+        for a in range(number_of_connections):
+            con = mimerpy.connect(**db_config.TSTUSR)
+            mylist.append([con, True])
+
+        for a in range(300):
+            rand = random.randint(0,number_of_connections - 1)
+            if(not mylist[rand][1]):
+                mylist.pop(rand)
+                con = mimerpy.connect(**db_config.TSTUSR)
+                mylist.append([con, True])
+            else:
+                mylist[rand][0].close()
+                mylist[rand][1] = False
+
+        for a in mylist:
+            if (a[1]):
+                a[0].close()
+
+    def test_connect_2(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = mimerpy.connect(**db_config.TSTUSR)
+        a.close()
+        b.close()
+
+    def test_connect_close(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        a.close()
+        with self.assertRaises(ProgrammingError):
+            a.commit()
+
+    def test_connect_invalid_login(self):
+        with self.assertRaises(DatabaseError):
+            wrong = db_config.TSTUSR.copy()
+            wrong['password'] = 'wrong'
+            a = mimerpy.connect(**wrong)
+
+    def test_connect_invalid_login_2(self):
+        with self.assertRaises(DatabaseError):
+            a = mimerpy.connect("self.d", "du", "där")
+
+    def test_connect_invalid_option(self):
+        with self.assertRaises(TypeError):
+            wrong = db_config.TSTUSR.copy()
+            wrong['warpspeed'] = 'extra'
+            a = mimerpy.connect(**wrong)
+
+    @unittest.skip("Connection cleanup failure")
+    def test_connect_invalid_login_3(self):
+        with self.assertRaises(IntegrityError):
+            a = mimerpy.connect()
+
+    def test_weakref(self):
+        from weakref import ref
+        import gc
+        con = mimerpy.connect(**db_config.TSTUSR)
+        w = ref(con)
+        con.close()
+        del con
+        gc.collect()
+        self.assertTrue(w() is None)
+
+    def test_connect_cursor(self):
+        con = mimerpy.connect(**db_config.TSTUSR)
+        b = con.cursor()
+        b.close()
+        con.close()
+
+    def test_connect_cursor_close(self):
+        con = mimerpy.connect(**db_config.TSTUSR)
+        b = con.cursor()
+        b.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("Hello")
+        con.close()
+
+    def test_connect_cursor_close_connection_only(self):
+        con = mimerpy.connect(**db_config.TSTUSR)
+        b = con.cursor()
+        con.close()
+
+    def test_connect_cursor_close_connection_only_2(self):
+        con = mimerpy.connect(**db_config.TSTUSR)
+        b = con.cursor()
+        con.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("Hello")
+
+    def test_multiple_cursors(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        b = a.cursor()
+        a.close()
+
+    def test_with(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+
+    def test_with_close(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+            b.execute("create table cbob2(c1 INTEGER, c2 NVARCHAR(10)) in pybank")
+        with self.assertRaises(ProgrammingError):
+            b.execute("select * from cbob2")
+
+    @unittest.skip("not yet")
+    #There is no rollback with DDL statements
+    def test_with_no_commit(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+            b.execute("create table cbob(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            with self.assertRaises(ProgrammingError):
+                b.execute("select * from cbob")
+
+
+    # &&&& Ska vi verkligen autocommitta?
+    def test_with_no_commit_insert(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+            b.execute("create table cbobc(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
+            a.commit()
+            a.execute("insert into cbobc values (?, ?)", (11, 'aaa'))
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            b.execute("select * from cbobc")
+            self.assertEqual(b.fetchall(), [])
+
+    def test_with_commit(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+            b.execute("create table cbob33(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
+            a.commit()
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            b.execute("select * from cbob33")
+
+    def test_with_commit_insert(self):
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            c = a.cursor()
+            b.execute("create table cbob373(c1 INTEGER, c2 NVARCHAR(10)) in pybank");
+            a.commit()
+            a.execute("insert into cbob373 values (?, ?)", (11, 'aaa'))
+            a.commit()
+        with mimerpy.connect(**db_config.TSTUSR) as a:
+            b = a.cursor()
+            b.execute("select * from cbob373")
+            self.assertEqual(b.fetchall(), [(11, 'aaa')])
+
+    def test_operate_after_closed(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        a.close()
+        a.close()
+        with self.assertRaises(ProgrammingError):
+            a.execute("Kalle")
+        with self.assertRaises(ProgrammingError):
+            a.executemany("Kalle", ("Kula"))
+
+    def test_execute(self):
+        b = self.tstcon.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10))"
+                                "in pybank")
+        b.close()
+
+
+    def test_executemany(self):
+        b = self.tstcon.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))"
+                                "in pybank")
+        b = self.tstcon.executemany("insert into bob2 values (:a, :b)",
+                                    ((11, 'aaa'), (22, 'bb'),
+                                     (33, 'cc'), (44, 'dd')))
+        self.tstcon.commit()
+        b.execute("select * from bob2")
+        self.assertEqual(b.fetchall(),
+                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
+        b.close()
+
+
+    def test_executemany_simple(self):
+        b = self.tstcon.execute("create table bob2_simple(c1 INTEGER)"
+                                "in pybank")
+        b = self.tstcon.executemany("insert into bob2_simple values (:a)",
+                                    ((11,),(22,),(33,),(44,)))
+        self.tstcon.commit()
+        b.execute("select * from bob2_simple")
+        self.assertEqual(b.fetchall(),
+                         [(11,),(22,),(33,),(44,)])
+        b.close()
+
+
+    def test_executemany_no_closing(self):
+        b = self.tstcon.execute("create table bob3(c1 INTEGER, c2 NVARCHAR(10))"
+                                "in pybank")
+        b.executemany("insert into bob3 values (:a, :b)",
+                      ((11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')))
+        self.tstcon.commit()
+        b.execute("select * from bob3")
+        self.assertEqual(b.fetchall(),
+                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
+
+    def test_executemany_no_closing_dummy(self):
+        b = self.tstcon.execute("create table bob4(c1 INTEGER, c2 NVARCHAR(10))"
+                                "in pybank")
+        b = self.tstcon.executemany("insert into bob4 values (:a, :b)",
+                                    ((11, 'aaa'), (22, 'bb'),
+                                     (33, 'cc'),  (44, 'dd')))
+        self.tstcon.commit()
+        b.execute("select * from bob4")
+        self.assertEqual(b.fetchall(),
+                         [(11, 'aaa'), (22, 'bb'), (33, 'cc'), (44, 'dd')])
+
+    def test_commit(self):
+        b = self.tstcon.execute("create table bob5(c1 INTEGER) in pybank")
+        b.execute("insert into bob5 values (:a)", (11))
+        self.tstcon.commit()
+        b.execute("select * from bob5")
+        self.assertEqual(b.fetchone(), (11,))
+        b.close()
+
+    def test_rollback(self):
+        b = self.tstcon.execute("create table bob6(c1 INTEGER) in pybank")
+        self.tstcon.commit()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.execute("insert into bob6 values (:a)", (1133))
+        a.rollback()
+        a.close()
+
+        b = self.tstcon.execute("select * from bob6")
+        self.assertEqual(b.fetchone(), [])
+        b.close()
+
+    def test_autocommit(self):
+        b = self.tstcon.execute("create table bob66(c1 INTEGER) in pybank")
+        self.tstcon.commit()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        a.autocommit(True)
+        b = a.execute("insert into bob66 values (:a)", (1133))
+        a.close()
+
+        b = self.tstcon.execute("select * from bob66")
+        self.assertEqual(b.fetchone(), (1133,))
+        b.close()
+
+    def test_autocommit_2(self):
+        b = self.tstcon.execute("create table bobr66(c1 INTEGER) in pybank")
+        self.tstcon.commit()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        a.autocommit(False)
+        b = a.execute("insert into bobr66 values (:a)", (1133))
+        a.close()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        a.autocommit(True)
+        b = a.execute("insert into bobr66 values (:a)", (23885))
+        a.close()
+
+        b = self.tstcon.execute("select * from bobr66")
+        self.assertEqual(b.fetchone(), (23885,))
+        b.close()
+
+    def test_autocommit_3(self):
+        b = self.tstcon.execute("create table bob63(c1 INTEGER) in pybank")
+        self.tstcon.commit()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.execute("insert into bob63 values (:a)", (1133))
+        a.close()
+
+        b = self.tstcon.execute("select * from bob63")
+        self.assertEqual(b.fetchone(), [])
+        b.close()
+
+    def test_autocommit_4(self):
+        b = self.tstcon.execute("create table bob64(c1 INTEGER) in pybank")
+        self.tstcon.commit()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.execute("insert into bob64 values (:a)", (1133))
+        a.autocommit(True)
+        a.close()
+
+        b = self.tstcon.execute("select * from bob64")
+        self.assertEqual(b.fetchone(), [])
+        b.close()
+
+
+    def test_threads(self):
+
+        def thread_test(self):
+            try:
+                a = mimerpy.connect(**db_config.TSTUSR)
+                a.close()
+            except Exception as e:
+               print("Error: in thread: ", e)
+               """ """
+            try:
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+               _thread.start_new_thread( thread_test,(self,) )
+
+            except Exception as e:
+               print("Error: unable to start thread: ", e)
+               """ """
+
+
+    def test_threads_2(self):
+
+        def thread_test(self):
+            try:
+                a = mimerpy.connect(**db_config.TSTUSR)
+                cur = a.cursor()
+                cur.execute("select * from threadbob")
+                cur.fetchone()
+                a.close()
+            except Exception as e:
+               ###print("Error: in thread: ", e)
+              """ """
+
+        b = self.tstcon.execute("create table threadbob(c1 INTEGER) in pybank")
+        b.execute("insert into threadbob values (:a)", (1133))
+        self.tstcon.commit()
+        b.close()
+
+        try:
+           t1 = _thread.start_new_thread( thread_test,(self,) )
+           t2 = _thread.start_new_thread( thread_test,(self,) )
+           t3 = _thread.start_new_thread( thread_test,(self,) )
+           t4 = _thread.start_new_thread( thread_test,(self,) )
+           t5 = _thread.start_new_thread( thread_test,(self,) )
+           t6 = _thread.start_new_thread( thread_test,(self,) )
+           t7 = _thread.start_new_thread( thread_test,(self,) )
+           t8 = _thread.start_new_thread( thread_test,(self,) )
+           t9 = _thread.start_new_thread( thread_test,(self,) )
+           t10 = _thread.start_new_thread( thread_test,(self,) )
+
+        except Exception as e:
+           print("Error: unable to start thread: ", e)
+           """ """
+        # Potato, needs later fix
+        # Need to change this for a _thread.join() later
+        time.sleep(2)
+
+    def test_xid(self):
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.xid()
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.tpc_begin()
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.tpc_prepare()
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.tpc_commit()
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.tpc_rollback()
+        with self.assertRaises(NotSupportedError):
+            self.tstcon.tpc_recover()
+
+    @unittest.skip("not yet")
+    # Not working atm. cant mix ddl and dml statements in one transaction
+    # When DDL and DML statements are mixed the behavior is not super clear
+    def test_rollback_not_working(self):
+        b = self.tstcon.execute("create table bob7(c1 INTEGER) in pybank")
+        b.execute("insert into bob7 values (:a)", (1133))
+        self.tstcon.rollback()
+        b.execute("select * from bob7")
+        self.assertEqual(b.fetchone(), ())
+        b.close()
+
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.execute("select * from bob6")
+        a.close()
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `mimerpy-1.1.3/tests/testCursor.py` & `mimerpy-1.1.4/tests/testCursor.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,1961 +1,1961 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import unittest, time, math, random, uuid, decimal
-import mimerpy, mimerapi
-from mimerpy.mimPyExceptions import *
-import db_config
-
-
-# noinspection SqlDialectInspection
-class TestCursorMethods(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(self):
-        (self.syscon, self.tstcon) = db_config.setup()
-
-    @classmethod
-    def tearDownClass(self):
-        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
-
-    def tearDown(self):
-        self.tstcon.rollback()
-
-########################################################################
-## Tests below
-########################################################################
-
-    def test_fetchall_ts(self):
-        with self.tstcon.cursor() as c:
-            c.execute("select 'a', cast('2020-09-17 11:21:51' as timestamp(2)) from system.onerow")
-            self.assertEqual(c.fetchall(), [('a', '2020-09-17 11:21:51.00')])
-
-    def test_fetchall_timestamp_one(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_timestamp(c1 TIMESTAMP(2)) in pybank")
-            c.execute("insert into bob_timestamp values (:a)", ('2020-09-17 11:21:51'))
-            self.tstcon.commit()
-            c.execute("select * from bob_timestamp")
-            r = c.fetchone()
-            self.assertEqual(r, ('2020-09-17 11:21:51.00',))
-
-    def test_fetchall_timestamp_two(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_timestamp2(c1 TIMESTAMP(9)) in pybank")
-            c.execute("insert into bob_timestamp2 values (:a)", ('2020-09-17 11:21:51.123456789'))
-            self.tstcon.commit()
-            c.execute("select * from bob_timestamp2")
-            r = c.fetchone()
-            self.assertEqual(r, ('2020-09-17 11:21:51.123456789',))
-
-    def test_privilege(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(DatabaseError):
-                c.execute("drop ident sysadm cascade")
-
-    def test_createTable(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-
-    def test_createTable_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobcr1(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("create table bobcr2(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("create table bobcr3(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("create table bobcr4(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-        self.tstcon.commit()
-
-    def test_createTable_DropTable(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("drop table bob2 CASCADE")
-        self.tstcon.commit()
-
-    def test_create_invalid_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon (c1 INTEGER, c2 INTEGER) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("banana INTO jon VALUES (3, 14)")
-
-# &&&& This test should fail when we can rollback DDL
-    def test_create_rollback_table(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonnynothere (c1 INTEGER, c2 INTEGER)"
-                      " in pybank")
-            self.tstcon.rollback()
-            c.execute("select * from jonnynothere")
-
-    def test_two_select(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonny (c1 INTEGER, c2 INTEGER) in pybank")
-            c.execute("select c1 from jonny where c1 = (?)", (2))
-            c.execute("select * from jonny")
-
-    def test_many_select(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob356 (c1 INTEGER) in pybank")
-            for val in range(100):
-                c.execute("insert into bob356 values (:a)", (val))
-            for gal in range(100):
-                c.execute("select c1 from bob356 where c1 > (?)", (gal))
-                r = c.fetchall()
-                # &&&& Check resultset
-
-    def test_select_no_commit(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobc (c1 INTEGER, c2 FLOAT) in pybank")
-            for val in range(100):
-                c.execute("insert into bobc values (:a, :b)", (val, val + 0.5))
-            c.execute("select * from bobc where c1 = 99")
-            self.assertEqual(c.fetchall(), [(99, 99.5)])
-
-    def test_select_description(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table description (columnone INTEGER) in pybank")
-            for val in range(10):
-                c.execute("insert into description values (?)", val)
-            c.execute("select * from description")
-            self.assertEqual(c.description,
-                             (('columnone', 50, None, None, None, None, None),))
-
-    def test_select_description2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table description2 (c1 INTEGER, c2 FLOAT)"
-                      " in pybank")
-            for val in range(10):
-                c.execute("insert into description2 values (?,?)",
-                          (val, val / 3))
-            c.execute("select * from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),
-                              ('c2', 56, None, None, None, None, None)))
-            c.execute("select c1 from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),))
-            c.execute("select c2 from description2")
-            self.assertEqual(c.description,
-                             (('c2', 56, None, None, None, None, None),))
-            c.execute("select * from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),
-                              ('c2', 56, None, None, None, None, None)))
-
-    def test_select_description3(self):
-        with self.tstcon.cursor() as c:
-            c.execute("""create table description3(price INTEGER,
-                                      currentvalue FLOAT,
-                                      currency NVARCHAR(128),
-                                      rate BIGINT,
-                                      currentyear INTEGER) in pybank""")
-            for val in range(10):
-                c.execute("insert into description3 values (?,?,?,?,?)",
-                          (val, val / 3, 'SEK', 2 ** 61, val + 2000))
-            c.execute("select * from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentvalue', 56, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None)))
-            c.execute("select price, currentyear, currency, rate from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None)))
-            c.execute("select rate, rate, rate, rate from description3")
-            self.assertEqual(c.description,
-                             (('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None)))
-            c.execute("select * from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentvalue', 56, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None)))
-
-    def test_select_description4(self):
-        with self.tstcon.cursor() as c:
-            name1 = "e" * 127 + "q"
-            name2 = "m" * 127 + "q"
-            query = ("create table description4 (" + name1 + " INTEGER, "
-                     + name2 + " BOOLEAN) in pybank")
-            c.execute(query)
-            for val in range(10):
-                c.execute("insert into description4 values (?,?)",
-                          (val, val % 2))
-            c.execute("select * from description4")
-            self.assertEqual(c.description,
-                             ((name1, 50, None, None, None, None, None),
-                              (name2, 42, None, None, None, None, None)))
-
-    def test_select_description5(self):
-        with self.tstcon.cursor() as c:
-            name1 = "e" * 127 + "q"
-            name2 = "m" * 127 + "q"
-            query = ("create table description5 (" + name1 + " INTEGER, " +
-                     name2 + " BOOLEAN) in pybank")
-            c.execute(query)
-            for val in range(10):
-                c.execute("insert into description5 values (?,?)",
-                          (val, val % 2))
-            c.execute("select * from description5")
-            self.assertEqual(c.description,
-                             ((name1, 50, None, None, None, None, None),
-                              (name2, 42, None, None, None, None, None)))
-
-    def test_invalid_create(self):
-        b = self.tstcon.cursor()
-        b.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("create table jon(i int) in pybank")
-
-    def test_insert_parametermarkers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob1 (c1 INTEGER,  c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("insert into bob1 values (:a, :b)", (3, 'bob'))
-
-    def test_insert_parametermarkers_long_string(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobstring (c1 INTEGER,  c2 NVARCHAR(256))"
-                      " in pybank")
-            string = "mimer" * 40
-            c.execute("insert into bobstring values (:a, :b)", (3, string))
-            self.tstcon.commit()
-            c.execute("select c2 from bobstring")
-            self.assertEqual(c.fetchall(), [(string,)])
-
-    def test_insert_parametermarkers_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob13 (c1 INTEGER, c2 NVARCHAR(10),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            pmarkers = [(1, 'pi', 14.345),
-                           (2, 'pii', 14.345),
-                           (-3, 'piii', 14.345),
-                           (7, 'piii', 14.345),
-                           (1121231, 'piiii', 14.345)]
-            c.executemany("insert into bob13 values (:a, :b, :c)",
-                         pmarkers)
-            self.tstcon.commit()
-            c.execute("select * from bob13")
-            self.assertEqual(c.fetchall(),
-                            pmarkers)
-
-    def test_insert_parametermarkers_russian(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob14 (c1 INTEGER, c2 NVARCHAR(128),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob14 values (:a, :b, :c)",
-                          ((1, 'продиктованной ангелом', 14.345),
-                           (2, '安排他們參', 14.345)))
-            self.tstcon.commit()
-            c.execute("select * from bob14")
-            self.assertEqual(c.fetchall(),
-                             [(1, 'продиктованной ангелом', 14.345),
-                              (2, '安排他們參', 14.345)])
-
-    def test_insert_parametermarkers_unicode(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table boby14 (c1 INTEGER, c2 NVARCHAR(128),"
-                      "                     c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into boby14 values (:a, :b, :c)",
-                          ((1, 'продиктованной ангелом', 14.345),
-                           (2, '安排他們參‱', 14.345)))
-            self.tstcon.commit()
-            c.execute("select * from boby14")
-            self.assertEqual(c.fetchall(),
-                             [(1, 'продиктованной ангелом', 14.345),
-                              (2, '安排他們參‱', 14.345)])
-
-    def test_insert_parametermarkers_goodchar(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobg14(c1 char(10)) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bobg14 values (?)", 'åååååååååå')
-            self.tstcon.commit()
-            c.execute("select * from bobg14")
-            self.assertEqual(c.fetchall(),
-                             [('åååååååååå',)])
-
-    def test_insert_parametermarkers_illchar(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobz14(c1 char(10)) in pybank")
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into bobz14 values (?)", '安排')
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into bobz14 values (?)", '€')
-
-    def test_insert_parametermarkers_too_long(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob15 (c1 NVARCHAR(10)) in pybank")
-            self.tstcon.commit()
-            with self.assertRaises(DatabaseError):
-                c.execute("insert into bob15 values (:a)",
-                          ('This sentence is too long'))
-        self.tstcon.commit()
-
-    def test_insert_too_few_parametermarkers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob3 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            with self.assertRaises(DatabaseError):
-                c.execute("insert into bob3 values (:a, :b)", (3))
-
-    def test_insert_too_many_parametermarkers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob33 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob33 values (:a, :b)",
-                              ((3, 'pi', 14), (3)))
-
-    def test_insert_parametermarkers_dict(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table poff_dict1 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("insert into poff_dict1 values (:a, :b)",
-                              {'a':3, 'b':'pi'})
-        self.tstcon.commit()
-
-    def test_to_many_parametermarkers_dict(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table poff_dict2 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.execute("insert into poff_dict2 values (:a, :b)",
-                              {'g':55, 'a':3, 'b':'pi', 'y':'Boo'})
-            c.execute("select * from poff_dict2")
-            r = c.fetchall()[0]
-            self.assertEqual(r, (3, 'pi'))
-        self.tstcon.commit()
-
-    def test_insert_many_times(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob34(c1 INTEGER, c2 NVARCHAR(10),"
-                      "                   c3 FLOAT) in pybank")
-            for i in range(0, 101):
-                c.execute("insert into bob34 values (5,'ウィキペディ', 4.4543543)")
-        self.tstcon.commit()
-
-    def test_executemany_one_value(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob4 (c1 INTEGER) in pybank")
-            c.executemany("insert into bob4 values (:a)", [(1,)])
-            #with self.assertRaises(ProgrammingError):
-            c.execute("insert into bob4 values (:a)", [(1)])
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob4 values (:a)", (1))
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob4 values (:a)", [1])
-
-    def test_executemany_one_tuple(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob5 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.executemany("insert into bob5 values (:a, :b)", ((1, 'bob1'),))
-
-    def test_executemany_several_tuples(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobe6 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.executemany("insert into bobe6 values (:a, :b)",
-                          [(1, 'bob1'), (2, 'bob2'),
-                           (3, 'bob3')])
-
-    def test_commit(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob7d (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            c.executemany("insert into bob7d values (:a, :b)",
-                          ((1, 'bob1'), (2, 'bob2'),
-                           (3, 'bob3')))
-            self.tstcon.commit()
-
-    ### &&&& Should fail since DDL has no commit
-    def test_fetchone(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.cursor()
-        b.execute("create table bob8 (c1 INTEGER, c2 NVARCHAR(10)) in pybank")
-        a.close()
-
-        with self.tstcon.cursor() as c:
-            c.execute("insert into bob8 values (:a, :b)", (8, 'bob'))
-            self.tstcon.commit()
-            c.execute("select * from bob8")
-            self.assertEqual(c.fetchone(), (8, 'bob'))
-
-    def test_fetchmany(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob9 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            self.tstcon.commit()
-
-            c.executemany("insert into bob9 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'),
-                           (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob9")
-            self.assertEqual(c.fetchmany(3),
-                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
-
-    def test_fetchmany_too_many(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob11 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob11 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'),
-                           (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob11")
-            self.assertEqual(c.fetchmany(5),
-                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
-
-    def test_fetchmany_notall(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob12 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob12 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'),
-                           (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob12")
-            self.assertEqual(c.fetchmany(2),
-                             [(9, 'bob9'), (10, 'bob10')])
-            self.assertEqual(c.fetchmany(2), [(11, 'bob11')])
-
-    def test_fetchmany_generator_smol(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_generator (c1 INTEGER, c2 INTEGER)"
-                      " in pybank")
-            generator = ((i,-i) for i in range(10))
-            c.executemany("insert into bob_generator values (:a, :b)", generator)
-            self.tstcon.commit()
-
-    def test_fetchmany_generator_large(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_generator2 (c1 INTEGER, c2 INTEGER)"
-                      " in pybank")
-        with self.tstcon.cursor() as c:
-            size = 100000
-            generator = ((i,-i) for i in range(size))
-            c.executemany("insert into bob_generator2 values (:a, :b)", generator)
-            self.tstcon.commit()
-            c.execute("SELECT MAX(c1), MIN(c2) AS maxv FROM bob_generator2")
-            self.assertEqual(c.fetchone(),(size - 1, -size + 1))
-
-    @unittest.skip
-    def test_fetchmany_generator_too_large(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_generator3 (c1 INTEGER, c2 INTEGER)"
-                    " in pybank")
-        with self.tstcon.cursor() as c:
-            size = 1000000
-            generator = ((i,-i) for i in range(size))
-            c.executemany("insert into bob_generator3 values (:a, :b)", generator)
-            self.tstcon.commit()
-            c.execute("SELECT MAX(c1), MIN(c2) AS maxv FROM bob_generator")
-            self.assertEqual(c.fetchone(),(size - 1, -size + 1))
-
-    def test_fetchall(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob10 (c1 INTEGER, c2 NVARCHAR(10))"
-                      " in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob10 values (:a, :b)",
-                          ((10, 'bob10'), (11, 'bob11'), (12, 'bob12'),))
-            self.tstcon.commit()
-            c.execute("select * from bob10")
-            self.assertEqual(c.fetchall(),
-                             [(10, 'bob10'), (11, 'bob11'), (12, 'bob12')])
-
-    def test_fetchall_correct_number_of_rows(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob101(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-            for i in range(1, 101):
-                c.execute("insert into bob101 values (5,'ウィキペディ', 4.4543543)")
-            self.tstcon.commit()
-            c.execute("select * from bob101")
-            r = c.fetchall()
-            self.assertEqual(len(r), 100)
-
-    def test_fetchall_correct_number_of_rows2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob102(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-        with self.tstcon.cursor() as c:
-            for i in range(1, 101):
-                c.execute("insert into bob102 values (5,'ウィキペディ', 4.4543543)")
-            self.tstcon.rollback()
-            c.execute("select * from bob102")
-            r = c.fetchall()
-            self.assertEqual(len(r), 0)
-
-    def test_fetchall_correct_number_of_rows3(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob103(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-        with self.tstcon.cursor() as c:  
-            for i in range(1, 101):
-                c.execute("insert into bob103 values (5,'ウィキペディ', 4.4543543)")
-                self.tstcon.rollback()
-                c.execute("select * from bob103")
-                r = c.fetchall()
-                self.assertEqual(len(r), 0)
-
-    def test_use_next(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobnext(c1 INTEGER) in pybank")
-            for i in range(0, 10):
-                c.execute("insert into bobnext values (?)", i)
-                self.tstcon.commit()
-                c.execute("select * from bobnext")
-            for i in range(0, 10):
-                val = c.next()
-                self.assertEqual(val, (i,))
-
-    def test_use_next_StopIteration(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobstop(c1 INTEGER) in pybank")
-            for i in range(0, 10):
-                c.execute("insert into bobstop values (?)", i)
-                self.tstcon.commit()
-                c.execute("select * from bobstop")
-            for i in range(0, 10):
-                c.next()
-            with self.assertRaises(StopIteration):
-                c.next()
-
-    def test_insert_wrong_type_parametermarkers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob1337 (c1 INTEGER, c2 INTEGER) in pybank")
-            with self.assertRaises(DataError):
-                c.execute("insert into bob1337  values (:a, :b)", (3, 3.14))
-
-    def test_operate_after_closed(self):
-        c = self.tstcon.cursor()
-        c.close()
-        with self.assertRaises(ProgrammingError):
-            c.execute("select * from system.onerow")
-
-    def test_operate_after_closed_2(self):
-        c = self.tstcon.cursor()
-        c.close()
-        c.close()
-        with self.assertRaises(ProgrammingError):
-            c.execute("Kalle")
-        with self.assertRaises(ProgrammingError):
-            c.executemany("Kalle", ("Kula"))
-        with self.assertRaises(ProgrammingError):
-            c.fetchone()
-        with self.assertRaises(ProgrammingError):
-            c.fetchmany("Kalle")
-        with self.assertRaises(ProgrammingError):
-            c.fetchall()
-        with self.assertRaises(ProgrammingError):
-            c.next()
-
-    def test_invalid_select(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(ProgrammingError):
-                c.execute("select * from jonisnotatablejo where c1 = ?", (5))
-
-    def test_same_table_twice(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob2437(c1 INTEGER) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob2437(c1 INTEGER) in pybank")
-
-    def test_invalid_sequence_select(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob6565(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("select * from bob6565")
-            r = c.fetchone()
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob6569(c1 INTEGER) in pybank")
-
-    # &&&& borde bli fel men blir rätt....
-    # Blir inte rätt för att man blandar DDL och DML i samma transaktion
-    @unittest.skip
-    def test_invalid_sequence_select_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob555(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("select * from bob555")
-            c.execute("create table bob556(c1 INTEGER) in pybank")
-            c.execute("insert into bob556 values (3)")
-            self.tstcon.rollback()
-            c.execute("select * from bob556")
-            self.assertEqual(c.fetchone(), [])
-
-    def test_invalid_sequence_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob6567(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bob6567 values (3)")
-            ## &&&& Should not fail
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob65ss(c1 INTEGER) in pybank")
-                self.tstcon.rollback()
-
-    def test_invalid_sequence_insert_parametermarkers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob6568(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bob6568 values (?)", (3))
-            ## &&&& Should not fail
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob6566(c1 INTEGER) in pybank")
-                self.tstcon.rollback()
-
-    def test_executemany_DDL(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(ProgrammingError):
-                b = c.executemany("create table bob6(c1 INTEGER) in pybank",
-                                  (3))
-
-    def test_insert_exceeded(self):
-        with self.tstcon.cursor() as c:
-            b = c.execute("create table bob16(c1 BIGINT) in pybank")
-            big = pow(2, 100)
-            with self.assertRaises(DataError):
-                c.execute("insert into bob16 values (?)", big)
-
-    def test_insert_too_long(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob17(c1 NVARCHAR(10)) in pybank")
-            self.tstcon.commit()
-            with self.assertRaises(DataError):
-                c.execute("insert into bob17 values ('ウィキペデBobWasAYoungBoy')")
-                self.tstcon.commit()
-
-    def test_valid_int32_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon32 (c1 INTEGER, c2 INTEGER) in pybank")
-            nvar = -2 ** 31
-            var = 2 ** 31 - 1
-            c.execute("insert INTO jon32 VALUES (?, ?)", (nvar, var))
-            self.tstcon.commit()
-
-    def test_invalid_int32_insert_too_small(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon31 (c1 INTEGER) in pybank")
-            nvar = -2 ** 31 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon31 VALUES (?)", (nvar))
-
-    def test_invalid_int32_insert_too_big(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon33 (c1 INTEGER) in pybank")
-            var = 2 ** 31
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon33 VALUES (?)", (var))
-
-    def test_valid_int64_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon64 (c1 BIGINT, c2 BIGINT) in pybank")
-            nvar = -2 ** 63
-            var = 2 ** 63 - 1
-            c.execute("insert INTO jon64 VALUES (?,?)", (nvar, var))
-            self.tstcon.commit()
-            c.execute("Select * from jon64")
-            self.assertEqual(c.fetchall(), [(nvar, var)])
-
-    def test_overflow_int64_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table intjon4 (c1 BIGINT, c2 BIGINT) in pybank")
-            nvar = -2 ** 633
-            var = 2 ** 63 - 1
-            with self.assertRaises(DataError):
-                c.executemany("insert INTO intjon4 VALUES (?,?)",
-                              ((nvar, var), (nvar, var)))
-
-    def test_invalid_int64_insert_too_small(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon63 (c1 BIGINT) in pybank")
-            nvar = -2 ** 63 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon63 VALUES (?)", (nvar))
-
-    def test_invalid_int64_insert_too_big(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon65 (c1 BIGINT) in pybank")
-            var = 2 ** 63
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon65 VALUES (?)", (var))
-
-    def test_valid_int16_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon26 (c1 SMALLINT, c2 SMALLINT) in pybank")
-            nvar = -2 ** 15
-            var = 2 ** 15 - 1
-            c.execute("insert INTO jon26 VALUES (?, ?)", (nvar, var))
-            self.tstcon.commit()
-            c.execute("SELECT * from jon26")
-            self.assertEqual(c.fetchall(), [(nvar,var)])
-
-    def test_invalid_int16_insert_too_small(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon15 (c1 SMALLINT) in pybank")
-            nvar = -2 ** 15 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon15 VALUES (?)", (nvar))
-
-    def test_invalid_int16_insert_too_big(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon17 (c1 SMALLINT) in pybank")
-            nvar = 2 ** 15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon17 VALUES (?)", (nvar))
-
-    # &&&& Gives a Warning we dont catch atm
-    def test_valid_double_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon16 (c1 REAL, c2 DOUBLE PRECISION)"
-                      " in pybank")
-            var = 2 / 3
-            c.execute("insert INTO jon16 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-            c.execute("select * from jon16")
-            self.assertEqual(c.fetchall(), [(0.6666666865348816, var)])
-
-    def test_invalid_double_insert(self):
-        b = self.tstcon.cursor()
-        c = self.tstcon.cursor()
-        d = self.tstcon.cursor()
-        e = self.tstcon.cursor()
-        f = self.tstcon.cursor()
-        b.execute("create table jondd (c1 FLOAT) in pybank")
-        var = 10 ** 309
-        with self.assertRaises(DataError):
-            b.execute("insert INTO jondd VALUES (?)", (var))
-        with self.assertRaises(ProgrammingError):
-            b.execute("insert INTO jondd VALUES (?, ?)", (-var, -var))
-        b.close()
-        c.close()
-        d.close()
-        e.close()
-        f.close()
-
-    def test_valid_double_insert_none(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon18 (c1 REAL, c2 DOUBLE PRECISION)"
-                      " in pybank")
-            var = None
-            c.execute("insert INTO jon18 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-            c.execute("select * from jon18")
-            self.assertEqual(c.fetchall(), [(None, None)])
-
-    def test_valid_double_select_none(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jon19 (c1 REAL, c2 DOUBLE PRECISION)"
-                      " in pybank")
-            var = None
-            c.execute("insert INTO jon19 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-            c.execute("select * from jon19")
-            self.assertEqual(c.fetchall(), [(None, None)])
-
-    def test_message_cleared(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonwas17 (c1 SMALLINT) in pybank")
-            nvar = 2 ** 15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jonwas17 VALUES (?)", (nvar))
-            c.execute("insert INTO jonwas17 VALUES (?)", (5))
-            self.assertEqual(c.messages, [])
-
-    def test_message_cleared_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonwas173 (c1 SMALLINT) in pybank")
-            nvar = 2 ** 15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jonwas173 VALUES (?)", (nvar))
-            self.assertEqual(c.messages[0][1],
-                             (-24010,
-                              'Value was too large to fit in destination'))
-
-    def test_None_is_returned(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonNone (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonNone VALUES (?)", (i))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonNone")
-            for i in range(1, 10):
-                c.fetchone()
-            self.assertEqual(c.fetchone(), [])
-
-    def test_empty_sequence_is_returned_many(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonEmpty (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonEmpty VALUES (?)", (i))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonEmpty")
-            c.fetchmany(10)
-            self.assertEqual(c.fetchmany(10), [])
-
-    def test_empty_sequence_is_returned_all(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonEmpty2 (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonEmpty2 VALUES (?)", (i))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonEmpty2")
-            c.fetchall()
-            self.assertEqual(c.fetchall(), [])
-
-    def test_empty_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonEmp (c1 NVARCHAR(128)) in pybank")
-            c.executemany("Insert INTO jonEmp VALUES (?)",
-                          (('',), ("",), (" ",)))
-            self.tstcon.commit()
-            c.execute("select * from jonEmp")
-            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
-
-    def test_empty_insert2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonEmp2 (c1 NVARCHAR(128)) in pybank")
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (''))
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (""))
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (" "))
-            self.tstcon.commit()
-            c.execute("select * from jonEmp2")
-            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
-
-    def test_invalid_databank(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bjonEmp2 (c1 NVARCHAR(128)) in potato")
-
-    def test_insert_rowcount_update(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobrowcount (c1 INTEGER, c2 NVARCHAR(256))"
-                      " in pybank")
-            string = "mimer"
-            c.execute("insert into bobrowcount values (:a, :b)", (3, string))
-            self.assertEqual(c.rowcount, 1)
-            c.executemany("insert into bobrowcount values (:a, :b)",
-                          ((5, string), (2, string)))
-            c.execute("select * from bobrowcount")
-            r = c.fetchall()
-            self.assertEqual(c.rowcount, 2)
-
-    def test_delete(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobrowcount2(c1 INTEGER) in pybank")
-            for i in range(1, 11):
-                c.execute("INSERT into bobrowcount2 values (?)", 10)
-                c.execute("INSERT into bobrowcount2 values (?)", 20)
-            c.execute("INSERT into bobrowcount2 values (?)", 10)
-            c.execute("SELECT * from bobrowcount2")
-            self.assertEqual(len(c.fetchall()), 21)
-            c.execute("DELETE from bobrowcount2 where c1 = 10")
-            self.assertEqual(c.rowcount, 11)
-            c.execute("SELECT * from bobrowcount2")
-            self.assertEqual(len(c.fetchall()), 10)
-
-    def test_update(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobupdate(c1 INTEGER) in pybank")
-            for i in range(1, 11):
-                c.execute("INSERT into bobupdate values (?)", 10)
-                c.execute("INSERT into bobupdate values (?)", 20)
-            c.execute("INSERT into bobupdate values (?)", 10)
-            c.execute("SELECT * from bobupdate")
-            self.assertEqual(len(c.fetchall()), 21)
-            c.execute("UPDATE bobupdate SET c1 = ? WHERE c1 = 20", 30)
-            self.assertEqual(c.rowcount, 10)
-            c.execute("SELECT * from bobupdate")
-            self.assertEqual(len(c.fetchall()), 21)
-
-    def test_invalid_sequence_fetchone(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonfetchone (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonfetchone VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchone()
-
-    def test_isolated(self):
-        b1 = self.tstcon.cursor()
-        b2 = self.tstcon.cursor()
-        b1.execute("create table jonisolated (c1 INTEGER) in pybank")
-        for c in range(1, 6):
-            b1.execute("Insert INTO jonisolated VALUES (?)", (c))
-        b2.execute("SELECT * FROM jonisolated")
-        c2 = b2.fetchall()
-        self.assertEqual(len(c2), 5)
-        self.assertEqual(c2, [(1,), (2,), (3,), (4,), (5,), ])
-
-    def test_isolated2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonisolated2 (c1 INTEGER) in pybank")
-            self.tstcon.commit()
-
-        cred = db_config.TSTUSR.copy()
-        cred['autocommit'] = True
-        a1 = mimerpy.connect(**cred)
-        a2 = mimerpy.connect(**cred)
-        b1 = a1.cursor()
-        b2 = a2.cursor()
-        for c in range(1, 6):
-            b1.execute("Insert INTO jonisolated2 VALUES (?)", (c))
-        b2.execute("SELECT * FROM jonisolated2 WHERE c1 < ?", 3)
-        c2 = b2.fetchall()
-        self.assertEqual(len(c2), 2)
-        self.assertEqual(c2, [(1,), (2,)])
-        b2.execute("SELECT * FROM jonisolated2")
-        c3 = b2.fetchall()
-        self.assertEqual(len(c3), 5)
-        self.assertEqual(c3, [(1,), (2,), (3,), (4,), (5,), ])
-        a1.close()
-        a2.close()
-
-    # fråga per
-    def test_isolated3(self):
-        a = mimerpy.connect(**db_config.TSTUSR)
-        b = a.cursor()
-        b.execute("create table jonisolated3 (c1 INTEGER) in pybank")
-        a.commit()
-        a.close()
-        with self.tstcon.cursor() as c:
-            for i in range(1, 6):
-                c.execute("Insert INTO jonisolated3 VALUES (?)", (i))
-            c.execute("SELECT * FROM jonisolated3")
-            c1 = c.fetchall()
-            self.assertEqual(c1, [(1,), (2,), (3,), (4,), (5,), ])
-            c.execute("SELECT * FROM jonisolated3")
-            c2 = c.fetchall()
-            self.assertEqual(c2, [(1,), (2,), (3,), (4,), (5,), ])
-
-    def test_invalid_sequence_fetchmany(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonfetchmany (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonfetchmany VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchmany(10)
-
-    def test_invalid_sequence_fetchall(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonfetchall (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonfetchall VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchall()
-
-    @unittest.skip
-    def test_UUID_one(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table uuidtable( id BUILTIN.UUID) in pybank")
-            vuuid = uuid.uuid4().bytes
-            c.execute("insert into uuidtable values(?)", (vuuid))
-            self.tstcon.commit()
-            c.execute("select id.as_text() from uuidtable")
-            r = c.fetchall()[0][0]
-            self.assertEqual(r, vuuid)
-
-    
-    def test_UUID_two(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table uuidtable2( id BUILTIN.UUID) in pybank")
-            vuuid = str(uuid.uuid1())
-            c.execute("insert into uuidtable2 values(builtin.uuid_from_text(cast(? as varchar(50))))", (vuuid))
-            self.tstcon.commit()
-            c.execute("select id.as_text() from uuidtable2")
-            r = c.fetchall()[0][0]
-            self.assertEqual(r, vuuid)
-
-    @unittest.skip
-    def test_datatype_GIS_one(self):
-        with self.tstcon.cursor() as c:
-            vuuid = '40.75,-74.0'
-            c.execute("create table gistable2( id BUILTIN.GIS_LATITUDE) in pybank")
-            c.execute("insert into gistable2 values(BUILTIN.GIS_LOCATION(40.75,-74.0))")
-            self.tstcon.commit()
-            c.execute("select id.as_text() from uuidtable2")
-            r = c.fetchall()[0][0]
-            self.assertEqual(r, vuuid)
-
-    @unittest.skip
-    def test_datatype_GIS(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table gistable2( id BUILTIN.GIS_LATITUDE) in pybank")
-            x,y = 40.75,-74.0
-            c.execute("insert into gistable2 values(BUILTIN.GIS_LOCATION(?,?))", (x,y))
-            self.tstcon.commit()
-            #c.execute("select id.as_text() from uuidtable2")
-            #r = c.fetchall()[0][0]
-            #self.assertEqual(r, vuuid)
-
-    def test_insert_blob(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonblob (c1 BLOB(18389)) in pybank")
-            ablob = bytes(bytearray("Hello there", encoding ='utf-8'))
-            c.execute("insert INTO jonblob VALUES (?)", (ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblob")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-
-    def test_insert_blob_21(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonblob2 (c1 BLOB(64111)) in pybank")
-            with open("testCursor.py", 'rb') as input_file:
-                ablob = input_file.read(200)
-                c.execute("insert INTO jonblob2 VALUES (?)", (ablob))
-                self.tstcon.commit()
-                c.execute("select * from jonblob2")
-                r = c.fetchall()[0]
-                self.assertEqual(r[0], ablob)
-
-    def test_insert_blob_multi_column(self):
-        with self.tstcon.cursor() as c:
-            ablob = ('åäö' * 1024 * 2000).encode('utf-8') 
-            c.execute("create table jonblobmulti (c1 BLOB(20m), c2 BLOB(20m)) in pybank")
-            c.execute("insert INTO jonblobmulti VALUES (?,?)", (ablob,ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblobmulti")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-    
-    def test_insert_blob_multi_column2(self):
-        with self.tstcon.cursor() as c:
-            ablob = (256).to_bytes(1024 * 10000,byteorder='big')
-            ablob2 = ('åäö' * 1024 * 3000).encode('utf-8')
-            c.execute("create table jonblobmulti2 (c1 BLOB(30m), c2 BLOB(30m), c3 BLOB(30m)) in pybank")
-            c.execute("insert INTO jonblobmulti2 VALUES (?,?,?)", (ablob,ablob,ablob2))
-            self.tstcon.commit()
-            c.execute("select * from jonblobmulti2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[2], ablob2)
-
-    def test_insert_blob_10mb(self):
-        with self.tstcon.cursor() as c:
-            ablob = (256).to_bytes(1024 * 10000,byteorder='big') 
-            c.execute("create table jonblob10 (c1 BLOB(100m)) in pybank")
-            c.execute("insert INTO jonblob10 VALUES (?)", (ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblob10")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-    
-    #@unittest.skip
-    def test_insert_blob_50mb(self):
-        with self.tstcon.cursor() as c:
-            ablob = (512).to_bytes(1024 * 50000,byteorder='big') 
-            c.execute("create table jonblob50 (c1 BLOB(100m)) in pybank")
-            c.execute("insert INTO jonblob50 VALUES (?)", (ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblob50")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-    
-    #@unittest.skip
-    def test_insert_blob_100mb(self):
-        with self.tstcon.cursor() as c:
-            ablob = (1024).to_bytes(1024 * 100000,byteorder='big') 
-            c.execute("create table jonblob100 (c1 BLOB(100m)) in pybank")
-            c.execute("insert INTO jonblob100 VALUES (?)", (ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblob100")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-
-    # Might have to up your bufferpool memory to run this
-    @unittest.skip
-    def test_insert_blob_1gb(self):
-        with self.tstcon.cursor() as c:
-            ablob = (1024).to_bytes(1024 * 1000000,byteorder='big') 
-            c.execute("create table jonblobgb (c1 BLOB(1000m)) in pybank")
-            c.execute("insert INTO jonblobgb VALUES (?)", (ablob))
-            self.tstcon.commit()
-            c.execute("select * from jonblobgb")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ablob)
-
-    def test_insert_nclob(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonnclob (c1 NCLOB(50000)) in pybank")
-            anclob = "mimer" * 1000
-            c.execute("insert INTO jonnclob VALUES (?)", (anclob))
-            self.tstcon.commit()
-            c.execute("select * from jonnclob")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], anclob)
-
-    def test_insert_nclob_unicode(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table unijonnclob (c1 NCLOB(50000)) in pybank")
-            uniclob = "安排他們參"
-            self.tstcon.commit()
-            c.execute("insert into unijonnclob values (:a)",(uniclob,))
-            self.tstcon.commit()
-            c.execute("select * from unijonnclob")
-            self.assertEqual(c.fetchall(),
-                             [(uniclob,)])
-
-    def test_insert_binary(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonbinary (c1 BINARY(3)) in pybank")
-            c.execute("insert INTO jonbinary VALUES (x'ABCD01')")
-            c.execute("insert INTO jonbinary VALUES (?)", (b'A01'))
-            self.tstcon.commit()
-            c.execute("select * from jonbinary")
-            r = c.fetchall()
-            self.assertEqual(r, [(b'\xab\xcd\x01',), (b'A01',)])
-
-    def test_insert_binary_parameter_markers(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonbinary2 (c1 BINARY(4)) in pybank")
-            bob = b"0x53"
-            c.execute("insert INTO jonbinary2 VALUES (?)", (bob))
-            self.tstcon.commit()
-            c.execute("select * from jonbinary2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], b'0x53')
-
-    def test_insert_nclob_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonnclob2 (c1 Nclob(450000)) in pybank")
-            res = ''.join(format(i, 'b') for i in bytearray("Hello there", encoding ='utf-8')) 
-            c.execute("insert INTO jonnclob2 VALUES (?)", (res))
-            self.tstcon.commit()
-            c.execute("select * from jonnclob2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], res)
-
-    def test_insert_clob(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonclob (c1 clob(30000)) in pybank")
-            aclob = "mimer" * 5
-            c.execute("insert INTO jonclob VALUES (?)", (aclob))
-            self.tstcon.commit()
-            c.execute("select * from jonclob")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], aclob)
-
-    def test_datatype_clob(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jonclob2 (c1 clob) in pybank")
-            aclob = "mimer" * 5
-            c.execute("insert INTO jonclob2 VALUES (?)", (aclob))
-            self.tstcon.commit()
-            c.execute("select * from jonclob2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], aclob)
-
-    def test_insert_date(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jondata (c1 DATE) in pybank")
-            data = "2020-09-24"
-            c.execute("insert INTO jondata VALUES (?)", (data))
-            self.tstcon.commit()
-            c.execute("select * from jondata")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], data)
-
-    def test_insert_time_one(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jontime (c1 TIME(0)) in pybank")
-            time = "16:04:55"
-            c.execute("insert INTO jontime VALUES (?)", (time))
-            self.tstcon.commit()
-            c.execute("select * from jontime")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], time)
-
-    def test_insert_time_two(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jontime2 (c1 TIME(4)) in pybank")
-            time = "16:04:55.1234"
-            c.execute("insert INTO jontime2 VALUES (?)", (time))
-            self.tstcon.commit()
-            c.execute("select * from jontime2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], time)
-    
-    def test_insert_decimal_str(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table jondecimal (c1 DECIMAL(7,2)) in pybank")
-            floatnum = '32423.23'
-            c.execute("insert INTO jondecimal VALUES (?)", (floatnum))
-            self.tstcon.commit()
-            c.execute("select * from jondecimal")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], decimal.Decimal(floatnum))
-
-    def test_insert_decimal_decimal(self):
-        with self.tstcon.cursor() as c:
-            decimal.getcontext().prec = 45
-            des = decimal.Decimal("1.14")
-            c.execute("create table jondecimal2 (c1 DECIMAL(3,2)) in pybank")
-            c.execute("insert INTO jondecimal2 VALUES (?)", (des))
-            self.tstcon.commit()
-            c.execute("select * from jondecimal2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], des)
-
-    # Bör runda av, men ger för tillfället en exception
-    @unittest.skip
-    def test_insert_decimal_decimal2(self):
-        with self.tstcon.cursor() as c:
-            decimal.getcontext().prec = 45
-            des = decimal.Decimal("1.141")
-            c.execute("create table jondecimal2 (c1 DECIMAL(3,2)) in pybank")
-            c.execute("insert INTO jondecimal2 VALUES (?)", (des))
-            self.tstcon.commit()
-            c.execute("select * from jondecimal2")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], des)
-
-    def test_insert_decimal_decimal3(self):
-        with self.tstcon.cursor() as c:
-            decimal.getcontext().prec = 45
-            des = decimal.Decimal("1.14")
-            c.execute("create table jondecimal22 (c1 DECIMAL(3,2)) in pybank")
-            c.execute("insert INTO jondecimal22 VALUES (cast(cast('1.141' as varchar(20)) as DECIMAL(3,2)))")
-            self.tstcon.commit()
-            c.execute("select * from jondecimal22")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], des)
-
-    def test_insert_decimal_none(self):
-        with self.tstcon.cursor() as c:
-            decimal.getcontext().prec = 45
-            c.execute("create table jondecimalnone (c1 DECIMAL(3,2)) in pybank")
-            c.execute("insert INTO jondecimalnone VALUES (?)", (None))
-            self.tstcon.commit()
-            c.execute("select * from jondecimalnone")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], None)
-
-    def test_datatype_interval_DAY(self):
-        with self.tstcon.cursor() as c:
-            day = "20005"
-            c.execute("create table jonday (c1 INTERVAL DAY(5)) in pybank")
-            c.execute("insert INTO jonday VALUES (?)", (day))
-            self.tstcon.commit()
-            c.execute("select * from jonday")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], day)
-
-    def test_datatype_interval_HOUR(self):
-        with self.tstcon.cursor() as c:
-            hour = "20005"
-            c.execute("create table jonhour (c1 INTERVAL HOUR(5)) in pybank")
-            c.execute("insert INTO jonhour VALUES (?)", (hour))
-            self.tstcon.commit()
-            c.execute("select * from jonhour")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], hour)
-
-    def test_datatype_interval_MINUTE(self):
-        with self.tstcon.cursor() as c:
-            minute = "1234567890"
-            c.execute("create table jonminute (c1 INTERVAL MINUTE(10)) in pybank")
-            c.execute("insert INTO jonminute VALUES (?)", (minute))
-            self.tstcon.commit()
-            c.execute("select * from jonminute")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], minute)
-
-    def test_datatype_interval_year(self):
-        with self.tstcon.cursor() as c:
-            year = "20005"
-            c.execute("create table jonyear (c1 INTERVAL year(5)) in pybank")
-            c.execute("insert INTO jonyear VALUES (?)", (year))
-            self.tstcon.commit()
-            c.execute("select * from jonyear")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], year)
-
-    def test_datatype_interval_SECOND(self):
-        with self.tstcon.cursor() as c:
-            second = "20005.000000"
-            c.execute("create table jonsecond (c1 INTERVAL SECOND(5)) in pybank")
-            c.execute("insert INTO jonsecond VALUES (?)", (second))
-            self.tstcon.commit()
-            c.execute("select * from jonsecond")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], second)
-
-    def test_datatype_interval_SECOND_P(self):
-        with self.tstcon.cursor() as c:
-            second = "12345.67"
-            c.execute("create table jonsecondp (c1 INTERVAL SECOND(5,2)) in pybank")
-            c.execute("insert INTO jonsecondp VALUES (?)", (second))
-            self.tstcon.commit()
-            c.execute("select * from jonsecondp")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], second)
-
-    def test_datatype_interval_YEAR_TO_MONTH(self):
-        with self.tstcon.cursor() as c:
-            ym = "5-10"
-            c.execute("create table jonytm (c1 INTERVAL YEAR(5) TO MONTH) in pybank")
-            c.execute("insert INTO jonytm VALUES (?)", (ym))
-            self.tstcon.commit()
-            c.execute("select * from jonytm")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], ym)
-
-    def test_datatype_interval_DAY_TO_HOUR(self):
-        with self.tstcon.cursor() as c:
-            dhms = "5 23"
-            c.execute("create table jondth (c1 INTERVAL DAY(5) TO HOUR) in pybank")
-            c.execute("insert INTO jondth VALUES (?)", (dhms))
-            self.tstcon.commit()
-            c.execute("select * from jondth")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], dhms)
-
-    def test_datatype_interval_DAY_TO_MINUTE(self):
-        with self.tstcon.cursor() as c:
-            dhm = "5 23:55"
-            c.execute("create table jondtm (c1 INTERVAL DAY(5) TO MINUTE) in pybank")
-            c.execute("insert INTO jondtm VALUES (?)", (dhm))
-            self.tstcon.commit()
-            c.execute("select * from jondtm")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], dhm)
-
-    def test_datatype_interval_DAY_TO_SECOND(self):
-        with self.tstcon.cursor() as c:
-            dhms = "5 23:05:01.123"
-            c.execute("create table jondts (c1 INTERVAL DAY(5) TO SECOND(3)) in pybank")
-            c.execute("insert INTO jondts VALUES (?)", (dhms))
-            self.tstcon.commit()
-            c.execute("select * from jondts")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], dhms)
-
-    def test_datatype_interval_HOUR_TO_MINUTE(self):
-        with self.tstcon.cursor() as c:
-            hts = "55555:01"
-            c.execute("create table jonhtm (c1 INTERVAL HOUR(5) TO MINUTE) in pybank")
-            c.execute("insert INTO jonhtm VALUES (?)", (hts))
-            self.tstcon.commit()
-            c.execute("select * from jonhtm")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], hts)
-
-    def test_datatype_interval_HOUR_TO_SECOND(self):
-        with self.tstcon.cursor() as c:
-            hts = "55555:23:02.12345"
-            c.execute("create table jonhts (c1 INTERVAL HOUR(5) TO SECOND(5)) in pybank")
-            c.execute("insert into jonhts values(cast(? as interval HOUR(5) to second(5)))", (hts))
-            #c.execute("insert INTO jonhts VALUES (?)", (hts))
-            self.tstcon.commit()
-            c.execute("select * from jonhts")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], hts)
-
-    def test_datatype_interval_MINUTE_TO_SECOND(self):
-        with self.tstcon.cursor() as c:
-            minute = '12345:12.12345679'
-            c.execute("create table jonmts (c1 INTERVAL MINUTE(5) TO SECOND(8)) in pybank")
-            c.execute("insert into jonmts values (?)", minute)
-            self.tstcon.commit()
-            c.execute("select * from jonmts")
-            r = c.fetchall()
-            self.assertEqual(r[0][0], minute)
-            
-    def test_insert_bool(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobybool (c1 boolean) in pybank")
-            c.execute("insert INTO bobybool VALUES (?)", (False))
-            c.execute("insert INTO bobybool VALUES (?)", (45))
-            self.tstcon.commit()
-
-    def test_select_bool(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobybool2 (c1 boolean) in pybank")
-            c.execute("insert INTO bobybool2 VALUES (?)", (False))
-            c.execute("insert INTO bobybool2 VALUES (?)", (45))
-            self.tstcon.commit()
-            c.execute("select * from bobybool2")
-            r = c.fetchone()
-            self.assertEqual(r[0], False)
-            r = c.fetchone()
-            self.assertEqual(r[0], True)
-
-    def test_get_connection(self):
-        c = self.tstcon.cursor()
-        self.assertEqual(c.connection, self.tstcon)
-        c.close()
-
-    def test_for(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table fortable (c1 INTEGER, c2 INTEGER)"
-                      " in pybank")
-            c.execute("insert INTO fortable VALUES (?,?)", (1,99))
-            c.execute("insert INTO fortable VALUES (?,?)", (3,97))
-            c.execute("insert INTO fortable VALUES (?,?)", (10,90))
-            c.execute("select * from fortable")
-            count = 0
-            for val in c:
-                self.assertEqual(val[0]+val[1], 100)
-                count = count + 1
-            self.assertEqual(count, 3)
-
-    def test_result_set_twice(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table kor (c1 INTEGER) in pybank")
-            c.execute("insert INTO kor VALUES (?)", (45))
-            c.execute("select * from kor")
-            for val in c:
-                self.assertEqual(val[0], 45)
-            c.execute("select * from kor")
-            c.execute("select c1 from kor")
-
-    def test_executemany_none(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table manytable (c1 INTEGER) in pybank")
-            c.executemany("insert INTO manytable VALUES (?)",
-                          [(2,), (34,), (435,), (34,), (63,), (47,), (None,)])
-            self.tstcon.commit()
-
-    def test_select_executemany(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobyselect (c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert INTO bobyselect VALUES (?)", (1))
-            with self.assertRaises(ProgrammingError):
-                c.executemany("select * from bobyselect where c1 = (?)",
-                              ((5,), (10,)))
-
-    def test_select_twice(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bananaselect (c1 INTEGER) in pybank")
-            c.execute("select * from bananaselect where c1 = (?)", (5))
-            c.execute("select c1 from bananaselect where c1 = (?)", (7))
-
-    def test_fetchall_no_select(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(ProgrammingError):
-                c.fetchall()
-
-    def test_bool_insert(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table boolt (c1 BOOLEAN) in pybank")
-            c.executemany("insert into boolt values (?)",
-                          [(None,), (1,), (0,), (3.1415,),
-                           ("potato",), ('code',)])
-            c.execute("select * from boolt")
-            r = c.fetchall()
-            self.assertEqual(r, [(None,), (True,), (False,),
-                                 (True,), (True,), (True,)])
-
-    def test_insert_parametermarkers_different_types(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob176(c1 NVARCHAR(128)) in pybank")
-            c.execute("INSERT INTO bob176 VALUES (?)", "bar")  # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ("bar"))  # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ("bar",))  # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ["bar"])  # correct
-            self.tstcon.commit()
-            c.execute("select * from bob176")
-            self.assertEqual(c.fetchall(), [("bar",), ("bar",),
-                                            ("bar",), ("bar",)])
-
-    def test_insert_parametermarkers_different_types2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bobd(c1 NVARCHAR(128), c2 INTEGER,"
-                      "                  c3 FLOAT) in pybank")
-            c.execute("INSERT INTO bobd VALUES (?,?,?)",
-                      ("bar", 314, 41.23))
-            c.execute("INSERT INTO bobd VALUES (?,?,?)",
-                      ("bar", 315, 41.23,))
-            with self.assertRaises(ProgrammingError):
-                c.execute("INSERT INTO bobd VALUES (?,?,?)",
-                          "bar", (316), (41.23))
-            c.execute("INSERT INTO bobd VALUES (?,?,?)",
-                      ["bar", 317, 41.23])
-            self.tstcon.commit()
-            c.execute("select * from bobd")
-            self.assertEqual(c.fetchall(),
-                             [('bar', 314, 41.23),
-                              ('bar', 315, 41.23),
-                              ('bar', 317, 41.23)])
-
-    def test_char_table(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table charbob(c1 CHAR(10)) in pybank")
-            c.execute("INSERT INTO charbob VALUES ('Kalle Kula')")
-            self.tstcon.commit()
-            c.execute("select * from charbob")
-            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
-
-    def test_invalid_char(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table invalidbob(c1 CHAR(10)) in pybank")
-            # kastar inget fel för tillfället, vilket är micro api's fel,
-            # men inget vi ska lösa just nu
-            # &&&& Fixme!
-            c.execute("INSERT INTO invalidbob VALUES ('?')", ("ィキペデ"))
-            with self.assertRaises(DataError):
-                c.execute("INSERT INTO invalidbob VALUES ('ィキペデ')")
-            self.tstcon.commit()
-            c.execute("select * from invalidbob")
-            r = c.fetchall()
-
-
-    def test_varchar_table(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table varcharbob(c1 VARCHAR(128)) in pybank")
-            c.execute("INSERT INTO varcharbob VALUES ('Kalle Kula')")
-            self.tstcon.commit()
-            c.execute("select * from varcharbob")
-            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
-
-    def test_nchar_table(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table ncharbob(c1 VARCHAR(128)) in pybank")
-            c.execute("INSERT INTO ncharbob VALUES ('Kalle Kula')")
-            self.tstcon.commit()
-            c.execute("select * from ncharbob")
-            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
-
-    def test_callproc_nextset(self):
-        with self.tstcon.cursor() as c:
-            with self.assertRaises(NotSupportedError):
-                c.nextset()
-            with self.assertRaises(NotSupportedError):
-                c.callproc()
-
-    def test_insert_blob_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("CREATE TABLE blob_table (blobcolumn BLOB)")
-            blob = bytes(bytearray("Hello there again", encoding ='utf-8'))
-            c.execute("INSERT INTO blob_table VALUES (?)", (blob))
-            self.tstcon.commit()
-            c.execute("SELECT * FROM blob_table")
-            r = c.fetchall()[0][0]
-            self.assertEqual(r, blob)
-
-    def test_conflict_drop(self):
-        with self.tstcon.cursor() as c:
-            mytuplelist = list(zip(list(range(100)), list(range(100))))
-            c.execute("CREATE TABLE conflict_test2 (int1 INTEGER, int2 INTEGER)")
-            c.executemany("INSERT INTO conflict_test2 VALUES (?,?)", (mytuplelist))
-            self.tstcon.commit()
-
-        conn1 = mimerpy.connect(**db_config.TSTUSR)
-        conn2 = mimerpy.connect(**db_config.TSTUSR)
-        conn1.execute("INSERT INTO conflict_test2 VALUES (?,?)", (200,200))
-        with self.assertRaises(OperationalError) as e:
-            conn2.execute("DROP TABLE conflict_test2 CASCADE")
-        self.assertEqual(-16001, e.exception.errno)
-        self.assertEqual("Table MIMERPY.conflict_test2 locked by another user", e.exception.message)
-        conn1.close()
-        conn2.close()
-    
-    def test_conflict_insert(self):
-        with self.tstcon.cursor() as c:
-            mytuplelist = list(zip(list(range(100)), list(range(100))))
-            c.execute("CREATE TABLE conflict_test3 (int1 INTEGER, int2 INTEGER, PRIMARY KEY (int1))")
-            c.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
-            self.tstcon.commit()
-
-        conn1 = mimerpy.connect(**db_config.TSTUSR)
-        conn2 = mimerpy.connect(**db_config.TSTUSR)
-        mytuplelist = list(zip(list(range(200,300)), list(range(200, 300))))
-        conn1.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
-        conn2.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
-        conn1.commit()
-        with self.assertRaises(TransactionAbortError) as e:
-            conn2.commit()
-        self.assertEqual(-10001, e.exception.errno)
-        self.assertEqual("Transaction aborted due to conflict with other transaction", e.exception.message)
-        conn1.close()
-        conn2.close()
-
-    def test_conflict_update(self):
-        with self.tstcon.cursor() as c:
-            mytuplelist = list(zip(list(range(100)), list(range(100))))
-            c.execute("CREATE TABLE conflict_test4 (int1 INTEGER, int2 INTEGER)")
-            c.executemany("INSERT INTO conflict_test4 VALUES (?,?)", (mytuplelist))
-            self.tstcon.commit()
-
-        conn1 = mimerpy.connect(**db_config.TSTUSR)
-        conn2 = mimerpy.connect(**db_config.TSTUSR)
-        conn1.execute("UPDATE conflict_test4 SET int1 = 500 where int1 = 50")
-        conn2.execute("UPDATE conflict_test4 SET int1 = 555 where int1 = 50")
-        conn1.commit()
-        with self.assertRaises(OperationalError) as e:
-            conn2.commit()
-        self.assertEqual(-10001, e.exception.errno)
-        self.assertEqual("Transaction aborted due to conflict with other transaction", e.exception.message)
-        conn1.close()
-        conn2.close()
-
-    # these are the test examples for the documentaion
-    def test_for_doc_1(self):
-        with self.tstcon.cursor() as c:
-            c.execute("CREATE TABLE with_table_cursor1(c1 INTEGER,"
-                      "                            c2 VARCHAR(32)) in pybank")
-            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
-                      (1, "This is an example"))
-            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
-                      (2, "on how to use"))
-            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
-                      (3, "the with functionality."))
-        with self.tstcon.cursor() as c:
-            c.execute("SELECT * from with_table_cursor1")
-
-    # these are the test examples for the documentaion
-    @unittest.skip
-    def test_for_doc_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("CREATE TABLE with_table_connection1(c1 INTEGER,"
-                             " c2 VARCHAR(32)) in pybank")
-        self.tstcon.commit()
-
-        with mimerpy.connect(**db_config.TSTUSR) as con:
-            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
-                        (1, "This is an example"))
-            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
-                        (2, "on how to use"))
-            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
-                        (3, "the with functionality."))
-            con.commit()
-
-        with mimerpy.connect(**db_config.TSTUSR) as con:
-            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
-                        (4, "Commit forgotten"))
-
-        cred = db_config.TSTUSR.copy()
-        cred['autocommit'] = True
-        with mimerpy.connect(**cred) as con:
-            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
-                        (5, "Autocommitted"))
-
-        with self.tstcon.cursor() as c:
-            c.execute("SELECT * from with_table_connection1")
-            self.assertEqual(c.fetchall(),
-                             [(1, 'This is an example'),
-                              (2, 'on how to use'),
-                              (3, 'the with functionality.'),
-                              (5, 'Autocommitted')])
-
-    # Inconsistent errors, needs to be fixed!
-    def test_invalid_NULL(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table boberror (c1 INTEGER not null,"
-                      "                c2 NVARCHAR(10) not null) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into boberror values (:a, :b)", (None, None))
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into boberror values (:a, :b)", (1, None))
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into boberror values (:a, :b)", (None, 'Hej'))
-            with self.assertRaises(DataError):
-                c.execute("insert into boberror values (NULL, NULL)")
-
-            c.execute("SELECT * from boberror")
-            self.assertEqual(c.fetchall(), [])
-
-    def test_bool_null(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table boolbob3 (c1 boolean)")
-            c.execute("insert into boolbob3 values (?)", (None))
-
-            c.execute("SELECT * from boolbob3")
-            self.assertEqual(c.fetchone(), (None,))
-
-    def test_unsupported_data_type(self):
-        with self.tstcon.cursor() as c:
-            long = """
-create table longboi (c1 char(10),
-                      c2 varchar(10),
-                      c3 CLOB(2000),
-                      c4 nchar(10),
-                      c5 nvarchar(30),
-                      c6 nclob(2000),
-                      c7 binary(2),
-                      c8 varbinary(2),
-                      c9 blob(1024),
-                      c10 SMALLINT,
-                      c11 INTEGER,
-                      c12 BIGINT,
-                      c13 INTEGER(2),
-                      c14 DECIMAL(5,2),
-                      c15 REAL,
-                      c16 DOUBLE PRECISION,
-                      c17 FLOAT,
-                      c18 DATE,
-                      c19 TIME(0),
-                      c20 TIMESTAMP(6)) in pybank"""
-            c.execute(long)
-            c.execute("insert into longboi (c4) values (?)", ("dude", ))
-
-# &&&& Add values in static SQL and then try to get individual columns
-# &&&& Then try to set individual columns from Python
-
-            c.execute("SELECT * from longboi")
-            self.assertEqual(c.fetchone(), (None, None, None, 'dude      ',
-                                            None, None, None, None, None,
-                                            None, None, None, None, None,
-                                            None, None, None, None, None, None))
-
-    def test_data_type_varbinary(self):
-        with self.tstcon.cursor() as c:
-            long = "create table longboi_varbinary (c1 VARBINARY(10)) in pybank"
-            c.execute(long)
-            c.execute("insert into longboi_varbinary values (?)", (b"x'ABCD01"))
-
-            c.execute("SELECT * from longboi_varbinary")
-            self.assertEqual(c.fetchall(), [(b"x'ABCD01",)])
-
-    def test_data_type_smallint(self):
-        with self.tstcon.cursor() as c:
-            long = "create table longboi_smallint (c1 SMALLINT) in pybank"
-            c.execute(long)
-            c.execute("insert into longboi_smallint values (?)", (32000))
-
-            c.execute("SELECT * from longboi_smallint")
-            self.assertEqual(c.fetchall(), [(32000,)])
-
-    def test_data_type_bigint(self):
-        with self.tstcon.cursor() as c:
-            long = "create table longboi_bigint(c1 BIGINT) in pybank"
-            c.execute(long)
-            c.execute("insert into longboi_bigint values (?)", (-2**63))
-
-            c.execute("SELECT * from longboi_bigint")
-            self.assertEqual(c.fetchall(), [(-2**63,)])
-
-    @unittest.skip
-    def test_data_type_precision_integer(self):
-        with self.tstcon.cursor() as c:
-            long = "create table longboi_integer45(c1 INTEGER(45)) in pybank"
-            c.execute(long)
-            c.execute("insert into longboi_integer45 values (?)", str(2**145))
-
-            c.execute("SELECT * from longboi_integer45")
-            self.assertEqual(c.fetchall(), [(str(2**140),)])
-
-    def test_parameter_name(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name (c1 boolean,c2 nchar(10),"
-                      "                       c3 int) in pybank")
-            c.execute("insert into bob_name (c1,c3) values (:a,:b)",
-                      {'a':True, 'b':3})
-
-            c.execute("SELECT * from bob_name")
-            self.assertEqual(c.fetchone(), (True, None, 3))
-
-    def test_error_message(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_message (c1 nchar(10)) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into bob_message (c1,c3) values (:a,:b)",
-                        {'a':2,})
-            print()
-            self.assertEqual(c.messages[0][1], (-12202, 'c3 is not a column of an inserted table, updated table or any table identified in a FROM clause'))
-
-    def test_error_exception_errno(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_message_1 (c1 nchar(10)) in pybank")
-            with self.assertRaises(ProgrammingError) as e:
-                c.execute("insert into bob_message_1 (c1,c3) values (:a,:b)",
-                        {'a':2,})
-            self.assertEqual(e.exception.errno, -12202)
-    
-    def test_error_exception_message(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_message_2 (c1 nchar(10)) in pybank")
-            with self.assertRaises(ProgrammingError) as e:
-                c.execute("insert into bob_message_2 (c1,c3) values (:a,:b)",
-                        {'a':2,})
-            self.assertEqual(e.exception.message, "c3 is not a column of an inserted table, updated table or any table identified in a FROM clause")
-    
-    def test_error_exception_str(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_message_3 (c1 nchar(10)) in pybank")
-            with self.assertRaises(ProgrammingError) as e:
-                c.execute("insert into bob_message_3 (c1,c3) values (:a,:b)",
-                        {'a':2,})
-            self.assertEqual(str(e.exception), "-12202 c3 is not a column of an inserted table, updated table or any table identified in a FROM clause")
-
-    def test_parameter_name_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name_2(c1 boolean, c2 nchar(10),"
-                      "                        c3 int) in pybank")
-            c.execute("insert into bob_name_2 (c1,c3,c2) values (:a,:b,:g)",
-                      dict(a=True, b=3, g="bobs table"))
-
-            c.execute("SELECT * from bob_name_2")
-            self.assertEqual(c.fetchone(), (True, "bobs table", 3))
-
-    def test_parameter_name_missing_key(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table pname_miss(c1 boolean,c2 nchar(10),"
-                      "                        c3 int) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("insert into pname_miss(c1,c2) values (:a,:b)",
-                          {'a':True, 'g':3})
-
-    def test_parameter_name_execute_many(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name_e(c1 boolean,c2 nchar(10),"
-                      "                        c3 int) in pybank")
-            c.executemany("insert into bob_name_e(c1,c3) values (:a,:b)",
-                          [{'a':True, 'b':1},
-                           {'a':False, 'b':2},
-                           {'a':True, 'b':3}])
-
-            c.execute("SELECT * from bob_name_e")
-            self.assertEqual(c.fetchall(),
-                             [(True, None, 1),
-                              (False, None, 2),
-                              (True, None, 3)])
-
-    def test_parameter_name_execute_many_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table pname__e2 (c1 boolean,c2 nchar(10),"
-                      "                        c3 int) in pybank")
-            c.executemany("insert into pname__e2 (c1,c3,c2) values (:a,:b,:g)",
-                          [{'a': True, 'b': 1, 'g': "bob table1"},
-                           {'a': False, 'b': 2, 'g': "bob table2"},
-                           {'a': True, 'b': 3, 'g': "bob table3"}])
-            c.execute("SELECT * from pname__e2")
-            self.assertEqual(c.fetchall(),
-                             [(True, 'bob table1', 1),
-                              (False, 'bob table2', 2),
-                              (True, 'bob table3', 3)])
-
-    def test_parameter_name_execute_many_invalid_key(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name_invalid(c1 boolean,c2 nchar(10),"
-                      "                              c3 int) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob_name_invalid (c1,c2)"
-                              " values (:a,:b)",
-                              [{'a':True, 'g':3},
-                               {'a':True, 'g':3}])
-
-    def test_parameter_name_execute_many_mixing(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name__e3 (c1 boolean,c2 nvarchar(10),"
-                      "                           c3 int) in pybank")
-            c.executemany("insert into bob_name__e3 (c1,c2,c3)"
-                          " values (:a,:b,:g)",
-                          [{'a': True, 'g': 1, 'b': "bob table1"},
-                           (True, "string ?", 5),
-                           (True, "string", 5)])
-            c.execute("SELECT * from bob_name__e3")
-            self.assertEqual(c.fetchall(),
-                             [(True, 'bob table1', 1),
-                              (True, 'string ?', 5),
-                              (True, 'string', 5)])
-
-    def test_parameter_name_execute_many_mixing_2(self):
-        with self.tstcon.cursor() as c:
-            c.execute("create table bob_name__e4 (c1 boolean,c2 nvarchar(10),"
-                      "                           c3 int) in pybank")
-            c.executemany("insert into bob_name__e4 (c1,c3,c2)"
-                          " values (:a,:b,:g)",
-                          [(True, 5,"string"),
-                           {'a': True, 'b': 1, 'g': "bob table1"},
-                           (True, 5, "string ?")])
-            c.execute("SELECT * from bob_name__e4")
-            self.assertEqual(c.fetchall(),
-                             [(True, 'string', 5),
-                              (True, 'bob table1', 1),
-                              (True, 'string ?', 5)])
-
-    @unittest.skip
-    def test_help(self):
-        a = mimerpy.connect(dsn=self.dbName, user=self.usrName, password=self.psw)
-        b = a.cursor()
-        help(b)
-        b.close()
-        a.close()
-
-    @unittest.skip
-    def test_error(self):
-        a = mimerpy.connect(dsn=self.dbName, user=self.usrName, password=self.psw)
-        b = a.cursor()
-        b.execute("create table boberror (c1 INTEGER,  c2 NVARCHAR(10)) in pybank")
-        print("table created --------------- ")
-        b.execute("insert into boberror values (:a, :b)", (3, 'bob'))
-        a.close()
-
-
-    if (mimerapi._level == 2):
-        def test_datatype_float_p(self):
-            with self.tstcon.cursor() as c:
-                c.execute("create table floatptable (c1 FLOAT(5)) in pybank")
-                floatnum = str(3.123)
-                c.execute("insert INTO floatptable VALUES (?)", (floatnum))
-                self.tstcon.commit()
-                c.execute("select * from floatptable")
-                r = c.fetchall()[0]
-                self.assertEqual(r[0], decimal.Decimal(floatnum))
-
-        def test_datatype_numeric(self):
-            with self.tstcon.cursor() as c:
-                c.execute("create table floatnumericptable (c1 numeric(5,2)) in pybank")
-                floatnum = str(322.13)
-                c.execute("insert INTO floatnumericptable VALUES (?)", (floatnum))
-                self.tstcon.commit()
-                c.execute("select * from floatnumericptable")
-                r = c.fetchall()[0]
-                self.assertEqual(r[0], decimal.Decimal(floatnum))
-
-        @unittest.skipUnless(db_config.MIMERPY_STABLE == False, "Currently gives incorrect error message")
-        def test_insert_decimal_invalid(self):
-            with self.tstcon.cursor() as c:
-                c.execute("create table jondecimal2 (c1 DECIMAL(5,2)) in pybank")
-                floatnum = '32423.23234'
-                #with self.assertRaises(ProgrammingError):
-                c.execute("insert INTO jondecimal2 VALUES (?)", (floatnum))
-
-
-if __name__ == '__main__':
-    unittest.TestLoader.sortTestMethodsUsing = None
-    unittest.main()
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import unittest, time, math, random, uuid, decimal
+import mimerpy, mimerapi
+from mimerpy.mimPyExceptions import *
+import db_config
+
+
+# noinspection SqlDialectInspection
+class TestCursorMethods(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(self):
+        (self.syscon, self.tstcon) = db_config.setup()
+
+    @classmethod
+    def tearDownClass(self):
+        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
+
+    def tearDown(self):
+        self.tstcon.rollback()
+
+########################################################################
+## Tests below
+########################################################################
+
+    def test_fetchall_ts(self):
+        with self.tstcon.cursor() as c:
+            c.execute("select 'a', cast('2020-09-17 11:21:51' as timestamp(2)) from system.onerow")
+            self.assertEqual(c.fetchall(), [('a', '2020-09-17 11:21:51.00')])
+
+    def test_fetchall_timestamp_one(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_timestamp(c1 TIMESTAMP(2)) in pybank")
+            c.execute("insert into bob_timestamp values (:a)", ('2020-09-17 11:21:51'))
+            self.tstcon.commit()
+            c.execute("select * from bob_timestamp")
+            r = c.fetchone()
+            self.assertEqual(r, ('2020-09-17 11:21:51.00',))
+
+    def test_fetchall_timestamp_two(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_timestamp2(c1 TIMESTAMP(9)) in pybank")
+            c.execute("insert into bob_timestamp2 values (:a)", ('2020-09-17 11:21:51.123456789'))
+            self.tstcon.commit()
+            c.execute("select * from bob_timestamp2")
+            r = c.fetchone()
+            self.assertEqual(r, ('2020-09-17 11:21:51.123456789',))
+
+    def test_privilege(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(DatabaseError):
+                c.execute("drop ident sysadm cascade")
+
+    def test_createTable(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+
+    def test_createTable_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobcr1(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("create table bobcr2(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("create table bobcr3(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("create table bobcr4(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+        self.tstcon.commit()
+
+    def test_createTable_DropTable(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("drop table bob2 CASCADE")
+        self.tstcon.commit()
+
+    def test_create_invalid_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon (c1 INTEGER, c2 INTEGER) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("banana INTO jon VALUES (3, 14)")
+
+# &&&& This test should fail when we can rollback DDL
+    def test_create_rollback_table(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonnynothere (c1 INTEGER, c2 INTEGER)"
+                      " in pybank")
+            self.tstcon.rollback()
+            c.execute("select * from jonnynothere")
+
+    def test_two_select(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonny (c1 INTEGER, c2 INTEGER) in pybank")
+            c.execute("select c1 from jonny where c1 = (?)", (2))
+            c.execute("select * from jonny")
+
+    def test_many_select(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob356 (c1 INTEGER) in pybank")
+            for val in range(100):
+                c.execute("insert into bob356 values (:a)", (val))
+            for gal in range(100):
+                c.execute("select c1 from bob356 where c1 > (?)", (gal))
+                r = c.fetchall()
+                # &&&& Check resultset
+
+    def test_select_no_commit(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobc (c1 INTEGER, c2 FLOAT) in pybank")
+            for val in range(100):
+                c.execute("insert into bobc values (:a, :b)", (val, val + 0.5))
+            c.execute("select * from bobc where c1 = 99")
+            self.assertEqual(c.fetchall(), [(99, 99.5)])
+
+    def test_select_description(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table description (columnone INTEGER) in pybank")
+            for val in range(10):
+                c.execute("insert into description values (?)", val)
+            c.execute("select * from description")
+            self.assertEqual(c.description,
+                             (('columnone', 50, None, None, None, None, None),))
+
+    def test_select_description2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table description2 (c1 INTEGER, c2 FLOAT)"
+                      " in pybank")
+            for val in range(10):
+                c.execute("insert into description2 values (?,?)",
+                          (val, val / 3))
+            c.execute("select * from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),
+                              ('c2', 56, None, None, None, None, None)))
+            c.execute("select c1 from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),))
+            c.execute("select c2 from description2")
+            self.assertEqual(c.description,
+                             (('c2', 56, None, None, None, None, None),))
+            c.execute("select * from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),
+                              ('c2', 56, None, None, None, None, None)))
+
+    def test_select_description3(self):
+        with self.tstcon.cursor() as c:
+            c.execute("""create table description3(price INTEGER,
+                                      currentvalue FLOAT,
+                                      currency NVARCHAR(128),
+                                      rate BIGINT,
+                                      currentyear INTEGER) in pybank""")
+            for val in range(10):
+                c.execute("insert into description3 values (?,?,?,?,?)",
+                          (val, val / 3, 'SEK', 2 ** 61, val + 2000))
+            c.execute("select * from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentvalue', 56, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None)))
+            c.execute("select price, currentyear, currency, rate from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None)))
+            c.execute("select rate, rate, rate, rate from description3")
+            self.assertEqual(c.description,
+                             (('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None)))
+            c.execute("select * from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentvalue', 56, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None)))
+
+    def test_select_description4(self):
+        with self.tstcon.cursor() as c:
+            name1 = "e" * 127 + "q"
+            name2 = "m" * 127 + "q"
+            query = ("create table description4 (" + name1 + " INTEGER, "
+                     + name2 + " BOOLEAN) in pybank")
+            c.execute(query)
+            for val in range(10):
+                c.execute("insert into description4 values (?,?)",
+                          (val, val % 2))
+            c.execute("select * from description4")
+            self.assertEqual(c.description,
+                             ((name1, 50, None, None, None, None, None),
+                              (name2, 42, None, None, None, None, None)))
+
+    def test_select_description5(self):
+        with self.tstcon.cursor() as c:
+            name1 = "e" * 127 + "q"
+            name2 = "m" * 127 + "q"
+            query = ("create table description5 (" + name1 + " INTEGER, " +
+                     name2 + " BOOLEAN) in pybank")
+            c.execute(query)
+            for val in range(10):
+                c.execute("insert into description5 values (?,?)",
+                          (val, val % 2))
+            c.execute("select * from description5")
+            self.assertEqual(c.description,
+                             ((name1, 50, None, None, None, None, None),
+                              (name2, 42, None, None, None, None, None)))
+
+    def test_invalid_create(self):
+        b = self.tstcon.cursor()
+        b.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("create table jon(i int) in pybank")
+
+    def test_insert_parametermarkers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob1 (c1 INTEGER,  c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("insert into bob1 values (:a, :b)", (3, 'bob'))
+
+    def test_insert_parametermarkers_long_string(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobstring (c1 INTEGER,  c2 NVARCHAR(256))"
+                      " in pybank")
+            string = "mimer" * 40
+            c.execute("insert into bobstring values (:a, :b)", (3, string))
+            self.tstcon.commit()
+            c.execute("select c2 from bobstring")
+            self.assertEqual(c.fetchall(), [(string,)])
+
+    def test_insert_parametermarkers_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob13 (c1 INTEGER, c2 NVARCHAR(10),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            pmarkers = [(1, 'pi', 14.345),
+                           (2, 'pii', 14.345),
+                           (-3, 'piii', 14.345),
+                           (7, 'piii', 14.345),
+                           (1121231, 'piiii', 14.345)]
+            c.executemany("insert into bob13 values (:a, :b, :c)",
+                         pmarkers)
+            self.tstcon.commit()
+            c.execute("select * from bob13")
+            self.assertEqual(c.fetchall(),
+                            pmarkers)
+
+    def test_insert_parametermarkers_russian(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob14 (c1 INTEGER, c2 NVARCHAR(128),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob14 values (:a, :b, :c)",
+                          ((1, 'продиктованной ангелом', 14.345),
+                           (2, '安排他們參', 14.345)))
+            self.tstcon.commit()
+            c.execute("select * from bob14")
+            self.assertEqual(c.fetchall(),
+                             [(1, 'продиктованной ангелом', 14.345),
+                              (2, '安排他們參', 14.345)])
+
+    def test_insert_parametermarkers_unicode(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table boby14 (c1 INTEGER, c2 NVARCHAR(128),"
+                      "                     c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into boby14 values (:a, :b, :c)",
+                          ((1, 'продиктованной ангелом', 14.345),
+                           (2, '安排他們參‱', 14.345)))
+            self.tstcon.commit()
+            c.execute("select * from boby14")
+            self.assertEqual(c.fetchall(),
+                             [(1, 'продиктованной ангелом', 14.345),
+                              (2, '安排他們參‱', 14.345)])
+
+    def test_insert_parametermarkers_goodchar(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobg14(c1 char(10)) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bobg14 values (?)", 'åååååååååå')
+            self.tstcon.commit()
+            c.execute("select * from bobg14")
+            self.assertEqual(c.fetchall(),
+                             [('åååååååååå',)])
+
+    def test_insert_parametermarkers_illchar(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobz14(c1 char(10)) in pybank")
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into bobz14 values (?)", '安排')
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into bobz14 values (?)", '€')
+
+    def test_insert_parametermarkers_too_long(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob15 (c1 NVARCHAR(10)) in pybank")
+            self.tstcon.commit()
+            with self.assertRaises(DatabaseError):
+                c.execute("insert into bob15 values (:a)",
+                          ('This sentence is too long'))
+        self.tstcon.commit()
+
+    def test_insert_too_few_parametermarkers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob3 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            with self.assertRaises(DatabaseError):
+                c.execute("insert into bob3 values (:a, :b)", (3))
+
+    def test_insert_too_many_parametermarkers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob33 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob33 values (:a, :b)",
+                              ((3, 'pi', 14), (3)))
+
+    def test_insert_parametermarkers_dict(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table poff_dict1 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("insert into poff_dict1 values (:a, :b)",
+                              {'a':3, 'b':'pi'})
+        self.tstcon.commit()
+
+    def test_to_many_parametermarkers_dict(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table poff_dict2 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.execute("insert into poff_dict2 values (:a, :b)",
+                              {'g':55, 'a':3, 'b':'pi', 'y':'Boo'})
+            c.execute("select * from poff_dict2")
+            r = c.fetchall()[0]
+            self.assertEqual(r, (3, 'pi'))
+        self.tstcon.commit()
+
+    def test_insert_many_times(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob34(c1 INTEGER, c2 NVARCHAR(10),"
+                      "                   c3 FLOAT) in pybank")
+            for i in range(0, 101):
+                c.execute("insert into bob34 values (5,'ウィキペディ', 4.4543543)")
+        self.tstcon.commit()
+
+    def test_executemany_one_value(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob4 (c1 INTEGER) in pybank")
+            c.executemany("insert into bob4 values (:a)", [(1,)])
+            #with self.assertRaises(ProgrammingError):
+            c.execute("insert into bob4 values (:a)", [(1)])
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob4 values (:a)", (1))
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob4 values (:a)", [1])
+
+    def test_executemany_one_tuple(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob5 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.executemany("insert into bob5 values (:a, :b)", ((1, 'bob1'),))
+
+    def test_executemany_several_tuples(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobe6 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.executemany("insert into bobe6 values (:a, :b)",
+                          [(1, 'bob1'), (2, 'bob2'),
+                           (3, 'bob3')])
+
+    def test_commit(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob7d (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            c.executemany("insert into bob7d values (:a, :b)",
+                          ((1, 'bob1'), (2, 'bob2'),
+                           (3, 'bob3')))
+            self.tstcon.commit()
+
+    ### &&&& Should fail since DDL has no commit
+    def test_fetchone(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.cursor()
+        b.execute("create table bob8 (c1 INTEGER, c2 NVARCHAR(10)) in pybank")
+        a.close()
+
+        with self.tstcon.cursor() as c:
+            c.execute("insert into bob8 values (:a, :b)", (8, 'bob'))
+            self.tstcon.commit()
+            c.execute("select * from bob8")
+            self.assertEqual(c.fetchone(), (8, 'bob'))
+
+    def test_fetchmany(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob9 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            self.tstcon.commit()
+
+            c.executemany("insert into bob9 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'),
+                           (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob9")
+            self.assertEqual(c.fetchmany(3),
+                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
+
+    def test_fetchmany_too_many(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob11 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob11 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'),
+                           (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob11")
+            self.assertEqual(c.fetchmany(5),
+                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
+
+    def test_fetchmany_notall(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob12 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob12 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'),
+                           (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob12")
+            self.assertEqual(c.fetchmany(2),
+                             [(9, 'bob9'), (10, 'bob10')])
+            self.assertEqual(c.fetchmany(2), [(11, 'bob11')])
+
+    def test_fetchmany_generator_smol(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_generator (c1 INTEGER, c2 INTEGER)"
+                      " in pybank")
+            generator = ((i,-i) for i in range(10))
+            c.executemany("insert into bob_generator values (:a, :b)", generator)
+            self.tstcon.commit()
+
+    def test_fetchmany_generator_large(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_generator2 (c1 INTEGER, c2 INTEGER)"
+                      " in pybank")
+        with self.tstcon.cursor() as c:
+            size = 100000
+            generator = ((i,-i) for i in range(size))
+            c.executemany("insert into bob_generator2 values (:a, :b)", generator)
+            self.tstcon.commit()
+            c.execute("SELECT MAX(c1), MIN(c2) AS maxv FROM bob_generator2")
+            self.assertEqual(c.fetchone(),(size - 1, -size + 1))
+
+    @unittest.skip
+    def test_fetchmany_generator_too_large(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_generator3 (c1 INTEGER, c2 INTEGER)"
+                    " in pybank")
+        with self.tstcon.cursor() as c:
+            size = 1000000
+            generator = ((i,-i) for i in range(size))
+            c.executemany("insert into bob_generator3 values (:a, :b)", generator)
+            self.tstcon.commit()
+            c.execute("SELECT MAX(c1), MIN(c2) AS maxv FROM bob_generator")
+            self.assertEqual(c.fetchone(),(size - 1, -size + 1))
+
+    def test_fetchall(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob10 (c1 INTEGER, c2 NVARCHAR(10))"
+                      " in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob10 values (:a, :b)",
+                          ((10, 'bob10'), (11, 'bob11'), (12, 'bob12'),))
+            self.tstcon.commit()
+            c.execute("select * from bob10")
+            self.assertEqual(c.fetchall(),
+                             [(10, 'bob10'), (11, 'bob11'), (12, 'bob12')])
+
+    def test_fetchall_correct_number_of_rows(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob101(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+            for i in range(1, 101):
+                c.execute("insert into bob101 values (5,'ウィキペディ', 4.4543543)")
+            self.tstcon.commit()
+            c.execute("select * from bob101")
+            r = c.fetchall()
+            self.assertEqual(len(r), 100)
+
+    def test_fetchall_correct_number_of_rows2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob102(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+        with self.tstcon.cursor() as c:
+            for i in range(1, 101):
+                c.execute("insert into bob102 values (5,'ウィキペディ', 4.4543543)")
+            self.tstcon.rollback()
+            c.execute("select * from bob102")
+            r = c.fetchall()
+            self.assertEqual(len(r), 0)
+
+    def test_fetchall_correct_number_of_rows3(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob103(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+        with self.tstcon.cursor() as c:  
+            for i in range(1, 101):
+                c.execute("insert into bob103 values (5,'ウィキペディ', 4.4543543)")
+                self.tstcon.rollback()
+                c.execute("select * from bob103")
+                r = c.fetchall()
+                self.assertEqual(len(r), 0)
+
+    def test_use_next(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobnext(c1 INTEGER) in pybank")
+            for i in range(0, 10):
+                c.execute("insert into bobnext values (?)", i)
+                self.tstcon.commit()
+                c.execute("select * from bobnext")
+            for i in range(0, 10):
+                val = c.next()
+                self.assertEqual(val, (i,))
+
+    def test_use_next_StopIteration(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobstop(c1 INTEGER) in pybank")
+            for i in range(0, 10):
+                c.execute("insert into bobstop values (?)", i)
+                self.tstcon.commit()
+                c.execute("select * from bobstop")
+            for i in range(0, 10):
+                c.next()
+            with self.assertRaises(StopIteration):
+                c.next()
+
+    def test_insert_wrong_type_parametermarkers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob1337 (c1 INTEGER, c2 INTEGER) in pybank")
+            with self.assertRaises(DataError):
+                c.execute("insert into bob1337  values (:a, :b)", (3, 3.14))
+
+    def test_operate_after_closed(self):
+        c = self.tstcon.cursor()
+        c.close()
+        with self.assertRaises(ProgrammingError):
+            c.execute("select * from system.onerow")
+
+    def test_operate_after_closed_2(self):
+        c = self.tstcon.cursor()
+        c.close()
+        c.close()
+        with self.assertRaises(ProgrammingError):
+            c.execute("Kalle")
+        with self.assertRaises(ProgrammingError):
+            c.executemany("Kalle", ("Kula"))
+        with self.assertRaises(ProgrammingError):
+            c.fetchone()
+        with self.assertRaises(ProgrammingError):
+            c.fetchmany("Kalle")
+        with self.assertRaises(ProgrammingError):
+            c.fetchall()
+        with self.assertRaises(ProgrammingError):
+            c.next()
+
+    def test_invalid_select(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(ProgrammingError):
+                c.execute("select * from jonisnotatablejo where c1 = ?", (5))
+
+    def test_same_table_twice(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob2437(c1 INTEGER) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob2437(c1 INTEGER) in pybank")
+
+    def test_invalid_sequence_select(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob6565(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("select * from bob6565")
+            r = c.fetchone()
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob6569(c1 INTEGER) in pybank")
+
+    # &&&& borde bli fel men blir rätt....
+    # Blir inte rätt för att man blandar DDL och DML i samma transaktion
+    @unittest.skip
+    def test_invalid_sequence_select_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob555(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("select * from bob555")
+            c.execute("create table bob556(c1 INTEGER) in pybank")
+            c.execute("insert into bob556 values (3)")
+            self.tstcon.rollback()
+            c.execute("select * from bob556")
+            self.assertEqual(c.fetchone(), [])
+
+    def test_invalid_sequence_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob6567(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bob6567 values (3)")
+            ## &&&& Should not fail
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob65ss(c1 INTEGER) in pybank")
+                self.tstcon.rollback()
+
+    def test_invalid_sequence_insert_parametermarkers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob6568(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bob6568 values (?)", (3))
+            ## &&&& Should not fail
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob6566(c1 INTEGER) in pybank")
+                self.tstcon.rollback()
+
+    def test_executemany_DDL(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(ProgrammingError):
+                b = c.executemany("create table bob6(c1 INTEGER) in pybank",
+                                  (3))
+
+    def test_insert_exceeded(self):
+        with self.tstcon.cursor() as c:
+            b = c.execute("create table bob16(c1 BIGINT) in pybank")
+            big = pow(2, 100)
+            with self.assertRaises(DataError):
+                c.execute("insert into bob16 values (?)", big)
+
+    def test_insert_too_long(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob17(c1 NVARCHAR(10)) in pybank")
+            self.tstcon.commit()
+            with self.assertRaises(DataError):
+                c.execute("insert into bob17 values ('ウィキペデBobWasAYoungBoy')")
+                self.tstcon.commit()
+
+    def test_valid_int32_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon32 (c1 INTEGER, c2 INTEGER) in pybank")
+            nvar = -2 ** 31
+            var = 2 ** 31 - 1
+            c.execute("insert INTO jon32 VALUES (?, ?)", (nvar, var))
+            self.tstcon.commit()
+
+    def test_invalid_int32_insert_too_small(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon31 (c1 INTEGER) in pybank")
+            nvar = -2 ** 31 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon31 VALUES (?)", (nvar))
+
+    def test_invalid_int32_insert_too_big(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon33 (c1 INTEGER) in pybank")
+            var = 2 ** 31
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon33 VALUES (?)", (var))
+
+    def test_valid_int64_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon64 (c1 BIGINT, c2 BIGINT) in pybank")
+            nvar = -2 ** 63
+            var = 2 ** 63 - 1
+            c.execute("insert INTO jon64 VALUES (?,?)", (nvar, var))
+            self.tstcon.commit()
+            c.execute("Select * from jon64")
+            self.assertEqual(c.fetchall(), [(nvar, var)])
+
+    def test_overflow_int64_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table intjon4 (c1 BIGINT, c2 BIGINT) in pybank")
+            nvar = -2 ** 633
+            var = 2 ** 63 - 1
+            with self.assertRaises(DataError):
+                c.executemany("insert INTO intjon4 VALUES (?,?)",
+                              ((nvar, var), (nvar, var)))
+
+    def test_invalid_int64_insert_too_small(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon63 (c1 BIGINT) in pybank")
+            nvar = -2 ** 63 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon63 VALUES (?)", (nvar))
+
+    def test_invalid_int64_insert_too_big(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon65 (c1 BIGINT) in pybank")
+            var = 2 ** 63
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon65 VALUES (?)", (var))
+
+    def test_valid_int16_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon26 (c1 SMALLINT, c2 SMALLINT) in pybank")
+            nvar = -2 ** 15
+            var = 2 ** 15 - 1
+            c.execute("insert INTO jon26 VALUES (?, ?)", (nvar, var))
+            self.tstcon.commit()
+            c.execute("SELECT * from jon26")
+            self.assertEqual(c.fetchall(), [(nvar,var)])
+
+    def test_invalid_int16_insert_too_small(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon15 (c1 SMALLINT) in pybank")
+            nvar = -2 ** 15 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon15 VALUES (?)", (nvar))
+
+    def test_invalid_int16_insert_too_big(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon17 (c1 SMALLINT) in pybank")
+            nvar = 2 ** 15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon17 VALUES (?)", (nvar))
+
+    # &&&& Gives a Warning we dont catch atm
+    def test_valid_double_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon16 (c1 REAL, c2 DOUBLE PRECISION)"
+                      " in pybank")
+            var = 2 / 3
+            c.execute("insert INTO jon16 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+            c.execute("select * from jon16")
+            self.assertEqual(c.fetchall(), [(0.6666666865348816, var)])
+
+    def test_invalid_double_insert(self):
+        b = self.tstcon.cursor()
+        c = self.tstcon.cursor()
+        d = self.tstcon.cursor()
+        e = self.tstcon.cursor()
+        f = self.tstcon.cursor()
+        b.execute("create table jondd (c1 FLOAT) in pybank")
+        var = 10 ** 309
+        with self.assertRaises(DataError):
+            b.execute("insert INTO jondd VALUES (?)", (var))
+        with self.assertRaises(ProgrammingError):
+            b.execute("insert INTO jondd VALUES (?, ?)", (-var, -var))
+        b.close()
+        c.close()
+        d.close()
+        e.close()
+        f.close()
+
+    def test_valid_double_insert_none(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon18 (c1 REAL, c2 DOUBLE PRECISION)"
+                      " in pybank")
+            var = None
+            c.execute("insert INTO jon18 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+            c.execute("select * from jon18")
+            self.assertEqual(c.fetchall(), [(None, None)])
+
+    def test_valid_double_select_none(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jon19 (c1 REAL, c2 DOUBLE PRECISION)"
+                      " in pybank")
+            var = None
+            c.execute("insert INTO jon19 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+            c.execute("select * from jon19")
+            self.assertEqual(c.fetchall(), [(None, None)])
+
+    def test_message_cleared(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonwas17 (c1 SMALLINT) in pybank")
+            nvar = 2 ** 15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jonwas17 VALUES (?)", (nvar))
+            c.execute("insert INTO jonwas17 VALUES (?)", (5))
+            self.assertEqual(c.messages, [])
+
+    def test_message_cleared_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonwas173 (c1 SMALLINT) in pybank")
+            nvar = 2 ** 15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jonwas173 VALUES (?)", (nvar))
+            self.assertEqual(c.messages[0][1],
+                             (-24010,
+                              'Value was too large to fit in destination'))
+
+    def test_None_is_returned(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonNone (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonNone VALUES (?)", (i))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonNone")
+            for i in range(1, 10):
+                c.fetchone()
+            self.assertEqual(c.fetchone(), [])
+
+    def test_empty_sequence_is_returned_many(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonEmpty (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonEmpty VALUES (?)", (i))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonEmpty")
+            c.fetchmany(10)
+            self.assertEqual(c.fetchmany(10), [])
+
+    def test_empty_sequence_is_returned_all(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonEmpty2 (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonEmpty2 VALUES (?)", (i))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonEmpty2")
+            c.fetchall()
+            self.assertEqual(c.fetchall(), [])
+
+    def test_empty_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonEmp (c1 NVARCHAR(128)) in pybank")
+            c.executemany("Insert INTO jonEmp VALUES (?)",
+                          (('',), ("",), (" ",)))
+            self.tstcon.commit()
+            c.execute("select * from jonEmp")
+            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
+
+    def test_empty_insert2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonEmp2 (c1 NVARCHAR(128)) in pybank")
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (''))
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (""))
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (" "))
+            self.tstcon.commit()
+            c.execute("select * from jonEmp2")
+            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
+
+    def test_invalid_databank(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bjonEmp2 (c1 NVARCHAR(128)) in potato")
+
+    def test_insert_rowcount_update(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobrowcount (c1 INTEGER, c2 NVARCHAR(256))"
+                      " in pybank")
+            string = "mimer"
+            c.execute("insert into bobrowcount values (:a, :b)", (3, string))
+            self.assertEqual(c.rowcount, 1)
+            c.executemany("insert into bobrowcount values (:a, :b)",
+                          ((5, string), (2, string)))
+            c.execute("select * from bobrowcount")
+            r = c.fetchall()
+            self.assertEqual(c.rowcount, 2)
+
+    def test_delete(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobrowcount2(c1 INTEGER) in pybank")
+            for i in range(1, 11):
+                c.execute("INSERT into bobrowcount2 values (?)", 10)
+                c.execute("INSERT into bobrowcount2 values (?)", 20)
+            c.execute("INSERT into bobrowcount2 values (?)", 10)
+            c.execute("SELECT * from bobrowcount2")
+            self.assertEqual(len(c.fetchall()), 21)
+            c.execute("DELETE from bobrowcount2 where c1 = 10")
+            self.assertEqual(c.rowcount, 11)
+            c.execute("SELECT * from bobrowcount2")
+            self.assertEqual(len(c.fetchall()), 10)
+
+    def test_update(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobupdate(c1 INTEGER) in pybank")
+            for i in range(1, 11):
+                c.execute("INSERT into bobupdate values (?)", 10)
+                c.execute("INSERT into bobupdate values (?)", 20)
+            c.execute("INSERT into bobupdate values (?)", 10)
+            c.execute("SELECT * from bobupdate")
+            self.assertEqual(len(c.fetchall()), 21)
+            c.execute("UPDATE bobupdate SET c1 = ? WHERE c1 = 20", 30)
+            self.assertEqual(c.rowcount, 10)
+            c.execute("SELECT * from bobupdate")
+            self.assertEqual(len(c.fetchall()), 21)
+
+    def test_invalid_sequence_fetchone(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonfetchone (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonfetchone VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchone()
+
+    def test_isolated(self):
+        b1 = self.tstcon.cursor()
+        b2 = self.tstcon.cursor()
+        b1.execute("create table jonisolated (c1 INTEGER) in pybank")
+        for c in range(1, 6):
+            b1.execute("Insert INTO jonisolated VALUES (?)", (c))
+        b2.execute("SELECT * FROM jonisolated")
+        c2 = b2.fetchall()
+        self.assertEqual(len(c2), 5)
+        self.assertEqual(c2, [(1,), (2,), (3,), (4,), (5,), ])
+
+    def test_isolated2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonisolated2 (c1 INTEGER) in pybank")
+            self.tstcon.commit()
+
+        cred = db_config.TSTUSR.copy()
+        cred['autocommit'] = True
+        a1 = mimerpy.connect(**cred)
+        a2 = mimerpy.connect(**cred)
+        b1 = a1.cursor()
+        b2 = a2.cursor()
+        for c in range(1, 6):
+            b1.execute("Insert INTO jonisolated2 VALUES (?)", (c))
+        b2.execute("SELECT * FROM jonisolated2 WHERE c1 < ?", 3)
+        c2 = b2.fetchall()
+        self.assertEqual(len(c2), 2)
+        self.assertEqual(c2, [(1,), (2,)])
+        b2.execute("SELECT * FROM jonisolated2")
+        c3 = b2.fetchall()
+        self.assertEqual(len(c3), 5)
+        self.assertEqual(c3, [(1,), (2,), (3,), (4,), (5,), ])
+        a1.close()
+        a2.close()
+
+    # fråga per
+    def test_isolated3(self):
+        a = mimerpy.connect(**db_config.TSTUSR)
+        b = a.cursor()
+        b.execute("create table jonisolated3 (c1 INTEGER) in pybank")
+        a.commit()
+        a.close()
+        with self.tstcon.cursor() as c:
+            for i in range(1, 6):
+                c.execute("Insert INTO jonisolated3 VALUES (?)", (i))
+            c.execute("SELECT * FROM jonisolated3")
+            c1 = c.fetchall()
+            self.assertEqual(c1, [(1,), (2,), (3,), (4,), (5,), ])
+            c.execute("SELECT * FROM jonisolated3")
+            c2 = c.fetchall()
+            self.assertEqual(c2, [(1,), (2,), (3,), (4,), (5,), ])
+
+    def test_invalid_sequence_fetchmany(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonfetchmany (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonfetchmany VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchmany(10)
+
+    def test_invalid_sequence_fetchall(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonfetchall (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonfetchall VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchall()
+
+    @unittest.skip
+    def test_UUID_one(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table uuidtable( id BUILTIN.UUID) in pybank")
+            vuuid = uuid.uuid4().bytes
+            c.execute("insert into uuidtable values(?)", (vuuid))
+            self.tstcon.commit()
+            c.execute("select id.as_text() from uuidtable")
+            r = c.fetchall()[0][0]
+            self.assertEqual(r, vuuid)
+
+    
+    def test_UUID_two(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table uuidtable2( id BUILTIN.UUID) in pybank")
+            vuuid = str(uuid.uuid1())
+            c.execute("insert into uuidtable2 values(builtin.uuid_from_text(cast(? as varchar(50))))", (vuuid))
+            self.tstcon.commit()
+            c.execute("select id.as_text() from uuidtable2")
+            r = c.fetchall()[0][0]
+            self.assertEqual(r, vuuid)
+
+    @unittest.skip
+    def test_datatype_GIS_one(self):
+        with self.tstcon.cursor() as c:
+            vuuid = '40.75,-74.0'
+            c.execute("create table gistable2( id BUILTIN.GIS_LATITUDE) in pybank")
+            c.execute("insert into gistable2 values(BUILTIN.GIS_LOCATION(40.75,-74.0))")
+            self.tstcon.commit()
+            c.execute("select id.as_text() from uuidtable2")
+            r = c.fetchall()[0][0]
+            self.assertEqual(r, vuuid)
+
+    @unittest.skip
+    def test_datatype_GIS(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table gistable2( id BUILTIN.GIS_LATITUDE) in pybank")
+            x,y = 40.75,-74.0
+            c.execute("insert into gistable2 values(BUILTIN.GIS_LOCATION(?,?))", (x,y))
+            self.tstcon.commit()
+            #c.execute("select id.as_text() from uuidtable2")
+            #r = c.fetchall()[0][0]
+            #self.assertEqual(r, vuuid)
+
+    def test_insert_blob(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonblob (c1 BLOB(18389)) in pybank")
+            ablob = bytes(bytearray("Hello there", encoding ='utf-8'))
+            c.execute("insert INTO jonblob VALUES (?)", (ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblob")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+
+    def test_insert_blob_21(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonblob2 (c1 BLOB(64111)) in pybank")
+            with open("testCursor.py", 'rb') as input_file:
+                ablob = input_file.read(200)
+                c.execute("insert INTO jonblob2 VALUES (?)", (ablob))
+                self.tstcon.commit()
+                c.execute("select * from jonblob2")
+                r = c.fetchall()[0]
+                self.assertEqual(r[0], ablob)
+
+    def test_insert_blob_multi_column(self):
+        with self.tstcon.cursor() as c:
+            ablob = ('åäö' * 1024 * 2000).encode('utf-8') 
+            c.execute("create table jonblobmulti (c1 BLOB(20m), c2 BLOB(20m)) in pybank")
+            c.execute("insert INTO jonblobmulti VALUES (?,?)", (ablob,ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblobmulti")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+    
+    def test_insert_blob_multi_column2(self):
+        with self.tstcon.cursor() as c:
+            ablob = (256).to_bytes(1024 * 10000,byteorder='big')
+            ablob2 = ('åäö' * 1024 * 3000).encode('utf-8')
+            c.execute("create table jonblobmulti2 (c1 BLOB(30m), c2 BLOB(30m), c3 BLOB(30m)) in pybank")
+            c.execute("insert INTO jonblobmulti2 VALUES (?,?,?)", (ablob,ablob,ablob2))
+            self.tstcon.commit()
+            c.execute("select * from jonblobmulti2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[2], ablob2)
+
+    def test_insert_blob_10mb(self):
+        with self.tstcon.cursor() as c:
+            ablob = (256).to_bytes(1024 * 10000,byteorder='big') 
+            c.execute("create table jonblob10 (c1 BLOB(100m)) in pybank")
+            c.execute("insert INTO jonblob10 VALUES (?)", (ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblob10")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+    
+    #@unittest.skip
+    def test_insert_blob_50mb(self):
+        with self.tstcon.cursor() as c:
+            ablob = (512).to_bytes(1024 * 50000,byteorder='big') 
+            c.execute("create table jonblob50 (c1 BLOB(100m)) in pybank")
+            c.execute("insert INTO jonblob50 VALUES (?)", (ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblob50")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+    
+    #@unittest.skip
+    def test_insert_blob_100mb(self):
+        with self.tstcon.cursor() as c:
+            ablob = (1024).to_bytes(1024 * 100000,byteorder='big') 
+            c.execute("create table jonblob100 (c1 BLOB(100m)) in pybank")
+            c.execute("insert INTO jonblob100 VALUES (?)", (ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblob100")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+
+    # Might have to up your bufferpool memory to run this
+    @unittest.skip
+    def test_insert_blob_1gb(self):
+        with self.tstcon.cursor() as c:
+            ablob = (1024).to_bytes(1024 * 1000000,byteorder='big') 
+            c.execute("create table jonblobgb (c1 BLOB(1000m)) in pybank")
+            c.execute("insert INTO jonblobgb VALUES (?)", (ablob))
+            self.tstcon.commit()
+            c.execute("select * from jonblobgb")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ablob)
+
+    def test_insert_nclob(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonnclob (c1 NCLOB(50000)) in pybank")
+            anclob = "mimer" * 1000
+            c.execute("insert INTO jonnclob VALUES (?)", (anclob))
+            self.tstcon.commit()
+            c.execute("select * from jonnclob")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], anclob)
+
+    def test_insert_nclob_unicode(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table unijonnclob (c1 NCLOB(50000)) in pybank")
+            uniclob = "安排他們參"
+            self.tstcon.commit()
+            c.execute("insert into unijonnclob values (:a)",(uniclob,))
+            self.tstcon.commit()
+            c.execute("select * from unijonnclob")
+            self.assertEqual(c.fetchall(),
+                             [(uniclob,)])
+
+    def test_insert_binary(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonbinary (c1 BINARY(3)) in pybank")
+            c.execute("insert INTO jonbinary VALUES (x'ABCD01')")
+            c.execute("insert INTO jonbinary VALUES (?)", (b'A01'))
+            self.tstcon.commit()
+            c.execute("select * from jonbinary")
+            r = c.fetchall()
+            self.assertEqual(r, [(b'\xab\xcd\x01',), (b'A01',)])
+
+    def test_insert_binary_parameter_markers(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonbinary2 (c1 BINARY(4)) in pybank")
+            bob = b"0x53"
+            c.execute("insert INTO jonbinary2 VALUES (?)", (bob))
+            self.tstcon.commit()
+            c.execute("select * from jonbinary2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], b'0x53')
+
+    def test_insert_nclob_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonnclob2 (c1 Nclob(450000)) in pybank")
+            res = ''.join(format(i, 'b') for i in bytearray("Hello there", encoding ='utf-8')) 
+            c.execute("insert INTO jonnclob2 VALUES (?)", (res))
+            self.tstcon.commit()
+            c.execute("select * from jonnclob2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], res)
+
+    def test_insert_clob(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonclob (c1 clob(30000)) in pybank")
+            aclob = "mimer" * 5
+            c.execute("insert INTO jonclob VALUES (?)", (aclob))
+            self.tstcon.commit()
+            c.execute("select * from jonclob")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], aclob)
+
+    def test_datatype_clob(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jonclob2 (c1 clob) in pybank")
+            aclob = "mimer" * 5
+            c.execute("insert INTO jonclob2 VALUES (?)", (aclob))
+            self.tstcon.commit()
+            c.execute("select * from jonclob2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], aclob)
+
+    def test_insert_date(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jondata (c1 DATE) in pybank")
+            data = "2020-09-24"
+            c.execute("insert INTO jondata VALUES (?)", (data))
+            self.tstcon.commit()
+            c.execute("select * from jondata")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], data)
+
+    def test_insert_time_one(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jontime (c1 TIME(0)) in pybank")
+            time = "16:04:55"
+            c.execute("insert INTO jontime VALUES (?)", (time))
+            self.tstcon.commit()
+            c.execute("select * from jontime")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], time)
+
+    def test_insert_time_two(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jontime2 (c1 TIME(4)) in pybank")
+            time = "16:04:55.1234"
+            c.execute("insert INTO jontime2 VALUES (?)", (time))
+            self.tstcon.commit()
+            c.execute("select * from jontime2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], time)
+    
+    def test_insert_decimal_str(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table jondecimal (c1 DECIMAL(7,2)) in pybank")
+            floatnum = '32423.23'
+            c.execute("insert INTO jondecimal VALUES (?)", (floatnum))
+            self.tstcon.commit()
+            c.execute("select * from jondecimal")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], decimal.Decimal(floatnum))
+
+    def test_insert_decimal_decimal(self):
+        with self.tstcon.cursor() as c:
+            decimal.getcontext().prec = 45
+            des = decimal.Decimal("1.14")
+            c.execute("create table jondecimal2 (c1 DECIMAL(3,2)) in pybank")
+            c.execute("insert INTO jondecimal2 VALUES (?)", (des))
+            self.tstcon.commit()
+            c.execute("select * from jondecimal2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], des)
+
+    # Bör runda av, men ger för tillfället en exception
+    @unittest.skip
+    def test_insert_decimal_decimal2(self):
+        with self.tstcon.cursor() as c:
+            decimal.getcontext().prec = 45
+            des = decimal.Decimal("1.141")
+            c.execute("create table jondecimal2 (c1 DECIMAL(3,2)) in pybank")
+            c.execute("insert INTO jondecimal2 VALUES (?)", (des))
+            self.tstcon.commit()
+            c.execute("select * from jondecimal2")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], des)
+
+    def test_insert_decimal_decimal3(self):
+        with self.tstcon.cursor() as c:
+            decimal.getcontext().prec = 45
+            des = decimal.Decimal("1.14")
+            c.execute("create table jondecimal22 (c1 DECIMAL(3,2)) in pybank")
+            c.execute("insert INTO jondecimal22 VALUES (cast(cast('1.141' as varchar(20)) as DECIMAL(3,2)))")
+            self.tstcon.commit()
+            c.execute("select * from jondecimal22")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], des)
+
+    def test_insert_decimal_none(self):
+        with self.tstcon.cursor() as c:
+            decimal.getcontext().prec = 45
+            c.execute("create table jondecimalnone (c1 DECIMAL(3,2)) in pybank")
+            c.execute("insert INTO jondecimalnone VALUES (?)", (None))
+            self.tstcon.commit()
+            c.execute("select * from jondecimalnone")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], None)
+
+    def test_datatype_interval_DAY(self):
+        with self.tstcon.cursor() as c:
+            day = "20005"
+            c.execute("create table jonday (c1 INTERVAL DAY(5)) in pybank")
+            c.execute("insert INTO jonday VALUES (?)", (day))
+            self.tstcon.commit()
+            c.execute("select * from jonday")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], day)
+
+    def test_datatype_interval_HOUR(self):
+        with self.tstcon.cursor() as c:
+            hour = "20005"
+            c.execute("create table jonhour (c1 INTERVAL HOUR(5)) in pybank")
+            c.execute("insert INTO jonhour VALUES (?)", (hour))
+            self.tstcon.commit()
+            c.execute("select * from jonhour")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], hour)
+
+    def test_datatype_interval_MINUTE(self):
+        with self.tstcon.cursor() as c:
+            minute = "1234567890"
+            c.execute("create table jonminute (c1 INTERVAL MINUTE(10)) in pybank")
+            c.execute("insert INTO jonminute VALUES (?)", (minute))
+            self.tstcon.commit()
+            c.execute("select * from jonminute")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], minute)
+
+    def test_datatype_interval_year(self):
+        with self.tstcon.cursor() as c:
+            year = "20005"
+            c.execute("create table jonyear (c1 INTERVAL year(5)) in pybank")
+            c.execute("insert INTO jonyear VALUES (?)", (year))
+            self.tstcon.commit()
+            c.execute("select * from jonyear")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], year)
+
+    def test_datatype_interval_SECOND(self):
+        with self.tstcon.cursor() as c:
+            second = "20005.000000"
+            c.execute("create table jonsecond (c1 INTERVAL SECOND(5)) in pybank")
+            c.execute("insert INTO jonsecond VALUES (?)", (second))
+            self.tstcon.commit()
+            c.execute("select * from jonsecond")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], second)
+
+    def test_datatype_interval_SECOND_P(self):
+        with self.tstcon.cursor() as c:
+            second = "12345.67"
+            c.execute("create table jonsecondp (c1 INTERVAL SECOND(5,2)) in pybank")
+            c.execute("insert INTO jonsecondp VALUES (?)", (second))
+            self.tstcon.commit()
+            c.execute("select * from jonsecondp")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], second)
+
+    def test_datatype_interval_YEAR_TO_MONTH(self):
+        with self.tstcon.cursor() as c:
+            ym = "5-10"
+            c.execute("create table jonytm (c1 INTERVAL YEAR(5) TO MONTH) in pybank")
+            c.execute("insert INTO jonytm VALUES (?)", (ym))
+            self.tstcon.commit()
+            c.execute("select * from jonytm")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], ym)
+
+    def test_datatype_interval_DAY_TO_HOUR(self):
+        with self.tstcon.cursor() as c:
+            dhms = "5 23"
+            c.execute("create table jondth (c1 INTERVAL DAY(5) TO HOUR) in pybank")
+            c.execute("insert INTO jondth VALUES (?)", (dhms))
+            self.tstcon.commit()
+            c.execute("select * from jondth")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], dhms)
+
+    def test_datatype_interval_DAY_TO_MINUTE(self):
+        with self.tstcon.cursor() as c:
+            dhm = "5 23:55"
+            c.execute("create table jondtm (c1 INTERVAL DAY(5) TO MINUTE) in pybank")
+            c.execute("insert INTO jondtm VALUES (?)", (dhm))
+            self.tstcon.commit()
+            c.execute("select * from jondtm")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], dhm)
+
+    def test_datatype_interval_DAY_TO_SECOND(self):
+        with self.tstcon.cursor() as c:
+            dhms = "5 23:05:01.123"
+            c.execute("create table jondts (c1 INTERVAL DAY(5) TO SECOND(3)) in pybank")
+            c.execute("insert INTO jondts VALUES (?)", (dhms))
+            self.tstcon.commit()
+            c.execute("select * from jondts")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], dhms)
+
+    def test_datatype_interval_HOUR_TO_MINUTE(self):
+        with self.tstcon.cursor() as c:
+            hts = "55555:01"
+            c.execute("create table jonhtm (c1 INTERVAL HOUR(5) TO MINUTE) in pybank")
+            c.execute("insert INTO jonhtm VALUES (?)", (hts))
+            self.tstcon.commit()
+            c.execute("select * from jonhtm")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], hts)
+
+    def test_datatype_interval_HOUR_TO_SECOND(self):
+        with self.tstcon.cursor() as c:
+            hts = "55555:23:02.12345"
+            c.execute("create table jonhts (c1 INTERVAL HOUR(5) TO SECOND(5)) in pybank")
+            c.execute("insert into jonhts values(cast(? as interval HOUR(5) to second(5)))", (hts))
+            #c.execute("insert INTO jonhts VALUES (?)", (hts))
+            self.tstcon.commit()
+            c.execute("select * from jonhts")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], hts)
+
+    def test_datatype_interval_MINUTE_TO_SECOND(self):
+        with self.tstcon.cursor() as c:
+            minute = '12345:12.12345679'
+            c.execute("create table jonmts (c1 INTERVAL MINUTE(5) TO SECOND(8)) in pybank")
+            c.execute("insert into jonmts values (?)", minute)
+            self.tstcon.commit()
+            c.execute("select * from jonmts")
+            r = c.fetchall()
+            self.assertEqual(r[0][0], minute)
+            
+    def test_insert_bool(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobybool (c1 boolean) in pybank")
+            c.execute("insert INTO bobybool VALUES (?)", (False))
+            c.execute("insert INTO bobybool VALUES (?)", (45))
+            self.tstcon.commit()
+
+    def test_select_bool(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobybool2 (c1 boolean) in pybank")
+            c.execute("insert INTO bobybool2 VALUES (?)", (False))
+            c.execute("insert INTO bobybool2 VALUES (?)", (45))
+            self.tstcon.commit()
+            c.execute("select * from bobybool2")
+            r = c.fetchone()
+            self.assertEqual(r[0], False)
+            r = c.fetchone()
+            self.assertEqual(r[0], True)
+
+    def test_get_connection(self):
+        c = self.tstcon.cursor()
+        self.assertEqual(c.connection, self.tstcon)
+        c.close()
+
+    def test_for(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table fortable (c1 INTEGER, c2 INTEGER)"
+                      " in pybank")
+            c.execute("insert INTO fortable VALUES (?,?)", (1,99))
+            c.execute("insert INTO fortable VALUES (?,?)", (3,97))
+            c.execute("insert INTO fortable VALUES (?,?)", (10,90))
+            c.execute("select * from fortable")
+            count = 0
+            for val in c:
+                self.assertEqual(val[0]+val[1], 100)
+                count = count + 1
+            self.assertEqual(count, 3)
+
+    def test_result_set_twice(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table kor (c1 INTEGER) in pybank")
+            c.execute("insert INTO kor VALUES (?)", (45))
+            c.execute("select * from kor")
+            for val in c:
+                self.assertEqual(val[0], 45)
+            c.execute("select * from kor")
+            c.execute("select c1 from kor")
+
+    def test_executemany_none(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table manytable (c1 INTEGER) in pybank")
+            c.executemany("insert INTO manytable VALUES (?)",
+                          [(2,), (34,), (435,), (34,), (63,), (47,), (None,)])
+            self.tstcon.commit()
+
+    def test_select_executemany(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobyselect (c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert INTO bobyselect VALUES (?)", (1))
+            with self.assertRaises(ProgrammingError):
+                c.executemany("select * from bobyselect where c1 = (?)",
+                              ((5,), (10,)))
+
+    def test_select_twice(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bananaselect (c1 INTEGER) in pybank")
+            c.execute("select * from bananaselect where c1 = (?)", (5))
+            c.execute("select c1 from bananaselect where c1 = (?)", (7))
+
+    def test_fetchall_no_select(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(ProgrammingError):
+                c.fetchall()
+
+    def test_bool_insert(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table boolt (c1 BOOLEAN) in pybank")
+            c.executemany("insert into boolt values (?)",
+                          [(None,), (1,), (0,), (3.1415,),
+                           ("potato",), ('code',)])
+            c.execute("select * from boolt")
+            r = c.fetchall()
+            self.assertEqual(r, [(None,), (True,), (False,),
+                                 (True,), (True,), (True,)])
+
+    def test_insert_parametermarkers_different_types(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob176(c1 NVARCHAR(128)) in pybank")
+            c.execute("INSERT INTO bob176 VALUES (?)", "bar")  # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ("bar"))  # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ("bar",))  # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ["bar"])  # correct
+            self.tstcon.commit()
+            c.execute("select * from bob176")
+            self.assertEqual(c.fetchall(), [("bar",), ("bar",),
+                                            ("bar",), ("bar",)])
+
+    def test_insert_parametermarkers_different_types2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bobd(c1 NVARCHAR(128), c2 INTEGER,"
+                      "                  c3 FLOAT) in pybank")
+            c.execute("INSERT INTO bobd VALUES (?,?,?)",
+                      ("bar", 314, 41.23))
+            c.execute("INSERT INTO bobd VALUES (?,?,?)",
+                      ("bar", 315, 41.23,))
+            with self.assertRaises(ProgrammingError):
+                c.execute("INSERT INTO bobd VALUES (?,?,?)",
+                          "bar", (316), (41.23))
+            c.execute("INSERT INTO bobd VALUES (?,?,?)",
+                      ["bar", 317, 41.23])
+            self.tstcon.commit()
+            c.execute("select * from bobd")
+            self.assertEqual(c.fetchall(),
+                             [('bar', 314, 41.23),
+                              ('bar', 315, 41.23),
+                              ('bar', 317, 41.23)])
+
+    def test_char_table(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table charbob(c1 CHAR(10)) in pybank")
+            c.execute("INSERT INTO charbob VALUES ('Kalle Kula')")
+            self.tstcon.commit()
+            c.execute("select * from charbob")
+            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
+
+    def test_invalid_char(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table invalidbob(c1 CHAR(10)) in pybank")
+            # kastar inget fel för tillfället, vilket är micro api's fel,
+            # men inget vi ska lösa just nu
+            # &&&& Fixme!
+            c.execute("INSERT INTO invalidbob VALUES ('?')", ("ィキペデ"))
+            with self.assertRaises(DataError):
+                c.execute("INSERT INTO invalidbob VALUES ('ィキペデ')")
+            self.tstcon.commit()
+            c.execute("select * from invalidbob")
+            r = c.fetchall()
+
+
+    def test_varchar_table(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table varcharbob(c1 VARCHAR(128)) in pybank")
+            c.execute("INSERT INTO varcharbob VALUES ('Kalle Kula')")
+            self.tstcon.commit()
+            c.execute("select * from varcharbob")
+            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
+
+    def test_nchar_table(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table ncharbob(c1 VARCHAR(128)) in pybank")
+            c.execute("INSERT INTO ncharbob VALUES ('Kalle Kula')")
+            self.tstcon.commit()
+            c.execute("select * from ncharbob")
+            self.assertEqual(c.fetchall(), [("Kalle Kula",)])
+
+    def test_callproc_nextset(self):
+        with self.tstcon.cursor() as c:
+            with self.assertRaises(NotSupportedError):
+                c.nextset()
+            with self.assertRaises(NotSupportedError):
+                c.callproc()
+
+    def test_insert_blob_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("CREATE TABLE blob_table (blobcolumn BLOB)")
+            blob = bytes(bytearray("Hello there again", encoding ='utf-8'))
+            c.execute("INSERT INTO blob_table VALUES (?)", (blob))
+            self.tstcon.commit()
+            c.execute("SELECT * FROM blob_table")
+            r = c.fetchall()[0][0]
+            self.assertEqual(r, blob)
+
+    def test_conflict_drop(self):
+        with self.tstcon.cursor() as c:
+            mytuplelist = list(zip(list(range(100)), list(range(100))))
+            c.execute("CREATE TABLE conflict_test2 (int1 INTEGER, int2 INTEGER)")
+            c.executemany("INSERT INTO conflict_test2 VALUES (?,?)", (mytuplelist))
+            self.tstcon.commit()
+
+        conn1 = mimerpy.connect(**db_config.TSTUSR)
+        conn2 = mimerpy.connect(**db_config.TSTUSR)
+        conn1.execute("INSERT INTO conflict_test2 VALUES (?,?)", (200,200))
+        with self.assertRaises(OperationalError) as e:
+            conn2.execute("DROP TABLE conflict_test2 CASCADE")
+        self.assertEqual(-16001, e.exception.errno)
+        self.assertEqual("Table MIMERPY.conflict_test2 locked by another user", e.exception.message)
+        conn1.close()
+        conn2.close()
+    
+    def test_conflict_insert(self):
+        with self.tstcon.cursor() as c:
+            mytuplelist = list(zip(list(range(100)), list(range(100))))
+            c.execute("CREATE TABLE conflict_test3 (int1 INTEGER, int2 INTEGER, PRIMARY KEY (int1))")
+            c.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
+            self.tstcon.commit()
+
+        conn1 = mimerpy.connect(**db_config.TSTUSR)
+        conn2 = mimerpy.connect(**db_config.TSTUSR)
+        mytuplelist = list(zip(list(range(200,300)), list(range(200, 300))))
+        conn1.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
+        conn2.executemany("INSERT INTO conflict_test3 VALUES (?,?)", (mytuplelist))
+        conn1.commit()
+        with self.assertRaises(TransactionAbortError) as e:
+            conn2.commit()
+        self.assertEqual(-10001, e.exception.errno)
+        self.assertEqual("Transaction aborted due to conflict with other transaction", e.exception.message)
+        conn1.close()
+        conn2.close()
+
+    def test_conflict_update(self):
+        with self.tstcon.cursor() as c:
+            mytuplelist = list(zip(list(range(100)), list(range(100))))
+            c.execute("CREATE TABLE conflict_test4 (int1 INTEGER, int2 INTEGER)")
+            c.executemany("INSERT INTO conflict_test4 VALUES (?,?)", (mytuplelist))
+            self.tstcon.commit()
+
+        conn1 = mimerpy.connect(**db_config.TSTUSR)
+        conn2 = mimerpy.connect(**db_config.TSTUSR)
+        conn1.execute("UPDATE conflict_test4 SET int1 = 500 where int1 = 50")
+        conn2.execute("UPDATE conflict_test4 SET int1 = 555 where int1 = 50")
+        conn1.commit()
+        with self.assertRaises(OperationalError) as e:
+            conn2.commit()
+        self.assertEqual(-10001, e.exception.errno)
+        self.assertEqual("Transaction aborted due to conflict with other transaction", e.exception.message)
+        conn1.close()
+        conn2.close()
+
+    # these are the test examples for the documentaion
+    def test_for_doc_1(self):
+        with self.tstcon.cursor() as c:
+            c.execute("CREATE TABLE with_table_cursor1(c1 INTEGER,"
+                      "                            c2 VARCHAR(32)) in pybank")
+            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
+                      (1, "This is an example"))
+            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
+                      (2, "on how to use"))
+            c.execute("INSERT INTO with_table_cursor1 VALUES (?,?)",
+                      (3, "the with functionality."))
+        with self.tstcon.cursor() as c:
+            c.execute("SELECT * from with_table_cursor1")
+
+    # these are the test examples for the documentaion
+    @unittest.skip
+    def test_for_doc_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("CREATE TABLE with_table_connection1(c1 INTEGER,"
+                             " c2 VARCHAR(32)) in pybank")
+        self.tstcon.commit()
+
+        with mimerpy.connect(**db_config.TSTUSR) as con:
+            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
+                        (1, "This is an example"))
+            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
+                        (2, "on how to use"))
+            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
+                        (3, "the with functionality."))
+            con.commit()
+
+        with mimerpy.connect(**db_config.TSTUSR) as con:
+            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
+                        (4, "Commit forgotten"))
+
+        cred = db_config.TSTUSR.copy()
+        cred['autocommit'] = True
+        with mimerpy.connect(**cred) as con:
+            con.execute("INSERT INTO with_table_connection1 VALUES (?,?)",
+                        (5, "Autocommitted"))
+
+        with self.tstcon.cursor() as c:
+            c.execute("SELECT * from with_table_connection1")
+            self.assertEqual(c.fetchall(),
+                             [(1, 'This is an example'),
+                              (2, 'on how to use'),
+                              (3, 'the with functionality.'),
+                              (5, 'Autocommitted')])
+
+    # Inconsistent errors, needs to be fixed!
+    def test_invalid_NULL(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table boberror (c1 INTEGER not null,"
+                      "                c2 NVARCHAR(10) not null) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into boberror values (:a, :b)", (None, None))
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into boberror values (:a, :b)", (1, None))
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into boberror values (:a, :b)", (None, 'Hej'))
+            with self.assertRaises(DataError):
+                c.execute("insert into boberror values (NULL, NULL)")
+
+            c.execute("SELECT * from boberror")
+            self.assertEqual(c.fetchall(), [])
+
+    def test_bool_null(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table boolbob3 (c1 boolean)")
+            c.execute("insert into boolbob3 values (?)", (None))
+
+            c.execute("SELECT * from boolbob3")
+            self.assertEqual(c.fetchone(), (None,))
+
+    def test_unsupported_data_type(self):
+        with self.tstcon.cursor() as c:
+            long = """
+create table longboi (c1 char(10),
+                      c2 varchar(10),
+                      c3 CLOB(2000),
+                      c4 nchar(10),
+                      c5 nvarchar(30),
+                      c6 nclob(2000),
+                      c7 binary(2),
+                      c8 varbinary(2),
+                      c9 blob(1024),
+                      c10 SMALLINT,
+                      c11 INTEGER,
+                      c12 BIGINT,
+                      c13 INTEGER(2),
+                      c14 DECIMAL(5,2),
+                      c15 REAL,
+                      c16 DOUBLE PRECISION,
+                      c17 FLOAT,
+                      c18 DATE,
+                      c19 TIME(0),
+                      c20 TIMESTAMP(6)) in pybank"""
+            c.execute(long)
+            c.execute("insert into longboi (c4) values (?)", ("dude", ))
+
+# &&&& Add values in static SQL and then try to get individual columns
+# &&&& Then try to set individual columns from Python
+
+            c.execute("SELECT * from longboi")
+            self.assertEqual(c.fetchone(), (None, None, None, 'dude      ',
+                                            None, None, None, None, None,
+                                            None, None, None, None, None,
+                                            None, None, None, None, None, None))
+
+    def test_data_type_varbinary(self):
+        with self.tstcon.cursor() as c:
+            long = "create table longboi_varbinary (c1 VARBINARY(10)) in pybank"
+            c.execute(long)
+            c.execute("insert into longboi_varbinary values (?)", (b"x'ABCD01"))
+
+            c.execute("SELECT * from longboi_varbinary")
+            self.assertEqual(c.fetchall(), [(b"x'ABCD01",)])
+
+    def test_data_type_smallint(self):
+        with self.tstcon.cursor() as c:
+            long = "create table longboi_smallint (c1 SMALLINT) in pybank"
+            c.execute(long)
+            c.execute("insert into longboi_smallint values (?)", (32000))
+
+            c.execute("SELECT * from longboi_smallint")
+            self.assertEqual(c.fetchall(), [(32000,)])
+
+    def test_data_type_bigint(self):
+        with self.tstcon.cursor() as c:
+            long = "create table longboi_bigint(c1 BIGINT) in pybank"
+            c.execute(long)
+            c.execute("insert into longboi_bigint values (?)", (-2**63))
+
+            c.execute("SELECT * from longboi_bigint")
+            self.assertEqual(c.fetchall(), [(-2**63,)])
+
+    @unittest.skip
+    def test_data_type_precision_integer(self):
+        with self.tstcon.cursor() as c:
+            long = "create table longboi_integer45(c1 INTEGER(45)) in pybank"
+            c.execute(long)
+            c.execute("insert into longboi_integer45 values (?)", str(2**145))
+
+            c.execute("SELECT * from longboi_integer45")
+            self.assertEqual(c.fetchall(), [(str(2**140),)])
+
+    def test_parameter_name(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name (c1 boolean,c2 nchar(10),"
+                      "                       c3 int) in pybank")
+            c.execute("insert into bob_name (c1,c3) values (:a,:b)",
+                      {'a':True, 'b':3})
+
+            c.execute("SELECT * from bob_name")
+            self.assertEqual(c.fetchone(), (True, None, 3))
+
+    def test_error_message(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_message (c1 nchar(10)) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into bob_message (c1,c3) values (:a,:b)",
+                        {'a':2,})
+            print()
+            self.assertEqual(c.messages[0][1], (-12202, 'c3 is not a column of an inserted table, updated table or any table identified in a FROM clause'))
+
+    def test_error_exception_errno(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_message_1 (c1 nchar(10)) in pybank")
+            with self.assertRaises(ProgrammingError) as e:
+                c.execute("insert into bob_message_1 (c1,c3) values (:a,:b)",
+                        {'a':2,})
+            self.assertEqual(e.exception.errno, -12202)
+    
+    def test_error_exception_message(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_message_2 (c1 nchar(10)) in pybank")
+            with self.assertRaises(ProgrammingError) as e:
+                c.execute("insert into bob_message_2 (c1,c3) values (:a,:b)",
+                        {'a':2,})
+            self.assertEqual(e.exception.message, "c3 is not a column of an inserted table, updated table or any table identified in a FROM clause")
+    
+    def test_error_exception_str(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_message_3 (c1 nchar(10)) in pybank")
+            with self.assertRaises(ProgrammingError) as e:
+                c.execute("insert into bob_message_3 (c1,c3) values (:a,:b)",
+                        {'a':2,})
+            self.assertEqual(str(e.exception), "-12202 c3 is not a column of an inserted table, updated table or any table identified in a FROM clause")
+
+    def test_parameter_name_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name_2(c1 boolean, c2 nchar(10),"
+                      "                        c3 int) in pybank")
+            c.execute("insert into bob_name_2 (c1,c3,c2) values (:a,:b,:g)",
+                      dict(a=True, b=3, g="bobs table"))
+
+            c.execute("SELECT * from bob_name_2")
+            self.assertEqual(c.fetchone(), (True, "bobs table", 3))
+
+    def test_parameter_name_missing_key(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table pname_miss(c1 boolean,c2 nchar(10),"
+                      "                        c3 int) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("insert into pname_miss(c1,c2) values (:a,:b)",
+                          {'a':True, 'g':3})
+
+    def test_parameter_name_execute_many(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name_e(c1 boolean,c2 nchar(10),"
+                      "                        c3 int) in pybank")
+            c.executemany("insert into bob_name_e(c1,c3) values (:a,:b)",
+                          [{'a':True, 'b':1},
+                           {'a':False, 'b':2},
+                           {'a':True, 'b':3}])
+
+            c.execute("SELECT * from bob_name_e")
+            self.assertEqual(c.fetchall(),
+                             [(True, None, 1),
+                              (False, None, 2),
+                              (True, None, 3)])
+
+    def test_parameter_name_execute_many_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table pname__e2 (c1 boolean,c2 nchar(10),"
+                      "                        c3 int) in pybank")
+            c.executemany("insert into pname__e2 (c1,c3,c2) values (:a,:b,:g)",
+                          [{'a': True, 'b': 1, 'g': "bob table1"},
+                           {'a': False, 'b': 2, 'g': "bob table2"},
+                           {'a': True, 'b': 3, 'g': "bob table3"}])
+            c.execute("SELECT * from pname__e2")
+            self.assertEqual(c.fetchall(),
+                             [(True, 'bob table1', 1),
+                              (False, 'bob table2', 2),
+                              (True, 'bob table3', 3)])
+
+    def test_parameter_name_execute_many_invalid_key(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name_invalid(c1 boolean,c2 nchar(10),"
+                      "                              c3 int) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob_name_invalid (c1,c2)"
+                              " values (:a,:b)",
+                              [{'a':True, 'g':3},
+                               {'a':True, 'g':3}])
+
+    def test_parameter_name_execute_many_mixing(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name__e3 (c1 boolean,c2 nvarchar(10),"
+                      "                           c3 int) in pybank")
+            c.executemany("insert into bob_name__e3 (c1,c2,c3)"
+                          " values (:a,:b,:g)",
+                          [{'a': True, 'g': 1, 'b': "bob table1"},
+                           (True, "string ?", 5),
+                           (True, "string", 5)])
+            c.execute("SELECT * from bob_name__e3")
+            self.assertEqual(c.fetchall(),
+                             [(True, 'bob table1', 1),
+                              (True, 'string ?', 5),
+                              (True, 'string', 5)])
+
+    def test_parameter_name_execute_many_mixing_2(self):
+        with self.tstcon.cursor() as c:
+            c.execute("create table bob_name__e4 (c1 boolean,c2 nvarchar(10),"
+                      "                           c3 int) in pybank")
+            c.executemany("insert into bob_name__e4 (c1,c3,c2)"
+                          " values (:a,:b,:g)",
+                          [(True, 5,"string"),
+                           {'a': True, 'b': 1, 'g': "bob table1"},
+                           (True, 5, "string ?")])
+            c.execute("SELECT * from bob_name__e4")
+            self.assertEqual(c.fetchall(),
+                             [(True, 'string', 5),
+                              (True, 'bob table1', 1),
+                              (True, 'string ?', 5)])
+
+    @unittest.skip
+    def test_help(self):
+        a = mimerpy.connect(dsn=self.dbName, user=self.usrName, password=self.psw)
+        b = a.cursor()
+        help(b)
+        b.close()
+        a.close()
+
+    @unittest.skip
+    def test_error(self):
+        a = mimerpy.connect(dsn=self.dbName, user=self.usrName, password=self.psw)
+        b = a.cursor()
+        b.execute("create table boberror (c1 INTEGER,  c2 NVARCHAR(10)) in pybank")
+        print("table created --------------- ")
+        b.execute("insert into boberror values (:a, :b)", (3, 'bob'))
+        a.close()
+
+
+    if (mimerapi._level == 2):
+        def test_datatype_float_p(self):
+            with self.tstcon.cursor() as c:
+                c.execute("create table floatptable (c1 FLOAT(5)) in pybank")
+                floatnum = str(3.123)
+                c.execute("insert INTO floatptable VALUES (?)", (floatnum))
+                self.tstcon.commit()
+                c.execute("select * from floatptable")
+                r = c.fetchall()[0]
+                self.assertEqual(r[0], decimal.Decimal(floatnum))
+
+        def test_datatype_numeric(self):
+            with self.tstcon.cursor() as c:
+                c.execute("create table floatnumericptable (c1 numeric(5,2)) in pybank")
+                floatnum = str(322.13)
+                c.execute("insert INTO floatnumericptable VALUES (?)", (floatnum))
+                self.tstcon.commit()
+                c.execute("select * from floatnumericptable")
+                r = c.fetchall()[0]
+                self.assertEqual(r[0], decimal.Decimal(floatnum))
+
+        @unittest.skipUnless(db_config.MIMERPY_STABLE == False, "Currently gives incorrect error message")
+        def test_insert_decimal_invalid(self):
+            with self.tstcon.cursor() as c:
+                c.execute("create table jondecimal2 (c1 DECIMAL(5,2)) in pybank")
+                floatnum = '32423.23234'
+                #with self.assertRaises(ProgrammingError):
+                c.execute("insert INTO jondecimal2 VALUES (?)", (floatnum))
+
+
+if __name__ == '__main__':
+    unittest.TestLoader.sortTestMethodsUsing = None
+    unittest.main()
```

### Comparing `mimerpy-1.1.3/tests/testMimerPool.py` & `mimerpy-1.1.4/tests/testMimerPool.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import unittest
-import mimerpy
-import sys
-import pathlib
-import db_config
-
-#To be able to run without installing the package
-m_path = str(pathlib.Path(__file__).parent.parent.absolute())
-sys.path.append(m_path)
-
-
-from mimerpy.pool import (
-    MimerPool, MimerPoolError, MimerPoolExhausted)
-
-__version__ = '1.0'
-
-class TestMimerPool(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(self):
-        (self.syscon, self.tstcon) = db_config.setup()
-        self.DSN = db_config.TSTUSR['dsn']
-        self.USER = db_config.TSTUSR['user']
-        self.PASSWORD = db_config.TSTUSR['password']
-
-    @classmethod
-    def tearDownClass(self):
-        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
-
-
-    def test_pool1_CreateConnection(self):
-        pool = MimerPool(
-            initialconnections=1, maxunused=2, maxconnections=3, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        self.assertEqual(pool.cached_connections, 1)
-        con = pool.get_connection()
-        from mimerpy.pool import PooledConnection
-        self.assertTrue(isinstance(con, PooledConnection))
-        con.close()
-        db = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 1)
-        db2 = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 2)
-        db3 = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 3)
-        db.autocommit(True)
-        cur = db.execute('select * from system.onerow')
-        r = cur.fetchone()
-        cur.close()
-        db.close()
-        self.assertEqual(pool.cached_connections, 1)
-        self.assertEqual(pool.used_connections, 2)
-        db2.close()
-        self.assertEqual(pool.cached_connections, 2)
-        self.assertEqual(pool.used_connections, 1)
-        db3.close()
-        self.assertEqual(pool.cached_connections, 2)
-        self.assertEqual(pool.used_connections, 0)
-        db = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 1)
-        self.assertEqual(pool.used_connections, 1)
-        pool.close()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
-        pool = None
-
-    def test_pool2_CreateConnectionNoMaxCache(self):
-        pool = MimerPool(
-            initialconnections=1, maxunused=0, maxconnections=3, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        del(pool)
-        pool = MimerPool(
-            initialconnections=1, maxunused=0, maxconnections=3, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        self.assertEqual(pool.cached_connections, 1)
-        self.assertEqual(pool.used_connections, 0)
-        con = pool.get_connection()
-        from mimerpy.pool import PooledConnection
-        self.assertTrue(isinstance(con, PooledConnection))
-        con.close()
-        db = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 1)
-        db2 = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 2)
-        db3 = pool.get_connection()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 3)
-        db.autocommit(True)
-        cursor = db.cursor()
-        cursor.execute('select * from system.onerow')
-        r = cursor.fetchone()
-        cursor.close()
-        db.close()
-        self.assertEqual(pool.cached_connections, 1)
-        self.assertEqual(pool.used_connections, 2)
-        db2.close()
-        self.assertEqual(pool.cached_connections, 2)
-        self.assertEqual(pool.used_connections, 1)
-        db3.close()
-        self.assertEqual(pool.cached_connections, 3)
-        self.assertEqual(pool.used_connections, 0)
-        pool.close()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
-
-    def test_pool3_CreateManyConnections(self):
-        #See how many connections the database allows, but no more than max_cons
-        max_cons = 100
-        available_cons = 0
-        cons = []
-        try:
-            while True and available_cons < max_cons:
-                c = mimerpy.mimerpy.connect(dsn = self.DSN, user=self.USER, password=self.PASSWORD)
-                cons.append(c)
-                available_cons = available_cons +1
-        except (mimerpy.mimPyExceptions.OperationalError):
-            pass
-        finally:
-            for c in cons:
-                c.close()                
-                
-        self.assertGreaterEqual(available_cons, 50, "50 available connections ore more needed")
-        pool = MimerPool(
-            initialconnections=5, maxunused=0, maxconnections=10, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        self.assertEqual(pool.cached_connections, 5)
-        self.assertEqual(pool.used_connections, 0)
-
-        cons = [pool.get_connection() for cnt in range(10)]
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 10)
-
-        for con in cons:
-            con.close()
-
-        self.assertEqual(pool.cached_connections, 10)
-        self.assertEqual(pool.used_connections, 0)
-
-        cons = [pool.get_connection() for cnt in range(10)]
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 10)
-        self.assertRaises(MimerPoolExhausted, pool.get_connection)
-        pool.close()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
-        del pool
-
-        pool = MimerPool(
-            initialconnections=5, maxunused=0, maxconnections=available_cons+1, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        #This will be slow since we have to create all the connection
-        cons = [pool.get_connection() for cnt in range(available_cons)]
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, available_cons)
-
-        for con in cons:
-            con.close()
-
-        self.assertEqual(pool.cached_connections, available_cons)
-        self.assertEqual(pool.used_connections, 0)
-        #This will be quick since the connections are already open
-        cons = [pool.get_connection() for cnt in range(available_cons)]
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, available_cons)
-        
-        self.assertRaises(mimerpy.mimPyExceptions.OperationalError, pool.get_connection)
-        for con in cons:
-            con.close()
-
-        self.assertEqual(pool.cached_connections, available_cons)
-        self.assertEqual(pool.used_connections, 0)
-
-        pool.close()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
-
-    def test_pool4_PoolWithStatement(self):
-        with MimerPool(initialconnections=1, maxunused=2, maxconnections=3, block=False,
-                dsn=self.DSN, user=self.USER, password=self.PASSWORD) as pool:
-            self.assertEqual(pool.cached_connections, 1)
-            con = pool.get_connection()
-            from mimerpy.pool import PooledConnection
-            self.assertTrue(isinstance(con, PooledConnection))
-            con.close()
-            db = pool.get_connection()
-            self.assertEqual(pool.cached_connections, 0)
-            self.assertEqual(pool.used_connections, 1)
-            db2 = pool.get_connection()
-            self.assertEqual(pool.cached_connections, 0)
-            self.assertEqual(pool.used_connections, 2)
-            db3 = pool.get_connection()
-            self.assertEqual(pool.cached_connections, 0)
-            self.assertEqual(pool.used_connections, 3)
-            db.autocommit(True)
-            cur = db.execute('select * from system.onerow')
-            r = cur.fetchone()
-            cur.close()
-            db.close()
-            self.assertEqual(pool.cached_connections, 1)
-            self.assertEqual(pool.used_connections, 2)
-            db2.close()
-            self.assertEqual(pool.cached_connections, 2)
-            self.assertEqual(pool.used_connections, 1)
-            db3.close()
-            self.assertEqual(pool.cached_connections, 2)
-            self.assertEqual(pool.used_connections, 0)
-            db = pool.get_connection()
-            self.assertEqual(pool.cached_connections, 1)
-            self.assertEqual(pool.used_connections, 1)
- 
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
- 
-    def test_pool5_PoolConnectionWithStatement(self):
-        pool = MimerPool(
-            initialconnections=1, maxunused=2, maxconnections=3, block=False,
-            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
-        self.assertEqual(pool.cached_connections, 1)
-        with pool.get_connection() as con:
-            from mimerpy.pool import PooledConnection
-            self.assertTrue(isinstance(con, PooledConnection))
-
-        db2 = None
-        with pool.get_connection() as db:
-            self.assertEqual(pool.cached_connections, 0)
-            self.assertEqual(pool.used_connections, 1)
-            db2 = pool.get_connection()
-            self.assertEqual(pool.cached_connections, 0)
-            self.assertEqual(pool.used_connections, 2)
-            cur = db.execute('select * from system.onerow')
-            r = cur.fetchone()
-            cur.close()
-
-        self.assertEqual(pool.cached_connections, 1)
-        self.assertEqual(pool.used_connections, 1)
-        db2.close()
-        self.assertEqual(pool.cached_connections, 2)
-        self.assertEqual(pool.used_connections, 0)
-
-        pool.close()
-        self.assertEqual(pool.cached_connections, 0)
-        self.assertEqual(pool.used_connections, 0)
-
-if __name__ == '__main__':
-    unittest.main()
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import unittest
+import mimerpy
+import sys
+import pathlib
+import db_config
+
+#To be able to run without installing the package
+m_path = str(pathlib.Path(__file__).parent.parent.absolute())
+sys.path.append(m_path)
+
+
+from mimerpy.pool import (
+    MimerPool, MimerPoolError, MimerPoolExhausted)
+
+__version__ = '1.0'
+
+class TestMimerPool(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(self):
+        (self.syscon, self.tstcon) = db_config.setup()
+        self.DSN = db_config.TSTUSR['dsn']
+        self.USER = db_config.TSTUSR['user']
+        self.PASSWORD = db_config.TSTUSR['password']
+
+    @classmethod
+    def tearDownClass(self):
+        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
+
+
+    def test_pool1_CreateConnection(self):
+        pool = MimerPool(
+            initialconnections=1, maxunused=2, maxconnections=3, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        self.assertEqual(pool.cached_connections, 1)
+        con = pool.get_connection()
+        from mimerpy.pool import PooledConnection
+        self.assertTrue(isinstance(con, PooledConnection))
+        con.close()
+        db = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 1)
+        db2 = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 2)
+        db3 = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 3)
+        db.autocommit(True)
+        cur = db.execute('select * from system.onerow')
+        r = cur.fetchone()
+        cur.close()
+        db.close()
+        self.assertEqual(pool.cached_connections, 1)
+        self.assertEqual(pool.used_connections, 2)
+        db2.close()
+        self.assertEqual(pool.cached_connections, 2)
+        self.assertEqual(pool.used_connections, 1)
+        db3.close()
+        self.assertEqual(pool.cached_connections, 2)
+        self.assertEqual(pool.used_connections, 0)
+        db = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 1)
+        self.assertEqual(pool.used_connections, 1)
+        pool.close()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+        pool = None
+
+    def test_pool2_CreateConnectionNoMaxCache(self):
+        pool = MimerPool(
+            initialconnections=1, maxunused=0, maxconnections=3, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        del(pool)
+        pool = MimerPool(
+            initialconnections=1, maxunused=0, maxconnections=3, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        self.assertEqual(pool.cached_connections, 1)
+        self.assertEqual(pool.used_connections, 0)
+        con = pool.get_connection()
+        from mimerpy.pool import PooledConnection
+        self.assertTrue(isinstance(con, PooledConnection))
+        con.close()
+        db = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 1)
+        db2 = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 2)
+        db3 = pool.get_connection()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 3)
+        db.autocommit(True)
+        cursor = db.cursor()
+        cursor.execute('select * from system.onerow')
+        r = cursor.fetchone()
+        cursor.close()
+        db.close()
+        self.assertEqual(pool.cached_connections, 1)
+        self.assertEqual(pool.used_connections, 2)
+        db2.close()
+        self.assertEqual(pool.cached_connections, 2)
+        self.assertEqual(pool.used_connections, 1)
+        db3.close()
+        self.assertEqual(pool.cached_connections, 3)
+        self.assertEqual(pool.used_connections, 0)
+        pool.close()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+
+    def test_pool3_CreateManyConnections(self):
+        #See how many connections the database allows, but no more than max_cons
+        max_cons = 100
+        available_cons = 0
+        cons = []
+        try:
+            while True and available_cons < max_cons:
+                c = mimerpy.mimerpy.connect(dsn = self.DSN, user=self.USER, password=self.PASSWORD)
+                cons.append(c)
+                available_cons = available_cons +1
+        except (mimerpy.mimPyExceptions.OperationalError):
+            pass
+        finally:
+            for c in cons:
+                c.close()                
+                
+        self.assertGreaterEqual(available_cons, 50, "50 available connections ore more needed")
+        pool = MimerPool(
+            initialconnections=5, maxunused=0, maxconnections=10, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        self.assertEqual(pool.cached_connections, 5)
+        self.assertEqual(pool.used_connections, 0)
+
+        cons = [pool.get_connection() for cnt in range(10)]
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 10)
+
+        for con in cons:
+            con.close()
+
+        self.assertEqual(pool.cached_connections, 10)
+        self.assertEqual(pool.used_connections, 0)
+
+        cons = [pool.get_connection() for cnt in range(10)]
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 10)
+        self.assertRaises(MimerPoolExhausted, pool.get_connection)
+        pool.close()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+        del pool
+
+        pool = MimerPool(
+            initialconnections=5, maxunused=0, maxconnections=available_cons+1, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        #This will be slow since we have to create all the connection
+        cons = [pool.get_connection() for cnt in range(available_cons)]
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, available_cons)
+
+        for con in cons:
+            con.close()
+
+        self.assertEqual(pool.cached_connections, available_cons)
+        self.assertEqual(pool.used_connections, 0)
+        #This will be quick since the connections are already open
+        cons = [pool.get_connection() for cnt in range(available_cons)]
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, available_cons)
+        
+        self.assertRaises(mimerpy.mimPyExceptions.OperationalError, pool.get_connection)
+        for con in cons:
+            con.close()
+
+        self.assertEqual(pool.cached_connections, available_cons)
+        self.assertEqual(pool.used_connections, 0)
+
+        pool.close()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+
+    def test_pool4_PoolWithStatement(self):
+        with MimerPool(initialconnections=1, maxunused=2, maxconnections=3, block=False,
+                dsn=self.DSN, user=self.USER, password=self.PASSWORD) as pool:
+            self.assertEqual(pool.cached_connections, 1)
+            con = pool.get_connection()
+            from mimerpy.pool import PooledConnection
+            self.assertTrue(isinstance(con, PooledConnection))
+            con.close()
+            db = pool.get_connection()
+            self.assertEqual(pool.cached_connections, 0)
+            self.assertEqual(pool.used_connections, 1)
+            db2 = pool.get_connection()
+            self.assertEqual(pool.cached_connections, 0)
+            self.assertEqual(pool.used_connections, 2)
+            db3 = pool.get_connection()
+            self.assertEqual(pool.cached_connections, 0)
+            self.assertEqual(pool.used_connections, 3)
+            db.autocommit(True)
+            cur = db.execute('select * from system.onerow')
+            r = cur.fetchone()
+            cur.close()
+            db.close()
+            self.assertEqual(pool.cached_connections, 1)
+            self.assertEqual(pool.used_connections, 2)
+            db2.close()
+            self.assertEqual(pool.cached_connections, 2)
+            self.assertEqual(pool.used_connections, 1)
+            db3.close()
+            self.assertEqual(pool.cached_connections, 2)
+            self.assertEqual(pool.used_connections, 0)
+            db = pool.get_connection()
+            self.assertEqual(pool.cached_connections, 1)
+            self.assertEqual(pool.used_connections, 1)
+ 
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+ 
+    def test_pool5_PoolConnectionWithStatement(self):
+        pool = MimerPool(
+            initialconnections=1, maxunused=2, maxconnections=3, block=False,
+            dsn=self.DSN, user=self.USER, password=self.PASSWORD)
+        self.assertEqual(pool.cached_connections, 1)
+        with pool.get_connection() as con:
+            from mimerpy.pool import PooledConnection
+            self.assertTrue(isinstance(con, PooledConnection))
+
+        db2 = None
+        with pool.get_connection() as db:
+            self.assertEqual(pool.cached_connections, 0)
+            self.assertEqual(pool.used_connections, 1)
+            db2 = pool.get_connection()
+            self.assertEqual(pool.cached_connections, 0)
+            self.assertEqual(pool.used_connections, 2)
+            cur = db.execute('select * from system.onerow')
+            r = cur.fetchone()
+            cur.close()
+
+        self.assertEqual(pool.cached_connections, 1)
+        self.assertEqual(pool.used_connections, 1)
+        db2.close()
+        self.assertEqual(pool.cached_connections, 2)
+        self.assertEqual(pool.used_connections, 0)
+
+        pool.close()
+        self.assertEqual(pool.cached_connections, 0)
+        self.assertEqual(pool.used_connections, 0)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `mimerpy-1.1.3/tests/testMonkey.py` & `mimerpy-1.1.4/tests/testMonkey.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import unittest
-import time
-import math
-import mimerpy
-import random
-import uuid
-import threading
-
-from mimerpy.mimPyExceptions import *
-import db_config
-
-
-class TestMonkey(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(self):
-        (self.syscon, self.tstcon) = db_config.setup()
-
-    @classmethod
-    def tearDownClass(self):
-        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
-
-    def setUp(self):
-        self.tstcon.rollback()
-        with self.tstcon.cursor() as c:
-            c.execute("""
-create table monkeyTable (c1 INTEGER,
-                          c2 BIGINT,
-                          c3 SMALLINT,
-                          c4 NVARCHAR(256),
-                          c5 BLOB,
-                          c6 NCLOB,
-                          c7 BOOLEAN,
-                          c8 FLOAT) in pybank""")
-        self.tstcon.commit()
-
-    def tearDown(self):
-        self.tstcon.rollback()
-        with self.tstcon.cursor() as c:
-            c.execute("drop table monkeyTable")
-        self.tstcon.commit()
-
-########################################################################
-## Tests below
-########################################################################
-
-    def test_cursor_dml(self):
-        cur = self.tstcon.cursor()
-        for nu in range(0,2000):
-            apa = random.randint(0,10)
-            if (apa == 0):
-                self.cursor_select(cur)
-            elif (apa == 1):
-                self.cursor_select_and_fetchone(cur)
-            elif (apa == 2):
-                self.cursor_select_and_fetchmany(cur, nu)
-            elif (apa == 3):
-                self.cursor_select_and_fetchall(cur)
-            elif (apa == 4):
-                self.cursor_insert_executemany(cur)
-            elif (apa == 5):
-                self.cursor_insert(cur)
-            elif (apa == 6):
-                self.cursor_insert_many(cur)
-            elif (apa == 7):
-                try:
-                    self.cursor_next(cur)
-                except StopIteration:
-                    """Caught exception"""
-            elif (apa == 8):
-                self.cursor_commit(self.tstcon)
-            elif (apa == 9):
-                self.cursor_rollback(self.tstcon)
-            elif (apa == 10):
-                self.cursor_description_all(cur)
-        cur.close()
-
-    def test_cursor_ddl_and_dml(self):
-        cur = self.tstcon.cursor()
-        for nu in range(0,1000):
-            apa = random.randint(0,15)
-            if (apa == 0):
-                try:
-                    self.cursor_select(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 1):
-                try:
-                    self.cursor_select_and_fetchone(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 2):
-                try:
-                    self.cursor_select_and_fetchmany(cur, nu)
-                except Exception:
-                    """ Ok """
-
-            elif (apa == 3):
-                try:
-                    self.cursor_select_and_fetchall(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 4):
-                try:
-                    self.cursor_insert_executemany(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 5):
-                try:
-                    self.cursor_insert(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 6):
-                try:
-                    self.cursor_insert_many(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 7):
-                try:
-                    self.cursor_next(cur)
-                except Exception:
-                    """Caught exception"""
-            elif (apa == 8):
-                try:
-                    self.cursor_update(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 9):
-                try:
-                    self.monkey_insert(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 11):
-                try:
-                    self.monkey_select_and_fetchone(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 12):
-                try:
-                    self.cursor_delete(cur)
-                except Exception:
-                    """ Ok """
-            elif (apa == 13):
-                try:
-                    self.cursor_commit(self.tstcon)
-                except Exception:
-                    """ Ok """
-            elif (apa == 14):
-                try:
-                    self.cursor_rollback(self.tstcon)
-                except Exception:
-                    """ Ok """
-            elif (apa == 15):
-                try:
-                    self.cursor_description_all(cur)
-                except Exception:
-                    """ Ok """
-        cur.close()
-
-    def test_condis(self):
-
-        def condis(self):
-            mylist = []
-            for ac in range(5):
-                con = mimerpy.connect(**db_config.TSTUSR)
-                mylist.append([con, True])
-
-            for a in range(100):
-                rand = random.randint(0,4)
-                if (not mylist[rand][1]):
-                    mylist.pop(rand)
-                    conn = mimerpy.connect(**db_config.TSTUSR)
-                    mylist.append([conn, True])
-                else:
-                    mylist[rand][0].close()
-                    mylist[rand][1] = False
-
-            for ab in mylist:
-                if (ab[1]):
-                    ab[0].close()
-
-        for i in range(9):
-            t = threading.Thread(target = condis, args = (self,))
-            t.start()
-        while (threading.active_count() > 1):
-            time.sleep(1)
-
-
-########################################################################
-## No Tests below
-## Support routines follow
-########################################################################
-
-
-    def cursor_insert(self, cur):
-        a = random.randint(-2**31, 2**31 - 1)
-        b = random.randint(-2**63, 2**63 - 1)
-        c = random.randint(-2**15, 2**15 - 1)
-        d = str(uuid.uuid4())
-        e = uuid.uuid4().bytes
-        f = str(uuid.uuid4())
-        g = random.randint(0,1)
-        h = random.random()
-        cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)",[(a),(b),(c),(d),(e),(f),(g),(h)])
-
-    def monkey_insert(self, cur):
-        a = random.randint(-2**100,2**100)
-        d = str(uuid.uuid4() * random.randint(0,1000))
-        g = random.randint(0,1)
-        h = random.random() / 3
-        cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)",[(a),(a),(a),(d),(d),(d),(d),(h)])
-
-    def cursor_select(self, cur):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-
-    def monkey_select(self, cur):
-        cul = random.randint(0,10)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-
-    def cursor_select_and_fetchone(self, cur):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-        cur.fetchone()
-
-    def monkey_select_and_fetchone(self, cur):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-        laps = random.randint(0,100)
-        for a in laps:
-            cur.fetchone()
-
-    def cursor_select_and_fetchmany(self, cur, numboflaps):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-        up = random.randint(0,numboflaps)
-        cur.fetchmany(up)
-
-    def cursor_select_and_fetchall(self, cur):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-        cur.fetchall()
-
-    def cursor_insert_executemany(self, cur):
-        monkeylist = []
-        for m in range(0,10):
-            a = random.randint(-2**31, 2**31 - 1)
-            b = random.randint(-2**63, 2**63 - 1)
-            c = random.randint(-2**15, 2**15 - 1)
-            d = str(uuid.uuid4())
-            e = uuid.uuid4().bytes
-            f = str(uuid.uuid4())
-            g = random.randint(0,1)
-            h = random.random()
-            monkeylist.append((a,b,c,d,e,f,g,h))
-        #print("monkeylist  ", monkeylist)
-        cur.executemany("insert into monkeyTable values (?,?,?,?,?,?,?,?)", monkeylist)
-
-    def cursor_insert_many(self, cur):
-        a = random.randint(-2**31, 2**31 - 1)
-        b = random.randint(-2**63, 2**63 - 1)
-        c = random.randint(-2**15, 2**15 - 1)
-        d = str(uuid.uuid4())
-        e = uuid.uuid4().bytes
-        f = str(uuid.uuid4())
-        g = random.randint(0,1)
-        h = random.random()
-        for a in range(0,10):
-            cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)", ((a),(b),(c),(d),(e),(f),(g),(h)))
-
-    def cursor_next(self, cur):
-        cul = random.randint(1,8)
-        a = "c" + str(cul)
-        query = "select " + a + " from monkeyTable"
-        cur.execute(query)
-        cur.next()
-
-    def cursor_update(self, cur):
-        a = random.randint(-2**31, 2**31 - 1)
-        cur.execute("update monkeyTable set where c1 = ? where c1 < ?", (a, a))
-
-    def cursor_delete(self, cur):
-        a = random.randint(-2**31, 2**31 - 1)
-        cur.execute("delete from monkeyTable where c1 = ? where c1 < ?", (a, a))
-
-    def cursor_next_StopIteration(self, cur):
-        cul = random.randint(1,8)
-        cur.execute("DELETE from monkeyTable")
-        try:
-            cur.next()
-        except StopIteration:
-            """Caught Exception"""
-
-    def cursor_commit(self, conn):
-        conn.commit()
-
-    def cursor_rollback(self, conn):
-        conn.rollback()
-
-    def cursor_description_all(self,cur):
-        cul = random.randint(1,8)
-        cur.execute("select * from monkeyTable")
-        self.assertEqual(cur.description,(('c1', 50, None, None, None, None, None),
-                                        ('c2', 52, None, None, None, None, None),
-                                        ('c3', 48, None, None, None, None, None),
-                                        ('c4', 63, None, None, None, None, None),
-                                        ('c5', 57, None, None, None, None, None),
-                                        ('c6', 59, None, None, None, None, None),
-                                        ('c7', 42, None, None, None, None, None),
-                                        ('c8', 56, None, None, None, None, None),))
-
-
-if __name__ == '__main__':
-    unittest.TestLoader.sortTestMethodsUsing = None
-    unittest.main()
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import unittest
+import time
+import math
+import mimerpy
+import random
+import uuid
+import threading
+
+from mimerpy.mimPyExceptions import *
+import db_config
+
+
+class TestMonkey(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(self):
+        (self.syscon, self.tstcon) = db_config.setup()
+
+    @classmethod
+    def tearDownClass(self):
+        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
+
+    def setUp(self):
+        self.tstcon.rollback()
+        with self.tstcon.cursor() as c:
+            c.execute("""
+create table monkeyTable (c1 INTEGER,
+                          c2 BIGINT,
+                          c3 SMALLINT,
+                          c4 NVARCHAR(256),
+                          c5 BLOB,
+                          c6 NCLOB,
+                          c7 BOOLEAN,
+                          c8 FLOAT) in pybank""")
+        self.tstcon.commit()
+
+    def tearDown(self):
+        self.tstcon.rollback()
+        with self.tstcon.cursor() as c:
+            c.execute("drop table monkeyTable")
+        self.tstcon.commit()
+
+########################################################################
+## Tests below
+########################################################################
+
+    def test_cursor_dml(self):
+        cur = self.tstcon.cursor()
+        for nu in range(0,2000):
+            apa = random.randint(0,10)
+            if (apa == 0):
+                self.cursor_select(cur)
+            elif (apa == 1):
+                self.cursor_select_and_fetchone(cur)
+            elif (apa == 2):
+                self.cursor_select_and_fetchmany(cur, nu)
+            elif (apa == 3):
+                self.cursor_select_and_fetchall(cur)
+            elif (apa == 4):
+                self.cursor_insert_executemany(cur)
+            elif (apa == 5):
+                self.cursor_insert(cur)
+            elif (apa == 6):
+                self.cursor_insert_many(cur)
+            elif (apa == 7):
+                try:
+                    self.cursor_next(cur)
+                except StopIteration:
+                    """Caught exception"""
+            elif (apa == 8):
+                self.cursor_commit(self.tstcon)
+            elif (apa == 9):
+                self.cursor_rollback(self.tstcon)
+            elif (apa == 10):
+                self.cursor_description_all(cur)
+        cur.close()
+
+    def test_cursor_ddl_and_dml(self):
+        cur = self.tstcon.cursor()
+        for nu in range(0,1000):
+            apa = random.randint(0,15)
+            if (apa == 0):
+                try:
+                    self.cursor_select(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 1):
+                try:
+                    self.cursor_select_and_fetchone(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 2):
+                try:
+                    self.cursor_select_and_fetchmany(cur, nu)
+                except Exception:
+                    """ Ok """
+
+            elif (apa == 3):
+                try:
+                    self.cursor_select_and_fetchall(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 4):
+                try:
+                    self.cursor_insert_executemany(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 5):
+                try:
+                    self.cursor_insert(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 6):
+                try:
+                    self.cursor_insert_many(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 7):
+                try:
+                    self.cursor_next(cur)
+                except Exception:
+                    """Caught exception"""
+            elif (apa == 8):
+                try:
+                    self.cursor_update(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 9):
+                try:
+                    self.monkey_insert(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 11):
+                try:
+                    self.monkey_select_and_fetchone(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 12):
+                try:
+                    self.cursor_delete(cur)
+                except Exception:
+                    """ Ok """
+            elif (apa == 13):
+                try:
+                    self.cursor_commit(self.tstcon)
+                except Exception:
+                    """ Ok """
+            elif (apa == 14):
+                try:
+                    self.cursor_rollback(self.tstcon)
+                except Exception:
+                    """ Ok """
+            elif (apa == 15):
+                try:
+                    self.cursor_description_all(cur)
+                except Exception:
+                    """ Ok """
+        cur.close()
+
+    def test_condis(self):
+
+        def condis(self):
+            mylist = []
+            for ac in range(5):
+                con = mimerpy.connect(**db_config.TSTUSR)
+                mylist.append([con, True])
+
+            for a in range(100):
+                rand = random.randint(0,4)
+                if (not mylist[rand][1]):
+                    mylist.pop(rand)
+                    conn = mimerpy.connect(**db_config.TSTUSR)
+                    mylist.append([conn, True])
+                else:
+                    mylist[rand][0].close()
+                    mylist[rand][1] = False
+
+            for ab in mylist:
+                if (ab[1]):
+                    ab[0].close()
+
+        for i in range(9):
+            t = threading.Thread(target = condis, args = (self,))
+            t.start()
+        while (threading.active_count() > 1):
+            time.sleep(1)
+
+
+########################################################################
+## No Tests below
+## Support routines follow
+########################################################################
+
+
+    def cursor_insert(self, cur):
+        a = random.randint(-2**31, 2**31 - 1)
+        b = random.randint(-2**63, 2**63 - 1)
+        c = random.randint(-2**15, 2**15 - 1)
+        d = str(uuid.uuid4())
+        e = uuid.uuid4().bytes
+        f = str(uuid.uuid4())
+        g = random.randint(0,1)
+        h = random.random()
+        cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)",[(a),(b),(c),(d),(e),(f),(g),(h)])
+
+    def monkey_insert(self, cur):
+        a = random.randint(-2**100,2**100)
+        d = str(uuid.uuid4() * random.randint(0,1000))
+        g = random.randint(0,1)
+        h = random.random() / 3
+        cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)",[(a),(a),(a),(d),(d),(d),(d),(h)])
+
+    def cursor_select(self, cur):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+
+    def monkey_select(self, cur):
+        cul = random.randint(0,10)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+
+    def cursor_select_and_fetchone(self, cur):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+        cur.fetchone()
+
+    def monkey_select_and_fetchone(self, cur):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+        laps = random.randint(0,100)
+        for a in laps:
+            cur.fetchone()
+
+    def cursor_select_and_fetchmany(self, cur, numboflaps):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+        up = random.randint(0,numboflaps)
+        cur.fetchmany(up)
+
+    def cursor_select_and_fetchall(self, cur):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+        cur.fetchall()
+
+    def cursor_insert_executemany(self, cur):
+        monkeylist = []
+        for m in range(0,10):
+            a = random.randint(-2**31, 2**31 - 1)
+            b = random.randint(-2**63, 2**63 - 1)
+            c = random.randint(-2**15, 2**15 - 1)
+            d = str(uuid.uuid4())
+            e = uuid.uuid4().bytes
+            f = str(uuid.uuid4())
+            g = random.randint(0,1)
+            h = random.random()
+            monkeylist.append((a,b,c,d,e,f,g,h))
+        #print("monkeylist  ", monkeylist)
+        cur.executemany("insert into monkeyTable values (?,?,?,?,?,?,?,?)", monkeylist)
+
+    def cursor_insert_many(self, cur):
+        a = random.randint(-2**31, 2**31 - 1)
+        b = random.randint(-2**63, 2**63 - 1)
+        c = random.randint(-2**15, 2**15 - 1)
+        d = str(uuid.uuid4())
+        e = uuid.uuid4().bytes
+        f = str(uuid.uuid4())
+        g = random.randint(0,1)
+        h = random.random()
+        for a in range(0,10):
+            cur.execute("insert into monkeyTable values (?,?,?,?,?,?,?,?)", ((a),(b),(c),(d),(e),(f),(g),(h)))
+
+    def cursor_next(self, cur):
+        cul = random.randint(1,8)
+        a = "c" + str(cul)
+        query = "select " + a + " from monkeyTable"
+        cur.execute(query)
+        cur.next()
+
+    def cursor_update(self, cur):
+        a = random.randint(-2**31, 2**31 - 1)
+        cur.execute("update monkeyTable set where c1 = ? where c1 < ?", (a, a))
+
+    def cursor_delete(self, cur):
+        a = random.randint(-2**31, 2**31 - 1)
+        cur.execute("delete from monkeyTable where c1 = ? where c1 < ?", (a, a))
+
+    def cursor_next_StopIteration(self, cur):
+        cul = random.randint(1,8)
+        cur.execute("DELETE from monkeyTable")
+        try:
+            cur.next()
+        except StopIteration:
+            """Caught Exception"""
+
+    def cursor_commit(self, conn):
+        conn.commit()
+
+    def cursor_rollback(self, conn):
+        conn.rollback()
+
+    def cursor_description_all(self,cur):
+        cul = random.randint(1,8)
+        cur.execute("select * from monkeyTable")
+        self.assertEqual(cur.description,(('c1', 50, None, None, None, None, None),
+                                        ('c2', 52, None, None, None, None, None),
+                                        ('c3', 48, None, None, None, None, None),
+                                        ('c4', 63, None, None, None, None, None),
+                                        ('c5', 57, None, None, None, None, None),
+                                        ('c6', 59, None, None, None, None, None),
+                                        ('c7', 42, None, None, None, None, None),
+                                        ('c8', 56, None, None, None, None, None),))
+
+
+if __name__ == '__main__':
+    unittest.TestLoader.sortTestMethodsUsing = None
+    unittest.main()
```

### Comparing `mimerpy-1.1.3/tests/testScrollCursor.py` & `mimerpy-1.1.4/tests/testScrollCursor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1258 +1,1258 @@
-# Copyright (c) 2017 Mimer Information Technology
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-#
-# See license for more details.
-
-import unittest
-import time
-import math
-import mimerpy
-
-from mimerpy.mimPyExceptions import *
-import db_config
-
-class TestScrollCursorMethods(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(self):
-        (self.syscon, self.tstcon) = db_config.setup()
-
-    @classmethod
-    def tearDownClass(self):
-        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
-
-    def tearDown(self):
-        self.tstcon.rollback()
-
-########################################################################
-## Tests below
-########################################################################
-
-    def test_createTable(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10)) in pybank")
-
-    def test_createTable_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobcr1(c1 INTEGER, c2 NVARCHAR(10))")
-            c.execute("create table bobcr2(c1 INTEGER, c2 NVARCHAR(10))")
-            c.execute("create table bobcr3(c1 INTEGER, c2 NVARCHAR(10))")
-            c.execute("create table bobcr4(c1 INTEGER, c2 NVARCHAR(10))")
-
-    def test_createTable_DropTable(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))")
-            c.execute("drop table bob2 CASCADE")
-
-    def test_create_invalid_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon (c1 INTEGER, c2 INTEGER) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("banana INTO jon VALUES (3, 14)")
-
-    def test_create_rollback_table(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonnynothere (c1 INTEGER, c2 INTEGER)")
-            self.tstcon.rollback()
-            c.execute("select * from jonnynothere")
-
-    def test_two_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonny (c1 INTEGER, c2 INTEGER) in pybank")
-            c.execute("select c1 from jonny where c1 = (?)",(2))
-            c.execute("select * from jonny")
-
-    def test_many_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob356 (c1 INTEGER) in pybank")
-            for val in range(100):
-                c.execute("insert into bob356 values (:a)", (val))
-            for gal in range(100):
-                c.execute("select c1 from bob356 where c1 > (?)",(gal))
-                temp = c.fetchall()
-                self.assertEqual(len(temp), 99 - gal)
-
-    def test_select_no_commit(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobc (c1 INTEGER, c2 FLOAT) in pybank")
-            for val in range(100):
-                c.execute("insert into bobc values (:a, :b)", (val, val + 0.5))
-            c.execute("select * from bobc where c1 = 99")
-            self.assertEqual(c.fetchall(),[(99,99.5)])
-
-    def test_select_description(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table description (columnone INTEGER) in pybank")
-            for val in range(10):
-                c.execute("insert into description values (?)", val)
-            c.execute("select * from description")
-            self.assertEqual(c.description,
-                             (('columnone', 50, None, None, None, None, None),))
-
-    def test_select_description2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table description2 (c1 INTEGER, c2 FLOAT)")
-            for val in range(10):
-                c.execute("insert into description2 values (?,?)", (val, val/3))
-            c.execute("select * from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),
-                              ('c2', 56, None, None, None, None, None)))
-            c.execute("select c1 from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),))
-            c.execute("select c2 from description2")
-            self.assertEqual(c.description,
-                             (('c2', 56, None, None, None, None, None),))
-            c.execute("select * from description2")
-            self.assertEqual(c.description,
-                             (('c1', 50, None, None, None, None, None),
-                              ('c2', 56, None, None, None, None, None)))
-
-    def test_select_description3(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table description3 (price INTEGER,"
-                      "                           currentval FLOAT,"
-                      "                           currency NVARCHAR(128),"
-                      "                           rate BIGINT,"
-                      "                           currentyear INTEGER)")
-            for val in range(10):
-                c.execute("insert into description3 values (?,?,?,?,?)",
-                          (val, val/3, 'SEK', 2**61, val+2000))
-            c.execute("select * from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentval', 56, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None)))
-            c.execute("select price, currentyear, currency, rate"
-                      "  from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None)))
-            c.execute("select rate, rate, rate, rate from description3")
-            self.assertEqual(c.description,
-                             (('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None)))
-            c.execute("select * from description3")
-            self.assertEqual(c.description,
-                             (('price', 50, None, None, None, None, None),
-                              ('currentval', 56, None, None, None, None, None),
-                              ('currency', 63, None, None, None, None, None),
-                              ('rate', 52, None, None, None, None, None),
-                              ('currentyear', 50, None, None, None, None, None)))
-
-    def test_select_description4(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            name1 = "e"*127+"q"
-            name2 = "m"*127+"q"
-            query = ("create table description4 (" + name1 + " INTEGER, "
-                     + name2 + " BOOLEAN) in pybank")
-            c.execute(query)
-            for val in range(10):
-                c.execute("insert into description4 values (?,?)", (val,val%2))
-            c.execute("select * from description4")
-            self.assertEqual(c.description,
-                             ((name1, 50, None, None, None, None, None),
-                              (name2, 42, None, None, None, None, None)))
-
-    def test_select_description5(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            name1 = "e"*127+"q"
-            name2 = "m"*127+"q"
-            query = ("create table description5 (" + name1 + " INTEGER, "
-                     + name2 + " BOOLEAN) in pybank")
-            c.execute(query)
-            for val in range(10):
-                c.execute("insert into description5 values (?,?)", (val,val%2))
-            c.execute("select * from description5")
-            self.assertEqual(c.description,
-                             ((name1, 50, None, None, None, None, None),
-                              (name2, 42, None, None, None, None, None)))
-
-    def test_invalid_create(self):
-        b = self.tstcon.cursor(scrollable = True)
-        b.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("creat table jon(i integer)")
-
-    def test_insert_parametermarkers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob1 (c1 INTEGER,  c2 NVARCHAR(10))")
-            c.execute("insert into bob1 values (:a, :b)", (3, 'bob'))
-
-    def test_insert_parametermarkers_long_string(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobstring (c1 INTEGER,  c2 NVARCHAR(256))")
-            string = "mimer" * 40
-            c.execute("insert into bobstring values (:a, :b)", (3, string))
-            self.tstcon.commit()
-            c.execute("select c2 from bobstring")
-            r = c.fetchall()
-            self.assertEqual(r, [(string,)])
-
-    def test_insert_parametermarkers_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob13 (c1 INTEGER, c2 NVARCHAR(10),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob13 values (:a, :b, :c)",
-                          ((1,'pi',14.345),
-                           (2,'pii',14.345),
-                           (-3,'piii',14.345),
-                           (7,'piii',14.345),
-                           (1121231,'piiii',14.345)))
-            self.tstcon.commit()
-            c.execute("select * from bob13")
-            r = c.fetchall()
-            self.assertEqual(r, [(1, 'pi', 14.345),
-                                 (2, 'pii', 14.345),
-                                 (-3, 'piii', 14.345),
-                                 (7, 'piii', 14.345),
-                                 (1121231, 'piiii', 14.345)])
-
-    def test_insert_parametermarkers_russian(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob14 (c1 INTEGER, c2 NVARCHAR(128),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into bob14 values (:a, :b, :c)",
-                          ((1,'продиктованной ангелом',14.345),
-                           (2,'安排他們參',14.345)))
-            self.tstcon.commit()
-            c.execute("select * from bob14")
-            self.assertEqual(c.fetchall(),
-                             [(1,'продиктованной ангелом',14.345),
-                              (2,'安排他們參',14.345)])
-
-    def test_insert_parametermarkers_unicode(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table boby14 (c1 INTEGER, c2 NVARCHAR(128),"
-                      "                     c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            c.executemany("insert into boby14 values (:a, :b, :c)",
-                          ((1,'продиктованной ангелом',14.345),
-                           (2,'安排他們參‱',14.345)))
-            self.tstcon.commit()
-            c.execute("select * from boby14")
-            self.assertEqual(c.fetchall(),
-                             [(1,'продиктованной ангелом',14.345),
-                              (2,'安排他們參‱',14.345)])
-
-    def test_insert_parametermarkers_too_long(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob15 (c1 NVARCHAR(10)) in pybank")
-            self.tstcon.commit()
-            with self.assertRaises(DatabaseError):
-                c.execute("insert into bob15 values (:a)",
-                          ('This sentence is too long'))
-        self.tstcon.commit()
-
-    def test_insert_too_few_parametermarkers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob3 (c1 INTEGER, c2 NVARCHAR(10))")
-            with self.assertRaises(DatabaseError):
-                c.execute("insert into bob3 values (:a, :b)", (3))
-
-    # &&&& Wrong exception. Fixme.
-    @unittest.skip
-    def test_insert_too_many_parametermarkers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob33 (c1 INTEGER, c2 NVARCHAR(10))")
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob33 values (:a, :b)",
-                              ((3,'pi',14), (3,)))
-
-    def test_insert_many_times(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob34(c1 INTEGER, c2 NVARCHAR(10),"
-                      "                   c3 FLOAT) in pybank")
-            for i in range(0, 101):
-                c.execute("insert into bob34 values (5,'ウィキペディ', 4.4543543)")
-        self.tstcon.commit()
-
-    def test_executemany_one_value(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob4 (c1 INTEGER) in pybank")
-            c.executemany("insert into bob4 values (:a)", [(1,)])
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob4 values (:a)", [(1)])
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob4 values (:a)", (1))
-            with self.assertRaises(ProgrammingError):
-                c.executemany("insert into bob4 values (:a)", [1])
-
-    def test_executemany_one_tuple(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob5 (c1 INTEGER, c2 NVARCHAR(10))")
-            c.executemany("insert into bob5 values (:a, :b)", ((1,'bob1'),))
-
-    def test_executemany_several_tuples(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobe6 (c1 INTEGER, c2 NVARCHAR(10))")
-            c.executemany("insert into bobe6 values (:a, :b)",
-                          [(1,'bob1'),
-                           (2, 'bob2'),
-                           (3,'bob3')])
-
-    def test_commit(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob7 (c1 INTEGER, c2 NVARCHAR(10))")
-            c.executemany("insert into bob7 values (:a, :b)",
-                          ((1,'bob1'),
-                           (2, 'bob2'),
-                           (3,'bob3')))
-        self.tstcon.commit()
-
-    def test_fetchone(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob8 (c1 INTEGER, c2 NVARCHAR(10))")
-
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("insert into bob8 values (:a, :b)", (8, 'bob'))
-            self.tstcon.commit()
-            c.execute("select * from bob8")
-            self.assertEqual(c.fetchone(), (8, 'bob'))
-
-    def test_fetchmany(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob9 (c1 INTEGER, c2 NVARCHAR(10))")
-
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.executemany("insert into bob9 values (:a, :b)",
-                          ((9, 'bob9'),
-                           (10, 'bob10'),
-                           (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob9")
-            self.assertEqual(c.fetchmany(3),
-                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
-
-    def test_fetchmany_too_many(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob11 (c1 INTEGER, c2 NVARCHAR(10))")
-            self.tstcon.commit()
-            c.executemany("insert into bob11 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob11")
-            self.assertEqual(c.fetchmany(5),
-                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
-
-    def test_fetchmany_notall(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob12 (c1 INTEGER, c2 NVARCHAR(10))")
-            self.tstcon.commit()
-            c.executemany("insert into bob12 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob12")
-            self.assertEqual(c.fetchmany(2), [(9, 'bob9'), (10, 'bob10')])
-            self.assertEqual(c.fetchmany(2), [(11, 'bob11')])
-
-    def test_fetchall(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob10 (c1 INTEGER, c2 NVARCHAR(10))")
-            c.executemany("insert into bob10 values (:a, :b)",
-                          ((10, 'bob10'), (11, 'bob11'), (12, 'bob12'),))
-            self.tstcon.commit()
-            c.execute("select * from bob10")
-            self.assertEqual(c.fetchall(),
-                             [(10, 'bob10'),(11, 'bob11'), (12, 'bob12')])
-
-    def test_fetchall_correct_number_of_rows(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob101(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            for d in range(1, 101):
-                c.execute("insert into bob101 values (5,'ウィキペディ', 4.4543543)")
-            self.tstcon.commit()
-            c.execute("select * from bob101")
-            r = c.fetchall()
-            self.assertEqual(len(r), 100)
-
-    def test_fetchall_correct_number_of_rows2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob102(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-            self.tstcon.commit()
-            for i in range(1, 101):
-                c.execute("insert into bob102 values (5,'ウィキペディ',"
-                          " 4.4543543)")
-            self.tstcon.rollback()
-            c.execute("select * from bob102")
-            r = c.fetchall()
-            self.assertEqual(len(r), 0)
-
-    @unittest.skip
-    def test_fetchall_correct_number_of_rows3(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob109(c1 INTEGER, c2 NVARCHAR(100),"
-                      "                    c3 FLOAT) in pybank")
-            for i in range(1, 101):
-                c.execute("insert into bob109 values (5,'ウィキペディ',"
-                          " 4.4543543)")
-            self.tstcon.rollback()
-            c.execute("select * from bob109")
-            r = c.fetchall()
-            self.assertEqual(len(r), 0)
-
-    def test_use_next(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobnext(c1 INTEGER) in pybank")
-            for i in range(0, 10):
-                c.execute("insert into bobnext values (?)", i)
-            self.tstcon.commit()
-            c.execute("select * from bobnext")
-            for i in range(0,10):
-                (val,) = c.next()
-                self.assertEqual(val, i)
-
-    def test_use_next_StopIteration(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobstop(c1 INTEGER) in pybank")
-            for i in range(0, 10):
-                c.execute("insert into bobstop values (?)", i)
-            self.tstcon.commit()
-            c.execute("select * from bobstop")
-            for i in range(0,10):
-                c.next()
-            with self.assertRaises(StopIteration):
-                c.next()
-
-    def test_insert_wrong_type_parametermarkers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob1337 (c1 INTEGER, c2 INTEGER)")
-            with self.assertRaises(DataError):
-                c.execute("insert into bob1337  values (:a, :b)", (3, 3.14))
-
-    def test_operate_after_closed(self):
-        b = self.tstcon.cursor(scrollable = True)
-        b.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("select * from jon")
-
-    def test_operate_after_closed_2(self):
-        b = self.tstcon.cursor(scrollable = True)
-        b.close()
-        b.close()
-        with self.assertRaises(ProgrammingError):
-            b.execute("Kalle")
-        with self.assertRaises(ProgrammingError):
-            b.executemany("Kalle", ("Kula"))
-        with self.assertRaises(ProgrammingError):
-            b.fetchone()
-        with self.assertRaises(ProgrammingError):
-            b.fetchmany("Kalle")
-        with self.assertRaises(ProgrammingError):
-            b.fetchall()
-        with self.assertRaises(ProgrammingError):
-            b.next()
-
-    def test_invalid_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            with self.assertRaises(ProgrammingError):
-                c.execute("select * from jonisnotatablejo where c1 = ?", (5))
-
-    def test_same_table_twice(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob2437(c1 INTEGER) in pybank")
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob2437(c1 INTEGER) in pybank")
-
-    def test_invalid_sequence_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob6565(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("select * from bob6565")
-            r = c.fetchone()
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob6569(c1 INTEGER) in pybank")
-            self.tstcon.rollback()
-
-    #borde bli fel men blir rätt....
-    def test_invalid_sequence_select_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob555(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("select * from bob555")
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob556(c1 INTEGER) in pybank")
-            self.tstcon.rollback()
-            c.execute("create table bob556(c1 INTEGER) in pybank")
-            c.execute("insert into bob556 values (3)")
-            c.execute("select * from bob556")
-            self.assertEqual(c.fetchone(), (3,))
-
-    def test_invalid_sequence_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob6567(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bob6567 values (3)")
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob6566(c1 INTEGER) in pybank")
-            self.tstcon.rollback()
-
-    def test_invalid_sequence_insert_parametermarkers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob6568(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bob6568 values (?)", (3))
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bob6566(c1 INTEGER) in pybank")
-            self.tstcon.rollback()
-
-    def test_executemany_DDL(self):
-        with self.assertRaises(ProgrammingError):
-            c = self.tstcon.executemany("create table bob6(c1 INTEGER)", (3))
-        with self.tstcon.cursor(scrollable = True) as c:
-            with self.assertRaises(ProgrammingError):
-                c.execute("select * from bob6")
-
-    def test_insert_exceeded(self):
-        c = self.tstcon.execute("create table bob16(c1 INTEGER) in pybank")
-        big = pow(2,100)
-        with self.assertRaises(DataError):
-            c.execute("insert into bob16 values (?)", big)
-
-    def test_insert_too_long(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob17(c1 NVARCHAR(10)) in pybank")
-            self.tstcon.commit()
-            with self.assertRaises(DataError):
-                c.execute("insert into bob17 values ('ウィキペデBobWasABoy')")
-            self.tstcon.commit()
-
-    def test_valid_int32_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon32 (c1 INTEGER, c2 INTEGER) in pybank")
-            nvar = -2**31
-            var = 2**31 - 1
-            c.execute("insert INTO jon32 VALUES (?, ?)", (nvar, var))
-
-    def test_invalid_int32_insert_too_small(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon31 (c1 INTEGER) in pybank")
-            nvar = -2**31 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon31 VALUES (?)", (nvar))
-
-    def test_invalid_int32_insert_too_big(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon33 (c1 INTEGER) in pybank")
-            var = 2**31
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon33 VALUES (?)", (var))
-
-    def test_valid_int64_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon64 (c1 BIGINT, c2 BIGINT) in pybank")
-            nvar = -2**63
-            var = 2**63 - 1
-            c.execute("insert INTO jon64 VALUES (?,?)", (nvar,var))
-
-    def test_overflow_int64_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table intjon4 (c1 BIGINT, c2 BIGINT) in pybank")
-            nvar = -2**633
-            var = 2**63 - 1
-            with self.assertRaises(DataError):
-                c.executemany("insert INTO intjon4 VALUES (?,?)",
-                              ((nvar,var),(nvar,var)))
-
-    def test_invalid_int64_insert_too_small(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon63 (c1 BIGINT) in pybank")
-            nvar = -2**63 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon63 VALUES (?)", (nvar))
-
-    def test_invalid_int64_insert_too_big(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon65 (c1 BIGINT) in pybank")
-            var = 2**63
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon65 VALUES (?)", (var))
-
-    def test_valid_int16_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon26 (c1 SMALLINT, c2 SMALLINT)")
-            nvar = -2**15
-            var = 2**15 - 1
-            c.execute("insert INTO jon26 VALUES (?, ?)", (nvar, var))
-
-    def test_invalid_int16_insert_too_small(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon15 (c1 SMALLINT) in pybank")
-            nvar = -2**15 - 1
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon15 VALUES (?)", (nvar))
-
-    def test_invalid_int16_insert_too_small(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon17 (c1 SMALLINT) in pybank")
-            nvar = 2**15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jon17 VALUES (?)", (nvar))
-
-    # &&&& Gives a Warning we dont catch atm
-    def test_valid_double_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon16 (c1 REAL, c2 DOUBLE PRECISION)")
-            var = 2/3
-            c.execute("insert INTO jon16 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-
-    def test_valid_double_insert_none(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon18 (c1 REAL, c2 DOUBLE PRECISION)")
-            var = None
-            c.execute("insert INTO jon18 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-
-    def test_valid_double_select_none(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jon19 (c1 REAL, c2 DOUBLE PRECISION)")
-            var = None
-            c.execute("insert INTO jon19 VALUES (?, ?)", (var, var))
-            self.tstcon.commit()
-            c.execute("select * from jon19")
-            self.assertEqual(c.fetchall(), [(None, None)])
-
-    def test_message_cleared(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonwas17 (c1 SMALLINT) in pybank")
-            nvar = 2**15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jonwas17 VALUES (?)", (nvar))
-            c.execute("insert INTO jonwas17 VALUES (?)", (5))
-            self.assertEqual(c.messages, [])
-
-    def test_message_cleared_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonwas173 (c1 SMALLINT) in pybank")
-            nvar = 2**15
-            with self.assertRaises(DataError):
-                c.execute("insert INTO jonwas173 VALUES (?)", (nvar))
-            self.assertEqual(c.messages[0][1],
-                             (-24010,
-                              'Value was too large to fit in destination'))
-
-    def test_None_is_returned(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonNone (c1 INTEGER) in pybank")
-            for i in range(1,10):
-                c.execute("Insert INTO jonNone VALUES (?)", (i,))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonNone")
-            for i in range(1,10):
-                c.fetchone()
-            self.assertEqual(c.fetchone(), [])
-
-    def test_empty_sequence_is_returned_many(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonEmpty (c1 INTEGER) in pybank")
-            for i in range(1,10):
-                c.execute("Insert INTO jonEmpty VALUES (?)", (i))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonEmpty")
-            c.fetchmany(10)
-            self.assertEqual(c.fetchmany(10), [])
-
-    def test_empty_sequence_is_returned_all(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonEmpty2 (c1 INTEGER) in pybank")
-            for i in range(1,10):
-                c.execute("Insert INTO jonEmpty2 VALUES (?)", (i))
-            self.tstcon.commit()
-            c.execute("SELECT * from jonEmpty2")
-            c.fetchall()
-            self.assertEqual(c.fetchall(), [])
-
-    def test_empty_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonEmp (c1 NVARCHAR(128)) in pybank")
-            c.executemany("Insert INTO jonEmp VALUES (?)",
-                          (('',),("",),(" ",)))
-            self.tstcon.commit()
-            c.execute("select * from jonEmp")
-            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
-
-    def test_empty_insert2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonEmp2 (c1 NVARCHAR(128)) in pybank")
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (''))
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (""))
-            c.execute("Insert INTO jonEmp2 VALUES (?)", (" "))
-            self.tstcon.commit()
-            c.execute("select * from jonEmp2")
-            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
-
-    def test_invalid_databank(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            with self.assertRaises(ProgrammingError):
-                c.execute("create table bjonEmp2 (c1 NVARCHAR(128)) in potato")
-
-    def test_insert_rowcount_update(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrowcount(c1 INTEGER, c2 NVARCHAR(256))")
-            string = "mimer"
-            c.execute("insert into bobrowcount values (:a, :b)", (3, string))
-            self.assertEqual(c.rowcount, 1)
-            c.executemany("insert into bobrowcount values (:a, :b)",
-                          ((5,string),(2,string)))
-            # self.assertEqual(c.rowcount, 2) # &&&& Should we set rowcount????
-            c.execute("select * from bobrowcount")
-            r = c.fetchall()
-            self.assertEqual(c.rowcount, 3)
-
-    def test_delete(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrowcount2(c1 INTEGER) in pybank")
-            for i in range(1,11):
-                c.execute("INSERT into bobrowcount2 values (?)", 10)
-                c.execute("INSERT into bobrowcount2 values (?)", 20)
-            c.execute("INSERT into bobrowcount2 values (?)", 10)
-            c.execute("SELECT * from bobrowcount2")
-            self.assertEqual(len(c.fetchall()), 21)
-            c.execute("DELETE from bobrowcount2 where c1 = 10")
-            self.assertEqual(c.rowcount, 11)
-            c.execute("SELECT * from bobrowcount2")
-            self.assertEqual(len(c.fetchall()), 10)
-
-    def test_update(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobupdate(c1 INTEGER) in pybank")
-            for i in range(1,11):
-                c.execute("INSERT into bobupdate values (?)", 10)
-                c.execute("INSERT into bobupdate values (?)", 20)
-            c.execute("INSERT into bobupdate values (?)", 10)
-            c.execute("SELECT * from bobupdate")
-            self.assertEqual(len(c.fetchall()), 21)
-            c.execute("UPDATE bobupdate SET c1 = ? WHERE c1 = 20", 30)
-            self.assertEqual(c.rowcount, 10)
-            c.execute("SELECT * from bobupdate")
-            self.assertEqual(len(c.fetchall()), 21)
-
-    def test_invalid_sequence_fetchone(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonfetchone (c1 INTEGER) in pybank")
-            for i in range(1,10):
-                c.execute("Insert INTO jonfetchone VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchone()
-
-    def test_isolated(self):
-        c1 = self.tstcon.cursor()
-        c2 = self.tstcon.cursor()
-        c1.execute("create table jonisolated (c1 INTEGER) in pybank")
-        for i in range(1,6):
-            c1.execute("Insert INTO jonisolated VALUES (?)", (i))
-        c2.execute("SELECT * FROM jonisolated")
-        r2 = c2.fetchall()
-        self.assertEqual(len(r2), 5)
-        self.assertEqual(r2, [(1,),(2,),(3,),(4,),(5,),])
-
-    def test_invalid_sequence_fetchmany(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonfetchmany (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonfetchmany VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchmany(10)
-
-    def test_invalid_sequence_fetchall(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonfetchall (c1 INTEGER) in pybank")
-            for i in range(1, 10):
-                c.execute("Insert INTO jonfetchall VALUES (?)", (i))
-            self.tstcon.commit()
-            with self.assertRaises(ProgrammingError):
-                c.fetchall()
-
-    @unittest.skip
-    # &&&& need to find a picture to put in the repo
-    # Nä, gör en psudorandom-blob
-    def test_insert_blob(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonblob (c1 BLOB(18389)) in pybank")
-            with open("../minikappa.jpg", 'rb') as input_file:
-                ablob = input_file.read()
-                c.execute("insert INTO jonblob VALUES (?)", (ablob))
-                self.tstcon.commit()
-                c.execute("select * from jonblob")
-                r = b.fetchall()[0]
-                self.assertEqual(r[0], ablob)
-
-    @unittest.skip
-    # &&&& need to find a picture to put in the repo
-    # Nä, gör en psudorandom-blob
-    def test_insert_blob_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonblob2 (c1 BLOB(64111)) in pybank")
-            with open("../mimerss.png", 'rb') as input_file:
-                ablob = input_file.read()
-                c.execute("insert INTO jonblob2 VALUES (?)", (ablob))
-                self.tstcon.commit()
-                c.execute("select * from jonblob2")
-                r = c.fetchall()[0]
-                self.assertEqual(r[0], ablob)
-
-    @unittest.skip
-    # &&&& need to find a picture to put in the repo
-    # Nä, gör en psudorandom-blob
-    def test_insert_blob_3(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonblob3 (c1 BLOB(3000000)) in pybank")
-            with open("../mimerd.jpg", 'rb') as input_file:
-                ablob = input_file.read()
-                c.execute("insert INTO jonblob3 VALUES (?)", (ablob))
-                self.tstcon.commit()
-                c.execute("select * from jonblob3")
-                r = c.fetchall()[0][0]
-            self.assertEqual(r, ablob)
-
-    @unittest.skip
-    # &&&& need to find a picture to put in the repo
-    # Nä, gör en psudorandom-blob
-    def test_insert_blob_4(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonblob4 (c1 BLOB(3000000)) in pybank")
-            with open("../kappa.jpg", 'rb') as input_file:
-                ablob = input_file.read()
-                c.execute("insert INTO jonblob4 VALUES (?)", (ablob))
-                self.tstcon.commit()
-                c.execute("select * from jonblob4")
-                r = c.fetchall()[0][0]
-            self.assertEqual(r, ablob)
-
-    def test_insert_nclob(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonnclob (c1 NCLOB(50000)) in pybank")
-            anclob = "mimer" * 1000
-            c.execute("insert INTO jonnclob VALUES (?)", (anclob))
-            self.tstcon.commit()
-            c.execute("select * from jonnclob")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], anclob)
-
-    def test_insert_binary(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonbinary (c1 BINARY(3)) in pybank")
-            c.execute("insert INTO jonbinary VALUES (x'ABCD01')")
-            c.execute("insert INTO jonbinary VALUES (?)", (b'A01'))
-            self.tstcon.commit()
-            c.execute("select * from jonbinary")
-            r = c.fetchall()
-            self.assertEqual(r, [(b'\xab\xcd\x01',), (b'A01',)])
-
-    def test_insert_binary_parameter_markers(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonbinary2 (c1 BINARY(2)) in pybank")
-            bob = b'\xab\xcd'
-            c.execute("insert INTO jonbinary2 VALUES (?)", (bob))
-            self.tstcon.commit()
-            c.execute("select * from jonbinary2")
-            (r,) = c.fetchall()[0]
-            self.assertEqual(r, bob)
-
-    @unittest.skip
-    def test_insert_nclob_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonnclob2 (c1 Nclob(450000)) in pybank")
-            with open("../book2.txt", "r") as input_file:
-                anclob = input_file.read()
-                c.execute("insert INTO jonnclob2 VALUES (?)", (anclob))
-                self.tstcon.commit()
-                c.execute("select * from jonnclob2")
-                r = c.fetchall()[0]
-                self.assertEqual(r[0], anclob)
-
-    def test_insert_clob(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table jonclob (c1 clob(30000)) in pybank")
-            anclob = "mimer" * 5
-            c.execute("insert INTO jonclob VALUES (?)", (anclob))
-            self.tstcon.commit()
-            c.execute("select * from jonclob")
-            r = c.fetchall()[0]
-            self.assertEqual(r[0], anclob)
-
-    def test_insert_bool(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobybool (c1 boolean) in pybank")
-            c.execute("insert INTO bobybool VALUES (?)", (False))
-            c.execute("insert INTO bobybool VALUES (?)", (True))
-            c.execute("insert INTO bobybool VALUES (?)", (None))
-            c.execute("insert INTO bobybool VALUES (?)", (45))
-            self.tstcon.commit()
-
-    def test_select_bool(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobybool2 (c1 boolean) in pybank")
-            c.execute("insert INTO bobybool2 VALUES (?)", (False))
-            c.execute("insert INTO bobybool2 VALUES (?)", (True))
-            c.execute("insert INTO bobybool2 VALUES (?)", (None))
-            c.execute("insert INTO bobybool2 VALUES (?)", (45))
-            self.tstcon.commit()
-            c.execute("select * from bobybool2")
-            r = c.fetchone()
-            self.assertEqual(r[0], False)
-            r = c.fetchone()
-            self.assertEqual(r[0], True)
-            r = c.fetchone()
-            self.assertEqual(r[0], None)
-            r = c.fetchone()
-            self.assertEqual(r[0], True)
-
-    def test_get_connection(self):
-        b = self.tstcon.cursor(scrollable = True)
-        self.assertEqual(b.connection, self.tstcon)
-        b.close()
-
-    def test_for(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table fortable (c1 INTEGER) in pybank")
-            c.execute("insert INTO fortable VALUES (?)", (45))
-            c.execute("select * from fortable")
-            for val in c:
-                self.assertEqual(val[0], 45)
-
-    def test_result_set_twice(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table kor (c1 INTEGER) in pybank")
-            c.execute("insert INTO kor VALUES (?)", (45))
-            c.execute("select * from kor")
-            for val in c:
-                self.assertEqual(val[0], 45)
-            c.execute("select * from kor")
-            for val in c:
-                self.assertEqual(val[0], 45)
-            c.execute("select c1 from kor")
-            for val in c:
-                self.assertEqual(val[0], 45)
-
-    def test_executemany_none(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table manytable (c1 INTEGER) in pybank")
-            c.executemany("insert INTO manytable VALUES (?)",
-                          [(2,),(34,),(435,),(34,),(63,),(47,),(None,)])
-            self.tstcon.commit()
-
-    def test_select_executemany(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobyselect (c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            c.execute("insert INTO bobyselect VALUES (?)", (1))
-            with self.assertRaises(ProgrammingError):
-                c.executemany("select * from bobyselect where c1 = (?)",
-                              ((5,),(10,)))
-
-    def test_select_twice(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bananaselect (c1 INTEGER) in pybank")
-            c.execute("select * from bananaselect where c1 = (?)", (5))
-            c.execute("select c1 from bananaselect where c1 = (?)", (7))
-
-    def test_fetchall_no_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            with self.assertRaises(ProgrammingError):
-                c.fetchone()
-            with self.assertRaises(ProgrammingError):
-                c.fetchmany()
-            with self.assertRaises(ProgrammingError):
-                c.fetchall()
-
-    def test_bool_insert(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table boolt (c1 BOOLEAN) in pybank")
-            c.executemany("insert into boolt values (?)",
-                          [(None,), (1,), (0,), (3.1415,),
-                           ("potato",), ('code',)])
-            c.execute("select * from boolt")
-
-    def test_insert_parametermarkers_different_types(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob176(c1 NVARCHAR(128)) in pybank")
-            c.execute("INSERT INTO bob176 VALUES (?)", "bar")    # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ("bar"))  # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ("bar",)) # correct
-            c.execute("INSERT INTO bob176 VALUES (?)", ["bar"])  # correct
-            self.tstcon.commit()
-            c.execute("select * from bob176")
-            self.assertEqual(c.fetchall(),
-                             [("bar",),("bar",),("bar",),("bar",)])
-
-    def test_insert_bigint(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobbig17(c1 BIGINT) in pybank")
-            self.tstcon.commit()
-            c.execute("insert into bobbig17 values (234)")
-            self.tstcon.commit()
-
-    @unittest.skip
-    def test_help(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            help(c)
-
-    #ScrollCursor specific tests
-
-    def test_fetchone_2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bob853 (c1 INTEGER, c2 NVARCHAR(10))")
-            self.tstcon.commit()
-            c.executemany("insert into bob853 values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bob853")
-            self.assertEqual(c.fetchone(), (9, 'bob9'))
-            self.assertEqual(c.fetchone(), (10, 'bob10'))
-            self.assertEqual(c.fetchone(), (11, 'bob11'))
-            self.assertEqual(c.fetchone(), [])
-
-    def test_fetchone_rownumber(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow (c1 INTEGER, c2 NVARCHAR(10))")
-            c.executemany("insert into bobrow values (:a, :b)",
-                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
-            self.tstcon.commit()
-            c.execute("select * from bobrow")
-            self.assertEqual(c.rownumber, 0)
-            self.assertEqual(c.fetchone(), (9, 'bob9'))
-            self.assertEqual(c.rownumber, 1)
-            self.assertEqual(c.fetchone(), (10, 'bob10'))
-            self.assertEqual(c.rownumber, 2)
-            self.assertEqual(c.fetchone(), (11, 'bob11'))
-            self.assertEqual(c.rownumber, 3)
-            self.assertEqual(c.fetchone(), [])
-            self.assertEqual(c.rownumber, 3)
-
-    def test_fetchmany_rownumber(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow2(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 11):
-                c.execute("insert into bobrow2 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow2")
-            self.assertEqual(c.rownumber, 0)
-            self.assertEqual(c.fetchmany(3),
-                             [(1, 'bob1'),(2, 'bob2'),(3, 'bob3')])
-            self.assertEqual(c.rownumber, 3)
-            self.assertEqual(c.fetchmany(3),
-                             [(4, 'bob4'),(5, 'bob5'),(6, 'bob6')])
-            self.assertEqual(c.rownumber, 6)
-            self.assertEqual(c.fetchmany(10),
-                             [(7, 'bob7'),(8, 'bob8'),(9, 'bob9'),(10, 'bob10')])
-            self.assertEqual(c.rownumber, 10)
-            self.assertEqual(c.fetchmany(2), [])
-
-    def test_fetchall_rownumber(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow3(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 6):
-                c.execute("insert into bobrow3 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow3")
-            self.assertEqual(c.rownumber, 0)
-            self.assertEqual(c.fetchall(),
-                             [(1, 'bob1'),(2, 'bob2'),(3, 'bob3'),
-                              (4, 'bob4'),(5, 'bob5')])
-            self.assertEqual(c.rownumber, 5)
-            self.assertEqual(c.fetchall(), [])
-
-    def test_mixfetch_rownumber(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow4(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 11):
-                c.execute("insert into bobrow4 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow4")
-            self.assertEqual(c.rownumber, 0)
-            self.assertEqual(c.fetchone(), (1, 'bob1'))
-            self.assertEqual(c.rownumber, 1)
-            self.assertEqual(c.fetchmany(3),
-                             [(2, 'bob2'),(3, 'bob3'), (4, 'bob4')])
-            self.assertEqual(c.rownumber, 4)
-            self.assertEqual(c.fetchone(), (5, 'bob5'))
-            self.assertEqual(c.rownumber, 5)
-            self.assertEqual(c.fetchall(),
-                             [(6, 'bob6'),(7, 'bob7'),(8, 'bob8'),
-                              (9, 'bob9'),(10, 'bob10')])
-            self.assertEqual(c.rownumber, 10)
-            self.assertEqual(c.fetchone(), [])
-            self.assertEqual(c.fetchmany(21), [])
-            self.assertEqual(c.fetchall(), [])
-
-    def test_mixfetch_rowcount(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow5(c1 INTEGER) in pybank")
-            for i in range(1, 101):
-                c.execute("insert into bobrow5 values (?)", (i))
-            self.tstcon.commit()
-            c.execute("select * from bobrow5")
-            self.assertEqual(c.rowcount, 100)
-            c.execute("select c1 from bobrow5 where c1 >= ?", (50))
-            self.assertEqual(c.rowcount, 51)
-            c.execute("select c1 from bobrow5 where c1 < ?", (10))
-            self.assertEqual(c.rowcount, 9)
-
-    def test_scroll(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow6(c1 INTEGER) in pybank")
-            for i in range(1, 101):
-                c.execute("insert into bobrow6 values (?)", (i))
-            self.tstcon.commit()
-            c.execute("select * from bobrow6")
-            c.scroll(2,mode='relative')
-            self.assertEqual(c.rownumber, 2)
-            self.assertEqual(c.fetchone(), (3,))
-            c.scroll(3,mode='relative')
-            self.assertEqual(c.rownumber, 6)
-            self.assertEqual(c.fetchone(), (7,))
-            c.scroll(3,mode='absolute')
-            self.assertEqual(c.rownumber, 3)
-            c.scroll(5,mode='relative')
-            self.assertEqual(c.rownumber, 8)
-
-    def test_scroll_error(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow7(c1 INTEGER) in pybank")
-            for i in range(1, 101):
-                c.execute("insert into bobrow7 values (?)", (i))
-            self.tstcon.commit()
-            c.execute("select * from bobrow7")
-            with self.assertRaises(ProgrammingError):
-                c.scroll(5,mode='nonexistingmode')
-            with self.assertRaises(IndexError):
-                c.scroll(101,mode='absolute')
-
-    def test_next(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow8(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 11):
-                c.execute("insert into bobrow8 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow8")
-            self.assertEqual(c.next(), (1, 'bob1'),)
-            c.scroll(5,mode='relative')
-            self.assertEqual(c.next(), (7, 'bob7'),)
-            c.scroll(9, mode='absolute')
-
-    def test_next_fetch(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow10(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 11):
-                c.execute("insert into bobrow10 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow10")
-            self.assertEqual(c.fetchone(), (1, 'bob1'),)
-            self.assertEqual(c.next(), (2, 'bob2'),)
-            self.assertEqual(c.fetchmany(2), [(3, 'bob3'), (4, 'bob4')])
-            self.assertEqual(c.next(), (5, 'bob5'),)
-            c.scroll(1, mode='relative')
-            self.assertEqual(c.fetchall(),
-                             [(7, 'bob7'), (8, 'bob8'),
-                              (9, 'bob9'), (10, 'bob10')])
-
-    def test_next_error(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobrow9(c1 INTEGER, c2 NVARCHAR(100))")
-            for i in range(1, 11):
-                c.execute("insert into bobrow9 values (:a, :b)",
-                          (i, 'bob' + str(i) ))
-            self.tstcon.commit()
-            c.execute("select * from bobrow9")
-            c.scroll(9, mode='absolute')
-            with self.assertRaises(StopIteration):
-                c.next()
-                c.next()
-
-    def test_fetchall_IndexError(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table indexerror (c1 INTEGER) in pybank")
-            for val in range(0,10):
-                c.execute("insert INTO indexerror VALUES (?)", (val))
-            c.execute("select * from indexerror")
-            r = c.fetchmany(9)
-            r = c.fetchall()
-
-    def test_fetchall_Scroll_outside(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table scrolloutside (c1 INTEGER) in pybank")
-            for val in range(0,10):
-                c.execute("insert INTO scrolloutside VALUES (?)", (val))
-            c.execute("select * from scrolloutside")
-            with self.assertRaises(IndexError):
-                r = c.scroll(100)
-
-    def test_no_select(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobnoselect(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            for i in range(1, 11):
-                c.execute("insert into bobnoselect values (5)")
-            self.tstcon.rollback()
-            c.execute("select * from bobnoselect")
-            r = c.fetchone()
-            self.assertEqual(len(r), 0)
-
-    def test_no_select2(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobnoselect2(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            for i in range(1, 11):
-                c.execute("insert into bobnoselect2 values (5)")
-            self.tstcon.rollback()
-            c.execute("select * from bobnoselect2")
-            r = c.fetchmany(5)
-            self.assertEqual(len(r), 0)
-
-    def test_no_select3(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            c.execute("create table bobnoselect3(c1 INTEGER) in pybank")
-            self.tstcon.commit()
-            for i in range(1, 11):
-                c.execute("insert into bobnoselect3 values (5)")
-            self.tstcon.rollback()
-            c.execute("select * from bobnoselect3")
-            r = c.next()
-            self.assertEqual(len(r), 0)
-
-    def test_next_noselect(self):
-        with self.tstcon.cursor(scrollable = True) as c:
-            with self.assertRaises(ProgrammingError):
-                c.next()
-
-if __name__ == '__main__':
-    unittest.TestLoader.sortTestMethodsUsing = None
-    unittest.main()
+# Copyright (c) 2017 Mimer Information Technology
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+# See license for more details.
+
+import unittest
+import time
+import math
+import mimerpy
+
+from mimerpy.mimPyExceptions import *
+import db_config
+
+class TestScrollCursorMethods(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(self):
+        (self.syscon, self.tstcon) = db_config.setup()
+
+    @classmethod
+    def tearDownClass(self):
+        db_config.teardown(tstcon=self.tstcon, syscon=self.syscon)
+
+    def tearDown(self):
+        self.tstcon.rollback()
+
+########################################################################
+## Tests below
+########################################################################
+
+    def test_createTable(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob(c1 INTEGER, c2 NVARCHAR(10)) in pybank")
+
+    def test_createTable_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobcr1(c1 INTEGER, c2 NVARCHAR(10))")
+            c.execute("create table bobcr2(c1 INTEGER, c2 NVARCHAR(10))")
+            c.execute("create table bobcr3(c1 INTEGER, c2 NVARCHAR(10))")
+            c.execute("create table bobcr4(c1 INTEGER, c2 NVARCHAR(10))")
+
+    def test_createTable_DropTable(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob2(c1 INTEGER, c2 NVARCHAR(10))")
+            c.execute("drop table bob2 CASCADE")
+
+    def test_create_invalid_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon (c1 INTEGER, c2 INTEGER) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("banana INTO jon VALUES (3, 14)")
+
+    def test_create_rollback_table(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonnynothere (c1 INTEGER, c2 INTEGER)")
+            self.tstcon.rollback()
+            c.execute("select * from jonnynothere")
+
+    def test_two_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonny (c1 INTEGER, c2 INTEGER) in pybank")
+            c.execute("select c1 from jonny where c1 = (?)",(2))
+            c.execute("select * from jonny")
+
+    def test_many_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob356 (c1 INTEGER) in pybank")
+            for val in range(100):
+                c.execute("insert into bob356 values (:a)", (val))
+            for gal in range(100):
+                c.execute("select c1 from bob356 where c1 > (?)",(gal))
+                temp = c.fetchall()
+                self.assertEqual(len(temp), 99 - gal)
+
+    def test_select_no_commit(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobc (c1 INTEGER, c2 FLOAT) in pybank")
+            for val in range(100):
+                c.execute("insert into bobc values (:a, :b)", (val, val + 0.5))
+            c.execute("select * from bobc where c1 = 99")
+            self.assertEqual(c.fetchall(),[(99,99.5)])
+
+    def test_select_description(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table description (columnone INTEGER) in pybank")
+            for val in range(10):
+                c.execute("insert into description values (?)", val)
+            c.execute("select * from description")
+            self.assertEqual(c.description,
+                             (('columnone', 50, None, None, None, None, None),))
+
+    def test_select_description2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table description2 (c1 INTEGER, c2 FLOAT)")
+            for val in range(10):
+                c.execute("insert into description2 values (?,?)", (val, val/3))
+            c.execute("select * from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),
+                              ('c2', 56, None, None, None, None, None)))
+            c.execute("select c1 from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),))
+            c.execute("select c2 from description2")
+            self.assertEqual(c.description,
+                             (('c2', 56, None, None, None, None, None),))
+            c.execute("select * from description2")
+            self.assertEqual(c.description,
+                             (('c1', 50, None, None, None, None, None),
+                              ('c2', 56, None, None, None, None, None)))
+
+    def test_select_description3(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table description3 (price INTEGER,"
+                      "                           currentval FLOAT,"
+                      "                           currency NVARCHAR(128),"
+                      "                           rate BIGINT,"
+                      "                           currentyear INTEGER)")
+            for val in range(10):
+                c.execute("insert into description3 values (?,?,?,?,?)",
+                          (val, val/3, 'SEK', 2**61, val+2000))
+            c.execute("select * from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentval', 56, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None)))
+            c.execute("select price, currentyear, currency, rate"
+                      "  from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None)))
+            c.execute("select rate, rate, rate, rate from description3")
+            self.assertEqual(c.description,
+                             (('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None)))
+            c.execute("select * from description3")
+            self.assertEqual(c.description,
+                             (('price', 50, None, None, None, None, None),
+                              ('currentval', 56, None, None, None, None, None),
+                              ('currency', 63, None, None, None, None, None),
+                              ('rate', 52, None, None, None, None, None),
+                              ('currentyear', 50, None, None, None, None, None)))
+
+    def test_select_description4(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            name1 = "e"*127+"q"
+            name2 = "m"*127+"q"
+            query = ("create table description4 (" + name1 + " INTEGER, "
+                     + name2 + " BOOLEAN) in pybank")
+            c.execute(query)
+            for val in range(10):
+                c.execute("insert into description4 values (?,?)", (val,val%2))
+            c.execute("select * from description4")
+            self.assertEqual(c.description,
+                             ((name1, 50, None, None, None, None, None),
+                              (name2, 42, None, None, None, None, None)))
+
+    def test_select_description5(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            name1 = "e"*127+"q"
+            name2 = "m"*127+"q"
+            query = ("create table description5 (" + name1 + " INTEGER, "
+                     + name2 + " BOOLEAN) in pybank")
+            c.execute(query)
+            for val in range(10):
+                c.execute("insert into description5 values (?,?)", (val,val%2))
+            c.execute("select * from description5")
+            self.assertEqual(c.description,
+                             ((name1, 50, None, None, None, None, None),
+                              (name2, 42, None, None, None, None, None)))
+
+    def test_invalid_create(self):
+        b = self.tstcon.cursor(scrollable = True)
+        b.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("creat table jon(i integer)")
+
+    def test_insert_parametermarkers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob1 (c1 INTEGER,  c2 NVARCHAR(10))")
+            c.execute("insert into bob1 values (:a, :b)", (3, 'bob'))
+
+    def test_insert_parametermarkers_long_string(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobstring (c1 INTEGER,  c2 NVARCHAR(256))")
+            string = "mimer" * 40
+            c.execute("insert into bobstring values (:a, :b)", (3, string))
+            self.tstcon.commit()
+            c.execute("select c2 from bobstring")
+            r = c.fetchall()
+            self.assertEqual(r, [(string,)])
+
+    def test_insert_parametermarkers_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob13 (c1 INTEGER, c2 NVARCHAR(10),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob13 values (:a, :b, :c)",
+                          ((1,'pi',14.345),
+                           (2,'pii',14.345),
+                           (-3,'piii',14.345),
+                           (7,'piii',14.345),
+                           (1121231,'piiii',14.345)))
+            self.tstcon.commit()
+            c.execute("select * from bob13")
+            r = c.fetchall()
+            self.assertEqual(r, [(1, 'pi', 14.345),
+                                 (2, 'pii', 14.345),
+                                 (-3, 'piii', 14.345),
+                                 (7, 'piii', 14.345),
+                                 (1121231, 'piiii', 14.345)])
+
+    def test_insert_parametermarkers_russian(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob14 (c1 INTEGER, c2 NVARCHAR(128),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into bob14 values (:a, :b, :c)",
+                          ((1,'продиктованной ангелом',14.345),
+                           (2,'安排他們參',14.345)))
+            self.tstcon.commit()
+            c.execute("select * from bob14")
+            self.assertEqual(c.fetchall(),
+                             [(1,'продиктованной ангелом',14.345),
+                              (2,'安排他們參',14.345)])
+
+    def test_insert_parametermarkers_unicode(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table boby14 (c1 INTEGER, c2 NVARCHAR(128),"
+                      "                     c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            c.executemany("insert into boby14 values (:a, :b, :c)",
+                          ((1,'продиктованной ангелом',14.345),
+                           (2,'安排他們參‱',14.345)))
+            self.tstcon.commit()
+            c.execute("select * from boby14")
+            self.assertEqual(c.fetchall(),
+                             [(1,'продиктованной ангелом',14.345),
+                              (2,'安排他們參‱',14.345)])
+
+    def test_insert_parametermarkers_too_long(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob15 (c1 NVARCHAR(10)) in pybank")
+            self.tstcon.commit()
+            with self.assertRaises(DatabaseError):
+                c.execute("insert into bob15 values (:a)",
+                          ('This sentence is too long'))
+        self.tstcon.commit()
+
+    def test_insert_too_few_parametermarkers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob3 (c1 INTEGER, c2 NVARCHAR(10))")
+            with self.assertRaises(DatabaseError):
+                c.execute("insert into bob3 values (:a, :b)", (3))
+
+    # &&&& Wrong exception. Fixme.
+    @unittest.skip
+    def test_insert_too_many_parametermarkers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob33 (c1 INTEGER, c2 NVARCHAR(10))")
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob33 values (:a, :b)",
+                              ((3,'pi',14), (3,)))
+
+    def test_insert_many_times(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob34(c1 INTEGER, c2 NVARCHAR(10),"
+                      "                   c3 FLOAT) in pybank")
+            for i in range(0, 101):
+                c.execute("insert into bob34 values (5,'ウィキペディ', 4.4543543)")
+        self.tstcon.commit()
+
+    def test_executemany_one_value(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob4 (c1 INTEGER) in pybank")
+            c.executemany("insert into bob4 values (:a)", [(1,)])
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob4 values (:a)", [(1)])
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob4 values (:a)", (1))
+            with self.assertRaises(ProgrammingError):
+                c.executemany("insert into bob4 values (:a)", [1])
+
+    def test_executemany_one_tuple(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob5 (c1 INTEGER, c2 NVARCHAR(10))")
+            c.executemany("insert into bob5 values (:a, :b)", ((1,'bob1'),))
+
+    def test_executemany_several_tuples(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobe6 (c1 INTEGER, c2 NVARCHAR(10))")
+            c.executemany("insert into bobe6 values (:a, :b)",
+                          [(1,'bob1'),
+                           (2, 'bob2'),
+                           (3,'bob3')])
+
+    def test_commit(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob7 (c1 INTEGER, c2 NVARCHAR(10))")
+            c.executemany("insert into bob7 values (:a, :b)",
+                          ((1,'bob1'),
+                           (2, 'bob2'),
+                           (3,'bob3')))
+        self.tstcon.commit()
+
+    def test_fetchone(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob8 (c1 INTEGER, c2 NVARCHAR(10))")
+
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("insert into bob8 values (:a, :b)", (8, 'bob'))
+            self.tstcon.commit()
+            c.execute("select * from bob8")
+            self.assertEqual(c.fetchone(), (8, 'bob'))
+
+    def test_fetchmany(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob9 (c1 INTEGER, c2 NVARCHAR(10))")
+
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.executemany("insert into bob9 values (:a, :b)",
+                          ((9, 'bob9'),
+                           (10, 'bob10'),
+                           (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob9")
+            self.assertEqual(c.fetchmany(3),
+                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
+
+    def test_fetchmany_too_many(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob11 (c1 INTEGER, c2 NVARCHAR(10))")
+            self.tstcon.commit()
+            c.executemany("insert into bob11 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob11")
+            self.assertEqual(c.fetchmany(5),
+                             [(9, 'bob9'), (10, 'bob10'), (11, 'bob11')])
+
+    def test_fetchmany_notall(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob12 (c1 INTEGER, c2 NVARCHAR(10))")
+            self.tstcon.commit()
+            c.executemany("insert into bob12 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob12")
+            self.assertEqual(c.fetchmany(2), [(9, 'bob9'), (10, 'bob10')])
+            self.assertEqual(c.fetchmany(2), [(11, 'bob11')])
+
+    def test_fetchall(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob10 (c1 INTEGER, c2 NVARCHAR(10))")
+            c.executemany("insert into bob10 values (:a, :b)",
+                          ((10, 'bob10'), (11, 'bob11'), (12, 'bob12'),))
+            self.tstcon.commit()
+            c.execute("select * from bob10")
+            self.assertEqual(c.fetchall(),
+                             [(10, 'bob10'),(11, 'bob11'), (12, 'bob12')])
+
+    def test_fetchall_correct_number_of_rows(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob101(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            for d in range(1, 101):
+                c.execute("insert into bob101 values (5,'ウィキペディ', 4.4543543)")
+            self.tstcon.commit()
+            c.execute("select * from bob101")
+            r = c.fetchall()
+            self.assertEqual(len(r), 100)
+
+    def test_fetchall_correct_number_of_rows2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob102(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+            self.tstcon.commit()
+            for i in range(1, 101):
+                c.execute("insert into bob102 values (5,'ウィキペディ',"
+                          " 4.4543543)")
+            self.tstcon.rollback()
+            c.execute("select * from bob102")
+            r = c.fetchall()
+            self.assertEqual(len(r), 0)
+
+    @unittest.skip
+    def test_fetchall_correct_number_of_rows3(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob109(c1 INTEGER, c2 NVARCHAR(100),"
+                      "                    c3 FLOAT) in pybank")
+            for i in range(1, 101):
+                c.execute("insert into bob109 values (5,'ウィキペディ',"
+                          " 4.4543543)")
+            self.tstcon.rollback()
+            c.execute("select * from bob109")
+            r = c.fetchall()
+            self.assertEqual(len(r), 0)
+
+    def test_use_next(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobnext(c1 INTEGER) in pybank")
+            for i in range(0, 10):
+                c.execute("insert into bobnext values (?)", i)
+            self.tstcon.commit()
+            c.execute("select * from bobnext")
+            for i in range(0,10):
+                (val,) = c.next()
+                self.assertEqual(val, i)
+
+    def test_use_next_StopIteration(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobstop(c1 INTEGER) in pybank")
+            for i in range(0, 10):
+                c.execute("insert into bobstop values (?)", i)
+            self.tstcon.commit()
+            c.execute("select * from bobstop")
+            for i in range(0,10):
+                c.next()
+            with self.assertRaises(StopIteration):
+                c.next()
+
+    def test_insert_wrong_type_parametermarkers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob1337 (c1 INTEGER, c2 INTEGER)")
+            with self.assertRaises(DataError):
+                c.execute("insert into bob1337  values (:a, :b)", (3, 3.14))
+
+    def test_operate_after_closed(self):
+        b = self.tstcon.cursor(scrollable = True)
+        b.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("select * from jon")
+
+    def test_operate_after_closed_2(self):
+        b = self.tstcon.cursor(scrollable = True)
+        b.close()
+        b.close()
+        with self.assertRaises(ProgrammingError):
+            b.execute("Kalle")
+        with self.assertRaises(ProgrammingError):
+            b.executemany("Kalle", ("Kula"))
+        with self.assertRaises(ProgrammingError):
+            b.fetchone()
+        with self.assertRaises(ProgrammingError):
+            b.fetchmany("Kalle")
+        with self.assertRaises(ProgrammingError):
+            b.fetchall()
+        with self.assertRaises(ProgrammingError):
+            b.next()
+
+    def test_invalid_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            with self.assertRaises(ProgrammingError):
+                c.execute("select * from jonisnotatablejo where c1 = ?", (5))
+
+    def test_same_table_twice(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob2437(c1 INTEGER) in pybank")
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob2437(c1 INTEGER) in pybank")
+
+    def test_invalid_sequence_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob6565(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("select * from bob6565")
+            r = c.fetchone()
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob6569(c1 INTEGER) in pybank")
+            self.tstcon.rollback()
+
+    #borde bli fel men blir rätt....
+    def test_invalid_sequence_select_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob555(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("select * from bob555")
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob556(c1 INTEGER) in pybank")
+            self.tstcon.rollback()
+            c.execute("create table bob556(c1 INTEGER) in pybank")
+            c.execute("insert into bob556 values (3)")
+            c.execute("select * from bob556")
+            self.assertEqual(c.fetchone(), (3,))
+
+    def test_invalid_sequence_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob6567(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bob6567 values (3)")
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob6566(c1 INTEGER) in pybank")
+            self.tstcon.rollback()
+
+    def test_invalid_sequence_insert_parametermarkers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob6568(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bob6568 values (?)", (3))
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bob6566(c1 INTEGER) in pybank")
+            self.tstcon.rollback()
+
+    def test_executemany_DDL(self):
+        with self.assertRaises(ProgrammingError):
+            c = self.tstcon.executemany("create table bob6(c1 INTEGER)", (3))
+        with self.tstcon.cursor(scrollable = True) as c:
+            with self.assertRaises(ProgrammingError):
+                c.execute("select * from bob6")
+
+    def test_insert_exceeded(self):
+        c = self.tstcon.execute("create table bob16(c1 INTEGER) in pybank")
+        big = pow(2,100)
+        with self.assertRaises(DataError):
+            c.execute("insert into bob16 values (?)", big)
+
+    def test_insert_too_long(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob17(c1 NVARCHAR(10)) in pybank")
+            self.tstcon.commit()
+            with self.assertRaises(DataError):
+                c.execute("insert into bob17 values ('ウィキペデBobWasABoy')")
+            self.tstcon.commit()
+
+    def test_valid_int32_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon32 (c1 INTEGER, c2 INTEGER) in pybank")
+            nvar = -2**31
+            var = 2**31 - 1
+            c.execute("insert INTO jon32 VALUES (?, ?)", (nvar, var))
+
+    def test_invalid_int32_insert_too_small(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon31 (c1 INTEGER) in pybank")
+            nvar = -2**31 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon31 VALUES (?)", (nvar))
+
+    def test_invalid_int32_insert_too_big(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon33 (c1 INTEGER) in pybank")
+            var = 2**31
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon33 VALUES (?)", (var))
+
+    def test_valid_int64_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon64 (c1 BIGINT, c2 BIGINT) in pybank")
+            nvar = -2**63
+            var = 2**63 - 1
+            c.execute("insert INTO jon64 VALUES (?,?)", (nvar,var))
+
+    def test_overflow_int64_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table intjon4 (c1 BIGINT, c2 BIGINT) in pybank")
+            nvar = -2**633
+            var = 2**63 - 1
+            with self.assertRaises(DataError):
+                c.executemany("insert INTO intjon4 VALUES (?,?)",
+                              ((nvar,var),(nvar,var)))
+
+    def test_invalid_int64_insert_too_small(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon63 (c1 BIGINT) in pybank")
+            nvar = -2**63 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon63 VALUES (?)", (nvar))
+
+    def test_invalid_int64_insert_too_big(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon65 (c1 BIGINT) in pybank")
+            var = 2**63
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon65 VALUES (?)", (var))
+
+    def test_valid_int16_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon26 (c1 SMALLINT, c2 SMALLINT)")
+            nvar = -2**15
+            var = 2**15 - 1
+            c.execute("insert INTO jon26 VALUES (?, ?)", (nvar, var))
+
+    def test_invalid_int16_insert_too_small(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon15 (c1 SMALLINT) in pybank")
+            nvar = -2**15 - 1
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon15 VALUES (?)", (nvar))
+
+    def test_invalid_int16_insert_too_small(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon17 (c1 SMALLINT) in pybank")
+            nvar = 2**15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jon17 VALUES (?)", (nvar))
+
+    # &&&& Gives a Warning we dont catch atm
+    def test_valid_double_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon16 (c1 REAL, c2 DOUBLE PRECISION)")
+            var = 2/3
+            c.execute("insert INTO jon16 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+
+    def test_valid_double_insert_none(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon18 (c1 REAL, c2 DOUBLE PRECISION)")
+            var = None
+            c.execute("insert INTO jon18 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+
+    def test_valid_double_select_none(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jon19 (c1 REAL, c2 DOUBLE PRECISION)")
+            var = None
+            c.execute("insert INTO jon19 VALUES (?, ?)", (var, var))
+            self.tstcon.commit()
+            c.execute("select * from jon19")
+            self.assertEqual(c.fetchall(), [(None, None)])
+
+    def test_message_cleared(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonwas17 (c1 SMALLINT) in pybank")
+            nvar = 2**15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jonwas17 VALUES (?)", (nvar))
+            c.execute("insert INTO jonwas17 VALUES (?)", (5))
+            self.assertEqual(c.messages, [])
+
+    def test_message_cleared_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonwas173 (c1 SMALLINT) in pybank")
+            nvar = 2**15
+            with self.assertRaises(DataError):
+                c.execute("insert INTO jonwas173 VALUES (?)", (nvar))
+            self.assertEqual(c.messages[0][1],
+                             (-24010,
+                              'Value was too large to fit in destination'))
+
+    def test_None_is_returned(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonNone (c1 INTEGER) in pybank")
+            for i in range(1,10):
+                c.execute("Insert INTO jonNone VALUES (?)", (i,))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonNone")
+            for i in range(1,10):
+                c.fetchone()
+            self.assertEqual(c.fetchone(), [])
+
+    def test_empty_sequence_is_returned_many(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonEmpty (c1 INTEGER) in pybank")
+            for i in range(1,10):
+                c.execute("Insert INTO jonEmpty VALUES (?)", (i))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonEmpty")
+            c.fetchmany(10)
+            self.assertEqual(c.fetchmany(10), [])
+
+    def test_empty_sequence_is_returned_all(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonEmpty2 (c1 INTEGER) in pybank")
+            for i in range(1,10):
+                c.execute("Insert INTO jonEmpty2 VALUES (?)", (i))
+            self.tstcon.commit()
+            c.execute("SELECT * from jonEmpty2")
+            c.fetchall()
+            self.assertEqual(c.fetchall(), [])
+
+    def test_empty_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonEmp (c1 NVARCHAR(128)) in pybank")
+            c.executemany("Insert INTO jonEmp VALUES (?)",
+                          (('',),("",),(" ",)))
+            self.tstcon.commit()
+            c.execute("select * from jonEmp")
+            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
+
+    def test_empty_insert2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonEmp2 (c1 NVARCHAR(128)) in pybank")
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (''))
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (""))
+            c.execute("Insert INTO jonEmp2 VALUES (?)", (" "))
+            self.tstcon.commit()
+            c.execute("select * from jonEmp2")
+            self.assertEqual(c.fetchall(), [('',), ('',), (' ',)])
+
+    def test_invalid_databank(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            with self.assertRaises(ProgrammingError):
+                c.execute("create table bjonEmp2 (c1 NVARCHAR(128)) in potato")
+
+    def test_insert_rowcount_update(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrowcount(c1 INTEGER, c2 NVARCHAR(256))")
+            string = "mimer"
+            c.execute("insert into bobrowcount values (:a, :b)", (3, string))
+            self.assertEqual(c.rowcount, 1)
+            c.executemany("insert into bobrowcount values (:a, :b)",
+                          ((5,string),(2,string)))
+            # self.assertEqual(c.rowcount, 2) # &&&& Should we set rowcount????
+            c.execute("select * from bobrowcount")
+            r = c.fetchall()
+            self.assertEqual(c.rowcount, 3)
+
+    def test_delete(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrowcount2(c1 INTEGER) in pybank")
+            for i in range(1,11):
+                c.execute("INSERT into bobrowcount2 values (?)", 10)
+                c.execute("INSERT into bobrowcount2 values (?)", 20)
+            c.execute("INSERT into bobrowcount2 values (?)", 10)
+            c.execute("SELECT * from bobrowcount2")
+            self.assertEqual(len(c.fetchall()), 21)
+            c.execute("DELETE from bobrowcount2 where c1 = 10")
+            self.assertEqual(c.rowcount, 11)
+            c.execute("SELECT * from bobrowcount2")
+            self.assertEqual(len(c.fetchall()), 10)
+
+    def test_update(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobupdate(c1 INTEGER) in pybank")
+            for i in range(1,11):
+                c.execute("INSERT into bobupdate values (?)", 10)
+                c.execute("INSERT into bobupdate values (?)", 20)
+            c.execute("INSERT into bobupdate values (?)", 10)
+            c.execute("SELECT * from bobupdate")
+            self.assertEqual(len(c.fetchall()), 21)
+            c.execute("UPDATE bobupdate SET c1 = ? WHERE c1 = 20", 30)
+            self.assertEqual(c.rowcount, 10)
+            c.execute("SELECT * from bobupdate")
+            self.assertEqual(len(c.fetchall()), 21)
+
+    def test_invalid_sequence_fetchone(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonfetchone (c1 INTEGER) in pybank")
+            for i in range(1,10):
+                c.execute("Insert INTO jonfetchone VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchone()
+
+    def test_isolated(self):
+        c1 = self.tstcon.cursor()
+        c2 = self.tstcon.cursor()
+        c1.execute("create table jonisolated (c1 INTEGER) in pybank")
+        for i in range(1,6):
+            c1.execute("Insert INTO jonisolated VALUES (?)", (i))
+        c2.execute("SELECT * FROM jonisolated")
+        r2 = c2.fetchall()
+        self.assertEqual(len(r2), 5)
+        self.assertEqual(r2, [(1,),(2,),(3,),(4,),(5,),])
+
+    def test_invalid_sequence_fetchmany(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonfetchmany (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonfetchmany VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchmany(10)
+
+    def test_invalid_sequence_fetchall(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonfetchall (c1 INTEGER) in pybank")
+            for i in range(1, 10):
+                c.execute("Insert INTO jonfetchall VALUES (?)", (i))
+            self.tstcon.commit()
+            with self.assertRaises(ProgrammingError):
+                c.fetchall()
+
+    @unittest.skip
+    # &&&& need to find a picture to put in the repo
+    # Nä, gör en psudorandom-blob
+    def test_insert_blob(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonblob (c1 BLOB(18389)) in pybank")
+            with open("../minikappa.jpg", 'rb') as input_file:
+                ablob = input_file.read()
+                c.execute("insert INTO jonblob VALUES (?)", (ablob))
+                self.tstcon.commit()
+                c.execute("select * from jonblob")
+                r = b.fetchall()[0]
+                self.assertEqual(r[0], ablob)
+
+    @unittest.skip
+    # &&&& need to find a picture to put in the repo
+    # Nä, gör en psudorandom-blob
+    def test_insert_blob_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonblob2 (c1 BLOB(64111)) in pybank")
+            with open("../mimerss.png", 'rb') as input_file:
+                ablob = input_file.read()
+                c.execute("insert INTO jonblob2 VALUES (?)", (ablob))
+                self.tstcon.commit()
+                c.execute("select * from jonblob2")
+                r = c.fetchall()[0]
+                self.assertEqual(r[0], ablob)
+
+    @unittest.skip
+    # &&&& need to find a picture to put in the repo
+    # Nä, gör en psudorandom-blob
+    def test_insert_blob_3(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonblob3 (c1 BLOB(3000000)) in pybank")
+            with open("../mimerd.jpg", 'rb') as input_file:
+                ablob = input_file.read()
+                c.execute("insert INTO jonblob3 VALUES (?)", (ablob))
+                self.tstcon.commit()
+                c.execute("select * from jonblob3")
+                r = c.fetchall()[0][0]
+            self.assertEqual(r, ablob)
+
+    @unittest.skip
+    # &&&& need to find a picture to put in the repo
+    # Nä, gör en psudorandom-blob
+    def test_insert_blob_4(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonblob4 (c1 BLOB(3000000)) in pybank")
+            with open("../kappa.jpg", 'rb') as input_file:
+                ablob = input_file.read()
+                c.execute("insert INTO jonblob4 VALUES (?)", (ablob))
+                self.tstcon.commit()
+                c.execute("select * from jonblob4")
+                r = c.fetchall()[0][0]
+            self.assertEqual(r, ablob)
+
+    def test_insert_nclob(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonnclob (c1 NCLOB(50000)) in pybank")
+            anclob = "mimer" * 1000
+            c.execute("insert INTO jonnclob VALUES (?)", (anclob))
+            self.tstcon.commit()
+            c.execute("select * from jonnclob")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], anclob)
+
+    def test_insert_binary(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonbinary (c1 BINARY(3)) in pybank")
+            c.execute("insert INTO jonbinary VALUES (x'ABCD01')")
+            c.execute("insert INTO jonbinary VALUES (?)", (b'A01'))
+            self.tstcon.commit()
+            c.execute("select * from jonbinary")
+            r = c.fetchall()
+            self.assertEqual(r, [(b'\xab\xcd\x01',), (b'A01',)])
+
+    def test_insert_binary_parameter_markers(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonbinary2 (c1 BINARY(2)) in pybank")
+            bob = b'\xab\xcd'
+            c.execute("insert INTO jonbinary2 VALUES (?)", (bob))
+            self.tstcon.commit()
+            c.execute("select * from jonbinary2")
+            (r,) = c.fetchall()[0]
+            self.assertEqual(r, bob)
+
+    @unittest.skip
+    def test_insert_nclob_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonnclob2 (c1 Nclob(450000)) in pybank")
+            with open("../book2.txt", "r") as input_file:
+                anclob = input_file.read()
+                c.execute("insert INTO jonnclob2 VALUES (?)", (anclob))
+                self.tstcon.commit()
+                c.execute("select * from jonnclob2")
+                r = c.fetchall()[0]
+                self.assertEqual(r[0], anclob)
+
+    def test_insert_clob(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table jonclob (c1 clob(30000)) in pybank")
+            anclob = "mimer" * 5
+            c.execute("insert INTO jonclob VALUES (?)", (anclob))
+            self.tstcon.commit()
+            c.execute("select * from jonclob")
+            r = c.fetchall()[0]
+            self.assertEqual(r[0], anclob)
+
+    def test_insert_bool(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobybool (c1 boolean) in pybank")
+            c.execute("insert INTO bobybool VALUES (?)", (False))
+            c.execute("insert INTO bobybool VALUES (?)", (True))
+            c.execute("insert INTO bobybool VALUES (?)", (None))
+            c.execute("insert INTO bobybool VALUES (?)", (45))
+            self.tstcon.commit()
+
+    def test_select_bool(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobybool2 (c1 boolean) in pybank")
+            c.execute("insert INTO bobybool2 VALUES (?)", (False))
+            c.execute("insert INTO bobybool2 VALUES (?)", (True))
+            c.execute("insert INTO bobybool2 VALUES (?)", (None))
+            c.execute("insert INTO bobybool2 VALUES (?)", (45))
+            self.tstcon.commit()
+            c.execute("select * from bobybool2")
+            r = c.fetchone()
+            self.assertEqual(r[0], False)
+            r = c.fetchone()
+            self.assertEqual(r[0], True)
+            r = c.fetchone()
+            self.assertEqual(r[0], None)
+            r = c.fetchone()
+            self.assertEqual(r[0], True)
+
+    def test_get_connection(self):
+        b = self.tstcon.cursor(scrollable = True)
+        self.assertEqual(b.connection, self.tstcon)
+        b.close()
+
+    def test_for(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table fortable (c1 INTEGER) in pybank")
+            c.execute("insert INTO fortable VALUES (?)", (45))
+            c.execute("select * from fortable")
+            for val in c:
+                self.assertEqual(val[0], 45)
+
+    def test_result_set_twice(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table kor (c1 INTEGER) in pybank")
+            c.execute("insert INTO kor VALUES (?)", (45))
+            c.execute("select * from kor")
+            for val in c:
+                self.assertEqual(val[0], 45)
+            c.execute("select * from kor")
+            for val in c:
+                self.assertEqual(val[0], 45)
+            c.execute("select c1 from kor")
+            for val in c:
+                self.assertEqual(val[0], 45)
+
+    def test_executemany_none(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table manytable (c1 INTEGER) in pybank")
+            c.executemany("insert INTO manytable VALUES (?)",
+                          [(2,),(34,),(435,),(34,),(63,),(47,),(None,)])
+            self.tstcon.commit()
+
+    def test_select_executemany(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobyselect (c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            c.execute("insert INTO bobyselect VALUES (?)", (1))
+            with self.assertRaises(ProgrammingError):
+                c.executemany("select * from bobyselect where c1 = (?)",
+                              ((5,),(10,)))
+
+    def test_select_twice(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bananaselect (c1 INTEGER) in pybank")
+            c.execute("select * from bananaselect where c1 = (?)", (5))
+            c.execute("select c1 from bananaselect where c1 = (?)", (7))
+
+    def test_fetchall_no_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            with self.assertRaises(ProgrammingError):
+                c.fetchone()
+            with self.assertRaises(ProgrammingError):
+                c.fetchmany()
+            with self.assertRaises(ProgrammingError):
+                c.fetchall()
+
+    def test_bool_insert(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table boolt (c1 BOOLEAN) in pybank")
+            c.executemany("insert into boolt values (?)",
+                          [(None,), (1,), (0,), (3.1415,),
+                           ("potato",), ('code',)])
+            c.execute("select * from boolt")
+
+    def test_insert_parametermarkers_different_types(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob176(c1 NVARCHAR(128)) in pybank")
+            c.execute("INSERT INTO bob176 VALUES (?)", "bar")    # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ("bar"))  # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ("bar",)) # correct
+            c.execute("INSERT INTO bob176 VALUES (?)", ["bar"])  # correct
+            self.tstcon.commit()
+            c.execute("select * from bob176")
+            self.assertEqual(c.fetchall(),
+                             [("bar",),("bar",),("bar",),("bar",)])
+
+    def test_insert_bigint(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobbig17(c1 BIGINT) in pybank")
+            self.tstcon.commit()
+            c.execute("insert into bobbig17 values (234)")
+            self.tstcon.commit()
+
+    @unittest.skip
+    def test_help(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            help(c)
+
+    #ScrollCursor specific tests
+
+    def test_fetchone_2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bob853 (c1 INTEGER, c2 NVARCHAR(10))")
+            self.tstcon.commit()
+            c.executemany("insert into bob853 values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bob853")
+            self.assertEqual(c.fetchone(), (9, 'bob9'))
+            self.assertEqual(c.fetchone(), (10, 'bob10'))
+            self.assertEqual(c.fetchone(), (11, 'bob11'))
+            self.assertEqual(c.fetchone(), [])
+
+    def test_fetchone_rownumber(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow (c1 INTEGER, c2 NVARCHAR(10))")
+            c.executemany("insert into bobrow values (:a, :b)",
+                          ((9, 'bob9'), (10, 'bob10'), (11, 'bob11')))
+            self.tstcon.commit()
+            c.execute("select * from bobrow")
+            self.assertEqual(c.rownumber, 0)
+            self.assertEqual(c.fetchone(), (9, 'bob9'))
+            self.assertEqual(c.rownumber, 1)
+            self.assertEqual(c.fetchone(), (10, 'bob10'))
+            self.assertEqual(c.rownumber, 2)
+            self.assertEqual(c.fetchone(), (11, 'bob11'))
+            self.assertEqual(c.rownumber, 3)
+            self.assertEqual(c.fetchone(), [])
+            self.assertEqual(c.rownumber, 3)
+
+    def test_fetchmany_rownumber(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow2(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 11):
+                c.execute("insert into bobrow2 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow2")
+            self.assertEqual(c.rownumber, 0)
+            self.assertEqual(c.fetchmany(3),
+                             [(1, 'bob1'),(2, 'bob2'),(3, 'bob3')])
+            self.assertEqual(c.rownumber, 3)
+            self.assertEqual(c.fetchmany(3),
+                             [(4, 'bob4'),(5, 'bob5'),(6, 'bob6')])
+            self.assertEqual(c.rownumber, 6)
+            self.assertEqual(c.fetchmany(10),
+                             [(7, 'bob7'),(8, 'bob8'),(9, 'bob9'),(10, 'bob10')])
+            self.assertEqual(c.rownumber, 10)
+            self.assertEqual(c.fetchmany(2), [])
+
+    def test_fetchall_rownumber(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow3(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 6):
+                c.execute("insert into bobrow3 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow3")
+            self.assertEqual(c.rownumber, 0)
+            self.assertEqual(c.fetchall(),
+                             [(1, 'bob1'),(2, 'bob2'),(3, 'bob3'),
+                              (4, 'bob4'),(5, 'bob5')])
+            self.assertEqual(c.rownumber, 5)
+            self.assertEqual(c.fetchall(), [])
+
+    def test_mixfetch_rownumber(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow4(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 11):
+                c.execute("insert into bobrow4 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow4")
+            self.assertEqual(c.rownumber, 0)
+            self.assertEqual(c.fetchone(), (1, 'bob1'))
+            self.assertEqual(c.rownumber, 1)
+            self.assertEqual(c.fetchmany(3),
+                             [(2, 'bob2'),(3, 'bob3'), (4, 'bob4')])
+            self.assertEqual(c.rownumber, 4)
+            self.assertEqual(c.fetchone(), (5, 'bob5'))
+            self.assertEqual(c.rownumber, 5)
+            self.assertEqual(c.fetchall(),
+                             [(6, 'bob6'),(7, 'bob7'),(8, 'bob8'),
+                              (9, 'bob9'),(10, 'bob10')])
+            self.assertEqual(c.rownumber, 10)
+            self.assertEqual(c.fetchone(), [])
+            self.assertEqual(c.fetchmany(21), [])
+            self.assertEqual(c.fetchall(), [])
+
+    def test_mixfetch_rowcount(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow5(c1 INTEGER) in pybank")
+            for i in range(1, 101):
+                c.execute("insert into bobrow5 values (?)", (i))
+            self.tstcon.commit()
+            c.execute("select * from bobrow5")
+            self.assertEqual(c.rowcount, 100)
+            c.execute("select c1 from bobrow5 where c1 >= ?", (50))
+            self.assertEqual(c.rowcount, 51)
+            c.execute("select c1 from bobrow5 where c1 < ?", (10))
+            self.assertEqual(c.rowcount, 9)
+
+    def test_scroll(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow6(c1 INTEGER) in pybank")
+            for i in range(1, 101):
+                c.execute("insert into bobrow6 values (?)", (i))
+            self.tstcon.commit()
+            c.execute("select * from bobrow6")
+            c.scroll(2,mode='relative')
+            self.assertEqual(c.rownumber, 2)
+            self.assertEqual(c.fetchone(), (3,))
+            c.scroll(3,mode='relative')
+            self.assertEqual(c.rownumber, 6)
+            self.assertEqual(c.fetchone(), (7,))
+            c.scroll(3,mode='absolute')
+            self.assertEqual(c.rownumber, 3)
+            c.scroll(5,mode='relative')
+            self.assertEqual(c.rownumber, 8)
+
+    def test_scroll_error(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow7(c1 INTEGER) in pybank")
+            for i in range(1, 101):
+                c.execute("insert into bobrow7 values (?)", (i))
+            self.tstcon.commit()
+            c.execute("select * from bobrow7")
+            with self.assertRaises(ProgrammingError):
+                c.scroll(5,mode='nonexistingmode')
+            with self.assertRaises(IndexError):
+                c.scroll(101,mode='absolute')
+
+    def test_next(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow8(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 11):
+                c.execute("insert into bobrow8 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow8")
+            self.assertEqual(c.next(), (1, 'bob1'),)
+            c.scroll(5,mode='relative')
+            self.assertEqual(c.next(), (7, 'bob7'),)
+            c.scroll(9, mode='absolute')
+
+    def test_next_fetch(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow10(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 11):
+                c.execute("insert into bobrow10 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow10")
+            self.assertEqual(c.fetchone(), (1, 'bob1'),)
+            self.assertEqual(c.next(), (2, 'bob2'),)
+            self.assertEqual(c.fetchmany(2), [(3, 'bob3'), (4, 'bob4')])
+            self.assertEqual(c.next(), (5, 'bob5'),)
+            c.scroll(1, mode='relative')
+            self.assertEqual(c.fetchall(),
+                             [(7, 'bob7'), (8, 'bob8'),
+                              (9, 'bob9'), (10, 'bob10')])
+
+    def test_next_error(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobrow9(c1 INTEGER, c2 NVARCHAR(100))")
+            for i in range(1, 11):
+                c.execute("insert into bobrow9 values (:a, :b)",
+                          (i, 'bob' + str(i) ))
+            self.tstcon.commit()
+            c.execute("select * from bobrow9")
+            c.scroll(9, mode='absolute')
+            with self.assertRaises(StopIteration):
+                c.next()
+                c.next()
+
+    def test_fetchall_IndexError(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table indexerror (c1 INTEGER) in pybank")
+            for val in range(0,10):
+                c.execute("insert INTO indexerror VALUES (?)", (val))
+            c.execute("select * from indexerror")
+            r = c.fetchmany(9)
+            r = c.fetchall()
+
+    def test_fetchall_Scroll_outside(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table scrolloutside (c1 INTEGER) in pybank")
+            for val in range(0,10):
+                c.execute("insert INTO scrolloutside VALUES (?)", (val))
+            c.execute("select * from scrolloutside")
+            with self.assertRaises(IndexError):
+                r = c.scroll(100)
+
+    def test_no_select(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobnoselect(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            for i in range(1, 11):
+                c.execute("insert into bobnoselect values (5)")
+            self.tstcon.rollback()
+            c.execute("select * from bobnoselect")
+            r = c.fetchone()
+            self.assertEqual(len(r), 0)
+
+    def test_no_select2(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobnoselect2(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            for i in range(1, 11):
+                c.execute("insert into bobnoselect2 values (5)")
+            self.tstcon.rollback()
+            c.execute("select * from bobnoselect2")
+            r = c.fetchmany(5)
+            self.assertEqual(len(r), 0)
+
+    def test_no_select3(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            c.execute("create table bobnoselect3(c1 INTEGER) in pybank")
+            self.tstcon.commit()
+            for i in range(1, 11):
+                c.execute("insert into bobnoselect3 values (5)")
+            self.tstcon.rollback()
+            c.execute("select * from bobnoselect3")
+            r = c.next()
+            self.assertEqual(len(r), 0)
+
+    def test_next_noselect(self):
+        with self.tstcon.cursor(scrollable = True) as c:
+            with self.assertRaises(ProgrammingError):
+                c.next()
+
+if __name__ == '__main__':
+    unittest.TestLoader.sortTestMethodsUsing = None
+    unittest.main()
```

