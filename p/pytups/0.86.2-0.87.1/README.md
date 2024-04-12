# Comparing `tmp/pytups-0.86.2.tar.gz` & `tmp/pytups-0.87.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytups-0.86.2.tar", last modified: Tue Nov 22 15:08:50 2022, max compression
+gzip compressed data, was "pytups-0.87.1.tar", last modified: Fri Apr 12 16:44:37 2024, max compression
```

## Comparing `pytups-0.86.2.tar` & `pytups-0.87.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 15:08:50.000000 pytups-0.86.2/
--rw-r--r--   0 runner    (1001) docker     (116)     4462 2022-11-22 15:08:50.000000 pytups-0.86.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3203 2022-11-22 15:08:45.000000 pytups-0.86.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups/
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-11-22 15:08:45.000000 pytups-0.86.2/pytups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4126 2022-11-22 15:08:45.000000 pytups-0.86.2/pytups/orderedSet.py
--rw-r--r--   0 runner    (1001) docker     (116)    18120 2022-11-22 15:08:45.000000 pytups-0.86.2/pytups/superdict.py
--rw-r--r--   0 runner    (1001) docker     (116)     1115 2022-11-22 15:08:45.000000 pytups-0.86.2/pytups/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)    13490 2022-11-22 15:08:45.000000 pytups-0.86.2/pytups/tuplist.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4462 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      233 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-11-22 15:08:50.000000 pytups-0.86.2/pytups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-22 15:08:50.000000 pytups-0.86.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      977 2022-11-22 15:08:45.000000 pytups-0.86.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:44:37.092387 pytups-0.87.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 16:44:33.000000 pytups-0.87.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-12 16:44:33.000000 pytups-0.87.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-12 16:44:37.088387 pytups-0.87.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 16:44:33.000000 pytups-0.87.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:44:37.088387 pytups-0.87.1/pytups/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/orderedSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/superdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-04-12 16:44:33.000000 pytups-0.87.1/pytups/tuplist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:44:37.088387 pytups-0.87.1/pytups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-12 16:44:37.000000 pytups-0.87.1/pytups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-12 16:44:37.000000 pytups-0.87.1/pytups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:44:37.000000 pytups-0.87.1/pytups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 16:44:37.000000 pytups-0.87.1/pytups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:44:37.092387 pytups-0.87.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 16:44:33.000000 pytups-0.87.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:44:37.088387 pytups-0.87.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-12 16:44:33.000000 pytups-0.87.1/tests/test_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-12 16:44:33.000000 pytups-0.87.1/tests/test_ordSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14046 2024-04-12 16:44:33.000000 pytups-0.87.1/tests/test_tuplists.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytups-0.86.2/PKG-INFO` & `pytups-0.87.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 Metadata-Version: 2.1
 Name: pytups
-Version: 0.86.2
+Version: 0.87.1
 Summary: data wrangling for lists of tuples and dictionaries
 Home-page: https://github.com/pchtsp/pytups
+Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
 Author: Franco Peschiera
 Author-email: pchtsp@gmail.com
 Maintainer: Franco Peschiera
 Maintainer-email: pchtsp@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
-Description: Pytups
-        **************************
-        .. image:: https://img.shields.io/pypi/v/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://img.shields.io/pypi/l/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://img.shields.io/pypi/pyversions/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://travis-ci.org/pchtsp/pytups.svg?branch=master
-            :target: https://travis-ci.org/pchtsp/pytups
-        
-        What and why
-        ================
-        
-        The idea is to allow sparse operations to be executed in matrix data.
-        
-        I grew used to the chained operations in R's `tidyverse <https://www.tidyverse.org/>`_  packages or, although not a great fan myself, python's `pandas <https://pandas.pydata.org/>`_ . I find myself using dictionary and list comprehensions all the time to pass from one data format to the other efficiently. But after doing it for the Nth time, I thought of automaticing it.
-        
-        In my case, it helps me construct optimisation models with  `PuLP <https://github.com/coin-or/pulp>`_. I see other possible uses not related to OR.
-        
-        I've implemented some additional methods to regular dictionaries, lists and sets to come up with interesting methods that somewhat quickly pass from one to the other and help with data wrangling.
-        
-        In order for the operations to make any sense, the assumption that is done is that whatever you are using has the same 'structure'. For example, if you a have a list of tuples: every element of the list is a tuple with the same size and the Nth element of the tuple has the same type, e.g. ``[(1, 'red', 'b', '2018-01'), (10, 'ccc', 'ttt', 'ff')]``. Note that both tuples have four elements and the first one is a number, not a string. We do not check that this is consistent.
-        
-        They're made to always return a new object, so no "in-place" editing, hopefully.
-        
-        Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
-        
-        Python versions
-        ================
-        
-        Python 3.6 and up.
-        
-        
-        Quick example
-        ================
-        
-        We index a tuple list according to some index positions.::
-        
-            import pytups as pt
-            some_list_of_tuples = [('a', 'b', 'c', 1), ('a', 'b', 'c', 2), ('a', 'b', 'c', 45)]
-            tp_list = pt.TupList(some_list_of_tuples)
-            tp_list.to_dict(result_col=3)
-            # {('a', 'b', 'c'): [1, 2, 45]}
-            tp_list.to_dict(result_col=3).to_dictdict()
-            # {'a': {'b': {'c': [1, 2, 45]}}}
-            tp_list.to_dict(result_col=[2, 3])
-            # {('a', 'b'): [('c', 1), ('c', 2), ('c', 45)]}
-        
-        We do some operations on dictionaries with common keys.::
-        
-            import pytups as pt
-            some_dict = pt.SuperDict(a=1, b=2, c=3, d=5)
-            some_other_dict = pt.SuperDict(a=5, b=7, c=1)
-            some_other_dict + some_dict
-            # {'a': 6, 'b': 9, 'c': 4}
-            some_other_dict.vapply(lambda v: v**2)
-            # {'a': 25, 'b': 49, 'c': 1}
-            some_other_dict.kvapply(lambda k, v: v/some_dict[k])
-            # {'a': 5.0, 'b': 3.5, 'c': 0.3333333333333333}
-        
-        Installing
-        ================
-        
-        ::
-        
-            pip install pytups
-        
-        or, for the development version::
-        
-            pip install https://github.com/pchtsp/pytups/archive/master.zip
-        
-        Testing
-        ================
-        
-        Run the command::
-            
-            python -m unittest discover -s tests
-        
-        if the output says OK, all tests were passed.
 Keywords: super dict dictionary tuple list math pulp
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+
+Pytups
+**************************
+.. image:: https://img.shields.io/pypi/v/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://img.shields.io/pypi/l/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://img.shields.io/pypi/pyversions/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://travis-ci.org/pchtsp/pytups.svg?branch=master
+    :target: https://travis-ci.org/pchtsp/pytups
+
+What and why
+================
+
+The idea is to allow sparse operations to be executed in matrix data.
+
+I grew used to the chained operations in R's `tidyverse <https://www.tidyverse.org/>`_  packages or, although not a great fan myself, python's `pandas <https://pandas.pydata.org/>`_ . I find myself using dictionary and list comprehensions all the time to pass from one data format to the other efficiently. But after doing it for the Nth time, I thought of automaticing it.
+
+In my case, it helps me construct optimisation models with  `PuLP <https://github.com/coin-or/pulp>`_. I see other possible uses not related to OR.
+
+I've implemented some additional methods to regular dictionaries, lists and sets to come up with interesting methods that somewhat quickly pass from one to the other and help with data wrangling.
+
+In order for the operations to make any sense, the assumption that is done is that whatever you are using has the same 'structure'. For example, if you a have a list of tuples: every element of the list is a tuple with the same size and the Nth element of the tuple has the same type, e.g. ``[(1, 'red', 'b', '2018-01'), (10, 'ccc', 'ttt', 'ff')]``. Note that both tuples have four elements and the first one is a number, not a string. We do not check that this is consistent.
+
+They're made to always return a new object, so no "in-place" editing, hopefully.
+
+Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
+
+Python versions
+================
+
+Python 3.6 and up.
+
+
+Quick example
+================
+
+We index a tuple list according to some index positions.::
+
+    import pytups as pt
+    some_list_of_tuples = [('a', 'b', 'c', 1), ('a', 'b', 'c', 2), ('a', 'b', 'c', 45)]
+    tp_list = pt.TupList(some_list_of_tuples)
+    tp_list.to_dict(result_col=3)
+    # {('a', 'b', 'c'): [1, 2, 45]}
+    tp_list.to_dict(result_col=3).to_dictdict()
+    # {'a': {'b': {'c': [1, 2, 45]}}}
+    tp_list.to_dict(result_col=[2, 3])
+    # {('a', 'b'): [('c', 1), ('c', 2), ('c', 45)]}
+
+We do some operations on dictionaries with common keys.::
+
+    import pytups as pt
+    some_dict = pt.SuperDict(a=1, b=2, c=3, d=5)
+    some_other_dict = pt.SuperDict(a=5, b=7, c=1)
+    some_other_dict + some_dict
+    # {'a': 6, 'b': 9, 'c': 4}
+    some_other_dict.vapply(lambda v: v**2)
+    # {'a': 25, 'b': 49, 'c': 1}
+    some_other_dict.kvapply(lambda k, v: v/some_dict[k])
+    # {'a': 5.0, 'b': 3.5, 'c': 0.3333333333333333}
+
+Installing
+================
+
+::
+
+    pip install pytups
+
+or, for the development version::
+
+    pip install https://github.com/pchtsp/pytups/archive/master.zip
+
+Testing
+================
+
+Run the command::
+    
+    python -m unittest discover -s tests
+
+if the output says OK, all tests were passed.
```

### Comparing `pytups-0.86.2/README.rst` & `pytups-0.87.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytups-0.86.2/pytups/orderedSet.py` & `pytups-0.87.1/pytups/orderedSet.py`

 * *Files identical despite different names*

### Comparing `pytups-0.86.2/pytups/superdict.py` & `pytups-0.87.1/pytups/superdict.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     def clean(self, default_value=0, func: Callable = None, **kwargs) -> "SuperDict":
         """
         Filters elements by value
 
         :param default_value: value of elements to take out
         :param function func: function that evaluates to true if we take out the element
-        :param **kwags: optional arguments for func
+        :param kwargs: optional arguments for func
         :return: new :py:class:`SuperDict`
         :rtype: :py:class:`SuperDict`
 
         >>> SuperDict({'a': 1, 'b': 0, 'c': 1}).clean(0)
         {'a': 1, 'c': 1}
         """
         if func is None:
```

### Comparing `pytups-0.86.2/pytups/tools.py` & `pytups-0.87.1/pytups/tools.py`

 * *Files identical despite different names*

### Comparing `pytups-0.86.2/pytups/tuplist.py` & `pytups-0.87.1/pytups/tuplist.py`

 * *Files 4% similar despite different names*

```diff
@@ -345,14 +345,26 @@
 
             return pd.DataFrame(self.to_list(), **kwargs)
         except ImportError:
             raise ImportError(
                 "Pandas is not present in your system. Try: pip install pandas"
             )
 
+    @classmethod
+    def from_df(cls, data, **kwargs):
+        try:
+            import pandas as pd
+
+            return cls(data.to_dict(orient="records", **kwargs))
+
+        except ImportError:
+            raise ImportError(
+                "Pandas is not present in your system. Try: pip install pandas"
+            )
+
     def sorted(self, **kwargs) -> "TupList":
         """
         Applies sorted function to elements and returns a TupList
 
         :param kwargs: arguments for sorted function
             main arguments for sorted are:
             - key
@@ -369,26 +381,36 @@
 
     def to_csv(self, path: str) -> "TupList":
         """
         Exports the list to a csv file
         :param path: filename
         :return: the same :py:class:`TupList`
         """
+        if len(self) == 0:
+            return None
+        first = self[0]
+        # Handle case of list of dict
+        if isinstance(first, dict):
+            cols = first.keys()
+            thing_to_write = [tuple(cols)] + self.take(list(cols))
+        else:
+            thing_to_write = self
         with open(path, "w", newline="\n", encoding="utf-8") as out:
             csv_out = csv.writer(out)
-            csv_out.writerows(self)
+            csv_out.writerows(thing_to_write)
         return self
 
     @classmethod
     def from_csv(cls, path: str, func: Callable = None, **kwargs) -> "TupList":
         """
         Generates a new TupList by reading a csv file
-        :param path: filename
+
+        :param str path: filename
         :param callable func: function to apply to each row
-        :**kwargs: arguments to csv.reader
+        :param kwargs: arguments to csv.reader
         :return: new :py:class:`TupList`
         """
         if func is None:
             func = tuple
         with open(path) as f:
             data = cls(csv.reader(f, **kwargs)).vapply(func)
         return data
```

### Comparing `pytups-0.86.2/pytups.egg-info/PKG-INFO` & `pytups-0.87.1/pytups.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 Metadata-Version: 2.1
 Name: pytups
-Version: 0.86.2
+Version: 0.87.1
 Summary: data wrangling for lists of tuples and dictionaries
 Home-page: https://github.com/pchtsp/pytups
+Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
 Author: Franco Peschiera
 Author-email: pchtsp@gmail.com
 Maintainer: Franco Peschiera
 Maintainer-email: pchtsp@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/pchtsp/pytups/archive/master.zip
-Description: Pytups
-        **************************
-        .. image:: https://img.shields.io/pypi/v/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://img.shields.io/pypi/l/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://img.shields.io/pypi/pyversions/pytups.svg
-            :target: https://pypi.org/project/pytups/
-        .. image:: https://travis-ci.org/pchtsp/pytups.svg?branch=master
-            :target: https://travis-ci.org/pchtsp/pytups
-        
-        What and why
-        ================
-        
-        The idea is to allow sparse operations to be executed in matrix data.
-        
-        I grew used to the chained operations in R's `tidyverse <https://www.tidyverse.org/>`_  packages or, although not a great fan myself, python's `pandas <https://pandas.pydata.org/>`_ . I find myself using dictionary and list comprehensions all the time to pass from one data format to the other efficiently. But after doing it for the Nth time, I thought of automaticing it.
-        
-        In my case, it helps me construct optimisation models with  `PuLP <https://github.com/coin-or/pulp>`_. I see other possible uses not related to OR.
-        
-        I've implemented some additional methods to regular dictionaries, lists and sets to come up with interesting methods that somewhat quickly pass from one to the other and help with data wrangling.
-        
-        In order for the operations to make any sense, the assumption that is done is that whatever you are using has the same 'structure'. For example, if you a have a list of tuples: every element of the list is a tuple with the same size and the Nth element of the tuple has the same type, e.g. ``[(1, 'red', 'b', '2018-01'), (10, 'ccc', 'ttt', 'ff')]``. Note that both tuples have four elements and the first one is a number, not a string. We do not check that this is consistent.
-        
-        They're made to always return a new object, so no "in-place" editing, hopefully.
-        
-        Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
-        
-        Python versions
-        ================
-        
-        Python 3.6 and up.
-        
-        
-        Quick example
-        ================
-        
-        We index a tuple list according to some index positions.::
-        
-            import pytups as pt
-            some_list_of_tuples = [('a', 'b', 'c', 1), ('a', 'b', 'c', 2), ('a', 'b', 'c', 45)]
-            tp_list = pt.TupList(some_list_of_tuples)
-            tp_list.to_dict(result_col=3)
-            # {('a', 'b', 'c'): [1, 2, 45]}
-            tp_list.to_dict(result_col=3).to_dictdict()
-            # {'a': {'b': {'c': [1, 2, 45]}}}
-            tp_list.to_dict(result_col=[2, 3])
-            # {('a', 'b'): [('c', 1), ('c', 2), ('c', 45)]}
-        
-        We do some operations on dictionaries with common keys.::
-        
-            import pytups as pt
-            some_dict = pt.SuperDict(a=1, b=2, c=3, d=5)
-            some_other_dict = pt.SuperDict(a=5, b=7, c=1)
-            some_other_dict + some_dict
-            # {'a': 6, 'b': 9, 'c': 4}
-            some_other_dict.vapply(lambda v: v**2)
-            # {'a': 25, 'b': 49, 'c': 1}
-            some_other_dict.kvapply(lambda k, v: v/some_dict[k])
-            # {'a': 5.0, 'b': 3.5, 'c': 0.3333333333333333}
-        
-        Installing
-        ================
-        
-        ::
-        
-            pip install pytups
-        
-        or, for the development version::
-        
-            pip install https://github.com/pchtsp/pytups/archive/master.zip
-        
-        Testing
-        ================
-        
-        Run the command::
-            
-            python -m unittest discover -s tests
-        
-        if the output says OK, all tests were passed.
 Keywords: super dict dictionary tuple list math pulp
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+License-File: AUTHORS.md
+
+Pytups
+**************************
+.. image:: https://img.shields.io/pypi/v/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://img.shields.io/pypi/l/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://img.shields.io/pypi/pyversions/pytups.svg
+    :target: https://pypi.org/project/pytups/
+.. image:: https://travis-ci.org/pchtsp/pytups.svg?branch=master
+    :target: https://travis-ci.org/pchtsp/pytups
+
+What and why
+================
+
+The idea is to allow sparse operations to be executed in matrix data.
+
+I grew used to the chained operations in R's `tidyverse <https://www.tidyverse.org/>`_  packages or, although not a great fan myself, python's `pandas <https://pandas.pydata.org/>`_ . I find myself using dictionary and list comprehensions all the time to pass from one data format to the other efficiently. But after doing it for the Nth time, I thought of automaticing it.
+
+In my case, it helps me construct optimisation models with  `PuLP <https://github.com/coin-or/pulp>`_. I see other possible uses not related to OR.
+
+I've implemented some additional methods to regular dictionaries, lists and sets to come up with interesting methods that somewhat quickly pass from one to the other and help with data wrangling.
+
+In order for the operations to make any sense, the assumption that is done is that whatever you are using has the same 'structure'. For example, if you a have a list of tuples: every element of the list is a tuple with the same size and the Nth element of the tuple has the same type, e.g. ``[(1, 'red', 'b', '2018-01'), (10, 'ccc', 'ttt', 'ff')]``. Note that both tuples have four elements and the first one is a number, not a string. We do not check that this is consistent.
+
+They're made to always return a new object, so no "in-place" editing, hopefully.
+
+Right now there are three classes to use: dictionaries, tuple lists and ordered sets.
+
+Python versions
+================
+
+Python 3.6 and up.
+
+
+Quick example
+================
+
+We index a tuple list according to some index positions.::
+
+    import pytups as pt
+    some_list_of_tuples = [('a', 'b', 'c', 1), ('a', 'b', 'c', 2), ('a', 'b', 'c', 45)]
+    tp_list = pt.TupList(some_list_of_tuples)
+    tp_list.to_dict(result_col=3)
+    # {('a', 'b', 'c'): [1, 2, 45]}
+    tp_list.to_dict(result_col=3).to_dictdict()
+    # {'a': {'b': {'c': [1, 2, 45]}}}
+    tp_list.to_dict(result_col=[2, 3])
+    # {('a', 'b'): [('c', 1), ('c', 2), ('c', 45)]}
+
+We do some operations on dictionaries with common keys.::
+
+    import pytups as pt
+    some_dict = pt.SuperDict(a=1, b=2, c=3, d=5)
+    some_other_dict = pt.SuperDict(a=5, b=7, c=1)
+    some_other_dict + some_dict
+    # {'a': 6, 'b': 9, 'c': 4}
+    some_other_dict.vapply(lambda v: v**2)
+    # {'a': 25, 'b': 49, 'c': 1}
+    some_other_dict.kvapply(lambda k, v: v/some_dict[k])
+    # {'a': 5.0, 'b': 3.5, 'c': 0.3333333333333333}
+
+Installing
+================
+
+::
+
+    pip install pytups
+
+or, for the development version::
+
+    pip install https://github.com/pchtsp/pytups/archive/master.zip
+
+Testing
+================
+
+Run the command::
+    
+    python -m unittest discover -s tests
+
+if the output says OK, all tests were passed.
```

### Comparing `pytups-0.86.2/setup.py` & `pytups-0.87.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 from setuptools import setup
 
 packages = ["pytups"]
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
+version_dict = {}
+exec(open("pytups/constants.py").read(), version_dict)
+VERSION = version_dict["VERSION"]
+
 required = []
 
 kwargs = {
     "name": "pytups",
-    "version": "0.86.2",
+    "version": VERSION,
     "packages": packages,
     "description": "data wrangling for lists of tuples and dictionaries",
     "long_description": long_description,
     "long_description_content_type": "text/x-rst",
     "author": "Franco Peschiera",
     "maintainer": "Franco Peschiera",
     "author_email": "pchtsp@gmail.com",
```

