# Comparing `tmp/elkoep-mqtt-0.2.27.tar.gz` & `tmp/elkoep-mqtt-0.2.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkoep-mqtt-0.2.27.tar", last modified: Thu Apr 11 12:02:37 2024, max compression
+gzip compressed data, was "elkoep-mqtt-0.2.28.tar", last modified: Fri Apr 12 13:45:26 2024, max compression
```

## Comparing `elkoep-mqtt-0.2.27.tar` & `elkoep-mqtt-0.2.28.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 12:02:37.000000 elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/inelsmqtt/
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/inelsmqtt/devices/
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/inelsmqtt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 12:02:37.241004 elkoep-mqtt-0.2.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:02:37.237004 elkoep-mqtt-0.2.27/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/devices/device_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/discovery_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/inels_mqtt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-11 12:02:30.000000 elkoep-mqtt-0.2.27/tests/online_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 13:45:26.000000 elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.794256 elkoep-mqtt-0.2.28/inelsmqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22709 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.794256 elkoep-mqtt-0.2.28/inelsmqtt/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105922 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/inelsmqtt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:45:26.798256 elkoep-mqtt-0.2.28/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/devices/device_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/discovery_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/inels_mqtt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-12 13:45:20.000000 elkoep-mqtt-0.2.28/tests/online_test.py
```

### Comparing `elkoep-mqtt-0.2.27/LICENSE` & `elkoep-mqtt-0.2.28/LICENSE`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/PKG-INFO` & `elkoep-mqtt-0.2.28/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.27
+Version: 0.2.28
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep-mqtt-0.2.27/README.md` & `elkoep-mqtt-0.2.28/README.md`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/PKG-INFO` & `elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkoep-mqtt
-Version: 0.2.27
+Version: 0.2.28
 Summary: Python library for iNELS mqtt protocol
 Home-page: https://github.com/epdevlab/elkoep-mqtt
 Author: Elko EP s.r.o.
 Author-email: epdevlab@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elkoep-mqtt-0.2.27/elkoep_mqtt.egg-info/SOURCES.txt` & `elkoep-mqtt-0.2.28/elkoep_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/__init__.py` & `elkoep-mqtt-0.2.28/inelsmqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/config.py` & `elkoep-mqtt-0.2.28/inelsmqtt/config.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/const.py` & `elkoep-mqtt-0.2.28/inelsmqtt/const.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/devices/__init__.py` & `elkoep-mqtt-0.2.28/inelsmqtt/devices/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,16 +136,17 @@
     def is_available(self) -> bool:
         """Get info about availability of device
 
         Returns:
             bool: True/False
         """
         gw = self.__mqtt.messages().get(self._Device__gw_connected_topic)
-        if not GW_CONNECTED.get(gw):
-            return False
+        if gw is not None:
+            if not GW_CONNECTED.get(gw):
+                return False
 
         val = self.__mqtt.messages().get(self._Device__connected_topic)
         if isinstance(val, (bytes, bytearray)):
             val = val.decode()
 
         return DEVICE_CONNECTED.get(val) and self.__values is not None and self.__values._DeviceValue__ha_value is not None
```

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/devices/switch.py` & `elkoep-mqtt-0.2.28/inelsmqtt/devices/switch.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/discovery.py` & `elkoep-mqtt-0.2.28/inelsmqtt/discovery.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/mqtt_client.py` & `elkoep-mqtt-0.2.28/inelsmqtt/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/inelsmqtt/util.py` & `elkoep-mqtt-0.2.28/inelsmqtt/util.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/setup.py` & `elkoep-mqtt-0.2.28/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup script for elkoep-mqtt package."""
 from setuptools import setup, find_packages
 
 setup(
     name="elkoep-mqtt",
-    version="0.2.27",
+    version="0.2.28",
     url="https://github.com/epdevlab/elkoep-mqtt",
     license="MIT",
     author="Elko EP s.r.o.",
     author_email="epdevlab@gmail.com",
     description="Python library for iNELS mqtt protocol",
     keywords=["iNels", "Elko EP", "Home assistant integration"],
     long_description_content_type="text/markdown",
```

### Comparing `elkoep-mqtt-0.2.27/tests/const.py` & `elkoep-mqtt-0.2.28/tests/const.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/tests/devices/device_test.py` & `elkoep-mqtt-0.2.28/tests/devices/device_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/tests/discovery_test.py` & `elkoep-mqtt-0.2.28/tests/discovery_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/tests/inels_mqtt_test.py` & `elkoep-mqtt-0.2.28/tests/inels_mqtt_test.py`

 * *Files identical despite different names*

### Comparing `elkoep-mqtt-0.2.27/tests/online_test.py` & `elkoep-mqtt-0.2.28/tests/online_test.py`

 * *Files identical despite different names*

