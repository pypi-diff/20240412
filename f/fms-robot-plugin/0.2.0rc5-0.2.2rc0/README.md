# Comparing `tmp/fms_robot_plugin-0.2.0rc5.tar.gz` & `tmp/fms_robot_plugin-0.2.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.2.0rc5.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.2.2rc0.tar", max compression
```

## Comparing `fms_robot_plugin-0.2.0rc5.tar` & `fms_robot_plugin-0.2.2rc0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       26 2024-03-22 10:09:19.311183 fms_robot_plugin-0.2.0rc5/README.md
--rw-r--r--   0        0        0       49 2024-03-22 10:09:19.315183 fms_robot_plugin-0.2.0rc5/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1824 2024-03-22 10:09:19.315183 fms_robot_plugin-0.2.0rc5/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     8727 2024-03-22 10:09:19.315183 fms_robot_plugin-0.2.0rc5/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3161 2024-03-22 10:09:19.315183 fms_robot_plugin-0.2.0rc5/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-03-22 10:09:19.315183 fms_robot_plugin-0.2.0rc5/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.0rc5/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.0rc5/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-04-12 08:08:58.136799 fms_robot_plugin-0.2.2rc0/README.md
+-rw-r--r--   0        0        0       49 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     8727 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3168 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/PKG-INFO
```

### Comparing `fms_robot_plugin-0.2.0rc5/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.0rc5/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.0rc5/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     angle_max: float
     angle_increment: float
     time_increment: float
     scan_time: float
     range_min: float
     range_max: float
     ranges: list[float | None]
-    intensities: list[float]
+    intensities: list[float | None]
 
 
 class Pose(BaseModel):
     """
     Based on ROS geometry_msgs/Pose
     """
```

### Comparing `fms_robot_plugin-0.2.0rc5/pyproject.toml` & `fms_robot_plugin-0.2.2rc0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.2.0rc5"
+version = "0.2.2rc0"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.2.0rc5/setup.py` & `fms_robot_plugin-0.2.2rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.2.0rc5',
+    'version': '0.2.2rc0',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

