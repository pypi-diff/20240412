# Comparing `tmp/janus_core-0.2.0b5.tar.gz` & `tmp/janus_core-0.2.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.2.0b5.tar", max compression
+gzip compressed data, was "janus_core-0.2.0b6.tar", max compression
```

## Comparing `janus_core-0.2.0b5.tar` & `janus_core-0.2.0b6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1533 2024-04-11 11:04:09.575169 janus_core-0.2.0b5/LICENSE
--rw-r--r--   0        0        0     8784 2024-04-11 11:04:09.575169 janus_core-0.2.0b5/README.md
--rw-r--r--   0        0        0       80 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/__init__.py
--rw-r--r--   0        0        0    29979 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/cli.py
--rw-r--r--   0        0        0     4790 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/janus_types.py
--rw-r--r--   0        0        0     4045 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/log.py
--rw-r--r--   0        0        0    32211 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/md.py
--rw-r--r--   0        0        0     3514 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/single_point.py
--rw-r--r--   0        0        0     3293 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/stats.py
--rw-r--r--   0        0        0      545 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/utils.py
--rw-r--r--   0        0        0     2553 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/pyproject.toml
--rw-r--r--   0        0        0     9845 1970-01-01 00:00:00.000000 janus_core-0.2.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/LICENSE
+-rw-r--r--   0        0        0     8612 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/README.md
+-rw-r--r--   0        0        0       80 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/__init__.py
+-rw-r--r--   0        0        0    30268 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/cli.py
+-rw-r--r--   0        0        0     4790 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/geom_opt.py
+-rw-r--r--   0        0        0     1664 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/janus_types.py
+-rw-r--r--   0        0        0     4045 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/log.py
+-rw-r--r--   0        0        0    32216 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/md.py
+-rw-r--r--   0        0        0     3514 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/mlip_calculators.py
+-rw-r--r--   0        0        0    12111 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/single_point.py
+-rw-r--r--   0        0        0     3293 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/stats.py
+-rw-r--r--   0        0        0     1544 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/janus_core/utils.py
+-rw-r--r--   0        0        0     2553 2024-04-12 12:29:54.805629 janus_core-0.2.0b6/pyproject.toml
+-rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 janus_core-0.2.0b6/PKG-INFO
```

### Comparing `janus_core-0.2.0b5/LICENSE` & `janus_core-0.2.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/README.md` & `janus_core-0.2.0b6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -169,33 +169,29 @@
 
 ```yaml
 struct: "NaCl.cif"
 properties:
   - "energy"
 out: "NaCl-results.xyz"
 arch: mace_mp
-calc_kwargs:
+calc-kwargs:
   model: medium
 ```
 
 ```shell
 janus singlepoint --struct KCl.cif --out KCl-results.cif --config config.yml
 ```
 
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
 > [!WARNING]
-> Options in the Yaml file must use `_` instead of `-`.
-> For example, `calc_kwargs` should be used in the configuration file for the `--calc-kwargs` option.
-
-> [!WARNING]
 > If an option in the configuration file does not match any variable names, an error will **not** be raised.
 > Please check the summary file to ensure the configuration has been read correctly.
 
 
 ## License
 
 [BSD 3-Clause License](LICENSE)
```

### Comparing `janus_core-0.2.0b5/janus_core/cli.py` & `janus_core-0.2.0b6/janus_core/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Set up commandline interface."""
 
 import ast
 import datetime
 import logging
 from pathlib import Path
-from typing import Annotated, Optional, Union, get_args
+from typing import Annotated, Any, Optional, Union, get_args
 
 from ase import Atoms
 import typer
-from typer_config import use_yaml_config
+from typer_config import conf_callback_factory, use_config, yaml_loader
 import yaml
 
 from janus_core import __version__
 from janus_core.geom_opt import optimize
 from janus_core.janus_types import ASEReadArgs, Ensembles
 from janus_core.md import NPH, NPT, NVE, NVT, NVT_NH
 from janus_core.single_point import SinglePoint
+from janus_core.utils import dict_paths_to_strs, dict_remove_hyphens
 
 app = typer.Typer(name="janus", no_args_is_help=True)
 
 
 class TyperDict:  #  pylint: disable=too-few-public-methods
     """
     Custom dictionary for typer.
@@ -97,29 +98,37 @@
             raise ValueError(
                 f"""{typer_dicts[i]} must be passed as a dictionary wrapped in quotes.\
  For example, "{{'key' : value}}" """
             )
     return typer_dicts
 
 
-def _dict_paths_to_strs(dictionary: dict) -> None:
+def yaml_converter_loader(config_file: str) -> dict[str, Any]:
     """
-    Recursively iterate over dictionary, converting Path values to strings.
+    Load yaml configuration and replace hyphens with underscores.
 
     Parameters
     ----------
-    dictionary : dict
-        Dictionary to be converted.
+    config_file : str
+        Yaml configuration file to read.
+
+    Returns
+    -------
+    dict[str, Any]
+        Dictionary with loaded configuration.
     """
-    for key, value in dictionary.items():
-        if isinstance(value, dict):
-            _dict_paths_to_strs(value)
-        elif isinstance(value, Path):
-            dictionary[key] = str(value)
+    if not config_file:
+        return {}
+
+    config = yaml_loader(config_file)
+    # Replace all "-"" with "_" in conf
+    return dict_remove_hyphens(config)
+
 
+yaml_converter_callback = conf_callback_factory(yaml_converter_loader)
 
 # Shared type aliases
 StructPath = Annotated[Path, typer.Option(help="Path of structure to simulate.")]
 Architecture = Annotated[
     str, typer.Option(help="MLIP architecture to use for calculations.")
 ]
 Device = Annotated[str, typer.Option(help="Device to run calculations on.")]
@@ -186,15 +195,15 @@
     """
     if version:
         print(f"janus-core version: {__version__}")
         raise typer.Exit()
 
 
 @app.command(help="Perform single point calculations and save to file.")
-@use_yaml_config()
+@use_config(yaml_converter_callback)
 def singlepoint(
     # pylint: disable=too-many-locals
     # numpydoc ignore=PR02
     struct: StructPath,
     arch: Architecture = "mace_mp",
     device: Device = "cpu",
     properties: Annotated[
@@ -304,15 +313,15 @@
 
     inputs["run"] = {
         "properties": properties,
         "write_kwargs": write_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
-    _dict_paths_to_strs(inputs)
+    dict_paths_to_strs(inputs)
 
     # Save summary information before singlepoint calculation begins
     save_info = {
         "command": "janus singlepoint",
         "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
         "inputs": inputs,
     }
@@ -331,15 +340,15 @@
         )
     logging.shutdown()
 
 
 @app.command(
     help="Perform geometry optimization and save optimized structure to file.",
 )
-@use_yaml_config()
+@use_config(yaml_converter_callback)
 def geomopt(
     # pylint: disable=too-many-arguments,too-many-locals
     # numpydoc ignore=PR02
     struct: StructPath,
     fmax: Annotated[float, typer.Option(help="Maximum force for convergence.")] = 0.1,
     steps: Annotated[
         int, typer.Option(help="Maximum number of optimization steps.")
@@ -505,15 +514,15 @@
         "arch": arch,
         "device": device,
         "read_kwargs": read_kwargs,
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
-    _dict_paths_to_strs(inputs)
+    dict_paths_to_strs(inputs)
 
     # Save summary information before optimization begins
     save_info = {
         "command": "janus geomopt",
         "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
         "inputs": inputs,
     }
@@ -532,15 +541,15 @@
         )
     logging.shutdown()
 
 
 @app.command(
     help="Run molecular dynamics simulation, and save trajectory and statistics.",
 )
-@use_yaml_config()
+@use_config(yaml_converter_callback)
 def md(
     # pylint: disable=too-many-arguments,too-many-locals,invalid-name
     # numpydoc ignore=PR02
     ensemble: Annotated[str, typer.Option(help="Name of thermodynamic ensemble.")],
     struct: StructPath,
     steps: Annotated[int, typer.Option(help="Number of steps in simulation.")] = 0,
     timestep: Annotated[
@@ -891,15 +900,15 @@
         "arch": arch,
         "device": device,
         "read_kwargs": read_kwargs,
         "calc_kwargs": calc_kwargs,
     }
 
     # Convert all paths to strings in inputs nested dictionary
-    _dict_paths_to_strs(inputs)
+    dict_paths_to_strs(inputs)
 
     # Save summary information before simulation begins
     save_info = {
         "command": "janus md",
         "start_time": datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S"),
         "inputs": inputs,
     }
```

### Comparing `janus_core-0.2.0b5/janus_core/geom_opt.py` & `janus_core-0.2.0b6/janus_core/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/janus_core/janus_types.py` & `janus_core-0.2.0b6/janus_core/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/janus_core/log.py` & `janus_core-0.2.0b6/janus_core/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/janus_core/md.py` & `janus_core-0.2.0b6/janus_core/md.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     def _reset_velocities(self) -> None:
         """Reset velocities and (optionally) rotation of system while equilibrating."""
         if self.dyn.nsteps < self.equil_steps:
             self._set_velocity_distribution()
 
     def _optimize_structure(self) -> None:
         """Perform geometry optimization."""
-        if self.dyn.nsteps < self.equil_steps:
+        if self.dyn.nsteps == 0 or self.dyn.nsteps < self.equil_steps:
             if self.logger:
                 self.minimize_kwargs["log_kwargs"] = {
                     "filename": self.log_kwargs["filename"],
                     "name": self.logger.name,
                     "filemode": "a",
                 }
                 self.logger.info("Minimizing at step %s", self.dyn.nsteps)
@@ -498,15 +498,15 @@
                 except (IndexError, ValueError) as e:
                     raise ValueError("Unable to read restart file") from e
             except FileNotFoundError as e:
                 raise FileNotFoundError("Unable to read restart file") from e
 
         else:
             if self.minimize:
-                optimize(self.struct, **self.minimize_kwargs)
+                self._optimize_structure()
             if self.rescale_velocities:
                 self._reset_velocities()
 
             log_header = self.get_log_header()
             with open(self.stats_file, "w", encoding="utf8") as stats_file:
                 print(log_header, file=stats_file)
```

### Comparing `janus_core-0.2.0b5/janus_core/mlip_calculators.py` & `janus_core-0.2.0b6/janus_core/mlip_calculators.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/janus_core/single_point.py` & `janus_core-0.2.0b6/janus_core/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/janus_core/stats.py` & `janus_core-0.2.0b6/janus_core/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b5/pyproject.toml` & `janus_core-0.2.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.2.0b5"
+version = "0.2.0b6"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
```

### Comparing `janus_core-0.2.0b5/PKG-INFO` & `janus_core-0.2.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.2.0b5
+Version: 0.2.0b6
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -195,33 +195,29 @@
 
 ```yaml
 struct: "NaCl.cif"
 properties:
   - "energy"
 out: "NaCl-results.xyz"
 arch: mace_mp
-calc_kwargs:
+calc-kwargs:
   model: medium
 ```
 
 ```shell
 janus singlepoint --struct KCl.cif --out KCl-results.cif --config config.yml
 ```
 
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
 > [!WARNING]
-> Options in the Yaml file must use `_` instead of `-`.
-> For example, `calc_kwargs` should be used in the configuration file for the `--calc-kwargs` option.
-
-> [!WARNING]
 > If an option in the configuration file does not match any variable names, an error will **not** be raised.
 > Please check the summary file to ensure the configuration has been read correctly.
 
 
 ## License
 
 [BSD 3-Clause License](LICENSE)
```

