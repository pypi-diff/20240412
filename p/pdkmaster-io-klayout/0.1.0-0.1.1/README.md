# Comparing `tmp/pdkmaster_io_klayout-0.1.0.tar.gz` & `tmp/pdkmaster_io_klayout-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdkmaster_io_klayout-0.1.0.tar", last modified: Wed Mar 27 18:12:10 2024, max compression
+gzip compressed data, was "pdkmaster_io_klayout-0.1.1.tar", last modified: Fri Apr 12 08:39:41 2024, max compression
```

## Comparing `pdkmaster_io_klayout-0.1.0.tar` & `pdkmaster_io_klayout-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      566 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.0/LICENSE.md
--rw-r--r--   0        0        0    34523 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.0/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    11358 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.0/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.0/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.0/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     2807 2024-03-27 18:04:59.962096 pdkmaster_io_klayout-0.1.0/README.md
--rw-r--r--   0        0        0      675 2024-03-27 18:12:10.267717 pdkmaster_io_klayout-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-03-26 08:41:13.656299 pdkmaster_io_klayout-0.1.0/test/__init__.py
--rw-r--r--   0        0        0      415 2024-03-26 09:34:50.831231 pdkmaster_io_klayout-0.1.0/test/cover_report.log
--rw-r--r--   0        0        0       98 2024-03-26 08:41:16.144261 pdkmaster_io_klayout-0.1.0/test/unit/__init__.py
--rw-r--r--   0        0        0    13555 2024-03-26 08:40:20.381103 pdkmaster_io_klayout-0.1.0/test/unit/dummy.py
--rw-r--r--   0        0        0       98 2024-03-26 08:42:02.583561 pdkmaster_io_klayout-0.1.0/test/unit/io/__init__.py
--rw-r--r--   0        0        0       98 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.0/test/unit/io/klayout/__init__.py
--rw-r--r--   0        0        0    13952 2024-03-26 09:34:45.931306 pdkmaster_io_klayout-0.1.0/test/unit/io/klayout/export.py
--rw-r--r--   0        0        0    20839 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.0/test/unit/io/klayout/merge.py
--rw-r--r--   0        0        0     3114 1970-01-01 00:00:00.000000 pdkmaster_io_klayout-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      566 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0    34523 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/agpl-3.0.txt
+-rw-r--r--   0        0        0    11358 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/apache-2.0.txt
+-rw-r--r--   0        0        0    13419 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/cern_ohl_s_v2.txt
+-rw-r--r--   0        0        0    18009 2024-03-25 12:52:27.794602 pdkmaster_io_klayout-0.1.1/LICENSES/gpl-2.0.txt
+-rw-r--r--   0        0        0     2914 2024-04-12 08:24:25.396742 pdkmaster_io_klayout-0.1.1/README.md
+-rw-r--r--   0        0        0      752 2024-04-12 08:39:41.499227 pdkmaster_io_klayout-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-03-26 08:41:13.656299 pdkmaster_io_klayout-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-12 08:19:15.877302 pdkmaster_io_klayout-0.1.1/test/cover_report.log
+-rw-r--r--   0        0        0       98 2024-03-26 08:41:16.144261 pdkmaster_io_klayout-0.1.1/test/unit/__init__.py
+-rw-r--r--   0        0        0    13633 2024-04-11 13:54:22.159579 pdkmaster_io_klayout-0.1.1/test/unit/dummy.py
+-rw-r--r--   0        0        0       98 2024-03-26 08:42:02.583561 pdkmaster_io_klayout-0.1.1/test/unit/io/__init__.py
+-rw-r--r--   0        0        0       98 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/__init__.py
+-rw-r--r--   0        0        0    14184 2024-04-11 13:54:22.159579 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/export.py
+-rw-r--r--   0        0        0    20839 2024-02-28 17:16:25.382380 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/merge.py
+-rw-r--r--   0        0        0     1576 2024-04-12 08:24:25.396742 pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/pcell.py
+-rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 pdkmaster_io_klayout-0.1.1/PKG-INFO
```

### Comparing `pdkmaster_io_klayout-0.1.0/LICENSE.md` & `pdkmaster_io_klayout-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/LICENSES/agpl-3.0.txt` & `pdkmaster_io_klayout-0.1.1/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/LICENSES/apache-2.0.txt` & `pdkmaster_io_klayout-0.1.1/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/LICENSES/cern_ohl_s_v2.txt` & `pdkmaster_io_klayout-0.1.1/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/LICENSES/gpl-2.0.txt` & `pdkmaster_io_klayout-0.1.1/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/README.md` & `pdkmaster_io_klayout-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 This is PDKMaster module to provide interoperation with klayout.
 This is WIP version with just the red tape setup for the project.
 
 ## Release history
 
+* v0.1.1: Some clean-up and implementation of klayout pcell library support for MOSFET and Via primitives.
 * v0.1.0: First version with split-off code from PDKMaster as is.
 
 # Contributing
 
 See [Contributing.md](Contributing.md)
 
 # Licensing Rationale
```

### Comparing `pdkmaster_io_klayout-0.1.0/pyproject.toml` & `pdkmaster_io_klayout-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 dynamic = []
 description = "KLayout interoperation for PDKMaster"
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
     "PDKMaster~=0.11.0",
+    "klayout>=0.27.13",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
+[tool.pdm.resolution.overrides]
+klayout = "0.27.13"
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "doit",
     "coverage[toml]",
```

### Comparing `pdkmaster_io_klayout-0.1.0/test/unit/dummy.py` & `pdkmaster_io_klayout-0.1.1/test/unit/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         pwell = _prm.Well(type_=_prm.pImpl, name="pwell", min_width=1.5, min_space=1.5)
         nplus = _prm.Implant(type_=_prm.nImpl, name="nplus", min_width=1.0, min_space=1.0)
         pplus = _prm.Implant(type_=_prm.pImpl, name="pplus", min_width=1.0, min_space=1.0)
         hvox = _prm.Insulator(name="hvox", min_width=0.5, min_space=0.5)
         active = _prm.WaferWire(
             name="active", min_width=0.3, min_space=0.2,
             allow_in_substrate=True,
-            implant=(nplus, pplus), min_implant_enclosure=_prp.Enclosure(0.2),
+            implant=(nplus, pplus), min_implant_enclosure=(
+                _prp.Enclosure(0.2), _prp.Enclosure((0.2, 0.25)),
+            ),
             implant_abut="none", allow_contactless_implant=False,
             well=(nwell, pwell), min_well_enclosure=_prp.Enclosure(1.0),
             min_substrate_enclosure=_prp.Enclosure(1.0),
             oxide=hvox, min_oxide_enclosure=_prp.Enclosure(0.2),
             allow_well_crossing=False,
         )
         poly = _prm.GateWire(name="poly", min_width=0.25, min_space=0.25)
@@ -71,15 +73,15 @@
             name="metal",
             min_width=0.1, min_space=0.1, space_table=((0.2, 0.5), ((1.0, 1.0), 1.0)),
             min_area=0.05, min_density=0.20,
             pin=metalpin,
         )
         contact = _prm.Via(
             name="contact", width=0.35, min_space=0.35, bottom=(active, poly), top=metal,
-            min_bottom_enclosure=_prp.Enclosure(0.2), min_top_enclosure=_prp.Enclosure(0.15),
+            min_bottom_enclosure=_prp.Enclosure((0.2, 0.25)), min_top_enclosure=_prp.Enclosure((0.20, 0.15)),
         )
         prims += (contact, metalpin, metal)
 
         mimtop = _prm.MIMTop(
             name="MIMTop", min_width=0.2, min_space=0.2,
         )
         prims += mimtop
```

### Comparing `pdkmaster_io_klayout-0.1.0/test/unit/io/klayout/export.py` & `pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,22 +353,28 @@
             _kl.export2db(msr1)
         kllay = _kl.export2db(msr1, gds_layers=dummy_gdslayers)
         self.assertIsInstance(kllay, pya.Layout)
         kllay = _kl.export2db(msr2, gds_layers=dummy_gdslayers)
         self.assertIsInstance(kllay, pya.Layout)
 
     def test_cells_library(self):
+        pya_lay = pya.Layout()
+        pya_cell = pya_lay.create_cell("test")
+
         # This mainly runs code to get coverage but does not extensive test of correctness
         # of results. This is assumed to be done with lower level unit tests.
         _kl.export2db(
             dummy_lib.cells.cell1, gds_layers=dummy_gdslayers, add_pin_label=True, merge=True,
+            pya_cell=pya_cell,
         )
 
-        with self.assertRaises(AssertionError):
+        with self.assertRaises(TypeError):
             _kl.export2db(dummy_lib, gds_layers=dummy_gdslayers, cell_name="test")
+        with self.assertRaises(TypeError):
+            _kl.export2db(dummy_lib, gds_layers=dummy_gdslayers, pya_cell=pya_cell)
         _kl.export2db(dummy_lib, gds_layers=dummy_gdslayers, add_pin_label=True, merge=True)
         _kl.export2db(
             dummy_lib, gds_layers=dummy_gdslayers, textgds_layers={},
             add_pin_label=True, merge=True,
         )
         _kl.export2db(
             dummy_lib, gds_layers=dummy_gdslayers, textgds_layers=dummy_textgdslayers,
```

### Comparing `pdkmaster_io_klayout-0.1.0/test/unit/io/klayout/merge.py` & `pdkmaster_io_klayout-0.1.1/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `pdkmaster_io_klayout-0.1.0/PKG-INFO` & `pdkmaster_io_klayout-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pdkmaster-io-klayout
-Version: 0.1.0
+Version: 0.1.1
 Summary: KLayout interoperation for PDKMaster
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster~=0.11.0
+Requires-Dist: klayout>=0.27.13
 Description-Content-Type: text/markdown
 
 This is PDKMaster module to provide interoperation with klayout.
 This is WIP version with just the red tape setup for the project.
 
 ## Release history
 
+* v0.1.1: Some clean-up and implementation of klayout pcell library support for MOSFET and Via primitives.
 * v0.1.0: First version with split-off code from PDKMaster as is.
 
 # Contributing
 
 See [Contributing.md](Contributing.md)
 
 # Licensing Rationale
```

