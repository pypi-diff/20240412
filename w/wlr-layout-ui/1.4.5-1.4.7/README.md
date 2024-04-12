# Comparing `tmp/wlr_layout_ui-1.4.5.tar.gz` & `tmp/wlr_layout_ui-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.4.5.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.4.7.tar", max compression
```

## Comparing `wlr_layout_ui-1.4.5.tar` & `wlr_layout_ui-1.4.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/README.md
--rw-r--r--   0        0        0      636 2024-04-01 15:31:36.231423 wlr_layout_ui-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.4.5/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4304 2023-12-20 15:42:38.511785 wlr_layout_ui-1.4.5/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    21897 2024-04-01 15:30:20.126238 wlr_layout_ui-1.4.5/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.4.5/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5449 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2023-10-31 19:56:35.664588 wlr_layout_ui-1.4.5/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4496 2024-03-30 19:09:30.198398 wlr_layout_ui-1.4.5/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.5/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 wlr_layout_ui-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.4.7/LICENSE
+-rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/README.md
+-rw-r--r--   0        0        0      652 2024-04-12 17:31:06.974882 wlr_layout_ui-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.4.7/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4304 2023-12-20 15:42:38.511785 wlr_layout_ui-1.4.7/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    21897 2024-04-01 15:30:20.126238 wlr_layout_ui-1.4.7/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.4.7/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5475 2024-04-08 16:08:47.075411 wlr_layout_ui-1.4.7/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.4.7/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4496 2024-03-30 19:09:30.198398 wlr_layout_ui-1.4.7/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 wlr_layout_ui-1.4.7/PKG-INFO
```

### Comparing `wlr_layout_ui-1.4.5/README.md` & `wlr_layout_ui-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/pyproject.toml` & `wlr_layout_ui-1.4.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.4.5"
+version = "1.4.7"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
+license = "MIT"
 
 [tool.poetry.scripts]
 wlrlui = 'wlr_layout_ui:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyglet = "^2.0.0"
```

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/gui.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/screens.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,19 +75,20 @@
 
 def load():
 
     if displayInfo:
         displayInfo.clear()
 
     try:
-        v = json.loads(subprocess.getoutput("hyprctl -j version"))["tag"]
-        good_v = (37, 38, 39)
-        new_hyprland = any(v.startswith("v0.%d" % x) for x in good_v) or (
-            not v.startswith("v0.2") and not v.startswith("v0.1")
-        )
+        version = json.loads(subprocess.getoutput("hyprctl -j version"))["tag"]
+        version = version[1:].split(".")
+        major = int(version[0])
+        minor = int(version[1])
+        _patch = int(version[2])
+        new_hyprland = major == 0 and minor >= 37 or major > 0
     except (KeyError, json.JSONDecodeError):
         new_hyprland = False
 
     if new_hyprland:
         config["hyprland"] = True
         load_from_hyprctl()
         return
```

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.4.7/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.5/PKG-INFO` & `wlr_layout_ui-1.4.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.4.5
+Version: 1.4.7
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
+License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyglet (>=2.0.0,<3.0.0)
```

