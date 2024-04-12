# Comparing `tmp/saucelabs_visual-0.0.4.tar.gz` & `tmp/saucelabs_visual-0.0.5.tar.gz`

## Comparing `saucelabs_visual-0.0.4.tar` & `saucelabs_visual-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/requirements/build.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/requirements/dev.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/requirements/user.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/client.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/regions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/frameworks/__init__.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/src/saucelabs_visual/frameworks/robot.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/.gitignore
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/README.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/build.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/requirements/user.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/client.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/regions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/__init__.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/robot.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/.gitignore
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/README.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.5/PKG-INFO
```

### Comparing `saucelabs_visual-0.0.4/src/saucelabs_visual/client.py` & `saucelabs_visual-0.0.5/src/saucelabs_visual/client.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.4/src/saucelabs_visual/regions.py` & `saucelabs_visual-0.0.5/src/saucelabs_visual/regions.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.4/src/saucelabs_visual/frameworks/robot.py` & `saucelabs_visual-0.0.5/src/saucelabs_visual/frameworks/robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if literal_type is dict:
             parsed_value = literal
         elif literal_type is bool:
             parsed_value = {} if literal is True else None
 
         return FullPageConfig(
             delay_after_scroll_ms=parsed_value.get('delay_after_scroll_ms'),
-            hide_after_first_scroll=parsed_value.get('delay_after_scroll_ms'),
+            hide_after_first_scroll=parsed_value.get('hide_after_first_scroll'),
         ) if parsed_value is not None else None
 
     @keyword(name="Create Visual Build")
     def create_visual_build(
             # Params 'duplicated' here, so we get type casting and named parameters provided by
             # Robot Framework for free.
             self,
```

### Comparing `saucelabs_visual-0.0.4/.gitignore` & `saucelabs_visual-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.4/pyproject.toml` & `saucelabs_visual-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saucelabs_visual"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python bindings for Sauce Labs Visual"
 dependencies=[
     "aiohttp",
     "gql",
 ]
 readme = "README.md"
```

