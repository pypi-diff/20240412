# Comparing `tmp/ansys_dpf_post-0.6.0.tar.gz` & `tmp/ansys_dpf_post-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_dpf_post-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_dpf_post-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_dpf_post-0.6.0.tar` & `ansys_dpf_post-0.7.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1066 2023-10-19 19:14:19.304420 ansys_dpf_post-0.6.0/LICENSE
--rw-r--r--   0        0        0     5592 2023-10-19 19:14:19.304420 ansys_dpf_post-0.6.0/README.md
--rw-r--r--   0        0        0     1565 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2300 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/__init__.py
--rw-r--r--   0        0        0     5184 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/common.py
--rw-r--r--   0        0        0     4878 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/connectivity.py
--rw-r--r--   0        0        0    46448 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/dataframe.py
--rw-r--r--   0        0        0     1042 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/displacement.py
--rw-r--r--   0        0        0     2706 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/dpf_path.py
--rwxr-xr-x   0        0        0    15841 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/dpf_solution.py
--rwxr-xr-x   0        0        0     1532 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/electric_results.py
--rw-r--r--   0        0        0     7761 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/elements.py
--rwxr-xr-x   0        0        0     1519 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/errors.py
--rw-r--r--   0        0        0     1962 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/examples/__init__.py
--rw-r--r--   0        0        0     5076 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/faces.py
--rw-r--r--   0        0        0   386332 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/fluid_simulation.py
--rw-r--r--   0        0        0      287 2023-10-19 19:14:19.312420 ansys_dpf_post-0.6.0/src/ansys/dpf/post/harmonic_analysis.py
--rw-r--r--   0        0        0   165367 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py
--rw-r--r--   0        0        0      118 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/helpers/__init__.py
--rw-r--r--   0        0        0     1173 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/helpers/selections.py
--rw-r--r--   0        0        0     3419 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/helpers/streamlines.py
--rw-r--r--   0        0        0    12567 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/index.py
--rw-r--r--   0        0        0    20305 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/mesh.py
--rw-r--r--   0        0        0     7123 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/mesh_info.py
--rw-r--r--   0        0        0     6218 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/meshes.py
--rw-r--r--   0        0        0     2117 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/misc.py
--rwxr-xr-x   0        0        0    31334 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/misc_results.py
--rw-r--r--   0        0        0      276 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/modal_analysis.py
--rw-r--r--   0        0        0   212763 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/modal_mechanical_simulation.py
--rw-r--r--   0        0        0     4735 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/named_selection.py
--rw-r--r--   0        0        0     4177 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/nodes.py
--rw-r--r--   0        0        0     3069 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/phase.py
--rw-r--r--   0        0        0    10862 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/post_utility.py
--rwxr-xr-x   0        0        0    15063 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_data.py
--rw-r--r--   0        0        0    10026 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_definition.py
--rwxr-xr-x   0        0        0    14351 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_evaluation.py
--rwxr-xr-x   0        0        0     3491 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_object.py
--rw-r--r--   0        0        0     1357 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/scalar.py
--rw-r--r--   0        0        0    37947 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/selection.py
--rw-r--r--   0        0        0    39891 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/simulation.py
--rw-r--r--   0        0        0     3091 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/species.py
--rw-r--r--   0        0        0      429 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/static_analysis.py
--rw-r--r--   0        0        0   322789 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/static_mechanical_simulation.py
--rw-r--r--   0        0        0     1748 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/strain.py
--rw-r--r--   0        0        0     1847 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/stress.py
--rw-r--r--   0        0        0     2440 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/temperature.py
--rw-r--r--   0        0        0     9225 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/tensor.py
--rw-r--r--   0        0        0      301 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/tools.py
--rw-r--r--   0        0        0      451 2023-10-19 19:14:19.316421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/transient_analysis.py
--rw-r--r--   0        0        0   246902 2023-10-19 19:14:19.320421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/transient_mechanical_simulation.py
--rw-r--r--   0        0        0     5785 2023-10-19 19:14:19.320421 ansys_dpf_post-0.6.0/src/ansys/dpf/post/vector.py
--rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 ansys_dpf_post-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-21 18:11:08.692793 ansys_dpf_post-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5592 2024-02-21 18:11:08.696792 ansys_dpf_post-0.7.0/README.md
+-rw-r--r--   0        0        0     1565 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1959 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/__init__.py
+-rw-r--r--   0        0        0     5184 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/common.py
+-rw-r--r--   0        0        0     4878 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/connectivity.py
+-rw-r--r--   0        0        0    46448 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/dataframe.py
+-rw-r--r--   0        0        0     1042 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/displacement.py
+-rw-r--r--   0        0        0     2706 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/dpf_path.py
+-rwxr-xr-x   0        0        0    15915 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/dpf_solution.py
+-rwxr-xr-x   0        0        0     1532 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/electric_results.py
+-rw-r--r--   0        0        0     7761 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/elements.py
+-rwxr-xr-x   0        0        0     1519 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/errors.py
+-rw-r--r--   0        0        0     1962 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/examples/__init__.py
+-rw-r--r--   0        0        0     5076 2024-02-21 18:11:08.700793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/faces.py
+-rw-r--r--   0        0        0   387351 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/fluid_simulation.py
+-rw-r--r--   0        0        0      287 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/harmonic_analysis.py
+-rw-r--r--   0        0        0   166458 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py
+-rw-r--r--   0        0        0      118 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/helpers/__init__.py
+-rw-r--r--   0        0        0     1173 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/helpers/selections.py
+-rw-r--r--   0        0        0     3419 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/helpers/streamlines.py
+-rw-r--r--   0        0        0    12567 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/index.py
+-rw-r--r--   0        0        0    20305 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/mesh.py
+-rw-r--r--   0        0        0     7123 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/mesh_info.py
+-rw-r--r--   0        0        0     6218 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/meshes.py
+-rw-r--r--   0        0        0     2117 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/misc.py
+-rwxr-xr-x   0        0        0    31334 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/misc_results.py
+-rw-r--r--   0        0        0      276 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/modal_analysis.py
+-rw-r--r--   0        0        0   213694 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/modal_mechanical_simulation.py
+-rw-r--r--   0        0        0     4735 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/named_selection.py
+-rw-r--r--   0        0        0     4177 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/nodes.py
+-rw-r--r--   0        0        0     3069 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/phase.py
+-rw-r--r--   0        0        0    10862 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/post_utility.py
+-rwxr-xr-x   0        0        0    15063 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_data.py
+-rw-r--r--   0        0        0    10026 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_definition.py
+-rwxr-xr-x   0        0        0    14351 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_evaluation.py
+-rwxr-xr-x   0        0        0     3491 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_object.py
+-rw-r--r--   0        0        0     1357 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/scalar.py
+-rw-r--r--   0        0        0    38497 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/selection.py
+-rw-r--r--   0        0        0    40299 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/simulation.py
+-rw-r--r--   0        0        0     3091 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/species.py
+-rw-r--r--   0        0        0      429 2024-02-21 18:11:08.704793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/static_analysis.py
+-rw-r--r--   0        0        0   323718 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/static_mechanical_simulation.py
+-rw-r--r--   0        0        0     1748 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/strain.py
+-rw-r--r--   0        0        0     1847 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/stress.py
+-rw-r--r--   0        0        0     2440 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/temperature.py
+-rw-r--r--   0        0        0     9225 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/tensor.py
+-rw-r--r--   0        0        0      301 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/tools.py
+-rw-r--r--   0        0        0      451 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/transient_analysis.py
+-rw-r--r--   0        0        0   247665 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/transient_mechanical_simulation.py
+-rw-r--r--   0        0        0     5785 2024-02-21 18:11:08.708793 ansys_dpf_post-0.7.0/src/ansys/dpf/post/vector.py
+-rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 ansys_dpf_post-0.7.0/PKG-INFO
```

### Comparing `ansys_dpf_post-0.6.0/LICENSE` & `ansys_dpf_post-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/README.md` & `ansys_dpf_post-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/pyproject.toml` & `ansys_dpf_post-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-dpf-post"
-version = "0.6.0"
+version = "0.7.0"
 description = "PyDPF-Post Python library."
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/__init__.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,16 +51,7 @@
 )
 from ansys.dpf.post.transient_mechanical_simulation import (  # noqa: F401
     TransientMechanicalSimulation,
 )
 
 # this must be after some ansys.dpf.post import
 __version__ = importlib_metadata.version("ansys-dpf-post")
-
-
-if hasattr(core, "settings") and hasattr(
-    core.settings, "set_dynamic_available_results_capability"
-):
-    core.settings.set_dynamic_available_results_capability(False)
-if hasattr(core, "settings") and hasattr(core.settings, "set_default_pyvista_config"):
-    core.settings.set_default_pyvista_config()
-# dpf.core.start_local_server()
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/common.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/common.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/connectivity.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/connectivity.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/dataframe.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/dataframe.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/displacement.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/displacement.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/dpf_path.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/dpf_path.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/dpf_solution.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/dpf_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
              -  stiffness_matrix_energy: Elemental Energy-stiffness matrix
              -  artificial_hourglass_energy: Elemental Hourglass Energy
              -  thermal_dissipation_energy: Elemental thermal dissipation energy
              -  kinetic_energy: Elemental Kinetic Energy
              -  co_energy: Elemental co-energy
              -  incremental_energy: Elemental incremental energy
              -  elastic_strain: ElementalNodal Strain
+             -  element_euler_angles: ElementalNodal Element Euler Angles
              -  structural_temperature: ElementalNodal Structural temperature
         """
         return self._model.metadata.result_info
 
     @staticmethod
     def _check_nodal_location(**kwargs):
         if _AvailableKeywords.location in kwargs:
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/electric_results.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/electric_results.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/elements.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/elements.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/errors.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/examples/__init__.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/faces.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/faces.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/fluid_simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/fluid_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,18 @@
     @property
     def cell_zones(self) -> dict:
         """Return a dictionary of the cell zones in the simulation."""
         return self.mesh_info.cell_zones
 
     @property
     def face_zones(self) -> dict:
-        """Return a dictionary of the face zones in the simulation."""
+        """Return a dictionary of the face zones in the simulation.
+
+        For CFX files, we gather face zones in COMPOSITE entities more physics-related.
+        """
         return self.mesh_info.face_zones
 
     @property
     def species(self) -> SpeciesDict:
         """Return a dictionary-like object of species in the simulation."""
         return SpeciesDict(self)
 
@@ -201,14 +204,122 @@
         """Filter zone IDs to only keep zones of the given type."""
         if keep == locations.elemental:
             ref = set(self.cell_zones.keys())
         elif keep == locations.faces:
             ref = set(self.face_zones.keys())
         return [i for i in zone_ids if i in ref]
 
+    def _get_result_workflow(
+        self,
+        base_name: str,
+        location: str,
+        category: ResultCategory,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        selection: Union[Selection, None] = None,
+        set_ids: Union[int, List[int], None] = None,
+        zone_ids: Union[List[int], None] = None,
+        phases: Union[List[Union[int, str]], None] = None,
+        species: Union[List[int], None] = None,
+        qualifiers: Union[dict, None] = None,
+    ) -> (dpf.Workflow, Union[str, list[str], None], str):
+        """Generate (without evaluating) the Workflow to extract results."""
+        comp, to_extract, columns = self._create_components(
+            base_name, category, components
+        )
+
+        # Initialize a workflow
+        wf, result_op = self._build_result_workflow(
+            name=base_name,
+            location=location,
+            force_elemental_nodal=False,
+        )
+        query_regions_meshes = False
+        lists = []
+        lists_labels = []
+        if qualifiers:
+            labels = list(qualifiers.keys())
+            lists_labels.extend(labels)
+            lists.extend([qualifiers[key] for key in labels])
+            if "zone" in labels:
+                query_regions_meshes = qualifiers["zone"]
+        else:
+            if set_ids:
+                lists.append(set_ids)
+                lists_labels.append("time")
+            if zone_ids:
+                lists.append(zone_ids)
+                lists_labels.append("zone")
+                query_regions_meshes = zone_ids
+            if phases:
+                phase_ids = []
+                available_phases = self.phases
+                for phase in phases:
+                    phase_ids.append(available_phases[phase].id)
+                lists.append(phase_ids)
+                lists_labels.append("phase")
+            if species:
+                lists.append(species)
+                lists_labels.append("species")
+
+        if lists:
+            import itertools
+
+            for i, c in enumerate(itertools.product(*lists)):
+                label_space = {}
+                for j, label in enumerate(lists_labels):
+                    label_space[label] = c[j]
+                result_op.connect(1000 + i, label_space)
+        # Its output is selected as future workflow output for now
+        # print(result_op)
+
+        if query_regions_meshes:
+            # Results have been queried on regions,
+            # A MeshesProvider is required to give meshes as input of the source operator
+            meshes_provider_op = self._model.operator("meshes_provider")
+            meshes_provider_op.connect(25, query_regions_meshes)
+            result_op.connect(7, meshes_provider_op.outputs.meshes)
+            wf.add_operator(meshes_provider_op)
+        else:
+            # Results have been queried on the whole mesh,
+            # A MeshProvider is required to give the mesh as input of the source operator
+            mesh_provider_op = self._model.operator("mesh_provider")
+            result_op.connect(7, mesh_provider_op.outputs.mesh)
+            wf.add_operator(mesh_provider_op)
+
+        out = result_op.outputs.fields_container
+        # Its inputs are selected as workflow inputs for merging with selection workflows
+        wf.set_input_name("time_scoping", result_op.inputs.time_scoping)
+        wf.set_input_name("mesh_scoping", result_op.inputs.mesh_scoping)
+
+        wf.connect_with(
+            selection.time_freq_selection._selection,
+            output_input_names=("scoping", "time_scoping"),
+        )
+        wf.connect_with(
+            selection.spatial_selection._selection,
+            output_input_names=("scoping", "mesh_scoping"),
+        )
+
+        # Connect data_sources and streams_container inputs of selection if necessary
+        if "streams" in wf.input_names:
+            wf.connect("streams", self._model.metadata.streams_provider)
+        if "data_sources" in wf.input_names:
+            wf.connect("data_sources", self._model.metadata.data_sources)
+
+        # Add an optional norm operation if requested
+        if norm:
+            wf, out, comp, base_name = self._append_norm(wf, out, base_name)
+
+        # Set the workflow output
+        wf.set_output_name("out", out)
+        wf.progress_bar = False
+
+        return wf, comp, base_name
+
     def _get_result(
         self,
         base_name: str,
         category: ResultCategory,
         native_location: str,
         location: Union[locations, str, None] = None,
         components: Union[str, List[str], int, List[int], None] = None,
@@ -380,120 +491,37 @@
             node_ids=node_ids,
             face_ids=face_ids,
             cell_ids=cell_ids,
             named_selections=named_selections,
             location=location,
         )
 
-        comp, to_extract, columns = self._create_components(
-            base_name, category, components
-        )
-
-        # Initialize a workflow
-        wf, result_op = self._build_result_workflow(
-            name=base_name,
+        wf, comp, base_name = self._get_result_workflow(
+            base_name=base_name,
             location=location,
-            force_elemental_nodal=False,
-        )
-        query_regions_meshes = False
-        lists = []
-        lists_labels = []
-        if qualifiers:
-            labels = list(qualifiers.keys())
-            lists_labels.extend(labels)
-            lists.extend([qualifiers[key] for key in labels])
-            if "zone" in labels:
-                query_regions_meshes = qualifiers["zone"]
-        else:
-            if set_ids:
-                lists.append(set_ids)
-                lists_labels.append("time")
-            if zone_ids:
-                lists.append(zone_ids)
-                lists_labels.append("zone")
-                query_regions_meshes = zone_ids
-            if phases:
-                phase_ids = []
-                available_phases = self.phases
-                for phase in phases:
-                    phase_ids.append(available_phases[phase].id)
-                lists.append(phase_ids)
-                lists_labels.append("phase")
-            if species:
-                lists.append(species)
-                lists_labels.append("species")
-
-        if lists:
-            import itertools
-
-            for i, c in enumerate(itertools.product(*lists)):
-                label_space = {}
-                for j, label in enumerate(lists_labels):
-                    label_space[label] = c[j]
-                result_op.connect(1000 + i, label_space)
-        # Its output is selected as future workflow output for now
-        # print(result_op)
-
-        if query_regions_meshes:
-            # Results have been queried on regions,
-            # A MeshesProvider is required to give meshes as input of the source operator
-            meshes_provider_op = self._model.operator("meshes_provider")
-            meshes_provider_op.connect(25, query_regions_meshes)
-            result_op.connect(7, meshes_provider_op.outputs.meshes)
-            wf.add_operator(meshes_provider_op)
-        else:
-            # Results have been queried on the whole mesh,
-            # A MeshProvider is required to give the mesh as input of the source operator
-            mesh_provider_op = self._model.operator("mesh_provider")
-            result_op.connect(7, mesh_provider_op.outputs.mesh)
-            wf.add_operator(mesh_provider_op)
-
-        out = result_op.outputs.fields_container
-        # Its inputs are selected as workflow inputs for merging with selection workflows
-        wf.set_input_name("time_scoping", result_op.inputs.time_scoping)
-        wf.set_input_name("mesh_scoping", result_op.inputs.mesh_scoping)
-
-        wf.connect_with(
-            selection.time_freq_selection._selection,
-            output_input_names=("scoping", "time_scoping"),
-        )
-        wf.connect_with(
-            selection.spatial_selection._selection,
-            output_input_names=("scoping", "mesh_scoping"),
+            category=category,
+            components=components,
+            norm=norm,
+            selection=selection,
+            set_ids=set_ids,
+            zone_ids=zone_ids,
+            phases=phases,
+            species=species,
+            qualifiers=qualifiers,
         )
 
-        # Connect data_sources and streams_container inputs of selection if necessary
-        if "streams" in wf.input_names:
-            wf.connect("streams", self._model.metadata.streams_provider)
-        if "data_sources" in wf.input_names:
-            wf.connect("data_sources", self._model.metadata.data_sources)
-
-        # Add an optional norm operation if requested
-        if norm:
-            norm_op = self._model.operator(name="norm_fc")
-            norm_op.connect(0, out)
-            wf.add_operator(operator=norm_op)
-            out = norm_op.outputs.fields_container
-
-        # if averaging_op_name:
-        #     average_op = self._model.operator(name=averaging_op_name)
-        #     average_op.connect(0, out)
-        #     wf.add_operator(operator=average_op)
-        #     out = average_op.outputs.fields_container
-
-        # Set the workflow output
-        wf.set_output_name("out", out)
-        wf.progress_bar = False
         # Evaluate  the workflow
         fc = wf.get_output("out", dpf.types.fields_container)
         # print(fc)
         if location is None and len(fc) > 0:
             location = fc[0].location
         if location == locations.elemental:
             location = "cells"
+
+        _, _, columns = self._create_components(base_name, category, components)
         return self._create_dataframe(
             fc, location, columns, comp, base_name.split("::")[-1], None
         )
 
     def _try_get_result_info(self, name: str):
         try:
             return self.result_info[name]
@@ -529,15 +557,16 @@
         Argument `qualifiers` overrides arguments `zones_ids`, `phases`, and `species`.
 
         Parameters
         ----------
         node_ids:
             List of IDs of nodes to get results for.
         face_ids:
-            List of IDs of faces to get results for.
+            List of faces IDs to get results for. For CFX files, these IDs correspond
+            to the COMPOSITE that gathers the related face zones.
         cell_ids:
             List of IDs of cells to get results for.
         zone_ids:
             List of IDs of zones to get results for.
         phases:
             List of IDs of phases to get results for.
         species:
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/harmonic_mechanical_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,163 +21,29 @@
 from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
 class HarmonicMechanicalSimulation(MechanicalSimulation):
     """Provides methods for mechanical harmonic simulations."""
 
-    def _get_result(
+    def _get_result_workflow(
         self,
         base_name: str,
         location: str,
         category: ResultCategory,
         components: Union[str, List[str], int, List[int], None] = None,
         norm: bool = False,
         amplitude: bool = False,
         sweeping_phase: Union[float, None] = 0.0,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        frequencies: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
-        external_layer: Union[bool, List[int]] = False,
-        skin: Union[bool, List[int]] = False,
-    ) -> DataFrame:
-        """Extract results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
-        exclusive.
-        If none of the above is given, only the first mode will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Parameters
-        ----------
-        base_name:
-            Base name for the requested result.
-        location:
-            Location to extract results at. Available locations are listed in
-            class:`post.locations` and are: `post.locations.nodal`,
-            `post.locations.elemental`, and `post.locations.elemental_nodal`.
-            Using the default `post.locations.elemental_nodal` results in a value
-            for every node at each element. Similarly, using `post.locations.elemental`
-            gives results with one value for each element, while using `post.locations.nodal`
-            gives results with one value for each node.
-        category:
-            Type of result requested. See the :class:`ResultCategory` class.
-        components:
-            Components to get results for.
-        norm:
-            Whether to return the norm of the results.
-        amplitude:
-            Whether to return the amplitude of the result. Overrides `sweeping_phase`.
-        sweeping_phase:
-            Sweeping phase value to extract result for. If a single `float` value is given, it
-            must be in degrees. Unused if `amplitude=True`.
-        selection:
-            Selection to get results for.
-            A Selection defines both spatial and time-like criteria for filtering.
-        frequencies:
-            Frequency value or list of frequency values to get results for.
-        set_ids:
-            List of sets to get results for.
-            A set is defined as a unique combination of {time, load step, sub-step}.
-        all_sets:
-            Whether to get results for all sets.
-        load_steps:
-            Load step number or list of load step numbers to get results for.
-            One can specify sub-steps of a load step with a tuple of format:
-            (load-step, sub-step number or list of sub-step numbers).
-        node_ids:
-            List of IDs of nodes to get results for.
-        element_ids:
-            List of IDs of elements to get results for.
-        named_selections:
-            Named selection or list of named selections to get results for.
-        expand_cyclic:
-            For cyclic problems, whether to expand the sectors.
-            Can take a list of sector numbers to select specific sectors to expand
-            (one-based indexing).
-            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-            by stage.
-        phase_angle_cyclic:
-             For cyclic problems, phase angle to apply (in degrees).
-        external_layer:
-             Select the external layer (last layer of solid elements under the skin)
-             of the mesh for plotting and data extraction. If a list is passed, the external
-             layer is computed over list of elements.
-        skin:
-             Select the skin (creates new 2D elements connecting the external nodes)
-             of the mesh for plotting and data extraction. If a list is passed, the skin
-             is computed over list of elements (not supported for cyclic symmetry). Getting the
-             skin on more than one result (several time freq sets, split data...) is only
-             supported starting with Ansys 2023R2.
-
-        Returns
-        -------
-        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        # Build the targeted spatial and time scoping
-        tot = (
-            (set_ids is not None)
-            + (all_sets is True)
-            + (frequencies is not None)
-            + (load_steps is not None)
-            + (selection is not None)
-        )
-        if tot > 1:
-            raise ValueError(
-                "Arguments all_sets, selection, set_ids, frequencies, "
-                "and load_steps are mutually exclusive."
-            )
-
-        tot = (
-            (node_ids is not None)
-            + (element_ids is not None)
-            + (named_selections is not None)
-            + (selection is not None)
-        )
-        if tot > 1:
-            raise ValueError(
-                "Arguments selection, named_selections, element_ids, "
-                "and node_ids are mutually exclusive"
-            )
-
-        selection = self._build_selection(
-            base_name=base_name,
-            category=category,
-            selection=selection,
-            set_ids=set_ids,
-            times=frequencies,
-            load_steps=load_steps,
-            all_sets=all_sets,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            location=location,
-            external_layer=external_layer,
-            skin=skin,
-        )
-
-        comp, to_extract, columns = self._create_components(
-            base_name, category, components
-        )
-
-        # Initialize a workflow
-        wf = dpf.Workflow(server=self._model._server)
+    ) -> (dpf.Workflow, Union[str, list[str], None], str):
+        """Generate (without evaluating) the Workflow to extract results."""
+        comp, to_extract, _ = self._create_components(base_name, category, components)
 
         force_elemental_nodal = self._requires_manual_averaging(
             base_name=base_name,
             location=location,
             category=category,
             selection=selection,
         )
@@ -198,14 +64,15 @@
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
         if selection.requires_mesh:
             # wf.set_input_name(_WfNames.mesh, result_op.inputs.mesh)
             mesh_wf = dpf.Workflow(server=self._model._server)
+            mesh_wf.add_operator(self._model.metadata.mesh_provider)
             mesh_wf.set_output_name(
                 _WfNames.initial_mesh, self._model.metadata.mesh_provider
             )
             selection.spatial_selection._selection.connect_with(
                 mesh_wf,
                 output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
             )
@@ -236,14 +103,15 @@
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
             if average_op is not None:
                 average_op[0].connect(0, out)
                 principal_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 average_op = None
             else:
                 principal_op.connect(0, out)
             wf.add_operator(operator=principal_op)
             # Set as future output of the workflow
             if len(to_extract) == 1:
@@ -260,30 +128,32 @@
             if (
                 average_op is not None
                 and category == ResultCategory.equivalent
                 and base_name[0] == "E"
             ):
                 equivalent_op.connect(0, out)
                 average_op[0].connect(0, equivalent_op)
-                wf.add_operator(operator=average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = average_op[1].outputs.fields_container
             elif average_op is not None:
                 average_op[0].connect(0, out)
                 equivalent_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = equivalent_op.outputs.fields_container
             else:
                 equivalent_op.connect(0, out)
                 out = equivalent_op.outputs.fields_container
             average_op = None
             base_name += "_VM"
 
         if average_op is not None:
             average_op[0].connect(0, out)
+            wf.add_operators(list(average_op))
             out = average_op[1].outputs.fields_container
 
         # Add an optional component selection step if result is vector, or matrix
         if (
             category
             in [
                 ResultCategory.vector,
@@ -323,29 +193,185 @@
             amplitude_op.connect(0, out)
             wf.add_operator(operator=amplitude_op)
             out = amplitude_op.outputs.fields_container
 
         # Add an optional norm operation if requested
         # (must be after sweeping_phase for U)
         if norm:
-            norm_op = self._model.operator(name="norm_fc")
-            norm_op.connect(0, out)
-            wf.add_operator(operator=norm_op)
-            out = norm_op.outputs.fields_container
-            comp = None
-            base_name += "_N"
+            wf, out, comp, base_name = self._append_norm(wf, out, base_name)
 
         # Set the workflow output
         wf.set_output_name("out", out)
         wf.progress_bar = False
+
+        return wf, comp, base_name
+
+    def _get_result(
+        self,
+        base_name: str,
+        location: str,
+        category: ResultCategory,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        amplitude: bool = False,
+        sweeping_phase: Union[float, None] = 0.0,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        frequencies: Union[float, List[float], None] = None,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        load_steps: Union[
+            int, List[int], Tuple[int, Union[int, List[int]]], None
+        ] = None,
+        named_selections: Union[List[str], str, None] = None,
+        selection: Union[Selection, None] = None,
+        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
+        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
+        exclusive.
+        If none of the above is given, only the first mode will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        amplitude:
+            Whether to return the amplitude of the result. Overrides `sweeping_phase`.
+        sweeping_phase:
+            Sweeping phase value to extract result for. If a single `float` value is given, it
+            must be in degrees. Unused if `amplitude=True`.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        # Build the targeted spatial and time scoping
+        tot = (
+            (set_ids is not None)
+            + (all_sets is True)
+            + (frequencies is not None)
+            + (load_steps is not None)
+            + (selection is not None)
+        )
+        if tot > 1:
+            raise ValueError(
+                "Arguments all_sets, selection, set_ids, frequencies, "
+                "and load_steps are mutually exclusive."
+            )
+
+        tot = (
+            (node_ids is not None)
+            + (element_ids is not None)
+            + (named_selections is not None)
+            + (selection is not None)
+        )
+        if tot > 1:
+            raise ValueError(
+                "Arguments selection, named_selections, element_ids, "
+                "and node_ids are mutually exclusive"
+            )
+
+        selection = self._build_selection(
+            base_name=base_name,
+            category=category,
+            selection=selection,
+            set_ids=set_ids,
+            times=frequencies,
+            load_steps=load_steps,
+            all_sets=all_sets,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            location=location,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+        wf, comp, base_name = self._get_result_workflow(
+            base_name=base_name,
+            location=location,
+            category=category,
+            components=components,
+            norm=norm,
+            amplitude=amplitude,
+            sweeping_phase=sweeping_phase,
+            selection=selection,
+            expand_cyclic=expand_cyclic,
+            phase_angle_cyclic=phase_angle_cyclic,
+        )
+
         # Evaluate  the workflow
         fc = wf.get_output("out", dpf.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
 
+        _, _, columns = self._create_components(base_name, category, components)
+
         # Test for empty results
         if (len(fc) == 0) or all([len(f) == 0 for f in fc]):
             warnings.warn(
                 message=f"Returned Dataframe with columns {columns} is empty.",
                 category=UserWarning,
             )
         comp_index = None
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/helpers/selections.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/helpers/selections.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/helpers/streamlines.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/helpers/streamlines.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/index.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/index.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/mesh.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/mesh.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/mesh_info.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/mesh_info.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/meshes.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/meshes.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/misc.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/misc_results.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/misc_results.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/modal_mechanical_simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/modal_mechanical_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,142 +12,27 @@
 from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
 class ModalMechanicalSimulation(MechanicalSimulation):
     """Provides methods for mechanical modal simulations."""
 
-    def _get_result(
+    def _get_result_workflow(
         self,
         base_name: str,
         location: str,
         category: ResultCategory,
         components: Union[str, List[str], int, List[int], None] = None,
         norm: bool = False,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        frequencies: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        modes: Union[int, List[int], None] = None,
-        named_selections: Union[List[str], str, None] = None,
         selection: Union[Selection, None] = None,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
-        external_layer: Union[bool, List[int]] = False,
-        skin: Union[bool, List[int]] = False,
-    ) -> DataFrame:
-        """Extract results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
-        exclusive.
-        If none of the above is given, only the first mode will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Parameters
-        ----------
-        base_name:
-            Base name for the requested result.
-        location:
-            Location to extract results at. Available locations are listed in
-            class:`post.locations` and are: `post.locations.nodal`,
-            `post.locations.elemental`, and `post.locations.elemental_nodal`.
-            Using the default `post.locations.elemental_nodal` results in a value
-            for every node at each element. Similarly, using `post.locations.elemental`
-            gives results with one value for each element, while using `post.locations.nodal`
-            gives results with one value for each node.
-        category:
-            Type of result requested. See the :class:`ResultCategory` class.
-        components:
-            Components to get results for.
-        norm:
-            Whether to return the norm of the results.
-        selection:
-            Selection to get results for.
-            A Selection defines both spatial and time-like criteria for filtering.
-        frequencies:
-            Frequency value or list of frequency values to get results for.
-        set_ids:
-            List of sets to get results for.
-            A set is defined as a unique combination of {time, load step, sub-step}.
-        all_sets:
-            Whether to get results for all sets/modes.
-        modes:
-            Mode number or list of mode numbers to get results for.
-        node_ids:
-            List of IDs of nodes to get results for.
-        element_ids:
-            List of IDs of elements to get results for.
-        named_selections:
-            Named selection or list of named selections to get results for.
-        expand_cyclic:
-            For cyclic problems, whether to expand the sectors.
-            Can take a list of sector numbers to select specific sectors to expand
-            (one-based indexing).
-            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-            by stage.
-        phase_angle_cyclic:
-             For cyclic problems, phase angle to apply (in degrees).
-        external_layer:
-             Select the external layer (last layer of solid elements under the skin)
-             of the mesh for plotting and data extraction. If a list is passed, the external
-             layer is computed over list of elements.
-        skin:
-             Select the skin (creates new 2D elements connecting the external nodes)
-             of the mesh for plotting and data extraction. If a list is passed, the skin
-             is computed over list of elements (not supported for cyclic symmetry). Getting the
-             skin on more than one result (several time freq sets, split data...) is only
-             supported starting with Ansys 2023R2.
-
-        Returns
-        -------
-        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        # Build the targeted spatial and time scoping
-        tot = (
-            (set_ids is not None)
-            + (all_sets is True)
-            + (frequencies is not None)
-            + (modes is not None)
-            + (selection is not None)
-        )
-        if tot > 1:
-            raise ValueError(
-                "Arguments all_sets, selection, set_ids, frequencies, "
-                "and modes are mutually exclusive."
-            )
-        elif tot == 0:
-            set_ids = 1
-
-        selection = self._build_selection(
-            base_name=base_name,
-            category=category,
-            selection=selection,
-            set_ids=set_ids if set_ids else modes,
-            times=frequencies,
-            load_steps=None,
-            all_sets=all_sets,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            location=location,
-            external_layer=external_layer,
-            skin=skin,
-        )
-
-        comp, to_extract, columns = self._create_components(
-            base_name, category, components
-        )
-
-        # Initialize a workflow
-        wf = dpf.Workflow(server=self._model._server)
+    ) -> (dpf.Workflow, Union[str, list[str], None], str):
+        """Generate (without evaluating) the Workflow to extract results."""
+        comp, to_extract, _ = self._create_components(base_name, category, components)
 
         force_elemental_nodal = self._requires_manual_averaging(
             base_name=base_name,
             location=location,
             category=category,
             selection=selection,
         )
@@ -167,14 +52,15 @@
 
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
         if selection.requires_mesh:
             mesh_wf = dpf.Workflow(server=self._model._server)
+            mesh_wf.add_operator(self._model.metadata.mesh_provider)
             mesh_wf.set_output_name(
                 _WfNames.initial_mesh, self._model.metadata.mesh_provider
             )
             selection.spatial_selection._selection.connect_with(
                 mesh_wf,
                 output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
             )
@@ -205,14 +91,15 @@
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
             if average_op is not None:
                 average_op[0].connect(0, out)
                 principal_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 average_op = None
             else:
                 principal_op.connect(0, out)
             wf.add_operator(operator=principal_op)
             # Set as future output of the workflow
             if len(to_extract) == 1:
@@ -229,30 +116,32 @@
             if (
                 average_op is not None
                 and category == ResultCategory.equivalent
                 and base_name[0] == "E"
             ):
                 equivalent_op.connect(0, out)
                 average_op[0].connect(0, equivalent_op)
-                wf.add_operator(operator=average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = average_op[1].outputs.fields_container
             elif average_op is not None:
                 average_op[0].connect(0, out)
                 equivalent_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = equivalent_op.outputs.fields_container
             else:
                 equivalent_op.connect(0, out)
                 out = equivalent_op.outputs.fields_container
             average_op = None
             base_name += "_VM"
 
         if average_op is not None:
             average_op[0].connect(0, out)
+            wf.add_operators(list(average_op))
             out = average_op[1].outputs.fields_container
 
         # Add an optional component selection step if result is vector, matrix, or principal
         if (category in [ResultCategory.vector, ResultCategory.matrix]) and (
             to_extract is not None
         ):
             # Instantiate a component selector operator
@@ -266,36 +155,168 @@
             out = extract_op.outputs.fields_container
             if len(to_extract) == 1:
                 base_name += f"_{comp[0]}"
                 comp = None
 
         # Add an optional norm operation if requested
         if norm:
-            norm_op = self._model.operator(name="norm_fc")
-            norm_op.connect(0, out)
-            wf.add_operator(operator=norm_op)
-            out = norm_op.outputs.fields_container
-            comp = None
-            base_name += "_N"
+            wf, out, comp, base_name = self._append_norm(wf, out, base_name)
 
         # Set the workflow output
         wf.set_output_name("out", out)
         wf.progress_bar = False
+
+        return wf, comp, base_name
+
+    def _get_result(
+        self,
+        base_name: str,
+        location: str,
+        category: ResultCategory,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        frequencies: Union[float, List[float], None] = None,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        modes: Union[int, List[int], None] = None,
+        named_selections: Union[List[str], str, None] = None,
+        selection: Union[Selection, None] = None,
+        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
+        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `frequencies`, and `modes` are mutually
+        exclusive.
+        If none of the above is given, only the first mode will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        frequencies:
+            Frequency value or list of frequency values to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets/modes.
+        modes:
+            Mode number or list of mode numbers to get results for.
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+        Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        # Build the targeted spatial and time scoping
+        tot = (
+            (set_ids is not None)
+            + (all_sets is True)
+            + (frequencies is not None)
+            + (modes is not None)
+            + (selection is not None)
+        )
+        if tot > 1:
+            raise ValueError(
+                "Arguments all_sets, selection, set_ids, frequencies, "
+                "and modes are mutually exclusive."
+            )
+        elif tot == 0:
+            set_ids = 1
+
+        selection = self._build_selection(
+            base_name=base_name,
+            category=category,
+            selection=selection,
+            set_ids=set_ids if set_ids else modes,
+            times=frequencies,
+            load_steps=None,
+            all_sets=all_sets,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            location=location,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+        wf, comp, base_name = self._get_result_workflow(
+            base_name=base_name,
+            location=location,
+            category=category,
+            components=components,
+            norm=norm,
+            selection=selection,
+            expand_cyclic=expand_cyclic,
+            phase_angle_cyclic=phase_angle_cyclic,
+        )
+
         # Evaluate  the workflow
         fc = wf.get_output("out", dpf.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
 
         submesh = None
         if selection.outputs_mesh:
             selection.spatial_selection._selection.progress_bar = False
             submesh = selection.spatial_selection._selection.get_output(
                 _WfNames.mesh, dpf.types.meshed_region
             )
 
+        _, _, columns = self._create_components(base_name, category, components)
         return self._create_dataframe(
             fc, location, columns, comp, base_name, disp_wf, submesh
         )
 
     def displacement(
         self,
         node_ids: Union[List[int], None] = None,
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/named_selection.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/named_selection.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/nodes.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/phase.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/phase.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/post_utility.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/post_utility.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_data.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_data.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_definition.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_definition.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_evaluation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/result_object.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/result_object.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/scalar.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/scalar.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/selection.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,42 +242,43 @@
         """
         if isinstance(named_selection, str):
             op = operators.scoping.on_named_selection(
                 requested_location=location,
                 named_selection_name=named_selection,
                 server=self._server,
             )
+            self._selection.add_operator(op)
             self._selection.set_input_name(
                 _WfNames.data_sources, op.inputs.data_sources
             )
             # self._selection.set_input_name(
             #     _WfNames.streams, op.inputs.streams_container
             # )
             self._selection.set_output_name(_WfNames.scoping, op.outputs.mesh_scoping)
         else:
             op = operators.utility.merge_scopings(server=self._server)
             forward_ds = operators.utility.forward(any=None, server=self._server)
             forward_sc = operators.utility.forward(any=None, server=self._server)
+            self._selection.add_operators([op, forward_ds, forward_sc])
             self._selection.set_input_name(_WfNames.data_sources, forward_ds.inputs.any)
             # self._selection.set_input_name(_WfNames.streams, forward_sc.inputs.any)
             for pin, ns in enumerate(named_selection):
                 mesh_scoping_op = operators.scoping.on_named_selection(
                     requested_location=location,
                     named_selection_name=ns,
                     server=self._server,
                     # data_sources=forward_ds.outputs.any,
                     # streams_container=forward_sc.outputs.any,
                 )
+                self._selection.add_operator(mesh_scoping_op)
                 mesh_scoping_op.connect(3, forward_sc.outputs.any)
                 mesh_scoping_op.connect(4, forward_ds.outputs.any)
                 op.connect(pin, mesh_scoping_op.outputs.mesh_scoping)
             self._selection.set_output_name(_WfNames.scoping, op.outputs.merged_scoping)
 
-        self._selection.add_operator(op)
-
     def select_external_layer(
         self,
         location: Union[locations, str] = locations.elemental,
         result_native_location: Union[str, locations, None] = None,
         elements: Union[List[int], Scoping, None] = None,
         is_model_cyclic: str = "not_cyclic",
     ) -> None:
@@ -308,17 +309,19 @@
         if (
             result_native_location is not None
             and _is_model_cyclic(is_model_cyclic)
             and location != result_native_location
         ):
             location = result_native_location
         op = operators.mesh.external_layer(server=self._server)
+        self._selection.add_operator(op)
 
         if _is_model_cyclic(is_model_cyclic):
             mesh_provider_cyc = operators.mesh.mesh_provider()
+            self._selection.add_operator(mesh_provider_cyc)
             self._selection.set_input_name(_WfNames.read_cyclic, mesh_provider_cyc, 14)
             self._selection.set_input_name(
                 _WfNames.cyclic_sectors_to_expand, mesh_provider_cyc, 18
             )
             self._selection.set_input_name(
                 _WfNames.data_sources, mesh_provider_cyc.inputs.data_sources
             )
@@ -331,28 +334,30 @@
                         server=self._server, ids=elements, location=locations.elemental
                     )
                 mesh_by_scop_op = operators.mesh.from_scoping(
                     mesh=mesh_provider_cyc,
                     scoping=elements,
                     server=self._server,
                 )
+                self._selection.add_operator(mesh_by_scop_op)
                 op.inputs.mesh.connect(mesh_by_scop_op)
             else:
                 op.inputs.mesh.connect(mesh_provider_cyc)
             self._selection.set_input_name(
                 _WfNames.initial_mesh, mesh_provider_cyc, 100
             )  # hack
         elif elements is not None:
             if not isinstance(elements, Scoping):
                 elements = Scoping(
                     server=self._server, ids=elements, location=locations.elemental
                 )
             mesh_by_scop_op = operators.mesh.from_scoping(
                 scoping=elements, server=self._server
             )
+            self._selection.add_operator(mesh_by_scop_op)
             self._selection.set_input_name(
                 _WfNames.initial_mesh, mesh_by_scop_op.inputs.mesh
             )
             op.inputs.mesh.connect(mesh_by_scop_op)
         else:
             self._selection.set_input_name(_WfNames.initial_mesh, op.inputs.mesh)
 
@@ -363,16 +368,14 @@
                 _WfNames.scoping, op.outputs.nodes_mesh_scoping
             )
         elif location == locations.elemental or location == locations.elemental_nodal:
             self._selection.set_output_name(
                 _WfNames.scoping, op.outputs.elements_mesh_scoping
             )
 
-        self._selection.add_operator(op)
-
     def select_skin(
         self,
         location: Union[locations, str] = locations.elemental,
         result_native_location: Union[str, locations, None] = None,
         elements: Union[List[int], Scoping, None] = None,
         is_model_cyclic: str = "not_cyclic",
     ) -> None:
@@ -398,18 +401,20 @@
             elements for cyclic symmetry is not supported.
         is_model_cyclic:
             Cyclic type: ``not_cyclic``, ``single_stage``, or ``multi_stage``. This value can
             be returned by the Operator ``operators.metadata.is_cyclic``. Used to get the skin
             on the expanded mesh.
         """
         op = operators.mesh.skin(server=self._server)
+        self._selection.add_operator(op)
         mesh_input = op.inputs.mesh
 
         if _is_model_cyclic(is_model_cyclic):
             mesh_provider_cyc = operators.mesh.mesh_provider()
+            self._selection.add_operator(mesh_provider_cyc)
             self._selection.set_input_name(_WfNames.read_cyclic, mesh_provider_cyc, 14)
             self._selection.set_input_name(
                 _WfNames.cyclic_sectors_to_expand, mesh_provider_cyc, 18
             )
             self._selection.set_input_name(
                 _WfNames.data_sources, mesh_provider_cyc.inputs.data_sources
             )
@@ -426,14 +431,15 @@
                         server=self._server, ids=elements, location=locations.elemental
                     )
                 mesh_by_scop_op = operators.mesh.from_scoping(
                     mesh=mesh_provider_cyc,
                     scoping=elements,
                     server=self._server,
                 )
+                self._selection.add_operator(mesh_by_scop_op)
                 op.inputs.mesh.connect(mesh_by_scop_op)
             else:
                 op.inputs.mesh.connect(mesh_provider_cyc)
             self._selection.set_input_name(
                 _WfNames.initial_mesh, mesh_provider_cyc, 100
             )  # hack
             mesh_input = None
@@ -442,14 +448,15 @@
             if not isinstance(elements, Scoping):
                 elements = Scoping(
                     server=self._server, ids=elements, location=locations.elemental
                 )
             mesh_by_scop_op = operators.mesh.from_scoping(
                 scoping=elements, server=self._server
             )
+            self._selection.add_operator(mesh_by_scop_op)
             mesh_input = mesh_by_scop_op.inputs.mesh
             op.inputs.mesh.connect(mesh_by_scop_op)
 
         if mesh_input is not None:
             self._selection.set_input_name(_WfNames.initial_mesh, mesh_input)
             if location == result_native_location:
                 self._selection.set_output_name(_WfNames.mesh, op.outputs.mesh)
@@ -462,23 +469,22 @@
         elif not _is_model_cyclic(is_model_cyclic) and (
             result_native_location == locations.elemental
             or result_native_location == locations.elemental_nodal
         ):
             transpose_op = operators.scoping.transpose(
                 mesh_scoping=op.outputs.nodes_mesh_scoping, server=self._server
             )
+            self._selection.add_operator(transpose_op)
             self._selection.set_input_name(
                 _WfNames.initial_mesh, transpose_op.inputs.meshed_region
             )
             self._selection.set_output_name(
                 _WfNames.scoping, transpose_op.outputs.mesh_scoping_as_scoping
             )
 
-        self._selection.add_operator(op)
-
     def select_with_scoping(self, scoping: Scoping):
         """Directly sets the scoping as the spatial selection.
 
         Parameters
         ----------
         scoping:
             Scoping to use for spatial selection.
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,20 +538,31 @@
         op = self._model.operator(name=name)
         op.connect(7, self.mesh._meshed_region)
         if force_elemental_nodal:
             op.connect(9, "ElementalNodal")
         elif location:
             op.connect(9, location)
         wf = Workflow(server=self._model._server)
+        wf.add_operator(op)
         wf.set_input_name(_WfNames.read_cyclic, op, 14)
         wf.set_input_name(_WfNames.cyclic_sectors_to_expand, op, 18)
         wf.set_input_name(_WfNames.cyclic_phase, op, 19)
         wf.set_output_name(_WfNames.result, op, 0)
         return wf, op
 
+    def _append_norm(self, wf, out, base_name):
+        """Append a norm operator to the current result workflow."""
+        norm_op = self._model.operator(name="norm_fc")
+        norm_op.connect(0, out)
+        wf.add_operator(operator=norm_op)
+        base_name += "_N"
+        out = norm_op.outputs.fields_container
+        comp = None
+        return wf, out, comp, base_name
+
     def _create_components(self, base_name, category, components):
         comp = None
         # Build the list of requested results
         if category in [ResultCategory.scalar, ResultCategory.equivalent]:
             # A scalar or equivalent result has no components
             to_extract = None
             columns = [base_name]
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/species.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/species.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/static_mechanical_simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/static_mechanical_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,144 +12,27 @@
 from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
 class StaticMechanicalSimulation(MechanicalSimulation):
     """Provides methods for mechanical static simulations."""
 
-    def _get_result(
+    def _get_result_workflow(
         self,
         base_name: str,
         location: str,
         category: ResultCategory,
         components: Union[str, List[str], int, List[int], None] = None,
         norm: bool = False,
         selection: Union[Selection, None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        named_selections: Union[List[str], str, None] = None,
         expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
         phase_angle_cyclic: Union[float, None] = None,
-        external_layer: Union[bool, List[int]] = False,
-        skin: Union[bool, List[int]] = False,
-    ) -> DataFrame:
-        """Extract results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Parameters
-        ----------
-        base_name:
-            Base name for the requested result.
-        location:
-            Location to extract results at. Available locations are listed in
-            class:`post.locations` and are: `post.locations.nodal`,
-            `post.locations.elemental`, and `post.locations.elemental_nodal`.
-            Using the default `post.locations.elemental_nodal` results in a value
-            for every node at each element. Similarly, using `post.locations.elemental`
-            gives results with one value for each element, while using `post.locations.nodal`
-            gives results with one value for each node.
-        category:
-            Type of result requested. See the :class:`ResultCategory` class.
-        components:
-            Components to get results for.
-        norm:
-            Whether to return the norm of the results.
-        selection:
-            Selection to get results for.
-            A Selection defines both spatial and time-like criteria for filtering.
-        times:
-            List of times to get results for.
-        set_ids:
-            List of sets to get results for.
-            A set is defined as a unique combination of {time, load step, sub-step}.
-        all_sets:
-            Whether to get results for all sets.
-        load_steps:
-            Load step number or list of load step numbers to get results for.
-            One can specify sub-steps of a load step with a tuple of format:
-            (load-step, sub-step number or list of sub-step numbers).
-        node_ids:
-            List of IDs of nodes to get results for.
-        element_ids:
-            List of IDs of elements to get results for.
-        named_selections:
-            Named selection or list of named selections to get results for.
-        expand_cyclic:
-            For cyclic problems, whether to expand the sectors.
-            Can take a list of sector numbers to select specific sectors to expand
-            (one-based indexing).
-            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
-            by stage.
-        phase_angle_cyclic:
-             For cyclic problems, phase angle to apply (in degrees).
-        external_layer:
-             Select the external layer (last layer of solid elements under the skin)
-             of the mesh for plotting and data extraction. If a list is passed, the external
-             layer is computed over list of elements.
-        skin:
-             Select the skin (creates new 2D elements connecting the external nodes)
-             of the mesh for plotting and data extraction. If a list is passed, the skin
-             is computed over list of elements (not supported for cyclic symmetry). Getting the
-             skin on more than one result (several time freq sets, split data...) is only
-             supported starting with Ansys 2023R2.
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        # Build the targeted time scoping
-        tot = (
-            (set_ids is not None)
-            + (all_sets is True)
-            + (times is not None)
-            + (load_steps is not None)
-            + (selection is not None)
-        )
-        if tot > 1:
-            raise ValueError(
-                "Arguments all_sets, selection, set_ids, times, "
-                "and load_steps are mutually exclusive."
-            )
-
-        selection = self._build_selection(
-            base_name=base_name,
-            category=category,
-            selection=selection,
-            set_ids=set_ids,
-            times=times,
-            load_steps=load_steps,
-            all_sets=all_sets,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            location=location,
-            external_layer=external_layer,
-            skin=skin,
-        )
-
-        comp, to_extract, columns = self._create_components(
-            base_name, category, components
-        )
-
-        # Initialize a workflow
-        # wf = core.Workflow(server=self._model._server)
+    ) -> (core.Workflow, Union[str, list[str], None], str):
+        """Generate (without evaluating) the Workflow to extract results."""
+        comp, to_extract, _ = self._create_components(base_name, category, components)
 
         force_elemental_nodal = self._requires_manual_averaging(
             base_name=base_name,
             location=location,
             category=category,
             selection=selection,
         )
@@ -169,14 +52,15 @@
 
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
         if selection.requires_mesh:
             mesh_wf = core.Workflow(server=self._model._server)
+            mesh_wf.add_operator(self._model.metadata.mesh_provider)
             mesh_wf.set_output_name(
                 _WfNames.initial_mesh, self._model.metadata.mesh_provider
             )
             selection.spatial_selection._selection.connect_with(
                 mesh_wf,
                 output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
             )
@@ -202,18 +86,18 @@
             )
 
         # Add a step to compute principal invariants if result is principal
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
-
             if average_op is not None:
                 average_op[0].connect(0, out)
                 principal_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 average_op = None
             else:
                 principal_op.connect(0, out)
             wf.add_operator(operator=principal_op)
             # Set as future output of the workflow
             if len(to_extract) == 1:
@@ -230,31 +114,33 @@
             if (
                 average_op is not None
                 and category == ResultCategory.equivalent
                 and base_name[0] == "E"
             ):
                 equivalent_op.connect(0, out)
                 average_op[0].connect(0, equivalent_op)
-                wf.add_operator(operator=average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = average_op[1].outputs.fields_container
             elif average_op is not None:
                 average_op[0].connect(0, out)
                 equivalent_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = equivalent_op.outputs.fields_container
             else:
                 equivalent_op.connect(0, out)
                 out = equivalent_op.outputs.fields_container
 
             average_op = None
             base_name += "_VM"
 
         if average_op is not None:
             average_op[0].connect(0, out)
+            wf.add_operators(list(average_op))
             out = average_op[1].outputs.fields_container
 
         # Add an optional component selection step if result is vector, matrix, or principal
         if (category in [ResultCategory.vector, ResultCategory.matrix]) and (
             to_extract is not None
         ):
             # Instantiate a component selector operator
@@ -268,35 +154,170 @@
             out = extract_op.outputs.fields_container
             if len(to_extract) == 1:
                 base_name += f"_{comp[0]}"
                 comp = None
 
         # Add an optional norm operation if requested
         if norm:
-            norm_op = self._model.operator(name="norm_fc")
-            norm_op.connect(0, out)
-            wf.add_operator(operator=norm_op)
-            out = norm_op.outputs.fields_container
-            comp = None
-            base_name += "_N"
+            wf, out, comp, base_name = self._append_norm(wf, out, base_name)
 
         # Set the workflow output
         wf.set_output_name("out", out)
         wf.progress_bar = False
+
+        return wf, comp, base_name
+
+    def _get_result(
+        self,
+        base_name: str,
+        location: str,
+        category: ResultCategory,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        selection: Union[Selection, None] = None,
+        times: Union[float, List[float], None] = None,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        load_steps: Union[
+            int, List[int], Tuple[int, Union[int, List[int]]], None
+        ] = None,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        named_selections: Union[List[str], str, None] = None,
+        expand_cyclic: Union[bool, List[Union[int, List[int]]]] = True,
+        phase_angle_cyclic: Union[float, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
+        exclusive.
+        If none of the above is given, only the last result will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        times:
+            List of times to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+        expand_cyclic:
+            For cyclic problems, whether to expand the sectors.
+            Can take a list of sector numbers to select specific sectors to expand
+            (one-based indexing).
+            If the problem is multi-stage, can take a list of lists of sector numbers, ordered
+            by stage.
+        phase_angle_cyclic:
+             For cyclic problems, phase angle to apply (in degrees).
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        # Build the targeted time scoping
+        tot = (
+            (set_ids is not None)
+            + (all_sets is True)
+            + (times is not None)
+            + (load_steps is not None)
+            + (selection is not None)
+        )
+        if tot > 1:
+            raise ValueError(
+                "Arguments all_sets, selection, set_ids, times, "
+                "and load_steps are mutually exclusive."
+            )
+
+        selection = self._build_selection(
+            base_name=base_name,
+            category=category,
+            selection=selection,
+            set_ids=set_ids,
+            times=times,
+            load_steps=load_steps,
+            all_sets=all_sets,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            location=location,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+        wf, comp, base_name = self._get_result_workflow(
+            base_name=base_name,
+            location=location,
+            category=category,
+            components=components,
+            norm=norm,
+            selection=selection,
+            expand_cyclic=expand_cyclic,
+            phase_angle_cyclic=phase_angle_cyclic,
+        )
+
         # Evaluate  the workflow
         fc = wf.get_output("out", core.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
         submesh = None
         if selection.outputs_mesh:
             selection.spatial_selection._selection.progress_bar = False
             submesh = selection.spatial_selection._selection.get_output(
                 _WfNames.mesh, core.types.meshed_region
             )
 
+        _, _, columns = self._create_components(base_name, category, components)
+
         return self._create_dataframe(
             fc, location, columns, comp, base_name, disp_wf, submesh
         )
 
     def displacement(
         self,
         node_ids: Union[List[int], None] = None,
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/strain.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/strain.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/stress.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/stress.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/temperature.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/temperature.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/tensor.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/tensor.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/transient_mechanical_simulation.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/transient_mechanical_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,136 +12,25 @@
 from ansys.dpf.post.selection import Selection, _WfNames
 from ansys.dpf.post.simulation import MechanicalSimulation, ResultCategory
 
 
 class TransientMechanicalSimulation(MechanicalSimulation):
     """Provides methods for mechanical transient simulations."""
 
-    def _get_result(
+    def _get_result_workflow(
         self,
         base_name: str,
         location: str,
         category: ResultCategory,
         components: Union[str, List[str], int, List[int], None] = None,
         norm: bool = False,
         selection: Union[Selection, None] = None,
-        times: Union[float, List[float], None] = None,
-        set_ids: Union[int, List[int], None] = None,
-        all_sets: bool = False,
-        load_steps: Union[
-            int, List[int], Tuple[int, Union[int, List[int]]], None
-        ] = None,
-        node_ids: Union[List[int], None] = None,
-        element_ids: Union[List[int], None] = None,
-        named_selections: Union[List[str], str, None] = None,
-        external_layer: Union[bool, List[int]] = False,
-        skin: Union[bool, List[int]] = False,
-    ) -> DataFrame:
-        """Extract results from the simulation.
-
-        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
-        exclusive.
-        If none of the above is given, only the last result will be returned.
-
-        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
-        exclusive.
-        If none of the above is given, results will be extracted for the whole mesh.
-
-        Parameters
-        ----------
-        base_name:
-            Base name for the requested result.
-        location:
-            Location to extract results at. Available locations are listed in
-            class:`post.locations` and are: `post.locations.nodal`,
-            `post.locations.elemental`, and `post.locations.elemental_nodal`.
-            Using the default `post.locations.elemental_nodal` results in a value
-            for every node at each element. Similarly, using `post.locations.elemental`
-            gives results with one value for each element, while using `post.locations.nodal`
-            gives results with one value for each node.
-        category:
-            Type of result requested. See the :class:`ResultCategory` class.
-        components:
-            Components to get results for.
-        norm:
-            Whether to return the norm of the results.
-        selection:
-            Selection to get results for.
-            A Selection defines both spatial and time-like criteria for filtering.
-            It takes precedence over any other filter argument.
-        times:
-            List of times to get results for.
-        set_ids:
-            List of sets to get results for.
-            A set is defined as a unique combination of {time, load step, sub-step}.
-        all_sets:
-            Whether to get results for all sets.
-        load_steps:
-            Load step number or list of load step numbers to get results for.
-            One can specify sub-steps of a load step with a tuple of format:
-            (load-step, sub-step number or list of sub-step numbers).
-        node_ids:
-            List of IDs of nodes to get results for.
-        element_ids:
-            List of IDs of elements to get results for.
-        named_selections:
-            Named selection or list of named selections to get results for.
-            A Selection defines both spatial and time-like criteria for filtering.
-        external_layer:
-             Select the external layer (last layer of solid elements under the skin)
-             of the mesh for plotting and data extraction. If a list is passed, the external
-             layer is computed over list of elements.
-        skin:
-             Select the skin (creates new 2D elements connecting the external nodes)
-             of the mesh for plotting and data extraction. If a list is passed, the skin
-             is computed over list of elements (not supported for cyclic symmetry). Getting the
-             skin on more than one result (several time freq sets, split data...) is only
-             supported starting with Ansys 2023R2.
-
-        Returns
-        -------
-            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
-
-        """
-        # Build the targeted time scoping
-        tot = (
-            (set_ids is not None)
-            + (all_sets is True)
-            + (times is not None)
-            + (load_steps is not None)
-            + (selection is not None)
-        )
-        if tot > 1:
-            raise ValueError(
-                "Arguments all_sets, selection, set_ids, times, "
-                "and load_steps are mutually exclusive."
-            )
-
-        selection = self._build_selection(
-            base_name=base_name,
-            category=category,
-            selection=selection,
-            set_ids=set_ids,
-            times=times,
-            load_steps=load_steps,
-            all_sets=all_sets,
-            node_ids=node_ids,
-            element_ids=element_ids,
-            named_selections=named_selections,
-            location=location,
-            external_layer=external_layer,
-            skin=skin,
-        )
-
-        comp, to_extract, columns = self._create_components(
-            base_name, category, components
-        )
-
-        # Initialize a workflow
-        wf = dpf.Workflow(server=self._model._server)
+    ) -> (dpf.Workflow, Union[str, list[str], None], str):
+        """Generate (without evaluating) the Workflow to extract results."""
+        comp, to_extract, _ = self._create_components(base_name, category, components)
 
         force_elemental_nodal = self._requires_manual_averaging(
             base_name=base_name,
             location=location,
             category=category,
             selection=selection,
         )
@@ -161,14 +50,15 @@
         wf.connect_with(
             selection.time_freq_selection._selection,
             output_input_names=("scoping", "time_scoping"),
         )
         if selection.requires_mesh:
             # wf.set_input_name(_WfNames.mesh, result_op.inputs.mesh)
             mesh_wf = dpf.Workflow(server=self._model._server)
+            mesh_wf.add_operator(self._model.metadata.mesh_provider)
             mesh_wf.set_output_name(
                 _WfNames.initial_mesh, self._model.metadata.mesh_provider
             )
             selection.spatial_selection._selection.connect_with(
                 mesh_wf,
                 output_input_names={_WfNames.initial_mesh: _WfNames.initial_mesh},
             )
@@ -195,18 +85,20 @@
         if category == ResultCategory.principal:
             # Instantiate the required operator
             principal_op = self._model.operator(name="invariants_fc")
             # Corresponds to scripting name principal_invariants
             if average_op is not None:
                 average_op[0].connect(0, out)
                 principal_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 average_op = None
             else:
                 principal_op.connect(0, out)
+            wf.add_operator(operator=principal_op)
             # Set as future output of the workflow
             if len(to_extract) == 1:
                 out = getattr(principal_op.outputs, f"fields_eig_{to_extract[0]+1}")
             else:
                 raise NotImplementedError("Cannot combine principal results yet.")
                 # We need to define the behavior for storing different results in a DataFrame
 
@@ -218,30 +110,32 @@
             if (
                 average_op is not None
                 and category == ResultCategory.equivalent
                 and base_name[0] == "E"
             ):
                 equivalent_op.connect(0, out)
                 average_op[0].connect(0, equivalent_op)
-                wf.add_operator(operator=average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = average_op[1].outputs.fields_container
             elif average_op is not None:
                 average_op[0].connect(0, out)
                 equivalent_op.connect(0, average_op[1])
+                wf.add_operators(list(average_op))
                 # Set as future output of the workflow
                 out = equivalent_op.outputs.fields_container
             else:
                 equivalent_op.connect(0, out)
                 out = equivalent_op.outputs.fields_container
             average_op = None
             base_name += "_VM"
 
         if average_op is not None:
             average_op[0].connect(0, out)
+            wf.add_operators(list(average_op))
             out = average_op[1].outputs.fields_container
 
         # Add an optional component selection step if result is vector, matrix, or principal
         if (
             category
             in [
                 ResultCategory.vector,
@@ -259,36 +153,160 @@
             out = extract_op.outputs.fields_container
             if len(to_extract) == 1:
                 base_name += f"_{comp[0]}"
                 comp = None
 
         # Add an optional norm operation if requested
         if norm:
-            norm_op = self._model.operator(name="norm_fc")
-            norm_op.connect(0, out)
-            wf.add_operator(operator=norm_op)
-            out = norm_op.outputs.fields_container
-            comp = None
-            base_name += "_N"
+            wf, out, comp, base_name = self._append_norm(wf, out, base_name)
 
         # Set the workflow output
         wf.set_output_name("out", out)
         wf.progress_bar = False
+
+        return wf, comp, base_name
+
+    def _get_result(
+        self,
+        base_name: str,
+        location: str,
+        category: ResultCategory,
+        components: Union[str, List[str], int, List[int], None] = None,
+        norm: bool = False,
+        selection: Union[Selection, None] = None,
+        times: Union[float, List[float], None] = None,
+        set_ids: Union[int, List[int], None] = None,
+        all_sets: bool = False,
+        load_steps: Union[
+            int, List[int], Tuple[int, Union[int, List[int]]], None
+        ] = None,
+        node_ids: Union[List[int], None] = None,
+        element_ids: Union[List[int], None] = None,
+        named_selections: Union[List[str], str, None] = None,
+        external_layer: Union[bool, List[int]] = False,
+        skin: Union[bool, List[int]] = False,
+    ) -> DataFrame:
+        """Extract results from the simulation.
+
+        Arguments `selection`, `set_ids`, `all_sets`, `times`, and `load_steps` are mutually
+        exclusive.
+        If none of the above is given, only the last result will be returned.
+
+        Arguments `selection`, `named_selections`, `element_ids`, and `node_ids` are mutually
+        exclusive.
+        If none of the above is given, results will be extracted for the whole mesh.
+
+        Parameters
+        ----------
+        base_name:
+            Base name for the requested result.
+        location:
+            Location to extract results at. Available locations are listed in
+            class:`post.locations` and are: `post.locations.nodal`,
+            `post.locations.elemental`, and `post.locations.elemental_nodal`.
+            Using the default `post.locations.elemental_nodal` results in a value
+            for every node at each element. Similarly, using `post.locations.elemental`
+            gives results with one value for each element, while using `post.locations.nodal`
+            gives results with one value for each node.
+        category:
+            Type of result requested. See the :class:`ResultCategory` class.
+        components:
+            Components to get results for.
+        norm:
+            Whether to return the norm of the results.
+        selection:
+            Selection to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+            It takes precedence over any other filter argument.
+        times:
+            List of times to get results for.
+        set_ids:
+            List of sets to get results for.
+            A set is defined as a unique combination of {time, load step, sub-step}.
+        all_sets:
+            Whether to get results for all sets.
+        load_steps:
+            Load step number or list of load step numbers to get results for.
+            One can specify sub-steps of a load step with a tuple of format:
+            (load-step, sub-step number or list of sub-step numbers).
+        node_ids:
+            List of IDs of nodes to get results for.
+        element_ids:
+            List of IDs of elements to get results for.
+        named_selections:
+            Named selection or list of named selections to get results for.
+            A Selection defines both spatial and time-like criteria for filtering.
+        external_layer:
+             Select the external layer (last layer of solid elements under the skin)
+             of the mesh for plotting and data extraction. If a list is passed, the external
+             layer is computed over list of elements.
+        skin:
+             Select the skin (creates new 2D elements connecting the external nodes)
+             of the mesh for plotting and data extraction. If a list is passed, the skin
+             is computed over list of elements (not supported for cyclic symmetry). Getting the
+             skin on more than one result (several time freq sets, split data...) is only
+             supported starting with Ansys 2023R2.
+
+        Returns
+        -------
+            Returns a :class:`ansys.dpf.post.data_object.DataFrame` instance.
+
+        """
+        # Build the targeted time scoping
+        tot = (
+            (set_ids is not None)
+            + (all_sets is True)
+            + (times is not None)
+            + (load_steps is not None)
+            + (selection is not None)
+        )
+        if tot > 1:
+            raise ValueError(
+                "Arguments all_sets, selection, set_ids, times, "
+                "and load_steps are mutually exclusive."
+            )
+
+        selection = self._build_selection(
+            base_name=base_name,
+            category=category,
+            selection=selection,
+            set_ids=set_ids,
+            times=times,
+            load_steps=load_steps,
+            all_sets=all_sets,
+            node_ids=node_ids,
+            element_ids=element_ids,
+            named_selections=named_selections,
+            location=location,
+            external_layer=external_layer,
+            skin=skin,
+        )
+
+        wf, comp, base_name = self._get_result_workflow(
+            base_name=base_name,
+            location=location,
+            category=category,
+            components=components,
+            norm=norm,
+            selection=selection,
+        )
+
         # Evaluate  the workflow
         fc = wf.get_output("out", dpf.types.fields_container)
 
         disp_wf = self._generate_disp_workflow(fc, selection)
 
         submesh = None
         if selection.outputs_mesh:
             selection.spatial_selection._selection.progress_bar = False
             submesh = selection.spatial_selection._selection.get_output(
                 _WfNames.mesh, dpf.types.meshed_region
             )
 
+        _, _, columns = self._create_components(base_name, category, components)
         return self._create_dataframe(
             fc, location, columns, comp, base_name, disp_wf=disp_wf, submesh=submesh
         )
 
     def displacement(
         self,
         node_ids: Union[List[int], None] = None,
```

### Comparing `ansys_dpf_post-0.6.0/src/ansys/dpf/post/vector.py` & `ansys_dpf_post-0.7.0/src/ansys/dpf/post/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_post-0.6.0/PKG-INFO` & `ansys_dpf_post-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-post
-Version: 0.6.0
+Version: 0.7.0
 Summary: PyDPF-Post Python library.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

