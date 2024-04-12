# Comparing `tmp/od-metrics-1.0.1.tar.gz` & `tmp/od_metrics-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "od-metrics-1.0.1.tar", last modified: Wed Apr 10 22:05:53 2024, max compression
+gzip compressed data, was "od_metrics-1.0.2.tar", last modified: Fri Apr 12 21:44:52 2024, max compression
```

## Comparing `od-metrics-1.0.1.tar` & `od_metrics-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-10 22:05:42.000000 od-metrics-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5397 2024-04-10 22:05:53.452681 od-metrics-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4873 2024-04-10 22:05:42.000000 od-metrics-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-10 22:05:42.000000 od-metrics-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-10 22:05:53.452681 od-metrics-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-10 22:05:42.000000 od-metrics-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.448681 od-metrics-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.448681 od-metrics-1.0.1/src/od_metrics/
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/constants.py
--rw-r--r--   0 root         (0) root         (0)    46880 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/od_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/utils.py
--rw-r--r--   0 root         (0) root         (0)    23245 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/src/od_metrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      401 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)    12838 2024-04-10 22:05:42.000000 od-metrics-1.0.1/tests/test_odmetrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-12 21:44:42.000000 od_metrics-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5463 2024-04-12 21:44:52.742132 od_metrics-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4939 2024-04-12 21:44:42.000000 od_metrics-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-12 21:44:42.000000 od_metrics-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-12 21:44:52.742132 od_metrics-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-12 21:44:42.000000 od_metrics-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.738132 od_metrics-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.738132 od_metrics-1.0.2/src/od_metrics/
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/constants.py
+-rw-r--r--   0 root         (0) root         (0)    46882 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/od_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23245 2024-04-12 21:44:42.000000 od_metrics-1.0.2/src/od_metrics/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/src/od_metrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5463 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 21:44:52.000000 od_metrics-1.0.2/src/od_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:44:52.742132 od_metrics-1.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)    12838 2024-04-12 21:44:42.000000 od_metrics-1.0.2/tests/test_odmetrics.py
```

### Comparing `od-metrics-1.0.1/LICENSE` & `od_metrics-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.1/PKG-INFO` & `od_metrics-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 1.0.1
+Version: 1.0.2
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,17 +22,18 @@
   <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
-  <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
   <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
     <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <a href="https://pypi.org/project/od-metrics/#description">
+    <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1"></a>
   <br>
   <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
   <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
     <img src="https://mybinder.org/badge_logo.svg"></a>
   <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.1 Summary: Object Detection
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.2 Summary: Object Detection
 metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
                             images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
-  img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
-    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+_c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]_[_h_t_t_p_s_:_/_/
+  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_E_M_a_l_a_g_o_l_i_9_2_/
+        _3_3_1_3_9_5_9_6_0_7_2_5_a_4_b_4_7_d_4_c_a_4_9_7_7_a_2_4_e_9_4_9_/_r_a_w_/_v_e_r_s_i_o_n_._j_s_o_n_?_k_i_l_l___c_a_c_h_e_=_1_]
  [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
                                      _M_I_T_]
       _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
       _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
                 AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
 ## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
 **Highly Customizable**: every parameters that occur in the definition of `mAP`
```

### Comparing `od-metrics-1.0.1/README.md` & `od_metrics-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
   <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
-  <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
   <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
     <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <a href="https://pypi.org/project/od-metrics/#description">
+    <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1"></a>
   <br>
   <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
   <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
     <img src="https://mybinder.org/badge_logo.svg"></a>
   <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
                             images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
-  img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
-    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+_c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]_[_h_t_t_p_s_:_/_/
+  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_E_M_a_l_a_g_o_l_i_9_2_/
+        _3_3_1_3_9_5_9_6_0_7_2_5_a_4_b_4_7_d_4_c_a_4_9_7_7_a_2_4_e_9_4_9_/_r_a_w_/_v_e_r_s_i_o_n_._j_s_o_n_?_k_i_l_l___c_a_c_h_e_=_1_]
  [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
                                      _M_I_T_]
       _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
       _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
                 AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
 ## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
 **Highly Customizable**: every parameters that occur in the definition of `mAP`
```

### Comparing `od-metrics-1.0.1/setup.cfg` & `od_metrics-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = od-metrics
-version = 1.0.1
+version = 1.0.2
 author = EMalagoli92
 author_email = emala.892@gmail.com
 description = Object Detection metrics.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EMalagoli92/OD-metrics
 classifiers =
```

### Comparing `od-metrics-1.0.1/src/od_metrics/constants.py` & `od_metrics-1.0.2/src/od_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.1/src/od_metrics/od_metrics.py` & `od_metrics-1.0.2/src/od_metrics/od_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             The default is `False`.
         box_format: Literal["xyxy", "xywh", "cxcywh"], optional
             Bounding box format.
             Supported formats are:<br>
                 - `"xyxy"`: boxes are represented via corners,
                         x1, y1 being top left and x2, y2
                         being bottom right.<br>
-                - `xywh`: boxes are represented via corner,
+                - `"xywh"`: boxes are represented via corner,
                         width and height, x1, y2 being top
                         left, w, h being width and height.
                         This is the default format; all
                         input formats will be converted
                         to this.<br>
                 - `"cxcywh"`: boxes are represented via centre,
                         width and height, cx, cy being
```

### Comparing `od-metrics-1.0.1/src/od_metrics/utils.py` & `od_metrics-1.0.2/src/od_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.1/src/od_metrics/validators.py` & `od_metrics-1.0.2/src/od_metrics/validators.py`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.1/src/od_metrics.egg-info/PKG-INFO` & `od_metrics-1.0.2/src/od_metrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 1.0.1
+Version: 1.0.2
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,17 +22,18 @@
   <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
-  <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
   <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
     <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <a href="https://pypi.org/project/od-metrics/#description">
+    <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1"></a>
   <br>
   <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
   <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
     <img src="https://mybinder.org/badge_logo.svg"></a>
   <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.1 Summary: Object Detection
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.2 Summary: Object Detection
 metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
                             images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
-  img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
-   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
-    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+    3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+_c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]_[_h_t_t_p_s_:_/_/
+  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_E_M_a_l_a_g_o_l_i_9_2_/
+        _3_3_1_3_9_5_9_6_0_7_2_5_a_4_b_4_7_d_4_c_a_4_9_7_7_a_2_4_e_9_4_9_/_r_a_w_/_v_e_r_s_i_o_n_._j_s_o_n_?_k_i_l_l___c_a_c_h_e_=_1_]
  [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
                                      _M_I_T_]
       _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
       _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
                 AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
 ## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
 **Highly Customizable**: every parameters that occur in the definition of `mAP`
```

### Comparing `od-metrics-1.0.1/tests/test_odmetrics.py` & `od_metrics-1.0.2/tests/test_odmetrics.py`

 * *Files identical despite different names*

