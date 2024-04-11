# Comparing `tmp/generation_models-0.6.0.tar.gz` & `tmp/generation_models-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.6.0.tar", max compression
+gzip compressed data, was "generation_models-0.7.0.tar", max compression
```

## Comparing `generation_models-0.6.0.tar` & `generation_models-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       13 2023-10-12 04:36:37.827057 generation_models-0.6.0/generation_models/.gitignore
--rw-r--r--   0        0        0       47 2024-04-05 22:18:23.392678 generation_models-0.6.0/generation_models/__init__.py
--rw-r--r--   0        0        0   128989 2024-04-10 03:52:53.009565 generation_models-0.6.0/generation_models/generation_models.py
--rw-r--r--   0        0        0      640 2024-04-10 03:52:53.010491 generation_models-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 generation_models-0.6.0/setup.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 generation_models-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-03-05 21:35:15.260012 generation_models-0.7.0/generation_models/.gitignore
+-rw-r--r--   0        0        0       47 2024-03-05 21:35:15.260057 generation_models-0.7.0/generation_models/__init__.py
+-rw-r--r--   0        0        0   129503 2024-04-11 21:49:09.360899 generation_models-0.7.0/generation_models/generation_models.py
+-rw-r--r--   0        0        0      640 2024-04-11 22:19:34.604783 generation_models-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 generation_models-0.7.0/PKG-INFO
```

### Comparing `generation_models-0.6.0/generation_models/generation_models.py` & `generation_models-0.7.0/generation_models/generation_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1504,20 +1504,34 @@
             _check_lengths({"power": values["power"], "ambient_temp": values["ambient_temp"]})
         return values
 
     def __len__(self) -> int:
         return len(self.power)
 
 
+class BoundedSignal(BaseModel):
+    min: t.List[float]
+    actual: t.List[float]
+    max: t.List[float]
+
+    @root_validator(skip_on_failure=True)
+    def check_length(cls, values):
+        _check_lengths(values)
+        return values
+
+    def __len__(self):
+        return len(self.min)
+
+
 class ACProductionProfile(BaseModel):
     r"""Time series inputs associated with an MV AC generation source (e.g. PV MV output, wind turbines etc.). For use
     with :class:`ACExternalGenerationModel`
     """
 
-    power: t.List[float]
+    power: t.Union[t.List[float], BoundedSignal]
     r"""The power at the MV AC bus (i.e. where a MV BESS system would tie-in) 
 
     - In PVSyst, this field is EOutInv if inverter modeling takes into account MV transformer losses. If not,
       use E_Grid with all models downstream of the mv transformer turned off or set to zero
     - Units: kW
     """
     ambient_temp: t.Optional[t.List[float]]
@@ -2357,14 +2371,17 @@
     
     :meta private:
     """
     approximate_soe_impact_potential: bool = False
     r""":meta private:"""
     triangular: bool = True
     r""":meta private:"""
+    rtm_bp_tol: float = None
+    r"""The tolerance in kW within which the optimizer will keep the RTM base point despite solar uncertainty. This is 
+    only applicable when using uncertain solar."""
 
     @root_validator(skip_on_failure=True)
     def coerce_strategy_to_market_config(cls, values):
         assert not (values["dart"] is not None and values["energy_strategy"] is not None), (
             "Only one of `dart` or `energy_strategy` may be provided. `dart` is deprecated; use `energy_strategy`"
             " instead."
         )
```

### Comparing `generation_models-0.6.0/pyproject.toml` & `generation_models-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.6.0"
+version = "0.7.0"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
 packages = [{include = "generation_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
```

