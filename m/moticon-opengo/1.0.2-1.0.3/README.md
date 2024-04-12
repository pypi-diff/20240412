# Comparing `tmp/moticon_opengo-1.0.2.tar.gz` & `tmp/moticon_opengo-1.0.3.tar.gz`

## Comparing `moticon_opengo-1.0.2.tar` & `moticon_opengo-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/examples/README.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/examples/demo_gait_report.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/examples/demo_txt_export_grf_curves.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/src/moticon_opengo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/src/moticon_opengo/__init__.py
--rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/src/moticon_opengo/gait_report.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/src/moticon_opengo/txt_export.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/src/moticon_opengo/utils.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/test_opengo.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/.gitignore
--rwxr-xr-x   0        0        0   579461 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/230927_102114.txt
--rwxr-xr-x   0        0        0   754746 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/230927_102137.txt
--rwxr-xr-x   0        0        0   330761 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/230927_102231.txt
--rw-r--r--   0        0        0   134552 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/gait_analysis.png
--rw-r--r--   0        0        0    58768 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_21_14.xlsx
--rw-r--r--   0        0        0    62016 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_21_37.xlsx
--rw-r--r--   0        0        0    43647 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_22_31.xlsx
--rw-r--r--   0        0        0   140759 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/tests/testdata/golden_gait_analysis.png
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/LICENSE
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/README.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 moticon_opengo-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/examples/README.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/examples/demo_gait_report.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/examples/demo_txt_export_events.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/examples/demo_txt_export_grf_curves.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/src/moticon_opengo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/src/moticon_opengo/__init__.py
+-rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/src/moticon_opengo/gait_report.py
+-rw-r--r--   0        0        0    17002 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/src/moticon_opengo/txt_export.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/src/moticon_opengo/utils.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/test_opengo.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/.gitignore
+-rwxr-xr-x   0        0        0   579461 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/230927_102114.txt
+-rwxr-xr-x   0        0        0   754746 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/230927_102137.txt
+-rwxr-xr-x   0        0        0   330761 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/230927_102231.txt
+-rw-r--r--   0        0        0   134552 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/gait_analysis.png
+-rw-r--r--   0        0        0    58768 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_21_14.xlsx
+-rw-r--r--   0        0        0    62016 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_21_37.xlsx
+-rw-r--r--   0        0        0    43647 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_22_31.xlsx
+-rw-r--r--   0        0        0   140759 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/golden_gait_analysis.png
+-rw-r--r--   0        0        0    55773 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/walk_data_with_events/golden_events.png
+-rw-r--r--   0        0        0   181407 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/tests/testdata/walk_data_with_events/text_export.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/README.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15982 2020-02-02 00:00:00.000000 moticon_opengo-1.0.3/PKG-INFO
```

### Comparing `moticon_opengo-1.0.2/.github/workflows/python-app.yml` & `moticon_opengo-1.0.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/examples/demo_txt_export_grf_curves.py` & `moticon_opengo-1.0.3/examples/demo_txt_export_grf_curves.py`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/src/moticon_opengo/gait_report.py` & `moticon_opengo-1.0.3/src/moticon_opengo/gait_report.py`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/src/moticon_opengo/utils.py` & `moticon_opengo-1.0.3/src/moticon_opengo/utils.py`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/test_opengo.py` & `moticon_opengo-1.0.3/tests/test_opengo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import unittest
 from datetime import datetime
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
-
-from moticon_opengo.txt_export import Measurement, TxtExportFileIterator
+from moticon_opengo.txt_export import Measurement, TxtExportEvent, TxtExportFileIterator
 
 # import filecmp
 
 dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class TestOpenGo(unittest.TestCase):
@@ -71,10 +70,29 @@
 
         self.assertTrue(os.path.exists(outfile))
         self.assertTrue(os.path.exists(golden_result))
 
         # filecmp did not work in github actions
         # self.assertTrue(filecmp.cmp(outfile, golden_result))
 
+    def test_import_event_data(self):
+        meas: Measurement = Measurement(
+            os.path.join(dir, "testdata", "walk_data_with_events", "text_export.txt")
+        )
+
+        self.assertIn("Left Events", meas.event_groups)
+        self.assertIn("Right Events", meas.event_groups)
+        self.assertEqual(len(meas.events), 16)
+        self.assertEqual(
+            meas.events[0],
+            TxtExportEvent(
+                event_name="Event",
+                group_name="Left Events",
+                index=20,
+                time=0.21,
+                value=1,
+            ),
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `moticon_opengo-1.0.2/tests/testdata/230927_102114.txt` & `moticon_opengo-1.0.3/tests/testdata/230927_102114.txt`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/230927_102137.txt` & `moticon_opengo-1.0.3/tests/testdata/230927_102137.txt`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/230927_102231.txt` & `moticon_opengo-1.0.3/tests/testdata/230927_102231.txt`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/gait_analysis.png` & `moticon_opengo-1.0.3/tests/testdata/gait_analysis.png`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_21_14.xlsx` & `moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_21_14.xlsx`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_21_37.xlsx` & `moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_21_37.xlsx`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/gait_report_230927_10_22_31.xlsx` & `moticon_opengo-1.0.3/tests/testdata/gait_report_230927_10_22_31.xlsx`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/tests/testdata/golden_gait_analysis.png` & `moticon_opengo-1.0.3/tests/testdata/golden_gait_analysis.png`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/.gitignore` & `moticon_opengo-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/LICENSE` & `moticon_opengo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/README.md` & `moticon_opengo-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 ### Text Export Data
 
 Assume we have a bunch of `.txt` files exported from a `.go` file using the
 OpenGo Software's text export. This library allows you to load and process
 these `.txt` files as demonstrated in the example
 `examples/demo_text_export_grf_curves.py`.
 
+If the measurement contains manually set events, then these events are also
+contained in the text export, and made available by the Python library. The
+example `examples/demo_text_export_events.py` shows how this can be used for
+convenient slicing of measurement data.
+
 ### Gait Report Data
 
 Assume we have a bunch of `.xlsx` files exported using the OpenGo Software's
 gait report. This library allows you to load and process these files as
 demonstrated in the example `examples/demo_gait_report.py`.
```

### Comparing `moticon_opengo-1.0.2/pyproject.toml` & `moticon_opengo-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moticon_opengo-1.0.2/PKG-INFO` & `moticon_opengo-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: moticon_opengo
-Version: 1.0.2
+Version: 1.0.3
 Summary: Moticon OpenGo Library
 Project-URL: Homepage, https://github.com/moticon-rego/moticon-opengo
 Project-URL: Bug Tracker, https://github.com/moticon-rego/moticon-opengo/issues
 Author-email: Moticon ReGo AG <support@moticon.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -253,14 +253,19 @@
 ### Text Export Data
 
 Assume we have a bunch of `.txt` files exported from a `.go` file using the
 OpenGo Software's text export. This library allows you to load and process
 these `.txt` files as demonstrated in the example
 `examples/demo_text_export_grf_curves.py`.
 
+If the measurement contains manually set events, then these events are also
+contained in the text export, and made available by the Python library. The
+example `examples/demo_text_export_events.py` shows how this can be used for
+convenient slicing of measurement data.
+
 ### Gait Report Data
 
 Assume we have a bunch of `.xlsx` files exported using the OpenGo Software's
 gait report. This library allows you to load and process these files as
 demonstrated in the example `examples/demo_gait_report.py`.
```

