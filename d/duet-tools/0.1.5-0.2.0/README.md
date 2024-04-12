# Comparing `tmp/duet-tools-0.1.5.tar.gz` & `tmp/duet_tools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duet-tools-0.1.5.tar", last modified: Tue Mar 26 15:45:42 2024, max compression
+gzip compressed data, was "duet_tools-0.2.tar", last modified: Fri Apr 12 20:49:56 2024, max compression
```

## Comparing `duet-tools-0.1.5.tar` & `duet_tools-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:45:42.761369 duet-tools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-26 15:45:31.000000 duet-tools-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-26 15:45:42.761369 duet-tools-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-26 15:45:31.000000 duet-tools-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:45:42.757368 duet-tools-0.1.5/duet_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25671 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:45:42.757368 duet-tools-0.1.5/duet_tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/data/sb40_parameters.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/landfire.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-26 15:45:31.000000 duet-tools-0.1.5/duet_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:45:42.761369 duet-tools-0.1.5/duet_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-26 15:45:42.000000 duet-tools-0.1.5/duet_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-26 15:45:42.000000 duet-tools-0.1.5/duet_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 15:45:42.000000 duet-tools-0.1.5/duet_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 15:45:42.000000 duet-tools-0.1.5/duet_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 15:45:42.000000 duet-tools-0.1.5/duet_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 15:45:42.761369 duet-tools-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-26 15:45:31.000000 duet-tools-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:45:42.761369 duet-tools-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-03-26 15:45:31.000000 duet-tools-0.1.5/tests/test_calibration_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:56.420755 duet_tools-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-12 20:49:48.000000 duet_tools-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 20:49:56.420755 duet_tools-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 20:49:48.000000 duet_tools-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:56.420755 duet_tools-0.2/duet_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26925 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:56.420755 duet_tools-0.2/duet_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/data/sb40_parameters.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/landfire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-12 20:49:48.000000 duet_tools-0.2/duet_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:56.420755 duet_tools-0.2/duet_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 20:49:56.000000 duet_tools-0.2/duet_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-12 20:49:56.000000 duet_tools-0.2/duet_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:49:56.000000 duet_tools-0.2/duet_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 20:49:56.000000 duet_tools-0.2/duet_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 20:49:56.000000 duet_tools-0.2/duet_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:49:56.420755 duet_tools-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-12 20:49:48.000000 duet_tools-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:49:56.420755 duet_tools-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-12 20:49:48.000000 duet_tools-0.2/tests/test_calibration_module.py
```

### Comparing `duet-tools-0.1.5/LICENSE` & `duet_tools-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/PKG-INFO` & `duet_tools-0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duet-tools
-Version: 0.1.5
+Version: 0.2.0
 Summary: Output management tools for LANL DUET program
 Home-page: https://github.com/nmc-cafes/duet-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nmc-cafes/duet-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duet-tools-0.1.5/duet_tools/__init__.py` & `duet_tools-0.2/duet_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/duet_tools/calibration.py` & `duet_tools-0.2/duet_tools/calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 
 class Targets:
     """
     Class containing and validating target methods and values for fuel parameters.
     """
 
-    def __init__(self, method: str, args: list(str), targets: list):
+    def __init__(self, method: str, args: list[str], targets: list):
         self.method = self._validate_method(method)
         self.args, self.targets = self._validate_target_args(method, args, targets)
         self.calibration_function = self._get_calibration_function(method)
 
     def _get_calibration_function(self, method):
         if method == "maxmin":
             return _maxmin_calibration
@@ -170,15 +170,15 @@
         methods_allowed = ["maxmin", "meansd", "constant"]
         if method not in methods_allowed:
             raise ValueError(
                 f"Method {method} not supported. Must be one of {methods_allowed}"
             )
         return method
 
-    def _validate_target_args(self, method: str, args: list(str), targets: list(float)):
+    def _validate_target_args(self, method: str, args: list[str], targets: list[float]):
         method_dict = {
             "constant": ["value"],
             "maxmin": ["max", "min"],
             "meansd": ["mean", "sd"],
         }
         args_allowed = method_dict.get(method)
         if set(args_allowed) != set(args):
@@ -199,15 +199,15 @@
 
 class FuelParameter:
     """
     Class containing and validating calibration targets for a single fuel parameter. Targets can
     be set for multiple fuel types.
     """
 
-    def __init__(self, parameter: str, fuel_types: list(str), targets: list(Targets)):
+    def __init__(self, parameter: str, fuel_types: list[str], targets: list[Targets]):
         self.parameter = self._validate_fuel_parameter(parameter)
         self.fuel_types = self._validate_fuel_types(fuel_types)
         self.targets = targets
 
     def _validate_fuel_types(self, fuel_types):
         fueltypes_allowed = ["grass", "litter", "all"]
         for fuel_type in fuel_types:
@@ -266,17 +266,19 @@
     Assigns target values and calculation method for exactly one fuel type and parameter
 
     Parameters
     ----------
     method : str
         Calibration method for the target values provided. Must be one of:
         "constant", "maxmin", "meansd", "sb40".
-    **kwargs : str
+    **kwargs : float
         Keyword arguments correspond to the calibration method.
-        #TODO: kwargs in docstring
+        For "maxmin" method, **kwargs keys must be `max` and `min`.
+        For "meansd" method, **kwargs keys must be `mean` and `sd`.
+        For "constant" method, **kwargs key must be `value`.
 
     Returns
     -------
     Instance of class Targets
     """
     args = list(kwargs.keys())
     targets = list(kwargs.values())
@@ -379,23 +381,24 @@
     Sets calibration targets for grass, litter, both separately, or all
     fuel types together, for a single fuel parameter.
 
     Parameters
     ----------
     parameter : str
         Fuel parameter for which to set targets
-    grass : Targets | None
-        Grass calibration targets. Only the grass layer of the DUET bulk
-        density array will be calibrated.
-    litter : Targets | None
-        Litter calibration targets. Only the litter layer of the DUET bulk
-        density array will be calibrated.
-    all : Targets | None
-        Calibration targets for all (both) fuel types. Both layers of the
-        DUET bulk density array will be calibrated together.
+    **kwargs : Targets
+        grass : Targets
+            Grass calibration targets. Only the grass layer of the DUET bulk
+            density array will be calibrated.
+        litter : Targets
+            Litter calibration targets. Only the litter layer of the DUET bulk
+            density array will be calibrated.
+        all : Targets
+            Calibration targets for all (both) fuel types. Both layers of the
+            DUET bulk density array will be calibrated together.
 
     Returns
     -------
     FuelParameter :
         Object representing targets for the given fuel parameter, for each provided fuel type
     """
     parameter = parameter
@@ -489,15 +492,15 @@
     fuel_types = list(kwargs.keys())
     targets = list(kwargs.values())
 
     return FuelParameter(parameter, fuel_types, targets)
 
 
 def calibrate(
-    duet_run: DuetRun, fuel_parameter_targets: list(FuelParameter) | FuelParameter
+    duet_run: DuetRun, fuel_parameter_targets: list[FuelParameter] | FuelParameter
 ) -> DuetRun:
     """
     Calibrates the arrays in a DuetRun object using the provided targets and methods for one
     or more fuel types.
 
     Parameters
     ----------
@@ -549,20 +552,41 @@
     -------
     geojson
     """
     # TODO: write get_unit_from_shapefile
 
 
 def write_numpy_to_quicfire(array: np.ndarray, directory: str | Path, filename: str):
+    """
+    Writes a numpy array to a QUIC-Fire fuel input (.dat) in the chosen directory.
+
+    Parameters
+    ----------
+    array : np.ndarray
+        The numpy array to be written. Must be 3D.
+    directory : str | Path
+        The directory where the file will be written.
+    filename : str
+        The name of the file to be written. Must end in ".dat".
+
+    Returns
+    -------
+    None
+        File is written to disk.
+    """
     if isinstance(directory, str):
         directory = Path(directory)
     write_array_to_dat(array=array, dat_name=filename, output_dir=directory)
 
 
 def _get_array_to_calibrate(duet_run: DuetRun, fueltype: str, fuelparam: str):
+    """
+    Identifies and returns the layer of the duet outputs should be processed based
+    on the fuel parameter and fuel type.
+    """
     if fuelparam == "density":
         if fueltype == "grass":
             return duet_run.density[0, :, :].copy()
         if fueltype == "litter":
             return duet_run.density[1, :, :].copy()
         return np.sum(duet_run.density, axis=0)
     if fuelparam == "height":
@@ -583,28 +607,34 @@
         raise ValueError(
             "No moisture array available to calibrate. Please add moisture"
             "array using DuetRun.add_moisture_array"
         )
 
 
 def _duplicate_duet_run(duet_run: DuetRun) -> DuetRun:
+    """
+    Makes a copy of a DuetRun object.
+    """
     new_density = duet_run.density.copy() if duet_run.density is not None else None
     new_moisture = duet_run.moisture.copy() if duet_run.moisture is not None else None
     new_height = duet_run.height.copy() if duet_run.height is not None else None
 
     new_duet = DuetRun(
         density=new_density,
         moisture=new_moisture,
         height=new_height,
     )
 
     return new_duet
 
 
 def _do_calibration(array: np.ndarray, target_obj: Targets):
+    """
+    Calibrates an array based on the method and values in a Targets object.
+    """
     kwarg_dict = {}
     for i in range(len(target_obj.args)):
         kwarg_dict[target_obj.args[i]] = target_obj.targets[i]
     new_array = target_obj.calibration_function(array, **kwarg_dict)
     return new_array
 
 
@@ -648,26 +678,33 @@
     if np.min(xnew) < 0:
         xnew = _truncate_at_0(xnew)
     return xnew
 
 
 # TODO: add option for fuel vs cell bulk density?
 def _constant_calibration(x: np.ndarray, **kwargs: float) -> np.ndarray:
+    """
+    Conducts constant calibration by changing all nonzero values in a
+    duet fuel parameter/type to a single given value.
+    """
     value = kwargs["value"]
     arr = x.copy()
     arr[arr > 0] = value
     return arr
 
 
 def _add_calibrated_array(
     duet_to_calibrate: DuetRun,
     calibrated_array: np.ndarray,
     fueltype: str,
     fuelparam: str,
 ) -> DuetRun:
+    """
+    Replaces or creates calibrated array(s) in a DuetRun object.
+    """
     for param in ["density", "moisture", "height"]:
         if fuelparam == param:
             if fueltype == "grass":
                 duet_to_calibrate.__dict__[param][0, :, :] = calibrated_array
             if fueltype == "litter":
                 duet_to_calibrate.__dict__[param][1, :, :] = calibrated_array
             if fueltype == "all":
@@ -676,14 +713,18 @@
                 )
     return duet_to_calibrate
 
 
 def _separate_2d_array(
     calibrated: np.ndarray, param: str, duet_run: DuetRun
 ) -> np.ndarray:
+    """
+    Separates a combined array into its component fuel types based on the
+    fuel parameter.
+    """
     separated = np.array([calibrated, calibrated])
     if param == "density":
         weights = duet_run.density.copy()
         weights[0, :, :] = duet_run.density[0, :, :] / np.sum(duet_run.density, axis=0)
         weights[1, :, :] = duet_run.density[1, :, :] / np.sum(duet_run.density, axis=0)
         separated[0, :, :] = calibrated * weights[0, :, :]
         separated[1, :, :] = calibrated * weights[1, :, :]
```

### Comparing `duet-tools-0.1.5/duet_tools/data/sb40_parameters.csv` & `duet_tools-0.2/duet_tools/data/sb40_parameters.csv`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/duet_tools/example.py` & `duet_tools-0.2/duet_tools/example.py`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/duet_tools/landfire.py` & `duet_tools-0.2/duet_tools/landfire.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,14 +267,15 @@
             row["fbfm_code"].values[0],
             row["dry_load"].values[0],
             row["sav"].values[0],
             row["dead_fuel_extinction_moisture"].values[0],
             row["fuel_bed_depth_m"].values[0],
             row["duet_fuel_type"].values[0],
         ]
+    sb40_dict[-9999] = ["NA", 0.0, 0.0, 0.0, 0.0, 0]
 
     return sb40_dict
 
 
 def _get_sb40_arrays(sb40_keys: np.ndarray, sb40_dict: dict) -> np.ndarray:
     """
     Use a dictionary of bulk density and fuel types that correspond to SB40
```

### Comparing `duet-tools-0.1.5/duet_tools/utils.py` & `duet_tools-0.2/duet_tools/utils.py`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/duet_tools.egg-info/PKG-INFO` & `duet_tools-0.2/duet_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duet-tools
-Version: 0.1.5
+Version: 0.2.0
 Summary: Output management tools for LANL DUET program
 Home-page: https://github.com/nmc-cafes/duet-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/nmc-cafes/duet-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duet-tools-0.1.5/setup.py` & `duet_tools-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `duet-tools-0.1.5/tests/test_calibration_module.py` & `duet_tools-0.2/tests/test_calibration_module.py`

 * *Files identical despite different names*

