# Comparing `tmp/python-espresso-1.8.3.tar.gz` & `tmp/python-espresso-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-espresso-1.8.3.tar", last modified: Mon Apr  8 13:31:20 2024, max compression
+gzip compressed data, was "python-espresso-1.8.4.tar", last modified: Fri Apr 12 04:27:09 2024, max compression
```

## Comparing `python-espresso-1.8.3.tar` & `python-espresso-1.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:31:20.740315 python-espresso-1.8.3/
--rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.3/LICENSE
--rw-rw-rw-   0        0        0     2226 2024-04-08 13:31:20.739314 python-espresso-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1854 2024-04-08 13:28:41.000000 python-espresso-1.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 13:31:20.727347 python-espresso-1.8.3/espresso/
--rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.3/espresso/Context.py
--rw-rw-rw-   0        0        0     4776 2024-04-08 13:25:43.000000 python-espresso-1.8.3/espresso/Evaluator.py
--rw-rw-rw-   0        0        0     3231 2024-04-08 13:10:00.000000 python-espresso-1.8.3/espresso/Lexer.py
--rw-rw-rw-   0        0        0     3747 2024-04-08 13:10:59.000000 python-espresso-1.8.3/espresso/Parser.py
--rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.3/espresso/__init__.py
--rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.3/espresso/exceptions.py
--rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.3/espresso/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:31:20.734321 python-espresso-1.8.3/python_espresso.egg-info/
--rw-rw-rw-   0        0        0     2226 2024-04-08 13:31:20.000000 python-espresso-1.8.3/python_espresso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-04-08 13:31:20.000000 python-espresso-1.8.3/python_espresso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:31:20.000000 python-espresso-1.8.3/python_espresso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 13:31:20.000000 python-espresso-1.8.3/python_espresso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 13:31:20.740315 python-espresso-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      533 2024-04-08 13:29:58.000000 python-espresso-1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:31:20.738315 python-espresso-1.8.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.3/tests/__init__.py
--rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.3/tests/test_evaluator.py
--rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.3/tests/test_lexer.py
--rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.3/tests/test_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:27:09.086117 python-espresso-1.8.4/
+-rw-rw-rw-   0        0        0     1082 2024-04-04 17:28:43.000000 python-espresso-1.8.4/LICENSE
+-rw-rw-rw-   0        0        0     2226 2024-04-12 04:27:09.086117 python-espresso-1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1854 2024-04-08 13:28:41.000000 python-espresso-1.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 04:27:09.070247 python-espresso-1.8.4/espresso/
+-rw-rw-rw-   0        0        0      437 2024-04-04 17:00:39.000000 python-espresso-1.8.4/espresso/Context.py
+-rw-rw-rw-   0        0        0     4845 2024-04-11 05:22:40.000000 python-espresso-1.8.4/espresso/Evaluator.py
+-rw-rw-rw-   0        0        0     3231 2024-04-08 13:10:00.000000 python-espresso-1.8.4/espresso/Lexer.py
+-rw-rw-rw-   0        0        0     3747 2024-04-08 13:10:59.000000 python-espresso-1.8.4/espresso/Parser.py
+-rw-rw-rw-   0        0        0      366 2024-04-03 13:48:41.000000 python-espresso-1.8.4/espresso/__init__.py
+-rw-rw-rw-   0        0        0      153 2024-04-03 13:48:09.000000 python-espresso-1.8.4/espresso/exceptions.py
+-rw-rw-rw-   0        0        0      586 2024-04-08 11:50:11.000000 python-espresso-1.8.4/espresso/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:27:09.070247 python-espresso-1.8.4/python_espresso.egg-info/
+-rw-rw-rw-   0        0        0     2226 2024-04-12 04:27:08.000000 python-espresso-1.8.4/python_espresso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-12 04:27:08.000000 python-espresso-1.8.4/python_espresso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 04:27:08.000000 python-espresso-1.8.4/python_espresso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 04:27:08.000000 python-espresso-1.8.4/python_espresso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 04:27:09.086117 python-espresso-1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      533 2024-04-11 05:24:18.000000 python-espresso-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 04:27:09.086117 python-espresso-1.8.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 12:52:27.000000 python-espresso-1.8.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      955 2024-04-08 12:01:19.000000 python-espresso-1.8.4/tests/test_evaluator.py
+-rw-rw-rw-   0        0        0      958 2024-04-05 13:25:22.000000 python-espresso-1.8.4/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     1316 2024-04-07 06:30:07.000000 python-espresso-1.8.4/tests/test_parser.py
```

### Comparing `python-espresso-1.8.3/LICENSE` & `python-espresso-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/PKG-INFO` & `python-espresso-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.3
+Version: 1.8.4
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.3/README.md` & `python-espresso-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/espresso/Evaluator.py` & `python-espresso-1.8.4/espresso/Evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,9 +120,11 @@
         ret = func_def.func_call(typed_params) if is_variadic else func_def.func_call(*typed_params)
 
         return ret
 
 
     def eval(self, call_stack: Stack) -> any:
         top = call_stack.pop()
+        if not isinstance(top, StackFrame):
+            return top
         result = self._eval_stack_frame(top)
         return result
```

### Comparing `python-espresso-1.8.3/espresso/Lexer.py` & `python-espresso-1.8.4/espresso/Lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/espresso/Parser.py` & `python-espresso-1.8.4/espresso/Parser.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/espresso/utils.py` & `python-espresso-1.8.4/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/python_espresso.egg-info/PKG-INFO` & `python-espresso-1.8.4/python_espresso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-espresso
-Version: 1.8.3
+Version: 1.8.4
 Summary: A tiny type-safe expression parser in Python
 Home-page: https://github.com/aadv1k/python-espresso
 Author: Aadvik P
 Author-email: aadv1k@outlook.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-espresso-1.8.3/setup.py` & `python-espresso-1.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python-espresso",
-    version="1.8.3",
+    version="1.8.4",
     description="A tiny type-safe expression parser in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Aadvik P",
     author_email="aadv1k@outlook.com",
     url="https://github.com/aadv1k/python-espresso",
     license="MIT",
```

### Comparing `python-espresso-1.8.3/tests/test_evaluator.py` & `python-espresso-1.8.4/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/tests/test_lexer.py` & `python-espresso-1.8.4/tests/test_lexer.py`

 * *Files identical despite different names*

### Comparing `python-espresso-1.8.3/tests/test_parser.py` & `python-espresso-1.8.4/tests/test_parser.py`

 * *Files identical despite different names*

