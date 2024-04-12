# Comparing `tmp/woffl-1.0.0.tar.gz` & `tmp/woffl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woffl-1.0.0.tar", last modified: Fri Apr 12 01:31:10 2024, max compression
+gzip compressed data, was "woffl-1.0.1.tar", last modified: Fri Apr 12 16:37:57 2024, max compression
```

## Comparing `woffl-1.0.0.tar` & `woffl-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.882084 woffl-1.0.0/
--rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3650 2024-04-12 01:31:10.879844 woffl-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.0/README.md
--rw-rw-rw-   0        0        0      910 2024-04-12 01:30:53.000000 woffl-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 01:31:10.882084 woffl-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.185497 woffl-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.0/tests/boil_test.py
--rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.0/tests/e41_test.py
--rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.0/tests/fgas_test.py
--rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.0/tests/flow_test.py
--rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.0/tests/jpump_test.py
--rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.0/tests/outflow_test.py
--rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.0/tests/pvt_test.py
--rw-rw-rw-   0        0        0     2375 2024-04-12 01:09:24.000000 woffl-1.0.0/tests/rmix_test.py
--rw-rw-rw-   0        0        0      358 2024-04-11 21:40:46.000000 woffl-1.0.0/tests/wprof_test.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.187427 woffl-1.0.0/woffl/
--rw-rw-rw-   0        0        0      412 2024-04-10 23:51:51.000000 woffl-1.0.0/woffl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.780760 woffl-1.0.0/woffl/assembly/
--rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.0/woffl/assembly/__init__.py
--rw-rw-rw-   0        0        0     2313 2024-04-11 21:31:27.000000 woffl-1.0.0/woffl/assembly/batchrun.py
--rw-rw-rw-   0        0        0     3780 2024-04-11 23:53:38.000000 woffl-1.0.0/woffl/assembly/easypump.py
--rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.0/woffl/assembly/sysops.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.842714 woffl-1.0.0/woffl/flow/
--rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.0/woffl/flow/__init__.py
--rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.0/woffl/flow/annflow.py
--rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.0/woffl/flow/inflow.py
--rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.0/woffl/flow/jetcheck.py
--rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.0/woffl/flow/jetflow.py
--rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.0/woffl/flow/jetplot.py
--rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.0/woffl/flow/outflow.py
--rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.0/woffl/flow/singlephase.py
--rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.0/woffl/flow/twophase.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.858180 woffl-1.0.0/woffl/geometry/
--rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.0/woffl/geometry/__init__.py
--rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.0/woffl/geometry/forms.py
--rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.0/woffl/geometry/jetpump.py
--rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.0/woffl/geometry/pipe.py
--rw-rw-rw-   0        0        0    26700 2024-03-19 20:18:56.000000 woffl-1.0.0/woffl/geometry/wellprofile.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.875140 woffl-1.0.0/woffl/pvt/
--rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.0/woffl/pvt/__init__.py
--rw-rw-rw-   0        0        0    23108 2024-04-10 22:58:23.000000 woffl-1.0.0/woffl/pvt/blackoil.py
--rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.0/woffl/pvt/deadoil.py
--rw-rw-rw-   0        0        0    13519 2024-04-11 21:35:54.000000 woffl-1.0.0/woffl/pvt/formgas.py
--rw-rw-rw-   0        0        0     3997 2024-04-11 22:33:24.000000 woffl-1.0.0/woffl/pvt/formwat.py
--rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.0/woffl/pvt/resmix.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:31:10.877845 woffl-1.0.0/woffl.egg-info/
--rw-rw-rw-   0        0        0     3650 2024-04-12 01:31:09.000000 woffl-1.0.0/woffl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2024-04-12 01:31:09.000000 woffl-1.0.0/woffl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 01:31:09.000000 woffl-1.0.0/woffl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-12 01:31:09.000000 woffl-1.0.0/woffl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-12 01:31:09.000000 woffl-1.0.0/woffl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.894872 woffl-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4028 2024-04-12 16:37:57.893322 woffl-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-12 16:36:35.000000 woffl-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:37:57.895899 woffl-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.745834 woffl-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.1/tests/boil_test.py
+-rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.1/tests/e41_test.py
+-rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.1/tests/fgas_test.py
+-rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.1/tests/flow_test.py
+-rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.1/tests/jpump_test.py
+-rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.1/tests/outflow_test.py
+-rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.1/tests/pvt_test.py
+-rw-rw-rw-   0        0        0     2375 2024-04-12 01:33:15.000000 woffl-1.0.1/tests/rmix_test.py
+-rw-rw-rw-   0        0        0      358 2024-04-11 21:40:46.000000 woffl-1.0.1/tests/wprof_test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.748254 woffl-1.0.1/woffl/
+-rw-rw-rw-   0        0        0       56 2024-04-12 16:35:28.000000 woffl-1.0.1/woffl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.776790 woffl-1.0.1/woffl/assembly/
+-rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.1/woffl/assembly/__init__.py
+-rw-rw-rw-   0        0        0     2313 2024-04-11 21:31:27.000000 woffl-1.0.1/woffl/assembly/batchrun.py
+-rw-rw-rw-   0        0        0     3756 2024-04-12 15:24:00.000000 woffl-1.0.1/woffl/assembly/easypump.py
+-rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.1/woffl/assembly/sysops.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.802540 woffl-1.0.1/woffl/flow/
+-rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.1/woffl/flow/__init__.py
+-rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.1/woffl/flow/annflow.py
+-rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.1/woffl/flow/inflow.py
+-rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.1/woffl/flow/jetcheck.py
+-rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.1/woffl/flow/jetflow.py
+-rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.1/woffl/flow/jetplot.py
+-rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.1/woffl/flow/outflow.py
+-rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.1/woffl/flow/singlephase.py
+-rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.1/woffl/flow/twophase.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.839105 woffl-1.0.1/woffl/geometry/
+-rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.1/woffl/geometry/__init__.py
+-rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.1/woffl/geometry/forms.py
+-rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.1/woffl/geometry/jetpump.py
+-rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.1/woffl/geometry/pipe.py
+-rw-rw-rw-   0        0        0    26650 2024-04-12 15:30:05.000000 woffl-1.0.1/woffl/geometry/wellprofile.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.877387 woffl-1.0.1/woffl/pvt/
+-rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.1/woffl/pvt/__init__.py
+-rw-rw-rw-   0        0        0    23100 2024-04-12 16:12:06.000000 woffl-1.0.1/woffl/pvt/blackoil.py
+-rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.1/woffl/pvt/deadoil.py
+-rw-rw-rw-   0        0        0    13803 2024-04-12 15:28:33.000000 woffl-1.0.1/woffl/pvt/formgas.py
+-rw-rw-rw-   0        0        0     4192 2024-04-12 15:27:26.000000 woffl-1.0.1/woffl/pvt/formwat.py
+-rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.1/woffl/pvt/resmix.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:37:57.890380 woffl-1.0.1/woffl.egg-info/
+-rw-rw-rw-   0        0        0     4028 2024-04-12 16:37:57.000000 woffl-1.0.1/woffl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2024-04-12 16:37:57.000000 woffl-1.0.1/woffl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:37:57.000000 woffl-1.0.1/woffl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-12 16:37:57.000000 woffl-1.0.1/woffl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-12 16:37:57.000000 woffl-1.0.1/woffl.egg-info/top_level.txt
```

### Comparing `woffl-1.0.0/LICENSE` & `woffl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/PKG-INFO` & `woffl-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.0
+Version: 1.0.1
+Summary: Numerically solve jet pump equations in multiphase oil wells
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,24 +21,31 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kwellis/woffl
-Keywords: jet pump,solver,numerical
+Keywords: jet pump,solver,numerical,multiphase
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scipy>=1.11.4
+Provides-Extra: dev
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: black; extra == "dev"
 
 ![woffl_github7](https://github.com/kwellis/woffl/assets/62774251/8b80146f-a503-4576-8f43-f1aa45d93a05)
 Numerical solver for liquid jet pumps with three-phase flow.   
 #### Background
 Jet pump studies fron the 1970's were interested in pumping single phase incompressible flows or single phase compressible flows. The models produced relied on assumptions such as constant density or an ideal gas to analytically solve the equations. In 1995 Cunningham wrote a paper with equations that govern a water jet for pumping a two-phase mixture. The equations relied on assumptions of constant density for the liquid and ideal gas law for the solution. Those assumptions are not valid when modeling a three-phase mixture of crude oil, water and natural gas. The crude oil is gas soluble and compressible. The equations for the inverse density of crude oil cannot be analytically integrated. A numerical solution needs to be applied.   
 #### Fundamental Equation
 The fundamental equation in the analysis of a jet pump is the un-integrated energy equation. No work is done, heat is not transferred and a significant height difference is not present. The un-integrated energy equation takes the following form.
```

### Comparing `woffl-1.0.0/README.md` & `woffl-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/boil_test.py` & `woffl-1.0.1/tests/boil_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/e41_test.py` & `woffl-1.0.1/tests/e41_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/fgas_test.py` & `woffl-1.0.1/tests/fgas_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/flow_test.py` & `woffl-1.0.1/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/jpump_test.py` & `woffl-1.0.1/tests/jpump_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/outflow_test.py` & `woffl-1.0.1/tests/outflow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/pvt_test.py` & `woffl-1.0.1/tests/pvt_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/tests/rmix_test.py` & `woffl-1.0.1/tests/rmix_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/assembly/batchrun.py` & `woffl-1.0.1/woffl/assembly/batchrun.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/assembly/easypump.py` & `woffl-1.0.1/woffl/assembly/easypump.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,24 +61,24 @@
         qnz_bwpd (float): Power Fluid Rate, BWPD
         mach_te(float): Mach Number Throat Entry, unitless
         total_wc (float): Total Water Cut (PF + Form), fraction
         total_water (float): Total Water Rate (PF + Form), BWPD
         wellname (str): Wellname
     """
     if is_sch:
-        mpu_oil = BlackOil.schrader_oil()  # class method
-        mpu_wat = FormWater.schrader_wat()  # class method
-        mpu_gas = FormGas.schrader_gas()  # class method
+        mpu_oil = BlackOil.schrader()  # class method
+        mpu_wat = FormWater.schrader()  # class method
+        mpu_gas = FormGas.schrader()  # class method
 
         wellprof = WellProfile.schrader()
 
     else:
-        mpu_oil = BlackOil.kuparuk_oil()  # class method
-        mpu_wat = FormWater.kuparuk_wat()  # class method
-        mpu_gas = FormGas.kuparuk_gas()  # class method
+        mpu_oil = BlackOil.kuparuk()  # class method
+        mpu_wat = FormWater.kuparuk()  # class method
+        mpu_gas = FormGas.kuparuk()  # class method
 
         wellprof = WellProfile.kuparuk()
 
     tube = Pipe(out_dia, thick)
 
     ipr_su = InFlow(qwf, pwf, res_pres)
```

### Comparing `woffl-1.0.0/woffl/assembly/sysops.py` & `woffl-1.0.1/woffl/assembly/sysops.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/annflow.py` & `woffl-1.0.1/woffl/flow/annflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/inflow.py` & `woffl-1.0.1/woffl/flow/inflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/jetcheck.py` & `woffl-1.0.1/woffl/flow/jetcheck.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/jetflow.py` & `woffl-1.0.1/woffl/flow/jetflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/jetplot.py` & `woffl-1.0.1/woffl/flow/jetplot.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/outflow.py` & `woffl-1.0.1/woffl/flow/outflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/singlephase.py` & `woffl-1.0.1/woffl/flow/singlephase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/flow/twophase.py` & `woffl-1.0.1/woffl/flow/twophase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/geometry/forms.py` & `woffl-1.0.1/woffl/geometry/forms.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/geometry/jetpump.py` & `woffl-1.0.1/woffl/geometry/jetpump.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/geometry/pipe.py` & `woffl-1.0.1/woffl/geometry/pipe.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/geometry/wellprofile.py` & `woffl-1.0.1/woffl/geometry/wellprofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                 text=f"{int(md_ray[idx])} ft.", xy=(hd_ray[idx] + 5, vd_ray[idx] - 10), rotation=30  # type: ignore
             )
         plt.axis("equal")
         plt.show()
 
     @classmethod
     def schrader(cls):
-        """Schrader Bluff Well Profile generic geometry based on MPE-42
+        """Schrader Bluff Generic Well Profile
 
         Generic Schrader Bluff well profile based on MPE-42 geometry.
 
         Args:
             md_list (list): MPE-42 Measured Depth
             vd_list (list): MPE-42 Vertical Depth
             jetpump_md (float): 6693 MD, feet
@@ -622,15 +622,15 @@
             4197.74213,
             4193.97265,
         ]
         return cls(md_list=e42_md, vd_list=e42_vd, jetpump_md=6693)
 
     @classmethod
     def kuparuk(cls):
-        """Kuparuk Well Profile generic geometry based on MPC-42
+        """Kuparuk Generic Well Profile
 
         Generic Kuparuk well profile based on MPC-23 geometry.
         MPC-23 is a slant Kuparuk Well, so not a perfect canidate.
 
         Args:
             md_list (list): MPC-23 Measured Depth
             vd_list (list): MPC-23 Vertical Depth
```

### Comparing `woffl-1.0.0/woffl/pvt/blackoil.py` & `woffl-1.0.1/woffl/pvt/blackoil.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,28 +37,28 @@
         self.pbp = bubblepoint
         self.gas_sg = gas_sg
 
     def __repr__(self):
         return f"Oil: {self.oil_api} API and a {round(self.gas_sg, 2)} SG Gas"
 
     @classmethod
-    def schrader_oil(cls):
+    def schrader(cls):
         """Schrader Bluff Black Oil
 
         Generic Schrader Bluff black oil with preset properties
 
         Args:
             oil_api (float): 22 API
             bubblepoint (float): 1750 psig
             gas_sg (float): 0.65
         """
         return cls(oil_api=22, bubblepoint=1750, gas_sg=0.65)
 
     @classmethod
-    def kuparuk_oil(cls):
+    def kuparuk(cls):
         """Kuparuk Black Oil
 
         Generic Kuparuk black oil with preset properties
 
         Args:
             oil_api (float): 24 API
             bubblepoint (float): 2250 psig
```

### Comparing `woffl-1.0.0/woffl/pvt/deadoil.py` & `woffl-1.0.1/woffl/pvt/deadoil.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl/pvt/formgas.py` & `woffl-1.0.1/woffl/pvt/formgas.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,35 @@
         self.ppc, self.tpc = self._sutton_pseudo_crit(gas_sg)
         self.mw = 28.96443 * gas_sg  # molecular weight
 
     def __repr__(self):
         return f"Gas: {self.gas_sg} SG and {self.mw} Mol Weight"
 
     @classmethod
-    def schrader_gas(cls):
+    def schrader(cls):
+        """Schrader Bluff Generic Formation Gas
+
+        Args:
+            gas_sg (float): 0.65"""
         return cls(gas_sg=0.65)
 
     @classmethod
-    def kuparuk_gas(cls):
+    def kuparuk(cls):
+        """Kuparuk Generic Formation Gas
+
+        Args:
+            gas_sg (float): 0.65"""
         return cls(gas_sg=0.65)
 
     @classmethod
     def methane_gas(cls):
+        """Pure Methane Formation Gas
+
+        Args:
+            gas_sg (float): 0.65"""
         return cls(gas_sg=0.55)
 
     # almost need seperate function to change pressure / temperature
     def condition(self, press, temp):
         """Set condition of evaluation
 
         Args:
```

### Comparing `woffl-1.0.0/woffl/pvt/formwat.py` & `woffl-1.0.1/woffl/pvt/formwat.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,27 @@
 
         self.wat_sg = wat_sg
 
     def __repr__(self) -> str:
         return f"Water {self.wat_sg} Specific Gravity"
 
     @classmethod
-    def schrader_wat(cls):
+    def schrader(cls):
+        """Schrader Bluff Generic Formation Water
+
+        Args:
+            wat_sg (float): 1.02"""
         return cls(wat_sg=1.02)
 
     @classmethod
-    def kuparuk_wat(cls):
+    def kuparuk(cls):
+        """Kuparuk Generic Formation Water
+
+        Args:
+            wat_sg (float): 1.02"""
         return cls(wat_sg=1.02)
 
     def condition(self, press: float, temp: float):
         """Set condition of evaluation
 
         Args:
             press (float): Pressure of the water, psig
```

### Comparing `woffl-1.0.0/woffl/pvt/resmix.py` & `woffl-1.0.1/woffl/pvt/resmix.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.0/woffl.egg-info/PKG-INFO` & `woffl-1.0.1/woffl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.0
+Version: 1.0.1
+Summary: Numerically solve jet pump equations in multiphase oil wells
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,24 +21,31 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kwellis/woffl
-Keywords: jet pump,solver,numerical
+Keywords: jet pump,solver,numerical,multiphase
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scipy>=1.11.4
+Provides-Extra: dev
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: black; extra == "dev"
 
 ![woffl_github7](https://github.com/kwellis/woffl/assets/62774251/8b80146f-a503-4576-8f43-f1aa45d93a05)
 Numerical solver for liquid jet pumps with three-phase flow.   
 #### Background
 Jet pump studies fron the 1970's were interested in pumping single phase incompressible flows or single phase compressible flows. The models produced relied on assumptions such as constant density or an ideal gas to analytically solve the equations. In 1995 Cunningham wrote a paper with equations that govern a water jet for pumping a two-phase mixture. The equations relied on assumptions of constant density for the liquid and ideal gas law for the solution. Those assumptions are not valid when modeling a three-phase mixture of crude oil, water and natural gas. The crude oil is gas soluble and compressible. The equations for the inverse density of crude oil cannot be analytically integrated. A numerical solution needs to be applied.   
 #### Fundamental Equation
 The fundamental equation in the analysis of a jet pump is the un-integrated energy equation. No work is done, heat is not transferred and a significant height difference is not present. The un-integrated energy equation takes the following form.
```

### Comparing `woffl-1.0.0/woffl.egg-info/SOURCES.txt` & `woffl-1.0.1/woffl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

