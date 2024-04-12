# Comparing `tmp/mosaik-3.3.0b1.tar.gz` & `tmp/mosaik-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-3.3.0b1.tar", last modified: Wed Jan 24 10:18:03 2024, max compression
+gzip compressed data, was "mosaik-3.3.1.tar", last modified: Fri Apr 12 11:40:34 2024, max compression
```

## Comparing `mosaik-3.3.0b1.tar` & `mosaik-3.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:18:03.402446 mosaik-3.3.0b1/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)    24436 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    16914 2024-01-24 10:18:03.402446 mosaik-3.3.0b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3555 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:18:03.397446 mosaik-3.3.0b1/mosaik/
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/adapters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:18:03.399446 mosaik-3.3.0b1/mosaik/basic_simulators/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/basic_simulators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/basic_simulators/input_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/basic_simulators/output_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/dense_time.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/in_or_out_set.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/internal_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     7745 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/proxies.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    40030 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    17016 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    25908 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/simmanager.py
--rw-rw-rw-   0 root         (0) root         (0)    18934 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/mosaik/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:18:03.402446 mosaik-3.3.0b1/mosaik.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16914 2024-01-24 10:18:03.000000 mosaik-3.3.0b1/mosaik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      929 2024-01-24 10:18:03.000000 mosaik-3.3.0b1/mosaik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 10:18:03.000000 mosaik-3.3.0b1/mosaik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-01-24 10:18:03.000000 mosaik-3.3.0b1/mosaik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-24 10:18:03.000000 mosaik-3.3.0b1/mosaik.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-01-24 10:18:03.403446 mosaik-3.3.0b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1767 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 10:18:03.401446 mosaik-3.3.0b1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2255 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_attr_specification.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_basic_simulators.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_benchmarks.py
--rw-rw-rw-   0 root         (0) root         (0)      969 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_dense_time.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7495 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)    14828 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)    14317 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    19452 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_simmanager.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_tutorial.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-01-24 10:17:52.000000 mosaik-3.3.0b1/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:40:34.681325 mosaik-3.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-08 13:12:09.000000 mosaik-3.3.1/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)    24436 2024-04-03 06:59:03.000000 mosaik-3.3.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    17073 2024-04-12 11:40:34.681325 mosaik-3.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2024-04-08 13:12:09.000000 mosaik-3.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:40:34.673325 mosaik-3.3.1/mosaik/
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/_debug.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/adapters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:40:34.677325 mosaik-3.3.1/mosaik/basic_simulators/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-03 06:59:03.000000 mosaik-3.3.1/mosaik/basic_simulators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/basic_simulators/input_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/basic_simulators/output_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/in_or_out_set.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/internal_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     7745 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/proxies.py
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 06:59:03.000000 mosaik-3.3.1/mosaik/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    44209 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)    17830 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    27130 2024-04-12 11:40:16.000000 mosaik-3.3.1/mosaik/simmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3235 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/tiered_time.py
+-rw-rw-rw-   0 root         (0) root         (0)    20903 2024-04-08 13:12:09.000000 mosaik-3.3.1/mosaik/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:40:34.681325 mosaik-3.3.1/mosaik.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17073 2024-04-12 11:40:34.000000 mosaik-3.3.1/mosaik.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2024-04-12 11:40:34.000000 mosaik-3.3.1/mosaik.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 11:40:34.000000 mosaik-3.3.1/mosaik.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-04-12 11:40:34.000000 mosaik-3.3.1/mosaik.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-12 11:40:34.000000 mosaik-3.3.1/mosaik.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2024-04-12 11:40:16.000000 mosaik-3.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-12 11:40:34.681325 mosaik-3.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2024-04-08 13:12:09.000000 mosaik-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:40:34.681325 mosaik-3.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2255 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5307 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_attr_specification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_basic_simulators.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-04-03 06:59:03.000000 mosaik-3.3.1/tests/test_benchmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-03 06:59:03.000000 mosaik-3.3.1/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)    15735 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)    16921 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    20527 2024-04-12 11:40:16.000000 mosaik-3.3.1/tests/test_simmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_tiered_time.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-08 13:12:09.000000 mosaik-3.3.1/tests/test_tutorial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-03 06:59:03.000000 mosaik-3.3.1/tests/test_util.py
```

### Comparing `mosaik-3.3.0b1/LICENSE.txt` & `mosaik-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/PKG-INFO` & `mosaik-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik
-Version: 3.3.0b1
+Version: 3.3.1
 Summary: Mosaik is a flexible Smart-Grid co-simulation framework.
 Home-page: https://mosaik.offis.de
 Author: mosaik development team
 Author-email: mosaik@offis.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -34,16 +34,14 @@
 
 Mosaik is a simulation compositor for Smart Grid simulations.
 
 It lets you re-use existing simulators and couple them to simulate large-scale
 Smart Grid scenarios. Mosaik offers powerful mechanisms to specify and compose
 these scenarios.
 
-Version: 3.3.0.b1
-
 License: LGPL
 
 Example
 -------
 
 A simple demo scenario with mosaik::
 
@@ -115,19 +113,20 @@
 You have a question, a feature request or want to generally discuss the amazing 
 possibilities with co-simulation and mosaik? We are curious to hear from you! 
 Join us on `GitHub Discussions <https://github.com/orgs/OFFIS-mosaik/discussions>`_.
 
 Changelog
 =========
 
-3.3.0 - 2024-01-17
--------------------
+3.3.0 - 2024-04-08
+------------------
 - [NEW] A simulator can now be connected to itself if the connection is weak or time_shifted (https://gitlab.com/mosaik/mosaik/-/issues/156)
 - [NEW] mosaik now provides a couple of basic simulators (https://gitlab.com/mosaik/mosaik/-/issues/192 , https://mosaik.readthedocs.io/en/latest/ecosystem/index.html#mosaik-basic-simulators)
 - [NEW] Simulators can return extra_info for their entities to be used in scenario script (https://gitlab.com/mosaik/mosaik/-/issues/197)
+- [NEW] Simulators now can (and potentially must) be grouped in a scenario script for more fine-grained control over same-time loops (https://gitlab.com/mosaik/mosaik/-/issues/215)
 - [IMPROVEMENT] Internal rework and refactoring of the time handling in mosaik (https://gitlab.com/mosaik/mosaik/-/issues/162)
 
 
 3.2.0 - 2023-08-31
 ------------------
 - [NEW] Visualizations for the simulation debug information (https://gitlab.com/mosaik/mosaik/-/issues/173)
 - [NEW] Allow to open a new console for simulator (https://gitlab.com/mosaik/mosaik/-/issues/84)
```

### Comparing `mosaik-3.3.0b1/README.rst` & `mosaik-3.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 Mosaik is a simulation compositor for Smart Grid simulations.
 
 It lets you re-use existing simulators and couple them to simulate large-scale
 Smart Grid scenarios. Mosaik offers powerful mechanisms to specify and compose
 these scenarios.
 
-Version: 3.3.0.b1
-
 License: LGPL
 
 Example
 -------
 
 A simple demo scenario with mosaik::
```

### Comparing `mosaik-3.3.0b1/mosaik/adapters.py` & `mosaik-3.3.1/mosaik/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # the mosaik code to use it. Then add a V(new)toV(old)Adapter class in
 # this file which turns adapts requests conforming to the new version
 # into requests conforming to the old version. Also add a version
 # check to ``init_and_get_adapter`` that wraps older simulators in
 # this new adapter.
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 import warnings
-from loguru import logger
+from loguru import logger  # noqa: F401  # type: ignore
 
 from mosaik_api_v3.types import Meta, SimId
 
 from mosaik.exceptions import ScenarioError
 from mosaik.proxies import BaseProxy, Proxy
 
 
@@ -111,48 +111,48 @@
     def __init__(self, out: Proxy):
         self._out = out
 
     @property
     def meta(self) -> Meta:
         return self._out.meta
 
-    async def send(self, request):
+    async def send(self, request: Any):
         return await self._out.send(request)
 
     async def stop(self):
         return await self._out.stop()
 
 
 class V3ToV2Adapter(Adapter):
     """API changes:
     - ``init`` is now supplied with the ``time_resolution`` (as a kwarg)
       (but this is handled in BaseConnection)
     - ``step`` is now supplied with ``max_advance`` (as an arg)
     """
-    async def send(self, request):
+    async def send(self, request: Any):
         try:
             func_name, args, kwargs = request
             if func_name == "step":
                 request = ("step", args[0:2], kwargs)
-        except:
+        except ValueError:
             pass
         return await self._out.send(request)
 
     @property
     def meta(self) -> Meta:
         self._out.meta.setdefault("type", "time-based")
         return self._out.meta
 
 
 class V2ToV1Adapter(Adapter):
     """API changes:
     - ``setup_done`` function was added to simulators
     """
-    async def send(self, request):
+    async def send(self, request: Any):
         try:
-            func_name, args, kwargs = request
+            func_name, _args, _kwargs = request
             if func_name == "setup_done":
                 return None
-        except:
+        except ValueError:
             pass
 
         return await self._out.send(request)
```

### Comparing `mosaik-3.3.0b1/mosaik/basic_simulators/input_simulator.py` & `mosaik-3.3.1/mosaik/basic_simulators/input_simulator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Callable, Dict, List
+from typing_extensions import override
 import mosaik_api_v3
 from mosaik_api_v3.types import (
     CreateResult,
     InputData,
     Meta,
     ModelName,
     OutputData,
@@ -32,34 +33,49 @@
     "extra_methods": [],
 }
 
 
 class InputSimulator(mosaik_api_v3.Simulator):
     """
     This simulator gives a steady input to a connected simulator.
-    This input can either be an constant numerical value or a custom
-    function. It is passed along as parameter in the :meth:`create()` method of this simulator.
-    Using the :meth:`get_data()` function, the generated values can be retrieved.
+    This input can either be an constant value or given by a custom
+    function based on the current time.
+
+    When starting the simulator, a custom step size may be provided
+    using the `step_size` parameter. The default is 1.
+
+    When creating a `Constant` entity, the constant must be passed as
+    the parameter `constant`.
+
+    When creating a `Function` entity, a function should be passed as
+    the `function` parameter. This function should take the current
+    mosaik time and return the desired value. This type of entity only
+    works when the simulator is started using the `"python"` method.
+
+    In either case, the entity will produce its output on the *value*
+    attribute.
     """
 
     step_size: int
     functions: Dict[str, Callable[[Time], Any]]
     constants: Dict[str, Any]
 
     def __init__(self):
         super().__init__(META)
         self.functions = {}
         self.constants = {}
         self.step_size = 1
         self.time = 0
 
+    @override
     def init(self, sid: SimId, time_resolution: float = 1, step_size: int = 1) -> Meta:
         self.step_size = step_size
         return self.meta
 
+    @override
     def create(
         self, num: int, model: ModelName, **model_params: Any
     ) -> List[CreateResult]:
         new_entities: List[CreateResult] = []
         if model == FUNCTION_KEY:
             for i in range(len(self.functions), len(self.functions) + num):
                 new_entities.append(
@@ -85,19 +101,21 @@
     def create_constant_entity(
         self, id: int, model: str, constant: Any
     ) -> CreateResult:
         eid = f"{CONSTANT_KEY}-{id}"
         self.constants[eid] = constant
         return {"eid": eid, "type": model}
 
+    @override
     def step(self, time: Time, inputs: InputData, max_advance: Time) -> Time:
         assert inputs == {}
         self.time = time
         return time + self.step_size
 
+    @override
     def get_data(self, outputs: OutputRequest) -> OutputData:
         data: OutputData = {}
         for eid in outputs:
             if CONSTANT_KEY in eid:
                 data[eid] = {"value": self.constants[eid]}
             else:
                 data[eid] = {"value": self.functions[eid](self.time)}
```

### Comparing `mosaik-3.3.0b1/mosaik/basic_simulators/output_simulator.py` & `mosaik-3.3.1/mosaik/basic_simulators/output_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class OutputSimulator(mosaik_api_v3.Simulator):
     """
     This simulator takes the input it is given and writes it into a python dictionary
     where the keys are the timestamps of the input and the values are the inputs values.
 
-    The dictionary can be retrieved using the :meth:`get_dict()` method.
+    The dictionary can be retrieved using the :meth:`get_dict` method.
     """
 
     entities: Dict[str, Dict[Time, Any]]
 
     def __init__(self):
         super().__init__(META)
         self.entities = {}  # Maps EIDs to model instances/entities
@@ -55,15 +55,14 @@
             model_instance = {}
             eid = f"{model}-{i}"
             self.entities[eid] = model_instance
             entities.append({"eid": eid, "type": model})
         return entities
 
     def step(self, time: Time, inputs:InputData, max_advance: Time):
-        print(inputs)
         for receiver, input in inputs.items():
             self.entities[receiver][time] = deepcopy(input) 
 
     def get_data(self, outputs: OutputRequest) -> OutputData:
         raise mosaik.exceptions.ScenarioError(
             "This function is not supposed to be used in this simulator. "
             "Use this simulator for input data only."
```

### Comparing `mosaik-3.3.0b1/mosaik/in_or_out_set.py` & `mosaik-3.3.1/mosaik/in_or_out_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
 from typing import (
+    Any,
     FrozenSet,
     Generic,
     Iterable,
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
-from typing_extensions import Self, TypeAlias
+from typing_extensions import TypeAlias
 
 E = TypeVar("E")
 
 
 class OutSet(Generic[E]):
     """An OutSet[E] represents all elements of the type E except for a finite number.
 
@@ -24,46 +26,51 @@
     """
 
     _set: FrozenSet[E]
 
     def __init__(self, elems: Iterable[E] = ()):
         self._set = frozenset(elems)
 
-    def __sub__(self, other: Union[FrozenSet[E], Self]) -> Union[Self, FrozenSet[E]]:
+    def __sub__(self, other: InOrOutSet[E]) -> InOrOutSet[E]:
         if isinstance(other, OutSet):
             return other._set - self._set
         else:
             return OutSet(self._set | other)
 
     def __rsub__(self, rother: FrozenSet[E]) -> FrozenSet[E]:
         return rother & self._set
 
-    def __and__(self, other: Union[FrozenSet[E], Self]) -> Union[Self, FrozenSet[E]]:
+    def __and__(self, other: InOrOutSet[E]) -> InOrOutSet[E]:
         if isinstance(other, OutSet):
             return OutSet(self._set | other._set)
         else:
             return other - self._set
 
     def __rand__(self, rother: FrozenSet[E]) -> FrozenSet[E]:
         return rother - self._set
 
-    def __or__(self, other: Union[FrozenSet[E], Self]) -> Self:
+    def __or__(self, other: InOrOutSet[E]) -> OutSet[E]:
         if isinstance(other, OutSet):
             return OutSet(self._set & other._set)
         else:
             return OutSet(self._set - other)
 
-    def __ror__(self, rother: FrozenSet[E]) -> Self:
+    def __ror__(self, rother: FrozenSet[E]) -> OutSet[E]:
         return OutSet(self._set - rother)
 
     def __contains__(self, item: E) -> bool:
         return item not in self._set
 
-    def __eq__(self, other: Self):
-        return self._set == other._set
+    def __eq__(self, other: Any):
+        if not isinstance(other, OutSet):
+            return False
+        return self._set == other._set  # type: ignore  (Pyright does not know E here)
+
+    def __str__(self):
+        return f"OutSet({{{', '.join(self._set)}}})"
 
 
 InOrOutSet: TypeAlias = Union[FrozenSet[E], OutSet[E]]
 """A InOrOutSet is either a FrozenSet or an OutSet. This means
 that it can represent either
 - a finite number of elements of the type E or
 - all but a finite number of element of the type E.
@@ -102,20 +109,23 @@
         else:
             raise missing_value_error
 
     if part_b is None:
         part_b = union - part_a
 
     if not part_a & part_b == frozenset():
-        raise ValueError(f"{part_a_name} and {part_b_name} are not disjoint")
+        raise ValueError(
+            f"{part_a_name} ({part_a}) and {part_b_name} ({part_b}) are not disjoint"
+        )
 
     if not union == (part_a | part_b):
         raise ValueError(
-            f"{part_a_name} and {part_b_name} must be subsets of {union_name}, "
-            f"and they must have {union_name} as their union if both given"
+            f"{part_a_name} ({part_a}) and {part_b_name} ({part_b}) must be subsets "
+            f"of {union_name} ({union}), and they must have {union_name} as their "
+            f"union if both given"
         )
 
     return part_a, part_b
 
 
 def wrap_set(set: Union[Iterable[E], OutSet[E], None]) -> Optional[InOrOutSet[E]]:
     """Wrap an iterable or OutSet, resulting in an InOrOutSet. Pass
```

### Comparing `mosaik-3.3.0b1/mosaik/internal_util.py` & `mosaik-3.3.1/mosaik/internal_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Callable, Dict
 from typing_extensions import TypeVar
 
+from mosaik._version import __version__
+
 K = TypeVar("K")
 V = TypeVar("V")
 
 
 def recursive_merge_existing(
     merger: Callable[[V, V], V],
     target: Dict[K, V],
@@ -23,7 +25,11 @@
 ) -> Dict[K, V]:
     for k, v in other.items():
         if k in target:
             target[k] = merger(target[k], v)
         else:
             target[k] = v
     return target
+
+
+def doc_link(page: str, anchor: str) -> str:
+    return f"https://mosaik.readthedocs.io/en/{__version__}/{page}.html#{anchor}"
```

### Comparing `mosaik-3.3.0b1/mosaik/proxies.py` & `mosaik-3.3.1/mosaik/proxies.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/mosaik/scenario.py` & `mosaik-3.3.1/mosaik/scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,63 +7,63 @@
 a :class:`ModelMock`) via which the user can instantiate model instances
 (*entities*). The method :meth:`World.run()` finally starts the simulation.
 """
 from __future__ import annotations
 
 import asyncio
 from collections import defaultdict
+import contextlib
 from copy import copy
+from dataclasses import dataclass
 import itertools
 from loguru import logger
+from mosaik_api_v3 import OutputData, OutputRequest
 import networkx
 from tqdm import tqdm
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     FrozenSet,
     Iterable,
     List,
+    NoReturn,
     Optional,
     Set,
     Tuple,
+    TypeVar,
     Union,
 )
 import warnings
-from typing_extensions import Literal, TypedDict
+from typing_extensions import Literal, TypeAlias, TypedDict
 
-from mosaik_api_v3.connection import Channel
 from mosaik_api_v3.types import Attr, CreateResult, EntityId, FullId, ModelDescription, ModelName, SimId
 
 from mosaik import simmanager
-from mosaik.dense_time import DenseTime
+from mosaik.internal_util import doc_link
 from mosaik.proxies import Proxy
-from mosaik.simmanager import SimRunner
+from mosaik.simmanager import SimRunner, MosaikConfigTotal
 from mosaik import scheduler
 from mosaik.exceptions import ScenarioError, SimulationError
 from mosaik.in_or_out_set import OutSet, InOrOutSet, parse_set_triple, wrap_set
+from mosaik.tiered_time import TieredInterval, TieredTime
 
+if TYPE_CHECKING:
+    from _typeshed import SupportsRichComparison
 
 class MosaikConfig(TypedDict, total=False):
-    addr: Tuple[str, int]
+    addr: Tuple[str, int | None]
     start_timeout: float
     stop_timeout: float
 
-class _MosaikConfigTotal(TypedDict):
-    """A total version for :cls:`MosaikConfig` for internal use.
-    """
-
-    addr: Tuple[str, int]
-    start_timeout: float
-    stop_timeout: float
-
-base_config: _MosaikConfigTotal = {
-    'addr': ('127.0.0.1', 5555),
-    'start_timeout': 10,  # seconds
-    'stop_timeout': 10,  # seconds
+base_config: MosaikConfigTotal = {
+    "addr": ("127.0.0.1", None),
+    "start_timeout": 10,  # seconds
+    "stop_timeout": 10,  # seconds
 }
 
 FULL_ID = simmanager.FULL_ID
 
 SENTINEL = object()
 """Sentinel for initial data call (we can't use None as the user might
 want to supply that value.)
@@ -75,14 +75,18 @@
     """The environment variables to set for this simulator."""
     cwd: str
     """The current working directory for this simulator."""
     api_version: str
     """The API version of the connected simulator. Set this to suppress
     warnings about this simulator being outdated.
     """
+    posix: bool
+    """Whether to split the given shell command using POSIX rules.
+    (Default: ``False`` on Windows, ``True`` otherwise.)
+    """
 
 
 class PythonModel(ModelOptionals):
     python: str
     """The Simulator subclass for this simulator, encoded as a string
     `module_name:ClassName`."""
 
@@ -95,15 +99,68 @@
 class CmdModel(ModelOptionals):
     cmd: str
     """The command to start this simulator. String %(python)s will be replaced
     by the python command used to start this scenario, %(addr)s will be replaced
     by the `host:port` combination to which the simulator should connect."""
 
 
-SimConfig = Dict[str, Union[PythonModel, ConnectModel, CmdModel]]
+SimConfig: TypeAlias = Dict[str, Union[PythonModel, ConnectModel, CmdModel]]
+"""Description of all the simulators you intend to use in your
+simulation.
+"""
+
+
+@dataclass
+class SimGroup:
+    parent: SimGroup | None
+
+    @property
+    def depth(self) -> int:
+        if not self.parent:
+            return 1
+        return self.parent.depth + 1
+
+
+def group_path(src: SimGroup, dest: SimGroup) -> Tuple[int, int, SimGroup]:
+    src_groups = [src]
+    while src.parent:
+        src = src.parent
+        src_groups.append(src)
+    
+    descent = 0
+    while True:
+        try:
+            ascent = src_groups.index(dest)
+            return (ascent, descent, dest)
+        except ValueError:
+            if not dest.parent:
+                raise ValueError("no joint parent")
+            dest = dest.parent
+            descent += 1
+
+
+def connect_interval(src_group: SimGroup, dest_group: SimGroup, time_shifted: int = 0, weak: int = 0):
+    ascent, _, common_group = group_path(src_group, dest_group)
+
+    pre_length = src_group.depth
+    cutoff = pre_length - ascent
+    list_tiers = [0] * dest_group.depth
+    if weak and not common_group.parent:
+        raise ScenarioError(
+            "Weak connections may only be used in groups. This is new in mosaik 3.3. "
+            "For more information, see "
+            f"{doc_link('scenario-definition', 'weak-connections')}."
+        )
+    if time_shifted:
+        list_tiers[0] = time_shifted
+    if weak:
+        assert cutoff >= 2
+        list_tiers[cutoff - 1] = weak
+    return TieredInterval(*list_tiers, cutoff=cutoff, pre_length=pre_length)
+
 
 
 class World(object):
     """
     The world holds all data required to specify and run the scenario.
 
     It provides a method to start a simulator process (:meth:`start()`) and
@@ -128,18 +185,21 @@
 
     If *execution_graph* is set to ``True``, an execution graph will be created
     during the simulation. This may be useful for debugging and testing. Note,
     that this increases the memory consumption and simulation time.
     """
 
     sim_config: SimConfig
-    config: _MosaikConfigTotal
-    until: int
+    """The config dictionary that tells mosaik how to start a simulator.
+    """
+    config: MosaikConfigTotal
+    """The config dictionary for general mosaik settings."""
+    until: int  # type: ignore  # set in run
     """The time until which this simulation will run."""
-    rt_factor: Optional[float]
+    rt_factor: Optional[float]  # type: ignore  # set in run
     """The number of real-time seconds corresponding to one mosaik step."""
 
     time_resolution: float
     """The number of seconds that correspond to one mosaik time step in
     this situation. The default value is 1.0, meaning that one integer
     step corresponds to one second simulated time.
     """
@@ -150,94 +210,85 @@
     to converge.
     """
 
     sim_progress: float
     """The progress of the entire simulation (in percent)."""
     use_cache: bool
     loop: asyncio.AbstractEventLoop
-    incoming_connections_queue: asyncio.Queue[Channel]
     sims: Dict[SimId, simmanager.SimRunner]
     """A dictionary of already started simulators instances."""
     _sim_ids: Dict[ModelName, itertools.count[int]]
 
+    main_group: SimGroup
+    current_group: SimGroup
+
     entity_graph: networkx.Graph[FullId]
+    """The :class:`graph <networkx.Graph>` of related entities.
+    Nodes are ``(sid, eid)`` tuples. Each note has an attribute
+    *entity* with an :class:`Entity`.
+    """
+
+    tqdm: tqdm[NoReturn]  # type: ignore  # set in run
+    """The tqdm progress bar for the total progress."""
 
     def __init__(
         self,
         sim_config: SimConfig,
         mosaik_config: Optional[MosaikConfig] = None,
         time_resolution: float = 1.,
         debug: bool = False,
         cache: bool = True,
         max_loop_iterations: int = 100,
         asyncio_loop: Optional[asyncio.AbstractEventLoop] = None,
     ):
         self.sim_config = sim_config
-        """The config dictionary that tells mosaik how to start a simulator."""
 
         self.config = copy(base_config)
-        """The config dictionary for general mosaik settings."""
         if mosaik_config:
             self.config.update(mosaik_config)
 
         self.sims = {}
+        self.main_group = SimGroup(parent=None)
+        self.current_group = self.main_group
+
         self.time_resolution = time_resolution
         self.max_loop_iterations = max_loop_iterations
 
         if asyncio_loop:
             self.loop = asyncio_loop
         else:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
 
-        # When simulators are started using `cmd`, they will connect
-        # back to mosaik using a TCP connection. Here we start the
-        # server that accepts these connections. Whenever an external
-        # simulator connects, a Channel is created from the 
-        # (reader, writer) pair and written to the 
-        # incoming_connections_queue so that the function starting the
-        # simulator can .get() the connection information.
-        async def setup_queue() -> asyncio.Queue[Channel]:
-            return asyncio.Queue()
-        self.incoming_connections_queue = self.loop.run_until_complete(setup_queue())
-
-        async def connected_cb(reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
-            await self.incoming_connections_queue.put(Channel(reader, writer))
-
-        self.server = self.loop.run_until_complete(
-            asyncio.start_server(
-                connected_cb,
-                self.config['addr'][0],
-                self.config['addr'][1],
-            )
-        )
-
         self.entity_graph = networkx.Graph()
-        """The :func:`graph <networkx.Graph>` of related entities. Nodes are
-        ``(sid, eid)`` tuples.  Each note has an attribute *entity* with an
-        :class:`Entity`."""
-
         self.sim_progress = 0
-        """Progress of the current simulation (in percent)."""
 
         self._debug = False
         if debug:
             logger.warning(
                 "You are running your simulation in debug mode. This can lead to "
                 "significant slow-downs, as it will create a graph of the entire "
                 "execution. Only use this mode if you intend to analyze the execution "
                 "graph afterwards."
             )
             self._debug = True
-            self.execution_graph: networkx.DiGraph[Tuple[SimId, DenseTime]] = networkx.DiGraph()
+            self.execution_graph: networkx.DiGraph[Tuple[SimId, TieredTime]] = networkx.DiGraph()
 
         # Contains ID counters for each simulator type.
         self._sim_ids = defaultdict(itertools.count)
         self.use_cache = cache
 
+    @contextlib.contextmanager
+    def group(self):
+        parent_group = self.current_group
+        new_group = SimGroup(parent=parent_group)
+        self.current_group = new_group
+        yield
+        self.current_group = parent_group
+
     def start(
         self,
         sim_name: str,
         sim_id: Optional[SimId] = None,
         **sim_params: Any,
     ) -> ModelFactory:
         """
@@ -258,16 +309,16 @@
             sim_id=sim_id,
         )
         proxy = self.loop.run_until_complete(
             simmanager.start(self, sim_name, sim_id, self.time_resolution, sim_params)
         )
         # Create the ModelFactory before the SimRunner as it performs
         # some checks on the simulator's meta.
-        model_factory = ModelFactory(self, sim_id, proxy)
-        self.sims[sim_id] = SimRunner(sim_id, proxy)
+        model_factory = ModelFactory(self, self.current_group, sim_id, proxy)
+        self.sims[sim_id] = SimRunner(sim_id, proxy, depth=self.current_group.depth)
         if self.use_cache:
             self.sims[sim_id].outputs = {}
         return model_factory
 
     def connect_one(
         self,
         src: Entity,
@@ -279,20 +330,20 @@
         initial_data: Any = SENTINEL,
     ):
         if not dest_attr:
             dest_attr = src_attr
 
         src_sim = self.sims[src.sid]
         dest_sim = self.sims[dest.sid]
-        
+
         src_port = (src.eid, src_attr)
         dest_port = (dest.eid, dest_attr)
 
         problems: List[str] = []
-        
+
         if src_attr not in src.model_mock.output_attrs:
             problems.append(
                 "the source attribute does not exist"
             )
         if dest_attr not in dest.model_mock.input_attrs:
             problems.append(
                 "the destination attribute does not exist"
@@ -325,61 +376,67 @@
                 f"A connection between the non-persistent attribute {src_attr} of "
                 f"{src.sid} and the non-trigger attribute {dest_attr} of "
                 f"{dest.sid} is not recommended. This might cause problems in the "
                 "simulation! See also: https://mosaik.readthedocs.io/en/latest/"
                 "scenario-definition.html#connecting-entities"
             )
 
-        delay = DenseTime(time_shifted, weak)
+        src_group = src.model_mock._factory._group
+        dest_group = dest.model_mock._factory._group
+        delay = connect_interval(src_group, dest_group, int(time_shifted), int(weak))
+
         dest_sim.input_delays[src_sim] = min(dest_sim.input_delays.get(src_sim, delay), delay)
 
         is_pulled = src_sim.outputs is not None and src.is_persistent(src_attr)
         
         if src.is_persistent(src_attr) and not self.use_cache:
             dest_sim.persistent_inputs.setdefault(dest.eid, {}).setdefault(dest_attr, {}).setdefault(src.full_id, None)
 
         src_sim.output_request.setdefault(src.eid, []).append(src_attr)
 
         if is_pulled:
-            dest_sim.pulled_inputs.setdefault((src_sim, time_shifted), set()).add((src_port, dest_port))
+            dest_sim.pulled_inputs.setdefault((src_sim, delay), set()).add((src_port, dest_port))
         else:
-            src_sim.output_to_push.setdefault(src_port, []).append((dest_sim, time_shifted, dest_port))
+            src_sim.output_to_push.setdefault(src_port, []).append((dest_sim, delay, dest_port))
 
-        src_sim.successors.add(dest_sim)
+        src_sim.successors[dest_sim] = connect_interval(src_group, dest_group)
 
         if dest.triggered_by(dest_attr):
             src_sim.triggers.setdefault(src_port, []).append((dest_sim, delay))
 
         if initial_data is not SENTINEL:
             if is_pulled:
+                assert src_sim.outputs is not None
                 src_sim.outputs.setdefault(
                     -int(time_shifted), {}
                 ).setdefault(src.eid, {})[src_attr] = initial_data
             else:
                 dest_sim.persistent_inputs.setdefault(
                     dest.eid, {}
                 ).setdefault(dest_attr, {})[src.full_id] = initial_data
 
         self.entity_graph.add_edge(src.full_id, dest.full_id)
-    
+
     def connect_async_requests(self, src: ModelFactory, dest: ModelFactory):
         warnings.warn(
             "Connections with async_requests are deprecated. They and the set_data "
             "function will be removed in a future release. Use time_shifted and weak "
             "connections instead.",
             category=DeprecationWarning,
         )
         src_sim = self.sims[src._sid]
         dest_sim = self.sims[dest._sid]
-        src_sim.successors.add(dest_sim)
-        src_sim.successors_to_wait_for.add(dest_sim)
-        # DenseTime(0) is always minimal, so we dont need to compare to
-        # previous value of input_delays[src_sim]
-        dest_sim.input_delays[src_sim] = DenseTime(0)  
-         
+        delay = connect_interval(src._group, dest._group)
+        src_sim.successors[dest_sim] = delay
+        src_sim.successors_to_wait_for[dest_sim] = delay
+        # Normally, we would only set the input delay if it is smaller
+        # than whatever is already there. However, in this case, the
+        # new value is the smallest possible, so no test is necessary.
+        dest_sim.input_delays[src_sim] = delay
+
     def connect(
         self,
         src: Entity,
         dest: Entity,
         *attr_pairs: Union[str, Tuple[str, str]],  # type: ignore
         async_requests: bool = False,
         time_shifted: Union[bool, int] = False,
@@ -452,15 +509,16 @@
         # Add relation in entity_graph
         self.entity_graph.add_edge(src.full_id, dest.full_id)
 
     def set_initial_event(self, sid: SimId, time: int = 0):
         """
         Set an initial step for simulator *sid* at time *time* (default=0).
         """
-        self.sims[sid].next_steps = [DenseTime(time)]
+        sim = self.sims[sid]
+        sim.next_steps = [TieredTime(time) + sim.from_world_time]
 
     def get_data(
         self,
         entity_set: Iterable[Entity],
         *attributes: Attr,
     ) -> Dict[Entity, Dict[Attr, Any]]:
         """
@@ -475,19 +533,19 @@
                     'attr_1': 'val_1',
                     'attr_2': 'val_2',
                     ...
                 },
                 ...
             }
         """
-        outputs_by_sim = defaultdict(dict)
+        outputs_by_sim: Dict[SimId, OutputRequest] = defaultdict(dict)
         for entity in entity_set:
-            outputs_by_sim[entity.sid][entity.eid] = attributes
+            outputs_by_sim[entity.sid][entity.eid] = list(attributes)
 
-        async def request_data():
+        async def request_data() -> Dict[SimId, OutputData]:
             requests = {
                 sid: asyncio.create_task(self.sims[sid].get_data(outputs))
                 for sid, outputs in outputs_by_sim.items()
             }
             try:
                 await asyncio.gather(*requests.values())
             except ConnectionError as e:
@@ -500,22 +558,22 @@
                             e,
                         ) from None
                 else:
                     raise RuntimeError(
                         "Could not determine which simulator closed its connection."
                     )
 
-            results_by_sim = {}
+            results_by_sim: Dict[SimId, OutputData] = {}
             for sid, task in requests.items():
                 results_by_sim[sid] = task.result()
 
             return results_by_sim
 
         results_by_sim = self.loop.run_until_complete(request_data())
-        results = {}
+        results: Dict[Entity, Dict[Attr, Any]] = {}
         for entity in entity_set:
             results[entity] = results_by_sim[entity.sid][entity.eid]
 
         return results
 
     
     def run(
@@ -632,65 +690,120 @@
             self.shutdown()
             if self._debug:
                 dbg.disable()
             if success:
                 logger.info('Simulation finished successfully.')
 
     def cache_triggering_ancestors(self):
+        """Collects the ancestors of each simulator and stores them in
+        the respective simulator object.
         """
-        Collects the ancestors of each simulator and stores them in the
-        respective simulator object.
-        """
-        trigger_graph: networkx.DiGraph[SimRunner] = networkx.DiGraph()
-        for src_sim in self.sims.values():
-            for successors in src_sim.triggers.values():
-                for (dest_sim, delay) in successors:
-                    min_delay = delay
-                    if trigger_graph.has_edge(src_sim, dest_sim):
-                        min_delay = min(delay, trigger_graph[src_sim][dest_sim]["delay"])
-                    trigger_graph.add_edge(src_sim, dest_sim, delay=min_delay)
-        for dest_sim in trigger_graph.nodes:
-            for src_sim in networkx.ancestors(trigger_graph, dest_sim):
-                distance = networkx.shortest_path_length(trigger_graph, src_sim, dest_sim, weight="delay")
-                dest_sim.triggering_ancestors.append((src_sim, distance))
+        # See ``ensure_no_dataflow_cycles`` for an explanation of this
+        # algorithm
+        dirty: Set[SimRunner] = set()
+        for sim in self.sims.values():
+            for port_triggers in sim.triggers.values():
+                for dest_sim, delay in port_triggers:
+                    dest_sim.triggering_ancestors[sim] = delay
+                    dirty.add(dest_sim)
+        while dirty:
+            sim = dirty.pop()
+            for port_triggers in sim.triggers.values():
+                for dest_sim, mid_to_dest in port_triggers:
+                    for src_sim, src_to_mid in sim.triggering_ancestors.items():
+                        src_to_dest = src_to_mid + mid_to_dest
+                        src_to_dest = update_min(dest_sim.triggering_ancestors.get(src_sim), src_to_dest)
+                        if src_to_dest is not None:
+                            dirty.add(dest_sim)
+                            dest_sim.triggering_ancestors[src_sim] = src_to_dest
+        return
 
     def ensure_no_dataflow_cycles(self):
+        """Make sure that there is no cyclic dataflow with 0 total
+        delay. Raise an exception with one such cycle otherwise.
         """
-        Deduce a simulator ranking from a topological sort of the df_graph.
+
+        # Short note on terminology: ancestors and descendants any
+        # number of steps removed; predecessors and successors are one
+        # step removed (i.e. they're *direct* ancestors/descendants)
+
+        dirty: Set[SimRunner] = set(self.sims.values())
+        """Sims that have changed descendants and thus require
+        recalculation
         """
-        immediate_graph: networkx.DiGraph[SimRunner] = networkx.DiGraph()
+        sim_descs: Dict[
+            SimRunner, Dict[SimRunner, Tuple[TieredInterval, List[SimRunner]]]
+        ] = {
+            sim: {} for sim in self.sims.values()
+        }
+        """For each SimRunner, all its descendants that have been found
+        so far with the shortest delay to them and the path that
+        exhibits this delay.
+        """
+
+        # At the start, enter each sim as a descendant of all its
+        # (direct) predecessors
         for sim in self.sims.values():
-            for pred_sim, delay in sim.input_delays.items():
-                if delay == DenseTime(0):
-                    immediate_graph.add_edge(pred_sim, sim)
-        # If there are performance problems, it might be faster to first try sorting
-        # this graph topologically. If that succeeds, there will be no cycles, so the
-        # cycles computation can be skipped.
-        for cycle in networkx.simple_cycles(immediate_graph):
-            # If we run into any cycles, we raise, thus not computing all cycles.
-            raise ScenarioError(
-                "Your scenario contains cycles that are not broken up using "
-                "time-shifted or weak connections. mosaik is unable to determine which "
-                "simulator to run first in these cases. Here is an example of one such "
-                f"cycle: {cycle}."
-            )
+            for pred, delay in sim.input_delays.items():
+                sim_descs[pred][sim] = (delay, [pred, sim])
+        while dirty:
+            mid_sim = dirty.pop()
+            # This sim has had updates to its descendants since we last
+            # processed it. These changes are pushed to its predecessors
+            for src_sim, src_to_mid in mid_sim.input_delays.items():
+                for dest_sim, (mid_to_dest, path) in sim_descs[mid_sim].items():
+                    src_to_dest = src_to_mid + mid_to_dest
+                    src_to_dest = update_min(
+                        sim_descs[src_sim].get(dest_sim, (None,))[0], src_to_dest
+                    )
+                    # update_min only return as non-None value if the
+                    # existing value needs to be updated, i.e. a shorter
+                    # path was found
+                    if src_to_dest is not None:
+                        # In this case we need to update the
+                        # predecessor's shortest path to the descendant
+                        # and reprocess the predecessor
+                        sim_descs[src_sim][dest_sim] = (src_to_dest, [src_sim] + path)
+                        dirty.add(src_sim)
+
+        # We need to raise an error if any sim has itself as a
+        # descendant with a delay of 0
+        for sim, descs in sim_descs.items():
+            if sim not in descs:
+                continue
+            (delay, path) = descs[sim]
+            if all(t == 0 for t in delay.tiers):
+                raise ScenarioError(
+                    f"Your scenario contains cycles, for example: {path}."
+                )
 
     def shutdown(self):
         """
         Shut-down all simulators and close the server socket.
         """
-        if self.server.is_serving():
-            self.server.close()
-
         if not self.loop.is_closed():
             for sim in self.sims.values():
                 self.loop.run_until_complete(sim.stop())
+
+            self.loop.stop()
+            self.loop.run_forever()
             self.loop.close()
 
 
+if TYPE_CHECKING:
+    T = TypeVar("T", bound=SupportsRichComparison)
+
+def update_min(a: T | None, b: T) -> T | None:
+    if a is None:
+        return b
+    if a <= b:  # type: ignore
+        return None
+    return b
+
+
 MOSAIK_METHODS = set(
     ["init", "create", "setup_done", "step", "get_data", "finalize", "stop"]
 )
 
 
 class ModelFactory():
     """
@@ -702,17 +815,18 @@
 
     If you access an attribute that is not a model or if the model is not
     marked as *public*, an :exc:`~mosaik.exceptions.ScenarioError` is raised.
     """
     type: Literal['event-based', 'time-based', 'hybrid']
     models: Dict[ModelName, ModelMock]
 
-    def __init__(self, world: World, sid: SimId, proxy: Proxy):
+    def __init__(self, world: World, group: SimGroup, sid: SimId, proxy: Proxy):
         self.meta = proxy.meta
         self._world = world
+        self._group = group
         self._proxy = proxy
         self._sid = sid
 
         if "type" not in proxy.meta:
             raise ScenarioError(
                 'The simulator is missing a type specification ("time-based", '
                 '"event-based" or "hybrid"). This is required starting from API '
@@ -760,15 +874,15 @@
                         connection.send([meth_name, args, kwargs])
                     )
                 wrapper.__name__ = meth_name
                 return wrapper
 
             setattr(self, meth_name, get_wrapper(proxy, meth_name))
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str):
         # Implemented in order to improve error messages.
         models = self.meta["models"]
         if name in models:
             raise AttributeError(f'Model "{name}" is not public.')
         else:
             raise AttributeError(
                 f'Model factory for "{self._sid}" has no model and no function '
@@ -803,27 +917,34 @@
     :return: A four-tuple of :class:`InOrOutSet`, giving the
         measurement inputs, event inputs, measurement outputs, and event
         outputs.        
     :raises ValueError: if the information is insufficient or
         inconsistent
     """
     error_template = (
-            "%s simulators may not specify %s attrs (use a hybrid simulator, instead, "
-            "if you need both types of %s attributes), and they must list all their "
-            "attrs as %s if that key is present"
+        "%s simulators may not specify %s attrs (use a hybrid simulator, instead, "
+        "if you need both types of %s attributes), and they must list all their "
+        "attrs as %s if that key is present"
     )
     
     if model_desc.get('any_inputs', False):
         inputs: Optional[InOrOutSet[Attr]] = OutSet()
     else:
         inputs = wrap_set(model_desc.get('attrs'))
     empty: FrozenSet[Attr] = frozenset()
-    default_measurements = empty if type == 'event-based' else None
+    if type == 'time-based':
+        default_measurements = None
+        default_events = empty
+    elif type == 'event-based':
+        default_measurements = empty
+        default_events = None
+    elif type == 'hybrid':
+        default_measurements = None if 'trigger' in model_desc else inputs
+        default_events = None
     measurement_inputs = wrap_set(model_desc.get('non-trigger', default_measurements))
-    default_events = None if type == 'event-based' else empty
     event_inputs = wrap_set(model_desc.get('trigger', default_events))
     measurement_inputs, event_inputs = parse_set_triple(
         inputs, measurement_inputs, event_inputs,
         "attrs", "non-trigger", "trigger"
     )
     if type == 'time-based' and event_inputs != frozenset():
         raise ValueError(
@@ -885,36 +1006,42 @@
         self._world = world
         self._factory = factory
         self.name = model
         self._proxy = proxy
         model_desc = proxy.meta['models'][model]
         self.params = frozenset(model_desc.get('params', []))
 
-        (
-            self.measurement_inputs,
-            self.event_inputs,
-            self.measurement_outputs,
-            self.event_outputs,
-        ) = parse_attrs(model_desc, self._factory.type)
+        try:
+            (
+                self.measurement_inputs,
+                self.event_inputs,
+                self.measurement_outputs,
+                self.event_outputs,
+            ) = parse_attrs(model_desc, self._factory.type)
+        except ValueError as e:
+            raise ValueError(
+                f"while parsing the model description of model {model} of the "
+                f"simulator {factory._sid}: {e}"
+            )
 
     @property
     def input_attrs(self) -> InOrOutSet[Attr]:
         return self.event_inputs | self.measurement_inputs
 
     @property
     def output_attrs(self) -> InOrOutSet[Attr]:
         return self.event_outputs | self.measurement_outputs
     
-    def __call__(self, **model_params):
+    def __call__(self, **model_params: Any):
         """
         Call :meth:`create()` to instantiate one model.
         """
         return self.create(1, **model_params)[0]
 
-    def create(self, num: int, **model_params):
+    def create(self, num: int, **model_params: Any):
         """
         Create *num* entities with the specified *model_params* and return
         a list with the entity dicts.
 
         The returned list of entities is the same as returned by
         :meth:`mosaik_api_v3.Simulator.create()`, but the simulator is prepended
         to every entity ID to make them globally unique.
@@ -926,15 +1053,15 @@
         )
         assert len(entities) == num, (
             f'{num} entities were requested but {len(entities)} were created.'
         )
 
         return self._make_entities(entities, assert_type=self.name)
 
-    def _check_params(self, **model_params):
+    def _check_params(self, **model_params: Any):
         unexpected_params = set(model_params.keys()).difference(self.params)
         if unexpected_params:
             sep = "', '"
             raise TypeError(
                 "create() got unexpected keyword arguments: '"
                 f"{sep.join(unexpected_params)}'"
             )
```

### Comparing `mosaik-3.3.0b1/mosaik/scheduler.py` & `mosaik-3.3.1/mosaik/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from heapq import heappop
 from loguru import logger
 from math import ceil
 from time import perf_counter
 
 from mosaik_api_v3 import InputData, SimId, Time
 
-from mosaik.dense_time import DenseTime
 from mosaik.exceptions import SimulationError
 from mosaik.internal_util import recursive_merge_all, recursive_merge_existing
 from mosaik.simmanager import FULL_ID, SimRunner
 
 from typing import TYPE_CHECKING, Any, Coroutine, Dict, List, Optional
+
+from mosaik.tiered_time import TieredTime
 if TYPE_CHECKING:
     from mosaik.scenario import World
 
 
 SENTINEL = object()
 
 
@@ -86,29 +87,32 @@
     """
     sim.started = True
     sim.rt_start = rt_start = perf_counter()
 
     try:
         advance_progress(sim, world)
         while await next_step_settled(sim, world):
-            #await rt_sleep(rt_factor, rt_start, sim, world)
             sim.tqdm.set_postfix_str('await input')
             await wait_for_dependencies(sim, lazy_stepping)
             sim.current_step = heappop(sim.next_steps)
-            if sim.current_step != sim.progress.value:
+            if sim.current_step != sim.progress.time:
                 raise SimulationError(
-                    f'Simulator {sim.sid} is trying to perform a step at time {sim.current_step}, '
-                    f'but it has already progressed to time {sim.progress.value}.'
+                    f"Simulator {sim.sid} is trying to perform a step at time "
+                    f"{sim.current_step}, but it has already progressed to time "
+                    f"{sim.progress.time}."
                 )
-            if sim.current_step.microstep >= world.max_loop_iterations:
+            if any(
+                t >= world.max_loop_iterations for t in sim.current_step.tiers[1:]
+            ):
                 raise SimulationError(
-                    f"Simulator {sim.sid} has performed step {sim.current_step.time} "
-                    f"more than {world.max_loop_iterations} times. This might indicate "
-                    "that you have run into an infinite loop. If not, you can increase "
-                    "max_loop_iterations to get rid of this warning."
+                    f"Simulator {sim.sid} has performed a sub-step more than "
+                    f"{world.max_loop_iterations} times. (The complete now is "
+                    f"{sim.current_step}.) This might indicate that you have run into "
+                    "an infinite loop. If not, you can increase max_loop_iterations to "
+                    "get rid of this warning."
                 )
             input_data = get_input_data(world, sim)
             max_advance = get_max_advance(world, sim, until)
             await step(world, sim, input_data, max_advance)
             rt_check(rt_factor, rt_start, rt_strict, sim)
             await get_outputs(world, sim)
             sim.current_step = None
@@ -137,19 +141,19 @@
     # simulator's progress and which can only go up.
     # Once these two numbers meet, we know that that time is the next
     # step.
     # As a slight complication, we also need to watch out for the end
     # of the simulation. Once that is reached, we also return, albeit
     # without having found a next step.
     sim.tqdm.set_postfix_str('await step')
-    while sim.progress.value.time < world.until:
-        if sim.next_steps and sim.next_steps[0] == sim.progress.value:
+    while sim.progress.time.time < world.until:
+        if sim.next_steps and sim.next_steps[0] == sim.progress.time:
             return True
         else:
-            await_time = sim.next_steps[0] if sim.next_steps else DenseTime(world.until)
+            await_time = sim.next_steps[0] if sim.next_steps else TieredTime(world.until) + sim.from_world_time
             _, pending = await asyncio.wait(
                 [
                     asyncio.create_task(sim.progress.has_reached(await_time)),
                     asyncio.create_task(sim.newer_step.wait()),
                 ],
                 return_when="FIRST_COMPLETED",
                 timeout=world.rt_factor,
@@ -185,27 +189,27 @@
     Wait until all simulators that can provide input for this simulator have run for
     this step.
 
     Also notify any simulator that is already waiting to perform its next step.
 
     *world* is a mosaik :class:`~mosaik.scenario.World`.
     """
-    futures: List[Coroutine[Any, Any, DenseTime]] = []
+    futures: List[Coroutine[Any, Any, TieredTime]] = []
     next_step = sim.next_steps[0]
 
     for pre_sim, delay in sim.input_delays.items():
         # Wait for pre_sim if it hasn't progressed enough to provide
         # the input for our current step.
-        futures.append(pre_sim.progress.has_passed(next_step - delay))
+        futures.append(pre_sim.progress.has_passed(next_step, shift=delay))
 
-    for suc_sim in sim.successors_to_wait_for:
-        futures.append(suc_sim.progress.has_reached(next_step))
+    for suc_sim, adapt in sim.successors_to_wait_for.items():
+        futures.append(suc_sim.progress.has_reached(next_step + adapt))
     if lazy_stepping:
-        for suc_sim in sim.successors:
-            futures.append(suc_sim.progress.has_reached(next_step))
+        for suc_sim, adapt in sim.successors.items():
+            futures.append(suc_sim.progress.has_reached(next_step + adapt))
 
     await asyncio.gather(*futures)
 
 
 def get_input_data(world: World, sim: SimRunner) -> InputData:
     """
     Return a dictionary with the input data for *sim*.
@@ -225,31 +229,36 @@
     inputs from multiple simulators (e.g., different consumers that provide
     loads for a node in a power grid) and cannot know how to aggregate that
     data (sum, max, ...?).
 
     *world* is a mosaik :class:`~mosaik.scenario.World`.
     """
     assert sim.current_step is not None
+    # Input data starts with the data from set_data calls
     input_data = sim.inputs_from_set_data
     sim.inputs_from_set_data = {}
+    # Merge the persistent inputs into the input data, adding keys as
+    # necessary. mosaik controls three levels deep, all further levels
+    # therefore should not be merged.
     recursive_merge_all(
         lambda attrs_new, attrs_old: recursive_merge_all(
             lambda data_new, data_old: recursive_merge_all(
                 lambda val_new, val_old: val_new, data_new, data_old
             ),
             attrs_new,
             attrs_old,
         ),
         input_data,
         sim.persistent_inputs,
     )
+    # Merge in pushed inputs from the timed input buffer
     input_data = sim.timed_input_buffer.get_input(input_data, sim.current_step.time)
 
     for (src_sim, delay), dataflows in sim.pulled_inputs.items():
-        cache = src_sim.get_output_for(sim.current_step.time - delay)
+        cache = src_sim.get_output_for(sim.current_step.time - delay.tiers[0])
         for (src_eid, src_attr), (dest_eid, dest_attr) in dataflows:
             try:
                 val = cache[src_eid][src_attr]
             except KeyError:
                 logger.warning(
                     f"Simulator {src_sim.sid}'s entity {src_eid} did not produce "
                     f"output on its persistent attribute {src_attr} during its last "
@@ -258,14 +267,17 @@
                     "persistent despite working like events. Supplying `None` for now. "
                     "This will be an error in future versions of mosaik."
                 )
                 val = None
             input_vals = input_data.setdefault(dest_eid, {}).setdefault(dest_attr, {})
             input_vals[FULL_ID % (src_sim.sid, src_eid)] = val
 
+    # Merge the data back into the persistent inputs. Here, only keys
+    # that already exist should be updated, as those are the persistent
+    # attributes. (Adding others would make those persistent as well.)
     recursive_merge_existing(
         lambda attrs_old, attrs_new: recursive_merge_existing(
             lambda data_old, data_new: recursive_merge_existing(
                 lambda val_old, val_new: val_new, data_old, data_new
             ),
             attrs_old,
             attrs_new,
@@ -277,24 +289,24 @@
 
 
 def get_max_advance(world: World, sim: SimRunner, until: int) -> int:
     """
     Checks how far *sim* can safely advance its internal time during next step
     without causing a causality error.
     """
-    ancs_next_steps: List[DenseTime] = []
-    for anc_sim, distance in sim.triggering_ancestors:
+    ancs_next_steps: List[Time] = []
+    for anc_sim, distance in sim.triggering_ancestors.items():
         if anc_sim.next_steps:
-            ancs_next_steps.append(anc_sim.next_steps[0] + distance)
+            ancs_next_steps.append((anc_sim.next_steps[0] + distance).time)
 
-    own_next_step = [sim.next_steps[0]] if sim.next_steps else []
+    own_next_step = [sim.next_steps[0].time] if sim.next_steps else []
 
     # The +1, -1 shenanigans exists due to how max_advance was
     # originally designed.
-    return min([*ancs_next_steps, *own_next_step, DenseTime(until + 1)]).time - 1
+    return min([*ancs_next_steps, *own_next_step, until + 1]) - 1
 
 
 async def step(
     world: World,
     sim: SimRunner,
     inputs: InputData,
     max_advance: int
@@ -326,16 +338,17 @@
             raise SimulationError(
                 f'the next step time returned by step must be later than the current '
                 f"step's time, but {next_step_time} <= {sim.current_step.time} "
                 f'for simulator "{sim.sid}"'
             )
 
         if next_step_time < world.until:
-            sim.schedule_step(DenseTime(next_step_time))
-            sim.next_self_step = next_step_time
+            next_step_tiered_time = TieredTime(next_step_time) + sim.from_world_time
+            sim.schedule_step(next_step_tiered_time)
+            sim.next_self_step = next_step_tiered_time
 
     if sim.type == 'time-based':
         assert next_step_time, "A time-based simulator must always return a next step"
 
 
 def rt_check(
     rt_factor: Optional[float],
@@ -375,18 +388,18 @@
     if outattr:
         sim.tqdm.set_postfix_str('get_data')
         data = await sim.get_data(outattr)
 
         output_time: int
         output_time = data.get('time', sim.last_step.time)  # type: ignore
         if output_time == sim.current_step.time:
-            output_dense_time = sim.current_step
+            output_tiered_time = sim.current_step
         else:
-            output_dense_time = DenseTime(output_time)
-        sim.output_time = output_dense_time
+            output_tiered_time = TieredTime(output_time, *([0] * (len(sim.current_step) - 1)))
+        sim.output_time = output_tiered_time
         if sim.last_step.time > output_time:
             raise SimulationError(
                 'Output time (%s) is not >= time (%s) for simulator "%s"'
                 % (output_time, sim.last_step, sim.sid))
 
         # Fill output cache. This will repeat some data that is also
         # pushed forward below, but it is faster to just save everything
@@ -396,15 +409,15 @@
 
         # Push forward certain data
         for (src_eid, src_attr), destinations in sim.output_to_push.items():
             try:
                 val = data[src_eid][src_attr]
                 for dest_sim, time_shift, (dest_eid, dest_attr) in destinations:
                     dest_sim.timed_input_buffer.add(
-                        output_time + time_shift, sid, src_eid, dest_eid, dest_attr, val
+                        output_time + time_shift.tiers[0], sid, src_eid, dest_eid, dest_attr, val
                     )
             except KeyError:
                 pass
         sim.data = data 
 
 
 def notify_dependencies(sim: SimRunner) -> None:
@@ -433,42 +446,42 @@
             }
 
 
 def get_progress(sims: Dict[SimId, SimRunner], until: int) -> float:
     """
     Return the current progress of the simulation in percent.
     """
-    times = [sim.progress.value.time for sim in sims.values()]
+    times = [sim.progress.time.time for sim in sims.values()]
     avg_time = sum(times) / len(times)
     return avg_time * 100 / until
 
 
 def get_avg_progress(sims: Dict[SimId, SimRunner], until: int) -> int:
     """Get the average progress of all simulations (in time steps)."""
-    times = [min(until, sim.progress.value.time + 1) for sim in sims.values()]
+    times = [min(until, sim.progress.time.time + 1) for sim in sims.values()]
     return sum(times) // len(times)
 
 
 def advance_progress(sim: SimRunner, world: World):
-    pre_sim_induced_progress: List[DenseTime] = [
+    pre_sim_induced_progress: List[TieredTime] = [
         pre_sim.next_steps[0] + distance
-        for pre_sim, distance in sim.triggering_ancestors
+        for pre_sim, distance in sim.triggering_ancestors.items()
         if pre_sim.next_steps
     ]
 
-    next_step_progress: List[DenseTime] = [sim.next_steps[0]] if sim.next_steps else []
+    next_step_progress: List[TieredTime] = [sim.next_steps[0]] if sim.next_steps else []
     current_step_prog = [sim.current_step] if sim.current_step else []
     if world.rt_factor:
         rt_passed = perf_counter() - sim.rt_start
-        rt_progress = [DenseTime(ceil(rt_passed / world.rt_factor), 0)]
+        rt_progress = [TieredTime(ceil(rt_passed / world.rt_factor))]
     else:
         rt_progress = []
     new_progress = min([
         *pre_sim_induced_progress,
         *next_step_progress,
         *current_step_prog,
         *rt_progress,
-        DenseTime(world.until),
+        TieredTime(world.until) + sim.from_world_time,
     ])
     sim.progress.set(new_progress)
     sim.tqdm.update(new_progress.time - sim.tqdm.n)
```

### Comparing `mosaik-3.3.0b1/mosaik/simmanager.py` & `mosaik-3.3.1/mosaik/simmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,61 +8,66 @@
 already running simulators and manage access to them.
 """
 from __future__ import annotations
 
 from ast import literal_eval
 import asyncio
 import collections
-from dataclasses import dataclass
 import heapq as hq
 import importlib
 import itertools
 import os
 import shlex
 import subprocess
 import sys
 import platform
 from loguru import logger
 from typing import (
     Any,
     Callable,
     Coroutine,
     Dict,
-    Iterable,
     List,
     NoReturn,
     Optional,
     OrderedDict,
     Set,
     Tuple,
     TYPE_CHECKING,
-    TypeVar,
     Union,
+    cast,
 )
 import tqdm
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Literal, TypeAlias, TypedDict
 
 import mosaik_api_v3
 from mosaik_api_v3.connection import Channel
 from mosaik_api_v3.types import OutputData, OutputRequest, SimId, Time, InputData, Attr, EntityId, FullId
-from mosaik.dense_time import DenseTime
 from mosaik.exceptions import ScenarioError, SimulationError
 from mosaik.progress import Progress
 from mosaik.proxies import Proxy, LocalProxy, BaseProxy, RemoteProxy
 from mosaik.adapters import init_and_get_adapter
+from mosaik.tiered_time import TieredInterval, TieredTime
 
 if 'Windows' in platform.system():
     from subprocess import CREATE_NEW_CONSOLE  # type: ignore (only Windows)
 
 if TYPE_CHECKING:
-    from mosaik.scenario import World
+    from mosaik.scenario import World, ConnectModel, PythonModel, CmdModel
 
 FULL_ID_SEP = '.'  # Separator for full entity IDs
 FULL_ID = '%s.%s'  # Template for full entity IDs ('sid.eid')
 
+class MosaikConfigTotal(TypedDict):
+    """A total version for :cls:`MosaikConfig` for internal use.
+    """
+
+    addr: Tuple[str, int | None]
+    start_timeout: float
+    stop_timeout: float
 
 async def start(
     world: World,
     sim_name: str,
     sim_id: SimId,
     time_resolution: float,
     sim_params: Dict[str, Any],
@@ -123,15 +128,15 @@
     # - cmd: start_proc
     # - connect: start_connect
     starters = StarterCollection()
 
     for sim_type, starter in starters.items():
         if sim_type in sim_config:
             proxy = await starter(
-                world, sim_name, sim_config, MosaikRemote(world, sim_id)
+                world.config, sim_name, sim_config, MosaikRemote(world, sim_id)
             )
             try:
                 proxy = await asyncio.wait_for(
                     init_and_get_adapter(
                         proxy,
                         sim_id,
                         {"time_resolution": time_resolution, **sim_params},
@@ -154,17 +159,17 @@
     else:
         raise ScenarioError(
             f'Simulator "{sim_name}" could not be started: Invalid configuration'
         )
 
 
 async def start_inproc(
-    world: World,
+    mosaik_config: MosaikConfigTotal,
     sim_name: str,
-    sim_config: Dict[Literal['python', 'env'], str],
+    sim_config: PythonModel,
     mosaik_remote: MosaikRemote,
 ) -> BaseProxy:
     """
     Import and instantiate the Python simulator *sim_name* based on its
     config entry *sim_config*.
 
     Return a :class:`LocalProcess` instance.
@@ -195,91 +200,97 @@
     if int(mosaik_api_v3.__version__.split('.')[0]) < 3:
         raise ScenarioError("Mosaik 3 requires mosaik_api_v3 or newer.")
 
     return LocalProxy(sim, mosaik_remote)
 
 
 async def start_proc(
-    world: World,
+    mosaik_config: MosaikConfigTotal,
     sim_name: str,
-    sim_config: Dict[Literal["cmd", "cwd", "env", "posix", "new_console"], Any],
+    sim_config: CmdModel,
     mosaik_remote: MosaikRemote,
 ) -> BaseProxy:
     """
     Start a new process for simulator *sim_name* based on its config entry
     *sim_config*.
 
     Return a :class:`RemoteProcess` instance.
 
     Raise a :exc:`~mosaik.exceptions.ScenarioError` if the simulator cannot be
     instantiated.
     """
-    replacements = {
-        'addr': '%s:%s' % (world.config['addr'][0], world.config['addr'][1]),
-        'python': sys.executable,
-    }
-    cmd = sim_config['cmd'] % replacements
-    if 'posix' in sim_config.keys():
-        posix = sim_config.pop('posix')
+    channel_future: asyncio.Future[Channel] = asyncio.Future()
+    async def on_connect(r: asyncio.StreamReader, w: asyncio.StreamWriter):
+        channel_future.set_result(Channel(r, w))
+
+    async with await asyncio.start_server(on_connect, *mosaik_config["addr"]) as server:
+        actual_addr = server.sockets[0].getsockname()
+        
+        replacements = {
+            "addr": "%s:%s" % actual_addr,
+            "python": sys.executable,
+        }
+        cmd = sim_config["cmd"] % replacements
+        posix = sim_config.pop("posix", os.name != "nt")
         cmd = shlex.split(cmd, posix=bool(posix))
-    else:
-        cmd = shlex.split(cmd, posix=(os.name != 'nt'))
-    cwd = sim_config['cwd'] if 'cwd' in sim_config else '.'
+        cwd = sim_config.get("cwd", ".")
 
-    # Make a copy of the current env. vars dictionary and update it with the
-    # user provided values (or an empty dict as a default):
-    env = dict(os.environ)
-    env.update(sim_config.get('env', {}))  # type: ignore
-
-    # CREATE_NEW_CONSOLE constant for subprocess is only available on Windows
-    creationflags = 0
-    new_console = sim_config.get('new_console', False)
-    if new_console:
-        if 'Windows' in platform.system():
-            creationflags = CREATE_NEW_CONSOLE
-        else:
-            logger.warning('Simulator "{sim_name}" could not be started in a new console: '
-                           'Only available on Windows', sim_name=sim_name)
+        # Make a copy of the current env vars dictionary and update it with the
+        # user provided values (or an empty dict as a default):
+        env = dict(os.environ)
+        env.update(sim_config.get('env', {}))
+
+        # CREATE_NEW_CONSOLE constant for subprocess is only available on Windows
+        creationflags: int = 0
+        new_console = sim_config.get('new_console', False)
+        if new_console:
+            if 'Windows' in platform.system():
+                creationflags = cast(int, CREATE_NEW_CONSOLE)  # type: ignore
+            else:
+                logger.warning(
+                    f'Simulator "{sim_name}" could not be started in a new console: '
+                    "Only available on Windows"
+                )
 
-    kwargs = {
-        'bufsize': 1,
-        'cwd': cwd,
-        'universal_newlines': True,
-        'env': env,  # pass the new env dict to the sub process
-        'creationflags': creationflags,
-    }
-    try:
-        subprocess.Popen(cmd, **kwargs)
-    except (FileNotFoundError, NotADirectoryError) as e:
-        # This distinction has to be made due to a change in python 3.8.0.
-        # It might become unecessary for future releases supporting
-        # python >= 3.8 only.
-        if str(e).count(':') == 2:
-            eout = e.args[1]
-        else:
-            eout = str(e).split('] ')[1]
-        raise ScenarioError('Simulator "%s" could not be started: %s'
-                            % (sim_name, eout)) from None
+        try:
+            subprocess.Popen(
+                cmd, 
+                bufsize=1,
+                cwd=cwd,
+                universal_newlines=True,
+                env=env,  # pass the new env dict to the sub process
+                creationflags=creationflags,
+            )
+        except (FileNotFoundError, NotADirectoryError) as e:
+            # This distinction has to be made due to a change in python 3.8.0.
+            # It might become unecessary for future releases supporting
+            # python >= 3.8 only.
+            if str(e).count(":") == 2:
+                eout = e.args[1]
+            else:
+                eout = str(e).split("] ")[1]
+            raise ScenarioError(
+                f'Simulator "{sim_name}" could not be started: {eout}'
+            ) from None
 
-    try:
-        channel = await asyncio.wait_for(
-            world.incoming_connections_queue.get(),
-            world.config['start_timeout'],
-        )
-        return RemoteProxy(channel, mosaik_remote)
-    except asyncio.TimeoutError:
-        raise SimulationError(
-            f'Simulator "{sim_name}" did not connect to mosaik in time.'
-        )
+        try:
+            channel = await asyncio.wait_for(
+                channel_future, timeout=mosaik_config["start_timeout"]
+            )
+            return RemoteProxy(channel, mosaik_remote)
+        except asyncio.TimeoutError:
+            raise SimulationError(
+                f'Simulator "{sim_name}" did not connect to mosaik in time.'
+            )
 
 
 async def start_connect(
-    world: World,
+    mosaik_config: MosaikConfigTotal,
     sim_name: str,
-    sim_config,
+    sim_config: ConnectModel,
     mosaik_remote: MosaikRemote,
 ) -> BaseProxy:
     """
     Connect to the already running simulator *sim_name* based on its config
     entry *sim_config*.
 
     Return a :class:`RemoteProcess` instance.
@@ -324,140 +335,149 @@
     type: Literal['time-based', 'event-based', 'hybrid']
     supports_set_events: bool
 
     _proxy: Proxy
     """The actual proxy for this simulator."""
 
     # Connection setup
-    input_delays: Dict[SimRunner, DenseTime]
+    input_delays: Dict[SimRunner, TieredInterval]
     """For each simulator that provides data to this simulator, the
     minimum over all input delays. This is used while waiting for
-    dependencies."""
-    triggers: Dict[Port, List[Tuple[SimRunner, DenseTime]]]
+    dependencies.
+    """
+    triggers: Dict[Port, List[Tuple[SimRunner, TieredInterval]]]
     """For each port of this simulator, the simulators that are
     triggered by output on that port and the delay accrued along that
     edge.
     """
-    successors: Set[SimRunner]
-    successors_to_wait_for: Set[SimRunner]
-    triggering_ancestors: List[Tuple[SimRunner, DenseTime]]
+    successors: Dict[SimRunner, TieredInterval]
+    successors_to_wait_for: Dict[SimRunner, TieredInterval]
+    triggering_ancestors: Dict[SimRunner, TieredInterval]
     """An iterable of this sim's ancestors that can trigger a step of
     this simulator. The second component specifies the least amount of
     time that output from the ancestor needs to reach us.
     """
-    pulled_inputs: Dict[Tuple[SimRunner, Time], Set[Tuple[Port, Port]]]
+    pulled_inputs: Dict[Tuple[SimRunner, TieredInterval], Set[Tuple[Port, Port]]]
     """Output to pull in whenever this simulator performs a step.
     The keys are the source SimRunner and the time shift, the values
     are the source and destination entity-attribute pairs.
     """
-    output_to_push: Dict[Port, List[Tuple[SimRunner, int, Port]]]
+    output_to_push: Dict[Port, List[Tuple[SimRunner, TieredInterval, Port]]]
     """This lists those connections that use the timed_input_buffer.
     The keys are the entity-attribute pairs of this simulator with
     the corresponding list of simulator-time-entity-attribute triples
     describing the destinations for that data and the time-shift
     occuring along the connection.
     """
 
+    to_world_time: TieredInterval
+    from_world_time: TieredInterval
+
     output_request: OutputRequest
 
     inputs_from_set_data: InputData
     """Inputs received via `set_data`."""
     persistent_inputs: InputData
     """Memory of previous inputs for persistent attributes."""
     timed_input_buffer: TimedInputBuffer
     """Inputs for this simulator."""
 
 
-    rt_start: float
+    rt_start: float  # type: ignore  # set at start of sim_process
     """The real time when this simulator started (as returned by
     `perf_counter()`."""
     started: bool
 
-    next_steps: List[DenseTime]
+    next_steps: List[TieredTime]
     """The scheduled next steps this simulator will take, organized as a heap.
     Once the immediate next step has been chosen (and the `has_next_step` event
     has been triggered), the step is moved to `next_step` instead."""
     newer_step: asyncio.Event
-    next_self_step: Optional[Time]
+    next_self_step: Optional[TieredTime]
     """The next self-scheduled step for this simulator."""
 
-    progress: Progress[DenseTime]
+    progress: Progress
     """This simulator's progress in mosaik time.
 
     This simulator has done all its work before time `progress`, so
     other simulator can rely on this simulator's output until this time.
     """
-    last_step: DenseTime
+    last_step: TieredTime
     """The most recent step this simulator performed."""
-    current_step: Optional[DenseTime]
+    current_step: Optional[TieredTime]
 
-    output_time: DenseTime
+    output_time: TieredTime  # type: ignore  # set on first get_data
     """The output time associated with `data`. Usually, this will be equal to
     `last_step` but simulators may specify a different time for their output."""
-    data: OutputData
+    data: OutputData  # type: ignore  # set on first get_data
     """The newest data returned by this simulator."""
     task: asyncio.Task[None]
     """The asyncio.Task for this simulator."""
 
     outputs: Optional[Dict[Time, OutputData]]
-    tqdm: tqdm.tqdm[NoReturn]
+    tqdm: tqdm.tqdm[NoReturn]  # type: ignore
 
     def __init__(
         self,
         sid: SimId,
         connection: Proxy,
+        depth: int = 1,
     ):
         self.sid = sid
         self._proxy = connection
 
         self.type = connection.meta['type']
         self.supports_set_events = connection.meta.get('set_events', False)
         # Simulation state
         self.started = False
-        self.last_step = DenseTime(-1)
+        self.last_step = TieredTime(-1, *([0] * (depth - 1)))
         self.current_step = None
         if self.type != 'event-based':
-            self.next_steps = [DenseTime(0)]
+            self.next_steps = [TieredTime(*([0] * depth))]
         else:
             self.next_steps = []
         self.next_self_step = None
-        self.progress = Progress(DenseTime(0))
+        self.progress = Progress(TieredTime(*([0] * depth)))
+
+        self.to_world_time = TieredInterval(0, cutoff=1, pre_length=depth)
+        self.from_world_time = TieredInterval(*([0] * depth), cutoff=1, pre_length=1)
+
         self.inputs_from_set_data = {}
         self.persistent_inputs = {}
         self.timed_input_buffer = TimedInputBuffer()
 
-        self.successors_to_wait_for = set()
-        self.successors = set()
-        self.triggering_ancestors = []
+        self.successors_to_wait_for = {}
+        self.successors = {}
+        self.triggering_ancestors = {}
         self.triggers = {}
         self.output_to_push = {}
         self.pulled_inputs = {}
 
         self.task = None  # type: ignore  # will be set in World.run
         self.newer_step = asyncio.Event()
         self.is_in_step = False
 
         self.input_delays = {}
 
         self.output_request = {}
 
         self.outputs = None
 
-    def schedule_step(self, dense_time: DenseTime):
+    def schedule_step(self, tiered_time: TieredTime):
         """Schedule a step for this simulator at the given time. This
         will trigger a re-evaluation whether this simulator's next
         step is settled, provided that the new step is earlier than the
         old one and the simulator is currently awaiting it's next
         settled step.
         """
-        if dense_time in self.next_steps:
-            return dense_time
+        if tiered_time in self.next_steps:
+            return tiered_time
 
-        is_earlier = not self.next_steps or dense_time < self.next_steps[0]
-        hq.heappush(self.next_steps, dense_time)
+        is_earlier = not self.next_steps or tiered_time < self.next_steps[0]
+        hq.heappush(self.next_steps, tiered_time)
         if is_earlier:
             self.newer_step.set()
 
     async def setup_done(self):
         return await self._proxy.send(["setup_done", (), {}])
 
     async def step(self, time: Time, inputs: InputData, max_advance: Time) -> Optional[Time]:
@@ -575,16 +595,18 @@
         data dictionaries, which in turn map attribute names to their
         respective values:
         (``{'sid/eid': {'attr1': val1, 'attr2': val2}}``).
         """
         assert self.sim.is_in_step, "get_data must happen in step"
         assert self.sim.current_step is not None, "no current step time"
 
-        data = {}
-        missing = collections.defaultdict(lambda: collections.defaultdict(list))
+        data: Dict[FullId, Dict[Attr, Any]] = {}
+        missing: Dict[SimId, OutputRequest] = collections.defaultdict(
+            lambda: collections.defaultdict(list)
+        )
         # Try to get data from cache
         for full_id, attr_names in attrs.items():
             sid, eid = full_id.split(FULL_ID_SEP, 1)
             src_sim = self.world.sims[sid]
             # Check if async_requests are enabled.
             self._assert_async_requests(src_sim, self.sim)
             if self.world.use_cache:
@@ -608,15 +630,15 @@
             for eid, vals in dep_data.items():
                 # Maybe there's already an entry for full_id, so we need
                 # to update the dict in that case.
                 data.setdefault(FULL_ID % (sid, eid), {}).update(vals)
 
         return data
 
-    async def set_data(self, data):
+    async def set_data(self, data: Dict[FullId, Dict[Attr, Any]]):
         """
         Set *data* as input data for all affected simulators.
 
         *data* is a dictionary mapping source entity IDs to destination entity
         IDs with dictionaries of attributes and values (``{'src_full_id':
         {'dest_full_id': {'attr1': 'val1', 'attr2': 'val2'}}}``).
         """
@@ -636,16 +658,15 @@
         sim = self.world.sims[self.sid]
         if not self.world.rt_factor:
             raise SimulationError(
                 f"Simulator '{self.sid}' tried to set an event in non-real-time "
                 "mode."
             )
         if event_time < self.world.until:
-            # TODO: Check whether progress.set is better
-            sim.schedule_step(DenseTime(event_time, 0))
+            sim.schedule_step(TieredTime(event_time))
         else:
             logger.warning(
                 "Event set at {event_time} by {sim_id} is after simulation end {until} "
                 "and will be ignored.",
                 event_time=event_time,
                 sim_id=sim.sid,
                 until=self.world.until,
@@ -682,15 +703,15 @@
 
         from mosaik.simmanager import StarterCollection
         s = StarterCollection()
         s['my_starter'] = my_starter_func
     """
 
     # Singleton instance of the starter collection.
-    __instance = None
+    __instance: OrderedDict[str, Callable[..., Coroutine[Any, Any, BaseProxy]]] | None = None
 
     def __new__(cls) -> OrderedDict[str, Callable[..., Coroutine[Any, Any, BaseProxy]]]:
         if StarterCollection.__instance is None:
             # Create collection with default starters (i.e., starters defined
             # my mosaik core).
             StarterCollection.__instance = collections.OrderedDict(
                 python=start_inproc,
```

### Comparing `mosaik-3.3.0b1/mosaik/util.py` & `mosaik-3.3.1/mosaik/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,56 @@
+# pyright: reportUnknownMemberType=false
 """
 This module contains some utility functions and classes.
 
 """
+from __future__ import annotations
+
 import random
-from typing import Optional
+from typing import TYPE_CHECKING, Collection, Dict, Iterable, List, MutableSequence, Optional, Set, Tuple
 from typing_extensions import Literal
+from mosaik_api_v3 import Attr, SimId
 import networkx as nx
 import datetime
 
-from mosaik.scenario import World
+from mosaik.scenario import Entity, World
+from mosaik.tiered_time import TieredTime
 
+if TYPE_CHECKING:
+    from matplotlib.figure import Figure
+    from matplotlib.axes import Axes
 
 STANDARD_DPI = 600
 STANDARD_FORMAT = "png"
 STANDARD_FOLDER = "figures"
 
 
-def connect_many_to_one(world, src_set, dest, *attrs, async_requests=False):
-    """
-    :meth:`~mosaik.scenario.World.connect` each entity in *src_set*
+def connect_many_to_one(
+    world: World,
+    src_set: Iterable[Entity],
+    dest: Entity,
+    *attrs: Attr | Tuple[Attr, Attr],
+    async_requests: bool = False
+):
+    """:meth:`~mosaik.scenario.World.connect` each entity in *src_set*
     to *dest*.
 
     See the :meth:`~mosaik.scenario.World.connect` for more details.
     """
     for src in src_set:
         world.connect(src, dest, *attrs, async_requests=async_requests)
 
 
 def connect_randomly(
-    world, src_set, dest_set, *attrs, evenly=True, max_connects=float("inf")
+    world: World,
+    src_set: MutableSequence[Entity],
+    dest_set: MutableSequence[Entity],
+    *attrs: Attr | Tuple[Attr, Attr],
+    evenly: bool = True,
+    max_connects: int =float("inf"),  # type: ignore
 ):
     """
     Randomly :meth:`~mosaik.scenario.World.connect` the entities from
     *src_set* to the entities from *dest_set* and return a subset of *dest_set*
     containing all entities with a connection.
 
     *world* is an instance of the :class:`~mosaik.scenario.World` to which the
@@ -71,38 +89,49 @@
         connected = _connect_randomly(
             world, src_set, dest_set, *attrs, max_connects=max_connects
         )
 
     return connected
 
 
-def _connect_evenly(world, src_set, dest_set, *attrs):
+def _connect_evenly(
+    world: World,
+    src_set: MutableSequence[Entity],
+    dest_set: MutableSequence[Entity],
+    *attrs: Attr | Tuple[Attr, Attr]
+) -> Set[Entity]:
     connect = world.connect
-    connected = set()
+    connected: Set[Entity] = set()
 
     src_size, dest_size = len(src_set), len(dest_set)
     pos = 0
     while pos < src_size:
         random.shuffle(dest_set)
         for src, dest in zip(src_set[pos:], dest_set):
             connect(src, dest, *attrs)
             connected.add(dest)
         pos += dest_size
 
     return connected
 
 
-def _connect_randomly(world, src_set, dest_set, *attrs, max_connects=float("inf")):
+def _connect_randomly(
+    world: World,
+    src_set: MutableSequence[Entity],
+    dest_set: MutableSequence[Entity],
+    *attrs: Attr | Tuple[Attr, Attr],
+    max_connects: int = float("inf"),  # type: ignore
+) -> Set[Entity]:
     connect = world.connect
-    connected = set()
+    connected: Set[Entity] = set()
 
     assert len(src_set) <= (len(dest_set) * max_connects)
     max_i = len(dest_set) - 1
     randint = random.randint
-    connects = {}
+    connects: Dict[Entity, int] = {}
     for src in src_set:
         i = randint(0, max_i)
         dest = dest_set[i]
         connect(src, dest, *attrs)
         connected.add(dest)
         connects[dest] = connects.get(dest, 0) + 1
         if connects[dest] >= max_connects:
@@ -110,35 +139,40 @@
             max_i -= 1
             assert max_i >= 0
 
     return connected
 
 
 def plot_execution_time(
-    world,
-    folder=STANDARD_FOLDER,
-    hdf5path=None,
-    dpi=STANDARD_DPI,
-    format=STANDARD_FORMAT,
-    show_plot=True,
-    slice=None,
+    world: World,
+    folder: str = STANDARD_FOLDER,
+    hdf5path: str | None = None,
+    dpi: int = STANDARD_DPI,
+    format: Literal["png", "pdf", "svg"] = STANDARD_FORMAT,
+    show_plot: bool = True,
+    slice: Tuple[int, int] | None = None,
 ):
-    """
-        Creates an image visualizing the execution time of the different simulators of a mosaik scenario.
+    """Creates an image visualizing the execution time of the different
+    simulators of a mosaik scenario.
 
     :param world: mosaik world object
-    :param folder: folder to store the image (only if no hdf5path is provided)
-    :param hdf5path: Path to HDF5 file, which will be used as path for the created image
+    :param folder: folder to store the image (only if no hdf5path is
+        provided)
+    :param hdf5path: Path to HDF5 file, which will be used as path for
+        the created image
     :param dpi: DPI for created images
     :param format: format for created image
-    :show_plot: open a window to show the plot
-    :param slice: reduce the timeframe that you show in the plot. Usage as python list slicing,
-    i.e., negative values are possible to start from the end of the list. Jumps are not possible.
-    Slice needs to be a two-parameter integer list, e.g. [0,5].
-    :return: no return object, but image file will be written to file system
+    :param show_plot: whether to open a window to show the plot
+    :param slice: reduce the timeframe that you show in the plot. Usage
+        as in Python list slicing, i.e., negative values are possible to
+        start from the end of the list. Jumps are not possible.
+        ``slice`` needs to be a two-element integer list, e.g.
+        ``(0, 5)``.
+
+    :return: ``None`` but image file will be written to file system
     """
     import matplotlib.pyplot as plt
 
     steps = {}
     all_nodes = list(world.execution_graph.nodes(data=True))
 
     # Slice the data if the slice reduces the timesteps to be shown
@@ -192,42 +226,42 @@
     folder: str = STANDARD_FOLDER,
     hdf5path: Optional[str] = None,
     dpi: int = STANDARD_DPI,
     format: Literal["png", "pdf", "svg"] = STANDARD_FORMAT,
     show_plot: bool = True,
 ):
     """Creates an image visualizing the data flow graph of a mosaik
-    scenario. Using the spring_layout from Matplotlib (Fruchterman-
+    scenario. Using the spring layout from Matplotlib (Fruchterman-
     Reingold force-directed algorithm) to position the nodes.
 
     :param world: mosaik world object
     :param folder: folder to store the image (only if no hdf5path is 
         provided)
     :param hdf5path: Path to HDF5 file, which will be used as path for
         the created image
     :param dpi: DPI for created images
     :param format: format for created image
-    :show_plot: open a window to show the plot
-    :return: no return object, but image file will be written to file
+    :param show_plot: whether open a window to show the plot
+    :return: ``None`` but image file will be written to file
         system
     """
     import matplotlib.pyplot as plt
     from matplotlib.patches import ConnectionPatch
 
     # Recreate the df_graph for plotting. There might be additional
     # useful information to be extracted from the SimRunners.
     df_graph: nx.DiGraph[str] = nx.DiGraph()
     for sim in world.sims.values():
         df_graph.add_node(sim.sid)
-        for pred, dt in sim.input_delays.items():
+        for pred, delay in sim.input_delays.items():
             df_graph.add_edge(
                 pred.sid,
                 sim.sid,
-                time_shifted=dt.time>0,
-                weak=dt.microstep>0,
+                time_shifted=delay.tiers[0]>0,
+                weak=any(t > 0 for t in delay.tiers[1:]),
             )
     positions = nx.spring_layout(df_graph)
 
     fig, ax = plt.subplots()
     for node in df_graph.nodes:
         # Draw a dot for the simulator
         ax.plot(positions[node][0], positions[node][1], "o")
@@ -279,15 +313,15 @@
         # When the line is more curved, the middle point here is further away from the actual line
         # One could suspect that the mid-point is actually the middle point in this array,
         # but the array starts with the stating point, then has the curve-control point in the middle
         # and then has the points that draw the arrow
         # Why not calculating the middle point on the straight line? Because then by a 50/50 chance
         # when you have a curved arrow back and forth between two points, you can have the annotation
         # above the wrong arrow.
-        midpoint = con.get_path().vertices[1]
+        midpoint: Tuple[float, float] = con.get_path().vertices[1]  # type: ignore  # close enough
 
         ax.annotate(
             annotation,
             (midpoint[0], midpoint[1]),
             xytext=(0, 0),
             textcoords="offset points",
             color=color,
@@ -312,67 +346,72 @@
         transparent=True,
         bbox_inches="tight",
     )
 
 
 def plot_execution_graph(
     world: World,
-    title: str ="",
-    folder=STANDARD_FOLDER,
-    hdf5path=None,
-    dpi=STANDARD_DPI,
-    format=STANDARD_FORMAT,
-    show_plot=True,
+    title: str = "",
+    folder: str =STANDARD_FOLDER,
+    hdf5path: str | None = None,
+    dpi: int = STANDARD_DPI,
+    format: Literal["png", "pdf", "svg"] = STANDARD_FORMAT,
+    show_plot: bool = True,
     save_plot: bool = True,
-    slice=None,
+    slice: Tuple[int, int] | None = None,
 ):
-    """
-        Creates an image visualizing the execution graph of a mosaik scenario.
+    """Creates an image visualizing the execution graph of a mosaik
+    scenario.
 
     :param world: mosaik world object
-    :param title:
-    :param folder: folder to store the image (only if no hdf5path is provided)
-    :param hdf5path: Path to HDF5 file, which will be used as path for the created image
+    :param title: the title of the graph
+    :param folder: folder to store the image (only if no hdf5path is
+        provided)
+    :param hdf5path: Path to HDF5 file, which will be used as path for
+        the created image
     :param dpi: DPI for created images
     :param format: format for created image
-    :show_plot: open a window to show the plot
-    :param slice: reduce the timeframe that you show in the plot. Usage as python list slicing,
-    i.e., negative values are possible to start from the end of the list. Jumps are not possible.
-    Slice needs to be a two-parameter integer list, e.g. [0,5].
-    :return: no return object, but image file will be written to file system
+    :param show_plot: whether to open a window to show the plot
+    :param slice: reduce the timeframe that you show in the plot.
+        Usage as in Python list slicing, i.e., negative values are
+        possible to start from the end of the list. Jumps are not
+        possible. ``slice`` needs to be a two-element integer tuple,
+        e.g. ``(0, 5)``.
+
+    :return: ``None`` but image file will be written to file system
     """
     import matplotlib.pyplot as plt
     from matplotlib import rcParams
     from matplotlib.ticker import MaxNLocator
 
     all_nodes = list(world.execution_graph.nodes(data=True))
 
     rcParams.update({"figure.autolayout": True})
 
-    steps_st = {}
+    steps_st: Dict[SimId, List[float]] = {}
     for sim_name in world.sims.keys():
         steps_st[sim_name] = []
 
     for node in all_nodes:
-        sim_name, t, n_rep = split_node(node[0])
-        steps_st[sim_name].append(t + n_rep * 0.1)
+        sim_name, tiered_time = node[0]
+        steps_st[sim_name].append(_tiered_time_pos(tiered_time))
 
     fig, ax = plt.subplots()
     if title:
         fig.suptitle(title)
 
     # Draw the time steps from the simulators
     number_of_steps = 0
-    colormap = ["black" for x in range(len(world.sims.keys()))]
-    for i, sim_name in enumerate(world.sims.keys()):
+    colormap = ["black" for _ in world.sims]
+    for i, sim_name in enumerate(world.sims):
         # We need the number of steps in the simulation for correct plotting with slices
         if number_of_steps < len(steps_st[sim_name]):
             number_of_steps = len(steps_st[sim_name])
 
-        if slice != None:
+        if slice is not None:
             dot = ax.plot(
                 steps_st[sim_name][slice[0] : slice[1]],
                 [i] * len(steps_st[sim_name][slice[0] : slice[1]]),
                 "o",
             )
         else:
             dot = ax.plot(steps_st[sim_name], [i] * len(steps_st[sim_name]), "o")
@@ -380,32 +419,32 @@
         colormap[i] = dot[0].get_color()
 
     ax.xaxis.set_major_locator(MaxNLocator(integer=True))
     ax.set_yticks(list(range(len(world.sims.keys()))))
     ax.set_yticklabels(list(world.sims.keys()))
 
     all_edges = list(world.execution_graph.edges())
-    y_pos = {}
+    y_pos: Dict[SimId, int] = {}
     for sim_count, sim_name in enumerate(world.sims.keys()):
         y_pos[sim_name] = sim_count
 
     # The slice values can be negative, so we want to have the correct time steps
     labels = None
     if slice is not None:
         labels = range(world.until)[slice[0] : slice[1]]
 
     for edge in all_edges:
-        isid_0, t0, n_rep0 = split_node(edge[0])
-        isid_1, t1, n_rep1 = split_node(edge[1])
+        isid_0, t0 = edge[0]
+        isid_1, t1 = edge[1]
 
-        if arrow_is_not_in_slice(labels, t0, t1):
+        if arrow_is_not_in_slice(labels, t0.time, t1.time):
             continue
 
-        x_pos0 = t0 + n_rep0 * 0.1
-        x_pos1 = t1 + n_rep1 * 0.1
+        x_pos0 = _tiered_time_pos(t0)
+        x_pos1 = _tiered_time_pos(t1)
         y_pos0 = y_pos[isid_0]
         y_pos1 = y_pos[isid_1]
 
         ax.annotate(
             "",
             (x_pos1, y_pos1),
             xytext=(x_pos0, y_pos0),
@@ -432,97 +471,111 @@
             dpi=dpi,
             facecolor="white",
             transparent=True,
             bbox_inches="tight",
         )
 
 
-def arrow_is_not_in_slice(labels, t0, t1):
+def arrow_is_not_in_slice(
+    labels: Collection[int] | None,
+    t0: int,
+    t1: int,
+):
     return labels is not None and (t0 not in labels or t1 not in labels)
 
 
-def split_node(node):
-    isid, dt = node
-    return isid, dt.time, dt.microstep
-
-
 def plot_execution_time_per_simulator(
-    world,
-    folder=STANDARD_FOLDER,
-    hdf5path=None,
-    dpi=STANDARD_DPI,
-    format=STANDARD_FORMAT,
-    show_plot=True,
+    world: World,
+    folder: str = STANDARD_FOLDER,
+    hdf5path: str | None = None,
+    dpi: int = STANDARD_DPI,
+    format: Literal["png", "pdf", "svg"] = STANDARD_FORMAT,
+    show_plot: bool = True,
     plot_per_simulator: bool = False,
-    slice=None,
+    slice: Tuple[int, int] | None = None,
 ):
-    """
-        Creates images visualizing the execution time of each of the different simulators of a mosaik scenario.
+    """Creates images visualizing the execution time of each of the
+    different simulators of a mosaik scenario.
 
     :param world: mosaik world object
-    :param folder: folder to store the image (only if no hdf5path is provided)
-    :param hdf5path: Path to HDF5 file, which will be used as path for the created image
+    :param folder: folder to store the image (only if no hdf5path is
+        provided)
+    :param hdf5path: Path to HDF5 file, which will be used as path for
+        the created image
     :param dpi: DPI for created images
     :param format: format for created image
-    :show_plot: open a window to show the plot
-    :plot_per_simulator: Create a separated plot per simulator. This is especially useful
-                         if the step sizes of the simulators are very different.
-    :param slice: reduce the timeframe that you show in the plot. Usage as python list slicing,
-    i.e., negative values are possible to start from the end of the list. Jumps are not possible.
-    Slice needs to be a two-parameter integer list, e.g. [0,5].
-    :return: no return object, but image file will be written to file system
+    :param show_plot: whether to open a window to show the plot
+    :param plot_per_simulator: whether to create a separated plot per
+        simulator. This is especially useful if the step sizes of the
+        simulators are very different.
+    :param slice: reduce the timeframe that you show in the plot. Usage
+        as in Python list slicing, i.e., negative values are possible to
+        start from the end of the list. Jumps are not possible.
+        ``slice`` needs to be a two-element integer tuple, e.g.
+        ``(0, 5)``.
+    :return: ``None`` but image file will be written to file system
     """
-    import matplotlib.pyplot as plt
-
     execution_graph = world.execution_graph
-    results = {}
+    results: Dict[SimId, List[float]] = {}
     for node in execution_graph.nodes:
         execution_time = (
             execution_graph.nodes[node]["t_end"] - execution_graph.nodes[node]["t"]
         )
         sim_id = node[0]
-        if sim_id not in results:
-            results[sim_id] = []
-        results[sim_id].append(execution_time)
+        results.setdefault(sim_id, []).append(execution_time)
 
     if plot_per_simulator is False:
-        fig, sub_figure = init_execution_time_per_simulator_plot(plt)
-
-    for key in results.keys():
-        if plot_per_simulator is True:
-            fig, sub_figure = init_execution_time_per_simulator_plot(plt)
-        plot_results = get_execution_time_per_simulator_plot_data(
-            slice, results, sub_figure, key
-        )
-        sub_figure.plot(plot_results, label=key)
-        if plot_per_simulator is True:
-            finish_execution_time_per_simulator_plot(
-                folder, hdf5path, dpi, format, show_plot, plt, fig, "_" + key
+        fig, sub_figure = init_execution_time_per_simulator_plot()
+        for key in results.keys():
+            plot_results = get_execution_time_per_simulator_plot_data(
+                slice, results, sub_figure, key
             )
-
-    if plot_per_simulator is False:
+            sub_figure.plot(plot_results, label=key)
         finish_execution_time_per_simulator_plot(
-            folder, hdf5path, dpi, format, show_plot, plt, fig
+            folder, hdf5path, dpi, format, show_plot, fig
         )
+    else:
+        for key in results.keys():
+            fig, sub_figure = init_execution_time_per_simulator_plot()
+            plot_results = get_execution_time_per_simulator_plot_data(
+                slice, results, sub_figure, key
+            )
+            sub_figure.plot(plot_results, label=key)
+            finish_execution_time_per_simulator_plot(
+                folder, hdf5path, dpi, format, show_plot, fig, "_" + key
+            )
 
 
-def get_execution_time_per_simulator_plot_data(slice, results, sub_figure, key):
+def get_execution_time_per_simulator_plot_data(
+    slice: Tuple[int, int] | None,
+    results: Dict[SimId, List[float]],
+    sub_figure: Axes,
+    key: SimId,
+) -> List[float]:
     if slice is not None:
         plot_results = results[key][slice[0] : slice[1]]
         # The slice values can be negative, so we want to have the correct time steps
         labels = range(len(results[key]))[slice[0] : slice[1]]
-        sub_figure.set_xticks(range(0, len(labels)), labels)
+        sub_figure.set_xticks(range(0, len(labels)), map(str, labels))
     else:
         plot_results = results[key]
     return plot_results
 
 
 def finish_execution_time_per_simulator_plot(
-    folder, hdf5path, dpi, format, show_plot, plt, fig, simulator_name: str = ""
+    folder: str,
+    hdf5path: str | None,
+    dpi: int,
+    format: Literal["png", "svg", "pdf"],
+    show_plot: bool,
+    fig: Figure,
+    simulator_name: str = "",
 ):
+    import matplotlib.pyplot as plt
+
     fig.legend()
     if hdf5path:
         filename: str = hdf5path.replace(".hdf5", "_" + "all" + ".png")
     else:
         filename: str = get_filename(folder, "execution_time_simulator" + simulator_name, format)
 
     fig.savefig(
@@ -536,19 +589,20 @@
 
     if show_plot is True:
         plt.show()
 
     plt.close()
 
 
-def init_execution_time_per_simulator_plot(plt):
+def init_execution_time_per_simulator_plot() -> Tuple[Figure, Axes]:
+    import matplotlib.pyplot as plt
     from matplotlib.ticker import MaxNLocator
 
-    fig = plt.figure()
-    sub_figure = fig.add_subplot()
+    fig: Figure = plt.figure()
+    sub_figure: Axes = fig.add_subplot()
     sub_figure.set_title("Execution time")
     sub_figure.set_ylabel("Execution time [s]")
     sub_figure.set_xlabel("Simulation time [steps of the simulator]")
     sub_figure.get_xaxis().set_major_locator(MaxNLocator(integer=True))
     return fig, sub_figure
 
 
@@ -561,7 +615,15 @@
         .replace(":", "")
         .replace(".", "")
         + "_"
         + type
         + "."
         + file_format
     )
+
+def _tiered_time_pos(time: TieredTime, base: float = 0.1) -> float:
+    result = 0.0
+    factor = 1.0
+    for tier in time.tiers:
+        result += factor * tier
+        factor *= base
+    return result
```

### Comparing `mosaik-3.3.0b1/mosaik.egg-info/PKG-INFO` & `mosaik-3.3.1/mosaik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik
-Version: 3.3.0b1
+Version: 3.3.1
 Summary: Mosaik is a flexible Smart-Grid co-simulation framework.
 Home-page: https://mosaik.offis.de
 Author: mosaik development team
 Author-email: mosaik@offis.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -34,16 +34,14 @@
 
 Mosaik is a simulation compositor for Smart Grid simulations.
 
 It lets you re-use existing simulators and couple them to simulate large-scale
 Smart Grid scenarios. Mosaik offers powerful mechanisms to specify and compose
 these scenarios.
 
-Version: 3.3.0.b1
-
 License: LGPL
 
 Example
 -------
 
 A simple demo scenario with mosaik::
 
@@ -115,19 +113,20 @@
 You have a question, a feature request or want to generally discuss the amazing 
 possibilities with co-simulation and mosaik? We are curious to hear from you! 
 Join us on `GitHub Discussions <https://github.com/orgs/OFFIS-mosaik/discussions>`_.
 
 Changelog
 =========
 
-3.3.0 - 2024-01-17
--------------------
+3.3.0 - 2024-04-08
+------------------
 - [NEW] A simulator can now be connected to itself if the connection is weak or time_shifted (https://gitlab.com/mosaik/mosaik/-/issues/156)
 - [NEW] mosaik now provides a couple of basic simulators (https://gitlab.com/mosaik/mosaik/-/issues/192 , https://mosaik.readthedocs.io/en/latest/ecosystem/index.html#mosaik-basic-simulators)
 - [NEW] Simulators can return extra_info for their entities to be used in scenario script (https://gitlab.com/mosaik/mosaik/-/issues/197)
+- [NEW] Simulators now can (and potentially must) be grouped in a scenario script for more fine-grained control over same-time loops (https://gitlab.com/mosaik/mosaik/-/issues/215)
 - [IMPROVEMENT] Internal rework and refactoring of the time handling in mosaik (https://gitlab.com/mosaik/mosaik/-/issues/162)
 
 
 3.2.0 - 2023-08-31
 ------------------
 - [NEW] Visualizations for the simulation debug information (https://gitlab.com/mosaik/mosaik/-/issues/173)
 - [NEW] Allow to open a new console for simulator (https://gitlab.com/mosaik/mosaik/-/issues/84)
```

### Comparing `mosaik-3.3.0b1/mosaik.egg-info/SOURCES.txt` & `mosaik-3.3.1/mosaik.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 pyproject.toml
 setup.cfg
 setup.py
 mosaik/__init__.py
 mosaik/_debug.py
 mosaik/_version.py
 mosaik/adapters.py
-mosaik/dense_time.py
 mosaik/exceptions.py
 mosaik/in_or_out_set.py
 mosaik/internal_util.py
 mosaik/progress.py
 mosaik/proxies.py
 mosaik/py.typed
 mosaik/scenario.py
 mosaik/scheduler.py
 mosaik/simmanager.py
+mosaik/tiered_time.py
 mosaik/util.py
 mosaik.egg-info/PKG-INFO
 mosaik.egg-info/SOURCES.txt
 mosaik.egg-info/dependency_links.txt
 mosaik.egg-info/requires.txt
 mosaik.egg-info/top_level.txt
 mosaik/basic_simulators/__init__.py
 mosaik/basic_simulators/input_simulator.py
 mosaik/basic_simulators/output_simulator.py
 tests/test_adapters.py
 tests/test_attr_specification.py
 tests/test_basic_simulators.py
 tests/test_benchmarks.py
-tests/test_dense_time.py
 tests/test_exceptions.py
 tests/test_mosaik.py
 tests/test_scenario.py
 tests/test_scheduler.py
 tests/test_simmanager.py
+tests/test_tiered_time.py
 tests/test_tutorial.py
 tests/test_util.py
```

### Comparing `mosaik-3.3.0b1/pyproject.toml` & `mosaik-3.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosaik"
-version = "3.3.0.b1"
+version = "3.3.0"
 description = "mosaik is a flexible smart-grid co-simulation framework"
 authors = ["mosaik development team <mosaik@offis.de>"]
 license = "LGPL-2.1-only"
 readme = ["README.rst", "CHANGES.txt", "AUTHORS.txt"]
 homepage = "https://mosaik.offis.de/"
 repository = "https://gitlab.com/mosaik/mosaik"
 documentation = "https://mosaik.readthedocs.io/"
@@ -16,35 +16,35 @@
     "Operating System :: OS Independent", 
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-loguru = "^0.6"
+loguru = ">=0.6, <1"
 networkx = "^2.5"
 tqdm = "^4.64.1"
 typing-extensions = "^4.5"
-mosaik-api-v3 = "^3.0.4"
+mosaik-api-v3 = "^3.0.9"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "3.7.9"
 pep8 = "1.7.1"
 pytest = "7.2.2"
 pytest-cov = "^2.8.1"
 pytest-benchmark = "^3.4.1"
 pytest-asyncio = "^0.20.3"
 tox = "^3.20.1"
-
+icecream = "^2.1.3"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = {version = "^7.2.5", python = "^3.9"}
 sphinx-rtd-theme = "^1.3.0"
-sphinxcontrib-plantuml = "^0.26"
+sphinx-toolbox = "^3.5.0"
+mosaik-heatpump = "^1.0"
 
 [tool.poetry.group.plotting.dependencies]
 matplotlib = { version = "^3.8.2", markers = "python_version >= '3.9'" }
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mosaik-3.3.0b1/setup.py` & `mosaik-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/tests/test_adapters.py` & `mosaik-3.3.1/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/tests/test_basic_simulators.py` & `mosaik-3.3.1/tests/test_basic_simulators.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/tests/test_benchmarks.py` & `mosaik-3.3.1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/tests/test_exceptions.py` & `mosaik-3.3.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaik-3.3.0b1/tests/test_scenario.py` & `mosaik-3.3.1/tests/test_scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List, cast
 
 from networkx import to_dict_of_dicts as to_dict
 
 from mosaik import scenario
-from mosaik.dense_time import DenseTime
 from mosaik.scenario import Entity, ModelFactory, World
 from mosaik.exceptions import ScenarioError
 import pytest
 
+from mosaik.tiered_time import TieredInterval
+
 sim_config: scenario.SimConfig = {
     'ExampleSim': {
         'python': 'example_sim.mosaik:ExampleSim',
     },
     'MetaMirror': {
         'python': 'tests.simulators.meta_mirror:MetaMirror',
     },
@@ -63,14 +64,22 @@
         assert world.sims == {}
         assert world.loop
         assert not hasattr(world, 'execution_graph')
     finally:
         world.shutdown()
 
 
+def test_two_worlds():
+    """Test that two worlds can exist without a port conflict."""
+    world_1 = World({})
+    world_2 = World({})
+    world_1.shutdown()
+    world_2.shutdown()
+
+
 def test_world_debug():
     world = World(sim_config, debug=True)
     try:
         assert world.execution_graph.adj == {}
     finally:
         world.shutdown()
 
@@ -115,20 +124,20 @@
     for i, j in zip(a, b):
         world.connect(i, j, ('val_out', 'val_in'), ('dummy_out', 'dummy_in'))
 
     sim_0 = world.sims[sim_0._sid]
     sim_1 = world.sims[sim_1._sid]
     
     # TODO: check for connections in new place
-    assert sim_0.successors == set((sim_1,))
-    assert sim_0.successors_to_wait_for == set()
-    assert sim_1.successors == set()
-    assert sim_1.input_delays[sim_0] == DenseTime(0, 0)
+    assert sim_0.successors == {sim_1: TieredInterval(0)}
+    assert sim_0.successors_to_wait_for == {}
+    assert sim_1.successors == {}
+    assert sim_1.input_delays[sim_0] == TieredInterval(0)
 
-    assert sim_1.pulled_inputs[(sim_0, 0)] == set([
+    assert sim_1.pulled_inputs[(sim_0, TieredInterval(0))] == set([
         ((a[0].eid, 'val_out'), (b[0].eid, 'val_in')),
         ((a[0].eid, 'dummy_out'), (b[0].eid, 'dummy_in')),
         ((a[1].eid, 'val_out'), (b[1].eid, 'val_in')),
         ((a[1].eid, 'dummy_out'), (b[1].eid, 'dummy_in')),
     ])
     
     assert to_dict(world.entity_graph) == {
@@ -143,36 +152,46 @@
     """Connections to entities belonging to the same simulator must have
     a delay (time-shifted or weak).
     """
     a = world.start('ExampleSim').A.create(2, init_val=0)
     with pytest.raises(ScenarioError) as err:
         world.connect(a[0], a[1], ('val_out', 'val_out'))
         world.run(1)
-    assert "cycles that are not broken up" in str(err.value)
+    assert "Your scenario contains cycles" in str(err.value)
 
 
 def test_world_connect_cycle(world: World):
     """
     If connecting two entities results in a cycle in the dataflow graph,
     an error must be raised.
     """
     a = world.start('ExampleSim').A(init_val=0)
     b = world.start('ExampleSim').B(init_val=0)
     world.connect(a, b, ('val_out', 'val_in'))
     world.connect(b, a, ('val_in', 'val_out'))
     with pytest.raises(ScenarioError) as err:
         world.run(1)
     assert (
-        "Your scenario contains cycles that are not broken up using time-shifted or "
-        "weak connections. mosaik is unable to determine which simulator to run first "
-        "in these cases. Here is an example of one such cycle:"
-        in str(err.value)
+        "Your scenario contains cycles" in str(err.value)
     )
 
 
+def test_group_cycle(world: World):
+    with world.group():
+        a = world.start('ExampleSim').B(init_val=0)
+        b = world.start('ExampleSim').B(init_val=0)
+    c = world.start('ExampleSim').B(init_val=0)
+    world.connect_one(a, b, 'val_out', 'val_in', weak=True, initial_data=None)
+    world.connect_one(b, c, 'val_out', 'val_in')
+    world.connect_one(c, a, 'val_out', 'val_in')
+    with pytest.raises(ScenarioError) as err:
+        world.run(0)
+    assert "Your scenario contains cycles" in str(err.value)
+
+
 def test_world_connect_wrong_attr_names(world: World):
     """
     The entities to be connected must have the listed attributes.
     """
     a = world.start('ExampleSim', sim_id="A").A(init_val=0)
     b = world.start('ExampleSim', sim_id="B").B(init_val=0)
     with pytest.raises(ScenarioError) as err:
@@ -202,15 +221,15 @@
     world.connect(a, b)
 
     sim_0 = world.sims["ExampleSim-0"]
     sim_1 = world.sims["ExampleSim-1"]
 
     sim_0.successors = set((sim_1,))
     sim_1.successors = set()
-    sim_1.input_delays = {sim_0: DenseTime(0)}
+    sim_1.input_delays = {sim_0: TieredInterval(0)}
     assert world.entity_graph.adj == {
         'ExampleSim-0.' + a.eid: {'ExampleSim-1.' + b.eid: {}},
         'ExampleSim-1.' + b.eid: {'ExampleSim-0.' + a.eid: {}},
     }
 
 
 def test_world_connect_any_inputs(world: World):
@@ -227,20 +246,20 @@
             "models": {"B": {"any_inputs": True, "attrs": []}},
         }
     ).B())
     sim_a = world.sims[a.sid]
     sim_b = world.sims[b.sid]
     world.connect(a, b, 'val_out')
 
-    assert sim_b.pulled_inputs[(sim_a, 0)] == set([
+    assert sim_b.pulled_inputs[(sim_a, TieredInterval(0))] == set([
         ((a.eid, "val_out"), (b.eid, "val_out")),
     ])
     
-    assert sim_a.successors == set((sim_b,))
-    assert sim_b.input_delays[sim_a] == DenseTime(0)
+    assert sim_a.successors == {sim_b: TieredInterval(0)}
+    assert sim_b.input_delays[sim_a] == TieredInterval(0)
     assert to_dict(world.entity_graph) == {
         'ExampleSim-0.' + a.eid: {'MetaMirror-0.' + b.eid: {}},
         'MetaMirror-0.' + b.eid: {'ExampleSim-0.' + a.eid: {}},
     }
 
 
 @pytest.mark.filterwarnings("ignore:Connections with async_requests")
@@ -256,26 +275,34 @@
 def test_world_connect_time_shifted(world: World):
     a = cast(Entity, world.start('ExampleSim').A(init_val=0))
     b = cast(Entity, world.start('ExampleSim').B(init_val=0))
     sim_a = world.sims[a.sid]
     sim_b = world.sims[b.sid]
     world.connect(a, b, 'val_out', time_shifted=True, initial_data={'val_out': 1.0})
 
-    assert sim_b.pulled_inputs[(sim_a, 1)] == set([
+    assert sim_b.pulled_inputs[(sim_a, TieredInterval(1))] == set([
         ((a.eid, 'val_out'), (b.eid, 'val_out')),
     ])
-    assert sim_a.successors == set((sim_b,))
-    assert sim_b.input_delays[sim_a] == DenseTime(1, 0)
+    assert sim_a.successors == {sim_b: TieredInterval(0)}
+    assert sim_b.input_delays[sim_a] == TieredInterval(1)
     assert world.sims['ExampleSim-0'].outputs[-1] == {
         a.eid: {
             'val_out': 1.0
         },
     }
 
 
+def test_weak_outside_group(world: World):
+    a = world.start('ExampleSim').A(init_val=0)
+    b = world.start('ExampleSim').B(init_val=0)
+    with pytest.raises(ScenarioError) as exc:
+        world.connect(a, b, "val_out", weak=True, initial_data={"val_out": 0})
+    assert "in groups" in str(exc.value)
+
+
 def test_world_get_data(world: World):
     sim1 = world.start('ExampleSim')
     sim2 = world.start('ExampleSim')
 
     es1 = sim1.A.create(2, init_val=1)
     es2 = sim2.B.create(1, init_val=2)
```

### Comparing `mosaik-3.3.0b1/tests/test_scheduler.py` & `mosaik-3.3.1/tests/test_scheduler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,67 @@
+from __future__ import annotations
+
 import asyncio
 from heapq import heappop, heappush
+from mosaik_api_v3 import InputData
 import pytest
+from pytest import mark, param
 from tqdm import tqdm
-from typing import Iterable, List
+from typing import Any, Coroutine, Iterable, List
 
 from mosaik import exceptions, scenario, scheduler, simmanager, World
 from mosaik.adapters import init_and_get_adapter
-from mosaik.dense_time import DenseTime
 from mosaik.progress import Progress
 from mosaik.proxies import LocalProxy
 from mosaik.simmanager import SimRunner
+from mosaik.tiered_time import TieredInterval, TieredTime
 
 from tests.mocks.simulator_mock import SimulatorMock
 
 
-async def does_coroutine_stall(coro, pass_backs=0):
+async def does_coroutine_stall(coro: Coroutine[Any, Any, Any], max_pass_backs: int = 0):
     """Executes the given coroutine as a task and give control back
     to it `pass_backs` times. If it doesn't complete in that time,
     the task is cancelled.
     
-    Returns whether the task is completed in the given time.
+    Returns ``False`` if the coroutine did not complete in the given
+    attempts, ``True`` otherwise.
     """
     task = asyncio.create_task(coro)
     async def canceller():
-        for _ in range(pass_backs):
+        for _ in range(max_pass_backs):
             await asyncio.sleep(0)
         if not task.done():
             task.cancel()
     await asyncio.gather(task, canceller(), return_exceptions=True)
     return task.cancelled()
 
 
 @pytest.fixture(name='world')
-def world_fixture(request):
-    event_based = request.param == 'event-based'
+def world_fixture(request: pytest.FixtureRequest):
+    """This fixture provides an example scenario for testing the
+    scheduler. It looks like this:
+
+    ┌───────┐                               ┌──────────────────────┐
+    │ Sim-0 ├─────────┐                     │ ┌───────┐            │
+    └───────┘         ▼                     │ │ Sim-4 │            │
+                  ┌───────┐     ┌───────┐   │ └─┬─────┘            │
+                  │ Sim-2 ├────►│ Sim-3 │   │   ▼   ▲time-shifted/ │
+                  └───────┘     └───────┘   │ ┌─────┴─┐   weak     │
+    ┌───────┐         ▲                     │ │ Sim-5 │            │
+    │ Sim-1 ├─────────┘                     │ └───────┘            │
+    └───────┘                               └──────────────────────┘
+    
+    All connections are non-triggering if the param value is
+    "time-based", and are triggering if the param value is
+    "event-based". The edge marked time-shifted/weak is time-shifted or
+    weak in these two cases, respectively. The box (indicating a
+    simulator group) only exists in the event-based case.
+    """
+    event_based = (request.param == 'event-based')
     world = scenario.World({})
     sims: List[SimRunner] = []
     for i in range(6):
         sim_id = f"Sim-{i}"
         proxy = LocalProxy(SimulatorMock(request.param), simmanager.MosaikRemote(world, sim_id))
         proxy = world.loop.run_until_complete(
             init_and_get_adapter(proxy, sim_id, {"time_resolution": 1.0})
@@ -46,23 +70,34 @@
         world.sims[sim_id] = sim
         sims.append(sim)
     class DummyTask:
         def done(self):
             return False
     for sim in world.sims.values():
         sim.task = DummyTask()
-    for src, dest in [(0, 2), (1, 2), (2, 3), (4, 5)]:
-        sims[src].successors.add(sims[dest])
-        sims[dest].input_delays[sims[src]] = DenseTime(0)
+    
+    for src, dest in [(0, 2), (1, 2), (2, 3)]:
+        sims[src].successors[sims[dest]] = TieredInterval(0)
+        sims[dest].input_delays[sims[src]] = TieredInterval(0)
         if event_based:
-            sims[src].triggers.setdefault(('1', 'x'), []).append((sims[dest], DenseTime(0)))
-    sims[5].successors.add(sims[4])
-    sims[4].input_delays[sims[5]] = DenseTime(0, 1) if event_based else DenseTime(1, 0)
+            sims[src].triggers.setdefault(('1', 'x'), []).append((sims[dest], TieredInterval(0)))
     if event_based:
-        sims[5].triggers[('1', 'x')] = [(sims[4], DenseTime(0, 1))]
+        sims[4].successors[sims[5]] = TieredInterval(0, 0)
+        sims[5].input_delays[sims[4]] = TieredInterval(0, 0)
+        sims[5].successors[sims[4]] = TieredInterval(0, 0)
+        sims[4].input_delays[sims[5]] = TieredInterval(0, 1)
+        sims[4].triggers[('1', 'x')] = [(sims[5], TieredInterval(0, 0))]
+        sims[5].triggers[('1', 'x')] = [(sims[4], TieredInterval(0, 1))]
+    else:
+        sims[4].successors[sims[5]] = TieredInterval(0)
+        sims[5].input_delays[sims[4]] = TieredInterval(0)
+        sims[5].successors[sims[4]] = TieredInterval(0)
+        sims[4].input_delays[sims[5]] = TieredInterval(1)
+
+
     world.until = 4
     world.rt_factor = None
     world.cache_triggering_ancestors()
     yield world
     world.shutdown()
 
 
@@ -134,73 +169,76 @@
     Returns whether any of the events of the given iterable is unset.
     """
     return any(not e.is_set() for e in events)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based', 'event-based'], indirect=True)
-@pytest.mark.parametrize("weak,number_waiting", [(True, 2), (False, 2)])
+@pytest.mark.parametrize("weak, number_waiting", [
+    param(True, 2, marks=mark.weak),
+    (False, 2),
+])
 async def test_wait_for_dependencies(world: World, weak: bool, number_waiting: int):
     """
     Test waiting for dependencies and triggering them.
     """
     test_sim: SimRunner = world.sims["Sim-2"]
     pred_sim: SimRunner = world.sims["Sim-1"]
-    heappush(test_sim.next_steps, DenseTime(0))
-    test_sim.input_delays[pred_sim] = DenseTime(0, 1)
+    heappush(test_sim.next_steps, TieredTime(0))
+    test_sim.input_delays[pred_sim] = TieredInterval(0, 1)
     stalled = await does_coroutine_stall(
         scheduler.wait_for_dependencies(test_sim, True)
     )
     assert stalled
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
 async def test_wait_for_dependencies_all_done(world: World):
     """
     All dependencies already stepped far enough. No waiting required.
     """
-    heappush(world.sims["Sim-2"].next_steps, DenseTime(0))
+    heappush(world.sims["Sim-2"].next_steps, TieredTime(0))
     for dep_sid in ["Sim-0", "Sim-1"]:
-        world.sims[dep_sid].progress.value = DenseTime(1)
+        world.sims[dep_sid].progress.time = TieredTime(1)
     stalled = await does_coroutine_stall(
         scheduler.wait_for_dependencies(world.sims["Sim-2"], True),
-        pass_backs=3,
+        max_pass_backs=3,
     )
     assert not stalled
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
 @pytest.mark.parametrize("progress, should_stall", [(0, True), (1, False)])
 async def test_wait_for_dependencies_shifted(world: World, progress: int, should_stall: bool):
     """
     Shifted dependency has not/has stepped far enough. Waiting is/is not
     required.
     """
-    world.sims["Sim-5"].progress = Progress(DenseTime(progress))
+    world.sims["Sim-5"].progress = Progress(TieredTime(progress))
     # Move this simulators first step to 1
     sim_under_test = world.sims["Sim-4"]
-    sim_under_test.next_steps = [DenseTime(1)]
+    sim_under_test.next_steps = [TieredTime(1)]
     stalled = await does_coroutine_stall(
         scheduler.wait_for_dependencies(sim_under_test, lazy_stepping=False),
-        pass_backs=3,
+        max_pass_backs=3,
     )
     assert stalled == should_stall
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
 @pytest.mark.parametrize("lazy_stepping", [True, False])
 async def test_wait_for_dependencies_lazy(world: World, lazy_stepping: bool):
     """
     Test waiting for dependencies and triggering them.
     """
     sim_under_test = world.sims["Sim-1"]
-    sim_under_test.next_steps = [DenseTime(1)]
+    sim_under_test.next_steps = [TieredTime(1)]
     stalled = await does_coroutine_stall(
         scheduler.wait_for_dependencies(sim_under_test, lazy_stepping)
     )
     assert stalled == lazy_stepping
     if lazy_stepping:
         await does_coroutine_stall(
             scheduler.wait_for_dependencies(sim_under_test, True)
@@ -211,106 +249,111 @@
 def test_get_input_data(world: World):
     """
     Simple test for get_input_data().
     """
     sim_0 = world.sims["Sim-0"]
     sim_1 = world.sims["Sim-1"]
     sim_2 = world.sims["Sim-2"]
-    sim_2.current_step = DenseTime(0)
+    sim_2.current_step = TieredTime(0)
     sim_0.outputs = {0: {'1': {'x': 0, 'y': 1}}}
     sim_1.outputs = {0: {'2': {'x': 2, 'z': 4}}}
     sim_2.inputs_from_set_data = {
         '0': {'in': {'3': 5}, 'spam': {'3': 'eggs'}}
     }
-    sim_2.pulled_inputs[(sim_0, 0)] = [(('1', 'x'), ('0', 'in'))]
-    sim_2.pulled_inputs[(sim_1, 0)] = [(('2', 'z'), ('0', 'in'))]
+    sim_2.pulled_inputs[(sim_0, TieredInterval(0))] = set([(('1', 'x'), ('0', 'in'))])
+    sim_2.pulled_inputs[(sim_1, TieredInterval(0))] = set([(('2', 'z'), ('0', 'in'))])
     data = scheduler.get_input_data(world, sim_2)
     assert data == {'0': {
         'in': {'Sim-0.1': 0, 'Sim-1.2': 4, '3': 5},
         'spam': {'3': 'eggs'},
     }}
 
 
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
 def test_get_input_data_shifted(world: World):
     """
     Getting input data transmitted via a shifted connection.
     """
     sim_4 = world.sims["Sim-4"]
     sim_5 = world.sims["Sim-5"]
-    sim_4.current_step = DenseTime(0)
+    sim_4.current_step = TieredTime(0)
     sim_5.outputs = {-1: {'1': {'z': 7}}}
-    sim_4.pulled_inputs[(sim_5, 1)] = [(('1', 'z'), ('0', 'in'))]
+    sim_4.pulled_inputs[(sim_5, TieredInterval(1))] = set([(('1', 'z'), ('0', 'in'))])
     data = scheduler.get_input_data(world, world.sims["Sim-4"])
     assert data == {'0': {'in': {'Sim-5.1': 7}}}
 
 
 @pytest.mark.parametrize(
     'world, next_steps, next_step_s1, expected',
     [
-        ('time-based', [], DenseTime(2), 5),
-        ('time-based', [DenseTime(4)], DenseTime(2), 3),
-        ('event-based', [DenseTime(3)], None, 2),
-        ('event-based', [DenseTime(3)], DenseTime(2), 1),
+        ('time-based', [], TieredTime(2), 5),
+        ('time-based', [TieredTime(4)], TieredTime(2), 3),
+        ('event-based', [TieredTime(3)], None, 2),
+        ('event-based', [TieredTime(3)], TieredTime(2), 1),
     ],
     indirect=['world'],
 )
-def test_get_max_advance(world, next_steps, next_step_s1, expected):
+def test_get_max_advance(
+    world: World,
+    next_steps: List[TieredTime],
+    next_step_s1: TieredTime | None,
+    expected: int,
+):
     sim = world.sims["Sim-2"]
     sim.next_steps = next_steps
     sim.tqdm = tqdm(disable=True)
-    heappush(sim.next_steps, DenseTime(1))
+    heappush(sim.next_steps, TieredTime(1))
     sim.current_step = heappop(sim.next_steps)
 
     # In the event-based world, Sim-0 and Sim-1 are triggering ancestors
     # of Sim-2:
-    world.sims["Sim-0"].next_steps = [DenseTime(3)]
+    world.sims["Sim-0"].next_steps = [TieredTime(3)]
     if next_step_s1 is not None:
         heappush(world.sims["Sim-1"].next_steps, next_step_s1)
 
     max_advance = scheduler.get_max_advance(world, sim, until=5)
     assert max_advance == expected
 
 
 # TODO: Implement test/parameter for new API (passing max_advance)
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based', 'event-based'], indirect=True)
-async def test_step(world):
-    inputs = {}
+async def test_step(world: World):
+    inputs: InputData = {}
     sim = world.sims["Sim-0"]
     sim.tqdm = tqdm(disable=True)
     if sim.type == 'event-based':
-        heappush(sim.next_steps, DenseTime(0))
-    assert (sim.last_step, sim.next_steps[0]) == (DenseTime(-1), DenseTime(0))
+        heappush(sim.next_steps, TieredTime(0))
+    assert (sim.last_step, sim.next_steps[0]) == (TieredTime(-1), TieredTime(0))
     sim.current_step = heappop(sim.next_steps)
 
     await scheduler.step(world, sim, inputs, 0)
     assert (sim.last_step, sim.next_steps) == (
-        DenseTime(0), [DenseTime(1)] if sim.type == 'time-based' else []
+        TieredTime(0), [TieredTime(1)] if sim.type == 'time-based' else []
     )
 
 
 # TODO: Test also for output_time if 'time' is indicated by event-based sims
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world, cache',
                          [('time-based', True),
                           ('event-based', False)], indirect=['world'])
-async def test_get_outputs(world, cache):
+async def test_get_outputs(world: World, cache: bool):
     world.use_cache = cache
     sim = world.sims["Sim-0"]
     sim.outputs = {} if cache else None
     sim.output_request = {0: ['x', 'y']}
-    sim.last_step = DenseTime(0) 
-    sim.output_time = -1
+    sim.last_step = TieredTime(0) 
+    sim.output_time = TieredTime(-1)
     sim.tqdm = tqdm(disable=True)
 
     if sim.type == 'time-based':
         sim.current_step = heappop(sim.next_steps)
     else:
-        sim.current_step = DenseTime(0)
+        sim.current_step = TieredTime(0)
     await scheduler.get_outputs(world, sim)
 
     expected_output_cache = {
         0: {
             '0': {'x': 0, 'y': 1},
         },
         1: {
@@ -323,121 +366,126 @@
         assert sim.get_output_for(1) == expected_output_cache[1]
     else:
         with pytest.raises(AssertionError):
             sim.get_output_for(0)
         with pytest.raises(AssertionError):
             sim.get_output_for(1)
 
-    assert sim.output_time == DenseTime(0)
+    assert sim.output_time == TieredTime(0)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['event-based'], indirect=True)
 async def test_get_outputs_buffered(world: scenario.World):
     sim = world.sims["Sim-0"]
     sim.outputs = {}
-    sim.last_step = DenseTime(0)
-    sim.current_step = DenseTime(0)
+    sim.last_step = TieredTime(0)
+    sim.current_step = TieredTime(0)
     sim.tqdm = tqdm(disable=True)
     sim.output_request = {0: ['x', 'y', 'z']}
     sim.output_to_push = {
-        ('0', 'x'): [(world.sims["Sim-2"], 0, ('0', 'in'))],
-        ('0', 'z'): [(world.sims["Sim-1"], 0, ('0', 'in'))],
+        ('0', 'x'): [(world.sims["Sim-2"], TieredInterval(0), ('0', 'in'))],
+        ('0', 'z'): [(world.sims["Sim-1"], TieredInterval(0), ('0', 'in'))],
     }
 
     await scheduler.get_outputs(world, sim)
     assert world.sims["Sim-2"].timed_input_buffer.input_queue == [(0, 0, 'Sim-0.0', '0', 'in', 0)]
     assert world.sims["Sim-1"].timed_input_buffer.input_queue == []
 
 
 @pytest.mark.parametrize('world', ['event-based'], indirect=True)
 @pytest.mark.parametrize('output_time, next_steps', [
-    (DenseTime(1), [DenseTime(1), DenseTime(2)]),
-    (DenseTime(2), [DenseTime(2)]),
-    (DenseTime(3), [DenseTime(2), DenseTime(3)])],
+    (TieredTime(1), [TieredTime(1), TieredTime(2)]),
+    (TieredTime(2), [TieredTime(2)]),
+    (TieredTime(3), [TieredTime(2), TieredTime(3)])],
 )
 @pytest.mark.parametrize('progress', [2, 3])
-def test_notify_dependencies(world, output_time, next_steps, progress):
+def test_notify_dependencies(
+    world: World,
+    output_time: TieredTime,
+    next_steps: List[TieredTime],
+    progress: int,
+):
     sim = world.sims["Sim-0"]
     sim.progress = 0
 
     sim.data = {'1': {'x': 1}}
     sim.output_time = output_time
 
-    heappush(world.sims["Sim-2"].next_steps, DenseTime(2))
+    heappush(world.sims["Sim-2"].next_steps, TieredTime(2))
 
     scheduler.notify_dependencies(sim)
 
     assert world.sims["Sim-2"].next_steps == next_steps
 
 
 @pytest.mark.parametrize('world', ['event-based'], indirect=True)
-def test_notify_dependencies_trigger(world):
+def test_notify_dependencies_trigger(world: World):
     sim = world.sims["Sim-0"]
-    sim.progress = 0
+    sim.progress = Progress(TieredTime(0))
 
     sim.data = {'1': {'x': 1}}
-    sim.output_time = 1
+    sim.output_time = TieredTime(1)
     scheduler.notify_dependencies(sim)
 
-    assert world.sims["Sim-2"].next_steps == [DenseTime(1)]
+    assert world.sims["Sim-2"].next_steps == [TieredTime(1)]
 
 
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
-def test_prune_dataflow_cache(world):
-    world._df_cache = True
+def test_prune_dataflow_cache(world: World):
+    world.use_cache = True
     world.sims["Sim-0"].outputs = {
         0: {'spam': 'eggs'},
         1: {'foo': 'bar'},
     }
     for s in world.sims.values():
-        s.last_step = DenseTime(1)
+        s.last_step = TieredTime(1)
         s.tqdm = tqdm(disable=True)
     scheduler.prune_dataflow_cache(world)
 
     assert world.sims["Sim-0"].outputs == {
         1: {'foo': 'bar'},
     }
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('world', ['time-based'], indirect=True)
-async def test_get_outputs_shifted(world):
+async def test_get_outputs_shifted(world: World):
     sim = world.sims["Sim-5"]
     sim.outputs = {}
     sim.output_request = {0: ['x', 'y']}
     sim.type = 'time-based'
-    sim.progress = DenseTime(1)
-    sim.last_step = DenseTime(1)
+    sim.progress = Progress(TieredTime(1))
+    sim.last_step = TieredTime(1)
     sim.tqdm = tqdm(disable=True)
-    heappush(world.sims["Sim-4"].next_steps, 2)
+    heappush(world.sims["Sim-4"].next_steps, TieredTime(2))
     
     sim.current_step = heappop(sim.next_steps)
     await scheduler.get_outputs(world, sim)
     scheduler.notify_dependencies(sim)
     scheduler.prune_dataflow_cache(world)
     assert sim.outputs[1] == {
         '0': {'x': 0, 'y': 1},
     }
 
 
 def test_get_progress():
     class Sim:
         def __init__(self, time):
-            self.progress = Progress(DenseTime(time))
+            self.progress = Progress(TieredTime(time))
 
     sims = {i: Sim(0) for i in range(2)}
     assert scheduler.get_progress(sims, 4) == 0
 
-    sims[0].progress.value = DenseTime(1)
+    sims[0].progress.time = TieredTime(1)
     assert scheduler.get_progress(sims, 4) == 12.5
 
-    sims[0].progress.value = DenseTime(2)
+    sims[0].progress.time = TieredTime(2)
     assert scheduler.get_progress(sims, 4) == 25
 
-    sims[1].progress.value = DenseTime(3)
-    sims[0].progress.value = DenseTime(3)
+    sims[1].progress.time = TieredTime(3)
+    sims[0].progress.time = TieredTime(3)
     assert scheduler.get_progress(sims, 4) == 75
 
-    sims[0].progress.value = DenseTime(4)
-    sims[1].progress.value = DenseTime(4)
+    sims[0].progress.time = TieredTime(4)
+    sims[1].progress.time = TieredTime(4)
     assert scheduler.get_progress(sims, 4) == 100
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mosaik-3.3.0b1/tests/test_simmanager.py` & `mosaik-3.3.1/tests/test_simmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+from __future__ import annotations
+
 import asyncio
 from asyncio import StreamReader, StreamWriter
+import os
 from loguru import logger
 import pytest
 import sys
 import time
-from typing import Any, Callable, Coroutine, Optional, Type
+from typing import Any, Callable, Coroutine, Type, cast
 
 from example_sim.mosaik import ExampleSim
 from mosaik_api_v3 import Meta, __api_version__ as api_version
 import mosaik_api_v3.connection
 from mosaik_api_v3.connection import Channel, RemoteException
 
 from mosaik import proxies, scenario, simmanager, World
-from mosaik.dense_time import DenseTime
 from mosaik.exceptions import ScenarioError, SimulationError
 from mosaik.proxies import BaseProxy, LocalProxy
+from mosaik.tiered_time import TieredInterval, TieredTime
+
 
+VENV = os.path.dirname(sys.executable)
 
 sim_config: scenario.SimConfig = {
     "ExampleSimA": {
         "python": "example_sim.mosaik:ExampleSim",
     },
     "ExampleSimB": {
-        "cmd": "pyexamplesim %(addr)s",
+        "cmd": f"{VENV}/pyexamplesim %(addr)s",
         "cwd": ".",
     },
     "ExampleSimC": {
         "connect": "127.0.0.1:5556",
     },
     "ExampleSimD": {},  # type: ignore  # this is used for testing for this error
     "Fail": {
-        "cmd": 'python -c "import time; time.sleep(0.2)"',
+        "cmd": '%(python)s -c "import time; time.sleep(0.2)"',
     },
     "SimulatorMock": {
         "python": "tests.mocks.simulator_mock:SimulatorMock",
     },
     "MetaMock": {
         "python": "tests.simulators.meta_mirror:MetaMirror",
     },
@@ -118,15 +123,15 @@
     )
     assert isinstance(connection, LocalProxy)
     assert isinstance(connection.sim, ExampleSim)
     assert connection.sim.step_size == 2
 
 
 @pytest.mark.cmd_process
-def test_start_external_process(world):
+def test_start_external_process(world: World):
     """
     Test starting a simulator as external process."""
     proxy = world.loop.run_until_complete(
         simmanager.start(world, "ExampleSimB", "ExampleSim-0", 1.0, {})
     )
     assert "api_version" in proxy.meta and "models" in proxy.meta
     world.loop.run_until_complete(proxy.stop())
@@ -137,20 +142,38 @@
     with pytest.raises(SimulationError) as exc_info:
         world.loop.run_until_complete(simmanager.start(world, "Fail", "", 1.0, {}))
     assert (
         exc_info.value.args[0] == 'Simulator "Fail" did not connect to mosaik in time.'
     )
 
 
+@pytest.mark.asyncio
+async def test_start_proc_no_port_conflict():
+    mosaik_config: scenario.MosaikConfigTotal = {
+        "addr": ("0.0.0.0", None),
+        "start_timeout": 0,
+        "stop_timeout": 1,
+    }
+    mosaik_remote = cast(simmanager.MosaikRemote, None)
+    exc_1, exc_2 = await asyncio.gather(
+        simmanager.start_proc(mosaik_config, "Sim-1", {"cmd": "true"}, mosaik_remote),
+        simmanager.start_proc(mosaik_config, "Sim-2", {"cmd": "true"}, mosaik_remote),
+        return_exceptions=True,
+    )
+    # We should get `SimulationError`s here, not `OSError`s
+    assert isinstance(exc_1, SimulationError)
+    assert isinstance(exc_2, SimulationError)
+
+
 @pytest.mark.cmd_process
 def test_start_external_process_with_environment_variables(world, tmpdir):
     """
     Assert that you can set environment variables for a new sub-process.
     """
-    # Replace sim_config for this test:
+    # Replace sim_config for this test:z
     print(tmpdir.strpath)
     world.sim_config = {
         "SimulatorMockTmp": {
             "cmd": "%(python)s -m simulator_mock %(addr)s",
             "env": {
                 "PYTHONPATH": tmpdir.strpath,
             },
@@ -312,15 +335,15 @@
         world.shutdown()
 
 
 def test_start_init_error(caplog):
     """
     Test simulator crashing during init().
     """
-    world = scenario.World({"spam": {"cmd": "pyexamplesim %(addr)s"}})
+    world = scenario.World({"spam": {"cmd": f"{VENV}/pyexamplesim %(addr)s"}})
     try:
         with pytest.raises(SystemExit) as exc_info:
             world.loop.run_until_complete(
                 simmanager.start(world, "spam", "", 1.0, {"foo": 3})
             )
         assert (
             'Simulator "spam" closed its connection during the init() call.'
@@ -365,16 +388,16 @@
 def test_local_process(world):
     es = ExampleSim()
     proxy = LocalProxy(es, None)
     world.loop.run_until_complete(proxy.init("ExampleSim-0", time_resolution=1.0))
     sim = simmanager.SimRunner("ExampleSim-0", proxy)
     assert sim.sid == "ExampleSim-0"
     assert sim._proxy.sim is es
-    assert sim.last_step == DenseTime(-1)
-    assert sim.next_steps == [DenseTime(0)]
+    assert sim.last_step == TieredTime(-1)
+    assert sim.next_steps == [TieredTime(0)]
 
 
 def test_local_process_finalized(world):
     """
     Test that ``finalize()`` is called for local processes (issue #23).
     """
     simulator = world.start("SimulatorMock")
@@ -519,74 +542,75 @@
 ):
     world = scenario.World({})
     world.use_cache = True
 
     try:
         edges = [(0, 1), (0, 2), (1, 2), (2, 3)]
         edges = [("X.%s" % x, "X.%s" % y) for x, y in edges]
-        # world.df_graph.add_edge("X", "X", async_requests=True)
-        # world.df_graph.add_edge("Y", "X", async_requests=False)
-        # world.df_graph.add_node("Z")
         world.entity_graph.add_edges_from(edges)
         for node in world.entity_graph:
             world.entity_graph.add_node(node, sim="ExampleSim", type="A")
         world.sim_progress = 23
 
-        async def simulator():
-            reader, writer = await asyncio.open_connection("localhost", 5555)
+        async def simulator(host: str, port: int):
+            reader, writer = await asyncio.open_connection(host, port)
             channel = mosaik_api_v3.connection.Channel(reader, writer)
             try:
                 await rpc(channel, world)
             finally:
                 await channel.close()
 
-        async def greeter():
-            channel = await world.incoming_connections_queue.get()
+        async def greeter(channel_future: asyncio.Future[Channel]):
+            channel = await channel_future
             proxy_x = proxies.RemoteProxy(channel, simmanager.MosaikRemote(world, "X"))
             proxy_x._meta = {"type": "time-based", "models": {}}
             sim_x = simmanager.SimRunner("X", proxy_x)
-            sim_x.successors.add(sim_x)
-            sim_x.successors_to_wait_for.add(sim_x)
-            sim_x.last_step = DenseTime(1)
-            sim_x.current_step = DenseTime(0)
+            sim_x.successors[sim_x] = TieredInterval(0)
+            sim_x.successors_to_wait_for[sim_x] = TieredInterval(0)
+            sim_x.last_step = TieredTime(1)
+            sim_x.current_step = TieredTime(0)
             sim_x.is_in_step = True
             sim_x.outputs = {1: {"2": {"attr": "val"}}}
             world.sims["X"] = sim_x
             class DummyProxy:
                 @property
                 def meta(self):
                     return {"type": "time-based", "models": {}}
+                async def stop(self):
+                    pass
             sim_y = simmanager.SimRunner("Y", DummyProxy())
             world.sims["Y"] = sim_y
             sim_z = simmanager.SimRunner("Z", DummyProxy())
             world.sims["Z"] = sim_z
 
-            sim_x.successors.add(sim_y)
-            
+            sim_x.successors[sim_y] = TieredInterval(0)
 
         async def run():
-            sim_exc, greeter_exc = await asyncio.gather(
-                simulator(),
-                greeter(),
-                return_exceptions=True,
-            )
+            channel_future: asyncio.Future[Channel] = asyncio.Future()
+            async def on_connect(r: asyncio.StreamReader, w: asyncio.StreamWriter):
+                channel_future.set_result(Channel(r, w))
+            async with await asyncio.start_server(on_connect, "0.0.0.0") as server:
+                actual_addr = server.sockets[0].getsockname()
+                sim_exc, greeter_exc = await asyncio.gather(
+                    simulator(*actual_addr),
+                    greeter(channel_future),
+                    return_exceptions=True,
+                )
             assert greeter_exc is None
             if sim_exc:
                 raise sim_exc
 
         if err:
             with pytest.raises(err):
                 world.loop.run_until_complete(run())
         else:
             world.loop.run_until_complete(run())
 
     finally:
-        world.loop.run_until_complete(world.sims["X"].stop())
-        world.server.close()
-        world.loop.close()
+        world.shutdown()
 
 
 def test_timed_input_buffer():
     """Test TimedInputBuffer, especially if a lower value is added at the same
     time for the same connection.
     """
     buffer = simmanager.TimedInputBuffer()
```

### Comparing `mosaik-3.3.0b1/tests/test_tutorial.py` & `mosaik-3.3.1/tests/test_tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 CODE_DIR = os.path.join(os.path.abspath('.'), 'docs', 'tutorials', 'code')
 
 CASES = glob.glob(os.path.join(glob.escape(CODE_DIR), '*.out'))
 
 
 @pytest.mark.cmd_process
 @pytest.mark.parametrize('outfile', CASES)
-def test_tutorial(outfile):
+def test_tutorial(outfile: str):
     python_file = outfile.rsplit('.', 1)[0] + '.py'
     expected = open(outfile).read()
     out = subprocess.check_output([sys.executable, python_file], cwd=CODE_DIR,
                                   universal_newlines=True)
     assert out == expected
```

### Comparing `mosaik-3.3.0b1/tests/test_util.py` & `mosaik-3.3.1/tests/test_util.py`

 * *Files identical despite different names*

