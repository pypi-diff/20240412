# Comparing `tmp/python_colored_print-1.0.0rc1.tar.gz` & `tmp/python_colored_print-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python_colored_print-1.0.0rc1.tar", last modified: Sat May  8 10:33:00 2021, max compression
+gzip compressed data, was "python_colored_print-1.1.0.tar", last modified: Fri Apr 12 09:51:55 2024, max compression
```

## Comparing `python_colored_print-1.0.0rc1.tar` & `python_colored_print-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 agn       (1000) agn       (1000)        0 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/
--rw-rw-r--   0 agn       (1000) agn       (1000)     1964 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/PKG-INFO
--rw-rw-r--   0 agn       (1000) agn       (1000)      981 2021-05-08 10:10:36.000000 python_colored_print-1.0.0rc1/setup.py
-drwxrwxr-x   0 agn       (1000) agn       (1000)        0 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/colored_print/
--rw-rw-r--   0 agn       (1000) agn       (1000)     1530 2021-05-08 06:00:20.000000 python_colored_print-1.0.0rc1/colored_print/colored_print.py
--rw-rw-r--   0 agn       (1000) agn       (1000)      133 2021-05-08 10:10:33.000000 python_colored_print-1.0.0rc1/colored_print/__init__.py
--rw-rw-r--   0 agn       (1000) agn       (1000)     1049 2021-05-08 10:04:08.000000 python_colored_print-1.0.0rc1/README.rst
-drwxrwxr-x   0 agn       (1000) agn       (1000)        0 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/python_colored_print.egg-info/
--rw-rw-r--   0 agn       (1000) agn       (1000)     1964 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/python_colored_print.egg-info/PKG-INFO
--rw-rw-r--   0 agn       (1000) agn       (1000)        1 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/python_colored_print.egg-info/dependency_links.txt
--rw-rw-r--   0 agn       (1000) agn       (1000)       14 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/python_colored_print.egg-info/top_level.txt
--rw-rw-r--   0 agn       (1000) agn       (1000)      262 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/python_colored_print.egg-info/SOURCES.txt
--rw-rw-r--   0 agn       (1000) agn       (1000)       80 2021-05-08 10:33:00.000000 python_colored_print-1.0.0rc1/setup.cfg
+drwxrwxr-x   0 benyamin  (1000) benyamin  (1000)        0 2024-04-12 09:51:55.177028 python_colored_print-1.1.0/
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)     1072 2022-07-23 06:22:51.000000 python_colored_print-1.1.0/LICENSE
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)     1603 2024-04-12 09:51:55.177028 python_colored_print-1.1.0/PKG-INFO
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)     1108 2024-01-06 13:53:22.000000 python_colored_print-1.1.0/README.rst
+drwxrwxr-x   0 benyamin  (1000) benyamin  (1000)        0 2024-04-12 09:51:55.177028 python_colored_print-1.1.0/colored_print/
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)      120 2024-04-12 09:19:33.000000 python_colored_print-1.1.0/colored_print/__init__.py
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)     2353 2024-04-12 09:20:35.000000 python_colored_print-1.1.0/colored_print/colored_print.py
+drwxrwxr-x   0 benyamin  (1000) benyamin  (1000)        0 2024-04-12 09:51:55.177028 python_colored_print-1.1.0/python_colored_print.egg-info/
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)     1603 2024-04-12 09:51:55.000000 python_colored_print-1.1.0/python_colored_print.egg-info/PKG-INFO
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)      270 2024-04-12 09:51:55.000000 python_colored_print-1.1.0/python_colored_print.egg-info/SOURCES.txt
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)        1 2024-04-12 09:51:55.000000 python_colored_print-1.1.0/python_colored_print.egg-info/dependency_links.txt
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)       14 2024-04-12 09:51:55.000000 python_colored_print-1.1.0/python_colored_print.egg-info/top_level.txt
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)       80 2024-04-12 09:51:55.177028 python_colored_print-1.1.0/setup.cfg
+-rw-rw-r--   0 benyamin  (1000) benyamin  (1000)      986 2024-01-06 14:33:08.000000 python_colored_print-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python_colored_print-1.0.0rc1/setup.py` & `python_colored_print-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     packages=find_packages(),
     keywords=[
         'log',
         'logging',
         'python3',
         'python',
     ],
-    download_url='https://github.com/agn-7/colored-print/archive/refs/tags/v1.0.0-rc1.zip',
+    download_url=f"https://github.com/agn-7/colored-print/archive/refs/tags/v{__version__}.zip",
     install_requires=[
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
 )
```

### Comparing `python_colored_print-1.0.0rc1/README.rst` & `python_colored_print-1.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 Colored Print
 -------------
 
 
-.. image:: https://img.shields.io/pypi/v/mix-mavis
-   :target: https://pypi.org/project/colored-print/
+.. image:: https://img.shields.io/pypi/v/python-colored-print
+   :target: https://pypi.org/project/python-colored-print/
    :alt: PyPI
 
 
-.. image:: https://img.shields.io/pypi/pyversions/wfuzz
-   :target: https://pypi.org/project/colored-print/
+.. image:: https://img.shields.io/pypi/pyversions/python-colored-print
+   :target: https://pypi.org/project/python-colored-print/
    :alt: Python Versions
 
 
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target: https://raw.githubusercontent.com/agn-7/colored-print/master/LICENSE
    :alt: GitHub license
 
@@ -28,24 +28,22 @@
    pip install python-colored-print
 
 Usage
 -----
 
 .. code-block:: python
 
-   from colored_print import ColoredPrint
-
-
-   log = ColoredPrint()
+   from colored_print import log
 
    log.success("Hello", 123, "Bye").store()
    log.info("Hello", 123, "Bye")
    log.warn("Hello", 123, "Bye")
    log.err("Hello", 123, "Bye").store()
    log.pink("Hello", 123, "Bye")
+   log("Hello", 123, "Bye")  # default color is white
 
 Output
 ------
 
 
 .. image:: https://i.stack.imgur.com/HMVP6.png
    :target: https://i.stack.imgur.com/HMVP6.png
```

