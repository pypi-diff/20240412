# Comparing `tmp/oil_reservoir_synthesizer-0.2.0.tar.gz` & `tmp/oil_reservoir_synthesizer-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oil_reservoir_synthesizer-0.2.0.tar", last modified: Fri Dec  8 10:21:09 2023, max compression
+gzip compressed data, was "oil_reservoir_synthesizer-0.2.1b0.tar", last modified: Fri Apr 12 11:24:27 2024, max compression
```

## Comparing `oil_reservoir_synthesizer-0.2.0.tar` & `oil_reservoir_synthesizer-0.2.1b0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.909087 oil_reservoir_synthesizer-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.909087 oil_reservoir_synthesizer-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.909087 oil_reservoir_synthesizer-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_oil_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_perlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_prime_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_shaped_perlin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-08 10:21:09.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-08 10:21:09.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 10:21:09.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-08 10:21:09.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-08 10:21:09.000000 oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:09.913087 oil_reservoir_synthesizer-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/tests/test_oil_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-08 10:21:01.000000 oil_reservoir_synthesizer-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.558466 oil_reservoir_synthesizer-0.2.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.558466 oil_reservoir_synthesizer-0.2.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.558466 oil_reservoir_synthesizer-0.2.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_oil_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_perlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_prime_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_shaped_perlin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 11:24:27.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 11:24:27.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:24:27.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 11:24:27.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 11:24:27.000000 oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:27.562466 oil_reservoir_synthesizer-0.2.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/tests/test_oil_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-12 11:24:23.000000 oil_reservoir_synthesizer-0.2.1b0/tox.ini
```

### Comparing `oil_reservoir_synthesizer-0.2.0/.github/workflows/testing.yml` & `oil_reservoir_synthesizer-0.2.1b0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `oil_reservoir_synthesizer-0.2.0/CODE_OF_CONDUCT.md` & `oil_reservoir_synthesizer-0.2.1b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `oil_reservoir_synthesizer-0.2.0/COPYING` & `oil_reservoir_synthesizer-0.2.1b0/COPYING`

 * *Files identical despite different names*

### Comparing `oil_reservoir_synthesizer-0.2.0/PKG-INFO` & `oil_reservoir_synthesizer-0.2.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oil_reservoir_synthesizer
-Version: 0.2.0
+Version: 0.2.1b0
 Summary: A generator for synthetic oil reservoir values
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/oil_reservoir_synthesizer
 Project-URL: Repository, https://github.com/equinor/oil_reservoir_synthesizer
 Project-URL: Bug Tracker, https://github.com/equinor/oil_reservoir_synthesizer/issues
@@ -42,16 +42,16 @@
 ```python
 
 from oil_reservoir_synthesizer import OilSimulator
 
 simulator = OilSimulator()
 
 # Build a model with one well and block
-simulator.addWell("wellName", seed=997)
-simulator.addBlock("5,5,5", seed=31)
+simulator.add_well("wellName", seed=997)
+simulator.add_block("5,5,5", seed=31)
 
 # Run simulation
 num_steps = 10
 fopr_values = []  # oil production rate for each time step
 for time_steps in range(num_steps):
     simulator.step(scale=1.0 / num_steps)
     fopr_values.append(simulator.fopr())
```

### Comparing `oil_reservoir_synthesizer-0.2.0/README.md` & `oil_reservoir_synthesizer-0.2.1b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 ```python
 
 from oil_reservoir_synthesizer import OilSimulator
 
 simulator = OilSimulator()
 
 # Build a model with one well and block
-simulator.addWell("wellName", seed=997)
-simulator.addBlock("5,5,5", seed=31)
+simulator.add_well("wellName", seed=997)
+simulator.add_block("5,5,5", seed=31)
 
 # Run simulation
 num_steps = 10
 fopr_values = []  # oil production rate for each time step
 for time_steps in range(num_steps):
     simulator.step(scale=1.0 / num_steps)
     fopr_values.append(simulator.fopr())
```

### Comparing `oil_reservoir_synthesizer-0.2.0/SECURITY.md` & `oil_reservoir_synthesizer-0.2.1b0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `oil_reservoir_synthesizer-0.2.0/pyproject.toml` & `oil_reservoir_synthesizer-0.2.1b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -39,7 +39,28 @@
 dev = [
     "pytest",
     "tox",
     "pre-commit"
 ]
 
 [tool.setuptools_scm]
+
+[tool.ruff]
+src = ["src"]
+select = [
+  "W",   # pycodestyle
+  "I",   # isort
+  "B",   # flake-8-bugbear
+  "SIM", # flake-8-simplify
+  "F",   # pyflakes
+  "PL",  # pylint
+]
+
+[tool.pylint]
+disable = [
+  "missing-class-docstring",
+  "missing-docstring",
+  "missing-module-docstring",
+  "too-few-public-methods",
+  "too-many-arguments",
+  "too-many-instance-attributes",
+]
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_oil_simulator.py` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_oil_simulator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+# ruff: noqa: PLR2004
+from warnings import warn
+
 from ._shaped_perlin import ShapeCreator, ShapeFunction
 
 
 class OilSimulator:
+    # pylint: disable=too-many-public-methods
     """OilSimulator is the builder of the model and the generator of the values.
 
 
     Generates oil simulator values based on perlin-noise.
 
     :param ooip: Oil in place for the entire field at initial conditions.
     :param goip: Gas in place for the entire field at initial conditions.
@@ -24,18 +28,18 @@
     B_DIVERGENCE = ShapeFunction([0.0, 0.5, 0.7, 0.9, 1.0], [0.0, 0.1, 0.2, 0.3, 0.5])
 
     def __init__(self, ooip=2000, goip=2500, woip=2250):
         self._foip = self.ooip = ooip
         self._fgip = self.goip = goip
         self._fwip = self.woip = woip
 
-        self._oprFunc = {}  # Oil production rate function for each well
-        self._gprFunc = {}  # Gas production rate function for each well
-        self._wprFunc = {}  # Water produtcion rate function for each well
-        self._bprFunc = {}  # Pressure function for each block
+        self._opr_func = {}  # Oil production rate function for each well
+        self._gpr_func = {}  # Gas production rate function for each well
+        self._wpr_func = {}  # Water produtcion rate function for each well
+        self._bpr_func = {}  # Pressure function for each block
         self._current_step = 0
 
         self._fopt = 0.0  # Oil production total for entire reservoir
         self._fopr = 0.0  # Oil production rate for entire reservoir
         self._fgpt = 0.0  # Gas production tota for entire reservoir
         self._fgpr = 0.0  # Gas production rate for entire reservoir
         self._fwpt = 0.0  # Water production total for entire reservoir
@@ -43,40 +47,47 @@
 
         self._fgor = 0.0  # Gas oil ratio for entire reservoir
         self._fwct = 0.0  # water cut for entire reservoir
 
         self._wells = {}
         self._bpr = {}  # Block pressure for each block
 
-    def addWell(
+    def addWell(self, *args, **kwargs):
+        # pylint: disable=invalid-name
+        warn(
+            "addWell() is deprecated. Use add_well().", DeprecationWarning, stacklevel=2
+        )
+        self.add_well(*args, **kwargs)
+
+    def add_well(  # noqa: PLR0913
         self, name, seed, persistence=0.2, octaves=8, divergence_scale=1.0, offset=0.0
     ):
         """Add a well to the simulator model."""
-        oil_div = OilSimulator.O_DIVERGENCE.scaledCopy(divergence_scale)
-        gas_div = OilSimulator.G_DIVERGENCE.scaledCopy(divergence_scale)
-        water_div = OilSimulator.W_DIVERGENCE.scaledCopy(divergence_scale)
-        self._oprFunc[name] = ShapeCreator.createNoiseFunction(
+        oil_div = OilSimulator.O_DIVERGENCE.scaled_copy(divergence_scale)
+        gas_div = OilSimulator.G_DIVERGENCE.scaled_copy(divergence_scale)
+        water_div = OilSimulator.W_DIVERGENCE.scaled_copy(divergence_scale)
+        self._opr_func[name] = ShapeCreator.create_noise_function(
             OilSimulator.OPR_SHAPE,
             oil_div,
             seed,
             persistence=persistence,
             octaves=octaves,
             cutoff=0.0,
             offset=offset,
         )
-        self._gprFunc[name] = ShapeCreator.createNoiseFunction(
+        self._gpr_func[name] = ShapeCreator.create_noise_function(
             OilSimulator.GPR_SHAPE,
             gas_div,
             seed * 7,
             persistence=persistence * 3.5,
             octaves=octaves / 2,
             cutoff=0.0,
             offset=offset,
         )
-        self._wprFunc[name] = ShapeCreator.createNoiseFunction(
+        self._wpr_func[name] = ShapeCreator.create_noise_function(
             OilSimulator.WPR_SHAPE,
             water_div,
             seed * 11,
             persistence=persistence,
             octaves=octaves,
             cutoff=0.0,
             offset=offset,
@@ -87,17 +98,26 @@
             "opt": 0.0,
             "gpr": 0.0,
             "gpt": 0.0,
             "wpr": 0.0,
             "wpt": 0.0,
         }
 
-    def addBlock(self, name, seed, persistence=0.2):
+    def addBlock(self, *args, **kwargs):
+        # pylint: disable=invalid-name
+        warn(
+            "addBlock() is deprecated. Use add_block().",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self.add_block(*args, **kwargs)
+
+    def add_block(self, name, seed, persistence=0.2):
         """Add a grid block to the model"""
-        self._bprFunc[name] = ShapeCreator.createNoiseFunction(
+        self._bpr_func[name] = ShapeCreator.create_noise_function(
             OilSimulator.BPR_SHAPE,
             OilSimulator.B_DIVERGENCE,
             seed,
             persistence=persistence,
             cutoff=0.0,
         )
         self._bpr[name] = 0.0
@@ -109,20 +129,20 @@
         """
         self._fopr = 0.0
         self._fgpr = 0.0
         self._fwpr = 0.0
         self._fgor = 0.0
         self._fwct = 0.0
         for key, well in self._wells.items():
-            oprFunction = self._oprFunc[key]
-            gprFunction = self._gprFunc[key]
-            wprFunction = self._wprFunc[key]
-            opr_value = oprFunction(self._current_step, scale)
-            gpr_value = gprFunction(self._current_step, scale)
-            wpr_value = wprFunction(self._current_step, scale)
+            opr_function = self._opr_func[key]
+            gpr_function = self._gpr_func[key]
+            wpr_function = self._wpr_func[key]
+            opr_value = opr_function(self._current_step, scale)
+            gpr_value = gpr_function(self._current_step, scale)
+            wpr_value = wpr_function(self._current_step, scale)
 
             if self._foip > 0.0:
                 well["opr"] = opr_value
                 well["opt"] += opr_value
                 self._fopr += opr_value
 
             if self._fgip > 0.0:
@@ -152,16 +172,16 @@
         self._fgpt += self._fgpr
         self._fwpt += self._fwpr
 
         self._fgor /= len(self._wells)
         self._fwct /= len(self._wells)
 
         for key in self._bpr:
-            bprFunction = self._bprFunc[key]
-            self._bpr[key] = bprFunction(self._current_step, scale)
+            bpr_function = self._bpr_func[key]
+            self._bpr[key] = bpr_function(self._current_step, scale)
 
         self._current_step += 1
 
     def fopt(self):
         """Get the field oil production total at the current time."""
         return self._fopt
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_perlin.py` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_perlin.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,58 +8,58 @@
         self.persistence = persistence
         self.number_of_octaves = number_of_octaves
 
         self.octave_primes = (
             prime_generator if prime_generator is not None else PrimeGenerator()
         )
 
-    def cosineInterpolation(self, a, b, x):
+    def cosine_interppolation(self, a, b, x):
         ft = x * 3.1415927
         f = (1.0 - math.cos(ft)) * 0.5
         return a * (1 - f) + b * f
 
     MAX_INT = (1 << 31) - 1
 
     def noise(self, x, perturbation):
         x += perturbation
         x = ((x << 13) & PerlinNoise.MAX_INT) ^ x
         x = (x * (x * x * 15731 + 789221) + 1376312589) & PerlinNoise.MAX_INT
         return 1.0 - x / 1073741824.0
 
-    def smoothedNoise(self, x, perturbation):
+    def smoothed_noise(self, x, perturbation):
         return (
             self.noise(x, perturbation) / 2.0
             + self.noise(x - 1, perturbation) / 4.0
             + self.noise(x + 1, perturbation) / 4.0
         )
 
-    def interpolatedNoise(self, x, octave_number):
+    def interpolated_noise(self, x, octave_number):
         int_x = int(x)
         frac_x = x - int_x
 
         perturbation = self.octave_primes[octave_number]
 
-        v1 = self.smoothedNoise(int_x, perturbation)
-        v2 = self.smoothedNoise(int_x + 1, perturbation)
+        v1 = self.smoothed_noise(int_x, perturbation)
+        v2 = self.smoothed_noise(int_x + 1, perturbation)
 
-        return self.cosineInterpolation(v1, v2, frac_x)
+        return self.cosine_interppolation(v1, v2, frac_x)
 
-    def perlinNoise1D(self, x):
+    def perlin_noise_1d(self, x):
         total = 0.0
 
         for octave in range(int(self.number_of_octaves) - 1):
             frequency = math.pow(2, octave)
             amplitude = math.pow(self.persistence, octave)
 
             total += (
-                self.interpolatedNoise(x * frequency, octave_number=octave) * amplitude
+                self.interpolated_noise(x * frequency, octave_number=octave) * amplitude
             )
 
         return total
 
     def __getitem__(self, x):
         """:rtype: float"""
-        return self.perlinNoise1D(x * 10.0)
+        return self.perlin_noise_1d(x * 10.0)
 
     def __call__(self, x):
         """:rtype: float"""
         return self[x]
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_prime_generator.py` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_prime_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         random.seed(seed)
 
     def __getitem__(self, index):
         if not isinstance(index, numbers.Rational) or index < 0:
             raise IndexError(f"Index must be a positive integer: {index}")
 
         if index not in self.__primes:
-            p1 = self.randomPrime()
+            p1 = self.random_prime()
             self.__primes[index] = p1
 
         return self.__primes[index]
 
-    def randomPrime(self):
+    def random_prime(self):
         random_index = self.__random.randint(0, len(PrimeGenerator.LIST_OF_PRIMES) - 1)
         return PrimeGenerator.LIST_OF_PRIMES[random_index]
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer/_shaped_perlin.py` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer/_shaped_perlin.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,128 +18,133 @@
             y = self.y[len(self.x) - 1]
         else:
             y = None
             for i in range(len(self.x) - 1):
                 if self.x[i] <= x < self.x[i + 1]:
                     x_diff = self.x[i + 1] - self.x[i]
                     frac_x = (x - self.x[i]) / x_diff
-                    y = self.cosineInterpolation(self.y[i], self.y[i + 1], frac_x)
+                    y = self.cosine_interpolation(self.y[i], self.y[i + 1], frac_x)
                     break
 
         return y
 
-    def cosineInterpolation(self, a, b, x):
+    def cosine_interpolation(self, a, b, x):
         ft = x * 3.1415927
         f = (1.0 - math.cos(ft)) * 0.5
         return a * (1 - f) + b * f
 
 
 class ShapeFunction:
     def __init__(self, x, y, scale=1.0):
         self.scale = scale
         self.interpolator = Interpolator(x, y)
 
     def __call__(self, x):
         return self.interpolator(x) * self.scale
 
-    def scaledCopy(self, scale=1.0):
+    def scaled_copy(self, scale=1.0):
         return ShapeFunction(self.interpolator.x, self.interpolator.y, scale)
 
 
 class ConstantShapeFunction(ShapeFunction):
     def __init__(self, value):
         super().__init__([0.0], [value])
 
 
 class ShapedNoise:
-    def __init__(
-        self, noiseFunction, shapeFunction, divergenceFunction, offset=0.0, cutoff=None
+    def __init__(  # noqa: PLR0913
+        self,
+        noise_function,
+        shape_function,
+        divergence_function,
+        offset=0.0,
+        cutoff=None,
     ):
-        self.shapeFunction = shapeFunction
-        self.divergenceFunction = divergenceFunction
-        self.noiseFunction = noiseFunction
+        self.shape_function = shape_function
+        self.divergence_function = divergence_function
+        self.noise_function = noise_function
         self.offset = offset
         self.cutoff = cutoff
 
     def __call__(self, x, scale=1.0):
         scaled_x = x * scale
-        result = self.shapeFunction(scaled_x) + self.noiseFunction(
+        result = self.shape_function(scaled_x) + self.noise_function(
             scaled_x
-        ) * self.divergenceFunction(scaled_x)
+        ) * self.divergence_function(scaled_x)
         result += self.offset
         if self.cutoff is not None:
             result = max(result, self.cutoff)
         return result
 
 
 class ShapeCreator:
     @staticmethod
-    def createShapeFunction(count=1000, persistence=0.2, octaves=8, seed=1):
-        """@rtype: ShapeFunction"""
+    def createshape_function(count=1000, persistence=0.2, octaves=8, seed=1):
+        """@rtype: shape_function"""
         prime_generator = PrimeGenerator(seed=seed)
         perlininator = PerlinNoise(
             persistence=persistence,
             number_of_octaves=octaves,
             prime_generator=prime_generator,
         )
 
         x_values = [x / float(count) for x in range(count)]
         y_values = [perlininator(x) for x in x_values]
 
         return ShapeFunction(x_values, y_values)
 
     @staticmethod
-    def createShapedPerlinFunction(
+    def create_shaped_perlin_function(  # noqa: PLR0913
         divergence_x,
         divergence_y,
         shape_seed=None,
         perlin_seed=None,
         count=1000,
         persistence=0.2,
         octaves=8,
         offset=0.0,
         cutoff=None,
     ):
         """@rtype: ShapedNoise"""
-        shapeFunction = ShapeCreator.createShapeFunction(
+        shape_function = ShapeCreator.createshape_function(
             count, persistence, octaves, shape_seed
         )
-        divergenceFunction = ShapeFunction(divergence_x, divergence_y)
+        divergence_function = shape_function(divergence_x, divergence_y)
         prime_generator = PrimeGenerator(perlin_seed)
         perlin_noise = PerlinNoise(persistence, octaves, prime_generator)
 
         return ShapedNoise(
             perlin_noise,
-            shapeFunction,
-            divergenceFunction,
+            shape_function,
+            divergence_function,
             offset=offset,
             cutoff=cutoff,
         )
 
     @staticmethod
-    def createNoiseFunction(
-        shapeFunction=None,
-        divergenceFunction=None,
+    def create_noise_function(  # noqa: PLR0913
+        shape_function=None,
+        divergence_function=None,
         seed=None,
         persistence=0.2,
         octaves=8,
         offset=0.0,
         cutoff=None,
     ):
         """@rtype: ShapedNoise"""
-        if shapeFunction is None:
-            shapeFunction = ConstantShapeFunction(0.0)
+        if shape_function is None:
+            shape_function = ConstantShapeFunction(0.0)
 
-        if divergenceFunction is None:
-            divergenceFunction = ConstantShapeFunction(1.0)
+        if divergence_function is None:
+            divergence_function = ConstantShapeFunction(1.0)
 
         prime_generator = PrimeGenerator(seed)
         perlin_noise = PerlinNoise(persistence, octaves, prime_generator)
 
         noise = ShapedNoise(
             perlin_noise,
-            shapeFunction,
-            divergenceFunction,
+            shape_function,
+            divergence_function,
             offset=offset,
             cutoff=cutoff,
         )
         return noise
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/PKG-INFO` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oil-reservoir-synthesizer
-Version: 0.2.0
+Name: oil_reservoir_synthesizer
+Version: 0.2.1b0
 Summary: A generator for synthetic oil reservoir values
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/oil_reservoir_synthesizer
 Project-URL: Repository, https://github.com/equinor/oil_reservoir_synthesizer
 Project-URL: Bug Tracker, https://github.com/equinor/oil_reservoir_synthesizer/issues
@@ -42,16 +42,16 @@
 ```python
 
 from oil_reservoir_synthesizer import OilSimulator
 
 simulator = OilSimulator()
 
 # Build a model with one well and block
-simulator.addWell("wellName", seed=997)
-simulator.addBlock("5,5,5", seed=31)
+simulator.add_well("wellName", seed=997)
+simulator.add_block("5,5,5", seed=31)
 
 # Run simulation
 num_steps = 10
 fopr_values = []  # oil production rate for each time step
 for time_steps in range(num_steps):
     simulator.step(scale=1.0 / num_steps)
     fopr_values.append(simulator.fopr())
```

### Comparing `oil_reservoir_synthesizer-0.2.0/src/oil_reservoir_synthesizer.egg-info/SOURCES.txt` & `oil_reservoir_synthesizer-0.2.1b0/src/oil_reservoir_synthesizer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 COPYING
 README.md
 SECURITY.md
 pyproject.toml
-setup.cfg
 tox.ini
 .github/workflows/publish_to_pypi.yml
 .github/workflows/style.yml
 .github/workflows/testing.yml
 src/oil_reservoir_synthesizer/__init__.py
 src/oil_reservoir_synthesizer/_oil_simulator.py
 src/oil_reservoir_synthesizer/_perlin.py
```

### Comparing `oil_reservoir_synthesizer-0.2.0/tests/test_oil_simulator.py` & `oil_reservoir_synthesizer-0.2.1b0/tests/test_oil_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from oil_reservoir_synthesizer import OilSimulator
 
 EXPECTED_VALUES = [
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 1.0],
     [
         0.36223552960708655,
         0.36223552960708655,
@@ -148,16 +149,16 @@
         0.09156245545255788,
     ],
 ]
 
 
 def test_oil_simulator():
     sim = OilSimulator()
-    sim.addWell("OP1", seed=1)
-    sim.addBlock("6,6,6", seed=2)
+    sim.add_well("OP1", seed=1)
+    sim.add_block("6,6,6", seed=2)
 
     for report_step in range(10):
         sim.step(scale=1.0 / 10.0)
 
         values = [
             sim.fopr(),
             sim.fopt(),
```

