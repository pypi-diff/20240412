# Comparing `tmp/gerber_writer-0.4.2.22.tar.gz` & `tmp/gerber_writer-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerber_writer-0.4.2.22.tar", last modified: Wed Apr 10 21:21:41 2024, max compression
+gzip compressed data, was "gerber_writer-0.4.3.tar", last modified: Fri Apr 12 18:40:05 2024, max compression
```

## Comparing `gerber_writer-0.4.2.22.tar` & `gerber_writer-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 21:21:41.887476 gerber_writer-0.4.2.22/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2024-04-09 14:53:35.000000 gerber_writer-0.4.2.22/LICENSE
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2776 2024-04-10 21:21:41.887476 gerber_writer-0.4.2.22/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1981 2024-04-09 14:53:35.000000 gerber_writer-0.4.2.22/README.rst
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1066 2024-04-10 21:08:01.000000 gerber_writer-0.4.2.22/pyproject.toml
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-10 21:21:41.887476 gerber_writer-0.4.2.22/setup.cfg
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 21:21:41.883476 gerber_writer-0.4.2.22/src/
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 21:21:41.883476 gerber_writer-0.4.2.22/src/gerber_writer/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       78 2024-04-10 21:08:01.000000 gerber_writer-0.4.2.22/src/gerber_writer/__init__.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.2.22/src/gerber_writer/lutils.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.22/src/gerber_writer/macros.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.22/src/gerber_writer/padmasters.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.2.22/src/gerber_writer/writer.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.2.22/src/gerber_writer/writer_test.py
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 21:21:41.883476 gerber_writer-0.4.2.22/src/gerber_writer.egg-info/
--rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2776 2024-04-10 21:21:41.000000 gerber_writer-0.4.2.22/src/gerber_writer.egg-info/PKG-INFO
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      418 2024-04-10 21:21:41.000000 gerber_writer-0.4.2.22/src/gerber_writer.egg-info/SOURCES.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-10 21:21:41.000000 gerber_writer-0.4.2.22/src/gerber_writer.egg-info/dependency_links.txt
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-10 21:21:41.000000 gerber_writer-0.4.2.22/src/gerber_writer.egg-info/top_level.txt
-drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-10 21:21:41.883476 gerber_writer-0.4.2.22/tests/
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.22/tests/test_arcs.py
--rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.2.22/tests/test_contours.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    11357 2024-04-09 14:53:35.000000 gerber_writer-0.4.3/LICENSE
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2533 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/PKG-INFO
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/doc/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1738 2024-04-12 18:24:55.000000 gerber_writer-0.4.3/doc/README.rst
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      990 2024-04-12 14:57:21.000000 gerber_writer-0.4.3/pyproject.toml
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       38 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/setup.cfg
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/gerber_writer/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       75 2024-04-12 09:41:07.000000 gerber_writer-0.4.3/src/gerber_writer/__init__.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      250 2024-03-24 15:01:36.000000 gerber_writer-0.4.3/src/gerber_writer/lutils.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2133 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/src/gerber_writer/macros.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    10754 2024-03-16 14:00:10.000000 gerber_writer-0.4.3/src/gerber_writer/padmasters.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    56441 2024-03-16 14:00:10.000000 gerber_writer-0.4.3/src/gerber_writer/writer.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)    20619 2023-12-04 16:51:31.000000 gerber_writer-0.4.3/src/gerber_writer/writer_test.py
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/src/gerber_writer.egg-info/
+-rw-r--r--   0 alaindef  (1000) alaindef  (1000)     2533 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/PKG-INFO
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)      422 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)        1 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)       14 2024-04-12 18:40:05.000000 gerber_writer-0.4.3/src/gerber_writer.egg-info/top_level.txt
+drwxrwxr-x   0 alaindef  (1000) alaindef  (1000)        0 2024-04-12 18:40:05.706092 gerber_writer-0.4.3/tests/
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     2401 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/tests/test_arcs.py
+-rw-rw-r--   0 alaindef  (1000) alaindef  (1000)     1264 2023-10-25 19:00:28.000000 gerber_writer-0.4.3/tests/test_contours.py
```

### Comparing `gerber_writer-0.4.2.22/LICENSE` & `gerber_writer-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/PKG-INFO` & `gerber_writer-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.2.22
+Version: 0.4.3
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
-Project-URL: Documentation, https://alaindef.github.io/alaindef.github.io.zerp/index.html
+Project-URL: Repository, https://github.com/karel-tavernier/gerber_writer
+Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/html
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
@@ -20,82 +20,70 @@
 
 Readme
 ======
 
 Purpose
 -------
 
-A Python library for writing Gerber files.
+A Python library for writing Gerber files. 
 
+* The API is much simpler than the Gerber format specification - 8 pages vs 200.
 * No need to read the 200 page Gerber format specification.
-* API much simpler than the Gerber format specification - 8 pages vs 200.
-* All common pad shapes built-in.
-* User-defined pad special shapes
-* 100% compliance with the specification, rev 2022.02.
+* All common pad shapes are built-in.
+* User-defined pads shapes are easily created.
+* 100% compliance with revision 2023.08 of the Gerber Layer Format Specification.
 * Conservative, robust output files.
-* Risky constructs that fail in some buggy implementations are not used.
-* Include standardized meta information needed for fabrication, such as which pads are vias.
-* Verify whether the input parameters comply with the Gerber spec.
+* Risky constructs failing in some buggy applications are avoided.
+* Standardized meta information for fabrication, such as which pads are vias.
+* Input parameters are checked for compliance with the Gerber spec.
 * Stateless input (the gerber_writer takes care of the Gerber states).
 
-Example:
-
-.. code-block:: python
+Example:: 
 
 	from gerber_writer import DataLayer, Circle, RoundedRectangle
-
+		
 	trace_width = 0.127
 	via_pad = Circle(0.508, 'ViaPad')
 	IC17_toe = RoundedRectangle(1.257, 2.286, 0.254, 'SMDPad,CuDef')
 	toe_point = (0, 2.54)
 	via_point = (5.08, 0)
 
 	top = DataLayer('Copper,L1,Top,Signal')
 
 	top.add_pad(IC17_toe, toe_point, angle=45)
 	top.add_trace_line(toe_point, (2.54, 0), trace_width, 'Conductor')
 	top.add_trace_line((2.54, 0), via_point, trace_width, 'Conductor')
 	top.add_pad(via_pad, via_point)
 
 	with open('gerbers\gerber_writer_example_small.gbr', 'w') as outfile:
-	    top.dump_gerber(outfile)
-
-.. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
+        top.dump_gerber(outfile)
+		
+.. image:: example_small.png
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
-
-+++++++
-Windows
-+++++++
-
-.. code-block:: batch
+Windows::
 
-	$ py -m pip install gerber_writer
+    $ py -m pip install gerber_writer
+	
+Linux::
 
-+++++
-Linux
-+++++
-
-.. code-block:: batch
-
-	$ python3 -m pip install gerber_writer
+    $ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
 * Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
-
+ 
 Contact
 -------
-
+ 
 karel_tavernier@hotmail.com
```

### Comparing `gerber_writer-0.4.2.22/README.rst` & `gerber_writer-0.4.3/doc/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 Readme
 ======
 
 Purpose
 -------
 
-A Python library for writing Gerber files.
+A Python library for writing Gerber files. 
 
+* The API is much simpler than the Gerber format specification - 8 pages vs 200.
 * No need to read the 200 page Gerber format specification.
-* API much simpler than the Gerber format specification - 8 pages vs 200.
-* All common pad shapes built-in.
-* User-defined pad special shapes
-* 100% compliance with the specification, rev 2022.02.
+* All common pad shapes are built-in.
+* User-defined pads shapes are easily created.
+* 100% compliance with revision 2023.08 of the Gerber Layer Format Specification.
 * Conservative, robust output files.
-* Risky constructs that fail in some buggy implementations are not used.
-* Include standardized meta information needed for fabrication, such as which pads are vias.
-* Verify whether the input parameters comply with the Gerber spec.
+* Risky constructs failing in some buggy applications are avoided.
+* Standardized meta information for fabrication, such as which pads are vias.
+* Input parameters are checked for compliance with the Gerber spec.
 * Stateless input (the gerber_writer takes care of the Gerber states).
 
-Example:
-
-.. code-block:: python
+Example:: 
 
 	from gerber_writer import DataLayer, Circle, RoundedRectangle
-
+		
 	trace_width = 0.127
 	via_pad = Circle(0.508, 'ViaPad')
 	IC17_toe = RoundedRectangle(1.257, 2.286, 0.254, 'SMDPad,CuDef')
 	toe_point = (0, 2.54)
 	via_point = (5.08, 0)
 
 	top = DataLayer('Copper,L1,Top,Signal')
 
 	top.add_pad(IC17_toe, toe_point, angle=45)
 	top.add_trace_line(toe_point, (2.54, 0), trace_width, 'Conductor')
 	top.add_trace_line((2.54, 0), via_point, trace_width, 'Conductor')
 	top.add_pad(via_pad, via_point)
 
 	with open('gerbers\gerber_writer_example_small.gbr', 'w') as outfile:
-	    top.dump_gerber(outfile)
-
-.. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
+        top.dump_gerber(outfile)
+		
+.. image:: example_small.png
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
-
-+++++++
-Windows
-+++++++
-
-.. code-block:: batch
+Windows::
 
-	$ py -m pip install gerber_writer
+    $ py -m pip install gerber_writer
+	
+Linux::
 
-+++++
-Linux
-+++++
-
-.. code-block:: batch
-
-	$ python3 -m pip install gerber_writer
+    $ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
 * Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
-
+ 
 Contact
 -------
-
-karel_tavernier@hotmail.com
+ 
+karel_tavernier@hotmail.com
```

### Comparing `gerber_writer-0.4.2.22/pyproject.toml` & `gerber_writer-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "gerber_writer"
-version = "0.4.2.22"
+version = "0.4.3"
 authors = [
   { name="Karel Tavernier", email="karel_tavernier@hotmail.com" },
 ]
 description = "A library to write Gerber files"
-readme = "README.rst"
+readme = "doc/README.rst"
 license = { text ="Apache 2.0 License" }
 requires-python = ">=3.9"
 keywords = ["Gerber", "RS-274X", "PCB", "CAD", "CAM", "library"]
 dependencies = []
 
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -21,10 +21,9 @@
 	"Development Status :: 5 - Production/Stable",
 	"Intended Audience :: Developers",
 	"Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
 	"Topic :: Software Development :: Libraries",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/Karel-Tavernier/gerber_writer"
-#"Documentation"= "https://karel-tavernier.github.io/gerber_writer/"
-"Documentation"= "https://alaindef.github.io/alaindef.github.io.zerp/index.html"
+"Repository" = "https://github.com/karel-tavernier/gerber_writer"
+"Documentation"= "https://karel-tavernier.github.io/gerber_writer/html"
```

### Comparing `gerber_writer-0.4.2.22/src/gerber_writer/macros.py` & `gerber_writer-0.4.3/src/gerber_writer/macros.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/src/gerber_writer/padmasters.py` & `gerber_writer-0.4.3/src/gerber_writer/padmasters.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/src/gerber_writer/writer.py` & `gerber_writer-0.4.3/src/gerber_writer/writer.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/src/gerber_writer/writer_test.py` & `gerber_writer-0.4.3/src/gerber_writer/writer_test.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/src/gerber_writer.egg-info/PKG-INFO` & `gerber_writer-0.4.3/src/gerber_writer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gerber_writer
-Version: 0.4.2.22
+Version: 0.4.3
 Summary: A library to write Gerber files
 Author-email: Karel Tavernier <karel_tavernier@hotmail.com>
 License: Apache 2.0 License
-Project-URL: Homepage, https://github.com/Karel-Tavernier/gerber_writer
-Project-URL: Documentation, https://alaindef.github.io/alaindef.github.io.zerp/index.html
+Project-URL: Repository, https://github.com/karel-tavernier/gerber_writer
+Project-URL: Documentation, https://karel-tavernier.github.io/gerber_writer/html
 Keywords: Gerber,RS-274X,PCB,CAD,CAM,library
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
@@ -20,82 +20,70 @@
 
 Readme
 ======
 
 Purpose
 -------
 
-A Python library for writing Gerber files.
+A Python library for writing Gerber files. 
 
+* The API is much simpler than the Gerber format specification - 8 pages vs 200.
 * No need to read the 200 page Gerber format specification.
-* API much simpler than the Gerber format specification - 8 pages vs 200.
-* All common pad shapes built-in.
-* User-defined pad special shapes
-* 100% compliance with the specification, rev 2022.02.
+* All common pad shapes are built-in.
+* User-defined pads shapes are easily created.
+* 100% compliance with revision 2023.08 of the Gerber Layer Format Specification.
 * Conservative, robust output files.
-* Risky constructs that fail in some buggy implementations are not used.
-* Include standardized meta information needed for fabrication, such as which pads are vias.
-* Verify whether the input parameters comply with the Gerber spec.
+* Risky constructs failing in some buggy applications are avoided.
+* Standardized meta information for fabrication, such as which pads are vias.
+* Input parameters are checked for compliance with the Gerber spec.
 * Stateless input (the gerber_writer takes care of the Gerber states).
 
-Example:
-
-.. code-block:: python
+Example:: 
 
 	from gerber_writer import DataLayer, Circle, RoundedRectangle
-
+		
 	trace_width = 0.127
 	via_pad = Circle(0.508, 'ViaPad')
 	IC17_toe = RoundedRectangle(1.257, 2.286, 0.254, 'SMDPad,CuDef')
 	toe_point = (0, 2.54)
 	via_point = (5.08, 0)
 
 	top = DataLayer('Copper,L1,Top,Signal')
 
 	top.add_pad(IC17_toe, toe_point, angle=45)
 	top.add_trace_line(toe_point, (2.54, 0), trace_width, 'Conductor')
 	top.add_trace_line((2.54, 0), via_point, trace_width, 'Conductor')
 	top.add_pad(via_pad, via_point)
 
 	with open('gerbers\gerber_writer_example_small.gbr', 'w') as outfile:
-	    top.dump_gerber(outfile)
-
-.. image:: https://github.com/Karel-Tavernier/gerber_writer/assets/56170852/7b351186-9cdc-4cc0-9f3b-04708ee50216
+        top.dump_gerber(outfile)
+		
+.. image:: example_small.png
 	:width: 800
 
 Installation
 ------------
 
-This package requires Python 3.9 or later, you can find it `here <https://www.python.org/downloads/>`_.
-
-+++++++
-Windows
-+++++++
-
-.. code-block:: batch
+Windows::
 
-	$ py -m pip install gerber_writer
+    $ py -m pip install gerber_writer
+	
+Linux::
 
-+++++
-Linux
-+++++
-
-.. code-block:: batch
-
-	$ python3 -m pip install gerber_writer
+    $ python3 -m pip install gerber_writer
 
 Requirements
 ------------
 
 * Python 3.9 or higher
 * Standard library only.
 * OS independent.
 
 License
 -------
 
 Apache 2.0 license
-
+ 
 Contact
 -------
-
+ 
 karel_tavernier@hotmail.com
```

### Comparing `gerber_writer-0.4.2.22/tests/test_arcs.py` & `gerber_writer-0.4.3/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `gerber_writer-0.4.2.22/tests/test_contours.py` & `gerber_writer-0.4.3/tests/test_contours.py`

 * *Files identical despite different names*

