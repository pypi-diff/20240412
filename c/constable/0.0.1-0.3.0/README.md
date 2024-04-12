# Comparing `tmp/constable-0.0.1.tar.gz` & `tmp/constable-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constable-0.0.1.tar", last modified: Thu Apr 11 12:37:03 2024, max compression
+gzip compressed data, was "constable-0.3.0.tar", last modified: Fri Apr 12 15:01:11 2024, max compression
```

## Comparing `constable-0.0.1.tar` & `constable-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 12:37:03.443135 constable-0.0.1/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1071 2024-04-11 12:34:49.000000 constable-0.0.1/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2078 2024-04-11 12:37:03.443135 constable-0.0.1/PKG-INFO
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1357 2024-04-11 12:34:49.000000 constable-0.0.1/README.rst
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 12:37:03.443135 constable-0.0.1/constable/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     6117 2024-04-11 12:34:49.000000 constable-0.0.1/constable/__init__.py
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 12:37:03.443135 constable-0.0.1/constable.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2078 2024-04-11 12:37:03.000000 constable-0.0.1/constable.egg-info/PKG-INFO
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      181 2024-04-11 12:37:03.000000 constable-0.0.1/constable.egg-info/SOURCES.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)        1 2024-04-11 12:37:03.000000 constable-0.0.1/constable.egg-info/dependency_links.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       10 2024-04-11 12:37:03.000000 constable-0.0.1/constable.egg-info/top_level.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       38 2024-04-11 12:37:03.443135 constable-0.0.1/setup.cfg
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1067 2024-04-11 12:34:49.000000 constable-0.0.1/setup.py
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-12 15:01:11.687677 constable-0.3.0/
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1071 2024-04-11 12:34:49.000000 constable-0.3.0/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2421 2024-04-12 15:01:11.687677 constable-0.3.0/PKG-INFO
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1700 2024-04-12 14:59:59.000000 constable-0.3.0/README.rst
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-12 15:01:11.687677 constable-0.3.0/constable/
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     7920 2024-04-12 14:55:54.000000 constable-0.3.0/constable/__init__.py
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-12 15:01:11.687677 constable-0.3.0/constable.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2421 2024-04-12 15:01:11.000000 constable-0.3.0/constable.egg-info/PKG-INFO
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      181 2024-04-12 15:01:11.000000 constable-0.3.0/constable.egg-info/SOURCES.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)        1 2024-04-12 15:01:11.000000 constable-0.3.0/constable.egg-info/dependency_links.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       10 2024-04-12 15:01:11.000000 constable-0.3.0/constable.egg-info/top_level.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       38 2024-04-12 15:01:11.687677 constable-0.3.0/setup.cfg
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1067 2024-04-12 14:55:54.000000 constable-0.3.0/setup.py
```

### Comparing `constable-0.0.1/LICENSE` & `constable-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `constable-0.0.1/PKG-INFO` & `constable-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constable
-Version: 0.0.1
+Version: 0.3.0
 Summary: One decorator for lazy debugging. Inserts print statements directly into your AST.
 Home-page: https://github.com/saurabh0719/constable
 Author: Saurabh Pujari
 Author-email: saurabhpuj99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/saurabh0719/constable#README
 Project-URL: Source, https://github.com/saurabh0719/constable
@@ -15,80 +15,76 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 constable
 --------------
 
-One decorator for lazy debugging. Inserts print statements directly into your AST.
+constable allows you to monitor the state of specified variables at each assignment operation, providing a step-by-step view of variable changes!
 
 View the `Github repository <https://github.com/saurabh0719/constable>`__ and the `official docs <https://github.com/saurabh0719/constable#README>`__.
 
+
+How does it work?
+~~~~~~~~~~~~~~~~~~
+
+The `constable.trace` decorator uses Python's Abstract Syntax Tree (AST) in much the same way we add `print`(s) to debug states. During runtime, it prepares and inserts `print` statements into the function's AST after every assignment operation (`ast.Assign`, `ast.AugAssign` and `ast.AnnAssign`), and then executes the modified code in a separate namespace with `exec`.
+
+
 .. code:: sh
 
     $ pip install constable
 
 Tested for python 3.8 and above.
 
-Key Features
-------------
-
-- Capture function args and result
-- Monitor variable state at each assignment op
-- Measure execution time
-- Any of the above can be turned on/off.
-
 
 Usage :
 ~~~~~~~~~~~~~
 
 
 Monitoring functions
 
 .. code:: python
 
     import constable
 
-    @constable.trace()
-    def add(a=1, b=2):
-        return a + b
-
-    add(1, 2)
-
-
-Output :
-
-::
-
-    executing: add(a = 1, b = 2)
-    execution time: add(a = 1, b = 2) -> 0.00014877 seconds
-
-
-Tracing variable assignments
-
-
-.. code:: python
-
-    import constable
-
     @constable.trace(['a', 'b'])
-    def do_something(a=5, b=6):
+    def example(a, b):
         a = a + b
         c = a
         a = "Experimenting with the AST"
         b = c + b
         a = c + b
         return a
 
-    do_something(1, 2)
+    example(5, 6)
 
 
 Output :
 
 ::
 
-    executing: do_something(a = 1, b = 2)
-    debug: do_something: a = 3
-    debug: do_something: a = Experimenting with the AST
-    debug: do_something: b = 5
-    debug: do_something: a = 8
-    execution time: do_something(a = 1, b = 2) -> 0.00009584 seconds
+    constable.trace: example:19 -
+        a = a + b
+        a = 11
+        type(a) = <class 'int'>
+
+    constable.trace: example:21 -
+        a = "Experimenting with the AST"
+        a = Experimenting with the AST
+        type(a) = <class 'str'>
+
+    constable.trace: example:22 -
+        b = c + b
+        b = 17
+        type(b) = <class 'int'>
+
+    constable.trace: example:23 -
+        a = c + b
+        a = 28
+        type(a) = <class 'int'>
+
+    constable.trace: example -
+        args: (5, 6)
+        kwargs: {}
+        returned: 28
+        execution time: 0.00029278 seconds
```

### Comparing `constable-0.0.1/constable.egg-info/PKG-INFO` & `constable-0.3.0/constable.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constable
-Version: 0.0.1
+Version: 0.3.0
 Summary: One decorator for lazy debugging. Inserts print statements directly into your AST.
 Home-page: https://github.com/saurabh0719/constable
 Author: Saurabh Pujari
 Author-email: saurabhpuj99@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/saurabh0719/constable#README
 Project-URL: Source, https://github.com/saurabh0719/constable
@@ -15,80 +15,76 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 constable
 --------------
 
-One decorator for lazy debugging. Inserts print statements directly into your AST.
+constable allows you to monitor the state of specified variables at each assignment operation, providing a step-by-step view of variable changes!
 
 View the `Github repository <https://github.com/saurabh0719/constable>`__ and the `official docs <https://github.com/saurabh0719/constable#README>`__.
 
+
+How does it work?
+~~~~~~~~~~~~~~~~~~
+
+The `constable.trace` decorator uses Python's Abstract Syntax Tree (AST) in much the same way we add `print`(s) to debug states. During runtime, it prepares and inserts `print` statements into the function's AST after every assignment operation (`ast.Assign`, `ast.AugAssign` and `ast.AnnAssign`), and then executes the modified code in a separate namespace with `exec`.
+
+
 .. code:: sh
 
     $ pip install constable
 
 Tested for python 3.8 and above.
 
-Key Features
-------------
-
-- Capture function args and result
-- Monitor variable state at each assignment op
-- Measure execution time
-- Any of the above can be turned on/off.
-
 
 Usage :
 ~~~~~~~~~~~~~
 
 
 Monitoring functions
 
 .. code:: python
 
     import constable
 
-    @constable.trace()
-    def add(a=1, b=2):
-        return a + b
-
-    add(1, 2)
-
-
-Output :
-
-::
-
-    executing: add(a = 1, b = 2)
-    execution time: add(a = 1, b = 2) -> 0.00014877 seconds
-
-
-Tracing variable assignments
-
-
-.. code:: python
-
-    import constable
-
     @constable.trace(['a', 'b'])
-    def do_something(a=5, b=6):
+    def example(a, b):
         a = a + b
         c = a
         a = "Experimenting with the AST"
         b = c + b
         a = c + b
         return a
 
-    do_something(1, 2)
+    example(5, 6)
 
 
 Output :
 
 ::
 
-    executing: do_something(a = 1, b = 2)
-    debug: do_something: a = 3
-    debug: do_something: a = Experimenting with the AST
-    debug: do_something: b = 5
-    debug: do_something: a = 8
-    execution time: do_something(a = 1, b = 2) -> 0.00009584 seconds
+    constable.trace: example:19 -
+        a = a + b
+        a = 11
+        type(a) = <class 'int'>
+
+    constable.trace: example:21 -
+        a = "Experimenting with the AST"
+        a = Experimenting with the AST
+        type(a) = <class 'str'>
+
+    constable.trace: example:22 -
+        b = c + b
+        b = 17
+        type(b) = <class 'int'>
+
+    constable.trace: example:23 -
+        a = c + b
+        a = 28
+        type(a) = <class 'int'>
+
+    constable.trace: example -
+        args: (5, 6)
+        kwargs: {}
+        returned: 28
+        execution time: 0.00029278 seconds
```

### Comparing `constable-0.0.1/setup.py` & `constable-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup
 
 long_description = pathlib.Path("README.rst").read_text()
 
 setup(
     name="constable",
     packages=["constable"],
-    version="0.0.1",
+    version="0.3.0",
     license="MIT",
     description="One decorator for lazy debugging. Inserts print statements directly into your AST.",
     long_description=long_description,
     long_description_content_type= 'text/x-rst',
     author="Saurabh Pujari",
     author_email="saurabhpuj99@gmail.com",
     url="https://github.com/saurabh0719/constable",
```

