# Comparing `tmp/dwave-inspector-0.4.4.tar.gz` & `tmp/dwave-inspector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-inspector-0.4.4.tar", last modified: Tue Dec  5 14:17:15 2023, max compression
+gzip compressed data, was "dwave-inspector-0.5.0.tar", last modified: Fri Apr 12 17:04:30 2024, max compression
```

## Comparing `dwave-inspector-0.4.4.tar` & `dwave-inspector-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-05 14:17:15.500880 dwave-inspector-0.4.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-12-05 14:17:15.500880 dwave-inspector-0.4.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3226 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-05 14:17:15.496880 dwave-inspector-0.4.4/dwave/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-05 14:17:15.500880 dwave-inspector-0.4.4/dwave/inspector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6610 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33419 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/adapters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1339 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1730 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/package_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2949 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/proxies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9554 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4851 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/storage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6758 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/dwave/inspector/viewers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-05 14:17:15.500880 dwave-inspector-0.4.4/dwave_inspector.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-12-05 14:17:15.000000 dwave-inspector-0.4.4/dwave_inspector.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-12-05 14:17:15.500880 dwave-inspector-0.4.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-12-05 14:16:45.000000 dwave-inspector-0.4.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 17:04:30.967925 dwave-inspector-0.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2024-04-12 17:04:30.967925 dwave-inspector-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3226 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 17:04:30.963925 dwave-inspector-0.5.0/dwave/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 17:04:30.963925 dwave-inspector-0.5.0/dwave/inspector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6610 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34379 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/adapters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1730 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/package_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2949 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/proxies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6658 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4897 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/storage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6638 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/dwave/inspector/viewers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 17:04:30.967925 dwave-inspector-0.5.0/dwave_inspector.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3988 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-12 17:04:30.000000 dwave-inspector-0.5.0/dwave_inspector.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-04-12 17:04:30.967925 dwave-inspector-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2593 2024-04-12 17:03:53.000000 dwave-inspector-0.5.0/setup.py
```

### Comparing `dwave-inspector-0.4.4/LICENSE` & `dwave-inspector-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/PKG-INFO` & `dwave-inspector-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-inspector
-Version: 0.4.4
+Version: 0.5.0
 Summary: D-Wave Problem Inspector tool
 Home-page: https://github.com/dwavesystems/dwave-inspector
 Author: D-Wave Systems Inc.
 Author-email: radomir@dwavesys.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dwave-inspector-0.4.4/README.rst` & `dwave-inspector-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/dwave/__init__.py` & `dwave-inspector-0.5.0/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/dwave/inspector/__init__.py` & `dwave-inspector-0.5.0/dwave/inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/dwave/inspector/adapters.py` & `dwave-inspector-0.5.0/dwave/inspector/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,27 +94,36 @@
 
     except KeyError:
         if hasattr(solver, 'edges') and hasattr(solver, 'nodes'):
             return {'type': 'chimera', 'shape': [16, 16, 4]}
 
     return default
 
-def solver_data_postprocessed(solver):
+def solver_data_postprocessed(solver, inplace=False):
     """Returns (possibly an old) solver's updated `data` that includes the
     missing properties like topology. Also, removes large unused properties.
+
+    Setting ``inplace`` flag will make permanent changes to ``solver`` data,
+    otherwise a copy will be returned.
     """
 
-    # make a copy to avoid modifying the original solver.data
-    data = copy.deepcopy(solver.data)
+    if inplace:
+        data = solver.data
+    else:
+        # make a copy to avoid modifying the original solver.data
+        data = copy.deepcopy(solver.data)
 
     # add missing but used properties
     data['properties'].setdefault('topology', _get_solver_topology(solver))
 
     # remove unused properties
-    del data['properties']['anneal_offset_ranges']
+    unused = {'anneal_offset_ranges'}
+    for key in unused:
+        if key in data['properties']:
+            del data['properties'][key]
 
     return data
 
 
 def _answer_dict(solutions, active_variables, energies, num_occurrences, timing, num_variables):
     return {
         "format": "qp",
@@ -156,14 +165,15 @@
         timing = {}
 
     default_annealing_time = solver.properties['default_annealing_time']
     default_programming_thermalization = solver.properties['default_programming_thermalization']
     default_readout_thermalization = solver.properties['default_readout_thermalization']
 
     # figure out `annealing_time`
+    # (valid for fast anneal as well)
     if "qpu_anneal_time_per_sample" in timing:
         # actual value is known
         annealing_time = timing["qpu_anneal_time_per_sample"]
     elif "annealing_time" in params:
         annealing_time = params["annealing_time"]
     elif "anneal_schedule" in params:
         anneal_schedule = params["anneal_schedule"]
@@ -179,36 +189,52 @@
 
     flux_biases = params.get('flux_biases')
     initial_state = params.get("initial_state")
 
     # set each parameter individually because defaults are not necessarily
     # constant; they can depend on one or more other parameters
     # TODO: cast to primary types for safe JSON serialization
-    return {
+    expanded = {
         "anneal_offsets": params.get("anneal_offsets"),
         "anneal_schedule": anneal_schedule,
         "annealing_time": annealing_time,
         "answer_mode": params.get("answer_mode", "histogram"),
         "auto_scale": params.get("auto_scale", True if not flux_biases else False),
-        "beta": params.get("beta", 10 if solver.is_vfyc else 1),
-        "chains": params.get("chains"),
         "flux_biases": flux_biases,
         "flux_drift_compensation": params.get("flux_drift_compensation", True),
         "h_gain_schedule": params.get("h_gain_schedule", [[0, 1], [annealing_time, 1]]),
         "initial_state": initial_state,
         "max_answers": params.get("max_answers"),
         "num_reads": params.get("num_reads", 1),
-        "num_spin_reversal_transforms": params.get("num_spin_reversal_transforms", 0),
-        "postprocess": params.get("postprocess", "sampling" if solver.is_vfyc else ""),
         "programming_thermalization": params.get("programming_thermalization", default_programming_thermalization),
         "readout_thermalization": params.get("readout_thermalization", default_readout_thermalization),
         "reduce_intersample_correlation": params.get("reduce_intersample_correlation", False),
         "reinitialize_state": params.get("reinitialize_state", True if initial_state else False)
     }
 
+    # num_spin_reversal_transforms has been removed from SAPI as of 2023-11-15
+    if "num_spin_reversal_transforms" in solver.parameters:
+        expanded.update(num_spin_reversal_transforms=params.get("num_spin_reversal_transforms", 0))
+
+    # post-processing and VFYC were last available on Chimera solvers, last
+    # of which (DW_2000Q_6) was decommissioned on 2023-05-31
+    if "postprocess" in solver.parameters:
+        expanded.update(postprocess=params.get("postprocess", "sampling" if solver.is_vfyc else ""))
+    if "beta" in solver.parameters:
+        expanded.update(beta=params.get("beta", 10 if solver.is_vfyc else 1))
+    if "chains" in solver.parameters:
+        expanded.update(chains=params.get("chains"))
+
+    # add fast anneal only if supported by the solver
+    if "fast_anneal" in solver.parameters:
+        expanded.update(fast_anneal=params.get("fast_anneal", False))
+
+    return expanded
+
+
 def _validated_problem_data(data):
     "Basic types validation/conversion."
 
     try:
         assert data['format'] == 'qp'
         assert isinstance(data['lin'], list)
         assert isinstance(data['quad'], list)
```

### Comparing `dwave-inspector-0.4.4/dwave/inspector/config.py` & `dwave-inspector-0.5.0/dwave/inspector/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,12 +35,26 @@
         return self._env('DWAVE_INSPECTOR_HOST', '127.0.0.1')
 
     @property
     def base_port(self):
         return int(self._env('DWAVE_INSPECTOR_BASE_PORT', 18000))
 
     @property
+    def max_port(self):
+        return int(self._env('DWAVE_INSPECTOR_MAX_PORT', 18999))
+
+    @property
+    def port_search_linear_tries(self):
+        # hard-code for now. unlikely users will want to control this from env
+        return 5
+
+    @property
+    def port_search_randomized_tries(self):
+        # hard-code for now. unlikely users will want to control this from env
+        return 50
+
+    @property
     def jupyter_server_proxy_external_url(self):
         return self._env('DWAVE_INSPECTOR_JUPYTER_SERVER_PROXY_EXTERNAL_URL')
 
 
 config = Config()
```

### Comparing `dwave-inspector-0.4.4/dwave/inspector/package_info.py` & `dwave-inspector-0.5.0/dwave/inspector/package_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     '__package_name__', '__title__', '__version__',
     '__author__', '__author_email__', '__description__',
     '__url__', '__license__', '__copyright__'
 ]
 
 __package_name__ = 'dwave-inspector'
 __title__ = 'D-Wave Problem Inspector'
-__version__ = '0.4.4'
+__version__ = '0.5.0'
 __author__ = 'D-Wave Systems Inc.'
 __author_email__ = 'radomir@dwavesys.com'
 __description__ = 'D-Wave Problem Inspector tool'
 __url__ = 'https://github.com/dwavesystems/dwave-inspector'
 __license__ = 'Apache 2.0'
 __copyright__ = '2019, D-Wave Systems Inc.'
 
@@ -35,15 +35,15 @@
     'title': 'D-Wave Problem Inspector',
     'description': 'This tool visualizes problems submitted to the quantum computer and the results returned.',
     'license': {
         'name': 'D-Wave EULA',
         'url': 'https://docs.ocean.dwavesys.com/eula',
     },
     'requirements': [
-        'dwave-inspectorapp==0.3.1',
+        'dwave-inspectorapp==0.3.3',
     ]
 }]
 
 
 # all entry point groups in one place
 entry_point_group = {
     'viewers': 'inspectorapp_viewers',
```

### Comparing `dwave-inspector-0.4.4/dwave/inspector/proxies.py` & `dwave-inspector-0.5.0/dwave/inspector/proxies.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/dwave/inspector/storage.py` & `dwave-inspector-0.5.0/dwave/inspector/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     if not problem_store:
         return None
 
     return next(reversed(problem_store))
 
 
-def get_solver_data(solver_id):
+def get_solver_data(solver_id, update_inplace=False):
     """Return solver data dict for `solver_id`. If solver hasn't been seen in
     any of the problems cached so far, fail with :exc:`KeyError`.
     """
     if solver_id in solvers:
-        return solver_data_postprocessed(solvers[solver_id])
+        return solver_data_postprocessed(solvers[solver_id], inplace=update_inplace)
 
     raise KeyError('solver not found')
```

### Comparing `dwave-inspector-0.4.4/dwave/inspector/utils.py` & `dwave-inspector-0.5.0/dwave/inspector/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 import re
 import sys
 import logging
 import operator
 import functools
 
-from typing import Sequence, Callable, Optional, Union, Dict
+from typing import Sequence, Callable, Optional, Union, Dict, Any
 from urllib.parse import urlparse, ParseResult
 
 try:
     from importlib.metadata import EntryPoint, DistributionFinder, Distribution
 except ImportError: # pragma: no cover
     from importlib_metadata import EntryPoint, DistributionFinder, Distribution
 
-import flask
-import numpy
+from flask.json.provider import JSONProvider
+import orjson
 
 __all__ = [
-    'itemsgetter', 'annotated', 'NumpyJSONProvider', 'patch_entry_points',
+    'itemsgetter', 'annotated', 'OrJSONProvider', 'patch_entry_points',
     'RichDisplayURL',
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def itemsgetter(*items):
@@ -76,37 +76,30 @@
         for key, val in kwargs.items():
             setattr(f, key, val)
         return f
 
     return _decorator
 
 
-# adapted from dwave-hybrid utils
-# (https://github.com/dwavesystems/dwave-hybrid/blob/b9025b5bb3d88dce98ec70e28cfdb25400a10e4a/hybrid/utils.py#L43-L61)
-# to provide numpy types serialization in flask 2.2+ (see https://github.com/pallets/flask/pull/4692)
-class NumpyJSONProvider(flask.json.provider.DefaultJSONProvider):
-    """JSON encoder for numpy types.
-
-    Supported types:
-     - basic numeric types: booleans, integers, floats
-     - arrays: ndarray, recarray
+# provide faster json serialization in flask 2.2+, with numpy support
+# (see https://github.com/pallets/flask/pull/4692)
+class OrJSONProvider(JSONProvider):
+    """Flask-specialized JSON encoder/decoder that uses ``orjson``.
+
+    By default, NumPy types are serialized, and non-string keys are supported.
     """
 
-    @staticmethod
-    def default(obj):
-        if isinstance(obj, numpy.integer):
-            return int(obj)
-        elif isinstance(obj, numpy.floating):
-            return float(obj)
-        elif isinstance(obj, numpy.bool_):
-            return bool(obj)
-        elif isinstance(obj, numpy.ndarray):
-            return obj.tolist()
+    def loads(self, s: str, **kwargs: Any) -> Any:
+        return orjson.loads(s, **kwargs)
 
-        return super().default(obj)
+    def dumps(self, obj: Any, **kwargs: Any) -> bytes:
+        kwargs.setdefault('option', (orjson.OPT_SERIALIZE_NUMPY
+                                     | orjson.OPT_NON_STR_KEYS
+                                     | orjson.OPT_NAIVE_UTC))
+        return orjson.dumps(obj, **kwargs)
 
 
 # TODO: move to `dwave.common.testing` or similar
 class patch_entry_points:
     """Patch entry points via an in-memory-installed distribution that provides
     the new (temporary) entry points.
     """
@@ -189,15 +182,15 @@
             path=lambda src, dst: f'{dst.path}{src.path}')
 
         assert(url, 'https://example.com/prefix/notebook?usernmae=lisa')
 
     """
 
     # handle schemeless urls -> assume http
-    if not re.match("^\w+://", url):
+    if not re.match(r"^\w+://", url):
         url = f"http://{url}"
 
     # deconstruct source and patch urls
     if not isinstance(url, ParseResult):
         url = urlparse(url)
     if not isinstance(patch, ParseResult):
         patch = urlparse(patch)
```

### Comparing `dwave-inspector-0.4.4/dwave/inspector/viewers.py` & `dwave-inspector-0.5.0/dwave/inspector/viewers.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/dwave_inspector.egg-info/PKG-INFO` & `dwave-inspector-0.5.0/dwave_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-inspector
-Version: 0.4.4
+Version: 0.5.0
 Summary: D-Wave Problem Inspector tool
 Home-page: https://github.com/dwavesystems/dwave-inspector
 Author: D-Wave Systems Inc.
 Author-email: radomir@dwavesys.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dwave-inspector-0.4.4/dwave_inspector.egg-info/SOURCES.txt` & `dwave-inspector-0.5.0/dwave_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.4/setup.py` & `dwave-inspector-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,19 @@
     exec(f.read(), package_info)
 
 
 # Package requirements, minimal pinning
 install_requires = [
     'dimod>=0.10.0',
     'dwave-system>=1.3.0',
-    'dwave-cloud-client>=0.8.3',    # for <0.10.6, also pydantic<2 is required!
-    'Flask>=2.2',
+    'dwave-cloud-client>=0.11.0,<0.12.0',
+    'Flask>=2.2,<4',
     'numpy',
-    # dwave-inspectorapp==0.3.1
+    'orjson>=3.10.0',
+    # dwave-inspectorapp==0.3.3
 ]
 
 # Package extras requirements
 extras_require = {
     'test': ['coverage', 'vcrpy'],
 
     # importlib.resources backport needed for reading distribution data files
```

