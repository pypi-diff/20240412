# Comparing `tmp/gauge-web-app-steps-0.60.tar.gz` & `tmp/gauge-web-app-steps-0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauge-web-app-steps-0.60.tar", last modified: Fri Apr  5 13:45:12 2024, max compression
+gzip compressed data, was "gauge-web-app-steps-0.61.tar", last modified: Fri Apr 12 14:18:30 2024, max compression
```

## Comparing `gauge-web-app-steps-0.60.tar` & `gauge-web-app-steps-0.61.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.679677 gauge-web-app-steps-0.60/gauge_web_app_steps/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/app_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/bymapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/gauge_web_app_steps/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/common_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/local_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/config/saucelabs_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/browsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/driver/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/element_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/imagepaths.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/keymapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/sauce_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/substitute.py
--rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/gauge_web_app_steps/web_app_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:45:12.679677 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 13:45:12.000000 gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:45:12.683677 gauge-web-app-steps-0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-05 13:45:01.000000 gauge-web-app-steps-0.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:18:30.698294 gauge-web-app-steps-0.61/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-12 14:18:30.698294 gauge-web-app-steps-0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:18:30.694294 gauge-web-app-steps-0.61/gauge_web_app_steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/app_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/bymapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:18:30.694294 gauge-web-app-steps-0.61/gauge_web_app_steps/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/config/common_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/config/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/config/saucelabs_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:18:30.698294 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/driver/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/element_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/imagepaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/keymapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/sauce_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40594 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/gauge_web_app_steps/web_app_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:18:30.694294 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 14:18:30.000000 gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:18:30.698294 gauge-web-app-steps-0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 14:18:20.000000 gauge-web-app-steps-0.61/setup.py
```

### Comparing `gauge-web-app-steps-0.60/LICENCE` & `gauge-web-app-steps-0.61/LICENCE`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/PKG-INFO` & `gauge-web-app-steps-0.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.60
+Version: 0.61
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `gauge-web-app-steps-0.60/README.md` & `gauge-web-app-steps-0.61/README.md`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/app_context.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/app_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 timeout_key = "_timeout"
 
 class AppContext:
     """
     Context objects are created and kept here.
     """
 
-    def __init__(self, ctx: ExecutionContext = None) -> None:
+    def __init__(self, ctx: ExecutionContext = None, suite_id: str = None) -> None:
         """Initiates objects used in the basic steps."""
         if ctx is None:
             # getgauge's loading mechanism might try to instantiate the class before the lib is ready.
             return
         self.report = Report(ctx, config.is_debug_log())
         self._report_driver_options()
         spec : Specification = ctx.specification
-        self.driver = self._create_driver(spec.name)
+        self.driver = self._create_driver(spec.name, suite_id)
         self.image_path = ImagePath(config.get_browser().value, config.is_headless())
         self.images = Images(self.report)
         self.diff_formats = config.get_diff_formats()
         self.mobile = config.get_operating_system().is_mobile()
         self.firefox_page_screenshot_no_scrolling = config.get_browser() == Browser.FIREFOX and config.is_whole_page_screenshot()
 
-    def _create_driver(self, spec_name: str) -> Remote:
-        driver_factory = DriverFactory.create_driver_factory(spec_name)
+    def _create_driver(self, spec_name: str, suite_id: str) -> Remote:
+        driver_factory = DriverFactory.create_driver_factory(spec_name, suite_id)
         return driver_factory.create_driver()
 
     def _report_driver_options(self) -> None:
         operating_system = config.get_operating_system()
         self.report.log(f"platform: {config.get_platform().value}")
         self.report.log(f"operating system: {operating_system}")
         self.report.log(f"operating system version: {config.get_operating_system_version()}")
```

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/bymapper.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/bymapper.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/config/common_config.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/config/common_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/config/local_config.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/config/local_config.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/config/saucelabs_config.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/config/saucelabs_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,18 @@
     return os.environ.get("driver_platform_saucelabs_test_title")
 
 
 def get_build() -> Optional[str]:
     return os.environ.get("driver_platform_saucelabs_build")
 
 
+def is_device_cached() -> bool:
+    return os.environ.get("driver_platform_saucelabs_devicecache", "false").lower() in ('true', '1')
+
+
 def get_sauce_status_address() -> Optional[str]:
     return os.environ.get("SAUCE_STATUS_ADDRESS")
 
 
 def is_sauce_tunnel_active() -> bool:
     return os.environ.get("SAUCE_TUNNEL_ACTIVE", "false").lower() in ('true', '1')
```

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/browsers.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/driver/browsers.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/driver_factory.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/driver/driver_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 class DriverFactory(ABC):
 
     """
     Abstract parent factory for all driver factories.
     """
 
     @staticmethod
-    def create_driver_factory(spec_name: str) -> DriverFactory:
+    def create_driver_factory(spec_name: str, suite_id: str) -> DriverFactory:
         if config.get_platform().is_remote():
-            return SaucelabsDriverFactory(spec_name)
+            return SaucelabsDriverFactory(spec_name, suite_id)
         elif config.get_platform().is_local():
             return LocalDriverFactory()
         else:
             raise RuntimeError("Given driver options are not supported")
 
     @abstractmethod
     def create_driver(self) -> Remote:
@@ -266,16 +266,17 @@
 
 
 class SaucelabsDriverFactory(DriverFactory):
     """
     This factory creates drivers for the remote Saucelabs environment.
     """
 
-    def __init__(self, spec_name: str) -> None:
+    def __init__(self, spec_name: str, suite_id: str) -> None:
         self.spec_name = spec_name
+        self.suite_id = suite_id
 
     def create_driver(self) -> Remote:
         """Creates and returns a driver for https://saucelabs.com/"""
         operating_system = config.get_operating_system()
         if operating_system.is_desktop():
             return self._create_desktop_driver()
         elif operating_system.is_mobile():
@@ -392,8 +393,10 @@
             sauce_options["tunnelName"] = tunnel_name
         custom_test_title = saucelabs_config.get_test_title()
         spec_name = self.spec_name
         sauce_options["name"] = f"{spec_name} - {custom_test_title}" if custom_test_title else spec_name
         build = saucelabs_config.get_build()
         if build:
             sauce_options["build"] = build
+        if saucelabs_config.is_device_cached():
+            sauce_options["cacheId"] = self.suite_id
         return sauce_options
```

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/driver/operating_system.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/driver/operating_system.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/element_lookup.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/element_lookup.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/imagepaths.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/imagepaths.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/images.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/images.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/keymapper.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/keymapper.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/report.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/report.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/sauce_tunnel.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/sauce_tunnel.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/screenshot.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/screenshot.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/selector.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/selector.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/substitute.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/substitute.py`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps/web_app_steps.py` & `gauge-web-app-steps-0.61/gauge_web_app_steps/web_app_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import base64
 import os
 import re
 import time
 import traceback
 import urllib
+from uuid import uuid4
 
 from itertools import filterfalse
 from typing import Tuple
 from getgauge.python import data_store, step, before_spec, after_spec, screenshot, before_suite, after_suite, before_step, ExecutionContext
 from selenium.common.exceptions import JavascriptException, WebDriverException
 from selenium.webdriver import Remote
 from selenium.webdriver.common.action_chains import ActionChains
@@ -33,29 +34,32 @@
 from .substitute import substitute
 
 
 # Repeat an action a number of times before failing
 max_attempts = 12
 basic_auth_key = "_basic_auth"
 error_message_key = "_err_msg"
+suite_id_key = "_suite_id"
 
 @before_suite
 def before_suite_hook() -> None:
     SauceTunnel.start()
+    data_store.suite[suite_id_key] = str(uuid4())
 
 
 @after_suite
 def after_suite_hook() -> None:
     SauceTunnel.terminate()
 
 
 @before_spec
 def before_spec_hook(exe_ctx: ExecutionContext) -> None:
     try:
-        app_ctx = AppContext(exe_ctx)
+        suite_id = data_store.suite[suite_id_key]
+        app_ctx = AppContext(exe_ctx, suite_id)
         data_store.spec[app_context_key] = app_ctx
     except BaseException as e:
         # Gauge swallows some exceptions, so they are handled here
         print(f"An exception occured while instantiating the driver: {e}")
         traceback.print_exception(e)
         raise e
```

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/PKG-INFO` & `gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-web-app-steps
-Version: 0.60
+Version: 0.61
 Summary: Provides basic steps for a Gauge project, that runs tests with Selenium and Appium
 Home-page: https://github.com/IBM/gauge-web-app-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `gauge-web-app-steps-0.60/gauge_web_app_steps.egg-info/SOURCES.txt` & `gauge-web-app-steps-0.61/gauge_web_app_steps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gauge-web-app-steps-0.60/setup.py` & `gauge-web-app-steps-0.61/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     long_description = long_description.replace('./docs/', 'https://github.com/IBM/gauge-web-app-steps/tree/master/docs/')
 
 setup(
     name='gauge-web-app-steps',
-    version='0.60',
+    version='0.61',
     description='Provides basic steps for a Gauge project, that runs tests with Selenium and Appium',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/IBM/gauge-web-app-steps',
     author='Tobias Lehmann',
     author_email='derdualist1@gmail.com',
     license='MIT',
```

