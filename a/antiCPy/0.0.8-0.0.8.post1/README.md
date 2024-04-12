# Comparing `tmp/antiCPy-0.0.8.tar.gz` & `tmp/antiCPy-0.0.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antiCPy-0.0.8.tar", last modified: Sat Jan 20 13:28:40 2024, max compression
+gzip compressed data, was "antiCPy-0.0.8.post1.tar", last modified: Fri Apr 12 06:45:16 2024, max compression
```

## Comparing `antiCPy-0.0.8.tar` & `antiCPy-0.0.8.post1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.464937 antiCPy-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-20 13:27:24.000000 antiCPy-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-01-20 13:28:40.464937 antiCPy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-20 13:27:24.000000 antiCPy-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.460937 antiCPy-0.0.8/antiCPy/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.460937 antiCPy-0.0.8/antiCPy/early_warnings/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.460937 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/param_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.464937 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/binning_langevin_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    89275 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/langevin_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)   107039 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/non_markov_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    33928 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/rocket_fast_resilience_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/summary_statistics_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.464937 antiCPy-0.0.8/antiCPy/trend_extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/trend_extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.464937 antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_configs_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_configs_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_configs_helper/create_configs_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_cp_segment_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    36417 2024-01-20 13:27:24.000000 antiCPy-0.0.8/antiCPy/trend_extrapolation/cp_segment_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 13:28:40.464937 antiCPy-0.0.8/antiCPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-01-20 13:28:40.000000 antiCPy-0.0.8/antiCPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-20 13:28:40.000000 antiCPy-0.0.8/antiCPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 13:28:40.000000 antiCPy-0.0.8/antiCPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-20 13:28:40.000000 antiCPy-0.0.8/antiCPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-20 13:28:40.000000 antiCPy-0.0.8/antiCPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 13:28:40.464937 antiCPy-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-20 13:27:24.000000 antiCPy-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.168744 antiCPy-0.0.8.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-12 06:45:16.168744 antiCPy-0.0.8.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.160745 antiCPy-0.0.8.post1/antiCPy/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.164744 antiCPy-0.0.8.post1/antiCPy/early_warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.164744 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/param_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.164744 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/binning_langevin_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89069 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/langevin_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107040 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/non_markov_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34632 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/rocket_fast_resilience_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/summary_statistics_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.164744 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.168744 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_configs_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_configs_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_configs_helper/create_configs_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_cp_segment_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36417 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/cp_segment_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:45:16.168744 antiCPy-0.0.8.post1/antiCPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-12 06:45:16.000000 antiCPy-0.0.8.post1/antiCPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 06:45:16.000000 antiCPy-0.0.8.post1/antiCPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:45:16.000000 antiCPy-0.0.8.post1/antiCPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 06:45:16.000000 antiCPy-0.0.8.post1/antiCPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 06:45:16.000000 antiCPy-0.0.8.post1/antiCPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:45:16.168744 antiCPy-0.0.8.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-12 06:43:51.000000 antiCPy-0.0.8.post1/setup.py
```

### Comparing `antiCPy-0.0.8/LICENSE` & `antiCPy-0.0.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/PKG-INFO` & `antiCPy-0.0.8.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antiCPy
-Version: 0.0.8
+Version: 0.0.8.post1
 Summary: A package that provides tools to estimate resilience and noise level of a system as well as extrapolate possible transition times.
 Home-page: https://github.com/MartinHessler/antiCPy
 Author: Martin Heßler
 Author-email: m_hess23@wwu.de
 License: GPL
 Keywords: time series analysis,critical transitions,leading indicators
 Platform: any
```

### Comparing `antiCPy-0.0.8/README.md` & `antiCPy-0.0.8.post1/README.md`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/__init__.py` & `antiCPy-0.0.8.post1/antiCPy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 if sys.version_info < (3, 6, 0):
     import warnings
 
     warnings.warn(
         'The installed Python version reached its end-of-life. Please upgrade to a newer Python version for receiving '
         'further antiCPy updates.', Warning)
 
-__version__ = '0.0.8'
+__version__ = '0.0.8.post1'
 
 __author__ = 'Martin Heßler'
```

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/analysis.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/analysis.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/graphics.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/graphics.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/param_opt.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/param_opt.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/dominant_eigenvalue/tutorial.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/dominant_eigenvalue/tutorial.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/binning_langevin_estimation.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/binning_langevin_estimation.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/langevin_estimation.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/langevin_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2169,18 +2169,18 @@
 00008780: 6c6f 7065 5f49 492c 2043 425f 6e6f 6973  lope_II, CB_nois
 00008790: 655f 492c 2043 425f 6e6f 6973 655f 4949  e_I, CB_noise_II
 000087a0: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
 000087b0: 6e64 6f77 5f73 6869 6674 203d 2069 0a20  ndow_shift = i. 
 000087c0: 2020 2020 2020 2073 656c 662e 6361 6c63         self.calc
 000087d0: 5f64 7269 6674 736c 6f70 655f 6e6f 6973  _driftslope_nois
 000087e0: 6528 736c 6f70 655f 6772 6964 2c20 6e6f  e(slope_grid, no
-000087f0: 6973 655f 6772 6964 2c20 6e5f 6a6f 696e  ise_grid, n_join
-00008800: 745f 7361 6d70 6c65 732c 206e 5f73 6c6f  t_samples, n_slo
-00008810: 7065 5f73 616d 706c 6573 2c20 6e62 7572  pe_samples, nbur
-00008820: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+000087f0: 6973 655f 6772 6964 2c20 6e62 7572 6e2c  ise_grid, nburn,
+00008800: 206e 5f6a 6f69 6e74 5f73 616d 706c 6573   n_joint_samples
+00008810: 2c20 6e5f 736c 6f70 655f 7361 6d70 6c65  , n_slope_sample
+00008820: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
 00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008840: 2020 2020 2020 6e5f 6e6f 6973 655f 7361        n_noise_sa
 00008850: 6d70 6c65 732c 2063 7265 645f 7065 7263  mples, cred_perc
 00008860: 656e 7469 6c65 732c 2070 7269 6e74 5f41  entiles, print_A
 00008870: 435f 7461 752c 2069 676e 6f72 655f 4143  C_tau, ignore_AC
 00008880: 5f65 7272 6f72 2c20 7468 696e 6e69 6e67  _error, thinning
 00008890: 5f62 792c 0a20 2020 2020 2020 2020 2020  _by,.           
@@ -2485,1708 +2485,1708 @@
 00009b40: 6e6e 696e 6720 6f66 2074 6865 204d 6172  nning of the Mar
 00009b50: 6b6f 7620 6368 6169 6e73 2077 6869 6368  kov chains which
 00009b60: 2061 7265 2064 6973 6361 7264 6564 2069   are discarded i
 00009b70: 6e20 7465 726d 7320 6f66 0a20 2020 2020  n terms of.     
 00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009b90: 2020 2061 2062 7572 6e20 696e 2070 6572     a burn in per
 00009ba0: 696f 642e 2055 7375 616c 6c79 2074 6865  iod. Usually the
-00009bb0: 2064 6566 6175 6c20 6973 2032 3030 2c20   defaul is 200, 
-00009bc0: 7365 7420 6279 2074 6865 2060 7065 7266  set by the `perf
-00009bd0: 6f72 6d5f 7265 7369 6c69 656e 6365 5f73  orm_resilience_s
-00009be0: 6361 6e60 206d 6574 686f 642e 0a20 2020  can` method..   
-00009bf0: 2020 2020 203a 7479 7065 206e 6275 726e       :type nburn
-00009c00: 3a20 696e 740a 2020 2020 2020 2020 3a70  : int.        :p
-00009c10: 6172 616d 206e 5f6a 6f69 6e74 5f73 616d  aram n_joint_sam
-00009c20: 706c 6573 3a20 4e75 6d62 6572 206f 6620  ples: Number of 
-00009c30: 6a6f 696e 7420 7361 6d70 6c65 7320 7468  joint samples th
-00009c40: 6174 2061 7265 2064 7261 776e 2066 726f  at are drawn fro
-00009c50: 6d20 7468 6520 6573 7469 6d61 7465 6420  m the estimated 
-00009c60: 6a6f 696e 7420 706f 7374 6572 696f 720a  joint posterior.
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 2020 2020 2020 7072 6f62 6162 696c          probabil
-00009c90: 6974 7920 696e 206f 7264 6572 2074 6f20  ity in order to 
-00009ca0: 6361 6c63 756c 6174 6520 7468 6520 6472  calculate the dr
-00009cb0: 6966 7420 736c 6f70 6520 6573 7469 6d61  ift slope estima
-00009cc0: 7465 203a 6d61 7468 3a60 5c7a 6574 6160  te :math:`\zeta`
-00009cd0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00009ce0: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
-00009cf0: 7265 7370 6f6e 6469 6e67 2063 7265 6469  responding credi
-00009d00: 6269 6c69 7479 2062 616e 6473 2e20 4465  bility bands. De
-00009d10: 6661 756c 7420 6973 2035 3030 3030 2e0a  fault is 50000..
-00009d20: 2020 2020 2020 2020 3a74 7970 6520 6e5f          :type n_
-00009d30: 6a6f 696e 745f 7361 6d70 6c65 733a 2069  joint_samples: i
-00009d40: 6e74 0a20 2020 2020 2020 203a 7061 7261  nt.        :para
-00009d50: 6d20 6e5f 736c 6f70 655f 7361 6d70 6c65  m n_slope_sample
-00009d60: 733a 204e 756d 6265 7220 6f66 2064 7269  s: Number of dri
-00009d70: 6674 2073 6c6f 7065 2073 616d 706c 6573  ft slope samples
-00009d80: 2074 6861 7420 6172 6520 6472 6177 6e20   that are drawn 
-00009d90: 6672 6f6d 2074 6865 2065 7374 696d 6174  from the estimat
-00009da0: 6564 2064 7269 6674 2073 6c6f 7065 0a20  ed drift slope. 
+00009bb0: 2064 6566 6175 6c74 2069 7320 3230 302c   default is 200,
+00009bc0: 2073 6574 2062 7920 7468 6520 6070 6572   set by the `per
+00009bd0: 666f 726d 5f72 6573 696c 6965 6e63 655f  form_resilience_
+00009be0: 7363 616e 6020 6d65 7468 6f64 2e0a 2020  scan` method..  
+00009bf0: 2020 2020 2020 3a74 7970 6520 6e62 7572        :type nbur
+00009c00: 6e3a 2069 6e74 0a20 2020 2020 2020 203a  n: int.        :
+00009c10: 7061 7261 6d20 6e5f 6a6f 696e 745f 7361  param n_joint_sa
+00009c20: 6d70 6c65 733a 204e 756d 6265 7220 6f66  mples: Number of
+00009c30: 206a 6f69 6e74 2073 616d 706c 6573 2074   joint samples t
+00009c40: 6861 7420 6172 6520 6472 6177 6e20 6672  hat are drawn fr
+00009c50: 6f6d 2074 6865 2065 7374 696d 6174 6564  om the estimated
+00009c60: 206a 6f69 6e74 2070 6f73 7465 7269 6f72   joint posterior
+00009c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c80: 2020 2020 2020 2020 2070 726f 6261 6269           probabi
+00009c90: 6c69 7479 2069 6e20 6f72 6465 7220 746f  lity in order to
+00009ca0: 2063 616c 6375 6c61 7465 2074 6865 2064   calculate the d
+00009cb0: 7269 6674 2073 6c6f 7065 2065 7374 696d  rift slope estim
+00009cc0: 6174 6520 3a6d 6174 683a 605c 7a65 7461  ate :math:`\zeta
+00009cd0: 6020 616e 640a 2020 2020 2020 2020 2020  ` and.          
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00009cf0: 7272 6573 706f 6e64 696e 6720 6372 6564  rresponding cred
+00009d00: 6962 696c 6974 7920 6261 6e64 732e 2044  ibility bands. D
+00009d10: 6566 6175 6c74 2069 7320 3530 3030 302e  efault is 50000.
+00009d20: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+00009d30: 5f6a 6f69 6e74 5f73 616d 706c 6573 3a20  _joint_samples: 
+00009d40: 696e 740a 2020 2020 2020 2020 3a70 6172  int.        :par
+00009d50: 616d 206e 5f73 6c6f 7065 5f73 616d 706c  am n_slope_sampl
+00009d60: 6573 3a20 4e75 6d62 6572 206f 6620 6472  es: Number of dr
+00009d70: 6966 7420 736c 6f70 6520 7361 6d70 6c65  ift slope sample
+00009d80: 7320 7468 6174 2061 7265 2064 7261 776e  s that are drawn
+00009d90: 2066 726f 6d20 7468 6520 6573 7469 6d61   from the estima
+00009da0: 7465 6420 6472 6966 7420 736c 6f70 650a  ted drift slope.
 00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2070 6f73 7465 7269 6f72         posterior
-00009dd0: 2063 6f6d 7075 7465 6420 6261 7365 6420   computed based 
-00009de0: 6f6e 2074 6865 2073 616d 706c 696e 6720  on the sampling 
-00009df0: 7265 7375 6c74 7320 6f66 2074 6865 206a  results of the j
-00009e00: 6f69 6e74 2070 6f73 7465 7269 6f72 2070  oint posterior p
-00009e10: 726f 6261 6269 6c69 7479 0a20 2020 2020  robability.     
+00009dc0: 2020 2020 2020 2020 706f 7374 6572 696f          posterio
+00009dd0: 7220 636f 6d70 7574 6564 2062 6173 6564  r computed based
+00009de0: 206f 6e20 7468 6520 7361 6d70 6c69 6e67   on the sampling
+00009df0: 2072 6573 756c 7473 206f 6620 7468 6520   results of the 
+00009e00: 6a6f 696e 7420 706f 7374 6572 696f 7220  joint posterior 
+00009e10: 7072 6f62 6162 696c 6974 790a 2020 2020  probability.    
 00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 206f 6620 7468 6520 4c61 6e67 6576     of the Langev
-00009e40: 696e 2070 6172 616d 6574 6572 7320 3a6d  in parameters :m
-00009e50: 6174 683a 605c 7468 6574 615f 6960 2e20  ath:`\theta_i`. 
-00009e60: 4465 6661 756c 7420 6973 2035 3030 3030  Default is 50000
-00009e70: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00009e80: 6e5f 736c 6f70 655f 7361 6d70 6c65 733a  n_slope_samples:
-00009e90: 2069 6e74 0a20 2020 2020 2020 203a 7061   int.        :pa
-00009ea0: 7261 6d20 6e5f 6e6f 6973 655f 7361 6d70  ram n_noise_samp
-00009eb0: 6c65 733a 204e 756d 6265 7220 6f66 2063  les: Number of c
-00009ec0: 6f6e 7374 616e 7420 6e6f 6973 6520 6c65  onstant noise le
-00009ed0: 7665 6c20 7361 6d70 6c65 7320 7468 6174  vel samples that
-00009ee0: 2061 7265 2064 7261 776e 2066 726f 6d20   are drawn from 
-00009ef0: 7468 6520 6573 7469 6d61 7465 640a 2020  the estimated.  
+00009e30: 2020 2020 6f66 2074 6865 204c 616e 6765      of the Lange
+00009e40: 7669 6e20 7061 7261 6d65 7465 7273 203a  vin parameters :
+00009e50: 6d61 7468 3a60 5c74 6865 7461 5f69 602e  math:`\theta_i`.
+00009e60: 2044 6566 6175 6c74 2069 7320 3530 3030   Default is 5000
+00009e70: 302e 0a20 2020 2020 2020 203a 7479 7065  0..        :type
+00009e80: 206e 5f73 6c6f 7065 5f73 616d 706c 6573   n_slope_samples
+00009e90: 3a20 696e 740a 2020 2020 2020 2020 3a70  : int.        :p
+00009ea0: 6172 616d 206e 5f6e 6f69 7365 5f73 616d  aram n_noise_sam
+00009eb0: 706c 6573 3a20 4e75 6d62 6572 206f 6620  ples: Number of 
+00009ec0: 636f 6e73 7461 6e74 206e 6f69 7365 206c  constant noise l
+00009ed0: 6576 656c 2073 616d 706c 6573 2074 6861  evel samples tha
+00009ee0: 7420 6172 6520 6472 6177 6e20 6672 6f6d  t are drawn from
+00009ef0: 2074 6865 2065 7374 696d 6174 6564 0a20   the estimated. 
 00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 2020 6d61 7269 676e 616c 2070        marignal p
-00009f20: 726f 6269 6c69 7479 2064 6973 7472 6962  robility distrib
-00009f30: 7574 696f 6e20 6f66 2074 6865 2064 6966  ution of the dif
-00009f40: 6675 7369 6f6e 206d 6f64 656c 2069 7320  fusion model is 
-00009f50: 6368 6f73 656e 2063 6f6e 7374 616e 742e  chosen constant.
-00009f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009f70: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00009f80: 2069 7320 3530 3030 302e 0a20 2020 2020   is 50000..     
-00009f90: 2020 203a 7479 7065 206e 5f6e 6f69 7365     :type n_noise
-00009fa0: 5f73 616d 706c 6573 3a20 696e 740a 2020  _samples: int.  
-00009fb0: 2020 2020 2020 3a70 6172 616d 2063 7265        :param cre
-00009fc0: 645f 7065 7263 656e 7469 6c65 733a 2054  d_percentiles: T
-00009fd0: 776f 2065 6e74 7269 6573 2074 6f20 6465  wo entries to de
-00009fe0: 6669 6e65 2074 6865 2070 6572 6365 6e74  fine the percent
-00009ff0: 696c 6573 206f 6620 7468 6520 6361 6c63  iles of the calc
-0000a000: 756c 6174 6564 2063 7265 6469 6269 6c69  ulated credibili
-0000a010: 7479 2062 616e 6473 0a20 2020 2020 2020  ty bands.       
+00009f10: 2020 2020 2020 206d 6172 6967 6e61 6c20         marignal 
+00009f20: 7072 6f62 696c 6974 7920 6469 7374 7269  probility distri
+00009f30: 6275 7469 6f6e 206f 6620 7468 6520 6469  bution of the di
+00009f40: 6666 7573 696f 6e20 6d6f 6465 6c20 6973  ffusion model is
+00009f50: 2063 686f 7365 6e20 636f 6e73 7461 6e74   chosen constant
+00009f60: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009f70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00009f80: 7420 6973 2035 3030 3030 2e0a 2020 2020  t is 50000..    
+00009f90: 2020 2020 3a74 7970 6520 6e5f 6e6f 6973      :type n_nois
+00009fa0: 655f 7361 6d70 6c65 733a 2069 6e74 0a20  e_samples: int. 
+00009fb0: 2020 2020 2020 203a 7061 7261 6d20 6372         :param cr
+00009fc0: 6564 5f70 6572 6365 6e74 696c 6573 3a20  ed_percentiles: 
+00009fd0: 5477 6f20 656e 7472 6965 7320 746f 2064  Two entries to d
+00009fe0: 6566 696e 6520 7468 6520 7065 7263 656e  efine the percen
+00009ff0: 7469 6c65 7320 6f66 2074 6865 2063 616c  tiles of the cal
+0000a000: 6375 6c61 7465 6420 6372 6564 6962 696c  culated credibil
+0000a010: 6974 7920 6261 6e64 730a 2020 2020 2020  ity bands.      
 0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 206f 6620 7468 6520 6573 7469 6d61 7465   of the estimate
-0000a040: 6420 7061 7261 6d65 7465 7273 2e20 4465  d parameters. De
-0000a050: 6661 756c 7420 6973 2060 606e 756d 7079  fault is ``numpy
-0000a060: 2e61 7272 6179 285b 3136 2c31 5d29 6060  .array([16,1])``
-0000a070: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000a080: 6372 6564 5f70 6572 6365 6e74 696c 6573  cred_percentiles
-0000a090: 3a20 4f6e 652d 6469 6d65 6e73 696f 6e61  : One-dimensiona
-0000a0a0: 6c20 6e75 6d70 7920 6172 7261 7920 6f66  l numpy array of
-0000a0b0: 2069 6e74 6567 6572 730a 2020 2020 2020   integers.      
-0000a0c0: 2020 3a70 6172 616d 2070 7269 6e74 5f41    :param print_A
-0000a0d0: 435f 7461 753a 2049 6620 6060 5472 7565  C_tau: If ``True
-0000a0e0: 6060 2074 6865 2065 7374 696d 6174 6564  `` the estimated
-0000a0f0: 2061 7574 6f63 6f72 7265 6c61 7469 6f6e   autocorrelation
-0000a100: 206c 656e 6774 6873 206f 6620 7468 6520   lengths of the 
-0000a110: 4d61 726b 6f76 2063 6861 696e 7320 6973  Markov chains is
-0000a120: 2073 686f 776e 2e0a 2020 2020 2020 2020   shown..        
+0000a030: 2020 6f66 2074 6865 2065 7374 696d 6174    of the estimat
+0000a040: 6564 2070 6172 616d 6574 6572 732e 2044  ed parameters. D
+0000a050: 6566 6175 6c74 2069 7320 6060 6e75 6d70  efault is ``nump
+0000a060: 792e 6172 7261 7928 5b31 362c 315d 2960  y.array([16,1])`
+0000a070: 602e 0a20 2020 2020 2020 203a 7479 7065  `..        :type
+0000a080: 2063 7265 645f 7065 7263 656e 7469 6c65   cred_percentile
+0000a090: 733a 204f 6e65 2d64 696d 656e 7369 6f6e  s: One-dimension
+0000a0a0: 616c 206e 756d 7079 2061 7272 6179 206f  al numpy array o
+0000a0b0: 6620 696e 7465 6765 7273 0a20 2020 2020  f integers.     
+0000a0c0: 2020 203a 7061 7261 6d20 7072 696e 745f     :param print_
+0000a0d0: 4143 5f74 6175 3a20 4966 2060 6054 7275  AC_tau: If ``Tru
+0000a0e0: 6560 6020 7468 6520 6573 7469 6d61 7465  e`` the estimate
+0000a0f0: 6420 6175 746f 636f 7272 656c 6174 696f  d autocorrelatio
+0000a100: 6e20 6c65 6e67 7468 7320 6f66 2074 6865  n lengths of the
+0000a110: 204d 6172 6b6f 7620 6368 6169 6e73 2069   Markov chains i
+0000a120: 7320 7368 6f77 6e2e 0a20 2020 2020 2020  s shown..       
 0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a140: 5468 6520 6d61 7869 6d75 6d20 6c65 6e67  The maximum leng
-0000a150: 7468 2069 7320 7573 6564 2066 6f72 2074  th is used for t
-0000a160: 6869 6e6e 696e 6720 6f66 2074 6865 2063  hinning of the c
-0000a170: 6861 696e 732e 2044 6566 6175 6c74 2069  hains. Default i
-0000a180: 7320 6060 4661 6c73 6560 602e 0a20 2020  s ``False``..   
-0000a190: 2020 2020 203a 7479 7065 2070 7269 6e64       :type prind
-0000a1a0: 5f41 435f 7461 753a 2062 6f6f 6c0a 2020  _AC_tau: bool.  
-0000a1b0: 2020 2020 2020 3a70 6172 616d 2069 676e        :param ign
-0000a1c0: 6f72 655f 4143 5f65 7272 6f72 3a20 4966  ore_AC_error: If
-0000a1d0: 2060 6054 7275 6560 6020 7468 6520 6175   ``True`` the au
-0000a1e0: 746f 636f 7272 656c 6174 696f 6e20 6c65  tocorrelation le
-0000a1f0: 6e67 7468 7320 6f66 2074 6865 204d 6172  ngths of the Mar
-0000a200: 6b6f 7620 6368 6169 6e73 2069 7320 6e6f  kov chains is no
-0000a210: 7420 6573 7469 6d61 7465 640a 2020 2020  t estimated.    
+0000a140: 2054 6865 206d 6178 696d 756d 206c 656e   The maximum len
+0000a150: 6774 6820 6973 2075 7365 6420 666f 7220  gth is used for 
+0000a160: 7468 696e 6e69 6e67 206f 6620 7468 6520  thinning of the 
+0000a170: 6368 6169 6e73 2e20 4465 6661 756c 7420  chains. Default 
+0000a180: 6973 2060 6046 616c 7365 6060 2e0a 2020  is ``False``..  
+0000a190: 2020 2020 2020 3a74 7970 6520 7072 696e        :type prin
+0000a1a0: 645f 4143 5f74 6175 3a20 626f 6f6c 0a20  d_AC_tau: bool. 
+0000a1b0: 2020 2020 2020 203a 7061 7261 6d20 6967         :param ig
+0000a1c0: 6e6f 7265 5f41 435f 6572 726f 723a 2049  nore_AC_error: I
+0000a1d0: 6620 6060 5472 7565 6060 2074 6865 2061  f ``True`` the a
+0000a1e0: 7574 6f63 6f72 7265 6c61 7469 6f6e 206c  utocorrelation l
+0000a1f0: 656e 6774 6873 206f 6620 7468 6520 4d61  engths of the Ma
+0000a200: 726b 6f76 2063 6861 696e 7320 6973 206e  rkov chains is n
+0000a210: 6f74 2065 7374 696d 6174 6564 0a20 2020  ot estimated.   
 0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2020 2020 616e 6420 7468 7573 2c20 6974      and thus, it
-0000a240: 2069 7320 6e6f 7420 6368 6563 6b65 6420   is not checked 
-0000a250: 7768 6574 6865 7220 7468 6520 6368 6169  whether the chai
-0000a260: 6e73 2061 7265 2074 6f6f 2073 686f 7274  ns are too short
-0000a270: 2074 6f20 6769 7665 2061 6e20 7265 6c69   to give an reli
-0000a280: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
-0000a290: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-0000a2a0: 6f63 6f72 7265 6c61 7469 6f6e 2065 7374  ocorrelation est
-0000a2b0: 696d 6174 652e 2054 6869 7320 6176 6f69  imate. This avoi
-0000a2c0: 6473 2065 7272 6f72 2069 6e74 6572 7275  ds error interru
-0000a2d0: 7074 696f 6e20 6f66 2074 6865 2070 726f  ption of the pro
-0000a2e0: 6365 6475 7265 2c20 6275 740a 2020 2020  cedure, but.    
+0000a230: 2020 2020 2061 6e64 2074 6875 732c 2069       and thus, i
+0000a240: 7420 6973 206e 6f74 2063 6865 636b 6564  t is not checked
+0000a250: 2077 6865 7468 6572 2074 6865 2063 6861   whether the cha
+0000a260: 696e 7320 6172 6520 746f 6f20 7368 6f72  ins are too shor
+0000a270: 7420 746f 2067 6976 6520 616e 2072 656c  t to give an rel
+0000a280: 6961 626c 650a 2020 2020 2020 2020 2020  iable.          
+0000a290: 2020 2020 2020 2020 2020 2020 2020 6175                au
+0000a2a0: 746f 636f 7272 656c 6174 696f 6e20 6573  tocorrelation es
+0000a2b0: 7469 6d61 7465 2e20 5468 6973 2061 766f  timate. This avo
+0000a2c0: 6964 7320 6572 726f 7220 696e 7465 7272  ids error interr
+0000a2d0: 7570 7469 6f6e 206f 6620 7468 6520 7072  uption of the pr
+0000a2e0: 6f63 6564 7572 652c 2062 7574 0a20 2020  ocedure, but.   
 0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 6361 6e20 6c65 6164 2074 6f20      can lead to 
-0000a310: 756e 7265 6c69 6162 6c65 2072 6573 756c  unreliable resul
-0000a320: 7473 2069 6620 7468 6520 6368 6169 6e73  ts if the chains
-0000a330: 2061 7265 2074 6f6f 2073 686f 7274 2e20   are too short. 
-0000a340: 5468 6520 6f70 7469 6f6e 2073 686f 756c  The option shoul
-0000a350: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000a360: 2020 2020 2020 2020 2020 6265 2063 686f            be cho
-0000a370: 7365 6e20 696e 206f 7264 6572 2074 6f20  sen in order to 
-0000a380: 7361 7665 2063 6f6d 7075 7461 7469 6f6e  save computation
-0000a390: 2074 696d 652c 2065 2e67 2e20 7768 656e   time, e.g. when
-0000a3a0: 2064 6562 7567 6769 6e67 2079 6f75 7220   debugging your 
-0000a3b0: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
-0000a3c0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-0000a3d0: 6820 7368 6f72 7420 4d61 726b 6f76 2063  h short Markov c
-0000a3e0: 6861 696e 732e 2044 6566 6175 6c74 2069  hains. Default i
-0000a3f0: 7320 6060 4661 6c73 6560 602e 0a20 2020  s ``False``..   
-0000a400: 2020 2020 203a 7479 7065 2069 676e 6f72       :type ignor
-0000a410: 655f 4143 5f65 7272 6f72 3a20 626f 6f6c  e_AC_error: bool
-0000a420: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000a430: 7468 696e 6e69 6e67 5f62 793a 2049 6620  thinning_by: If 
-0000a440: 6060 6967 6e6f 7265 5f41 435f 6572 726f  ``ignore_AC_erro
-0000a450: 7220 3d20 5472 7565 6060 2074 6865 2063  r = True`` the c
-0000a460: 6861 696e 7320 6172 6520 7468 696e 6e65  hains are thinne
-0000a470: 6420 6279 2060 6074 6869 6e6e 696e 675f  d by ``thinning_
-0000a480: 6279 6060 2e20 4576 6572 790a 2020 2020  by``. Every.    
+0000a300: 2020 2020 2063 616e 206c 6561 6420 746f       can lead to
+0000a310: 2075 6e72 656c 6961 626c 6520 7265 7375   unreliable resu
+0000a320: 6c74 7320 6966 2074 6865 2063 6861 696e  lts if the chain
+0000a330: 7320 6172 6520 746f 6f20 7368 6f72 742e  s are too short.
+0000a340: 2054 6865 206f 7074 696f 6e20 7368 6f75   The option shou
+0000a350: 6c64 0a20 2020 2020 2020 2020 2020 2020  ld.             
+0000a360: 2020 2020 2020 2020 2020 2062 6520 6368             be ch
+0000a370: 6f73 656e 2069 6e20 6f72 6465 7220 746f  osen in order to
+0000a380: 2073 6176 6520 636f 6d70 7574 6174 696f   save computatio
+0000a390: 6e20 7469 6d65 2c20 652e 672e 2077 6865  n time, e.g. whe
+0000a3a0: 6e20 6465 6275 6767 696e 6720 796f 7572  n debugging your
+0000a3b0: 2063 6f64 650a 2020 2020 2020 2020 2020   code.          
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+0000a3d0: 7468 2073 686f 7274 204d 6172 6b6f 7620  th short Markov 
+0000a3e0: 6368 6169 6e73 2e20 4465 6661 756c 7420  chains. Default 
+0000a3f0: 6973 2060 6046 616c 7365 6060 2e0a 2020  is ``False``..  
+0000a400: 2020 2020 2020 3a74 7970 6520 6967 6e6f        :type igno
+0000a410: 7265 5f41 435f 6572 726f 723a 2062 6f6f  re_AC_error: boo
+0000a420: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
+0000a430: 2074 6869 6e6e 696e 675f 6279 3a20 4966   thinning_by: If
+0000a440: 2060 6069 676e 6f72 655f 4143 5f65 7272   ``ignore_AC_err
+0000a450: 6f72 203d 2054 7275 6560 6020 7468 6520  or = True`` the 
+0000a460: 6368 6169 6e73 2061 7265 2074 6869 6e6e  chains are thinn
+0000a470: 6564 2062 7920 6060 7468 696e 6e69 6e67  ed by ``thinning
+0000a480: 5f62 7960 602e 2045 7665 7279 0a20 2020  _by``. Every.   
 0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 6060 7468 696e 6e69 6e67 5f62      ``thinning_b
-0000a4b0: 7960 602d 7468 2064 6174 6120 706f 696e  y``-th data poin
-0000a4c0: 7420 6973 2073 746f 7265 642e 2044 6566  t is stored. Def
-0000a4d0: 6175 6c74 2069 7320 3630 2e0a 2020 2020  ault is 60..    
-0000a4e0: 2020 2020 3a74 7970 6520 7468 696e 6e69      :type thinni
-0000a4f0: 6e67 5f62 793a 2069 6e74 0a20 2020 2020  ng_by: int.     
-0000a500: 2020 203a 7061 7261 6d20 7072 696e 745f     :param print_
-0000a510: 7072 6f67 7265 7373 3a20 4966 2060 6054  progress: If ``T
-0000a520: 7275 6560 6020 7468 6520 7072 6f67 7265  rue`` the progre
-0000a530: 7373 206f 6620 7468 6520 4d43 4d43 2073  ss of the MCMC s
-0000a540: 616d 706c 696e 6720 6973 2073 686f 776e  ampling is shown
-0000a550: 2e20 4465 6661 756c 7420 6973 2060 6046  . Default is ``F
-0000a560: 616c 7365 6060 2e0a 2020 2020 2020 2020  alse``..        
-0000a570: 3a74 7970 6520 7072 696e 745f 7072 6f67  :type print_prog
-0000a580: 7265 7373 3a20 626f 6f6c 0a20 2020 2020  ress: bool.     
-0000a590: 2020 203a 7061 7261 6d20 6465 7472 656e     :param detren
-0000a5a0: 6469 6e67 5f70 6572 5f77 696e 646f 773a  ding_per_window:
-0000a5b0: 2044 6566 6175 6c74 2069 7320 6060 4e6f   Default is ``No
-0000a5c0: 6e65 6060 2e20 4966 2060 6027 6c69 6e65  ne``. If ``'line
-0000a5d0: 6172 2760 602c 2074 6865 2060 6073 656c  ar'``, the ``sel
-0000a5e0: 662e 6461 7461 5f77 696e 646f 7760 6020  f.data_window`` 
-0000a5f0: 6973 2064 6574 7265 6e64 6564 206c 696e  is detrended lin
-0000a600: 6561 726c 792e 2049 660a 2020 2020 2020  early. If.      
+0000a4a0: 2020 2020 2060 6074 6869 6e6e 696e 675f       ``thinning_
+0000a4b0: 6279 6060 2d74 6820 6461 7461 2070 6f69  by``-th data poi
+0000a4c0: 6e74 2069 7320 7374 6f72 6564 2e20 4465  nt is stored. De
+0000a4d0: 6661 756c 7420 6973 2036 302e 0a20 2020  fault is 60..   
+0000a4e0: 2020 2020 203a 7479 7065 2074 6869 6e6e       :type thinn
+0000a4f0: 696e 675f 6279 3a20 696e 740a 2020 2020  ing_by: int.    
+0000a500: 2020 2020 3a70 6172 616d 2070 7269 6e74      :param print
+0000a510: 5f70 726f 6772 6573 733a 2049 6620 6060  _progress: If ``
+0000a520: 5472 7565 6060 2074 6865 2070 726f 6772  True`` the progr
+0000a530: 6573 7320 6f66 2074 6865 204d 434d 4320  ess of the MCMC 
+0000a540: 7361 6d70 6c69 6e67 2069 7320 7368 6f77  sampling is show
+0000a550: 6e2e 2044 6566 6175 6c74 2069 7320 6060  n. Default is ``
+0000a560: 4661 6c73 6560 602e 0a20 2020 2020 2020  False``..       
+0000a570: 203a 7479 7065 2070 7269 6e74 5f70 726f   :type print_pro
+0000a580: 6772 6573 733a 2062 6f6f 6c0a 2020 2020  gress: bool.    
+0000a590: 2020 2020 3a70 6172 616d 2064 6574 7265      :param detre
+0000a5a0: 6e64 696e 675f 7065 725f 7769 6e64 6f77  nding_per_window
+0000a5b0: 3a20 4465 6661 756c 7420 6973 2060 604e  : Default is ``N
+0000a5c0: 6f6e 6560 602e 2049 6620 6060 276c 696e  one``. If ``'lin
+0000a5d0: 6561 7227 6060 2c20 7468 6520 6060 7365  ear'``, the ``se
+0000a5e0: 6c66 2e64 6174 615f 7769 6e64 6f77 6060  lf.data_window``
+0000a5f0: 2069 7320 6465 7472 656e 6465 6420 6c69   is detrended li
+0000a600: 6e65 6172 6c79 2e20 4966 0a20 2020 2020  nearly. If.     
 0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 6060 4761 7573 7369 616e 206b 6572    ``Gaussian ker
-0000a630: 6e65 6c20 736d 6f6f 7468 6564 6060 2c20  nel smoothed``, 
-0000a640: 6120 4761 7573 7369 616e 2073 6d6f 6f74  a Gaussian smoot
-0000a650: 6865 6420 6375 7276 6520 6973 2073 7562  hed curve is sub
-0000a660: 7472 6163 7465 6420 6672 6f6d 2060 6073  tracted from ``s
-0000a670: 656c 662e 6461 7461 5f77 696e 646f 7760  elf.data_window`
-0000a680: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
-0000a690: 2020 2020 2020 2020 2020 2054 6865 2070             The p
-0000a6a0: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
-0000a6b0: 206b 6572 6e65 6c20 736d 6f6f 7468 696e   kernel smoothin
-0000a6c0: 6720 6361 6e20 6265 2073 6574 2062 7920  g can be set by 
-0000a6d0: 6060 6761 7573 735f 6669 6c74 6572 5f6d  ``gauss_filter_m
-0000a6e0: 6f64 6560 602c 2060 6067 6175 7373 5f66  ode``, ``gauss_f
-0000a6f0: 696c 7465 725f 7369 676d 6160 602c 0a20  ilter_sigma``,. 
+0000a620: 2020 2060 6047 6175 7373 6961 6e20 6b65     ``Gaussian ke
+0000a630: 726e 656c 2073 6d6f 6f74 6865 6460 602c  rnel smoothed``,
+0000a640: 2061 2047 6175 7373 6961 6e20 736d 6f6f   a Gaussian smoo
+0000a650: 7468 6564 2063 7572 7665 2069 7320 7375  thed curve is su
+0000a660: 6274 7261 6374 6564 2066 726f 6d20 6060  btracted from ``
+0000a670: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
+0000a680: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
+0000a690: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000a6a0: 7061 7261 6d65 7465 7273 206f 6620 7468  parameters of th
+0000a6b0: 6520 6b65 726e 656c 2073 6d6f 6f74 6869  e kernel smoothi
+0000a6c0: 6e67 2063 616e 2062 6520 7365 7420 6279  ng can be set by
+0000a6d0: 2060 6067 6175 7373 5f66 696c 7465 725f   ``gauss_filter_
+0000a6e0: 6d6f 6465 6060 2c20 6060 6761 7573 735f  mode``, ``gauss_
+0000a6f0: 6669 6c74 6572 5f73 6967 6d61 6060 2c0a  filter_sigma``,.
 0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a710: 2020 2020 2020 2060 6067 6175 7373 5f66         ``gauss_f
-0000a720: 696c 7465 725f 6f72 6465 7260 602c 2060  ilter_order``, `
-0000a730: 6067 6175 7373 5f66 696c 7465 725f 6376  `gauss_filter_cv
-0000a740: 616c 6060 2061 6e64 2060 6067 6175 7373  al`` and ``gauss
-0000a750: 5f66 696c 7465 725f 7472 756e 6361 7465  _filter_truncate
-0000a760: 6060 2e20 4472 6966 7420 736c 6f70 6520  ``. Drift slope 
-0000a770: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-0000a780: 2020 2020 2020 2020 2020 2020 6e6f 6973              nois
-0000a790: 6520 6c65 7665 6c20 6172 6520 6573 7469  e level are esti
-0000a7a0: 6d61 7465 6420 6166 7465 7220 6465 7472  mated after detr
-0000a7b0: 656e 6469 6e67 2069 6e20 7468 6573 6520  ending in these 
-0000a7c0: 6361 7365 732e 0a20 2020 2020 2020 203a  cases..        :
-0000a7d0: 7479 7065 2064 6574 7265 6e64 696e 675f  type detrending_
-0000a7e0: 7065 725f 7769 6e64 6f77 3a20 7374 720a  per_window: str.
-0000a7f0: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
-0000a800: 6175 7373 5f66 696c 7465 725f 6d6f 6465  auss_filter_mode
-0000a810: 3a20 4163 636f 7264 696e 6720 746f 2074  : According to t
-0000a820: 6865 2060 6073 6369 7079 2e6e 6469 6d61  he ``scipy.ndima
-0000a830: 6765 2e66 696c 7465 7273 2e67 6175 7373  ge.filters.gauss
-0000a840: 6961 6e5f 6669 6c74 6572 6060 206f 7074  ian_filter`` opt
-0000a850: 696f 6e2e 0a20 2020 2020 2020 203a 7479  ion..        :ty
-0000a860: 7065 2067 6175 7373 5f66 696c 7465 725f  pe gauss_filter_
-0000a870: 6d6f 6465 3a20 7374 720a 2020 2020 2020  mode: str.      
-0000a880: 2020 3a70 6172 616d 2067 6175 7373 5f66    :param gauss_f
-0000a890: 696c 7465 725f 7369 676d 613a 2041 6363  ilter_sigma: Acc
-0000a8a0: 6f72 6469 6e67 2074 6f20 7468 6520 6060  ording to the ``
-0000a8b0: 7363 6970 792e 6e64 696d 6167 652e 6669  scipy.ndimage.fi
-0000a8c0: 6c74 6572 732e 6761 7573 7369 616e 5f66  lters.gaussian_f
-0000a8d0: 696c 7465 7260 6020 6f70 7469 6f6e 2e0a  ilter`` option..
-0000a8e0: 2020 2020 2020 2020 3a74 7970 6520 6761          :type ga
-0000a8f0: 7573 735f 6669 6c74 6572 5f73 6967 6d61  uss_filter_sigma
-0000a900: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-0000a910: 3a70 6172 616d 2067 6175 7373 5f66 696c  :param gauss_fil
-0000a920: 7465 725f 6f72 6465 723a 2041 6363 6f72  ter_order: Accor
-0000a930: 6469 6e67 2074 6f20 7468 6520 6060 7363  ding to the ``sc
-0000a940: 6970 792e 6e64 696d 6167 652e 6669 6c74  ipy.ndimage.filt
-0000a950: 6572 732e 6761 7573 7369 616e 5f66 696c  ers.gaussian_fil
-0000a960: 7465 7260 6020 6f70 7469 6f6e 2e0a 2020  ter`` option..  
-0000a970: 2020 2020 2020 3a74 7970 6520 6761 7573        :type gaus
-0000a980: 735f 6669 6c74 6572 5f6f 7264 6572 3a20  s_filter_order: 
-0000a990: 696e 740a 2020 2020 2020 2020 3a70 6172  int.        :par
-0000a9a0: 616d 2067 6175 7373 5f66 696c 7465 725f  am gauss_filter_
-0000a9b0: 6376 616c 3a20 4163 636f 7264 696e 6720  cval: According 
-0000a9c0: 746f 2074 6865 2060 6073 6369 7079 2e6e  to the ``scipy.n
-0000a9d0: 6469 6d61 6765 2e66 696c 7465 7273 2e67  dimage.filters.g
-0000a9e0: 6175 7373 6961 6e5f 6669 6c74 6572 6060  aussian_filter``
-0000a9f0: 206f 7074 696f 6e2e 0a20 2020 2020 2020   option..       
-0000aa00: 203a 7479 7065 2067 6175 7373 5f66 696c   :type gauss_fil
-0000aa10: 7465 725f 6376 616c 3a20 666c 6f61 740a  ter_cval: float.
-0000aa20: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
-0000aa30: 6175 7373 5f66 696c 7465 725f 7472 756e  auss_filter_trun
-0000aa40: 6361 7465 3a20 4163 636f 7264 696e 6720  cate: According 
-0000aa50: 746f 2074 6865 2060 6073 6369 7079 2e6e  to the ``scipy.n
-0000aa60: 6469 6d61 6765 2e66 696c 7465 7273 2e67  dimage.filters.g
-0000aa70: 6175 7373 6961 6e5f 6669 6c74 6572 6060  aussian_filter``
-0000aa80: 206f 7074 696f 6e2e 0a20 2020 2020 2020   option..       
-0000aa90: 203a 7479 7065 2067 6175 7373 5f66 696c   :type gauss_fil
-0000aaa0: 7465 725f 7472 756e 6361 7465 3a20 666c  ter_truncate: fl
-0000aab0: 6f61 740a 2020 2020 2020 2020 3a70 6172  oat.        :par
-0000aac0: 616d 2070 6c6f 745f 6465 7472 656e 6469  am plot_detrendi
-0000aad0: 6e67 3a20 4465 6661 756c 7420 6973 2060  ng: Default is `
-0000aae0: 6046 616c 7365 6060 2e20 4966 2060 6054  `False``. If ``T
-0000aaf0: 7275 6560 602c 2074 6865 2060 6073 656c  rue``, the ``sel
-0000ab00: 662e 6461 7461 6060 2061 7320 7765 6c6c  f.data`` as well
-0000ab10: 2061 7320 7468 650a 2020 2020 2020 2020   as the.        
+0000a710: 2020 2020 2020 2020 6060 6761 7573 735f          ``gauss_
+0000a720: 6669 6c74 6572 5f6f 7264 6572 6060 2c20  filter_order``, 
+0000a730: 6060 6761 7573 735f 6669 6c74 6572 5f63  ``gauss_filter_c
+0000a740: 7661 6c60 6020 616e 6420 6060 6761 7573  val`` and ``gaus
+0000a750: 735f 6669 6c74 6572 5f74 7275 6e63 6174  s_filter_truncat
+0000a760: 6560 602e 2044 7269 6674 2073 6c6f 7065  e``. Drift slope
+0000a770: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+0000a780: 2020 2020 2020 2020 2020 2020 206e 6f69               noi
+0000a790: 7365 206c 6576 656c 2061 7265 2065 7374  se level are est
+0000a7a0: 696d 6174 6564 2061 6674 6572 2064 6574  imated after det
+0000a7b0: 7265 6e64 696e 6720 696e 2074 6865 7365  rending in these
+0000a7c0: 2063 6173 6573 2e0a 2020 2020 2020 2020   cases..        
+0000a7d0: 3a74 7970 6520 6465 7472 656e 6469 6e67  :type detrending
+0000a7e0: 5f70 6572 5f77 696e 646f 773a 2073 7472  _per_window: str
+0000a7f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000a800: 6761 7573 735f 6669 6c74 6572 5f6d 6f64  gauss_filter_mod
+0000a810: 653a 2041 6363 6f72 6469 6e67 2074 6f20  e: According to 
+0000a820: 7468 6520 6060 7363 6970 792e 6e64 696d  the ``scipy.ndim
+0000a830: 6167 652e 6669 6c74 6572 732e 6761 7573  age.filters.gaus
+0000a840: 7369 616e 5f66 696c 7465 7260 6020 6f70  sian_filter`` op
+0000a850: 7469 6f6e 2e0a 2020 2020 2020 2020 3a74  tion..        :t
+0000a860: 7970 6520 6761 7573 735f 6669 6c74 6572  ype gauss_filter
+0000a870: 5f6d 6f64 653a 2073 7472 0a20 2020 2020  _mode: str.     
+0000a880: 2020 203a 7061 7261 6d20 6761 7573 735f     :param gauss_
+0000a890: 6669 6c74 6572 5f73 6967 6d61 3a20 4163  filter_sigma: Ac
+0000a8a0: 636f 7264 696e 6720 746f 2074 6865 2060  cording to the `
+0000a8b0: 6073 6369 7079 2e6e 6469 6d61 6765 2e66  `scipy.ndimage.f
+0000a8c0: 696c 7465 7273 2e67 6175 7373 6961 6e5f  ilters.gaussian_
+0000a8d0: 6669 6c74 6572 6060 206f 7074 696f 6e2e  filter`` option.
+0000a8e0: 0a20 2020 2020 2020 203a 7479 7065 2067  .        :type g
+0000a8f0: 6175 7373 5f66 696c 7465 725f 7369 676d  auss_filter_sigm
+0000a900: 613a 2066 6c6f 6174 0a20 2020 2020 2020  a: float.       
+0000a910: 203a 7061 7261 6d20 6761 7573 735f 6669   :param gauss_fi
+0000a920: 6c74 6572 5f6f 7264 6572 3a20 4163 636f  lter_order: Acco
+0000a930: 7264 696e 6720 746f 2074 6865 2060 6073  rding to the ``s
+0000a940: 6369 7079 2e6e 6469 6d61 6765 2e66 696c  cipy.ndimage.fil
+0000a950: 7465 7273 2e67 6175 7373 6961 6e5f 6669  ters.gaussian_fi
+0000a960: 6c74 6572 6060 206f 7074 696f 6e2e 0a20  lter`` option.. 
+0000a970: 2020 2020 2020 203a 7479 7065 2067 6175         :type gau
+0000a980: 7373 5f66 696c 7465 725f 6f72 6465 723a  ss_filter_order:
+0000a990: 2069 6e74 0a20 2020 2020 2020 203a 7061   int.        :pa
+0000a9a0: 7261 6d20 6761 7573 735f 6669 6c74 6572  ram gauss_filter
+0000a9b0: 5f63 7661 6c3a 2041 6363 6f72 6469 6e67  _cval: According
+0000a9c0: 2074 6f20 7468 6520 6060 7363 6970 792e   to the ``scipy.
+0000a9d0: 6e64 696d 6167 652e 6669 6c74 6572 732e  ndimage.filters.
+0000a9e0: 6761 7573 7369 616e 5f66 696c 7465 7260  gaussian_filter`
+0000a9f0: 6020 6f70 7469 6f6e 2e0a 2020 2020 2020  ` option..      
+0000aa00: 2020 3a74 7970 6520 6761 7573 735f 6669    :type gauss_fi
+0000aa10: 6c74 6572 5f63 7661 6c3a 2066 6c6f 6174  lter_cval: float
+0000aa20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000aa30: 6761 7573 735f 6669 6c74 6572 5f74 7275  gauss_filter_tru
+0000aa40: 6e63 6174 653a 2041 6363 6f72 6469 6e67  ncate: According
+0000aa50: 2074 6f20 7468 6520 6060 7363 6970 792e   to the ``scipy.
+0000aa60: 6e64 696d 6167 652e 6669 6c74 6572 732e  ndimage.filters.
+0000aa70: 6761 7573 7369 616e 5f66 696c 7465 7260  gaussian_filter`
+0000aa80: 6020 6f70 7469 6f6e 2e0a 2020 2020 2020  ` option..      
+0000aa90: 2020 3a74 7970 6520 6761 7573 735f 6669    :type gauss_fi
+0000aaa0: 6c74 6572 5f74 7275 6e63 6174 653a 2066  lter_truncate: f
+0000aab0: 6c6f 6174 0a20 2020 2020 2020 203a 7061  loat.        :pa
+0000aac0: 7261 6d20 706c 6f74 5f64 6574 7265 6e64  ram plot_detrend
+0000aad0: 696e 673a 2044 6566 6175 6c74 2069 7320  ing: Default is 
+0000aae0: 6060 4661 6c73 6560 602e 2049 6620 6060  ``False``. If ``
+0000aaf0: 5472 7565 6060 2c20 7468 6520 6060 7365  True``, the ``se
+0000ab00: 6c66 2e64 6174 6160 6020 6173 2077 656c  lf.data`` as wel
+0000ab10: 6c20 6173 2074 6865 0a20 2020 2020 2020  l as the.       
 0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab30: 2020 2020 6060 7365 6c66 2e73 6c6f 775f      ``self.slow_
-0000ab40: 7472 656e 6460 6020 616e 6420 7468 6520  trend`` and the 
-0000ab50: 6465 7472 656e 6465 6420 7665 7273 696f  detrended versio
-0000ab60: 6e20 6172 6520 7368 6f77 6e2e 0a20 2020  n are shown..   
-0000ab70: 2020 2020 203a 7479 7065 2070 6c6f 745f       :type plot_
-0000ab80: 6465 7472 656e 6469 6e67 3a20 626f 6f6c  detrending: bool
-0000ab90: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0000aba0: 2020 2020 2063 7265 645f 7065 7263 656e       cred_percen
-0000abb0: 7469 6c65 7320 3d20 6e70 2e61 7272 6179  tiles = np.array
-0000abc0: 2863 7265 645f 7065 7263 656e 7469 6c65  (cred_percentile
-0000abd0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000abe0: 6461 7461 5f77 696e 646f 7720 3d20 6e70  data_window = np
-0000abf0: 2e72 6f6c 6c28 7365 6c66 2e64 6174 612c  .roll(self.data,
-0000ac00: 2073 6869 6674 3d2d 2073 656c 662e 7769   shift=- self.wi
-0000ac10: 6e64 6f77 5f73 6869 6674 295b 3a73 656c  ndow_shift)[:sel
-0000ac20: 662e 7769 6e64 6f77 5f73 697a 655d 0a20  f.window_size]. 
-0000ac30: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-0000ac40: 5f77 696e 646f 7720 3d20 6e70 2e72 6f6c  _window = np.rol
-0000ac50: 6c28 7365 6c66 2e74 696d 652c 2073 6869  l(self.time, shi
-0000ac60: 6674 3d2d 2073 656c 662e 7769 6e64 6f77  ft=- self.window
-0000ac70: 5f73 6869 6674 295b 3a73 656c 662e 7769  _shift)[:self.wi
-0000ac80: 6e64 6f77 5f73 697a 655d 0a20 2020 2020  ndow_size].     
-0000ac90: 2020 2069 6620 6465 7472 656e 6469 6e67     if detrending
-0000aca0: 5f70 6572 5f77 696e 646f 7720 213d 204e  _per_window != N
-0000acb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000acc0: 2073 656c 662e 6461 7461 5f77 696e 646f   self.data_windo
-0000acd0: 772c 2073 656c 662e 736c 6f77 5f74 7265  w, self.slow_tre
-0000ace0: 6e64 203d 2073 656c 662e 6465 7472 656e  nd = self.detren
-0000acf0: 6428 7365 6c66 2e74 696d 655f 7769 6e64  d(self.time_wind
-0000ad00: 6f77 2c20 7365 6c66 2e64 6174 615f 7769  ow, self.data_wi
-0000ad10: 6e64 6f77 2c0a 2020 2020 2020 2020 2020  ndow,.          
+0000ab30: 2020 2020 2060 6073 656c 662e 736c 6f77       ``self.slow
+0000ab40: 5f74 7265 6e64 6060 2061 6e64 2074 6865  _trend`` and the
+0000ab50: 2064 6574 7265 6e64 6564 2076 6572 7369   detrended versi
+0000ab60: 6f6e 2061 7265 2073 686f 776e 2e0a 2020  on are shown..  
+0000ab70: 2020 2020 2020 3a74 7970 6520 706c 6f74        :type plot
+0000ab80: 5f64 6574 7265 6e64 696e 673a 2062 6f6f  _detrending: boo
+0000ab90: 6c0a 2020 2020 2020 2020 2727 270a 2020  l.        '''.  
+0000aba0: 2020 2020 2020 6372 6564 5f70 6572 6365        cred_perce
+0000abb0: 6e74 696c 6573 203d 206e 702e 6172 7261  ntiles = np.arra
+0000abc0: 7928 6372 6564 5f70 6572 6365 6e74 696c  y(cred_percentil
+0000abd0: 6573 290a 2020 2020 2020 2020 7365 6c66  es).        self
+0000abe0: 2e64 6174 615f 7769 6e64 6f77 203d 206e  .data_window = n
+0000abf0: 702e 726f 6c6c 2873 656c 662e 6461 7461  p.roll(self.data
+0000ac00: 2c20 7368 6966 743d 2d20 7365 6c66 2e77  , shift=- self.w
+0000ac10: 696e 646f 775f 7368 6966 7429 5b3a 7365  indow_shift)[:se
+0000ac20: 6c66 2e77 696e 646f 775f 7369 7a65 5d0a  lf.window_size].
+0000ac30: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+0000ac40: 655f 7769 6e64 6f77 203d 206e 702e 726f  e_window = np.ro
+0000ac50: 6c6c 2873 656c 662e 7469 6d65 2c20 7368  ll(self.time, sh
+0000ac60: 6966 743d 2d20 7365 6c66 2e77 696e 646f  ift=- self.windo
+0000ac70: 775f 7368 6966 7429 5b3a 7365 6c66 2e77  w_shift)[:self.w
+0000ac80: 696e 646f 775f 7369 7a65 5d0a 2020 2020  indow_size].    
+0000ac90: 2020 2020 6966 2064 6574 7265 6e64 696e      if detrendin
+0000aca0: 675f 7065 725f 7769 6e64 6f77 2021 3d20  g_per_window != 
+0000acb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000acc0: 2020 7365 6c66 2e64 6174 615f 7769 6e64    self.data_wind
+0000acd0: 6f77 2c20 7365 6c66 2e73 6c6f 775f 7472  ow, self.slow_tr
+0000ace0: 656e 6420 3d20 7365 6c66 2e64 6574 7265  end = self.detre
+0000acf0: 6e64 2873 656c 662e 7469 6d65 5f77 696e  nd(self.time_win
+0000ad00: 646f 772c 2073 656c 662e 6461 7461 5f77  dow, self.data_w
+0000ad10: 696e 646f 772c 0a20 2020 2020 2020 2020  indow,.         
 0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad50: 2020 2020 2020 2020 6465 7472 656e 6469          detrendi
-0000ad60: 6e67 5f70 6572 5f77 696e 646f 772c 6761  ng_per_window,ga
-0000ad70: 7573 735f 6669 6c74 6572 5f6d 6f64 652c  uss_filter_mode,
-0000ad80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad50: 2020 2020 2020 2020 2064 6574 7265 6e64           detrend
+0000ad60: 696e 675f 7065 725f 7769 6e64 6f77 2c67  ing_per_window,g
+0000ad70: 6175 7373 5f66 696c 7465 725f 6d6f 6465  auss_filter_mode
+0000ad80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adc0: 2020 2067 6175 7373 5f66 696c 7465 725f     gauss_filter_
-0000add0: 7369 676d 612c 6761 7573 735f 6669 6c74  sigma,gauss_filt
-0000ade0: 6572 5f6f 7264 6572 2c0a 2020 2020 2020  er_order,.      
+0000adc0: 2020 2020 6761 7573 735f 6669 6c74 6572      gauss_filter
+0000add0: 5f73 6967 6d61 2c67 6175 7373 5f66 696c  _sigma,gauss_fil
+0000ade0: 7465 725f 6f72 6465 722c 0a20 2020 2020  ter_order,.     
 0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 2020 2020 2020 2020 2020 6761 7573              gaus
-0000ae30: 735f 6669 6c74 6572 5f63 7661 6c2c 2067  s_filter_cval, g
-0000ae40: 6175 7373 5f66 696c 7465 725f 7472 756e  auss_filter_trun
-0000ae50: 6361 7465 2c0a 2020 2020 2020 2020 2020  cate,.          
+0000ae20: 2020 2020 2020 2020 2020 2020 2067 6175               gau
+0000ae30: 7373 5f66 696c 7465 725f 6376 616c 2c20  ss_filter_cval, 
+0000ae40: 6761 7573 735f 6669 6c74 6572 5f74 7275  gauss_filter_tru
+0000ae50: 6e63 6174 652c 0a20 2020 2020 2020 2020  ncate,.         
 0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 2020 2020 2020 2020 706c 6f74 5f64 6574          plot_det
-0000aea0: 7265 6e64 696e 6729 0a20 2020 2020 2020  rending).       
-0000aeb0: 2073 656c 662e 696e 6372 656d 656e 7473   self.increments
-0000aec0: 203d 2073 656c 662e 6461 7461 5f77 696e   = self.data_win
-0000aed0: 646f 775b 313a 5d20 2d20 7365 6c66 2e64  dow[1:] - self.d
-0000aee0: 6174 615f 7769 6e64 6f77 5b3a 2d31 5d0a  ata_window[:-1].
-0000aef0: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
-0000af00: 6c61 7265 5f4d 4150 5f73 7461 7274 696e  lare_MAP_startin
-0000af10: 675f 6775 6573 7365 7328 290a 2020 2020  g_guesses().    
-0000af20: 2020 2020 7365 6c66 2e63 6f6d 7075 7465      self.compute
-0000af30: 5f70 6f73 7465 7269 6f72 5f73 616d 706c  _posterior_sampl
-0000af40: 6573 2870 7269 6e74 5f41 435f 7461 753d  es(print_AC_tau=
-0000af50: 7072 696e 745f 4143 5f74 6175 2c20 6967  print_AC_tau, ig
-0000af60: 6e6f 7265 5f41 435f 6572 726f 723d 6967  nore_AC_error=ig
-0000af70: 6e6f 7265 5f41 435f 6572 726f 722c 206e  nore_AC_error, n
-0000af80: 6275 726e 203d 206e 6275 726e 2c0a 2020  burn = nburn,.  
+0000ae90: 2020 2020 2020 2020 2070 6c6f 745f 6465           plot_de
+0000aea0: 7472 656e 6469 6e67 290a 2020 2020 2020  trending).      
+0000aeb0: 2020 7365 6c66 2e69 6e63 7265 6d65 6e74    self.increment
+0000aec0: 7320 3d20 7365 6c66 2e64 6174 615f 7769  s = self.data_wi
+0000aed0: 6e64 6f77 5b31 3a5d 202d 2073 656c 662e  ndow[1:] - self.
+0000aee0: 6461 7461 5f77 696e 646f 775b 3a2d 315d  data_window[:-1]
+0000aef0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+0000af00: 636c 6172 655f 4d41 505f 7374 6172 7469  clare_MAP_starti
+0000af10: 6e67 5f67 7565 7373 6573 2829 0a20 2020  ng_guesses().   
+0000af20: 2020 2020 2073 656c 662e 636f 6d70 7574       self.comput
+0000af30: 655f 706f 7374 6572 696f 725f 7361 6d70  e_posterior_samp
+0000af40: 6c65 7328 7072 696e 745f 4143 5f74 6175  les(print_AC_tau
+0000af50: 3d70 7269 6e74 5f41 435f 7461 752c 2069  =print_AC_tau, i
+0000af60: 676e 6f72 655f 4143 5f65 7272 6f72 3d69  gnore_AC_error=i
+0000af70: 676e 6f72 655f 4143 5f65 7272 6f72 2c0a  gnore_AC_error,.
+0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2074 6869 6e6e 696e 675f 6279       thinning_by
-0000afc0: 3d74 6869 6e6e 696e 675f 6279 2c20 7072  =thinning_by, pr
-0000afd0: 696e 745f 7072 6f67 7265 7373 3d70 7269  int_progress=pri
-0000afe0: 6e74 5f70 726f 6772 6573 732c 0a20 2020  nt_progress,.   
+0000afa0: 2020 2020 2020 2074 6869 6e6e 696e 675f         thinning_
+0000afb0: 6279 3d74 6869 6e6e 696e 675f 6279 2c20  by=thinning_by, 
+0000afc0: 7072 696e 745f 7072 6f67 7265 7373 3d70  print_progress=p
+0000afd0: 7269 6e74 5f70 726f 6772 6573 732c 206e  rint_progress, n
+0000afe0: 6275 726e 203d 206e 6275 726e 2c0a 2020  burn = nburn,.  
 0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b010: 2020 2020 4d43 4d43 5f70 6172 616c 6c65      MCMC_paralle
-0000b020: 6c69 7a61 7469 6f6e 5f6d 6574 686f 643d  lization_method=
-0000b030: 4e6f 6e65 2c20 6e75 6d5f 7072 6f63 6573  None, num_proces
-0000b040: 7365 733d 4e6f 6e65 2c20 6e75 6d5f 6368  ses=None, num_ch
-0000b050: 6f70 5f63 6861 696e 733d 4e6f 6e65 290a  op_chains=None).
-0000b060: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b070: 6472 6966 745f 6d6f 6465 6c20 3d3d 2027  drift_model == '
-0000b080: 3372 6420 6f72 6465 7220 706f 6c79 6e6f  3rd order polyno
-0000b090: 6d69 616c 273a 0a20 2020 2020 2020 2020  mial':.         
-0000b0a0: 2020 2073 656c 662e 6a6f 696e 745f 6b65     self.joint_ke
-0000b0b0: 726e 656c 5f64 656e 7369 7479 5f6f 626a  rnel_density_obj
-0000b0c0: 203d 2063 7079 2e67 6175 7373 6961 6e5f   = cpy.gaussian_
-0000b0d0: 6b64 6528 7365 6c66 2e74 6865 7461 5f61  kde(self.theta_a
-0000b0e0: 7272 6179 2c20 6277 5f6d 6574 686f 643d  rray, bw_method=
-0000b0f0: 2773 696c 7665 726d 616e 2729 0a20 2020  'silverman').   
-0000b100: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0000b110: 696e 745f 7361 6d70 6c65 7320 3d20 7365  int_samples = se
-0000b120: 6c66 2e6a 6f69 6e74 5f6b 6572 6e65 6c5f  lf.joint_kernel_
-0000b130: 6465 6e73 6974 795f 6f62 6a2e 7265 7361  density_obj.resa
-0000b140: 6d70 6c65 2873 697a 653d 6e5f 6a6f 696e  mple(size=n_join
-0000b150: 745f 7361 6d70 6c65 7329 0a20 2020 2020  t_samples).     
-0000b160: 2020 2020 2020 2073 656c 662e 7468 6972         self.thir
-0000b170: 645f 6f72 6465 725f 706f 6c79 6e6f 6d5f  d_order_polynom_
-0000b180: 736c 6f70 655f 696e 5f66 6978 6564 5f70  slope_in_fixed_p
-0000b190: 6f69 6e74 2829 0a20 2020 2020 2020 2020  oint().         
-0000b1a0: 2020 2073 656c 662e 6e6f 6973 655f 6b65     self.noise_ke
-0000b1b0: 726e 656c 5f64 656e 7369 7479 5f6f 626a  rnel_density_obj
-0000b1c0: 203d 2063 7079 2e67 6175 7373 6961 6e5f   = cpy.gaussian_
-0000b1d0: 6b64 6528 7365 6c66 2e74 6865 7461 5f61  kde(self.theta_a
-0000b1e0: 7272 6179 5b34 2c20 3a5d 2c20 6277 5f6d  rray[4, :], bw_m
-0000b1f0: 6574 686f 643d 2773 696c 7665 726d 616e  ethod='silverman
-0000b200: 2729 0a20 2020 2020 2020 2065 6c69 6620  ').        elif 
-0000b210: 7365 6c66 2e64 7269 6674 5f6d 6f64 656c  self.drift_model
-0000b220: 203d 3d20 2766 6972 7374 206f 7264 6572   == 'first order
-0000b230: 2070 6f6c 796e 6f6d 6961 6c27 3a0a 2020   polynomial':.  
-0000b240: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000b250: 6c6f 7065 5f65 7374 696d 6174 6573 203d  lope_estimates =
-0000b260: 2073 656c 662e 7468 6574 615f 6172 7261   self.theta_arra
-0000b270: 795b 3a2c 2031 5d0a 2020 2020 2020 2020  y[:, 1].        
-0000b280: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6b      self.noise_k
-0000b290: 6572 6e65 6c5f 6465 6e73 6974 795f 6f62  ernel_density_ob
-0000b2a0: 6a20 3d20 6370 792e 6761 7573 7369 616e  j = cpy.gaussian
-0000b2b0: 5f6b 6465 2873 656c 662e 7468 6574 615f  _kde(self.theta_
-0000b2c0: 6172 7261 795b 322c 203a 5d2c 2062 775f  array[2, :], bw_
-0000b2d0: 6d65 7468 6f64 3d27 7369 6c76 6572 6d61  method='silverma
-0000b2e0: 6e27 290a 2020 2020 2020 2020 7365 6c66  n').        self
-0000b2f0: 2e73 6c6f 7065 5f6b 6572 6e65 6c5f 6465  .slope_kernel_de
-0000b300: 6e73 6974 795f 6f62 6a20 3d20 6370 792e  nsity_obj = cpy.
-0000b310: 6761 7573 7369 616e 5f6b 6465 2873 656c  gaussian_kde(sel
-0000b320: 662e 736c 6f70 655f 6573 7469 6d61 7465  f.slope_estimate
-0000b330: 732c 2062 775f 6d65 7468 6f64 3d27 7369  s, bw_method='si
-0000b340: 6c76 6572 6d61 6e27 290a 2020 2020 2020  lverman').      
-0000b350: 2020 736c 6f70 655f 7361 6d70 6c65 7320    slope_samples 
-0000b360: 3d20 7365 6c66 2e73 6c6f 7065 5f6b 6572  = self.slope_ker
-0000b370: 6e65 6c5f 6465 6e73 6974 795f 6f62 6a2e  nel_density_obj.
-0000b380: 7265 7361 6d70 6c65 2873 697a 653d 6e5f  resample(size=n_
-0000b390: 736c 6f70 655f 7361 6d70 6c65 7329 0a20  slope_samples). 
-0000b3a0: 2020 2020 2020 206d 6178 5f73 6c6f 7065         max_slope
-0000b3b0: 203d 2073 6c6f 7065 5f67 7269 645b 0a20   = slope_grid[. 
-0000b3c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b3d0: 736c 6f70 655f 6b65 726e 656c 5f64 656e  slope_kernel_den
-0000b3e0: 7369 7479 5f6f 626a 2873 6c6f 7065 5f67  sity_obj(slope_g
-0000b3f0: 7269 6429 203d 3d20 6e70 2e6d 6178 2873  rid) == np.max(s
-0000b400: 656c 662e 736c 6f70 655f 6b65 726e 656c  elf.slope_kernel
-0000b410: 5f64 656e 7369 7479 5f6f 626a 2873 6c6f  _density_obj(slo
-0000b420: 7065 5f67 7269 6429 295d 0a20 2020 2020  pe_grid))].     
-0000b430: 2020 2069 6620 6d61 785f 736c 6f70 652e     if max_slope.
-0000b440: 7369 7a65 203d 3d20 313a 0a20 2020 2020  size == 1:.     
-0000b450: 2020 2020 2020 2073 656c 662e 6472 6966         self.drif
-0000b460: 745f 736c 6f70 655b 305d 203d 206d 6178  t_slope[0] = max
-0000b470: 5f73 6c6f 7065 0a20 2020 2020 2020 2065  _slope.        e
-0000b480: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b490: 2073 656c 662e 6472 6966 745f 736c 6f70   self.drift_slop
-0000b4a0: 655b 305d 203d 206d 6178 5f73 6c6f 7065  e[0] = max_slope
-0000b4b0: 5b30 5d0a 2020 2020 2020 2020 736c 6f70  [0].        slop
-0000b4c0: 655f 6372 6564 6962 696c 6974 795f 7065  e_credibility_pe
-0000b4d0: 7263 656e 7469 6c65 7320 3d20 6e70 2e70  rcentiles = np.p
-0000b4e0: 6572 6365 6e74 696c 6528 736c 6f70 655f  ercentile(slope_
-0000b4f0: 7361 6d70 6c65 732c 205b 6372 6564 5f70  samples, [cred_p
-0000b500: 6572 6365 6e74 696c 6573 5b30 5d2c 2031  ercentiles[0], 1
-0000b510: 3030 202d 2063 7265 645f 7065 7263 656e  00 - cred_percen
-0000b520: 7469 6c65 735b 305d 5d29 0a20 2020 2020  tiles[0]]).     
-0000b530: 2020 2073 656c 662e 6472 6966 745f 736c     self.drift_sl
-0000b540: 6f70 655b 315d 203d 2073 6c6f 7065 5f63  ope[1] = slope_c
-0000b550: 7265 6469 6269 6c69 7479 5f70 6572 6365  redibility_perce
-0000b560: 6e74 696c 6573 5b30 5d0a 2020 2020 2020  ntiles[0].      
-0000b570: 2020 7365 6c66 2e64 7269 6674 5f73 6c6f    self.drift_slo
-0000b580: 7065 5b32 5d20 3d20 736c 6f70 655f 6372  pe[2] = slope_cr
-0000b590: 6564 6962 696c 6974 795f 7065 7263 656e  edibility_percen
-0000b5a0: 7469 6c65 735b 315d 0a20 2020 2020 2020  tiles[1].       
-0000b5b0: 2073 6c6f 7065 5f63 7265 6469 6269 6c69   slope_credibili
-0000b5c0: 7479 5f70 6572 6365 6e74 696c 6573 203d  ty_percentiles =
-0000b5d0: 206e 702e 7065 7263 656e 7469 6c65 2873   np.percentile(s
-0000b5e0: 6c6f 7065 5f73 616d 706c 6573 2c20 5b63  lope_samples, [c
-0000b5f0: 7265 645f 7065 7263 656e 7469 6c65 735b  red_percentiles[
-0000b600: 315d 2c20 3130 3020 2d20 6372 6564 5f70  1], 100 - cred_p
-0000b610: 6572 6365 6e74 696c 6573 5b31 5d5d 290a  ercentiles[1]]).
-0000b620: 2020 2020 2020 2020 7365 6c66 2e64 7269          self.dri
-0000b630: 6674 5f73 6c6f 7065 5b33 5d20 3d20 736c  ft_slope[3] = sl
-0000b640: 6f70 655f 6372 6564 6962 696c 6974 795f  ope_credibility_
-0000b650: 7065 7263 656e 7469 6c65 735b 305d 0a20  percentiles[0]. 
-0000b660: 2020 2020 2020 2073 656c 662e 6472 6966         self.drif
-0000b670: 745f 736c 6f70 655b 345d 203d 2073 6c6f  t_slope[4] = slo
-0000b680: 7065 5f63 7265 6469 6269 6c69 7479 5f70  pe_credibility_p
-0000b690: 6572 6365 6e74 696c 6573 5b31 5d0a 2020  ercentiles[1].  
-0000b6a0: 2020 2020 2020 6e6f 6973 655f 7361 6d70        noise_samp
-0000b6b0: 6c65 7320 3d20 7365 6c66 2e6e 6f69 7365  les = self.noise
-0000b6c0: 5f6b 6572 6e65 6c5f 6465 6e73 6974 795f  _kernel_density_
-0000b6d0: 6f62 6a2e 7265 7361 6d70 6c65 2873 697a  obj.resample(siz
-0000b6e0: 653d 6e5f 6e6f 6973 655f 7361 6d70 6c65  e=n_noise_sample
-0000b6f0: 7329 0a20 2020 2020 2020 206e 6f69 7365  s).        noise
-0000b700: 5f6c 6576 656c 203d 206e 6f69 7365 5f67  _level = noise_g
-0000b710: 7269 645b 0a20 2020 2020 2020 2020 2020  rid[.           
-0000b720: 2073 656c 662e 6e6f 6973 655f 6b65 726e   self.noise_kern
-0000b730: 656c 5f64 656e 7369 7479 5f6f 626a 286e  el_density_obj(n
-0000b740: 6f69 7365 5f67 7269 6429 203d 3d20 6e70  oise_grid) == np
-0000b750: 2e6d 6178 2873 656c 662e 6e6f 6973 655f  .max(self.noise_
-0000b760: 6b65 726e 656c 5f64 656e 7369 7479 5f6f  kernel_density_o
-0000b770: 626a 286e 6f69 7365 5f67 7269 6429 295d  bj(noise_grid))]
-0000b780: 0a20 2020 2020 2020 2069 6620 6e6f 6973  .        if nois
-0000b790: 655f 6c65 7665 6c2e 7369 7a65 203d 3d20  e_level.size == 
-0000b7a0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000b7b0: 656c 662e 6e6f 6973 655f 6c65 7665 6c5f  elf.noise_level_
-0000b7c0: 6573 7469 6d61 7465 5b30 5d20 3d20 6e6f  estimate[0] = no
-0000b7d0: 6973 655f 6c65 7665 6c0a 2020 2020 2020  ise_level.      
-0000b7e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b7f0: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6c      self.noise_l
-0000b800: 6576 656c 5f65 7374 696d 6174 655b 305d  evel_estimate[0]
-0000b810: 203d 206e 6f69 7365 5f6c 6576 656c 5b30   = noise_level[0
-0000b820: 5d0a 2020 2020 2020 2020 6e6f 6973 655f  ].        noise_
-0000b830: 6372 6564 6962 696c 6974 795f 7065 7263  credibility_perc
-0000b840: 656e 7469 6c65 7320 3d20 6e70 2e70 6572  entiles = np.per
-0000b850: 6365 6e74 696c 6528 6e6f 6973 655f 7361  centile(noise_sa
-0000b860: 6d70 6c65 732c 205b 6372 6564 5f70 6572  mples, [cred_per
-0000b870: 6365 6e74 696c 6573 5b30 5d2c 2031 3030  centiles[0], 100
-0000b880: 202d 2063 7265 645f 7065 7263 656e 7469   - cred_percenti
-0000b890: 6c65 735b 305d 5d29 0a20 2020 2020 2020  les[0]]).       
-0000b8a0: 2073 656c 662e 6e6f 6973 655f 6c65 7665   self.noise_leve
-0000b8b0: 6c5f 6573 7469 6d61 7465 5b31 5d20 3d20  l_estimate[1] = 
-0000b8c0: 6e6f 6973 655f 6372 6564 6962 696c 6974  noise_credibilit
-0000b8d0: 795f 7065 7263 656e 7469 6c65 735b 305d  y_percentiles[0]
-0000b8e0: 0a20 2020 2020 2020 2073 656c 662e 6e6f  .        self.no
-0000b8f0: 6973 655f 6c65 7665 6c5f 6573 7469 6d61  ise_level_estima
-0000b900: 7465 5b32 5d20 3d20 6e6f 6973 655f 6372  te[2] = noise_cr
-0000b910: 6564 6962 696c 6974 795f 7065 7263 656e  edibility_percen
-0000b920: 7469 6c65 735b 315d 0a20 2020 2020 2020  tiles[1].       
-0000b930: 206e 6f69 7365 5f63 7265 6469 6269 6c69   noise_credibili
-0000b940: 7479 5f70 6572 6365 6e74 696c 6573 203d  ty_percentiles =
-0000b950: 206e 702e 7065 7263 656e 7469 6c65 286e   np.percentile(n
-0000b960: 6f69 7365 5f73 616d 706c 6573 2c20 5b63  oise_samples, [c
-0000b970: 7265 645f 7065 7263 656e 7469 6c65 735b  red_percentiles[
-0000b980: 315d 2c20 3130 3020 2d20 6372 6564 5f70  1], 100 - cred_p
-0000b990: 6572 6365 6e74 696c 6573 5b31 5d5d 290a  ercentiles[1]]).
-0000b9a0: 2020 2020 2020 2020 7365 6c66 2e6e 6f69          self.noi
-0000b9b0: 7365 5f6c 6576 656c 5f65 7374 696d 6174  se_level_estimat
-0000b9c0: 655b 335d 203d 206e 6f69 7365 5f63 7265  e[3] = noise_cre
-0000b9d0: 6469 6269 6c69 7479 5f70 6572 6365 6e74  dibility_percent
-0000b9e0: 696c 6573 5b30 5d0a 2020 2020 2020 2020  iles[0].        
-0000b9f0: 7365 6c66 2e6e 6f69 7365 5f6c 6576 656c  self.noise_level
-0000ba00: 5f65 7374 696d 6174 655b 345d 203d 206e  _estimate[4] = n
-0000ba10: 6f69 7365 5f63 7265 6469 6269 6c69 7479  oise_credibility
-0000ba20: 5f70 6572 6365 6e74 696c 6573 5b31 5d0a  _percentiles[1].
-0000ba30: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0000ba40: 6f64 0a20 2020 2064 6566 2069 6e69 745f  od.    def init_
-0000ba50: 7061 7261 6c6c 656c 5f45 6e73 656d 626c  parallel_Ensembl
-0000ba60: 6553 616d 706c 6572 2864 6174 615f 7769  eSampler(data_wi
-0000ba70: 6e64 6f77 2c20 6474 2c20 6472 6966 745f  ndow, dt, drift_
-0000ba80: 6d6f 6465 6c2c 2064 6966 6675 7369 6f6e  model, diffusion
-0000ba90: 5f6d 6f64 656c 2c20 7072 696f 725f 7479  _model, prior_ty
-0000baa0: 7065 2c20 7072 696f 725f 7261 6e67 652c  pe, prior_range,
-0000bab0: 2073 6361 6c65 7329 3a0a 2020 2020 2020   scales):.      
-0000bac0: 2020 676c 6f62 616c 2073 6861 7265 645f    global shared_
-0000bad0: 6d65 6d6f 7279 5f64 6963 740a 2020 2020  memory_dict.    
-0000bae0: 2020 2020 7368 6172 6564 5f6d 656d 6f72      shared_memor
-0000baf0: 795f 6469 6374 203d 207b 7d0a 2020 2020  y_dict = {}.    
-0000bb00: 2020 2020 7368 6172 6564 5f6d 656d 6f72      shared_memor
-0000bb10: 795f 6469 6374 5b27 6461 7461 5f77 696e  y_dict['data_win
-0000bb20: 646f 7727 5d20 3d20 6461 7461 5f77 696e  dow'] = data_win
-0000bb30: 646f 770a 2020 2020 2020 2020 7368 6172  dow.        shar
-0000bb40: 6564 5f6d 656d 6f72 795f 6469 6374 5b27  ed_memory_dict['
-0000bb50: 6474 275d 203d 2064 740a 2020 2020 2020  dt'] = dt.      
-0000bb60: 2020 7368 6172 6564 5f6d 656d 6f72 795f    shared_memory_
-0000bb70: 6469 6374 5b27 6472 6966 745f 6d6f 6465  dict['drift_mode
-0000bb80: 6c27 5d20 3d20 6472 6966 745f 6d6f 6465  l'] = drift_mode
-0000bb90: 6c0a 2020 2020 2020 2020 7368 6172 6564  l.        shared
-0000bba0: 5f6d 656d 6f72 795f 6469 6374 5b27 6469  _memory_dict['di
-0000bbb0: 6666 7573 696f 6e5f 6d6f 6465 6c27 5d20  ffusion_model'] 
-0000bbc0: 3d20 6469 6666 7573 696f 6e5f 6d6f 6465  = diffusion_mode
-0000bbd0: 6c0a 2020 2020 2020 2020 7368 6172 6564  l.        shared
-0000bbe0: 5f6d 656d 6f72 795f 6469 6374 5b27 7072  _memory_dict['pr
-0000bbf0: 696f 725f 7479 7065 275d 203d 2070 7269  ior_type'] = pri
-0000bc00: 6f72 5f74 7970 650a 2020 2020 2020 2020  or_type.        
-0000bc10: 7368 6172 6564 5f6d 656d 6f72 795f 6469  shared_memory_di
-0000bc20: 6374 5b27 7072 696f 725f 7261 6e67 6527  ct['prior_range'
-0000bc30: 5d20 3d20 7072 696f 725f 7261 6e67 650a  ] = prior_range.
-0000bc40: 2020 2020 2020 2020 7368 6172 6564 5f6d          shared_m
-0000bc50: 656d 6f72 795f 6469 6374 5b27 7363 616c  emory_dict['scal
-0000bc60: 6573 275d 203d 2073 6361 6c65 730a 0a20  es'] = scales.. 
-0000bc70: 2020 2064 6566 2070 6572 666f 726d 5f72     def perform_r
-0000bc80: 6573 696c 6965 6e63 655f 7363 616e 2873  esilience_scan(s
-0000bc90: 656c 662c 2077 696e 646f 775f 7369 7a65  elf, window_size
-0000bca0: 2c20 7769 6e64 6f77 5f73 6869 6674 2c20  , window_shift, 
-0000bcb0: 736c 6f70 655f 6772 6964 2c20 6e6f 6973  slope_grid, nois
-0000bcc0: 655f 6772 6964 2c0a 2020 2020 2020 2020  e_grid,.        
+0000b010: 2020 2020 204d 434d 435f 7061 7261 6c6c       MCMC_parall
+0000b020: 656c 697a 6174 696f 6e5f 6d65 7468 6f64  elization_method
+0000b030: 3d4e 6f6e 652c 206e 756d 5f70 726f 6365  =None, num_proce
+0000b040: 7373 6573 3d4e 6f6e 652c 206e 756d 5f63  sses=None, num_c
+0000b050: 686f 705f 6368 6169 6e73 3d4e 6f6e 6529  hop_chains=None)
+0000b060: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b070: 2e64 7269 6674 5f6d 6f64 656c 203d 3d20  .drift_model == 
+0000b080: 2733 7264 206f 7264 6572 2070 6f6c 796e  '3rd order polyn
+0000b090: 6f6d 6961 6c27 3a0a 2020 2020 2020 2020  omial':.        
+0000b0a0: 2020 2020 7365 6c66 2e6a 6f69 6e74 5f6b      self.joint_k
+0000b0b0: 6572 6e65 6c5f 6465 6e73 6974 795f 6f62  ernel_density_ob
+0000b0c0: 6a20 3d20 6370 792e 6761 7573 7369 616e  j = cpy.gaussian
+0000b0d0: 5f6b 6465 2873 656c 662e 7468 6574 615f  _kde(self.theta_
+0000b0e0: 6172 7261 792c 2062 775f 6d65 7468 6f64  array, bw_method
+0000b0f0: 3d27 7369 6c76 6572 6d61 6e27 290a 2020  ='silverman').  
+0000b100: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+0000b110: 6f69 6e74 5f73 616d 706c 6573 203d 2073  oint_samples = s
+0000b120: 656c 662e 6a6f 696e 745f 6b65 726e 656c  elf.joint_kernel
+0000b130: 5f64 656e 7369 7479 5f6f 626a 2e72 6573  _density_obj.res
+0000b140: 616d 706c 6528 7369 7a65 3d6e 5f6a 6f69  ample(size=n_joi
+0000b150: 6e74 5f73 616d 706c 6573 290a 2020 2020  nt_samples).    
+0000b160: 2020 2020 2020 2020 7365 6c66 2e74 6869          self.thi
+0000b170: 7264 5f6f 7264 6572 5f70 6f6c 796e 6f6d  rd_order_polynom
+0000b180: 5f73 6c6f 7065 5f69 6e5f 6669 7865 645f  _slope_in_fixed_
+0000b190: 706f 696e 7428 290a 2020 2020 2020 2020  point().        
+0000b1a0: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6b      self.noise_k
+0000b1b0: 6572 6e65 6c5f 6465 6e73 6974 795f 6f62  ernel_density_ob
+0000b1c0: 6a20 3d20 6370 792e 6761 7573 7369 616e  j = cpy.gaussian
+0000b1d0: 5f6b 6465 2873 656c 662e 7468 6574 615f  _kde(self.theta_
+0000b1e0: 6172 7261 795b 342c 203a 5d2c 2062 775f  array[4, :], bw_
+0000b1f0: 6d65 7468 6f64 3d27 7369 6c76 6572 6d61  method='silverma
+0000b200: 6e27 290a 2020 2020 2020 2020 656c 6966  n').        elif
+0000b210: 2073 656c 662e 6472 6966 745f 6d6f 6465   self.drift_mode
+0000b220: 6c20 3d3d 2027 6669 7273 7420 6f72 6465  l == 'first orde
+0000b230: 7220 706f 6c79 6e6f 6d69 616c 273a 0a20  r polynomial':. 
+0000b240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b250: 736c 6f70 655f 6573 7469 6d61 7465 7320  slope_estimates 
+0000b260: 3d20 7365 6c66 2e74 6865 7461 5f61 7272  = self.theta_arr
+0000b270: 6179 5b3a 2c20 315d 0a20 2020 2020 2020  ay[:, 1].       
+0000b280: 2020 2020 2073 656c 662e 6e6f 6973 655f       self.noise_
+0000b290: 6b65 726e 656c 5f64 656e 7369 7479 5f6f  kernel_density_o
+0000b2a0: 626a 203d 2063 7079 2e67 6175 7373 6961  bj = cpy.gaussia
+0000b2b0: 6e5f 6b64 6528 7365 6c66 2e74 6865 7461  n_kde(self.theta
+0000b2c0: 5f61 7272 6179 5b32 2c20 3a5d 2c20 6277  _array[2, :], bw
+0000b2d0: 5f6d 6574 686f 643d 2773 696c 7665 726d  _method='silverm
+0000b2e0: 616e 2729 0a20 2020 2020 2020 2073 656c  an').        sel
+0000b2f0: 662e 736c 6f70 655f 6b65 726e 656c 5f64  f.slope_kernel_d
+0000b300: 656e 7369 7479 5f6f 626a 203d 2063 7079  ensity_obj = cpy
+0000b310: 2e67 6175 7373 6961 6e5f 6b64 6528 7365  .gaussian_kde(se
+0000b320: 6c66 2e73 6c6f 7065 5f65 7374 696d 6174  lf.slope_estimat
+0000b330: 6573 2c20 6277 5f6d 6574 686f 643d 2773  es, bw_method='s
+0000b340: 696c 7665 726d 616e 2729 0a20 2020 2020  ilverman').     
+0000b350: 2020 2073 6c6f 7065 5f73 616d 706c 6573     slope_samples
+0000b360: 203d 2073 656c 662e 736c 6f70 655f 6b65   = self.slope_ke
+0000b370: 726e 656c 5f64 656e 7369 7479 5f6f 626a  rnel_density_obj
+0000b380: 2e72 6573 616d 706c 6528 7369 7a65 3d6e  .resample(size=n
+0000b390: 5f73 6c6f 7065 5f73 616d 706c 6573 290a  _slope_samples).
+0000b3a0: 2020 2020 2020 2020 6d61 785f 736c 6f70          max_slop
+0000b3b0: 6520 3d20 736c 6f70 655f 6772 6964 5b0a  e = slope_grid[.
+0000b3c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b3d0: 2e73 6c6f 7065 5f6b 6572 6e65 6c5f 6465  .slope_kernel_de
+0000b3e0: 6e73 6974 795f 6f62 6a28 736c 6f70 655f  nsity_obj(slope_
+0000b3f0: 6772 6964 2920 3d3d 206e 702e 6d61 7828  grid) == np.max(
+0000b400: 7365 6c66 2e73 6c6f 7065 5f6b 6572 6e65  self.slope_kerne
+0000b410: 6c5f 6465 6e73 6974 795f 6f62 6a28 736c  l_density_obj(sl
+0000b420: 6f70 655f 6772 6964 2929 5d0a 2020 2020  ope_grid))].    
+0000b430: 2020 2020 6966 206d 6178 5f73 6c6f 7065      if max_slope
+0000b440: 2e73 697a 6520 3d3d 2031 3a0a 2020 2020  .size == 1:.    
+0000b450: 2020 2020 2020 2020 7365 6c66 2e64 7269          self.dri
+0000b460: 6674 5f73 6c6f 7065 5b30 5d20 3d20 6d61  ft_slope[0] = ma
+0000b470: 785f 736c 6f70 650a 2020 2020 2020 2020  x_slope.        
+0000b480: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b490: 2020 7365 6c66 2e64 7269 6674 5f73 6c6f    self.drift_slo
+0000b4a0: 7065 5b30 5d20 3d20 6d61 785f 736c 6f70  pe[0] = max_slop
+0000b4b0: 655b 305d 0a20 2020 2020 2020 2073 6c6f  e[0].        slo
+0000b4c0: 7065 5f63 7265 6469 6269 6c69 7479 5f70  pe_credibility_p
+0000b4d0: 6572 6365 6e74 696c 6573 203d 206e 702e  ercentiles = np.
+0000b4e0: 7065 7263 656e 7469 6c65 2873 6c6f 7065  percentile(slope
+0000b4f0: 5f73 616d 706c 6573 2c20 5b63 7265 645f  _samples, [cred_
+0000b500: 7065 7263 656e 7469 6c65 735b 305d 2c20  percentiles[0], 
+0000b510: 3130 3020 2d20 6372 6564 5f70 6572 6365  100 - cred_perce
+0000b520: 6e74 696c 6573 5b30 5d5d 290a 2020 2020  ntiles[0]]).    
+0000b530: 2020 2020 7365 6c66 2e64 7269 6674 5f73      self.drift_s
+0000b540: 6c6f 7065 5b31 5d20 3d20 736c 6f70 655f  lope[1] = slope_
+0000b550: 6372 6564 6962 696c 6974 795f 7065 7263  credibility_perc
+0000b560: 656e 7469 6c65 735b 305d 0a20 2020 2020  entiles[0].     
+0000b570: 2020 2073 656c 662e 6472 6966 745f 736c     self.drift_sl
+0000b580: 6f70 655b 325d 203d 2073 6c6f 7065 5f63  ope[2] = slope_c
+0000b590: 7265 6469 6269 6c69 7479 5f70 6572 6365  redibility_perce
+0000b5a0: 6e74 696c 6573 5b31 5d0a 2020 2020 2020  ntiles[1].      
+0000b5b0: 2020 736c 6f70 655f 6372 6564 6962 696c    slope_credibil
+0000b5c0: 6974 795f 7065 7263 656e 7469 6c65 7320  ity_percentiles 
+0000b5d0: 3d20 6e70 2e70 6572 6365 6e74 696c 6528  = np.percentile(
+0000b5e0: 736c 6f70 655f 7361 6d70 6c65 732c 205b  slope_samples, [
+0000b5f0: 6372 6564 5f70 6572 6365 6e74 696c 6573  cred_percentiles
+0000b600: 5b31 5d2c 2031 3030 202d 2063 7265 645f  [1], 100 - cred_
+0000b610: 7065 7263 656e 7469 6c65 735b 315d 5d29  percentiles[1]])
+0000b620: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+0000b630: 6966 745f 736c 6f70 655b 335d 203d 2073  ift_slope[3] = s
+0000b640: 6c6f 7065 5f63 7265 6469 6269 6c69 7479  lope_credibility
+0000b650: 5f70 6572 6365 6e74 696c 6573 5b30 5d0a  _percentiles[0].
+0000b660: 2020 2020 2020 2020 7365 6c66 2e64 7269          self.dri
+0000b670: 6674 5f73 6c6f 7065 5b34 5d20 3d20 736c  ft_slope[4] = sl
+0000b680: 6f70 655f 6372 6564 6962 696c 6974 795f  ope_credibility_
+0000b690: 7065 7263 656e 7469 6c65 735b 315d 0a20  percentiles[1]. 
+0000b6a0: 2020 2020 2020 206e 6f69 7365 5f73 616d         noise_sam
+0000b6b0: 706c 6573 203d 2073 656c 662e 6e6f 6973  ples = self.nois
+0000b6c0: 655f 6b65 726e 656c 5f64 656e 7369 7479  e_kernel_density
+0000b6d0: 5f6f 626a 2e72 6573 616d 706c 6528 7369  _obj.resample(si
+0000b6e0: 7a65 3d6e 5f6e 6f69 7365 5f73 616d 706c  ze=n_noise_sampl
+0000b6f0: 6573 290a 2020 2020 2020 2020 6e6f 6973  es).        nois
+0000b700: 655f 6c65 7665 6c20 3d20 6e6f 6973 655f  e_level = noise_
+0000b710: 6772 6964 5b0a 2020 2020 2020 2020 2020  grid[.          
+0000b720: 2020 7365 6c66 2e6e 6f69 7365 5f6b 6572    self.noise_ker
+0000b730: 6e65 6c5f 6465 6e73 6974 795f 6f62 6a28  nel_density_obj(
+0000b740: 6e6f 6973 655f 6772 6964 2920 3d3d 206e  noise_grid) == n
+0000b750: 702e 6d61 7828 7365 6c66 2e6e 6f69 7365  p.max(self.noise
+0000b760: 5f6b 6572 6e65 6c5f 6465 6e73 6974 795f  _kernel_density_
+0000b770: 6f62 6a28 6e6f 6973 655f 6772 6964 2929  obj(noise_grid))
+0000b780: 5d0a 2020 2020 2020 2020 6966 206e 6f69  ].        if noi
+0000b790: 7365 5f6c 6576 656c 2e73 697a 6520 3d3d  se_level.size ==
+0000b7a0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000b7b0: 7365 6c66 2e6e 6f69 7365 5f6c 6576 656c  self.noise_level
+0000b7c0: 5f65 7374 696d 6174 655b 305d 203d 206e  _estimate[0] = n
+0000b7d0: 6f69 7365 5f6c 6576 656c 0a20 2020 2020  oise_level.     
+0000b7e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b7f0: 2020 2020 2073 656c 662e 6e6f 6973 655f       self.noise_
+0000b800: 6c65 7665 6c5f 6573 7469 6d61 7465 5b30  level_estimate[0
+0000b810: 5d20 3d20 6e6f 6973 655f 6c65 7665 6c5b  ] = noise_level[
+0000b820: 305d 0a20 2020 2020 2020 206e 6f69 7365  0].        noise
+0000b830: 5f63 7265 6469 6269 6c69 7479 5f70 6572  _credibility_per
+0000b840: 6365 6e74 696c 6573 203d 206e 702e 7065  centiles = np.pe
+0000b850: 7263 656e 7469 6c65 286e 6f69 7365 5f73  rcentile(noise_s
+0000b860: 616d 706c 6573 2c20 5b63 7265 645f 7065  amples, [cred_pe
+0000b870: 7263 656e 7469 6c65 735b 305d 2c20 3130  rcentiles[0], 10
+0000b880: 3020 2d20 6372 6564 5f70 6572 6365 6e74  0 - cred_percent
+0000b890: 696c 6573 5b30 5d5d 290a 2020 2020 2020  iles[0]]).      
+0000b8a0: 2020 7365 6c66 2e6e 6f69 7365 5f6c 6576    self.noise_lev
+0000b8b0: 656c 5f65 7374 696d 6174 655b 315d 203d  el_estimate[1] =
+0000b8c0: 206e 6f69 7365 5f63 7265 6469 6269 6c69   noise_credibili
+0000b8d0: 7479 5f70 6572 6365 6e74 696c 6573 5b30  ty_percentiles[0
+0000b8e0: 5d0a 2020 2020 2020 2020 7365 6c66 2e6e  ].        self.n
+0000b8f0: 6f69 7365 5f6c 6576 656c 5f65 7374 696d  oise_level_estim
+0000b900: 6174 655b 325d 203d 206e 6f69 7365 5f63  ate[2] = noise_c
+0000b910: 7265 6469 6269 6c69 7479 5f70 6572 6365  redibility_perce
+0000b920: 6e74 696c 6573 5b31 5d0a 2020 2020 2020  ntiles[1].      
+0000b930: 2020 6e6f 6973 655f 6372 6564 6962 696c    noise_credibil
+0000b940: 6974 795f 7065 7263 656e 7469 6c65 7320  ity_percentiles 
+0000b950: 3d20 6e70 2e70 6572 6365 6e74 696c 6528  = np.percentile(
+0000b960: 6e6f 6973 655f 7361 6d70 6c65 732c 205b  noise_samples, [
+0000b970: 6372 6564 5f70 6572 6365 6e74 696c 6573  cred_percentiles
+0000b980: 5b31 5d2c 2031 3030 202d 2063 7265 645f  [1], 100 - cred_
+0000b990: 7065 7263 656e 7469 6c65 735b 315d 5d29  percentiles[1]])
+0000b9a0: 0a20 2020 2020 2020 2073 656c 662e 6e6f  .        self.no
+0000b9b0: 6973 655f 6c65 7665 6c5f 6573 7469 6d61  ise_level_estima
+0000b9c0: 7465 5b33 5d20 3d20 6e6f 6973 655f 6372  te[3] = noise_cr
+0000b9d0: 6564 6962 696c 6974 795f 7065 7263 656e  edibility_percen
+0000b9e0: 7469 6c65 735b 305d 0a20 2020 2020 2020  tiles[0].       
+0000b9f0: 2073 656c 662e 6e6f 6973 655f 6c65 7665   self.noise_leve
+0000ba00: 6c5f 6573 7469 6d61 7465 5b34 5d20 3d20  l_estimate[4] = 
+0000ba10: 6e6f 6973 655f 6372 6564 6962 696c 6974  noise_credibilit
+0000ba20: 795f 7065 7263 656e 7469 6c65 735b 315d  y_percentiles[1]
+0000ba30: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+0000ba40: 686f 640a 2020 2020 6465 6620 696e 6974  hod.    def init
+0000ba50: 5f70 6172 616c 6c65 6c5f 456e 7365 6d62  _parallel_Ensemb
+0000ba60: 6c65 5361 6d70 6c65 7228 6461 7461 5f77  leSampler(data_w
+0000ba70: 696e 646f 772c 2064 742c 2064 7269 6674  indow, dt, drift
+0000ba80: 5f6d 6f64 656c 2c20 6469 6666 7573 696f  _model, diffusio
+0000ba90: 6e5f 6d6f 6465 6c2c 2070 7269 6f72 5f74  n_model, prior_t
+0000baa0: 7970 652c 2070 7269 6f72 5f72 616e 6765  ype, prior_range
+0000bab0: 2c20 7363 616c 6573 293a 0a20 2020 2020  , scales):.     
+0000bac0: 2020 2067 6c6f 6261 6c20 7368 6172 6564     global shared
+0000bad0: 5f6d 656d 6f72 795f 6469 6374 0a20 2020  _memory_dict.   
+0000bae0: 2020 2020 2073 6861 7265 645f 6d65 6d6f       shared_memo
+0000baf0: 7279 5f64 6963 7420 3d20 7b7d 0a20 2020  ry_dict = {}.   
+0000bb00: 2020 2020 2073 6861 7265 645f 6d65 6d6f       shared_memo
+0000bb10: 7279 5f64 6963 745b 2764 6174 615f 7769  ry_dict['data_wi
+0000bb20: 6e64 6f77 275d 203d 2064 6174 615f 7769  ndow'] = data_wi
+0000bb30: 6e64 6f77 0a20 2020 2020 2020 2073 6861  ndow.        sha
+0000bb40: 7265 645f 6d65 6d6f 7279 5f64 6963 745b  red_memory_dict[
+0000bb50: 2764 7427 5d20 3d20 6474 0a20 2020 2020  'dt'] = dt.     
+0000bb60: 2020 2073 6861 7265 645f 6d65 6d6f 7279     shared_memory
+0000bb70: 5f64 6963 745b 2764 7269 6674 5f6d 6f64  _dict['drift_mod
+0000bb80: 656c 275d 203d 2064 7269 6674 5f6d 6f64  el'] = drift_mod
+0000bb90: 656c 0a20 2020 2020 2020 2073 6861 7265  el.        share
+0000bba0: 645f 6d65 6d6f 7279 5f64 6963 745b 2764  d_memory_dict['d
+0000bbb0: 6966 6675 7369 6f6e 5f6d 6f64 656c 275d  iffusion_model']
+0000bbc0: 203d 2064 6966 6675 7369 6f6e 5f6d 6f64   = diffusion_mod
+0000bbd0: 656c 0a20 2020 2020 2020 2073 6861 7265  el.        share
+0000bbe0: 645f 6d65 6d6f 7279 5f64 6963 745b 2770  d_memory_dict['p
+0000bbf0: 7269 6f72 5f74 7970 6527 5d20 3d20 7072  rior_type'] = pr
+0000bc00: 696f 725f 7479 7065 0a20 2020 2020 2020  ior_type.       
+0000bc10: 2073 6861 7265 645f 6d65 6d6f 7279 5f64   shared_memory_d
+0000bc20: 6963 745b 2770 7269 6f72 5f72 616e 6765  ict['prior_range
+0000bc30: 275d 203d 2070 7269 6f72 5f72 616e 6765  '] = prior_range
+0000bc40: 0a20 2020 2020 2020 2073 6861 7265 645f  .        shared_
+0000bc50: 6d65 6d6f 7279 5f64 6963 745b 2773 6361  memory_dict['sca
+0000bc60: 6c65 7327 5d20 3d20 7363 616c 6573 0a0a  les'] = scales..
+0000bc70: 2020 2020 6465 6620 7065 7266 6f72 6d5f      def perform_
+0000bc80: 7265 7369 6c69 656e 6365 5f73 6361 6e28  resilience_scan(
+0000bc90: 7365 6c66 2c20 7769 6e64 6f77 5f73 697a  self, window_siz
+0000bca0: 652c 2077 696e 646f 775f 7368 6966 742c  e, window_shift,
+0000bcb0: 2073 6c6f 7065 5f67 7269 642c 206e 6f69   slope_grid, noi
+0000bcc0: 7365 5f67 7269 642c 0a20 2020 2020 2020  se_grid,.       
 0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcf0: 2020 2020 206e 7761 6c6b 6572 733d 3530       nwalkers=50
-0000bd00: 2c20 6e73 7465 7073 3d31 3030 3030 2c20  , nsteps=10000, 
-0000bd10: 6e62 7572 6e3d 3230 302c 206e 5f6a 6f69  nburn=200, n_joi
-0000bd20: 6e74 5f73 616d 706c 6573 3d35 3030 3030  nt_samples=50000
-0000bd30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bcf0: 2020 2020 2020 6e77 616c 6b65 7273 3d35        nwalkers=5
+0000bd00: 302c 206e 7374 6570 733d 3130 3030 302c  0, nsteps=10000,
+0000bd10: 206e 6275 726e 3d32 3030 2c20 6e5f 6a6f   nburn=200, n_jo
+0000bd20: 696e 745f 7361 6d70 6c65 733d 3530 3030  int_samples=5000
+0000bd30: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
 0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000bd60: 5f73 6c6f 7065 5f73 616d 706c 6573 3d35  _slope_samples=5
-0000bd70: 3030 3030 2c20 6e5f 6e6f 6973 655f 7361  0000, n_noise_sa
-0000bd80: 6d70 6c65 733d 3530 3030 302c 0a20 2020  mples=50000,.   
+0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd60: 6e5f 736c 6f70 655f 7361 6d70 6c65 733d  n_slope_samples=
+0000bd70: 3530 3030 302c 206e 5f6e 6f69 7365 5f73  50000, n_noise_s
+0000bd80: 616d 706c 6573 3d35 3030 3030 2c0a 2020  amples=50000,.  
 0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 2020 2020 2020 6372 6564 5f70            cred_p
-0000bdc0: 6572 6365 6e74 696c 6573 3d5b 3136 2c20  ercentiles=[16, 
-0000bdd0: 315d 2c20 7072 696e 745f 4143 5f74 6175  1], print_AC_tau
-0000bde0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000bdb0: 2020 2020 2020 2020 2020 2063 7265 645f             cred_
+0000bdc0: 7065 7263 656e 7469 6c65 733d 5b31 362c  percentiles=[16,
+0000bdd0: 2031 5d2c 2070 7269 6e74 5f41 435f 7461   1], print_AC_ta
+0000bde0: 753d 4661 6c73 652c 0a20 2020 2020 2020  u=False,.       
 0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 2020 2020 2069 676e 6f72 655f 4143 5f65       ignore_AC_e
-0000be20: 7272 6f72 3d46 616c 7365 2c20 7468 696e  rror=False, thin
-0000be30: 6e69 6e67 5f62 793d 3630 2c20 7072 696e  ning_by=60, prin
-0000be40: 745f 7072 6f67 7265 7373 3d46 616c 7365  t_progress=False
-0000be50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000be10: 2020 2020 2020 6967 6e6f 7265 5f41 435f        ignore_AC_
+0000be20: 6572 726f 723d 4661 6c73 652c 2074 6869  error=False, thi
+0000be30: 6e6e 696e 675f 6279 3d36 302c 2070 7269  nning_by=60, pri
+0000be40: 6e74 5f70 726f 6772 6573 733d 4661 6c73  nt_progress=Fals
+0000be50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
 0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000be80: 6c6f 7065 5f73 6176 655f 6e61 6d65 3d27  lope_save_name='
-0000be90: 6465 6661 756c 745f 7361 7665 5f73 6c6f  default_save_slo
-0000bea0: 7065 7327 2c0a 2020 2020 2020 2020 2020  pes',.          
+0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be80: 736c 6f70 655f 7361 7665 5f6e 616d 653d  slope_save_name=
+0000be90: 2764 6566 6175 6c74 5f73 6176 655f 736c  'default_save_sl
+0000bea0: 6f70 6573 272c 0a20 2020 2020 2020 2020  opes',.         
 0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 2020 206e 6f69 7365 5f6c 6576 656c 5f73     noise_level_s
-0000bee0: 6176 655f 6e61 6d65 3d27 6465 6661 756c  ave_name='defaul
-0000bef0: 745f 7361 7665 5f6e 6f69 7365 272c 2073  t_save_noise', s
-0000bf00: 6176 653d 5472 7565 2c0a 2020 2020 2020  ave=True,.      
+0000bed0: 2020 2020 6e6f 6973 655f 6c65 7665 6c5f      noise_level_
+0000bee0: 7361 7665 5f6e 616d 653d 2764 6566 6175  save_name='defau
+0000bef0: 6c74 5f73 6176 655f 6e6f 6973 6527 2c20  lt_save_noise', 
+0000bf00: 7361 7665 3d54 7275 652c 0a20 2020 2020  save=True,.     
 0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2020 2020 2020 2063 7265 6174 655f 616e         create_an
-0000bf40: 696d 6174 696f 6e3d 4661 6c73 652c 2061  imation=False, a
-0000bf50: 6e69 5f73 6176 655f 6e61 6d65 3d27 6465  ni_save_name='de
-0000bf60: 6661 756c 745f 616e 696d 6174 696f 6e5f  fault_animation_
-0000bf70: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
+0000bf30: 2020 2020 2020 2020 6372 6561 7465 5f61          create_a
+0000bf40: 6e69 6d61 7469 6f6e 3d46 616c 7365 2c20  nimation=False, 
+0000bf50: 616e 695f 7361 7665 5f6e 616d 653d 2764  ani_save_name='d
+0000bf60: 6566 6175 6c74 5f61 6e69 6d61 7469 6f6e  efault_animation
+0000bf70: 5f6e 616d 6527 2c0a 2020 2020 2020 2020  _name',.        
 0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2020 616e 696d 6174 696f 6e5f 7469      animation_ti
-0000bfb0: 746c 653d 2727 2c20 6d61 726b 5f63 7269  tle='', mark_cri
-0000bfc0: 7469 6361 6c5f 706f 696e 743d 4e6f 6e65  tical_point=None
-0000bfd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bfa0: 2020 2020 2061 6e69 6d61 7469 6f6e 5f74       animation_t
+0000bfb0: 6974 6c65 3d27 272c 206d 6172 6b5f 6372  itle='', mark_cr
+0000bfc0: 6974 6963 616c 5f70 6f69 6e74 3d4e 6f6e  itical_point=Non
+0000bfd0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
 0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000c000: 6172 6b5f 6e6f 6973 655f 6c65 7665 6c3d  ark_noise_level=
-0000c010: 4e6f 6e65 2c20 6465 7472 656e 6469 6e67  None, detrending
-0000c020: 5f70 6572 5f77 696e 646f 7720 3d20 4e6f  _per_window = No
-0000c030: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c000: 6d61 726b 5f6e 6f69 7365 5f6c 6576 656c  mark_noise_level
+0000c010: 3d4e 6f6e 652c 2064 6574 7265 6e64 696e  =None, detrendin
+0000c020: 675f 7065 725f 7769 6e64 6f77 203d 204e  g_per_window = N
+0000c030: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
 0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2067 6175 7373 5f66 696c 7465 725f 6d6f   gauss_filter_mo
-0000c070: 6465 203d 2027 7265 666c 6563 7427 2c67  de = 'reflect',g
-0000c080: 6175 7373 5f66 696c 7465 725f 7369 676d  auss_filter_sigm
-0000c090: 6120 3d20 362c 0a20 2020 2020 2020 2020  a = 6,.         
+0000c060: 2020 6761 7573 735f 6669 6c74 6572 5f6d    gauss_filter_m
+0000c070: 6f64 6520 3d20 2772 6566 6c65 6374 272c  ode = 'reflect',
+0000c080: 6761 7573 735f 6669 6c74 6572 5f73 6967  gauss_filter_sig
+0000c090: 6d61 203d 2036 2c0a 2020 2020 2020 2020  ma = 6,.        
 0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 6761 7573 735f 6669 6c74 6572      gauss_filter
-0000c0d0: 5f6f 7264 6572 203d 2030 2c20 6761 7573  _order = 0, gaus
-0000c0e0: 735f 6669 6c74 6572 5f63 7661 6c20 3d20  s_filter_cval = 
-0000c0f0: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+0000c0c0: 2020 2020 2067 6175 7373 5f66 696c 7465       gauss_filte
+0000c0d0: 725f 6f72 6465 7220 3d20 302c 2067 6175  r_order = 0, gau
+0000c0e0: 7373 5f66 696c 7465 725f 6376 616c 203d  ss_filter_cval =
+0000c0f0: 2030 2e30 2c0a 2020 2020 2020 2020 2020   0.0,.          
 0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 2020 6761 7573 735f 6669 6c74 6572 5f74    gauss_filter_t
-0000c130: 7275 6e63 6174 6520 3d20 342e 302c 2070  runcate = 4.0, p
-0000c140: 6c6f 745f 6465 7472 656e 6469 6e67 203d  lot_detrending =
-0000c150: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000c120: 2020 2067 6175 7373 5f66 696c 7465 725f     gauss_filter_
+0000c130: 7472 756e 6361 7465 203d 2034 2e30 2c20  truncate = 4.0, 
+0000c140: 706c 6f74 5f64 6574 7265 6e64 696e 6720  plot_detrending 
+0000c150: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
 0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2020 2020 204d 434d 435f 7061 7261 6c6c       MCMC_parall
-0000c190: 656c 697a 6174 696f 6e5f 6d65 7468 6f64  elization_method
-0000c1a0: 203d 204e 6f6e 652c 206e 756d 5f70 726f   = None, num_pro
-0000c1b0: 6365 7373 6573 203d 204e 6f6e 652c 0a20  cesses = None,. 
+0000c180: 2020 2020 2020 4d43 4d43 5f70 6172 616c        MCMC_paral
+0000c190: 6c65 6c69 7a61 7469 6f6e 5f6d 6574 686f  lelization_metho
+0000c1a0: 6420 3d20 4e6f 6e65 2c20 6e75 6d5f 7072  d = None, num_pr
+0000c1b0: 6f63 6573 7365 7320 3d20 4e6f 6e65 2c0a  ocesses = None,.
 0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1e0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-0000c1f0: 6368 6f70 5f63 6861 696e 7320 3d20 4e6f  chop_chains = No
-0000c200: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
-0000c210: 0a20 2020 2020 2020 2050 6572 666f 726d  .        Perform
-0000c220: 7320 616e 2061 7574 6f6d 6174 6564 2077  s an automated w
-0000c230: 696e 646f 7720 7363 616e 2077 6974 6820  indow scan with 
-0000c240: 6465 6669 6e65 6420 6060 7769 6e64 6f77  defined ``window
-0000c250: 5f73 6869 6674 6060 206f 7665 7220 7468  _shift`` over th
-0000c260: 6520 7768 6f6c 6520 7469 6d65 2073 6572  e whole time ser
-0000c270: 6965 732e 2049 6e20 6561 6368 0a20 2020  ies. In each.   
-0000c280: 2020 2020 2077 696e 646f 7720 7468 6520       window the 
-0000c290: 6472 6966 7420 736c 6f70 6520 616e 6420  drift slope and 
-0000c2a0: 6e6f 6973 6520 6c65 7665 6c20 6573 7469  noise level esti
-0000c2b0: 6d61 7465 7320 7769 7468 2063 6f72 7265  mates with corre
-0000c2c0: 7370 6f6e 6469 6e67 2063 7265 6469 6269  sponding credibi
-0000c2d0: 6c69 7479 2062 616e 6473 2061 7265 2063  lity bands are c
-0000c2e0: 6f6d 7075 7465 640a 2020 2020 2020 2020  omputed.        
-0000c2f0: 616e 6420 7361 7665 6420 696e 2074 6865  and saved in the
-0000c300: 2060 6073 6c6f 7065 5f73 746f 7261 6765   ``slope_storage
-0000c310: 6060 2061 6e64 2074 6865 2060 606e 6f69  `` and the ``noi
-0000c320: 7365 5f6c 6576 656c 5f73 746f 7261 6765  se_level_storage
-0000c330: 6060 2e20 4974 2063 616e 2061 6c73 6f20  ``. It can also 
-0000c340: 6265 2075 7365 6420 746f 2063 7265 6174  be used to creat
-0000c350: 6520 616e 0a20 2020 2020 2020 2061 6e69  e an.        ani
-0000c360: 6d61 7469 6f6e 206f 6620 7468 6520 736c  mation of the sl
-0000c370: 6964 696e 6720 7769 6e64 6f77 2061 7070  iding window app
-0000c380: 726f 6163 6820 706c 6f74 7469 6e67 2074  roach plotting t
-0000c390: 6865 2074 696d 6520 7365 7269 6573 2c20  he time series, 
-0000c3a0: 7468 6520 6d6f 7669 6e67 2077 696e 646f  the moving windo
-0000c3b0: 772c 2061 6e64 2074 6865 0a20 2020 2020  w, and the.     
-0000c3c0: 2020 2074 696d 6520 6576 6f6c 7574 696f     time evolutio
-0000c3d0: 6e20 6f66 2074 6865 2064 7269 6674 2073  n of the drift s
-0000c3e0: 6c6f 7065 2065 7374 696d 6174 6573 203a  lope estimates :
-0000c3f0: 6d61 7468 3a60 5c68 6174 7b5c 7a65 7461  math:`\hat{\zeta
-0000c400: 7d60 2c20 7468 6520 6e6f 6973 6520 6c65  }`, the noise le
-0000c410: 7665 6c20 3a6d 6174 683a 605c 6861 747b  vel :math:`\hat{
-0000c420: 5c73 6967 6d61 7d60 0a20 2020 2020 2020  \sigma}`.       
-0000c430: 2061 6e64 2074 6865 206e 6f69 7365 206b   and the noise k
-0000c440: 6572 6e65 6c20 6465 6e73 6974 7920 6573  ernel density es
-0000c450: 7469 6d61 7465 2e20 5468 6520 7374 6172  timate. The star
-0000c460: 7420 696e 6469 6365 7320 6f66 2074 6865  t indices of the
-0000c470: 2073 6869 6674 6564 2077 696e 646f 7773   shifted windows
-0000c480: 2069 7320 616c 736f 2073 6176 6564 0a20   is also saved. 
-0000c490: 2020 2020 2020 2069 6e20 6f72 6465 7220         in order 
-0000c4a0: 746f 2066 6163 696c 6974 6174 6520 6375  to facilitate cu
-0000c4b0: 7374 6f6d 697a 6564 2070 6c6f 7473 2e0a  stomized plots..
-0000c4c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c4d0: 7769 6e64 6f77 5f73 697a 653a 2054 696d  window_size: Tim
-0000c4e0: 6520 7769 6e64 6f77 2073 697a 652e 0a20  e window size.. 
-0000c4f0: 2020 2020 2020 203a 7479 7065 2077 696e         :type win
-0000c500: 646f 775f 7369 7a65 3a20 696e 740a 2020  dow_size: int.  
-0000c510: 2020 2020 2020 3a70 6172 616d 2077 696e        :param win
-0000c520: 646f 775f 7368 6966 743a 2054 6865 2072  dow_shift: The r
-0000c530: 6f6c 6c69 6e67 2074 696d 6520 7769 6e64  olling time wind
-0000c540: 6f77 2069 7320 7368 6966 7465 6420 6162  ow is shifted ab
-0000c550: 6f75 7420 6060 7769 6e64 6f77 5f73 6869  out ``window_shi
-0000c560: 6674 6060 2064 6174 6120 706f 696e 7473  ft`` data points
-0000c570: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000c580: 7769 6e64 6f77 5f73 6869 6674 3a20 696e  window_shift: in
-0000c590: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-0000c5a0: 2073 6c6f 7065 5f67 7269 643a 2041 7272   slope_grid: Arr
-0000c5b0: 6179 206f 6e20 7768 6963 6820 7468 6520  ay on which the 
-0000c5c0: 6472 6966 7420 736c 6f70 6520 6b65 726e  drift slope kern
-0000c5d0: 656c 2064 656e 7369 7479 2065 7374 696d  el density estim
-0000c5e0: 6174 6520 6973 2065 7661 6c75 6174 6564  ate is evaluated
-0000c5f0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000c600: 736c 6f70 655f 6772 6964 3a20 4f6e 652d  slope_grid: One-
-0000c610: 6469 6d65 6e73 696f 6e61 6c20 6e75 6d70  dimensional nump
-0000c620: 7920 6172 7261 7920 6f66 2066 6c6f 6174  y array of float
-0000c630: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-0000c640: 206e 6f69 7365 5f67 7269 643a 2041 7272   noise_grid: Arr
-0000c650: 6179 206f 6e20 7768 6963 6820 7468 6520  ay on which the 
-0000c660: 6e6f 6973 6520 6c65 7665 6c20 6b65 726e  noise level kern
-0000c670: 656c 2064 656e 7369 7479 2065 7374 696d  el density estim
-0000c680: 6174 6520 6973 2065 7661 6c75 6174 6564  ate is evaluated
-0000c690: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000c6a0: 6e6f 6973 655f 6772 6964 3a20 4f6e 652d  noise_grid: One-
-0000c6b0: 6469 6d65 6e73 696f 6e61 6c20 6e75 6d70  dimensional nump
-0000c6c0: 7920 6172 7261 7920 6f66 2066 6c6f 6174  y array of float
-0000c6d0: 730a 2020 2020 2020 2020 3a70 6172 616d  s.        :param
-0000c6e0: 206e 7761 6c6b 6572 733a 204e 756d 6265   nwalkers: Numbe
-0000c6f0: 7220 6f66 2077 616c 6b65 7273 2074 6861  r of walkers tha
-0000c700: 7420 6172 6520 696e 6974 6961 6c69 7a65  t are initialize
-0000c710: 6420 666f 7220 7468 6520 4d43 4d43 2073  d for the MCMC s
-0000c720: 616d 706c 696e 6720 7669 6120 7468 6520  ampling via the 
-0000c730: 7061 636b 6167 6520 6060 656d 6365 6560  package ``emcee`
-0000c740: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
-0000c750: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-0000c760: 6c74 2069 7320 3530 2e0a 2020 2020 2020  lt is 50..      
-0000c770: 2020 3a74 7970 6520 6e77 616c 6b65 7273    :type nwalkers
-0000c780: 3a20 696e 740a 2020 2020 2020 2020 3a70  : int.        :p
-0000c790: 6172 616d 206e 7374 6570 733a 204c 656e  aram nsteps: Len
-0000c7a0: 6774 6820 6f66 2074 6865 2073 616d 706c  gth of the sampl
-0000c7b0: 6564 204d 434d 4320 6368 6169 6e73 2e20  ed MCMC chains. 
-0000c7c0: 4465 6661 756c 7420 6973 2031 3030 3030  Default is 10000
-0000c7d0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-0000c7e0: 6e73 7465 7073 3a20 696e 740a 2020 2020  nsteps: int.    
-0000c7f0: 2020 2020 3a70 6172 616d 206e 6275 726e      :param nburn
-0000c800: 3a20 4e75 6d62 6572 206f 6620 6461 7461  : Number of data
-0000c810: 2070 6f69 6e74 7320 6174 2074 6865 2062   points at the b
-0000c820: 6567 696e 6e69 6e67 206f 6620 7468 6520  eginning of the 
-0000c830: 4d61 726b 6f76 2063 6861 696e 7320 7768  Markov chains wh
-0000c840: 6963 6820 6172 6520 6469 7363 6172 6465  ich are discarde
-0000c850: 6420 696e 2074 6572 6d73 206f 660a 2020  d in terms of.  
+0000c1e0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+0000c1f0: 5f63 686f 705f 6368 6169 6e73 203d 204e  _chop_chains = N
+0000c200: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
+0000c210: 270a 2020 2020 2020 2020 5065 7266 6f72  '.        Perfor
+0000c220: 6d73 2061 6e20 6175 746f 6d61 7465 6420  ms an automated 
+0000c230: 7769 6e64 6f77 2073 6361 6e20 7769 7468  window scan with
+0000c240: 2064 6566 696e 6564 2060 6077 696e 646f   defined ``windo
+0000c250: 775f 7368 6966 7460 6020 6f76 6572 2074  w_shift`` over t
+0000c260: 6865 2077 686f 6c65 2074 696d 6520 7365  he whole time se
+0000c270: 7269 6573 2e20 496e 2065 6163 680a 2020  ries. In each.  
+0000c280: 2020 2020 2020 7769 6e64 6f77 2074 6865        window the
+0000c290: 2064 7269 6674 2073 6c6f 7065 2061 6e64   drift slope and
+0000c2a0: 206e 6f69 7365 206c 6576 656c 2065 7374   noise level est
+0000c2b0: 696d 6174 6573 2077 6974 6820 636f 7272  imates with corr
+0000c2c0: 6573 706f 6e64 696e 6720 6372 6564 6962  esponding credib
+0000c2d0: 696c 6974 7920 6261 6e64 7320 6172 6520  ility bands are 
+0000c2e0: 636f 6d70 7574 6564 0a20 2020 2020 2020  computed.       
+0000c2f0: 2061 6e64 2073 6176 6564 2069 6e20 7468   and saved in th
+0000c300: 6520 6060 736c 6f70 655f 7374 6f72 6167  e ``slope_storag
+0000c310: 6560 6020 616e 6420 7468 6520 6060 6e6f  e`` and the ``no
+0000c320: 6973 655f 6c65 7665 6c5f 7374 6f72 6167  ise_level_storag
+0000c330: 6560 602e 2049 7420 6361 6e20 616c 736f  e``. It can also
+0000c340: 2062 6520 7573 6564 2074 6f20 6372 6561   be used to crea
+0000c350: 7465 2061 6e0a 2020 2020 2020 2020 616e  te an.        an
+0000c360: 696d 6174 696f 6e20 6f66 2074 6865 2073  imation of the s
+0000c370: 6c69 6469 6e67 2077 696e 646f 7720 6170  liding window ap
+0000c380: 7072 6f61 6368 2070 6c6f 7474 696e 6720  proach plotting 
+0000c390: 7468 6520 7469 6d65 2073 6572 6965 732c  the time series,
+0000c3a0: 2074 6865 206d 6f76 696e 6720 7769 6e64   the moving wind
+0000c3b0: 6f77 2c20 616e 6420 7468 650a 2020 2020  ow, and the.    
+0000c3c0: 2020 2020 7469 6d65 2065 766f 6c75 7469      time evoluti
+0000c3d0: 6f6e 206f 6620 7468 6520 6472 6966 7420  on of the drift 
+0000c3e0: 736c 6f70 6520 6573 7469 6d61 7465 7320  slope estimates 
+0000c3f0: 3a6d 6174 683a 605c 6861 747b 5c7a 6574  :math:`\hat{\zet
+0000c400: 617d 602c 2074 6865 206e 6f69 7365 206c  a}`, the noise l
+0000c410: 6576 656c 203a 6d61 7468 3a60 5c68 6174  evel :math:`\hat
+0000c420: 7b5c 7369 676d 617d 600a 2020 2020 2020  {\sigma}`.      
+0000c430: 2020 616e 6420 7468 6520 6e6f 6973 6520    and the noise 
+0000c440: 6b65 726e 656c 2064 656e 7369 7479 2065  kernel density e
+0000c450: 7374 696d 6174 652e 2054 6865 2073 7461  stimate. The sta
+0000c460: 7274 2069 6e64 6963 6573 206f 6620 7468  rt indices of th
+0000c470: 6520 7368 6966 7465 6420 7769 6e64 6f77  e shifted window
+0000c480: 7320 6973 2061 6c73 6f20 7361 7665 640a  s is also saved.
+0000c490: 2020 2020 2020 2020 696e 206f 7264 6572          in order
+0000c4a0: 2074 6f20 6661 6369 6c69 7461 7465 2063   to facilitate c
+0000c4b0: 7573 746f 6d69 7a65 6420 706c 6f74 732e  ustomized plots.
+0000c4c0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000c4d0: 2077 696e 646f 775f 7369 7a65 3a20 5469   window_size: Ti
+0000c4e0: 6d65 2077 696e 646f 7720 7369 7a65 2e0a  me window size..
+0000c4f0: 2020 2020 2020 2020 3a74 7970 6520 7769          :type wi
+0000c500: 6e64 6f77 5f73 697a 653a 2069 6e74 0a20  ndow_size: int. 
+0000c510: 2020 2020 2020 203a 7061 7261 6d20 7769         :param wi
+0000c520: 6e64 6f77 5f73 6869 6674 3a20 5468 6520  ndow_shift: The 
+0000c530: 726f 6c6c 696e 6720 7469 6d65 2077 696e  rolling time win
+0000c540: 646f 7720 6973 2073 6869 6674 6564 2061  dow is shifted a
+0000c550: 626f 7574 2060 6077 696e 646f 775f 7368  bout ``window_sh
+0000c560: 6966 7460 6020 6461 7461 2070 6f69 6e74  ift`` data point
+0000c570: 732e 0a20 2020 2020 2020 203a 7479 7065  s..        :type
+0000c580: 2077 696e 646f 775f 7368 6966 743a 2069   window_shift: i
+0000c590: 6e74 0a20 2020 2020 2020 203a 7061 7261  nt.        :para
+0000c5a0: 6d20 736c 6f70 655f 6772 6964 3a20 4172  m slope_grid: Ar
+0000c5b0: 7261 7920 6f6e 2077 6869 6368 2074 6865  ray on which the
+0000c5c0: 2064 7269 6674 2073 6c6f 7065 206b 6572   drift slope ker
+0000c5d0: 6e65 6c20 6465 6e73 6974 7920 6573 7469  nel density esti
+0000c5e0: 6d61 7465 2069 7320 6576 616c 7561 7465  mate is evaluate
+0000c5f0: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
+0000c600: 2073 6c6f 7065 5f67 7269 643a 204f 6e65   slope_grid: One
+0000c610: 2d64 696d 656e 7369 6f6e 616c 206e 756d  -dimensional num
+0000c620: 7079 2061 7272 6179 206f 6620 666c 6f61  py array of floa
+0000c630: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+0000c640: 6d20 6e6f 6973 655f 6772 6964 3a20 4172  m noise_grid: Ar
+0000c650: 7261 7920 6f6e 2077 6869 6368 2074 6865  ray on which the
+0000c660: 206e 6f69 7365 206c 6576 656c 206b 6572   noise level ker
+0000c670: 6e65 6c20 6465 6e73 6974 7920 6573 7469  nel density esti
+0000c680: 6d61 7465 2069 7320 6576 616c 7561 7465  mate is evaluate
+0000c690: 642e 0a20 2020 2020 2020 203a 7479 7065  d..        :type
+0000c6a0: 206e 6f69 7365 5f67 7269 643a 204f 6e65   noise_grid: One
+0000c6b0: 2d64 696d 656e 7369 6f6e 616c 206e 756d  -dimensional num
+0000c6c0: 7079 2061 7272 6179 206f 6620 666c 6f61  py array of floa
+0000c6d0: 7473 0a20 2020 2020 2020 203a 7061 7261  ts.        :para
+0000c6e0: 6d20 6e77 616c 6b65 7273 3a20 4e75 6d62  m nwalkers: Numb
+0000c6f0: 6572 206f 6620 7761 6c6b 6572 7320 7468  er of walkers th
+0000c700: 6174 2061 7265 2069 6e69 7469 616c 697a  at are initializ
+0000c710: 6564 2066 6f72 2074 6865 204d 434d 4320  ed for the MCMC 
+0000c720: 7361 6d70 6c69 6e67 2076 6961 2074 6865  sampling via the
+0000c730: 2070 6163 6b61 6765 2060 6065 6d63 6565   package ``emcee
+0000c740: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
+0000c750: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0000c760: 756c 7420 6973 2035 302e 0a20 2020 2020  ult is 50..     
+0000c770: 2020 203a 7479 7065 206e 7761 6c6b 6572     :type nwalker
+0000c780: 733a 2069 6e74 0a20 2020 2020 2020 203a  s: int.        :
+0000c790: 7061 7261 6d20 6e73 7465 7073 3a20 4c65  param nsteps: Le
+0000c7a0: 6e67 7468 206f 6620 7468 6520 7361 6d70  ngth of the samp
+0000c7b0: 6c65 6420 4d43 4d43 2063 6861 696e 732e  led MCMC chains.
+0000c7c0: 2044 6566 6175 6c74 2069 7320 3130 3030   Default is 1000
+0000c7d0: 302e 0a20 2020 2020 2020 203a 7479 7065  0..        :type
+0000c7e0: 206e 7374 6570 733a 2069 6e74 0a20 2020   nsteps: int.   
+0000c7f0: 2020 2020 203a 7061 7261 6d20 6e62 7572       :param nbur
+0000c800: 6e3a 204e 756d 6265 7220 6f66 2064 6174  n: Number of dat
+0000c810: 6120 706f 696e 7473 2061 7420 7468 6520  a points at the 
+0000c820: 6265 6769 6e6e 696e 6720 6f66 2074 6865  beginning of the
+0000c830: 204d 6172 6b6f 7620 6368 6169 6e73 2077   Markov chains w
+0000c840: 6869 6368 2061 7265 2064 6973 6361 7264  hich are discard
+0000c850: 6564 2069 6e20 7465 726d 7320 6f66 0a20  ed in terms of. 
 0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c870: 2020 2020 2020 6120 6275 726e 2069 6e20        a burn in 
-0000c880: 7065 7269 6f64 2e20 4465 6661 756c 7420  period. Default 
-0000c890: 6973 2032 3030 2e0a 2020 2020 2020 2020  is 200..        
-0000c8a0: 3a74 7970 6520 6e62 7572 6e3a 2069 6e74  :type nburn: int
-0000c8b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c8c0: 6e5f 6a6f 696e 745f 7361 6d70 6c65 733a  n_joint_samples:
-0000c8d0: 204e 756d 6265 7220 6f66 206a 6f69 6e74   Number of joint
-0000c8e0: 2073 616d 706c 6573 2074 6861 7420 6172   samples that ar
-0000c8f0: 6520 6472 6177 6e20 6672 6f6d 2074 6865  e drawn from the
-0000c900: 2065 7374 696d 6174 6564 206a 6f69 6e74   estimated joint
-0000c910: 2070 6f73 7465 7269 6f72 0a20 2020 2020   posterior.     
+0000c870: 2020 2020 2020 2061 2062 7572 6e20 696e         a burn in
+0000c880: 2070 6572 696f 642e 2044 6566 6175 6c74   period. Default
+0000c890: 2069 7320 3230 302e 0a20 2020 2020 2020   is 200..       
+0000c8a0: 203a 7479 7065 206e 6275 726e 3a20 696e   :type nburn: in
+0000c8b0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+0000c8c0: 206e 5f6a 6f69 6e74 5f73 616d 706c 6573   n_joint_samples
+0000c8d0: 3a20 4e75 6d62 6572 206f 6620 6a6f 696e  : Number of join
+0000c8e0: 7420 7361 6d70 6c65 7320 7468 6174 2061  t samples that a
+0000c8f0: 7265 2064 7261 776e 2066 726f 6d20 7468  re drawn from th
+0000c900: 6520 6573 7469 6d61 7465 6420 6a6f 696e  e estimated join
+0000c910: 7420 706f 7374 6572 696f 720a 2020 2020  t posterior.    
 0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c930: 2020 2070 726f 6261 6269 6c69 7479 2069     probability i
-0000c940: 6e20 6f72 6465 7220 746f 2063 616c 6375  n order to calcu
-0000c950: 6c61 7465 2074 6865 2064 7269 6674 2073  late the drift s
-0000c960: 6c6f 7065 2065 7374 696d 6174 6520 3a6d  lope estimate :m
-0000c970: 6174 683a 605c 7a65 7461 6020 616e 640a  ath:`\zeta` and.
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
-0000c9a0: 6e64 696e 6720 6372 6564 6962 696c 6974  nding credibilit
-0000c9b0: 7920 6261 6e64 732e 2044 6566 6175 6c74  y bands. Default
-0000c9c0: 2069 7320 3530 3030 302e 0a20 2020 2020   is 50000..     
-0000c9d0: 2020 203a 7479 7065 206e 5f6a 6f69 6e74     :type n_joint
-0000c9e0: 5f73 616d 706c 6573 3a20 696e 740a 2020  _samples: int.  
-0000c9f0: 2020 2020 2020 3a70 6172 616d 206e 5f73        :param n_s
-0000ca00: 6c6f 7065 5f73 616d 706c 6573 3a20 4e75  lope_samples: Nu
-0000ca10: 6d62 6572 206f 6620 6472 6966 7420 736c  mber of drift sl
-0000ca20: 6f70 6520 7361 6d70 6c65 7320 7468 6174  ope samples that
-0000ca30: 2061 7265 2064 7261 776e 2066 726f 6d20   are drawn from 
-0000ca40: 7468 6520 6573 7469 6d61 7465 6420 6472  the estimated dr
-0000ca50: 6966 7420 736c 6f70 650a 2020 2020 2020  ift slope.      
+0000c930: 2020 2020 7072 6f62 6162 696c 6974 7920      probability 
+0000c940: 696e 206f 7264 6572 2074 6f20 6361 6c63  in order to calc
+0000c950: 756c 6174 6520 7468 6520 6472 6966 7420  ulate the drift 
+0000c960: 736c 6f70 6520 6573 7469 6d61 7465 203a  slope estimate :
+0000c970: 6d61 7468 3a60 5c7a 6574 6160 2061 6e64  math:`\zeta` and
+0000c980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c990: 2020 2020 2020 2020 2063 6f72 7265 7370           corresp
+0000c9a0: 6f6e 6469 6e67 2063 7265 6469 6269 6c69  onding credibili
+0000c9b0: 7479 2062 616e 6473 2e20 4465 6661 756c  ty bands. Defaul
+0000c9c0: 7420 6973 2035 3030 3030 2e0a 2020 2020  t is 50000..    
+0000c9d0: 2020 2020 3a74 7970 6520 6e5f 6a6f 696e      :type n_join
+0000c9e0: 745f 7361 6d70 6c65 733a 2069 6e74 0a20  t_samples: int. 
+0000c9f0: 2020 2020 2020 203a 7061 7261 6d20 6e5f         :param n_
+0000ca00: 736c 6f70 655f 7361 6d70 6c65 733a 204e  slope_samples: N
+0000ca10: 756d 6265 7220 6f66 2064 7269 6674 2073  umber of drift s
+0000ca20: 6c6f 7065 2073 616d 706c 6573 2074 6861  lope samples tha
+0000ca30: 7420 6172 6520 6472 6177 6e20 6672 6f6d  t are drawn from
+0000ca40: 2074 6865 2065 7374 696d 6174 6564 2064   the estimated d
+0000ca50: 7269 6674 2073 6c6f 7065 0a20 2020 2020  rift slope.     
 0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 706f 7374 6572 696f 7220 636f 6d70    posterior comp
-0000ca80: 7574 6564 2062 6173 6564 206f 6e20 7468  uted based on th
-0000ca90: 6520 7361 6d70 6c69 6e67 2072 6573 756c  e sampling resul
-0000caa0: 7473 206f 6620 7468 6520 6a6f 696e 7420  ts of the joint 
-0000cab0: 706f 7374 6572 696f 7220 7072 6f62 6162  posterior probab
-0000cac0: 696c 6974 790a 2020 2020 2020 2020 2020  ility.          
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-0000cae0: 2074 6865 204c 616e 6765 7669 6e20 7061   the Langevin pa
-0000caf0: 7261 6d65 7465 7273 203a 6d61 7468 3a60  rameters :math:`
-0000cb00: 5c74 6865 7461 5f69 602e 2044 6566 6175  \theta_i`. Defau
-0000cb10: 6c74 2069 7320 3530 3030 302e 0a20 2020  lt is 50000..   
-0000cb20: 2020 2020 203a 7479 7065 206e 5f73 6c6f       :type n_slo
-0000cb30: 7065 5f73 616d 706c 6573 3a20 696e 740a  pe_samples: int.
-0000cb40: 2020 2020 2020 2020 3a70 6172 616d 206e          :param n
-0000cb50: 5f6e 6f69 7365 5f73 616d 706c 6573 3a20  _noise_samples: 
-0000cb60: 4e75 6d62 6572 206f 6620 636f 6e73 7461  Number of consta
-0000cb70: 6e74 206e 6f69 7365 206c 6576 656c 2073  nt noise level s
-0000cb80: 616d 706c 6573 2074 6861 7420 6172 6520  amples that are 
-0000cb90: 6472 6177 6e20 6672 6f6d 2074 6865 2065  drawn from the e
-0000cba0: 7374 696d 6174 6564 0a20 2020 2020 2020  stimated.       
+0000ca70: 2020 2070 6f73 7465 7269 6f72 2063 6f6d     posterior com
+0000ca80: 7075 7465 6420 6261 7365 6420 6f6e 2074  puted based on t
+0000ca90: 6865 2073 616d 706c 696e 6720 7265 7375  he sampling resu
+0000caa0: 6c74 7320 6f66 2074 6865 206a 6f69 6e74  lts of the joint
+0000cab0: 2070 6f73 7465 7269 6f72 2070 726f 6261   posterior proba
+0000cac0: 6269 6c69 7479 0a20 2020 2020 2020 2020  bility.         
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000cae0: 6620 7468 6520 4c61 6e67 6576 696e 2070  f the Langevin p
+0000caf0: 6172 616d 6574 6572 7320 3a6d 6174 683a  arameters :math:
+0000cb00: 605c 7468 6574 615f 6960 2e20 4465 6661  `\theta_i`. Defa
+0000cb10: 756c 7420 6973 2035 3030 3030 2e0a 2020  ult is 50000..  
+0000cb20: 2020 2020 2020 3a74 7970 6520 6e5f 736c        :type n_sl
+0000cb30: 6f70 655f 7361 6d70 6c65 733a 2069 6e74  ope_samples: int
+0000cb40: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000cb50: 6e5f 6e6f 6973 655f 7361 6d70 6c65 733a  n_noise_samples:
+0000cb60: 204e 756d 6265 7220 6f66 2063 6f6e 7374   Number of const
+0000cb70: 616e 7420 6e6f 6973 6520 6c65 7665 6c20  ant noise level 
+0000cb80: 7361 6d70 6c65 7320 7468 6174 2061 7265  samples that are
+0000cb90: 2064 7261 776e 2066 726f 6d20 7468 6520   drawn from the 
+0000cba0: 6573 7469 6d61 7465 640a 2020 2020 2020  estimated.      
 0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 206d 6172 6967 6e61 6c20 7072 6f62 696c   marignal probil
-0000cbd0: 6974 7920 6469 7374 7269 6275 7469 6f6e  ity distribution
-0000cbe0: 206f 6620 7468 6520 6469 6666 7573 696f   of the diffusio
-0000cbf0: 6e20 6d6f 6465 6c20 6973 2063 686f 7365  n model is chose
-0000cc00: 6e20 636f 6e73 7461 6e74 2e0a 2020 2020  n constant..    
+0000cbc0: 2020 6d61 7269 676e 616c 2070 726f 6269    marignal probi
+0000cbd0: 6c69 7479 2064 6973 7472 6962 7574 696f  lity distributio
+0000cbe0: 6e20 6f66 2074 6865 2064 6966 6675 7369  n of the diffusi
+0000cbf0: 6f6e 206d 6f64 656c 2069 7320 6368 6f73  on model is chos
+0000cc00: 656e 2063 6f6e 7374 616e 742e 0a20 2020  en constant..   
 0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 4465 6661 756c 7420 6973 2035      Default is 5
-0000cc30: 3030 3030 2e0a 2020 2020 2020 2020 3a74  0000..        :t
-0000cc40: 7970 6520 6e5f 6e6f 6973 655f 7361 6d70  ype n_noise_samp
-0000cc50: 6c65 733a 2069 6e74 0a20 2020 2020 2020  les: int.       
-0000cc60: 203a 7061 7261 6d20 6372 6564 5f70 6572   :param cred_per
-0000cc70: 6365 6e74 696c 6573 3a20 5477 6f20 656e  centiles: Two en
-0000cc80: 7472 6965 7320 746f 2064 6566 696e 6520  tries to define 
-0000cc90: 7468 6520 7065 7263 656e 7469 6c65 7320  the percentiles 
-0000cca0: 6f66 2074 6865 2063 616c 6375 6c61 7465  of the calculate
-0000ccb0: 6420 6372 6564 6962 696c 6974 7920 6261  d credibility ba
-0000ccc0: 6e64 730a 2020 2020 2020 2020 2020 2020  nds.            
-0000ccd0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-0000cce0: 6865 2065 7374 696d 6174 6564 2070 6172  he estimated par
-0000ccf0: 616d 6574 6572 732e 2044 6566 6175 6c74  ameters. Default
-0000cd00: 2069 7320 6060 6e75 6d70 792e 6172 7261   is ``numpy.arra
-0000cd10: 7928 5b31 362c 315d 2960 602e 0a20 2020  y([16,1])``..   
-0000cd20: 2020 2020 203a 7479 7065 2063 7265 645f       :type cred_
-0000cd30: 7065 7263 656e 7469 6c65 733a 204f 6e65  percentiles: One
-0000cd40: 2d64 696d 656e 7369 6f6e 616c 206e 756d  -dimensional num
-0000cd50: 7079 2061 7272 6179 206f 6620 696e 7465  py array of inte
-0000cd60: 6765 7273 0a20 2020 2020 2020 203a 7061  gers.        :pa
-0000cd70: 7261 6d20 7072 696e 745f 4143 5f74 6175  ram print_AC_tau
-0000cd80: 3a20 4966 2060 6054 7275 6560 6020 7468  : If ``True`` th
-0000cd90: 6520 6573 7469 6d61 7465 6420 6175 746f  e estimated auto
-0000cda0: 636f 7272 656c 6174 696f 6e20 6c65 6e67  correlation leng
-0000cdb0: 7468 7320 6f66 2074 6865 204d 6172 6b6f  ths of the Marko
-0000cdc0: 7620 6368 6169 6e73 2069 7320 7368 6f77  v chains is show
-0000cdd0: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
-0000cde0: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-0000cdf0: 6178 696d 756d 206c 656e 6774 6820 6973  aximum length is
-0000ce00: 2075 7365 6420 666f 7220 7468 696e 6e69   used for thinni
-0000ce10: 6e67 206f 6620 7468 6520 6368 6169 6e73  ng of the chains
-0000ce20: 2e20 4465 6661 756c 7420 6973 2060 6046  . Default is ``F
-0000ce30: 616c 7365 6060 2e0a 2020 2020 2020 2020  alse``..        
-0000ce40: 3a74 7970 6520 7072 696e 645f 4143 5f74  :type prind_AC_t
-0000ce50: 6175 3a20 626f 6f6c 0a20 2020 2020 2020  au: bool.       
-0000ce60: 203a 7061 7261 6d20 6967 6e6f 7265 5f41   :param ignore_A
-0000ce70: 435f 6572 726f 723a 2049 6620 6060 5472  C_error: If ``Tr
-0000ce80: 7565 6060 2074 6865 2061 7574 6f63 6f72  ue`` the autocor
-0000ce90: 7265 6c61 7469 6f6e 206c 656e 6774 6873  relation lengths
-0000cea0: 206f 6620 7468 6520 4d61 726b 6f76 2063   of the Markov c
-0000ceb0: 6861 696e 7320 6973 206e 6f74 2065 7374  hains is not est
-0000cec0: 696d 6174 6564 0a20 2020 2020 2020 2020  imated.         
-0000ced0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000cee0: 6e64 2074 6875 732c 2069 7420 6973 206e  nd thus, it is n
-0000cef0: 6f74 2063 6865 636b 6564 2077 6865 7468  ot checked wheth
-0000cf00: 6572 2074 6865 2063 6861 696e 7320 6172  er the chains ar
-0000cf10: 6520 746f 6f20 7368 6f72 7420 746f 2067  e too short to g
-0000cf20: 6976 6520 616e 2072 656c 6961 626c 650a  ive an reliable.
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 2020 2020 2020 6175 746f 636f 7272          autocorr
-0000cf50: 656c 6174 696f 6e20 6573 7469 6d61 7465  elation estimate
-0000cf60: 2e20 5468 6973 2061 766f 6964 7320 6572  . This avoids er
-0000cf70: 726f 7220 696e 7465 7272 7570 7469 6f6e  ror interruption
-0000cf80: 206f 6620 7468 6520 7072 6f63 6564 7572   of the procedur
-0000cf90: 652c 2062 7574 0a20 2020 2020 2020 2020  e, but.         
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cfb0: 616e 206c 6561 6420 746f 2075 6e72 656c  an lead to unrel
-0000cfc0: 6961 626c 6520 7265 7375 6c74 7320 6966  iable results if
-0000cfd0: 2074 6865 2063 6861 696e 7320 6172 6520   the chains are 
-0000cfe0: 746f 6f20 7368 6f72 742e 2054 6865 206f  too short. The o
-0000cff0: 7074 696f 6e20 7368 6f75 6c64 0a20 2020  ption should.   
+0000cc20: 2020 2020 2044 6566 6175 6c74 2069 7320       Default is 
+0000cc30: 3530 3030 302e 0a20 2020 2020 2020 203a  50000..        :
+0000cc40: 7479 7065 206e 5f6e 6f69 7365 5f73 616d  type n_noise_sam
+0000cc50: 706c 6573 3a20 696e 740a 2020 2020 2020  ples: int.      
+0000cc60: 2020 3a70 6172 616d 2063 7265 645f 7065    :param cred_pe
+0000cc70: 7263 656e 7469 6c65 733a 2054 776f 2065  rcentiles: Two e
+0000cc80: 6e74 7269 6573 2074 6f20 6465 6669 6e65  ntries to define
+0000cc90: 2074 6865 2070 6572 6365 6e74 696c 6573   the percentiles
+0000cca0: 206f 6620 7468 6520 6361 6c63 756c 6174   of the calculat
+0000ccb0: 6564 2063 7265 6469 6269 6c69 7479 2062  ed credibility b
+0000ccc0: 616e 6473 0a20 2020 2020 2020 2020 2020  ands.           
+0000ccd0: 2020 2020 2020 2020 2020 2020 206f 6620               of 
+0000cce0: 7468 6520 6573 7469 6d61 7465 6420 7061  the estimated pa
+0000ccf0: 7261 6d65 7465 7273 2e20 4465 6661 756c  rameters. Defaul
+0000cd00: 7420 6973 2060 606e 756d 7079 2e61 7272  t is ``numpy.arr
+0000cd10: 6179 285b 3136 2c31 5d29 6060 2e0a 2020  ay([16,1])``..  
+0000cd20: 2020 2020 2020 3a74 7970 6520 6372 6564        :type cred
+0000cd30: 5f70 6572 6365 6e74 696c 6573 3a20 4f6e  _percentiles: On
+0000cd40: 652d 6469 6d65 6e73 696f 6e61 6c20 6e75  e-dimensional nu
+0000cd50: 6d70 7920 6172 7261 7920 6f66 2069 6e74  mpy array of int
+0000cd60: 6567 6572 730a 2020 2020 2020 2020 3a70  egers.        :p
+0000cd70: 6172 616d 2070 7269 6e74 5f41 435f 7461  aram print_AC_ta
+0000cd80: 753a 2049 6620 6060 5472 7565 6060 2074  u: If ``True`` t
+0000cd90: 6865 2065 7374 696d 6174 6564 2061 7574  he estimated aut
+0000cda0: 6f63 6f72 7265 6c61 7469 6f6e 206c 656e  ocorrelation len
+0000cdb0: 6774 6873 206f 6620 7468 6520 4d61 726b  gths of the Mark
+0000cdc0: 6f76 2063 6861 696e 7320 6973 2073 686f  ov chains is sho
+0000cdd0: 776e 2e0a 2020 2020 2020 2020 2020 2020  wn..            
+0000cde0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000cdf0: 6d61 7869 6d75 6d20 6c65 6e67 7468 2069  maximum length i
+0000ce00: 7320 7573 6564 2066 6f72 2074 6869 6e6e  s used for thinn
+0000ce10: 696e 6720 6f66 2074 6865 2063 6861 696e  ing of the chain
+0000ce20: 732e 2044 6566 6175 6c74 2069 7320 6060  s. Default is ``
+0000ce30: 4661 6c73 6560 602e 0a20 2020 2020 2020  False``..       
+0000ce40: 203a 7479 7065 2070 7269 6e64 5f41 435f   :type prind_AC_
+0000ce50: 7461 753a 2062 6f6f 6c0a 2020 2020 2020  tau: bool.      
+0000ce60: 2020 3a70 6172 616d 2069 676e 6f72 655f    :param ignore_
+0000ce70: 4143 5f65 7272 6f72 3a20 4966 2060 6054  AC_error: If ``T
+0000ce80: 7275 6560 6020 7468 6520 6175 746f 636f  rue`` the autoco
+0000ce90: 7272 656c 6174 696f 6e20 6c65 6e67 7468  rrelation length
+0000cea0: 7320 6f66 2074 6865 204d 6172 6b6f 7620  s of the Markov 
+0000ceb0: 6368 6169 6e73 2069 7320 6e6f 7420 6573  chains is not es
+0000cec0: 7469 6d61 7465 640a 2020 2020 2020 2020  timated.        
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 616e 6420 7468 7573 2c20 6974 2069 7320  and thus, it is 
+0000cef0: 6e6f 7420 6368 6563 6b65 6420 7768 6574  not checked whet
+0000cf00: 6865 7220 7468 6520 6368 6169 6e73 2061  her the chains a
+0000cf10: 7265 2074 6f6f 2073 686f 7274 2074 6f20  re too short to 
+0000cf20: 6769 7665 2061 6e20 7265 6c69 6162 6c65  give an reliable
+0000cf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf40: 2020 2020 2020 2020 2061 7574 6f63 6f72           autocor
+0000cf50: 7265 6c61 7469 6f6e 2065 7374 696d 6174  relation estimat
+0000cf60: 652e 2054 6869 7320 6176 6f69 6473 2065  e. This avoids e
+0000cf70: 7272 6f72 2069 6e74 6572 7275 7074 696f  rror interruptio
+0000cf80: 6e20 6f66 2074 6865 2070 726f 6365 6475  n of the procedu
+0000cf90: 7265 2c20 6275 740a 2020 2020 2020 2020  re, but.        
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 6361 6e20 6c65 6164 2074 6f20 756e 7265  can lead to unre
+0000cfc0: 6c69 6162 6c65 2072 6573 756c 7473 2069  liable results i
+0000cfd0: 6620 7468 6520 6368 6169 6e73 2061 7265  f the chains are
+0000cfe0: 2074 6f6f 2073 686f 7274 2e20 5468 6520   too short. The 
+0000cff0: 6f70 7469 6f6e 2073 686f 756c 640a 2020  option should.  
 0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2062 6520 6368 6f73 656e 2069       be chosen i
-0000d020: 6e20 6f72 6465 7220 746f 2073 6176 6520  n order to save 
-0000d030: 636f 6d70 7574 6174 696f 6e20 7469 6d65  computation time
-0000d040: 2c20 652e 672e 2077 6865 6e20 6465 6275  , e.g. when debu
-0000d050: 6767 696e 6720 796f 7572 2063 6f64 650a  gging your code.
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2020 2020 2020 2020 7769 7468 2073 686f          with sho
-0000d080: 7274 204d 6172 6b6f 7620 6368 6169 6e73  rt Markov chains
-0000d090: 2e20 4465 6661 756c 7420 6973 2060 6046  . Default is ``F
-0000d0a0: 616c 7365 6060 2e0a 2020 2020 2020 2020  alse``..        
-0000d0b0: 3a74 7970 6520 6967 6e6f 7265 5f41 435f  :type ignore_AC_
-0000d0c0: 6572 726f 723a 2062 6f6f 6c0a 2020 2020  error: bool.    
-0000d0d0: 2020 2020 3a70 6172 616d 2074 6869 6e6e      :param thinn
-0000d0e0: 696e 675f 6279 3a20 4966 2060 6069 676e  ing_by: If ``ign
-0000d0f0: 6f72 655f 4143 5f65 7272 6f72 203d 3d20  ore_AC_error == 
-0000d100: 5472 7565 6060 2074 6865 2063 6861 696e  True`` the chain
-0000d110: 7320 6172 6520 7468 696e 6e65 6420 6279  s are thinned by
-0000d120: 2060 6074 6869 6e6e 696e 675f 6279 6060   ``thinning_by``
-0000d130: 2e20 4576 6572 790a 2020 2020 2020 2020  . Every.        
+0000d010: 2020 2020 2020 6265 2063 686f 7365 6e20        be chosen 
+0000d020: 696e 206f 7264 6572 2074 6f20 7361 7665  in order to save
+0000d030: 2063 6f6d 7075 7461 7469 6f6e 2074 696d   computation tim
+0000d040: 652c 2065 2e67 2e20 7768 656e 2064 6562  e, e.g. when deb
+0000d050: 7567 6769 6e67 2079 6f75 7220 636f 6465  ugging your code
+0000d060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d070: 2020 2020 2020 2020 2077 6974 6820 7368           with sh
+0000d080: 6f72 7420 4d61 726b 6f76 2063 6861 696e  ort Markov chain
+0000d090: 732e 2044 6566 6175 6c74 2069 7320 6060  s. Default is ``
+0000d0a0: 4661 6c73 6560 602e 0a20 2020 2020 2020  False``..       
+0000d0b0: 203a 7479 7065 2069 676e 6f72 655f 4143   :type ignore_AC
+0000d0c0: 5f65 7272 6f72 3a20 626f 6f6c 0a20 2020  _error: bool.   
+0000d0d0: 2020 2020 203a 7061 7261 6d20 7468 696e       :param thin
+0000d0e0: 6e69 6e67 5f62 793a 2049 6620 6060 6967  ning_by: If ``ig
+0000d0f0: 6e6f 7265 5f41 435f 6572 726f 7220 3d3d  nore_AC_error ==
+0000d100: 2054 7275 6560 6020 7468 6520 6368 6169   True`` the chai
+0000d110: 6e73 2061 7265 2074 6869 6e6e 6564 2062  ns are thinned b
+0000d120: 7920 6060 7468 696e 6e69 6e67 5f62 7960  y ``thinning_by`
+0000d130: 602e 2045 7665 7279 0a20 2020 2020 2020  `. Every.       
 0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 6060 7468 696e 6e69 6e67 5f62 7960 602d  ``thinning_by``-
-0000d160: 7468 2064 6174 6120 706f 696e 7420 6973  th data point is
-0000d170: 2073 746f 7265 642e 2044 6566 6175 6c74   stored. Default
-0000d180: 2069 7320 3630 2e0a 2020 2020 2020 2020   is 60..        
-0000d190: 3a74 7970 6520 7468 696e 6e69 6e67 5f62  :type thinning_b
-0000d1a0: 793a 2069 6e74 0a20 2020 2020 2020 203a  y: int.        :
-0000d1b0: 7061 7261 6d20 7072 696e 745f 7072 6f67  param print_prog
-0000d1c0: 7265 7373 3a20 4966 2060 6054 7275 6560  ress: If ``True`
-0000d1d0: 6020 7468 6520 7072 6f67 7265 7373 206f  ` the progress o
-0000d1e0: 6620 7468 6520 4d43 4d43 2073 616d 706c  f the MCMC sampl
-0000d1f0: 696e 6720 6973 2073 686f 776e 2e20 4465  ing is shown. De
-0000d200: 6661 756c 7420 6973 2060 6046 616c 7365  fault is ``False
-0000d210: 6060 2e0a 2020 2020 2020 2020 3a74 7970  ``..        :typ
-0000d220: 6520 7072 696e 745f 7072 6f67 7265 7373  e print_progress
-0000d230: 3a20 626f 6f6c 0a20 2020 2020 2020 203a  : bool.        :
-0000d240: 7061 7261 6d20 736c 6f70 655f 7361 7665  param slope_save
-0000d250: 5f6e 616d 653a 204e 616d 6520 6f66 2074  _name: Name of t
-0000d260: 6865 2066 696c 6520 696e 2077 6869 6368  he file in which
-0000d270: 2074 6865 2060 6073 6c6f 7065 5f73 746f   the ``slope_sto
-0000d280: 7261 6765 6060 2061 7272 6179 2077 696c  rage`` array wil
-0000d290: 6c20 6265 2073 6176 6564 2e20 4465 6661  l be saved. Defa
-0000d2a0: 756c 7420 6973 0a20 2020 2020 2020 2020  ult is.         
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-0000d2c0: 6064 6566 6175 6c74 5f73 6176 655f 736c  `default_save_sl
-0000d2d0: 6f70 6573 6060 2e0a 2020 2020 2020 2020  opes``..        
-0000d2e0: 3a74 7970 6520 736c 6f70 655f 7361 7665  :type slope_save
-0000d2f0: 5f6e 616d 653a 2073 7472 0a20 2020 2020  _name: str.     
-0000d300: 2020 203a 7061 7261 6d20 206e 6f69 7365     :param  noise
-0000d310: 5f6c 6576 656c 5f73 6176 655f 6e61 6d65  _level_save_name
-0000d320: 3a20 4e61 6d65 206f 6620 7468 6520 6669  : Name of the fi
-0000d330: 6c65 2069 6e20 7768 6963 6820 7468 6520  le in which the 
-0000d340: 6060 6e6f 6973 655f 6c65 7665 6c5f 7374  ``noise_level_st
-0000d350: 6f72 6167 6560 6020 6172 7261 7920 7769  orage`` array wi
-0000d360: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
-0000d370: 2020 2020 2020 2020 2020 2062 6520 7361             be sa
-0000d380: 7665 642e 2044 6566 6175 6c74 2069 7320  ved. Default is 
-0000d390: 6060 6465 6661 756c 745f 7361 7665 5f6e  ``default_save_n
-0000d3a0: 6f69 7365 6060 2e0a 2020 2020 2020 2020  oise``..        
-0000d3b0: 3a74 7970 6520 6e6f 6973 655f 6c65 7665  :type noise_leve
-0000d3c0: 6c5f 7361 7665 5f6e 616d 653a 2073 7472  l_save_name: str
-0000d3d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000d3e0: 7361 7665 3a20 4966 2060 6054 7275 6560  save: If ``True`
-0000d3f0: 6020 7468 6520 6060 736c 6f70 655f 7374  ` the ``slope_st
-0000d400: 6f72 6167 6560 6020 616e 6420 7468 6520  orage`` and the 
-0000d410: 6060 6e6f 6973 655f 6c65 7665 6c5f 7374  ``noise_level_st
-0000d420: 6f72 6167 6560 6020 6172 7261 7973 2061  orage`` arrays a
-0000d430: 7265 2073 6176 6564 2069 6e20 7468 650a  re saved in the.
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 2020 2020 656e 6420 6f66 2074          end of t
-0000d460: 6865 2073 6361 6e20 696e 2061 6e20 602e  he scan in an `.
-0000d470: 6e70 7960 2066 696c 652e 2044 6566 6175  npy` file. Defau
-0000d480: 6c74 2069 7320 6060 5472 7565 6060 2e0a  lt is ``True``..
-0000d490: 2020 2020 2020 2020 3a74 7970 6520 7361          :type sa
-0000d4a0: 7665 3a20 626f 6f6c 0a20 2020 2020 2020  ve: bool.       
-0000d4b0: 203a 7061 7261 6d20 6372 6561 7465 5f61   :param create_a
-0000d4c0: 6e69 6d61 7469 6f6e 3a20 4966 2060 6054  nimation: If ``T
-0000d4d0: 7275 6560 6020 616e 2061 7574 6f6d 6174  rue`` an automat
-0000d4e0: 6564 2061 6e69 6d61 7469 6f6e 206f 6620  ed animation of 
-0000d4f0: 7468 6520 7469 6d65 2065 766f 6c75 7469  the time evoluti
-0000d500: 6f6e 206f 6620 7468 6520 6472 6966 7420  on of the drift 
-0000d510: 736c 6f70 650a 2020 2020 2020 2020 2020  slope.          
-0000d520: 2020 2020 2020 2020 2020 2020 2020 6573                es
-0000d530: 7469 6d61 7465 203a 6d61 7468 3a5c 6861  timate :math:\ha
-0000d540: 747b 5c7a 6574 617d 602c 2074 6865 206e  t{\zeta}`, the n
-0000d550: 6f69 7365 206c 6576 656c 203a 6d61 7468  oise level :math
-0000d560: 3a60 5c68 6174 7b5c 7369 676d 617d 6020  :`\hat{\sigma}` 
-0000d570: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
+0000d150: 2060 6074 6869 6e6e 696e 675f 6279 6060   ``thinning_by``
+0000d160: 2d74 6820 6461 7461 2070 6f69 6e74 2069  -th data point i
+0000d170: 7320 7374 6f72 6564 2e20 4465 6661 756c  s stored. Defaul
+0000d180: 7420 6973 2036 302e 0a20 2020 2020 2020  t is 60..       
+0000d190: 203a 7479 7065 2074 6869 6e6e 696e 675f   :type thinning_
+0000d1a0: 6279 3a20 696e 740a 2020 2020 2020 2020  by: int.        
+0000d1b0: 3a70 6172 616d 2070 7269 6e74 5f70 726f  :param print_pro
+0000d1c0: 6772 6573 733a 2049 6620 6060 5472 7565  gress: If ``True
+0000d1d0: 6060 2074 6865 2070 726f 6772 6573 7320  `` the progress 
+0000d1e0: 6f66 2074 6865 204d 434d 4320 7361 6d70  of the MCMC samp
+0000d1f0: 6c69 6e67 2069 7320 7368 6f77 6e2e 2044  ling is shown. D
+0000d200: 6566 6175 6c74 2069 7320 6060 4661 6c73  efault is ``Fals
+0000d210: 6560 602e 0a20 2020 2020 2020 203a 7479  e``..        :ty
+0000d220: 7065 2070 7269 6e74 5f70 726f 6772 6573  pe print_progres
+0000d230: 733a 2062 6f6f 6c0a 2020 2020 2020 2020  s: bool.        
+0000d240: 3a70 6172 616d 2073 6c6f 7065 5f73 6176  :param slope_sav
+0000d250: 655f 6e61 6d65 3a20 4e61 6d65 206f 6620  e_name: Name of 
+0000d260: 7468 6520 6669 6c65 2069 6e20 7768 6963  the file in whic
+0000d270: 6820 7468 6520 6060 736c 6f70 655f 7374  h the ``slope_st
+0000d280: 6f72 6167 6560 6020 6172 7261 7920 7769  orage`` array wi
+0000d290: 6c6c 2062 6520 7361 7665 642e 2044 6566  ll be saved. Def
+0000d2a0: 6175 6c74 2069 730a 2020 2020 2020 2020  ault is.        
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 6060 6465 6661 756c 745f 7361 7665 5f73  ``default_save_s
+0000d2d0: 6c6f 7065 7360 602e 0a20 2020 2020 2020  lopes``..       
+0000d2e0: 203a 7479 7065 2073 6c6f 7065 5f73 6176   :type slope_sav
+0000d2f0: 655f 6e61 6d65 3a20 7374 720a 2020 2020  e_name: str.    
+0000d300: 2020 2020 3a70 6172 616d 2020 6e6f 6973      :param  nois
+0000d310: 655f 6c65 7665 6c5f 7361 7665 5f6e 616d  e_level_save_nam
+0000d320: 653a 204e 616d 6520 6f66 2074 6865 2066  e: Name of the f
+0000d330: 696c 6520 696e 2077 6869 6368 2074 6865  ile in which the
+0000d340: 2060 606e 6f69 7365 5f6c 6576 656c 5f73   ``noise_level_s
+0000d350: 746f 7261 6765 6060 2061 7272 6179 2077  torage`` array w
+0000d360: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
+0000d370: 2020 2020 2020 2020 2020 2020 6265 2073              be s
+0000d380: 6176 6564 2e20 4465 6661 756c 7420 6973  aved. Default is
+0000d390: 2060 6064 6566 6175 6c74 5f73 6176 655f   ``default_save_
+0000d3a0: 6e6f 6973 6560 602e 0a20 2020 2020 2020  noise``..       
+0000d3b0: 203a 7479 7065 206e 6f69 7365 5f6c 6576   :type noise_lev
+0000d3c0: 656c 5f73 6176 655f 6e61 6d65 3a20 7374  el_save_name: st
+0000d3d0: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
+0000d3e0: 2073 6176 653a 2049 6620 6060 5472 7565   save: If ``True
+0000d3f0: 6060 2074 6865 2060 6073 6c6f 7065 5f73  `` the ``slope_s
+0000d400: 746f 7261 6765 6060 2061 6e64 2074 6865  torage`` and the
+0000d410: 2060 606e 6f69 7365 5f6c 6576 656c 5f73   ``noise_level_s
+0000d420: 746f 7261 6765 6060 2061 7272 6179 7320  torage`` arrays 
+0000d430: 6172 6520 7361 7665 6420 696e 2074 6865  are saved in the
+0000d440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d450: 2020 2020 2020 2020 2065 6e64 206f 6620           end of 
+0000d460: 7468 6520 7363 616e 2069 6e20 616e 2060  the scan in an `
+0000d470: 2e6e 7079 6020 6669 6c65 2e20 4465 6661  .npy` file. Defa
+0000d480: 756c 7420 6973 2060 6054 7275 6560 602e  ult is ``True``.
+0000d490: 0a20 2020 2020 2020 203a 7479 7065 2073  .        :type s
+0000d4a0: 6176 653a 2062 6f6f 6c0a 2020 2020 2020  ave: bool.      
+0000d4b0: 2020 3a70 6172 616d 2063 7265 6174 655f    :param create_
+0000d4c0: 616e 696d 6174 696f 6e3a 2049 6620 6060  animation: If ``
+0000d4d0: 5472 7565 6060 2061 6e20 6175 746f 6d61  True`` an automa
+0000d4e0: 7465 6420 616e 696d 6174 696f 6e20 6f66  ted animation of
+0000d4f0: 2074 6865 2074 696d 6520 6576 6f6c 7574   the time evolut
+0000d500: 696f 6e20 6f66 2074 6865 2064 7269 6674  ion of the drift
+0000d510: 2073 6c6f 7065 0a20 2020 2020 2020 2020   slope.         
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d530: 7374 696d 6174 6520 3a6d 6174 683a 5c68  stimate :math:\h
+0000d540: 6174 7b5c 7a65 7461 7d60 2c20 7468 6520  at{\zeta}`, the 
+0000d550: 6e6f 6973 6520 6c65 7665 6c20 3a6d 6174  noise level :mat
+0000d560: 683a 605c 6861 747b 5c73 6967 6d61 7d60  h:`\hat{\sigma}`
+0000d570: 2061 6e64 2074 6865 0a20 2020 2020 2020   and the.       
 0000d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d590: 6e6f 6973 6520 6b65 726e 656c 2064 656e  noise kernel den
-0000d5a0: 7369 7479 2069 7320 7368 6f77 6e20 746f  sity is shown to
-0000d5b0: 6765 7468 6572 2077 6974 6820 7468 6520  gether with the 
-0000d5c0: 7469 6d65 2073 6572 6965 7320 616e 6420  time series and 
-0000d5d0: 726f 6c6c 696e 670a 2020 2020 2020 2020  rolling.        
+0000d590: 206e 6f69 7365 206b 6572 6e65 6c20 6465   noise kernel de
+0000d5a0: 6e73 6974 7920 6973 2073 686f 776e 2074  nsity is shown t
+0000d5b0: 6f67 6574 6865 7220 7769 7468 2074 6865  ogether with the
+0000d5c0: 2074 696d 6520 7365 7269 6573 2061 6e64   time series and
+0000d5d0: 2072 6f6c 6c69 6e67 0a20 2020 2020 2020   rolling.       
 0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 7769 6e64 6f77 732e 2044 6566 6175 6c74  windows. Default
-0000d600: 2069 7320 6060 4661 6c73 6560 602e 0a0a   is ``False``...
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 2020 2020 2e2e 2077 6172 6e69          .. warni
-0000d630: 6e67 3a3a 0a0a 2020 2020 2020 2020 2020  ng::..          
+0000d5f0: 2077 696e 646f 7773 2e20 4465 6661 756c   windows. Defaul
+0000d600: 7420 6973 2060 6046 616c 7365 6060 2e0a  t is ``False``..
+0000d610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d620: 2020 2020 2020 2020 202e 2e20 7761 726e           .. warn
+0000d630: 696e 673a 3a0a 0a20 2020 2020 2020 2020  ing::..         
 0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2020 4974 206d 616b 6573 2075 7365 206f    It makes use o
-0000d660: 6620 676c 6f62 616c 2076 6172 6961 626c  f global variabl
-0000d670: 6573 2074 6f20 696e 636f 7270 6f72 6174  es to incorporat
-0000d680: 6520 7468 6520 6d6f 7669 6520 616e 696d  e the movie anim
-0000d690: 6174 696f 6e20 746f 6f6c 2069 6e20 7468  ation tool in th
-0000d6a0: 6520 636c 6173 732e 0a20 2020 2020 2020  e class..       
+0000d650: 2020 2049 7420 6d61 6b65 7320 7573 6520     It makes use 
+0000d660: 6f66 2067 6c6f 6261 6c20 7661 7269 6162  of global variab
+0000d670: 6c65 7320 746f 2069 6e63 6f72 706f 7261  les to incorpora
+0000d680: 7465 2074 6865 206d 6f76 6965 2061 6e69  te the movie ani
+0000d690: 6d61 7469 6f6e 2074 6f6f 6c20 696e 2074  mation tool in t
+0000d6a0: 6865 2063 6c61 7373 2e0a 2020 2020 2020  he class..      
 0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 2020 2054 6865 2060 6063 7265 6174       The ``creat
-0000d6d0: 655f 616e 696d 6174 696f 6e60 6020 7061  e_animation`` pa
-0000d6e0: 7261 6d65 7465 7220 6973 206f 6e6c 7920  rameter is only 
-0000d6f0: 696e 7465 6e64 6564 2074 6f20 6561 7369  intended to easi
-0000d700: 6c79 2072 6563 6f6e 7374 7275 6374 0a20  ly reconstruct. 
+0000d6c0: 2020 2020 2020 5468 6520 6060 6372 6561        The ``crea
+0000d6d0: 7465 5f61 6e69 6d61 7469 6f6e 6060 2070  te_animation`` p
+0000d6e0: 6172 616d 6574 6572 2069 7320 6f6e 6c79  arameter is only
+0000d6f0: 2069 6e74 656e 6465 6420 746f 2065 6173   intended to eas
+0000d700: 696c 7920 7265 636f 6e73 7472 7563 740a  ily reconstruct.
 0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d720: 2020 2020 2020 2020 2020 2074 6865 2070             the p
-0000d730: 6c6f 7420 7265 7375 6c74 7320 6f66 2074  lot results of t
-0000d740: 6865 2072 656c 6174 6564 2070 7562 6c69  he related publi
-0000d750: 6361 7469 6f6e 2e20 496e 206f 7468 6572  cation. In other
-0000d760: 2063 6972 6375 6d73 7461 6e63 6573 2069   circumstances i
-0000d770: 7420 7368 6f75 6c64 206e 6f74 0a20 2020  t should not.   
+0000d720: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+0000d730: 706c 6f74 2072 6573 756c 7473 206f 6620  plot results of 
+0000d740: 7468 6520 7265 6c61 7465 6420 7075 626c  the related publ
+0000d750: 6963 6174 696f 6e2e 2049 6e20 6f74 6865  ication. In othe
+0000d760: 7220 6369 7263 756d 7374 616e 6365 7320  r circumstances 
+0000d770: 6974 2073 686f 756c 6420 6e6f 740a 2020  it should not.  
 0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d790: 2020 2020 2020 2020 2062 6520 7573 6564           be used
-0000d7a0: 2069 6e20 6f72 6465 7220 746f 2061 766f   in order to avo
-0000d7b0: 6964 2063 6f6e 666c 6963 7473 2077 6974  id conflicts wit
-0000d7c0: 6820 7468 6520 676c 6f62 616c 2076 6172  h the global var
-0000d7d0: 6961 626c 6520 6e61 6d65 732e 0a0a 2020  iable names...  
-0000d7e0: 2020 2020 2020 3a74 7970 6520 6372 6561        :type crea
-0000d7f0: 7465 5f61 6e69 6d61 7469 6f6e 3a20 626f  te_animation: bo
-0000d800: 6f6c 0a20 2020 2020 2020 203a 7061 7261  ol.        :para
-0000d810: 6d20 616e 695f 7361 7665 5f6e 616d 653a  m ani_save_name:
-0000d820: 2049 6620 6060 6372 6561 7465 5f61 6e69   If ``create_ani
-0000d830: 6d61 7469 6f6e 203d 2054 7275 6560 6020  mation = True`` 
-0000d840: 7468 6520 616e 696d 6174 696f 6e20 6973  the animation is
-0000d850: 2073 6176 6564 2069 6e20 6120 602e 6d70   saved in a `.mp
-0000d860: 3460 2066 696c 6520 7769 7468 2074 6869  4` file with thi
-0000d870: 7320 6e61 6d65 2e0a 2020 2020 2020 2020  s name..        
+0000d790: 2020 2020 2020 2020 2020 6265 2075 7365            be use
+0000d7a0: 6420 696e 206f 7264 6572 2074 6f20 6176  d in order to av
+0000d7b0: 6f69 6420 636f 6e66 6c69 6374 7320 7769  oid conflicts wi
+0000d7c0: 7468 2074 6865 2067 6c6f 6261 6c20 7661  th the global va
+0000d7d0: 7269 6162 6c65 206e 616d 6573 2e0a 0a20  riable names... 
+0000d7e0: 2020 2020 2020 203a 7479 7065 2063 7265         :type cre
+0000d7f0: 6174 655f 616e 696d 6174 696f 6e3a 2062  ate_animation: b
+0000d800: 6f6f 6c0a 2020 2020 2020 2020 3a70 6172  ool.        :par
+0000d810: 616d 2061 6e69 5f73 6176 655f 6e61 6d65  am ani_save_name
+0000d820: 3a20 4966 2060 6063 7265 6174 655f 616e  : If ``create_an
+0000d830: 696d 6174 696f 6e20 3d20 5472 7565 6060  imation = True``
+0000d840: 2074 6865 2061 6e69 6d61 7469 6f6e 2069   the animation i
+0000d850: 7320 7361 7665 6420 696e 2061 2060 2e6d  s saved in a `.m
+0000d860: 7034 6020 6669 6c65 2077 6974 6820 7468  p4` file with th
+0000d870: 6973 206e 616d 652e 0a20 2020 2020 2020  is name..       
 0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d890: 4465 6661 756c 7420 6973 2060 6064 6566  Default is ``def
-0000d8a0: 6175 6c74 5f61 6e69 6d61 7469 6f6e 5f6e  ault_animation_n
-0000d8b0: 616d 6560 602e 0a20 2020 2020 2020 203a  ame``..        :
-0000d8c0: 7479 7065 2061 6e69 5f73 6176 655f 6e61  type ani_save_na
-0000d8d0: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
-0000d8e0: 3a70 6172 616d 2061 6e69 6d61 7469 6f6e  :param animation
-0000d8f0: 5f74 6974 6c65 3a20 4120 7469 746c 6520  _title: A title 
-0000d900: 6361 6e20 6265 2067 6976 656e 2074 6f20  can be given to 
-0000d910: 7468 6520 616e 696d 6174 696f 6e2e 0a20  the animation.. 
-0000d920: 2020 2020 2020 203a 7479 7065 2061 6e69         :type ani
-0000d930: 6d61 7469 6f6e 5f74 6974 6c65 3a20 7374  mation_title: st
-0000d940: 720a 2020 2020 2020 2020 3a70 6172 616d  r.        :param
-0000d950: 206d 6172 6b5f 6372 6974 6963 616c 5f70   mark_critical_p
-0000d960: 6f69 6e74 3a20 4120 7265 6420 646f 7474  oint: A red dott
-0000d970: 6564 2076 6572 7469 6361 6c20 6c69 6e65  ed vertical line
-0000d980: 2069 7320 7368 6f77 6e20 6174 2074 696d   is shown at tim
-0000d990: 6520 6060 6d61 726b 5f63 7269 7469 6361  e ``mark_critica
-0000d9a0: 6c5f 706f 696e 7460 602e 0a20 2020 2020  l_point``..     
+0000d890: 2044 6566 6175 6c74 2069 7320 6060 6465   Default is ``de
+0000d8a0: 6661 756c 745f 616e 696d 6174 696f 6e5f  fault_animation_
+0000d8b0: 6e61 6d65 6060 2e0a 2020 2020 2020 2020  name``..        
+0000d8c0: 3a74 7970 6520 616e 695f 7361 7665 5f6e  :type ani_save_n
+0000d8d0: 616d 653a 2073 7472 0a20 2020 2020 2020  ame: str.       
+0000d8e0: 203a 7061 7261 6d20 616e 696d 6174 696f   :param animatio
+0000d8f0: 6e5f 7469 746c 653a 2041 2074 6974 6c65  n_title: A title
+0000d900: 2063 616e 2062 6520 6769 7665 6e20 746f   can be given to
+0000d910: 2074 6865 2061 6e69 6d61 7469 6f6e 2e0a   the animation..
+0000d920: 2020 2020 2020 2020 3a74 7970 6520 616e          :type an
+0000d930: 696d 6174 696f 6e5f 7469 746c 653a 2073  imation_title: s
+0000d940: 7472 0a20 2020 2020 2020 203a 7061 7261  tr.        :para
+0000d950: 6d20 6d61 726b 5f63 7269 7469 6361 6c5f  m mark_critical_
+0000d960: 706f 696e 743a 2041 2072 6564 2064 6f74  point: A red dot
+0000d970: 7465 6420 7665 7274 6963 616c 206c 696e  ted vertical lin
+0000d980: 6520 6973 2073 686f 776e 2061 7420 7469  e is shown at ti
+0000d990: 6d65 2060 606d 6172 6b5f 6372 6974 6963  me ``mark_critic
+0000d9a0: 616c 5f70 6f69 6e74 6060 2e0a 2020 2020  al_point``..    
 0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 2020 2044 6566 6175 6c74 2069 7320 6060     Default is ``
-0000d9d0: 4e6f 6e65 6060 2e0a 2020 2020 2020 2020  None``..        
-0000d9e0: 3a74 7970 6520 6d61 726b 5f63 7269 7469  :type mark_criti
-0000d9f0: 6361 6c5f 706f 696e 743a 2066 6c6f 6174  cal_point: float
-0000da00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000da10: 6d61 726b 5f6e 6f69 7365 5f6c 6576 656c  mark_noise_level
-0000da20: 3a20 4120 6772 6565 6e20 646f 7474 6564  : A green dotted
-0000da30: 206c 696e 6520 6973 2073 686f 776e 2061   line is shown a
-0000da40: 7420 7468 6520 6e6f 6973 6520 6c65 7665  t the noise leve
-0000da50: 6c20 6060 6d61 726b 5f6e 6f69 7365 5f6c  l ``mark_noise_l
-0000da60: 6576 656c 6060 2069 6e20 7468 650a 2020  evel`` in the.  
+0000d9c0: 2020 2020 4465 6661 756c 7420 6973 2060      Default is `
+0000d9d0: 604e 6f6e 6560 602e 0a20 2020 2020 2020  `None``..       
+0000d9e0: 203a 7479 7065 206d 6172 6b5f 6372 6974   :type mark_crit
+0000d9f0: 6963 616c 5f70 6f69 6e74 3a20 666c 6f61  ical_point: floa
+0000da00: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+0000da10: 206d 6172 6b5f 6e6f 6973 655f 6c65 7665   mark_noise_leve
+0000da20: 6c3a 2041 2067 7265 656e 2064 6f74 7465  l: A green dotte
+0000da30: 6420 6c69 6e65 2069 7320 7368 6f77 6e20  d line is shown 
+0000da40: 6174 2074 6865 206e 6f69 7365 206c 6576  at the noise lev
+0000da50: 656c 2060 606d 6172 6b5f 6e6f 6973 655f  el ``mark_noise_
+0000da60: 6c65 7665 6c60 6020 696e 2074 6865 0a20  level`` in the. 
 0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2020 2020 2020 6e6f 6973 6520 6b65 726e        noise kern
-0000da90: 656c 2064 656e 7369 7479 2070 6c6f 7420  el density plot 
-0000daa0: 616e 6420 7468 6520 7469 6d65 2065 766f  and the time evo
-0000dab0: 6c75 7469 6f6e 2070 6c6f 7420 6f66 2074  lution plot of t
-0000dac0: 6865 206e 6f69 7365 206c 6576 656c 2e0a  he noise level..
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0000daf0: 6973 2060 604e 6f6e 6560 602e 0a20 2020  is ``None``..   
-0000db00: 2020 2020 203a 7479 7065 206d 6172 6b5f       :type mark_
-0000db10: 6e6f 6973 655f 6c65 7665 6c3a 2066 6c6f  noise_level: flo
-0000db20: 6174 0a20 2020 2020 2020 203a 7061 7261  at.        :para
-0000db30: 6d20 6465 7472 656e 6469 6e67 5f70 6572  m detrending_per
-0000db40: 5f77 696e 646f 773a 2044 6566 6175 6c74  _window: Default
-0000db50: 2069 7320 6060 4e6f 6e65 6060 2e20 4966   is ``None``. If
-0000db60: 2060 6027 6c69 6e65 6172 2760 6020 7468   ``'linear'`` th
-0000db70: 6520 6060 6461 7461 5f77 696e 646f 7760  e ``data_window`
-0000db80: 6020 6973 2064 6574 7265 6e64 6564 206c  ` is detrended l
-0000db90: 696e 6561 726c 792e 2049 660a 2020 2020  inearly. If.    
+0000da80: 2020 2020 2020 206e 6f69 7365 206b 6572         noise ker
+0000da90: 6e65 6c20 6465 6e73 6974 7920 706c 6f74  nel density plot
+0000daa0: 2061 6e64 2074 6865 2074 696d 6520 6576   and the time ev
+0000dab0: 6f6c 7574 696f 6e20 706c 6f74 206f 6620  olution plot of 
+0000dac0: 7468 6520 6e6f 6973 6520 6c65 7665 6c2e  the noise level.
+0000dad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dae0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+0000daf0: 2069 7320 6060 4e6f 6e65 6060 2e0a 2020   is ``None``..  
+0000db00: 2020 2020 2020 3a74 7970 6520 6d61 726b        :type mark
+0000db10: 5f6e 6f69 7365 5f6c 6576 656c 3a20 666c  _noise_level: fl
+0000db20: 6f61 740a 2020 2020 2020 2020 3a70 6172  oat.        :par
+0000db30: 616d 2064 6574 7265 6e64 696e 675f 7065  am detrending_pe
+0000db40: 725f 7769 6e64 6f77 3a20 4465 6661 756c  r_window: Defaul
+0000db50: 7420 6973 2060 604e 6f6e 6560 602e 2049  t is ``None``. I
+0000db60: 6620 6060 276c 696e 6561 7227 6060 2074  f ``'linear'`` t
+0000db70: 6865 2060 6064 6174 615f 7769 6e64 6f77  he ``data_window
+0000db80: 6060 2069 7320 6465 7472 656e 6465 6420  `` is detrended 
+0000db90: 6c69 6e65 6172 6c79 2e20 4966 0a20 2020  linearly. If.   
 0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbb0: 2020 2020 6060 4761 7573 7369 616e 206b      ``Gaussian k
-0000dbc0: 6572 6e65 6c20 736d 6f6f 7468 6564 6060  ernel smoothed``
-0000dbd0: 2061 2047 6175 7373 6961 6e20 736d 6f6f   a Gaussian smoo
-0000dbe0: 7468 6564 2063 7572 7665 2069 7320 7375  thed curve is su
-0000dbf0: 6274 7261 6374 6564 2066 726f 6d20 7468  btracted from th
-0000dc00: 6520 6060 6461 7461 5f77 696e 646f 7760  e ``data_window`
-0000dc10: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
-0000dc20: 2020 2020 2020 2020 2020 2054 6865 2070             The p
-0000dc30: 6172 616d 6574 6572 7320 6f66 2074 6865  arameters of the
-0000dc40: 206b 6572 6e65 6c20 736d 6f6f 7468 696e   kernel smoothin
-0000dc50: 6720 6361 6e20 6265 2073 6574 2062 7920  g can be set by 
-0000dc60: 6060 6761 7573 735f 6669 6c74 6572 5f6d  ``gauss_filter_m
-0000dc70: 6f64 6560 602c 2060 6067 6175 7373 5f66  ode``, ``gauss_f
-0000dc80: 696c 7465 725f 7369 676d 6160 602c 0a20  ilter_sigma``,. 
+0000dbb0: 2020 2020 2060 6047 6175 7373 6961 6e20       ``Gaussian 
+0000dbc0: 6b65 726e 656c 2073 6d6f 6f74 6865 6460  kernel smoothed`
+0000dbd0: 6020 6120 4761 7573 7369 616e 2073 6d6f  ` a Gaussian smo
+0000dbe0: 6f74 6865 6420 6375 7276 6520 6973 2073  othed curve is s
+0000dbf0: 7562 7472 6163 7465 6420 6672 6f6d 2074  ubtracted from t
+0000dc00: 6865 2060 6064 6174 615f 7769 6e64 6f77  he ``data_window
+0000dc10: 6060 2e0a 2020 2020 2020 2020 2020 2020  ``..            
+0000dc20: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000dc30: 7061 7261 6d65 7465 7273 206f 6620 7468  parameters of th
+0000dc40: 6520 6b65 726e 656c 2073 6d6f 6f74 6869  e kernel smoothi
+0000dc50: 6e67 2063 616e 2062 6520 7365 7420 6279  ng can be set by
+0000dc60: 2060 6067 6175 7373 5f66 696c 7465 725f   ``gauss_filter_
+0000dc70: 6d6f 6465 6060 2c20 6060 6761 7573 735f  mode``, ``gauss_
+0000dc80: 6669 6c74 6572 5f73 6967 6d61 6060 2c0a  filter_sigma``,.
 0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2020 2020 2060 6067 6175 7373 5f66         ``gauss_f
-0000dcb0: 696c 7465 725f 6f72 6465 7260 602c 2060  ilter_order``, `
-0000dcc0: 6067 6175 7373 5f66 696c 7465 725f 6376  `gauss_filter_cv
-0000dcd0: 616c 6060 2061 6e64 2060 6067 6175 7373  al`` and ``gauss
-0000dce0: 5f66 696c 7465 725f 7472 756e 6361 7465  _filter_truncate
-0000dcf0: 6060 2e0a 2020 2020 2020 2020 3a74 7970  ``..        :typ
-0000dd00: 6520 6465 7472 656e 6469 6e67 5f6f 665f  e detrending_of_
-0000dd10: 7768 6f6c 655f 6461 7461 7365 743a 2073  whole_dataset: s
-0000dd20: 7472 0a20 2020 2020 2020 203a 7061 7261  tr.        :para
-0000dd30: 6d20 6761 7573 735f 6669 6c74 6572 5f6d  m gauss_filter_m
-0000dd40: 6f64 653a 2041 6363 6f72 6469 6e67 2074  ode: According t
-0000dd50: 6f20 7468 6520 6060 7363 6970 792e 6e64  o the ``scipy.nd
-0000dd60: 696d 6167 652e 6669 6c74 6572 732e 6761  image.filters.ga
-0000dd70: 7573 7369 616e 5f66 696c 7465 7260 6020  ussian_filter`` 
-0000dd80: 6f70 7469 6f6e 2e0a 2020 2020 2020 2020  option..        
-0000dd90: 3a74 7970 6520 6761 7573 735f 6669 6c74  :type gauss_filt
-0000dda0: 6572 5f6d 6f64 653a 2073 7472 0a20 2020  er_mode: str.   
-0000ddb0: 2020 2020 203a 7061 7261 6d20 6761 7573       :param gaus
-0000ddc0: 735f 6669 6c74 6572 5f73 6967 6d61 3a20  s_filter_sigma: 
-0000ddd0: 4163 636f 7264 696e 6720 746f 2074 6865  According to the
-0000dde0: 2060 6073 6369 7079 2e6e 6469 6d61 6765   ``scipy.ndimage
-0000ddf0: 2e66 696c 7465 7273 2e67 6175 7373 6961  .filters.gaussia
-0000de00: 6e5f 6669 6c74 6572 6060 206f 7074 696f  n_filter`` optio
-0000de10: 6e2e 0a20 2020 2020 2020 203a 7479 7065  n..        :type
-0000de20: 2067 6175 7373 5f66 696c 7465 725f 7369   gauss_filter_si
-0000de30: 676d 613a 2066 6c6f 6174 0a20 2020 2020  gma: float.     
-0000de40: 2020 203a 7061 7261 6d20 6761 7573 735f     :param gauss_
-0000de50: 6669 6c74 6572 5f6f 7264 6572 3a20 4163  filter_order: Ac
-0000de60: 636f 7264 696e 6720 746f 2074 6865 2060  cording to the `
-0000de70: 6073 6369 7079 2e6e 6469 6d61 6765 2e66  `scipy.ndimage.f
-0000de80: 696c 7465 7273 2e67 6175 7373 6961 6e5f  ilters.gaussian_
-0000de90: 6669 6c74 6572 6060 206f 7074 696f 6e2e  filter`` option.
-0000dea0: 0a20 2020 2020 2020 203a 7479 7065 2067  .        :type g
-0000deb0: 6175 7373 5f66 696c 7465 725f 6f72 6465  auss_filter_orde
-0000dec0: 723a 2069 6e74 0a20 2020 2020 2020 203a  r: int.        :
-0000ded0: 7061 7261 6d20 6761 7573 735f 6669 6c74  param gauss_filt
-0000dee0: 6572 5f63 7661 6c3a 2041 6363 6f72 6469  er_cval: Accordi
-0000def0: 6e67 2074 6f20 7468 6520 6060 7363 6970  ng to the ``scip
-0000df00: 792e 6e64 696d 6167 652e 6669 6c74 6572  y.ndimage.filter
-0000df10: 732e 6761 7573 7369 616e 5f66 696c 7465  s.gaussian_filte
-0000df20: 7260 6020 6f70 7469 6f6e 2e0a 2020 2020  r`` option..    
-0000df30: 2020 2020 3a74 7970 6520 6761 7573 735f      :type gauss_
-0000df40: 6669 6c74 6572 5f63 7661 6c3a 2066 6c6f  filter_cval: flo
-0000df50: 6174 0a20 2020 2020 2020 203a 7061 7261  at.        :para
-0000df60: 6d20 6761 7573 735f 6669 6c74 6572 5f74  m gauss_filter_t
-0000df70: 7275 6e63 6174 653a 2041 6363 6f72 6469  runcate: Accordi
-0000df80: 6e67 2074 6f20 7468 6520 6060 7363 6970  ng to the ``scip
-0000df90: 792e 6e64 696d 6167 652e 6669 6c74 6572  y.ndimage.filter
-0000dfa0: 732e 6761 7573 7369 616e 5f66 696c 7465  s.gaussian_filte
-0000dfb0: 7260 6020 6f70 7469 6f6e 2e0a 2020 2020  r`` option..    
-0000dfc0: 2020 2020 3a74 7970 6520 6761 7573 735f      :type gauss_
-0000dfd0: 6669 6c74 6572 5f74 7275 6e63 6174 653a  filter_truncate:
-0000dfe0: 2066 6c6f 6174 0a20 2020 2020 2020 203a   float.        :
-0000dff0: 7061 7261 6d20 706c 6f74 5f64 6574 7265  param plot_detre
-0000e000: 6e64 696e 673a 2044 6566 6175 6c74 2069  nding: Default i
-0000e010: 7320 6060 4661 6c73 6560 602e 2049 6620  s ``False``. If 
-0000e020: 6060 5472 7565 6060 2c20 7468 6520 6060  ``True``, the ``
-0000e030: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
-0000e040: 6060 2061 7320 7765 6c6c 2061 7320 7468  `` as well as th
-0000e050: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000e060: 2020 2020 2020 2020 2020 6060 7365 6c66            ``self
-0000e070: 2e73 6c6f 775f 7472 656e 6460 6020 616e  .slow_trend`` an
-0000e080: 6420 7468 6520 6465 7472 656e 6465 6420  d the detrended 
-0000e090: 7665 7273 696f 6e20 6172 6520 7368 6f77  version are show
-0000e0a0: 6e2e 0a20 2020 2020 2020 203a 7479 7065  n..        :type
-0000e0b0: 2070 6c6f 745f 6465 7472 656e 6469 6e67   plot_detrending
-0000e0c0: 3a20 626f 6f6c 0a20 2020 2020 2020 203a  : bool.        :
-0000e0d0: 7061 7261 6d20 4d43 4d43 5f70 6172 616c  param MCMC_paral
-0000e0e0: 6c65 6c69 7a61 7469 6f6e 5f6d 6574 686f  lelization_metho
-0000e0f0: 643a 2044 6566 6175 6c74 2069 7320 604e  d: Default is `N
-0000e100: 6f6e 6560 2e20 4966 2060 4e6f 6e65 6020  one`. If `None` 
-0000e110: 7468 6520 6261 7369 6320 7365 7269 616c  the basic serial
-0000e120: 204d 434d 4320 636f 6d70 7574 6174 696f   MCMC computatio
-0000e130: 6e20 6973 2070 6572 666f 726d 6564 2e20  n is performed. 
-0000e140: 4966 0a20 2020 2020 2020 2020 2020 2020  If.             
-0000e150: 2020 2020 2020 2020 2020 2060 604d 434d             ``MCM
-0000e160: 435f 7061 7261 6c6c 656c 697a 6174 696f  C_parallelizatio
-0000e170: 6e5f 6d65 7468 6f64 203d 2027 6d75 6c74  n_method = 'mult
-0000e180: 6970 726f 6365 7373 696e 6727 6060 2c20  iprocessing'``, 
-0000e190: 6120 6d75 6c74 6970 726f 6365 7373 696e  a multiprocessin
-0000e1a0: 6720 706f 6f6c 2077 6974 6820 606e 756d  g pool with `num
-0000e1b0: 5f70 726f 6365 7373 6573 600a 2020 2020  _processes`.    
+0000dca0: 2020 2020 2020 2020 6060 6761 7573 735f          ``gauss_
+0000dcb0: 6669 6c74 6572 5f6f 7264 6572 6060 2c20  filter_order``, 
+0000dcc0: 6060 6761 7573 735f 6669 6c74 6572 5f63  ``gauss_filter_c
+0000dcd0: 7661 6c60 6020 616e 6420 6060 6761 7573  val`` and ``gaus
+0000dce0: 735f 6669 6c74 6572 5f74 7275 6e63 6174  s_filter_truncat
+0000dcf0: 6560 602e 0a20 2020 2020 2020 203a 7479  e``..        :ty
+0000dd00: 7065 2064 6574 7265 6e64 696e 675f 6f66  pe detrending_of
+0000dd10: 5f77 686f 6c65 5f64 6174 6173 6574 3a20  _whole_dataset: 
+0000dd20: 7374 720a 2020 2020 2020 2020 3a70 6172  str.        :par
+0000dd30: 616d 2067 6175 7373 5f66 696c 7465 725f  am gauss_filter_
+0000dd40: 6d6f 6465 3a20 4163 636f 7264 696e 6720  mode: According 
+0000dd50: 746f 2074 6865 2060 6073 6369 7079 2e6e  to the ``scipy.n
+0000dd60: 6469 6d61 6765 2e66 696c 7465 7273 2e67  dimage.filters.g
+0000dd70: 6175 7373 6961 6e5f 6669 6c74 6572 6060  aussian_filter``
+0000dd80: 206f 7074 696f 6e2e 0a20 2020 2020 2020   option..       
+0000dd90: 203a 7479 7065 2067 6175 7373 5f66 696c   :type gauss_fil
+0000dda0: 7465 725f 6d6f 6465 3a20 7374 720a 2020  ter_mode: str.  
+0000ddb0: 2020 2020 2020 3a70 6172 616d 2067 6175        :param gau
+0000ddc0: 7373 5f66 696c 7465 725f 7369 676d 613a  ss_filter_sigma:
+0000ddd0: 2041 6363 6f72 6469 6e67 2074 6f20 7468   According to th
+0000dde0: 6520 6060 7363 6970 792e 6e64 696d 6167  e ``scipy.ndimag
+0000ddf0: 652e 6669 6c74 6572 732e 6761 7573 7369  e.filters.gaussi
+0000de00: 616e 5f66 696c 7465 7260 6020 6f70 7469  an_filter`` opti
+0000de10: 6f6e 2e0a 2020 2020 2020 2020 3a74 7970  on..        :typ
+0000de20: 6520 6761 7573 735f 6669 6c74 6572 5f73  e gauss_filter_s
+0000de30: 6967 6d61 3a20 666c 6f61 740a 2020 2020  igma: float.    
+0000de40: 2020 2020 3a70 6172 616d 2067 6175 7373      :param gauss
+0000de50: 5f66 696c 7465 725f 6f72 6465 723a 2041  _filter_order: A
+0000de60: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+0000de70: 6060 7363 6970 792e 6e64 696d 6167 652e  ``scipy.ndimage.
+0000de80: 6669 6c74 6572 732e 6761 7573 7369 616e  filters.gaussian
+0000de90: 5f66 696c 7465 7260 6020 6f70 7469 6f6e  _filter`` option
+0000dea0: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+0000deb0: 6761 7573 735f 6669 6c74 6572 5f6f 7264  gauss_filter_ord
+0000dec0: 6572 3a20 696e 740a 2020 2020 2020 2020  er: int.        
+0000ded0: 3a70 6172 616d 2067 6175 7373 5f66 696c  :param gauss_fil
+0000dee0: 7465 725f 6376 616c 3a20 4163 636f 7264  ter_cval: Accord
+0000def0: 696e 6720 746f 2074 6865 2060 6073 6369  ing to the ``sci
+0000df00: 7079 2e6e 6469 6d61 6765 2e66 696c 7465  py.ndimage.filte
+0000df10: 7273 2e67 6175 7373 6961 6e5f 6669 6c74  rs.gaussian_filt
+0000df20: 6572 6060 206f 7074 696f 6e2e 0a20 2020  er`` option..   
+0000df30: 2020 2020 203a 7479 7065 2067 6175 7373       :type gauss
+0000df40: 5f66 696c 7465 725f 6376 616c 3a20 666c  _filter_cval: fl
+0000df50: 6f61 740a 2020 2020 2020 2020 3a70 6172  oat.        :par
+0000df60: 616d 2067 6175 7373 5f66 696c 7465 725f  am gauss_filter_
+0000df70: 7472 756e 6361 7465 3a20 4163 636f 7264  truncate: Accord
+0000df80: 696e 6720 746f 2074 6865 2060 6073 6369  ing to the ``sci
+0000df90: 7079 2e6e 6469 6d61 6765 2e66 696c 7465  py.ndimage.filte
+0000dfa0: 7273 2e67 6175 7373 6961 6e5f 6669 6c74  rs.gaussian_filt
+0000dfb0: 6572 6060 206f 7074 696f 6e2e 0a20 2020  er`` option..   
+0000dfc0: 2020 2020 203a 7479 7065 2067 6175 7373       :type gauss
+0000dfd0: 5f66 696c 7465 725f 7472 756e 6361 7465  _filter_truncate
+0000dfe0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+0000dff0: 3a70 6172 616d 2070 6c6f 745f 6465 7472  :param plot_detr
+0000e000: 656e 6469 6e67 3a20 4465 6661 756c 7420  ending: Default 
+0000e010: 6973 2060 6046 616c 7365 6060 2e20 4966  is ``False``. If
+0000e020: 2060 6054 7275 6560 602c 2074 6865 2060   ``True``, the `
+0000e030: 6073 656c 662e 6461 7461 5f77 696e 646f  `self.data_windo
+0000e040: 7760 6020 6173 2077 656c 6c20 6173 2074  w`` as well as t
+0000e050: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+0000e060: 2020 2020 2020 2020 2020 2060 6073 656c             ``sel
+0000e070: 662e 736c 6f77 5f74 7265 6e64 6060 2061  f.slow_trend`` a
+0000e080: 6e64 2074 6865 2064 6574 7265 6e64 6564  nd the detrended
+0000e090: 2076 6572 7369 6f6e 2061 7265 2073 686f   version are sho
+0000e0a0: 776e 2e0a 2020 2020 2020 2020 3a74 7970  wn..        :typ
+0000e0b0: 6520 706c 6f74 5f64 6574 7265 6e64 696e  e plot_detrendin
+0000e0c0: 673a 2062 6f6f 6c0a 2020 2020 2020 2020  g: bool.        
+0000e0d0: 3a70 6172 616d 204d 434d 435f 7061 7261  :param MCMC_para
+0000e0e0: 6c6c 656c 697a 6174 696f 6e5f 6d65 7468  llelization_meth
+0000e0f0: 6f64 3a20 4465 6661 756c 7420 6973 2060  od: Default is `
+0000e100: 4e6f 6e65 602e 2049 6620 604e 6f6e 6560  None`. If `None`
+0000e110: 2074 6865 2062 6173 6963 2073 6572 6961   the basic seria
+0000e120: 6c20 4d43 4d43 2063 6f6d 7075 7461 7469  l MCMC computati
+0000e130: 6f6e 2069 7320 7065 7266 6f72 6d65 642e  on is performed.
+0000e140: 2049 660a 2020 2020 2020 2020 2020 2020   If.            
+0000e150: 2020 2020 2020 2020 2020 2020 6060 4d43              ``MC
+0000e160: 4d43 5f70 6172 616c 6c65 6c69 7a61 7469  MC_parallelizati
+0000e170: 6f6e 5f6d 6574 686f 6420 3d20 276d 756c  on_method = 'mul
+0000e180: 7469 7072 6f63 6573 7369 6e67 2760 602c  tiprocessing'``,
+0000e190: 2061 206d 756c 7469 7072 6f63 6573 7369   a multiprocessi
+0000e1a0: 6e67 2070 6f6f 6c20 7769 7468 2060 6e75  ng pool with `nu
+0000e1b0: 6d5f 7072 6f63 6573 7365 7360 0a20 2020  m_processes`.   
 0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1d0: 2020 2020 6973 2075 7365 6420 746f 2061      is used to a
-0000e1e0: 6363 656c 6572 6174 6520 4d43 4d43 2073  ccelerate MCMC s
-0000e1f0: 616d 706c 696e 672e 2049 6620 6060 4d43  ampling. If ``MC
-0000e200: 4d43 5f70 6172 616c 6c65 6c69 7a61 7469  MC_parallelizati
-0000e210: 6f6e 5f6d 6574 686f 6420 3d20 2763 686f  on_method = 'cho
-0000e220: 705f 6368 6169 6e27 6060 2069 7320 7573  p_chain'`` is us
-0000e230: 6564 2c20 7468 650a 2020 2020 2020 2020  ed, the.        
+0000e1d0: 2020 2020 2069 7320 7573 6564 2074 6f20       is used to 
+0000e1e0: 6163 6365 6c65 7261 7465 204d 434d 4320  accelerate MCMC 
+0000e1f0: 7361 6d70 6c69 6e67 2e20 4966 2060 604d  sampling. If ``M
+0000e200: 434d 435f 7061 7261 6c6c 656c 697a 6174  CMC_parallelizat
+0000e210: 696f 6e5f 6d65 7468 6f64 203d 2027 6368  ion_method = 'ch
+0000e220: 6f70 5f63 6861 696e 2760 6020 6973 2075  op_chain'`` is u
+0000e230: 7365 642c 2074 6865 0a20 2020 2020 2020  sed, the.       
 0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e250: 746f 7461 6c20 6c65 6e67 7468 206f 6620  total length of 
-0000e260: 7468 6520 6465 7369 7265 6420 4d61 726b  the desired Mark
-0000e270: 6f76 2063 6861 696e 2069 7320 6469 7669  ov chain is divi
-0000e280: 6465 6420 696e 746f 2060 6027 6368 6f70  ded into ``'chop
-0000e290: 5f63 6861 696e 2760 6020 7061 7274 7320  _chain'`` parts 
-0000e2a0: 6561 6368 206f 6620 7768 6963 6820 6973  each of which is
-0000e2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e2c0: 2020 2020 2020 2020 2073 616d 706c 6564           sampled
-0000e2d0: 2069 6e20 7061 7261 6c6c 656c 2061 6e64   in parallel and
-0000e2e0: 206a 6f69 6e65 6420 746f 6765 7468 6572   joined together
-0000e2f0: 2069 6e20 7468 6520 656e 642e 0a20 2020   in the end..   
-0000e300: 2020 2020 203a 7479 7065 204d 434d 435f       :type MCMC_
-0000e310: 7061 7261 6c6c 656c 697a 6174 696f 6e5f  parallelization_
-0000e320: 6d65 7468 6f64 3a20 7374 720a 2020 2020  method: str.    
-0000e330: 2020 2020 3a70 6172 616d 206e 756d 5f70      :param num_p
-0000e340: 726f 6365 7373 6573 3a20 4465 6661 756c  rocesses: Defaul
-0000e350: 7420 6973 2060 604e 6f6e 6560 602e 2049  t is ``None``. I
-0000e360: 6620 6060 2768 616c 6660 602c 2061 6c6d  f ``'half``, alm
-0000e370: 6f73 7420 6861 6c66 206f 6620 7468 6520  ost half of the 
-0000e380: 4350 5520 6b65 726e 656c 7320 6172 6520  CPU kernels are 
-0000e390: 7573 6564 2e20 4966 2060 6027 616c 6c27  used. If ``'all'
-0000e3a0: 6060 2c0a 2020 2020 2020 2020 2020 2020  ``,.            
-0000e3b0: 2020 2020 2020 2020 2020 2020 616c 6c20              all 
-0000e3c0: 4350 5520 6b65 726e 656c 7320 6172 6520  CPU kernels are 
-0000e3d0: 7573 6564 2e20 4966 2069 6e74 6567 6572  used. If integer
-0000e3e0: 206e 756d 6265 722c 2074 6865 2064 6566   number, the def
-0000e3f0: 696e 6564 206e 756d 6265 7220 6f66 2043  ined number of C
-0000e400: 5055 206b 6572 6e65 6c73 2069 7320 7573  PU kernels is us
-0000e410: 6564 2066 6f72 0a20 2020 2020 2020 2020  ed for.         
-0000e420: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000e430: 756c 7469 7072 6f63 6573 7369 6e67 2e0a  ultiprocessing..
-0000e440: 2020 2020 2020 2020 3a74 7970 6520 6e75          :type nu
-0000e450: 6d5f 7072 6f63 6573 7365 733a 2073 7472  m_processes: str
-0000e460: 206f 7220 696e 740a 2020 2020 2020 2020   or int.        
-0000e470: 3a70 6172 616d 206e 756d 5f63 686f 705f  :param num_chop_
-0000e480: 6368 6169 6e73 3a20 4e75 6d62 6572 2062  chains: Number b
-0000e490: 7920 7768 6963 6820 7468 6520 746f 7461  y which the tota
-0000e4a0: 6c20 6c65 6e67 7468 206f 6620 7468 6520  l length of the 
-0000e4b0: 4d61 726b 6f76 2063 6861 696e 2069 7320  Markov chain is 
-0000e4c0: 6469 7669 6465 642e 2045 6163 6820 736c  divided. Each sl
-0000e4d0: 6963 6520 6973 2073 616d 706c 6564 0a20  ice is sampled. 
+0000e250: 2074 6f74 616c 206c 656e 6774 6820 6f66   total length of
+0000e260: 2074 6865 2064 6573 6972 6564 204d 6172   the desired Mar
+0000e270: 6b6f 7620 6368 6169 6e20 6973 2064 6976  kov chain is div
+0000e280: 6964 6564 2069 6e74 6f20 6060 2763 686f  ided into ``'cho
+0000e290: 705f 6368 6169 6e27 6060 2070 6172 7473  p_chain'`` parts
+0000e2a0: 2065 6163 6820 6f66 2077 6869 6368 2069   each of which i
+0000e2b0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000e2c0: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
+0000e2d0: 6420 696e 2070 6172 616c 6c65 6c20 616e  d in parallel an
+0000e2e0: 6420 6a6f 696e 6564 2074 6f67 6574 6865  d joined togethe
+0000e2f0: 7220 696e 2074 6865 2065 6e64 2e0a 2020  r in the end..  
+0000e300: 2020 2020 2020 3a74 7970 6520 4d43 4d43        :type MCMC
+0000e310: 5f70 6172 616c 6c65 6c69 7a61 7469 6f6e  _parallelization
+0000e320: 5f6d 6574 686f 643a 2073 7472 0a20 2020  _method: str.   
+0000e330: 2020 2020 203a 7061 7261 6d20 6e75 6d5f       :param num_
+0000e340: 7072 6f63 6573 7365 733a 2044 6566 6175  processes: Defau
+0000e350: 6c74 2069 7320 6060 4e6f 6e65 6060 2e20  lt is ``None``. 
+0000e360: 4966 2060 6027 6861 6c66 6060 2c20 616c  If ``'half``, al
+0000e370: 6d6f 7374 2068 616c 6620 6f66 2074 6865  most half of the
+0000e380: 2043 5055 206b 6572 6e65 6c73 2061 7265   CPU kernels are
+0000e390: 2075 7365 642e 2049 6620 6060 2761 6c6c   used. If ``'all
+0000e3a0: 2760 602c 0a20 2020 2020 2020 2020 2020  '``,.           
+0000e3b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+0000e3c0: 2043 5055 206b 6572 6e65 6c73 2061 7265   CPU kernels are
+0000e3d0: 2075 7365 642e 2049 6620 696e 7465 6765   used. If intege
+0000e3e0: 7220 6e75 6d62 6572 2c20 7468 6520 6465  r number, the de
+0000e3f0: 6669 6e65 6420 6e75 6d62 6572 206f 6620  fined number of 
+0000e400: 4350 5520 6b65 726e 656c 7320 6973 2075  CPU kernels is u
+0000e410: 7365 6420 666f 720a 2020 2020 2020 2020  sed for.        
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 6d75 6c74 6970 726f 6365 7373 696e 672e  multiprocessing.
+0000e440: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+0000e450: 756d 5f70 726f 6365 7373 6573 3a20 7374  um_processes: st
+0000e460: 7220 6f72 2069 6e74 0a20 2020 2020 2020  r or int.       
+0000e470: 203a 7061 7261 6d20 6e75 6d5f 6368 6f70   :param num_chop
+0000e480: 5f63 6861 696e 733a 204e 756d 6265 7220  _chains: Number 
+0000e490: 6279 2077 6869 6368 2074 6865 2074 6f74  by which the tot
+0000e4a0: 616c 206c 656e 6774 6820 6f66 2074 6865  al length of the
+0000e4b0: 204d 6172 6b6f 7620 6368 6169 6e20 6973   Markov chain is
+0000e4c0: 2064 6976 6964 6564 2e20 4561 6368 2073   divided. Each s
+0000e4d0: 6c69 6365 2069 7320 7361 6d70 6c65 640a  lice is sampled.
 0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 2020 2020 2020 2069 6e20 7061 7261 6c6c         in parall
-0000e500: 656c 2061 6e64 206a 6f69 6e65 6420 746f  el and joined to
-0000e510: 6765 7468 6572 2069 6e20 7468 6520 656e  gether in the en
-0000e520: 6420 6f66 2074 6865 2063 616c 6375 6c61  d of the calcula
-0000e530: 7469 6f6e 732e 0a20 2020 2020 2020 203a  tions..        :
-0000e540: 7479 7065 206e 756d 5f63 686f 705f 6368  type num_chop_ch
-0000e550: 6169 6e73 3a20 696e 740a 0a20 2020 2020  ains: int..     
-0000e560: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-0000e570: 6372 6564 5f70 6572 6365 6e74 696c 6573  cred_percentiles
-0000e580: 203d 206e 702e 6172 7261 7928 6372 6564   = np.array(cred
-0000e590: 5f70 6572 6365 6e74 696c 6573 290a 2020  _percentiles).  
-0000e5a0: 2020 2020 2020 7365 6c66 2e77 696e 646f        self.windo
-0000e5b0: 775f 7369 7a65 203d 2077 696e 646f 775f  w_size = window_
-0000e5c0: 7369 7a65 0a20 2020 2020 2020 2073 656c  size.        sel
-0000e5d0: 662e 7769 6e64 6f77 5f73 6869 6674 203d  f.window_shift =
-0000e5e0: 2077 696e 646f 775f 7368 6966 740a 2020   window_shift.  
-0000e5f0: 2020 2020 2020 7365 6c66 2e64 6174 615f        self.data_
-0000e600: 7769 6e64 6f77 203d 206e 702e 7a65 726f  window = np.zero
-0000e610: 7328 7769 6e64 6f77 5f73 697a 6529 0a20  s(window_size). 
-0000e620: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-0000e630: 5f77 696e 646f 7720 3d20 6e70 2e7a 6572  _window = np.zer
-0000e640: 6f73 2877 696e 646f 775f 7369 7a65 290a  os(window_size).
-0000e650: 2020 2020 2020 2020 7365 6c66 2e69 6e63          self.inc
-0000e660: 7265 6d65 6e74 7320 3d20 6e70 2e7a 6572  rements = np.zer
-0000e670: 6f73 2877 696e 646f 775f 7369 7a65 202d  os(window_size -
-0000e680: 2031 290a 2020 2020 2020 2020 7365 6c66   1).        self
-0000e690: 2e6e 7761 6c6b 6572 7320 3d20 6e77 616c  .nwalkers = nwal
-0000e6a0: 6b65 7273 0a20 2020 2020 2020 2073 656c  kers.        sel
-0000e6b0: 662e 6e73 7465 7073 203d 206e 7374 6570  f.nsteps = nstep
-0000e6c0: 730a 2020 2020 2020 2020 7365 6c66 2e6e  s.        self.n
-0000e6d0: 6275 726e 203d 206e 6275 726e 0a20 2020  burn = nburn.   
-0000e6e0: 2020 2020 2073 656c 662e 6c6f 6f70 5f72       self.loop_r
-0000e6f0: 616e 6765 203d 206e 702e 6172 616e 6765  ange = np.arange
-0000e700: 2830 2c20 7365 6c66 2e64 6174 615f 7369  (0, self.data_si
-0000e710: 7a65 202d 2073 656c 662e 7769 6e64 6f77  ze - self.window
-0000e720: 5f73 697a 652c 2073 656c 662e 7769 6e64  _size, self.wind
-0000e730: 6f77 5f73 6869 6674 290a 2020 2020 2020  ow_shift).      
-0000e740: 2020 7365 6c66 2e73 6c6f 7065 5f73 746f    self.slope_sto
-0000e750: 7261 6765 203d 206e 702e 7a65 726f 7328  rage = np.zeros(
-0000e760: 2835 2c20 7365 6c66 2e6c 6f6f 705f 7261  (5, self.loop_ra
-0000e770: 6e67 652e 7369 7a65 2929 0a20 2020 2020  nge.size)).     
-0000e780: 2020 2073 656c 662e 6e6f 6973 655f 6c65     self.noise_le
-0000e790: 7665 6c5f 7374 6f72 6167 6520 3d20 6e70  vel_storage = np
-0000e7a0: 2e7a 6572 6f73 2828 352c 2073 656c 662e  .zeros((5, self.
-0000e7b0: 6c6f 6f70 5f72 616e 6765 2e73 697a 6529  loop_range.size)
-0000e7c0: 290a 2020 2020 2020 2020 6966 2063 7265  ).        if cre
-0000e7d0: 6174 655f 616e 696d 6174 696f 6e20 3d3d  ate_animation ==
-0000e7e0: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
-0000e7f0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000e800: 6765 2873 656c 662e 6c6f 6f70 5f72 616e  ge(self.loop_ran
-0000e810: 6765 2e73 697a 6529 3a0a 2020 2020 2020  ge.size):.      
-0000e820: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0000e830: 696e 646f 775f 7368 6966 7420 3d20 7365  indow_shift = se
-0000e840: 6c66 2e6c 6f6f 705f 7261 6e67 655b 695d  lf.loop_range[i]
-0000e850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e860: 2073 656c 662e 6361 6c63 5f64 7269 6674   self.calc_drift
-0000e870: 736c 6f70 655f 6e6f 6973 6528 736c 6f70  slope_noise(slop
-0000e880: 655f 6772 6964 2c20 6e6f 6973 655f 6772  e_grid, noise_gr
-0000e890: 6964 2c20 6e5f 6a6f 696e 745f 7361 6d70  id, n_joint_samp
-0000e8a0: 6c65 732c 206e 6275 726e 2c0a 2020 2020  les, nburn,.    
+0000e4f0: 2020 2020 2020 2020 696e 2070 6172 616c          in paral
+0000e500: 6c65 6c20 616e 6420 6a6f 696e 6564 2074  lel and joined t
+0000e510: 6f67 6574 6865 7220 696e 2074 6865 2065  ogether in the e
+0000e520: 6e64 206f 6620 7468 6520 6361 6c63 756c  nd of the calcul
+0000e530: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
+0000e540: 3a74 7970 6520 6e75 6d5f 6368 6f70 5f63  :type num_chop_c
+0000e550: 6861 696e 733a 2069 6e74 0a0a 2020 2020  hains: int..    
+0000e560: 2020 2020 2727 270a 0a20 2020 2020 2020      '''..       
+0000e570: 2063 7265 645f 7065 7263 656e 7469 6c65   cred_percentile
+0000e580: 7320 3d20 6e70 2e61 7272 6179 2863 7265  s = np.array(cre
+0000e590: 645f 7065 7263 656e 7469 6c65 7329 0a20  d_percentiles). 
+0000e5a0: 2020 2020 2020 2073 656c 662e 7769 6e64         self.wind
+0000e5b0: 6f77 5f73 697a 6520 3d20 7769 6e64 6f77  ow_size = window
+0000e5c0: 5f73 697a 650a 2020 2020 2020 2020 7365  _size.        se
+0000e5d0: 6c66 2e77 696e 646f 775f 7368 6966 7420  lf.window_shift 
+0000e5e0: 3d20 7769 6e64 6f77 5f73 6869 6674 0a20  = window_shift. 
+0000e5f0: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+0000e600: 5f77 696e 646f 7720 3d20 6e70 2e7a 6572  _window = np.zer
+0000e610: 6f73 2877 696e 646f 775f 7369 7a65 290a  os(window_size).
+0000e620: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+0000e630: 655f 7769 6e64 6f77 203d 206e 702e 7a65  e_window = np.ze
+0000e640: 726f 7328 7769 6e64 6f77 5f73 697a 6529  ros(window_size)
+0000e650: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+0000e660: 6372 656d 656e 7473 203d 206e 702e 7a65  crements = np.ze
+0000e670: 726f 7328 7769 6e64 6f77 5f73 697a 6520  ros(window_size 
+0000e680: 2d20 3129 0a20 2020 2020 2020 2073 656c  - 1).        sel
+0000e690: 662e 6e77 616c 6b65 7273 203d 206e 7761  f.nwalkers = nwa
+0000e6a0: 6c6b 6572 730a 2020 2020 2020 2020 7365  lkers.        se
+0000e6b0: 6c66 2e6e 7374 6570 7320 3d20 6e73 7465  lf.nsteps = nste
+0000e6c0: 7073 0a20 2020 2020 2020 2073 656c 662e  ps.        self.
+0000e6d0: 6e62 7572 6e20 3d20 6e62 7572 6e0a 2020  nburn = nburn.  
+0000e6e0: 2020 2020 2020 7365 6c66 2e6c 6f6f 705f        self.loop_
+0000e6f0: 7261 6e67 6520 3d20 6e70 2e61 7261 6e67  range = np.arang
+0000e700: 6528 302c 2073 656c 662e 6461 7461 5f73  e(0, self.data_s
+0000e710: 697a 6520 2d20 7365 6c66 2e77 696e 646f  ize - self.windo
+0000e720: 775f 7369 7a65 2c20 7365 6c66 2e77 696e  w_size, self.win
+0000e730: 646f 775f 7368 6966 7429 0a20 2020 2020  dow_shift).     
+0000e740: 2020 2073 656c 662e 736c 6f70 655f 7374     self.slope_st
+0000e750: 6f72 6167 6520 3d20 6e70 2e7a 6572 6f73  orage = np.zeros
+0000e760: 2828 352c 2073 656c 662e 6c6f 6f70 5f72  ((5, self.loop_r
+0000e770: 616e 6765 2e73 697a 6529 290a 2020 2020  ange.size)).    
+0000e780: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6c      self.noise_l
+0000e790: 6576 656c 5f73 746f 7261 6765 203d 206e  evel_storage = n
+0000e7a0: 702e 7a65 726f 7328 2835 2c20 7365 6c66  p.zeros((5, self
+0000e7b0: 2e6c 6f6f 705f 7261 6e67 652e 7369 7a65  .loop_range.size
+0000e7c0: 2929 0a20 2020 2020 2020 2069 6620 6372  )).        if cr
+0000e7d0: 6561 7465 5f61 6e69 6d61 7469 6f6e 203d  eate_animation =
+0000e7e0: 3d20 4661 6c73 653a 0a20 2020 2020 2020  = False:.       
+0000e7f0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000e800: 6e67 6528 7365 6c66 2e6c 6f6f 705f 7261  nge(self.loop_ra
+0000e810: 6e67 652e 7369 7a65 293a 0a20 2020 2020  nge.size):.     
+0000e820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e830: 7769 6e64 6f77 5f73 6869 6674 203d 2073  window_shift = s
+0000e840: 656c 662e 6c6f 6f70 5f72 616e 6765 5b69  elf.loop_range[i
+0000e850: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000e860: 2020 7365 6c66 2e63 616c 635f 6472 6966    self.calc_drif
+0000e870: 7473 6c6f 7065 5f6e 6f69 7365 2873 6c6f  tslope_noise(slo
+0000e880: 7065 5f67 7269 642c 206e 6f69 7365 5f67  pe_grid, noise_g
+0000e890: 7269 642c 206e 6275 726e 2c20 6e5f 6a6f  rid, nburn, n_jo
+0000e8a0: 696e 745f 7361 6d70 6c65 732c 0a20 2020  int_samples,.   
 0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8d0: 2020 2020 2020 206e 5f73 6c6f 7065 5f73         n_slope_s
-0000e8e0: 616d 706c 6573 2c20 6e5f 6e6f 6973 655f  amples, n_noise_
-0000e8f0: 7361 6d70 6c65 732c 2063 7265 645f 7065  samples, cred_pe
-0000e900: 7263 656e 7469 6c65 732c 2070 7269 6e74  rcentiles, print
-0000e910: 5f41 435f 7461 752c 0a20 2020 2020 2020  _AC_tau,.       
+0000e8d0: 2020 2020 2020 2020 6e5f 736c 6f70 655f          n_slope_
+0000e8e0: 7361 6d70 6c65 732c 206e 5f6e 6f69 7365  samples, n_noise
+0000e8f0: 5f73 616d 706c 6573 2c20 6372 6564 5f70  _samples, cred_p
+0000e900: 6572 6365 6e74 696c 6573 2c20 7072 696e  ercentiles, prin
+0000e910: 745f 4143 5f74 6175 2c0a 2020 2020 2020  t_AC_tau,.      
 0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e940: 2020 2020 6967 6e6f 7265 5f41 435f 6572      ignore_AC_er
-0000e950: 726f 722c 2074 6869 6e6e 696e 675f 6279  ror, thinning_by
-0000e960: 2c20 7072 696e 745f 7072 6f67 7265 7373  , print_progress
-0000e970: 2c20 6465 7472 656e 6469 6e67 5f70 6572  , detrending_per
-0000e980: 5f77 696e 646f 772c 0a20 2020 2020 2020  _window,.       
+0000e940: 2020 2020 2069 676e 6f72 655f 4143 5f65       ignore_AC_e
+0000e950: 7272 6f72 2c20 7468 696e 6e69 6e67 5f62  rror, thinning_b
+0000e960: 792c 2070 7269 6e74 5f70 726f 6772 6573  y, print_progres
+0000e970: 732c 2064 6574 7265 6e64 696e 675f 7065  s, detrending_pe
+0000e980: 725f 7769 6e64 6f77 2c0a 2020 2020 2020  r_window,.      
 0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 6761 7573 735f 6669 6c74 6572      gauss_filter
-0000e9c0: 5f6d 6f64 652c 6761 7573 735f 6669 6c74  _mode,gauss_filt
-0000e9d0: 6572 5f73 6967 6d61 2c20 6761 7573 735f  er_sigma, gauss_
-0000e9e0: 6669 6c74 6572 5f6f 7264 6572 2c0a 2020  filter_order,.  
+0000e9b0: 2020 2020 2067 6175 7373 5f66 696c 7465       gauss_filte
+0000e9c0: 725f 6d6f 6465 2c67 6175 7373 5f66 696c  r_mode,gauss_fil
+0000e9d0: 7465 725f 7369 676d 612c 2067 6175 7373  ter_sigma, gauss
+0000e9e0: 5f66 696c 7465 725f 6f72 6465 722c 0a20  _filter_order,. 
 0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 2020 2020 2020 2020 2067 6175 7373 5f66           gauss_f
-0000ea20: 696c 7465 725f 6376 616c 2c20 6761 7573  ilter_cval, gaus
-0000ea30: 735f 6669 6c74 6572 5f74 7275 6e63 6174  s_filter_truncat
-0000ea40: 652c 2070 6c6f 745f 6465 7472 656e 6469  e, plot_detrendi
-0000ea50: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+0000ea10: 2020 2020 2020 2020 2020 6761 7573 735f            gauss_
+0000ea20: 6669 6c74 6572 5f63 7661 6c2c 2067 6175  filter_cval, gau
+0000ea30: 7373 5f66 696c 7465 725f 7472 756e 6361  ss_filter_trunca
+0000ea40: 7465 2c20 706c 6f74 5f64 6574 7265 6e64  te, plot_detrend
+0000ea50: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
 0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-0000ea80: 434d 435f 7061 7261 6c6c 656c 697a 6174  CMC_parallelizat
-0000ea90: 696f 6e5f 6d65 7468 6f64 2c20 6e75 6d5f  ion_method, num_
-0000eaa0: 7072 6f63 6573 7365 732c 206e 756d 5f63  processes, num_c
-0000eab0: 686f 705f 6368 6169 6e73 290a 2020 2020  hop_chains).    
-0000eac0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ead0: 2e73 6c6f 7065 5f73 746f 7261 6765 5b3a  .slope_storage[:
-0000eae0: 2c20 695d 203d 2073 656c 662e 6472 6966  , i] = self.drif
-0000eaf0: 745f 736c 6f70 650a 2020 2020 2020 2020  t_slope.        
-0000eb00: 2020 2020 2020 2020 7365 6c66 2e6e 6f69          self.noi
-0000eb10: 7365 5f6c 6576 656c 5f73 746f 7261 6765  se_level_storage
-0000eb20: 5b3a 2c20 695d 203d 2073 656c 662e 6e6f  [:, i] = self.no
-0000eb30: 6973 655f 6c65 7665 6c5f 6573 7469 6d61  ise_level_estima
-0000eb40: 7465 0a20 2020 2020 2020 2065 6c69 6620  te.        elif 
-0000eb50: 6372 6561 7465 5f61 6e69 6d61 7469 6f6e  create_animation
-0000eb60: 203d 3d20 5472 7565 3a0a 2020 2020 2020   == True:.      
-0000eb70: 2020 2020 2020 676c 6f62 616c 2066 6967        global fig
-0000eb80: 2c20 6178 732c 2073 6c5f 6772 5f61 6e69  , axs, sl_gr_ani
-0000eb90: 6d61 7469 6f6e 2c20 6e6f 6973 655f 6772  mation, noise_gr
-0000eba0: 5f61 6e69 6d61 7469 6f6e 2c20 616e 696d  _animation, anim
-0000ebb0: 6174 696f 6e5f 636f 756e 742c 2061 6e69  ation_count, ani
-0000ebc0: 6d61 7469 6f6e 5f74 696d 652c 2061 6e69  mation_time, ani
-0000ebd0: 6d61 7469 6f6e 5f64 6174 612c 206e 6f69  mation_data, noi
-0000ebe0: 5f6c 652c 2063 7269 745f 706f 692c 2076  _le, crit_poi, v
-0000ebf0: 7370 616e 5f77 696e 646f 772c 206e 6f69  span_window, noi
-0000ec00: 7365 5f70 6466 5f6c 696e 652c 2064 7269  se_pdf_line, dri
-0000ec10: 6674 5f73 6c6f 7065 5f6c 696e 652c 206e  ft_slope_line, n
-0000ec20: 6f69 7365 5f6c 696e 652c 2043 425f 736c  oise_line, CB_sl
-0000ec30: 6f70 655f 492c 2043 425f 736c 6f70 655f  ope_I, CB_slope_
-0000ec40: 4949 2c20 4342 5f6e 6f69 7365 5f49 2c20  II, CB_noise_I, 
-0000ec50: 4342 5f6e 6f69 7365 5f49 490a 2020 2020  CB_noise_II.    
-0000ec60: 2020 2020 2020 2020 616e 696d 6174 696f          animatio
-0000ec70: 6e5f 7469 6d65 203d 2073 656c 662e 7469  n_time = self.ti
-0000ec80: 6d65 0a20 2020 2020 2020 2020 2020 2061  me.            a
-0000ec90: 6e69 6d61 7469 6f6e 5f64 6174 6120 3d20  nimation_data = 
-0000eca0: 7365 6c66 2e64 6174 610a 2020 2020 2020  self.data.      
-0000ecb0: 2020 2020 2020 6e6f 695f 6c65 203d 206d        noi_le = m
-0000ecc0: 6172 6b5f 6e6f 6973 655f 6c65 7665 6c0a  ark_noise_level.
-0000ecd0: 2020 2020 2020 2020 2020 2020 6372 6974              crit
-0000ece0: 5f70 6f69 203d 206d 6172 6b5f 6372 6974  _poi = mark_crit
-0000ecf0: 6963 616c 5f70 6f69 6e74 0a20 2020 2020  ical_point.     
-0000ed00: 2020 2020 2020 2073 6c5f 6772 5f61 6e69         sl_gr_ani
-0000ed10: 6d61 7469 6f6e 203d 2073 6c6f 7065 5f67  mation = slope_g
-0000ed20: 7269 640a 2020 2020 2020 2020 2020 2020  rid.            
-0000ed30: 6e6f 6973 655f 6772 5f61 6e69 6d61 7469  noise_gr_animati
-0000ed40: 6f6e 203d 206e 6f69 7365 5f67 7269 640a  on = noise_grid.
-0000ed50: 2020 2020 2020 2020 2020 2020 616e 696d              anim
-0000ed60: 6174 696f 6e5f 636f 756e 7420 3d20 300a  ation_count = 0.
-0000ed70: 2020 2020 2020 2020 2020 2020 6669 672c              fig,
-0000ed80: 2061 7873 203d 2070 6c74 2e73 7562 706c   axs = plt.subpl
-0000ed90: 6f74 7328 322c 2032 2c20 6669 6773 697a  ots(2, 2, figsiz
-0000eda0: 653d 2831 392c 2038 2929 0a20 2020 2020  e=(19, 8)).     
-0000edb0: 2020 2020 2020 2070 6c74 2e73 7570 7469         plt.supti
-0000edc0: 746c 6528 616e 696d 6174 696f 6e5f 7469  tle(animation_ti
-0000edd0: 746c 652c 2066 6f6e 7473 697a 653d 3135  tle, fontsize=15
-0000ede0: 290a 2020 2020 2020 2020 2020 2020 7673  ).            vs
-0000edf0: 7061 6e5f 7769 6e64 6f77 203d 2061 7873  pan_window = axs
-0000ee00: 5b30 2c20 305d 2e61 7876 7370 616e 2830  [0, 0].axvspan(0
-0000ee10: 2c20 302c 2061 6c70 6861 3d30 2e37 2c20  , 0, alpha=0.7, 
-0000ee20: 636f 6c6f 723d 2767 2729 0a20 2020 2020  color='g').     
-0000ee30: 2020 2020 2020 206e 6f69 7365 5f70 6466         noise_pdf
-0000ee40: 5f6c 696e 652c 203d 2061 7873 5b30 2c20  _line, = axs[0, 
-0000ee50: 315d 2e70 6c6f 7428 5b5d 2c20 5b5d 2c20  1].plot([], [], 
-0000ee60: 6c69 6e65 7769 6474 683d 322c 2063 6f6c  linewidth=2, col
-0000ee70: 6f72 3d27 7227 290a 2020 2020 2020 2020  or='r').        
-0000ee80: 2020 2020 6472 6966 745f 736c 6f70 655f      drift_slope_
-0000ee90: 6c69 6e65 2c20 3d20 6178 735b 312c 2030  line, = axs[1, 0
-0000eea0: 5d2e 706c 6f74 285b 5d2c 205b 5d2c 206c  ].plot([], [], l
-0000eeb0: 696e 6577 6964 7468 3d32 2c20 636f 6c6f  inewidth=2, colo
-0000eec0: 723d 2762 2729 0a20 2020 2020 2020 2020  r='b').         
-0000eed0: 2020 206e 6f69 7365 5f6c 696e 652c 203d     noise_line, =
-0000eee0: 2061 7873 5b31 2c20 315d 2e70 6c6f 7428   axs[1, 1].plot(
-0000eef0: 5b5d 2c20 5b5d 2c20 6c69 6e65 7769 6474  [], [], linewidt
-0000ef00: 683d 322c 2063 6f6c 6f72 3d27 6227 290a  h=2, color='b').
-0000ef10: 2020 2020 2020 2020 2020 2020 4342 5f73              CB_s
-0000ef20: 6c6f 7065 5f49 203d 2061 7873 5b31 2c20  lope_I = axs[1, 
-0000ef30: 305d 2e66 696c 6c5f 6265 7477 6565 6e28  0].fill_between(
-0000ef40: 5b5d 2c20 5b5d 2c20 5b5d 2c20 616c 7068  [], [], [], alph
-0000ef50: 613d 302e 372c 2063 6f6c 6f72 3d27 6f72  a=0.7, color='or
-0000ef60: 616e 6765 2729 0a20 2020 2020 2020 2020  ange').         
-0000ef70: 2020 2043 425f 736c 6f70 655f 4949 203d     CB_slope_II =
-0000ef80: 2061 7873 5b31 2c20 305d 2e66 696c 6c5f   axs[1, 0].fill_
-0000ef90: 6265 7477 6565 6e28 5b5d 2c20 5b5d 2c20  between([], [], 
-0000efa0: 5b5d 2c20 616c 7068 613d 302e 342c 2063  [], alpha=0.4, c
-0000efb0: 6f6c 6f72 3d27 6f72 616e 6765 2729 0a20  olor='orange'). 
-0000efc0: 2020 2020 2020 2020 2020 2043 425f 6e6f             CB_no
-0000efd0: 6973 655f 4920 3d20 6178 735b 312c 2031  ise_I = axs[1, 1
-0000efe0: 5d2e 6669 6c6c 5f62 6574 7765 656e 285b  ].fill_between([
-0000eff0: 5d2c 205b 5d2c 205b 5d2c 2061 6c70 6861  ], [], [], alpha
-0000f000: 3d30 2e37 2c20 636f 6c6f 723d 276f 7261  =0.7, color='ora
-0000f010: 6e67 6527 290a 2020 2020 2020 2020 2020  nge').          
-0000f020: 2020 4342 5f6e 6f69 7365 5f49 4920 3d20    CB_noise_II = 
-0000f030: 6178 735b 312c 2031 5d2e 6669 6c6c 5f62  axs[1, 1].fill_b
-0000f040: 6574 7765 656e 285b 5d2c 205b 5d2c 205b  etween([], [], [
-0000f050: 5d2c 2061 6c70 6861 3d30 2e34 2c20 636f  ], alpha=0.4, co
-0000f060: 6c6f 723d 276f 7261 6e67 6527 290a 2020  lor='orange').  
-0000f070: 2020 2020 2020 2020 2020 5772 6974 6572            Writer
-0000f080: 203d 206d 6174 706c 6f74 6c69 622e 616e   = matplotlib.an
-0000f090: 696d 6174 696f 6e2e 7772 6974 6572 735b  imation.writers[
-0000f0a0: 2766 666d 7065 6727 5d0a 2020 2020 2020  'ffmpeg'].      
-0000f0b0: 2020 2020 2020 7772 6974 6572 203d 2057        writer = W
-0000f0c0: 7269 7465 7228 6670 733d 3630 2c20 6d65  riter(fps=60, me
-0000f0d0: 7461 6461 7461 3d64 6963 7428 6172 7469  tadata=dict(arti
-0000f0e0: 7374 3d27 4d65 2729 2c20 6269 7472 6174  st='Me'), bitrat
-0000f0f0: 653d 3138 3030 290a 2020 2020 2020 2020  e=1800).        
-0000f100: 2020 2020 616e 6920 3d20 4675 6e63 416e      ani = FuncAn
-0000f110: 696d 6174 696f 6e28 6669 672c 2073 656c  imation(fig, sel
-0000f120: 662e 616e 696d 6174 696f 6e2c 2066 7261  f.animation, fra
-0000f130: 6d65 733d 7365 6c66 2e6c 6f6f 705f 7261  mes=self.loop_ra
-0000f140: 6e67 652c 2069 6e69 745f 6675 6e63 3d73  nge, init_func=s
-0000f150: 656c 662e 696e 6974 2c20 626c 6974 3d54  elf.init, blit=T
-0000f160: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea80: 4d43 4d43 5f70 6172 616c 6c65 6c69 7a61  MCMC_paralleliza
+0000ea90: 7469 6f6e 5f6d 6574 686f 642c 206e 756d  tion_method, num
+0000eaa0: 5f70 726f 6365 7373 6573 2c20 6e75 6d5f  _processes, num_
+0000eab0: 6368 6f70 5f63 6861 696e 7329 0a20 2020  chop_chains).   
+0000eac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ead0: 662e 736c 6f70 655f 7374 6f72 6167 655b  f.slope_storage[
+0000eae0: 3a2c 2069 5d20 3d20 7365 6c66 2e64 7269  :, i] = self.dri
+0000eaf0: 6674 5f73 6c6f 7065 0a20 2020 2020 2020  ft_slope.       
+0000eb00: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+0000eb10: 6973 655f 6c65 7665 6c5f 7374 6f72 6167  ise_level_storag
+0000eb20: 655b 3a2c 2069 5d20 3d20 7365 6c66 2e6e  e[:, i] = self.n
+0000eb30: 6f69 7365 5f6c 6576 656c 5f65 7374 696d  oise_level_estim
+0000eb40: 6174 650a 2020 2020 2020 2020 656c 6966  ate.        elif
+0000eb50: 2063 7265 6174 655f 616e 696d 6174 696f   create_animatio
+0000eb60: 6e20 3d3d 2054 7275 653a 0a20 2020 2020  n == True:.     
+0000eb70: 2020 2020 2020 2067 6c6f 6261 6c20 6669         global fi
+0000eb80: 672c 2061 7873 2c20 736c 5f67 725f 616e  g, axs, sl_gr_an
+0000eb90: 696d 6174 696f 6e2c 206e 6f69 7365 5f67  imation, noise_g
+0000eba0: 725f 616e 696d 6174 696f 6e2c 2061 6e69  r_animation, ani
+0000ebb0: 6d61 7469 6f6e 5f63 6f75 6e74 2c20 616e  mation_count, an
+0000ebc0: 696d 6174 696f 6e5f 7469 6d65 2c20 616e  imation_time, an
+0000ebd0: 696d 6174 696f 6e5f 6461 7461 2c20 6e6f  imation_data, no
+0000ebe0: 695f 6c65 2c20 6372 6974 5f70 6f69 2c20  i_le, crit_poi, 
+0000ebf0: 7673 7061 6e5f 7769 6e64 6f77 2c20 6e6f  vspan_window, no
+0000ec00: 6973 655f 7064 665f 6c69 6e65 2c20 6472  ise_pdf_line, dr
+0000ec10: 6966 745f 736c 6f70 655f 6c69 6e65 2c20  ift_slope_line, 
+0000ec20: 6e6f 6973 655f 6c69 6e65 2c20 4342 5f73  noise_line, CB_s
+0000ec30: 6c6f 7065 5f49 2c20 4342 5f73 6c6f 7065  lope_I, CB_slope
+0000ec40: 5f49 492c 2043 425f 6e6f 6973 655f 492c  _II, CB_noise_I,
+0000ec50: 2043 425f 6e6f 6973 655f 4949 0a20 2020   CB_noise_II.   
+0000ec60: 2020 2020 2020 2020 2061 6e69 6d61 7469           animati
+0000ec70: 6f6e 5f74 696d 6520 3d20 7365 6c66 2e74  on_time = self.t
+0000ec80: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
+0000ec90: 616e 696d 6174 696f 6e5f 6461 7461 203d  animation_data =
+0000eca0: 2073 656c 662e 6461 7461 0a20 2020 2020   self.data.     
+0000ecb0: 2020 2020 2020 206e 6f69 5f6c 6520 3d20         noi_le = 
+0000ecc0: 6d61 726b 5f6e 6f69 7365 5f6c 6576 656c  mark_noise_level
+0000ecd0: 0a20 2020 2020 2020 2020 2020 2063 7269  .            cri
+0000ece0: 745f 706f 6920 3d20 6d61 726b 5f63 7269  t_poi = mark_cri
+0000ecf0: 7469 6361 6c5f 706f 696e 740a 2020 2020  tical_point.    
+0000ed00: 2020 2020 2020 2020 736c 5f67 725f 616e          sl_gr_an
+0000ed10: 696d 6174 696f 6e20 3d20 736c 6f70 655f  imation = slope_
+0000ed20: 6772 6964 0a20 2020 2020 2020 2020 2020  grid.           
+0000ed30: 206e 6f69 7365 5f67 725f 616e 696d 6174   noise_gr_animat
+0000ed40: 696f 6e20 3d20 6e6f 6973 655f 6772 6964  ion = noise_grid
+0000ed50: 0a20 2020 2020 2020 2020 2020 2061 6e69  .            ani
+0000ed60: 6d61 7469 6f6e 5f63 6f75 6e74 203d 2030  mation_count = 0
+0000ed70: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+0000ed80: 2c20 6178 7320 3d20 706c 742e 7375 6270  , axs = plt.subp
+0000ed90: 6c6f 7473 2832 2c20 322c 2066 6967 7369  lots(2, 2, figsi
+0000eda0: 7a65 3d28 3139 2c20 3829 290a 2020 2020  ze=(19, 8)).    
+0000edb0: 2020 2020 2020 2020 706c 742e 7375 7074          plt.supt
+0000edc0: 6974 6c65 2861 6e69 6d61 7469 6f6e 5f74  itle(animation_t
+0000edd0: 6974 6c65 2c20 666f 6e74 7369 7a65 3d31  itle, fontsize=1
+0000ede0: 3529 0a20 2020 2020 2020 2020 2020 2076  5).            v
+0000edf0: 7370 616e 5f77 696e 646f 7720 3d20 6178  span_window = ax
+0000ee00: 735b 302c 2030 5d2e 6178 7673 7061 6e28  s[0, 0].axvspan(
+0000ee10: 302c 2030 2c20 616c 7068 613d 302e 372c  0, 0, alpha=0.7,
+0000ee20: 2063 6f6c 6f72 3d27 6727 290a 2020 2020   color='g').    
+0000ee30: 2020 2020 2020 2020 6e6f 6973 655f 7064          noise_pd
+0000ee40: 665f 6c69 6e65 2c20 3d20 6178 735b 302c  f_line, = axs[0,
+0000ee50: 2031 5d2e 706c 6f74 285b 5d2c 205b 5d2c   1].plot([], [],
+0000ee60: 206c 696e 6577 6964 7468 3d32 2c20 636f   linewidth=2, co
+0000ee70: 6c6f 723d 2772 2729 0a20 2020 2020 2020  lor='r').       
+0000ee80: 2020 2020 2064 7269 6674 5f73 6c6f 7065       drift_slope
+0000ee90: 5f6c 696e 652c 203d 2061 7873 5b31 2c20  _line, = axs[1, 
+0000eea0: 305d 2e70 6c6f 7428 5b5d 2c20 5b5d 2c20  0].plot([], [], 
+0000eeb0: 6c69 6e65 7769 6474 683d 322c 2063 6f6c  linewidth=2, col
+0000eec0: 6f72 3d27 6227 290a 2020 2020 2020 2020  or='b').        
+0000eed0: 2020 2020 6e6f 6973 655f 6c69 6e65 2c20      noise_line, 
+0000eee0: 3d20 6178 735b 312c 2031 5d2e 706c 6f74  = axs[1, 1].plot
+0000eef0: 285b 5d2c 205b 5d2c 206c 696e 6577 6964  ([], [], linewid
+0000ef00: 7468 3d32 2c20 636f 6c6f 723d 2762 2729  th=2, color='b')
+0000ef10: 0a20 2020 2020 2020 2020 2020 2043 425f  .            CB_
+0000ef20: 736c 6f70 655f 4920 3d20 6178 735b 312c  slope_I = axs[1,
+0000ef30: 2030 5d2e 6669 6c6c 5f62 6574 7765 656e   0].fill_between
+0000ef40: 285b 5d2c 205b 5d2c 205b 5d2c 2061 6c70  ([], [], [], alp
+0000ef50: 6861 3d30 2e37 2c20 636f 6c6f 723d 276f  ha=0.7, color='o
+0000ef60: 7261 6e67 6527 290a 2020 2020 2020 2020  range').        
+0000ef70: 2020 2020 4342 5f73 6c6f 7065 5f49 4920      CB_slope_II 
+0000ef80: 3d20 6178 735b 312c 2030 5d2e 6669 6c6c  = axs[1, 0].fill
+0000ef90: 5f62 6574 7765 656e 285b 5d2c 205b 5d2c  _between([], [],
+0000efa0: 205b 5d2c 2061 6c70 6861 3d30 2e34 2c20   [], alpha=0.4, 
+0000efb0: 636f 6c6f 723d 276f 7261 6e67 6527 290a  color='orange').
+0000efc0: 2020 2020 2020 2020 2020 2020 4342 5f6e              CB_n
+0000efd0: 6f69 7365 5f49 203d 2061 7873 5b31 2c20  oise_I = axs[1, 
+0000efe0: 315d 2e66 696c 6c5f 6265 7477 6565 6e28  1].fill_between(
+0000eff0: 5b5d 2c20 5b5d 2c20 5b5d 2c20 616c 7068  [], [], [], alph
+0000f000: 613d 302e 372c 2063 6f6c 6f72 3d27 6f72  a=0.7, color='or
+0000f010: 616e 6765 2729 0a20 2020 2020 2020 2020  ange').         
+0000f020: 2020 2043 425f 6e6f 6973 655f 4949 203d     CB_noise_II =
+0000f030: 2061 7873 5b31 2c20 315d 2e66 696c 6c5f   axs[1, 1].fill_
+0000f040: 6265 7477 6565 6e28 5b5d 2c20 5b5d 2c20  between([], [], 
+0000f050: 5b5d 2c20 616c 7068 613d 302e 342c 2063  [], alpha=0.4, c
+0000f060: 6f6c 6f72 3d27 6f72 616e 6765 2729 0a20  olor='orange'). 
+0000f070: 2020 2020 2020 2020 2020 2057 7269 7465             Write
+0000f080: 7220 3d20 6d61 7470 6c6f 746c 6962 2e61  r = matplotlib.a
+0000f090: 6e69 6d61 7469 6f6e 2e77 7269 7465 7273  nimation.writers
+0000f0a0: 5b27 6666 6d70 6567 275d 0a20 2020 2020  ['ffmpeg'].     
+0000f0b0: 2020 2020 2020 2077 7269 7465 7220 3d20         writer = 
+0000f0c0: 5772 6974 6572 2866 7073 3d36 302c 206d  Writer(fps=60, m
+0000f0d0: 6574 6164 6174 613d 6469 6374 2861 7274  etadata=dict(art
+0000f0e0: 6973 743d 274d 6527 292c 2062 6974 7261  ist='Me'), bitra
+0000f0f0: 7465 3d31 3830 3029 0a20 2020 2020 2020  te=1800).       
+0000f100: 2020 2020 2061 6e69 203d 2046 756e 6341       ani = FuncA
+0000f110: 6e69 6d61 7469 6f6e 2866 6967 2c20 7365  nimation(fig, se
+0000f120: 6c66 2e61 6e69 6d61 7469 6f6e 2c20 6672  lf.animation, fr
+0000f130: 616d 6573 3d73 656c 662e 6c6f 6f70 5f72  ames=self.loop_r
+0000f140: 616e 6765 2c20 696e 6974 5f66 756e 633d  ange, init_func=
+0000f150: 7365 6c66 2e69 6e69 742c 2062 6c69 743d  self.init, blit=
+0000f160: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
 0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2072 6570 6561 743d 4661 6c73       repeat=Fals
-0000f190: 652c 2066 6172 6773 3d5b 736c 6f70 655f  e, fargs=[slope_
-0000f1a0: 6772 6964 2c20 6e6f 6973 655f 6772 6964  grid, noise_grid
-0000f1b0: 2c20 6e77 616c 6b65 7273 2c20 6e73 7465  , nwalkers, nste
-0000f1c0: 7073 2c20 6e62 7572 6e2c 206e 5f6a 6f69  ps, nburn, n_joi
-0000f1d0: 6e74 5f73 616d 706c 6573 2c0a 2020 2020  nt_samples,.    
+0000f180: 2020 2020 2020 7265 7065 6174 3d46 616c        repeat=Fal
+0000f190: 7365 2c20 6661 7267 733d 5b73 6c6f 7065  se, fargs=[slope
+0000f1a0: 5f67 7269 642c 206e 6f69 7365 5f67 7269  _grid, noise_gri
+0000f1b0: 642c 206e 7761 6c6b 6572 732c 206e 7374  d, nwalkers, nst
+0000f1c0: 6570 732c 206e 6275 726e 2c20 6e5f 6a6f  eps, nburn, n_jo
+0000f1d0: 696e 745f 7361 6d70 6c65 732c 0a20 2020  int_samples,.   
 0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f210: 206e 5f73 6c6f 7065 5f73 616d 706c 6573   n_slope_samples
-0000f220: 2c20 6e5f 6e6f 6973 655f 7361 6d70 6c65  , n_noise_sample
-0000f230: 732c 2063 7265 645f 7065 7263 656e 7469  s, cred_percenti
-0000f240: 6c65 732c 2070 7269 6e74 5f41 435f 7461  les, print_AC_ta
-0000f250: 752c 0a20 2020 2020 2020 2020 2020 2020  u,.             
+0000f210: 2020 6e5f 736c 6f70 655f 7361 6d70 6c65    n_slope_sample
+0000f220: 732c 206e 5f6e 6f69 7365 5f73 616d 706c  s, n_noise_sampl
+0000f230: 6573 2c20 6372 6564 5f70 6572 6365 6e74  es, cred_percent
+0000f240: 696c 6573 2c20 7072 696e 745f 4143 5f74  iles, print_AC_t
+0000f250: 6175 2c0a 2020 2020 2020 2020 2020 2020  au,.            
 0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f280: 2020 2020 2020 2020 6967 6e6f 7265 5f41          ignore_A
-0000f290: 435f 6572 726f 722c 2074 6869 6e6e 696e  C_error, thinnin
-0000f2a0: 675f 6279 2c20 7072 696e 745f 7072 6f67  g_by, print_prog
-0000f2b0: 7265 7373 2c64 6574 7265 6e64 696e 675f  ress,detrending_
-0000f2c0: 7065 725f 7769 6e64 6f77 2c0a 2020 2020  per_window,.    
+0000f280: 2020 2020 2020 2020 2069 676e 6f72 655f           ignore_
+0000f290: 4143 5f65 7272 6f72 2c20 7468 696e 6e69  AC_error, thinni
+0000f2a0: 6e67 5f62 792c 2070 7269 6e74 5f70 726f  ng_by, print_pro
+0000f2b0: 6772 6573 732c 6465 7472 656e 6469 6e67  gress,detrending
+0000f2c0: 5f70 6572 5f77 696e 646f 772c 0a20 2020  _per_window,.   
 0000f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f300: 2067 6175 7373 5f66 696c 7465 725f 6d6f   gauss_filter_mo
-0000f310: 6465 2c67 6175 7373 5f66 696c 7465 725f  de,gauss_filter_
-0000f320: 7369 676d 612c 2067 6175 7373 5f66 696c  sigma, gauss_fil
-0000f330: 7465 725f 6f72 6465 722c 0a20 2020 2020  ter_order,.     
+0000f300: 2020 6761 7573 735f 6669 6c74 6572 5f6d    gauss_filter_m
+0000f310: 6f64 652c 6761 7573 735f 6669 6c74 6572  ode,gauss_filter
+0000f320: 5f73 6967 6d61 2c20 6761 7573 735f 6669  _sigma, gauss_fi
+0000f330: 6c74 6572 5f6f 7264 6572 2c0a 2020 2020  lter_order,.    
 0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f370: 6761 7573 735f 6669 6c74 6572 5f63 7661  gauss_filter_cva
-0000f380: 6c2c 2067 6175 7373 5f66 696c 7465 725f  l, gauss_filter_
-0000f390: 7472 756e 6361 7465 2c20 706c 6f74 5f64  truncate, plot_d
-0000f3a0: 6574 7265 6e64 696e 672c 0a20 2020 2020  etrending,.     
+0000f370: 2067 6175 7373 5f66 696c 7465 725f 6376   gauss_filter_cv
+0000f380: 616c 2c20 6761 7573 735f 6669 6c74 6572  al, gauss_filter
+0000f390: 5f74 7275 6e63 6174 652c 2070 6c6f 745f  _truncate, plot_
+0000f3a0: 6465 7472 656e 6469 6e67 2c0a 2020 2020  detrending,.    
 0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3e0: 4d43 4d43 5f70 6172 616c 6c65 6c69 7a61  MCMC_paralleliza
-0000f3f0: 7469 6f6e 5f6d 6574 686f 642c 206e 756d  tion_method, num
-0000f400: 5f70 726f 6365 7373 6573 2c20 6e75 6d5f  _processes, num_
-0000f410: 6368 6f70 5f63 6861 696e 735d 290a 2020  chop_chains]).  
-0000f420: 2020 2020 2020 2020 2020 616e 692e 7361            ani.sa
-0000f430: 7665 2861 6e69 5f73 6176 655f 6e61 6d65  ve(ani_save_name
-0000f440: 202b 2027 2e6d 7034 272c 2077 7269 7465   + '.mp4', write
-0000f450: 723d 7772 6974 6572 2920 2023 202c 2077  r=writer)  # , w
-0000f460: 7269 7465 7220 3d20 7772 6974 6572 0a20  riter = writer. 
-0000f470: 2020 2020 2020 2069 6620 7361 7665 3a0a         if save:.
-0000f480: 2020 2020 2020 2020 2020 2020 6e70 2e73              np.s
-0000f490: 6176 6528 736c 6f70 655f 7361 7665 5f6e  ave(slope_save_n
-0000f4a0: 616d 6520 2b20 272e 6e70 7927 2c20 7365  ame + '.npy', se
-0000f4b0: 6c66 2e73 6c6f 7065 5f73 746f 7261 6765  lf.slope_storage
-0000f4c0: 290a 2020 2020 2020 2020 2020 2020 6e70  ).            np
-0000f4d0: 2e73 6176 6528 6e6f 6973 655f 6c65 7665  .save(noise_leve
-0000f4e0: 6c5f 7361 7665 5f6e 616d 6520 2b20 272e  l_save_name + '.
-0000f4f0: 6e70 7927 2c20 7365 6c66 2e6e 6f69 7365  npy', self.noise
-0000f500: 5f6c 6576 656c 5f73 746f 7261 6765 290a  _level_storage).
-0000f510: 0a20 2020 2064 6566 2070 6572 666f 726d  .    def perform
-0000f520: 5f4d 4150 5f72 6573 696c 6965 6e63 655f  _MAP_resilience_
-0000f530: 7363 616e 2873 656c 662c 2077 696e 646f  scan(self, windo
-0000f540: 775f 7369 7a65 2c20 7769 6e64 6f77 5f73  w_size, window_s
-0000f550: 6869 6674 2c0a 2020 2020 2020 2020 2020  hift,.          
+0000f3e0: 204d 434d 435f 7061 7261 6c6c 656c 697a   MCMC_paralleliz
+0000f3f0: 6174 696f 6e5f 6d65 7468 6f64 2c20 6e75  ation_method, nu
+0000f400: 6d5f 7072 6f63 6573 7365 732c 206e 756d  m_processes, num
+0000f410: 5f63 686f 705f 6368 6169 6e73 5d29 0a20  _chop_chains]). 
+0000f420: 2020 2020 2020 2020 2020 2061 6e69 2e73             ani.s
+0000f430: 6176 6528 616e 695f 7361 7665 5f6e 616d  ave(ani_save_nam
+0000f440: 6520 2b20 272e 6d70 3427 2c20 7772 6974  e + '.mp4', writ
+0000f450: 6572 3d77 7269 7465 7229 2020 2320 2c20  er=writer)  # , 
+0000f460: 7772 6974 6572 203d 2077 7269 7465 720a  writer = writer.
+0000f470: 2020 2020 2020 2020 6966 2073 6176 653a          if save:
+0000f480: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+0000f490: 7361 7665 2873 6c6f 7065 5f73 6176 655f  save(slope_save_
+0000f4a0: 6e61 6d65 202b 2027 2e6e 7079 272c 2073  name + '.npy', s
+0000f4b0: 656c 662e 736c 6f70 655f 7374 6f72 6167  elf.slope_storag
+0000f4c0: 6529 0a20 2020 2020 2020 2020 2020 206e  e).            n
+0000f4d0: 702e 7361 7665 286e 6f69 7365 5f6c 6576  p.save(noise_lev
+0000f4e0: 656c 5f73 6176 655f 6e61 6d65 202b 2027  el_save_name + '
+0000f4f0: 2e6e 7079 272c 2073 656c 662e 6e6f 6973  .npy', self.nois
+0000f500: 655f 6c65 7665 6c5f 7374 6f72 6167 6529  e_level_storage)
+0000f510: 0a0a 2020 2020 6465 6620 7065 7266 6f72  ..    def perfor
+0000f520: 6d5f 4d41 505f 7265 7369 6c69 656e 6365  m_MAP_resilience
+0000f530: 5f73 6361 6e28 7365 6c66 2c20 7769 6e64  _scan(self, wind
+0000f540: 6f77 5f73 697a 652c 2077 696e 646f 775f  ow_size, window_
+0000f550: 7368 6966 742c 0a20 2020 2020 2020 2020  shift,.         
 0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f570: 2020 2020 2020 2020 2020 6372 6564 5f70            cred_p
-0000f580: 6572 6365 6e74 696c 6573 3d6e 702e 6172  ercentiles=np.ar
-0000f590: 7261 7928 5b31 362c 2031 5d29 2c20 6572  ray([16, 1]), er
-0000f5a0: 726f 725f 7072 6f70 6167 6174 696f 6e3d  ror_propagation=
-0000f5b0: 2773 756d 6d61 7279 2073 7461 7469 7374  'summary statist
-0000f5c0: 6963 7327 2c0a 2020 2020 2020 2020 2020  ics',.          
+0000f570: 2020 2020 2020 2020 2020 2063 7265 645f             cred_
+0000f580: 7065 7263 656e 7469 6c65 733d 6e70 2e61  percentiles=np.a
+0000f590: 7272 6179 285b 3136 2c20 315d 292c 2065  rray([16, 1]), e
+0000f5a0: 7272 6f72 5f70 726f 7061 6761 7469 6f6e  rror_propagation
+0000f5b0: 3d27 7375 6d6d 6172 7920 7374 6174 6973  ='summary statis
+0000f5c0: 7469 6373 272c 0a20 2020 2020 2020 2020  tics',.         
 0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2020 2020 2020 2020 2020 7375 6d6d 6172            summar
-0000f5f0: 795f 7769 6e64 6f77 5f73 697a 6520 3d20  y_window_size = 
-0000f600: 3130 2c20 7369 676d 615f 6d75 6c74 6970  10, sigma_multip
-0000f610: 6c65 7320 3d20 6e70 2e61 7272 6179 285b  les = np.array([
-0000f620: 312c 335d 292c 0a20 2020 2020 2020 2020  1,3]),.         
+0000f5e0: 2020 2020 2020 2020 2020 2073 756d 6d61             summa
+0000f5f0: 7279 5f77 696e 646f 775f 7369 7a65 203d  ry_window_size =
+0000f600: 2031 302c 2073 6967 6d61 5f6d 756c 7469   10, sigma_multi
+0000f610: 706c 6573 203d 206e 702e 6172 7261 7928  ples = np.array(
+0000f620: 5b31 2c33 5d29 2c0a 2020 2020 2020 2020  [1,3]),.        
 0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000f650: 5f70 726f 6772 6573 733d 5472 7565 2c20  _progress=True, 
-0000f660: 7072 696e 745f 6465 7461 696c 733d 4661  print_details=Fa
-0000f670: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0000f640: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000f650: 745f 7072 6f67 7265 7373 3d54 7275 652c  t_progress=True,
+0000f660: 2070 7269 6e74 5f64 6574 6169 6c73 3d46   print_details=F
+0000f670: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
 0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2020 2020 2020 2020 2073 6c6f 7065 5f73           slope_s
-0000f6a0: 6176 655f 6e61 6d65 3d27 6465 6661 756c  ave_name='defaul
-0000f6b0: 745f 7361 7665 5f73 6c6f 7065 7327 2c0a  t_save_slopes',.
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2020 2020 2020 2020 2020 736c 6f70 655f            slope_
+0000f6a0: 7361 7665 5f6e 616d 653d 2764 6566 6175  save_name='defau
+0000f6b0: 6c74 5f73 6176 655f 736c 6f70 6573 272c  lt_save_slopes',
+0000f6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 2020 6e6f 6973 655f 6c65 7665 6c5f      noise_level_
-0000f6f0: 7361 7665 5f6e 616d 653d 2764 6566 6175  save_name='defau
-0000f700: 6c74 5f73 6176 655f 6e6f 6973 6527 2c20  lt_save_noise', 
-0000f710: 7361 7665 3d54 7275 652c 0a20 2020 2020  save=True,.     
+0000f6e0: 2020 2020 206e 6f69 7365 5f6c 6576 656c       noise_level
+0000f6f0: 5f73 6176 655f 6e61 6d65 3d27 6465 6661  _save_name='defa
+0000f700: 756c 745f 7361 7665 5f6e 6f69 7365 272c  ult_save_noise',
+0000f710: 2073 6176 653d 5472 7565 2c0a 2020 2020   save=True,.    
 0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f740: 7265 6174 655f 706c 6f74 3d46 616c 7365  reate_plot=False
-0000f750: 2c20 616e 695f 7361 7665 5f6e 616d 653d  , ani_save_name=
-0000f760: 2764 6566 6175 6c74 5f61 6e69 6d61 7469  'default_animati
-0000f770: 6f6e 5f6e 616d 6527 2c0a 2020 2020 2020  on_name',.      
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 6372 6561 7465 5f70 6c6f 743d 4661 6c73  create_plot=Fals
+0000f750: 652c 2061 6e69 5f73 6176 655f 6e61 6d65  e, ani_save_name
+0000f760: 3d27 6465 6661 756c 745f 616e 696d 6174  ='default_animat
+0000f770: 696f 6e5f 6e61 6d65 272c 0a20 2020 2020  ion_name',.     
 0000f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f790: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0000f7a0: 696d 6174 696f 6e5f 7469 746c 653d 2727  imation_title=''
-0000f7b0: 2c20 6d61 726b 5f63 7269 7469 6361 6c5f  , mark_critical_
-0000f7c0: 706f 696e 743d 4e6f 6e65 2c0a 2020 2020  point=None,.    
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f7a0: 6e69 6d61 7469 6f6e 5f74 6974 6c65 3d27  nimation_title='
+0000f7b0: 272c 206d 6172 6b5f 6372 6974 6963 616c  ', mark_critical
+0000f7c0: 5f70 6f69 6e74 3d4e 6f6e 652c 0a20 2020  _point=None,.   
 0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7f0: 6d61 726b 5f6e 6f69 7365 5f6c 6576 656c  mark_noise_level
-0000f800: 3d4e 6f6e 652c 2070 7269 6e74 5f68 696e  =None, print_hin
-0000f810: 7420 3d20 5472 7565 2c20 6661 7374 4d41  t = True, fastMA
-0000f820: 5066 6c61 6720 3d20 4661 6c73 6529 3a0a  Pflag = False):.
-0000f830: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f840: 2020 2020 5065 7266 6f72 6d73 2061 6e20      Performs an 
-0000f850: 6175 746f 6d61 7465 6420 4d41 5020 7769  automated MAP wi
-0000f860: 6e64 6f77 2073 6361 6e20 7769 7468 2064  ndow scan with d
-0000f870: 6566 696e 6564 2060 7769 6e64 6f77 5f73  efined `window_s
-0000f880: 6869 6674 6020 6f76 6572 2074 6865 2077  hift` over the w
-0000f890: 686f 6c65 2074 696d 6520 7365 7269 6573  hole time series
-0000f8a0: 2e20 496e 2065 6163 680a 2020 2020 2020  . In each.      
-0000f8b0: 2020 7769 6e64 6f77 2074 6865 2064 7269    window the dri
-0000f8c0: 6674 2073 6c6f 7065 2061 6e64 206e 6f69  ft slope and noi
-0000f8d0: 7365 206c 6576 656c 2065 7374 696d 6174  se level estimat
-0000f8e0: 6573 2077 6974 6820 636f 7272 6573 706f  es with correspo
-0000f8f0: 6e64 696e 6720 6372 6564 6962 696c 6974  nding credibilit
-0000f900: 7920 6261 6e64 7320 6172 6520 636f 6d70  y bands are comp
-0000f910: 7574 6564 0a20 2020 2020 2020 2061 6e64  uted.        and
-0000f920: 2073 6176 6564 2069 6e20 7468 6520 6073   saved in the `s
-0000f930: 6c6f 7065 5f73 746f 7261 6765 6020 616e  lope_storage` an
-0000f940: 6420 7468 6520 606e 6f69 7365 5f6c 6576  d the `noise_lev
-0000f950: 656c 5f73 746f 7261 6765 602e 2049 7420  el_storage`. It 
-0000f960: 6361 6e20 616c 736f 2062 6520 7573 6564  can also be used
-0000f970: 2074 6f20 6372 6561 7465 2061 6e0a 2020   to create an.  
-0000f980: 2020 2020 2020 706c 6f74 206f 6620 7468        plot of th
-0000f990: 6520 736c 6964 696e 6720 7769 6e64 6f77  e sliding window
-0000f9a0: 2061 7070 726f 6163 6820 706c 6f74 7469   approach plotti
-0000f9b0: 6e67 2074 6865 2074 696d 6520 7365 7269  ng the time seri
-0000f9c0: 6573 2c20 7468 6520 6d6f 7669 6e67 2077  es, the moving w
-0000f9d0: 696e 646f 772c 2061 6e64 2074 6865 0a20  indow, and the. 
-0000f9e0: 2020 2020 2020 2074 696d 6520 6576 6f6c         time evol
-0000f9f0: 7574 696f 6e20 6f66 2074 6865 2064 7269  ution of the dri
-0000fa00: 6674 2073 6c6f 7065 2065 7374 696d 6174  ft slope estimat
-0000fa10: 6573 203a 6d61 7468 3a60 5c68 6174 7b5c  es :math:`\hat{\
-0000fa20: 7a65 7461 7d60 2061 6e64 2074 6865 206e  zeta}` and the n
-0000fa30: 6f69 7365 206c 6576 656c 203a 6d61 7468  oise level :math
-0000fa40: 3a60 5c68 6174 7b5c 7369 676d 617d 602e  :`\hat{\sigma}`.
-0000fa50: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
-0000fa60: 7274 2069 6e64 6963 6573 206f 6620 7468  rt indices of th
-0000fa70: 6520 7368 6966 7465 6420 7769 6e64 6f77  e shifted window
-0000fa80: 7320 6172 6520 616c 736f 2073 6176 6564  s are also saved
-0000fa90: 2069 6e20 6f72 6465 7220 746f 2066 6163   in order to fac
-0000faa0: 696c 6974 6174 6520 6375 7374 6f6d 697a  ilitate customiz
-0000fab0: 6564 2070 6c6f 7473 2e0a 0a20 2020 2020  ed plots...     
-0000fac0: 2020 203a 7061 7261 6d20 7769 6e64 6f77     :param window
-0000fad0: 5f73 697a 653a 2054 696d 6520 7769 6e64  _size: Time wind
-0000fae0: 6f77 2073 697a 652e 0a20 2020 2020 2020  ow size..       
-0000faf0: 203a 7479 7065 2077 696e 646f 775f 7369   :type window_si
-0000fb00: 7a65 3a20 696e 740a 2020 2020 2020 2020  ze: int.        
-0000fb10: 3a70 6172 616d 2077 696e 646f 775f 7368  :param window_sh
-0000fb20: 6966 743a 2054 6865 2072 6f6c 6c69 6e67  ift: The rolling
-0000fb30: 2074 696d 6520 7769 6e64 6f77 2069 7320   time window is 
-0000fb40: 7368 6966 7465 6420 6162 6f75 7420 6077  shifted about `w
-0000fb50: 696e 646f 775f 7368 6966 7460 2064 6174  indow_shift` dat
-0000fb60: 6120 706f 696e 7473 2e0a 2020 2020 2020  a points..      
-0000fb70: 2020 3a74 7970 6520 7769 6e64 6f77 5f73    :type window_s
-0000fb80: 6869 6674 3a20 696e 740a 2020 2020 2020  hift: int.      
-0000fb90: 2020 3a70 6172 616d 2063 7265 645f 7065    :param cred_pe
-0000fba0: 7263 656e 7469 6c65 733a 204f 6e65 206f  rcentiles: One o
-0000fbb0: 7220 7477 6f20 656e 7472 6965 7320 746f  r two entries to
-0000fbc0: 2064 6566 696e 6520 7468 6520 7065 7263   define the perc
-0000fbd0: 656e 7469 6c65 7320 6f66 2074 6865 2063  entiles of the c
-0000fbe0: 616c 6375 6c61 7465 6420 6372 6564 6962  alculated credib
-0000fbf0: 696c 6974 7920 6261 6e64 730a 2020 2020  ility bands.    
+0000f7f0: 206d 6172 6b5f 6e6f 6973 655f 6c65 7665   mark_noise_leve
+0000f800: 6c3d 4e6f 6e65 2c20 7072 696e 745f 6869  l=None, print_hi
+0000f810: 6e74 203d 2054 7275 652c 2066 6173 744d  nt = True, fastM
+0000f820: 4150 666c 6167 203d 2046 616c 7365 293a  APflag = False):
+0000f830: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f840: 2020 2020 2050 6572 666f 726d 7320 616e       Performs an
+0000f850: 2061 7574 6f6d 6174 6564 204d 4150 2077   automated MAP w
+0000f860: 696e 646f 7720 7363 616e 2077 6974 6820  indow scan with 
+0000f870: 6465 6669 6e65 6420 6077 696e 646f 775f  defined `window_
+0000f880: 7368 6966 7460 206f 7665 7220 7468 6520  shift` over the 
+0000f890: 7768 6f6c 6520 7469 6d65 2073 6572 6965  whole time serie
+0000f8a0: 732e 2049 6e20 6561 6368 0a20 2020 2020  s. In each.     
+0000f8b0: 2020 2077 696e 646f 7720 7468 6520 6472     window the dr
+0000f8c0: 6966 7420 736c 6f70 6520 616e 6420 6e6f  ift slope and no
+0000f8d0: 6973 6520 6c65 7665 6c20 6573 7469 6d61  ise level estima
+0000f8e0: 7465 7320 7769 7468 2063 6f72 7265 7370  tes with corresp
+0000f8f0: 6f6e 6469 6e67 2063 7265 6469 6269 6c69  onding credibili
+0000f900: 7479 2062 616e 6473 2061 7265 2063 6f6d  ty bands are com
+0000f910: 7075 7465 640a 2020 2020 2020 2020 616e  puted.        an
+0000f920: 6420 7361 7665 6420 696e 2074 6865 2060  d saved in the `
+0000f930: 736c 6f70 655f 7374 6f72 6167 6560 2061  slope_storage` a
+0000f940: 6e64 2074 6865 2060 6e6f 6973 655f 6c65  nd the `noise_le
+0000f950: 7665 6c5f 7374 6f72 6167 6560 2e20 4974  vel_storage`. It
+0000f960: 2063 616e 2061 6c73 6f20 6265 2075 7365   can also be use
+0000f970: 6420 746f 2063 7265 6174 6520 616e 0a20  d to create an. 
+0000f980: 2020 2020 2020 2070 6c6f 7420 6f66 2074         plot of t
+0000f990: 6865 2073 6c69 6469 6e67 2077 696e 646f  he sliding windo
+0000f9a0: 7720 6170 7072 6f61 6368 2070 6c6f 7474  w approach plott
+0000f9b0: 696e 6720 7468 6520 7469 6d65 2073 6572  ing the time ser
+0000f9c0: 6965 732c 2074 6865 206d 6f76 696e 6720  ies, the moving 
+0000f9d0: 7769 6e64 6f77 2c20 616e 6420 7468 650a  window, and the.
+0000f9e0: 2020 2020 2020 2020 7469 6d65 2065 766f          time evo
+0000f9f0: 6c75 7469 6f6e 206f 6620 7468 6520 6472  lution of the dr
+0000fa00: 6966 7420 736c 6f70 6520 6573 7469 6d61  ift slope estima
+0000fa10: 7465 7320 3a6d 6174 683a 605c 6861 747b  tes :math:`\hat{
+0000fa20: 5c7a 6574 617d 6020 616e 6420 7468 6520  \zeta}` and the 
+0000fa30: 6e6f 6973 6520 6c65 7665 6c20 3a6d 6174  noise level :mat
+0000fa40: 683a 605c 6861 747b 5c73 6967 6d61 7d60  h:`\hat{\sigma}`
+0000fa50: 2e0a 2020 2020 2020 2020 5468 6520 7374  ..        The st
+0000fa60: 6172 7420 696e 6469 6365 7320 6f66 2074  art indices of t
+0000fa70: 6865 2073 6869 6674 6564 2077 696e 646f  he shifted windo
+0000fa80: 7773 2061 7265 2061 6c73 6f20 7361 7665  ws are also save
+0000fa90: 6420 696e 206f 7264 6572 2074 6f20 6661  d in order to fa
+0000faa0: 6369 6c69 7461 7465 2063 7573 746f 6d69  cilitate customi
+0000fab0: 7a65 6420 706c 6f74 732e 0a0a 2020 2020  zed plots...    
+0000fac0: 2020 2020 3a70 6172 616d 2077 696e 646f      :param windo
+0000fad0: 775f 7369 7a65 3a20 5469 6d65 2077 696e  w_size: Time win
+0000fae0: 646f 7720 7369 7a65 2e0a 2020 2020 2020  dow size..      
+0000faf0: 2020 3a74 7970 6520 7769 6e64 6f77 5f73    :type window_s
+0000fb00: 697a 653a 2069 6e74 0a20 2020 2020 2020  ize: int.       
+0000fb10: 203a 7061 7261 6d20 7769 6e64 6f77 5f73   :param window_s
+0000fb20: 6869 6674 3a20 5468 6520 726f 6c6c 696e  hift: The rollin
+0000fb30: 6720 7469 6d65 2077 696e 646f 7720 6973  g time window is
+0000fb40: 2073 6869 6674 6564 2061 626f 7574 2060   shifted about `
+0000fb50: 7769 6e64 6f77 5f73 6869 6674 6020 6461  window_shift` da
+0000fb60: 7461 2070 6f69 6e74 732e 0a20 2020 2020  ta points..     
+0000fb70: 2020 203a 7479 7065 2077 696e 646f 775f     :type window_
+0000fb80: 7368 6966 743a 2069 6e74 0a20 2020 2020  shift: int.     
+0000fb90: 2020 203a 7061 7261 6d20 6372 6564 5f70     :param cred_p
+0000fba0: 6572 6365 6e74 696c 6573 3a20 4f6e 6520  ercentiles: One 
+0000fbb0: 6f72 2074 776f 2065 6e74 7269 6573 2074  or two entries t
+0000fbc0: 6f20 6465 6669 6e65 2074 6865 2070 6572  o define the per
+0000fbd0: 6365 6e74 696c 6573 206f 6620 7468 6520  centiles of the 
+0000fbe0: 6361 6c63 756c 6174 6564 2063 7265 6469  calculated credi
+0000fbf0: 6269 6c69 7479 2062 616e 6473 0a20 2020  bility bands.   
 0000fc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc10: 2020 2020 6f66 2074 6865 2065 7374 696d      of the estim
-0000fc20: 6174 6564 2070 6172 616d 6574 6572 732e  ated parameters.
-0000fc30: 2049 7420 6973 2073 746f 7265 6420 696e   It is stored in
-0000fc40: 2074 6865 2061 7474 7269 6275 7465 2060   the attribute `
-0000fc50: 6372 6564 6962 696c 6974 795f 6261 6e64  credibility_band
-0000fc60: 7360 2e0a 2020 2020 2020 2020 2020 2020  s`..            
-0000fc70: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-0000fc80: 756c 7420 6973 2060 6e75 6d70 792e 6172  ult is `numpy.ar
-0000fc90: 7261 7928 5b31 362c 315d 2960 2e0a 0a20  ray([16,1])`... 
-0000fca0: 2020 2020 2020 203a 7479 7065 2063 7265         :type cre
-0000fcb0: 645f 7065 7263 656e 7469 6c65 733a 204f  d_percentiles: O
-0000fcc0: 6e65 2d64 696d 656e 7369 6f6e 616c 206e  ne-dimensional n
-0000fcd0: 756d 7079 2061 7272 6179 206f 6620 696e  umpy array of in
-0000fce0: 7465 6765 7273 2e0a 2020 2020 2020 2020  tegers..        
-0000fcf0: 3a70 6172 616d 2065 7272 6f72 5f70 726f  :param error_pro
-0000fd00: 7061 6761 7469 6f6e 3a20 4465 6669 6e65  pagation: Define
-0000fd10: 7320 7468 6520 6d65 7468 6f64 2074 6861  s the method tha
-0000fd20: 7420 6973 2075 7365 6420 746f 2063 6f6d  t is used to com
-0000fd30: 7075 7465 2074 6865 2063 6f6e 6669 6465  pute the confide
-0000fd40: 6e63 6520 6261 6e64 732e 2044 6566 6175  nce bands. Defau
-0000fd50: 6c74 2069 730a 2020 2020 2020 2020 2020  lt is.          
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 6060                ``
-0000fd70: 2773 756d 6d61 7279 2073 7461 7469 7374  'summary statist
-0000fd80: 6963 7360 602e 2049 6e20 7468 6174 2063  ics``. In that c
-0000fd90: 6173 6520 6472 6966 7420 736c 6f70 6520  ase drift slope 
-0000fda0: 7361 6d70 6c65 7320 6f66 2073 697a 6520  samples of size 
-0000fdb0: 6060 7375 6d6d 6172 795f 7769 6e64 6f77  ``summary_window
-0000fdc0: 5f73 697a 6560 6020 6172 650a 2020 2020  _size`` are.    
+0000fc10: 2020 2020 206f 6620 7468 6520 6573 7469       of the esti
+0000fc20: 6d61 7465 6420 7061 7261 6d65 7465 7273  mated parameters
+0000fc30: 2e20 4974 2069 7320 7374 6f72 6564 2069  . It is stored i
+0000fc40: 6e20 7468 6520 6174 7472 6962 7574 6520  n the attribute 
+0000fc50: 6063 7265 6469 6269 6c69 7479 5f62 616e  `credibility_ban
+0000fc60: 6473 602e 0a20 2020 2020 2020 2020 2020  ds`..           
+0000fc70: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+0000fc80: 6175 6c74 2069 7320 606e 756d 7079 2e61  ault is `numpy.a
+0000fc90: 7272 6179 285b 3136 2c31 5d29 602e 0a0a  rray([16,1])`...
+0000fca0: 2020 2020 2020 2020 3a74 7970 6520 6372          :type cr
+0000fcb0: 6564 5f70 6572 6365 6e74 696c 6573 3a20  ed_percentiles: 
+0000fcc0: 4f6e 652d 6469 6d65 6e73 696f 6e61 6c20  One-dimensional 
+0000fcd0: 6e75 6d70 7920 6172 7261 7920 6f66 2069  numpy array of i
+0000fce0: 6e74 6567 6572 732e 0a20 2020 2020 2020  ntegers..       
+0000fcf0: 203a 7061 7261 6d20 6572 726f 725f 7072   :param error_pr
+0000fd00: 6f70 6167 6174 696f 6e3a 2044 6566 696e  opagation: Defin
+0000fd10: 6573 2074 6865 206d 6574 686f 6420 7468  es the method th
+0000fd20: 6174 2069 7320 7573 6564 2074 6f20 636f  at is used to co
+0000fd30: 6d70 7574 6520 7468 6520 636f 6e66 6964  mpute the confid
+0000fd40: 656e 6365 2062 616e 6473 2e20 4465 6661  ence bands. Defa
+0000fd50: 756c 7420 6973 0a20 2020 2020 2020 2020  ult is.         
+0000fd60: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+0000fd70: 6027 7375 6d6d 6172 7920 7374 6174 6973  `'summary statis
+0000fd80: 7469 6373 6060 2e20 496e 2074 6861 7420  tics``. In that 
+0000fd90: 6361 7365 2064 7269 6674 2073 6c6f 7065  case drift slope
+0000fda0: 2073 616d 706c 6573 206f 6620 7369 7a65   samples of size
+0000fdb0: 2060 6073 756d 6d61 7279 5f77 696e 646f   ``summary_windo
+0000fdc0: 775f 7369 7a65 6060 2061 7265 0a20 2020  w_size`` are.   
 0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2020 7573 6564 2074 6f20 636f 6d70      used to comp
-0000fdf0: 7574 6520 7468 6520 6472 6966 7420 736c  ute the drift sl
-0000fe00: 6f70 6520 6d65 616e 2061 6e64 2069 7473  ope mean and its
-0000fe10: 2073 7461 6e64 6172 6420 6572 726f 722e   standard error.
-0000fe20: 2054 6865 2070 6172 616d 6574 6572 2060   The parameter `
-0000fe30: 6073 6967 6d61 5f6d 756c 7469 706c 6573  `sigma_multiples
-0000fe40: 6060 0a20 2020 2020 2020 2020 2020 2020  ``.             
-0000fe50: 2020 2020 2020 2020 2020 2064 6566 696e             defin
-0000fe60: 6573 2074 6865 2077 6964 7468 206f 6620  es the width of 
-0000fe70: 7468 6520 7375 6d6d 6172 7920 7374 6174  the summary stat
-0000fe80: 6973 7469 6373 2720 7379 6d6d 6574 7269  istics' symmetri
-0000fe90: 6320 6572 726f 7220 6261 6e64 732e 0a20  c error bands.. 
+0000fde0: 2020 2020 2075 7365 6420 746f 2063 6f6d       used to com
+0000fdf0: 7075 7465 2074 6865 2064 7269 6674 2073  pute the drift s
+0000fe00: 6c6f 7065 206d 6561 6e20 616e 6420 6974  lope mean and it
+0000fe10: 7320 7374 616e 6461 7264 2065 7272 6f72  s standard error
+0000fe20: 2e20 5468 6520 7061 7261 6d65 7465 7220  . The parameter 
+0000fe30: 6060 7369 676d 615f 6d75 6c74 6970 6c65  ``sigma_multiple
+0000fe40: 7360 600a 2020 2020 2020 2020 2020 2020  s``.            
+0000fe50: 2020 2020 2020 2020 2020 2020 6465 6669              defi
+0000fe60: 6e65 7320 7468 6520 7769 6474 6820 6f66  nes the width of
+0000fe70: 2074 6865 2073 756d 6d61 7279 2073 7461   the summary sta
+0000fe80: 7469 7374 6963 7327 2073 796d 6d65 7472  tistics' symmetr
+0000fe90: 6963 2065 7272 6f72 2062 616e 6473 2e0a  ic error bands..
 0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000feb0: 2020 2020 2020 2049 6620 6060 2765 7272         If ``'err
-0000fec0: 6f72 2062 6f75 6e64 2760 6020 6f72 2060  or bound'`` or `
-0000fed0: 6027 756e 636f 7272 656c 6174 6564 2047  `'uncorrelated G
-0000fee0: 6175 7373 6961 6e27 6060 2069 7320 6368  aussian'`` is ch
-0000fef0: 6f73 656e 2c20 7468 6520 6d61 7267 696e  osen, the margin
-0000ff00: 616c 2075 6e63 6572 7461 696e 7469 6573  al uncertainties
-0000ff10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ff20: 2020 2020 2020 2020 2063 6f72 7265 7370           corresp
-0000ff30: 6f6e 6469 6e67 2074 6f20 6060 6372 6564  onding to ``cred
-0000ff40: 5f70 6572 6365 6e74 696c 6573 6060 2061  _percentiles`` a
-0000ff50: 7265 2063 6f6d 7075 7465 6420 656d 706c  re computed empl
-0000ff60: 6f79 696e 6720 5769 6c6b 7327 2074 6865  oying Wilks' the
-0000ff70: 6f72 656d 2e20 5769 7468 2060 6027 6572  orem. With ``'er
-0000ff80: 726f 7220 626f 756e 6427 6060 0a20 2020  ror bound'``.   
+0000feb0: 2020 2020 2020 2020 4966 2060 6027 6572          If ``'er
+0000fec0: 726f 7220 626f 756e 6427 6060 206f 7220  ror bound'`` or 
+0000fed0: 6060 2775 6e63 6f72 7265 6c61 7465 6420  ``'uncorrelated 
+0000fee0: 4761 7573 7369 616e 2760 6020 6973 2063  Gaussian'`` is c
+0000fef0: 686f 7365 6e2c 2074 6865 206d 6172 6769  hosen, the margi
+0000ff00: 6e61 6c20 756e 6365 7274 6169 6e74 6965  nal uncertaintie
+0000ff10: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000ff20: 2020 2020 2020 2020 2020 636f 7272 6573            corres
+0000ff30: 706f 6e64 696e 6720 746f 2060 6063 7265  ponding to ``cre
+0000ff40: 645f 7065 7263 656e 7469 6c65 7360 6020  d_percentiles`` 
+0000ff50: 6172 6520 636f 6d70 7574 6564 2065 6d70  are computed emp
+0000ff60: 6c6f 7969 6e67 2057 696c 6b73 2720 7468  loying Wilks' th
+0000ff70: 656f 7265 6d2e 2057 6974 6820 6060 2765  eorem. With ``'e
+0000ff80: 7272 6f72 2062 6f75 6e64 2760 600a 2020  rror bound'``.  
 0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffa0: 2020 2020 2074 6865 2068 6967 6865 7374       the highest
-0000ffb0: 2075 6e63 6572 7461 696e 7469 6573 2070   uncertainties p
-0000ffc0: 6572 2070 6172 616d 6574 6572 2061 6e64  er parameter and
-0000ffd0: 2060 6063 7265 645f 7065 7263 656e 7469   ``cred_percenti
-0000ffe0: 6c65 7360 6020 6c65 7665 6c20 6973 2069  les`` level is i
-0000fff0: 6e74 6572 7072 6574 6564 2061 7320 6120  nterpreted as a 
-00010000: 7379 6d6d 6574 7269 630a 2020 2020 2020  symmetric.      
+0000ffa0: 2020 2020 2020 7468 6520 6869 6768 6573        the highes
+0000ffb0: 7420 756e 6365 7274 6169 6e74 6965 7320  t uncertainties 
+0000ffc0: 7065 7220 7061 7261 6d65 7465 7220 616e  per parameter an
+0000ffd0: 6420 6060 6372 6564 5f70 6572 6365 6e74  d ``cred_percent
+0000ffe0: 696c 6573 6060 206c 6576 656c 2069 7320  iles`` level is 
+0000fff0: 696e 7465 7270 7265 7465 6420 6173 2061  interpreted as a
+00010000: 2073 796d 6d65 7472 6963 0a20 2020 2020   symmetric.     
 00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010020: 2020 776f 7273 7420 6361 7365 2062 6f75    worst case bou
-00010030: 6e64 206f 6620 7468 6520 6572 726f 722e  nd of the error.
-00010040: 2049 6620 2060 6027 756e 636f 7272 656c   If  ``'uncorrel
-00010050: 6174 6564 2047 6175 7373 6961 6e27 6060  ated Gaussian'``
-00010060: 2069 7320 6368 6f73 656e 2c20 7468 6520   is chosen, the 
-00010070: 756e 6365 7274 6169 6e74 6965 7320 6172  uncertainties ar
-00010080: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00010090: 2020 2020 2020 2020 2020 7472 6561 7465            treate
-000100a0: 6420 636f 7272 6573 706f 6e64 696e 6720  d corresponding 
-000100b0: 746f 2074 6865 2073 6c69 6768 7420 6173  to the slight as
-000100c0: 796d 6d65 7472 6963 2072 6573 756c 7473  ymmetric results
-000100d0: 206f 6620 7468 6520 5769 6c6b 7327 2074   of the Wilks' t
-000100e0: 6865 6f72 656d 2063 6f6e 6669 6465 6e63  heorem confidenc
-000100f0: 6520 696e 7465 7276 616c 732e 0a20 2020  e intervals..   
+00010020: 2020 2077 6f72 7374 2063 6173 6520 626f     worst case bo
+00010030: 756e 6420 6f66 2074 6865 2065 7272 6f72  und of the error
+00010040: 2e20 4966 2020 6060 2775 6e63 6f72 7265  . If  ``'uncorre
+00010050: 6c61 7465 6420 4761 7573 7369 616e 2760  lated Gaussian'`
+00010060: 6020 6973 2063 686f 7365 6e2c 2074 6865  ` is chosen, the
+00010070: 2075 6e63 6572 7461 696e 7469 6573 2061   uncertainties a
+00010080: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+00010090: 2020 2020 2020 2020 2020 2074 7265 6174             treat
+000100a0: 6564 2063 6f72 7265 7370 6f6e 6469 6e67  ed corresponding
+000100b0: 2074 6f20 7468 6520 736c 6967 6874 2061   to the slight a
+000100c0: 7379 6d6d 6574 7269 6320 7265 7375 6c74  symmetric result
+000100d0: 7320 6f66 2074 6865 2057 696c 6b73 2720  s of the Wilks' 
+000100e0: 7468 656f 7265 6d20 636f 6e66 6964 656e  theorem confiden
+000100f0: 6365 2069 6e74 6572 7661 6c73 2e0a 2020  ce intervals..  
 00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2020 2020 2042 6f74 6820 6f70 7469 6f6e       Both option
-00010120: 7320 6769 7665 2074 7275 7374 776f 7274  s give trustwort
-00010130: 6879 2072 6573 756c 7473 2069 6e20 7468  hy results in th
-00010140: 6520 6361 7365 206f 6620 6120 6669 7273  e case of a firs
-00010150: 7420 6f72 6465 7220 706f 6c79 6e6f 6d69  t order polynomi
-00010160: 616c 2064 7269 6674 2e20 496e 2063 6173  al drift. In cas
-00010170: 6520 6f66 2074 6865 0a20 2020 2020 2020  e of the.       
+00010110: 2020 2020 2020 426f 7468 206f 7074 696f        Both optio
+00010120: 6e73 2067 6976 6520 7472 7573 7477 6f72  ns give trustwor
+00010130: 7468 7920 7265 7375 6c74 7320 696e 2074  thy results in t
+00010140: 6865 2063 6173 6520 6f66 2061 2066 6972  he case of a fir
+00010150: 7374 206f 7264 6572 2070 6f6c 796e 6f6d  st order polynom
+00010160: 6961 6c20 6472 6966 742e 2049 6e20 6361  ial drift. In ca
+00010170: 7365 206f 6620 7468 650a 2020 2020 2020  se of the.      
 00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2074 6869 7264 206f 7264 6572 2070 6f6c   third order pol
-000101a0: 796e 6f6d 6961 6c20 6472 6966 7420 7468  ynomial drift th
-000101b0: 6579 2061 7265 2074 6f6f 206f 7074 696d  ey are too optim
-000101c0: 6973 7469 632c 2069 2e65 2e20 6e61 7272  istic, i.e. narr
-000101d0: 6f77 2c20 7369 6e63 6520 7468 6520 6572  ow, since the er
-000101e0: 726f 7220 626f 756e 6473 0a20 2020 2020  ror bounds.     
+00010190: 2020 7468 6972 6420 6f72 6465 7220 706f    third order po
+000101a0: 6c79 6e6f 6d69 616c 2064 7269 6674 2074  lynomial drift t
+000101b0: 6865 7920 6172 6520 746f 6f20 6f70 7469  hey are too opti
+000101c0: 6d69 7374 6963 2c20 692e 652e 206e 6172  mistic, i.e. nar
+000101d0: 726f 772c 2073 696e 6365 2074 6865 2065  row, since the e
+000101e0: 7272 6f72 2062 6f75 6e64 730a 2020 2020  rror bounds.    
 000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010200: 2020 2028 6060 2765 7272 6f72 2062 6f75     (``'error bou
-00010210: 6e64 2760 6029 206f 7220 6572 726f 7273  nd'``) or errors
-00010220: 2028 6060 2775 6e63 6f72 7265 6c61 7465   (``'uncorrelate
-00010230: 6420 4761 7573 7369 616e 2760 6029 2061  d Gaussian'``) a
-00010240: 7265 2070 726f 7061 6761 7465 6420 7769  re propagated wi
-00010250: 7468 6f75 7420 7265 6761 7264 206f 660a  thout regard of.
-00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010270: 2020 2020 2020 2020 636f 7272 656c 6174          correlat
-00010280: 696f 6e73 2069 6e20 7468 6520 6d6f 6465  ions in the mode
-00010290: 6c20 7061 7261 6d65 7465 7273 2e20 5468  l parameters. Th
-000102a0: 6973 2069 7373 7565 206d 6967 6874 2062  is issue might b
-000102b0: 6520 736f 6c76 6162 6c65 2062 7920 696e  e solvable by in
-000102c0: 7472 6f64 7563 696e 6720 616e 2065 7374  troducing an est
-000102d0: 696d 6174 6520 6f66 2074 6865 0a20 2020  imate of the.   
+00010200: 2020 2020 2860 6027 6572 726f 7220 626f      (``'error bo
+00010210: 756e 6427 6060 2920 6f72 2065 7272 6f72  und'``) or error
+00010220: 7320 2860 6027 756e 636f 7272 656c 6174  s (``'uncorrelat
+00010230: 6564 2047 6175 7373 6961 6e27 6060 2920  ed Gaussian'``) 
+00010240: 6172 6520 7072 6f70 6167 6174 6564 2077  are propagated w
+00010250: 6974 686f 7574 2072 6567 6172 6420 6f66  ithout regard of
+00010260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010270: 2020 2020 2020 2020 2063 6f72 7265 6c61           correla
+00010280: 7469 6f6e 7320 696e 2074 6865 206d 6f64  tions in the mod
+00010290: 656c 2070 6172 616d 6574 6572 732e 2054  el parameters. T
+000102a0: 6869 7320 6973 7375 6520 6d69 6768 7420  his issue might 
+000102b0: 6265 2073 6f6c 7661 626c 6520 6279 2069  be solvable by i
+000102c0: 6e74 726f 6475 6369 6e67 2061 6e20 6573  ntroducing an es
+000102d0: 7469 6d61 7465 206f 6620 7468 650a 2020  timate of the.  
 000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 2020 2063 6f76 6172 6961 6e63 6520       covariance 
-00010300: 6d61 7472 6978 2069 6e20 6675 7475 7265  matrix in future
-00010310: 2c20 6275 7420 6973 206e 6f74 2070 6c61  , but is not pla
-00010320: 6e6e 6564 2066 6f72 206e 6f77 2e20 4675  nned for now. Fu
-00010330: 7274 6865 726d 6f72 652c 2074 6865 2060  rthermore, the `
-00010340: 6027 756e 636f 7272 656c 6174 6564 2047  `'uncorrelated G
-00010350: 6175 7373 6961 6e27 6060 0a20 2020 2020  aussian'``.     
+000102f0: 2020 2020 2020 636f 7661 7269 616e 6365        covariance
+00010300: 206d 6174 7269 7820 696e 2066 7574 7572   matrix in futur
+00010310: 652c 2062 7574 2069 7320 6e6f 7420 706c  e, but is not pl
+00010320: 616e 6e65 6420 666f 7220 6e6f 772e 2046  anned for now. F
+00010330: 7572 7468 6572 6d6f 7265 2c20 7468 6520  urthermore, the 
+00010340: 6060 2775 6e63 6f72 7265 6c61 7465 6420  ``'uncorrelated 
+00010350: 4761 7573 7369 616e 2760 600a 2020 2020  Gaussian'``.    
 00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010370: 2020 206f 7074 696f 6e20 6b65 6570 7320     option keeps 
-00010380: 7468 6520 736c 6967 6874 6c79 2061 7379  the slightly asy
-00010390: 6d6d 6574 7269 6320 6572 726f 7273 2070  mmetric errors p
-000103a0: 726f 706f 7365 6420 6279 2057 696c 6b73  roposed by Wilks
-000103b0: 2720 7468 656f 7265 6d20 666f 7220 7468  ' theorem for th
-000103c0: 6520 6d61 7267 696e 616c 2070 6172 616d  e marginal param
-000103d0: 6574 6572 0a20 2020 2020 2020 2020 2020  eter.           
-000103e0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000103f0: 7472 6962 7574 696f 6e73 2e20 5468 6973  tributions. This
-00010400: 2073 6d61 6c6c 2066 6f72 6d61 6c20 696e   small formal in
-00010410: 636f 7272 6563 746e 6573 7320 6973 2074  correctness is t
-00010420: 6f20 6d61 696e 7461 696e 2069 6e66 6f72  o maintain infor
-00010430: 6d61 7469 6f6e 2061 626f 7574 2061 7379  mation about asy
-00010440: 6d6d 6574 7279 2069 6e20 7468 650a 2020  mmetry in the.  
+00010370: 2020 2020 6f70 7469 6f6e 206b 6565 7073      option keeps
+00010380: 2074 6865 2073 6c69 6768 746c 7920 6173   the slightly as
+00010390: 796d 6d65 7472 6963 2065 7272 6f72 7320  ymmetric errors 
+000103a0: 7072 6f70 6f73 6564 2062 7920 5769 6c6b  proposed by Wilk
+000103b0: 7327 2074 6865 6f72 656d 2066 6f72 2074  s' theorem for t
+000103c0: 6865 206d 6172 6769 6e61 6c20 7061 7261  he marginal para
+000103d0: 6d65 7465 720a 2020 2020 2020 2020 2020  meter.          
+000103e0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+000103f0: 7374 7269 6275 7469 6f6e 732e 2054 6869  stributions. Thi
+00010400: 7320 736d 616c 6c20 666f 726d 616c 2069  s small formal i
+00010410: 6e63 6f72 7265 6374 6e65 7373 2069 7320  ncorrectness is 
+00010420: 746f 206d 6169 6e74 6169 6e20 696e 666f  to maintain info
+00010430: 726d 6174 696f 6e20 6162 6f75 7420 6173  rmation about as
+00010440: 796d 6d65 7472 7920 696e 2074 6865 0a20  ymmetry in the. 
 00010450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010460: 2020 2020 2020 6573 7469 6d61 7465 7320        estimates 
-00010470: 696e 2061 2066 6972 7374 2057 696c 6b73  in a first Wilks
-00010480: 2720 7468 656f 7265 6d20 6775 6573 732e  ' theorem guess.
-00010490: 2054 6865 2060 6063 7265 645f 7065 7263   The ``cred_perc
-000104a0: 656e 7469 6c65 7360 6020 6172 6520 6669  entiles`` are fi
-000104b0: 7865 6420 746f 0a20 2020 2020 2020 2020  xed to.         
-000104c0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-000104d0: 6063 7265 645f 7065 7263 656e 7469 6c65  `cred_percentile
-000104e0: 7320 3d20 6e75 6d70 792e 6172 7261 7928  s = numpy.array(
-000104f0: 5b35 2c31 5d29 6060 2074 6f20 7472 616e  [5,1])`` to tran
-00010500: 7366 6f72 6d20 7468 6520 6861 6c66 2063  sform the half c
-00010510: 6f6e 6669 6465 6e63 6520 6261 6e64 7320  onfidence bands 
-00010520: 756e 6465 7220 7468 6520 6173 7375 6d70  under the assump
-00010530: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00010540: 2020 2020 2020 2020 2020 2020 206f 6620               of 
-00010550: 4761 7573 7369 616e 2064 6973 7472 6962  Gaussian distrib
-00010560: 7574 696f 6e73 2062 7920 7468 6520 6661  utions by the fa
-00010570: 6374 6f72 7320 312e 3936 2061 6e64 2032  ctors 1.96 and 2
-00010580: 2e35 3532 352c 2072 6573 7065 6374 6976  .5525, respectiv
+00010460: 2020 2020 2020 2065 7374 696d 6174 6573         estimates
+00010470: 2069 6e20 6120 6669 7273 7420 5769 6c6b   in a first Wilk
+00010480: 7327 2074 6865 6f72 656d 2067 7565 7373  s' theorem guess
+00010490: 2e20 5468 6520 6060 6372 6564 5f70 6572  . The ``cred_per
+000104a0: 6365 6e74 696c 6573 6060 2061 7265 2066  centiles`` are f
+000104b0: 6978 6564 2074 6f0a 2020 2020 2020 2020  ixed to.        
+000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104d0: 6060 6372 6564 5f70 6572 6365 6e74 696c  ``cred_percentil
+000104e0: 6573 203d 206e 756d 7079 2e61 7272 6179  es = numpy.array
+000104f0: 285b 352c 315d 2960 6020 746f 2074 7261  ([5,1])`` to tra
+00010500: 6e73 666f 726d 2074 6865 2068 616c 6620  nsform the half 
+00010510: 636f 6e66 6964 656e 6365 2062 616e 6473  confidence bands
+00010520: 2075 6e64 6572 2074 6865 2061 7373 756d   under the assum
+00010530: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
+00010540: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00010550: 2047 6175 7373 6961 6e20 6469 7374 7269   Gaussian distri
+00010560: 6275 7469 6f6e 7320 6279 2074 6865 2066  butions by the f
+00010570: 6163 746f 7273 2031 2e39 3620 616e 6420  actors 1.96 and 
+00010580: 322e 3537 352c 2072 6573 7065 6374 6976  2.575, respectiv
 00010590: 656c 792e 2054 6865 2070 726f 7061 6761  ely. The propaga
 000105a0: 7465 6420 7265 7375 6c74 2069 730a 2020  ted result is.  
 000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000105c0: 2020 2020 2020 7472 616e 7366 6f72 6d65        transforme
 000105d0: 6420 6261 636b 2e0a 0a20 2020 2020 2020  d back...       
 000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000105f0: 202e 2e20 6869 6e74 3a3a 0a20 2020 2020   .. hint::.     
@@ -4319,1262 +4319,1249 @@
 00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010df0: 2020 2020 6279 206f 6e65 2e0a 2020 2020      by one..    
 00010e00: 2020 2020 3a74 7970 6520 7375 6d6d 6172      :type summar
 00010e10: 795f 7769 6e64 6f77 5f73 697a 653a 2069  y_window_size: i
 00010e20: 6e74 0a20 2020 2020 2020 203a 7061 7261  nt.        :para
 00010e30: 6d20 7369 676d 615f 6d75 6c74 6970 6c65  m sigma_multiple
 00010e40: 733a 2054 6865 2061 7272 6179 2068 6173  s: The array has
-00010e50: 7420 7477 6f20 656e 7472 6965 732e 2049  t two entries. I
-00010e60: 6620 6060 6572 726f 725f 7072 6f70 6167  f ``error_propag
-00010e70: 6174 696f 6e20 3d20 2773 756d 6d61 7279  ation = 'summary
-00010e80: 2073 7461 7469 7374 6963 7327 6060 2069   statistics'`` i
-00010e90: 7320 6368 6f73 656e 2c0a 2020 2020 2020  s chosen,.      
+00010e50: 2074 776f 2065 6e74 7269 6573 2e20 4966   two entries. If
+00010e60: 2060 6065 7272 6f72 5f70 726f 7061 6761   ``error_propaga
+00010e70: 7469 6f6e 203d 2027 7375 6d6d 6172 7920  tion = 'summary 
+00010e80: 7374 6174 6973 7469 6373 2760 6020 6973  statistics'`` is
+00010e90: 2063 686f 7365 6e2c 0a20 2020 2020 2020   chosen,.       
 00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 2020 7468 6520 656e 7472 6965 7320 6465    the entries de
-00010ec0: 6669 6e65 2074 6865 2064 7269 6674 2073  fine the drift s
-00010ed0: 6c6f 7065 2073 7461 6e64 6172 6420 6572  lope standard er
-00010ee0: 726f 7220 6d75 6c74 6970 6c65 7320 7768  ror multiples wh
-00010ef0: 6963 6820 6172 6520 7573 6564 2074 6f20  ich are used to 
-00010f00: 6361 6c63 756c 6174 6520 7468 650a 2020  calculate the.  
+00010eb0: 2074 6865 2065 6e74 7269 6573 2064 6566   the entries def
+00010ec0: 696e 6520 7468 6520 6472 6966 7420 736c  ine the drift sl
+00010ed0: 6f70 6520 7374 616e 6461 7264 2065 7272  ope standard err
+00010ee0: 6f72 206d 756c 7469 706c 6573 2077 6869  or multiples whi
+00010ef0: 6368 2061 7265 2075 7365 6420 746f 2063  ch are used to c
+00010f00: 616c 6375 6c61 7465 2074 6865 0a20 2020  alculate the.   
 00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 2020 2020 2020 756e 6365 7274 6169 6e74        uncertaint
-00010f30: 7920 6261 6e64 732e 0a20 2020 2020 2020  y bands..       
-00010f40: 203a 7479 7065 2073 6967 6d61 5f6d 756c   :type sigma_mul
-00010f50: 7469 706c 6573 3a20 4f6e 6520 6469 6d65  tiples: One dime
-00010f60: 6e73 696f 6e61 6c20 6e75 6d70 7920 6172  nsional numpy ar
-00010f70: 7261 7920 6f66 2066 6c6f 6174 202e 0a20  ray of float .. 
-00010f80: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00010f90: 2020 2020 6966 2065 7272 6f72 5f70 726f      if error_pro
-00010fa0: 7061 6761 7469 6f6e 203d 3d20 2775 6e63  pagation == 'unc
-00010fb0: 6f72 7265 6c61 7465 6420 4761 7573 7369  orrelated Gaussi
-00010fc0: 616e 2720 616e 6420 7365 6c66 2e64 7269  an' and self.dri
-00010fd0: 6674 5f6d 6f64 656c 203d 3d20 2733 7264  ft_model == '3rd
-00010fe0: 206f 7264 6572 2070 6f6c 796e 6f6d 6961   order polynomia
-00010ff0: 6c27 3a0a 2020 2020 2020 2020 2020 2020  l':.            
-00011000: 6372 6564 6962 696c 6974 795f 6261 6e64  credibility_band
-00011010: 7320 3d20 6e70 2e61 7272 6179 285b 352c  s = np.array([5,
-00011020: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-00011030: 6966 2070 7269 6e74 5f68 696e 743a 0a20  if print_hint:. 
-00011040: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011050: 7269 6e74 2827 4849 4e54 3a20 4669 7865  rint('HINT: Fixe
-00011060: 6420 6372 6564 5f70 6572 6365 6e74 696c  d cred_percentil
-00011070: 6573 203d 206e 756d 7079 2e61 7272 6179  es = numpy.array
-00011080: 5b35 2c31 5d29 2066 6f72 2074 6865 2075  [5,1]) for the u
-00011090: 6e63 6f72 7265 6c61 7465 6420 4761 7573  ncorrelated Gaus
-000110a0: 7369 616e 2065 7272 6f72 2070 726f 7061  sian error propa
-000110b0: 6761 7469 6f6e 2027 0a20 2020 2020 2020  gation '.       
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000110d0: 6f66 2074 6865 2064 7269 6674 2073 6c6f  of the drift slo
-000110e0: 7065 2069 7320 7573 6564 2066 6f72 2064  pe is used for d
-000110f0: 7269 6674 5f6d 6f64 656c 203d 3d20 6033  rift_model == `3
-00011100: 7264 5f6f 7264 6572 5f70 6f6c 796e 6f6d  rd_order_polynom
-00011110: 6961 6c60 2e27 290a 2020 2020 2020 2020  ial`.').        
-00011120: 656c 6966 2065 7272 6f72 5f70 726f 7061  elif error_propa
-00011130: 6761 7469 6f6e 203d 3d20 2775 6e63 6f72  gation == 'uncor
-00011140: 7265 6c61 7465 6420 4761 7573 7369 616e  related Gaussian
-00011150: 2720 616e 6420 7365 6c66 2e64 7269 6674  ' and self.drift
-00011160: 5f6d 6f64 656c 203d 3d20 2766 6972 7374  _model == 'first
-00011170: 206f 7264 6572 2070 6f6c 796e 6f6d 6961   order polynomia
-00011180: 6c27 3a0a 2020 2020 2020 2020 2020 2020  l':.            
-00011190: 6372 6564 6962 696c 6974 795f 6261 6e64  credibility_band
-000111a0: 7320 3d20 6372 6564 5f70 6572 6365 6e74  s = cred_percent
-000111b0: 696c 6573 0a20 2020 2020 2020 2065 6c69  iles.        eli
-000111c0: 6620 6572 726f 725f 7072 6f70 6167 6174  f error_propagat
-000111d0: 696f 6e20 3d3d 2027 6572 726f 7220 626f  ion == 'error bo
-000111e0: 756e 6427 3a0a 2020 2020 2020 2020 2020  und':.          
-000111f0: 2020 6372 6564 6962 696c 6974 795f 6261    credibility_ba
-00011200: 6e64 7320 3d20 6372 6564 5f70 6572 6365  nds = cred_perce
-00011210: 6e74 696c 6573 0a20 2020 2020 2020 2065  ntiles.        e
-00011220: 6c69 6620 6e6f 7420 6572 726f 725f 7072  lif not error_pr
-00011230: 6f70 6167 6174 696f 6e20 3d3d 2027 7375  opagation == 'su
-00011240: 6d6d 6172 7920 7374 6174 6973 7469 6373  mmary statistics
-00011250: 273a 0a20 2020 2020 2020 2020 2020 2070  ':.            p
-00011260: 7269 6e74 2827 4552 524f 523a 204e 6f20  rint('ERROR: No 
-00011270: 7375 6974 6162 6c65 2065 7272 6f72 5f70  suitable error_p
-00011280: 726f 7061 6761 7469 6f6e 206f 7074 696f  ropagation optio
-00011290: 6e20 6465 6669 6e65 642e 2729 0a20 2020  n defined.').   
-000112a0: 2020 2020 2073 656c 662e 7769 6e64 6f77       self.window
-000112b0: 5f73 697a 6520 3d20 7769 6e64 6f77 5f73  _size = window_s
-000112c0: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
-000112d0: 2e77 696e 646f 775f 7368 6966 7420 3d20  .window_shift = 
-000112e0: 7769 6e64 6f77 5f73 6869 6674 0a20 2020  window_shift.   
-000112f0: 2020 2020 2073 656c 662e 6461 7461 5f77       self.data_w
-00011300: 696e 646f 7720 3d20 6e70 2e7a 6572 6f73  indow = np.zeros
-00011310: 2877 696e 646f 775f 7369 7a65 290a 2020  (window_size).  
-00011320: 2020 2020 2020 7365 6c66 2e74 696d 655f        self.time_
-00011330: 7769 6e64 6f77 203d 206e 702e 7a65 726f  window = np.zero
-00011340: 7328 7769 6e64 6f77 5f73 697a 6529 0a20  s(window_size). 
-00011350: 2020 2020 2020 2073 656c 662e 6c6f 6f70         self.loop
-00011360: 5f72 616e 6765 203d 206e 702e 6172 616e  _range = np.aran
-00011370: 6765 2830 2c20 7365 6c66 2e64 6174 615f  ge(0, self.data_
-00011380: 7369 7a65 202d 2073 656c 662e 7769 6e64  size - self.wind
-00011390: 6f77 5f73 697a 652c 2073 656c 662e 7769  ow_size, self.wi
-000113a0: 6e64 6f77 5f73 6869 6674 290a 2020 2020  ndow_shift).    
-000113b0: 2020 2020 7365 6c66 2e73 6c6f 7065 5f73      self.slope_s
-000113c0: 746f 7261 6765 203d 206e 702e 7a65 726f  torage = np.zero
-000113d0: 7328 2835 2c20 7365 6c66 2e6c 6f6f 705f  s((5, self.loop_
-000113e0: 7261 6e67 652e 7369 7a65 2929 0a20 2020  range.size)).   
-000113f0: 2020 2020 2073 656c 662e 6e6f 6973 655f       self.noise_
-00011400: 6c65 7665 6c5f 7374 6f72 6167 6520 3d20  level_storage = 
-00011410: 6e70 2e7a 6572 6f73 2828 352c 2073 656c  np.zeros((5, sel
-00011420: 662e 6c6f 6f70 5f72 616e 6765 2e73 697a  f.loop_range.siz
-00011430: 6529 290a 2020 2020 2020 2020 6966 2063  e)).        if c
-00011440: 7265 6174 655f 706c 6f74 203d 3d20 4661  reate_plot == Fa
-00011450: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00011460: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00011470: 7365 6c66 2e6c 6f6f 705f 7261 6e67 652e  self.loop_range.
-00011480: 7369 7a65 293a 0a20 2020 2020 2020 2020  size):.         
-00011490: 2020 2020 2020 2069 6620 7072 696e 745f         if print_
-000114a0: 7072 6f67 7265 7373 3a0a 2020 2020 2020  progress:.      
-000114b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000114c0: 696e 7428 2743 616c 6375 6c61 7465 204d  int('Calculate M
-000114d0: 4150 2072 6573 696c 6965 6e63 6520 666f  AP resilience fo
-000114e0: 7220 7769 6e64 6f77 2027 202b 2073 7472  r window ' + str
-000114f0: 2869 202b 2031 2920 2b20 2720 6f66 2027  (i + 1) + ' of '
-00011500: 202b 2073 7472 2873 656c 662e 6c6f 6f70   + str(self.loop
-00011510: 5f72 616e 6765 2e73 697a 6529 202b 2027  _range.size) + '
-00011520: 2e27 290a 2020 2020 2020 2020 2020 2020  .').            
-00011530: 2020 2020 7365 6c66 2e77 696e 646f 775f      self.window_
-00011540: 7368 6966 7420 3d20 7365 6c66 2e6c 6f6f  shift = self.loo
-00011550: 705f 7261 6e67 655b 695d 0a20 2020 2020  p_range[i].     
-00011560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011570: 5f63 616c 635f 4d41 505f 7265 7369 6c69  _calc_MAP_resili
-00011580: 656e 6365 2863 7265 645f 7065 7263 656e  ence(cred_percen
-00011590: 7469 6c65 732c 2065 7272 6f72 5f70 726f  tiles, error_pro
-000115a0: 7061 6761 7469 6f6e 2c20 7375 6d6d 6172  pagation, summar
-000115b0: 795f 7769 6e64 6f77 5f73 697a 652c 0a20  y_window_size,. 
+00010f20: 2020 2020 2075 6e63 6572 7461 696e 7479       uncertainty
+00010f30: 2062 616e 6473 2e0a 2020 2020 2020 2020   bands..        
+00010f40: 3a74 7970 6520 7369 676d 615f 6d75 6c74  :type sigma_mult
+00010f50: 6970 6c65 733a 204f 6e65 2064 696d 656e  iples: One dimen
+00010f60: 7369 6f6e 616c 206e 756d 7079 2061 7272  sional numpy arr
+00010f70: 6179 206f 6620 666c 6f61 7420 2e0a 2020  ay of float ..  
+00010f80: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00010f90: 2020 2069 6620 6572 726f 725f 7072 6f70     if error_prop
+00010fa0: 6167 6174 696f 6e20 3d3d 2027 756e 636f  agation == 'unco
+00010fb0: 7272 656c 6174 6564 2047 6175 7373 6961  rrelated Gaussia
+00010fc0: 6e27 2061 6e64 2073 656c 662e 6472 6966  n' and self.drif
+00010fd0: 745f 6d6f 6465 6c20 3d3d 2027 3372 6420  t_model == '3rd 
+00010fe0: 6f72 6465 7220 706f 6c79 6e6f 6d69 616c  order polynomial
+00010ff0: 273a 0a20 2020 2020 2020 2020 2020 2063  ':.            c
+00011000: 7265 6469 6269 6c69 7479 5f62 616e 6473  redibility_bands
+00011010: 203d 206e 702e 6172 7261 7928 5b35 2c31   = np.array([5,1
+00011020: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+00011030: 6620 7072 696e 745f 6869 6e74 3a0a 2020  f print_hint:.  
+00011040: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00011050: 696e 7428 2748 494e 543a 2046 6978 6564  int('HINT: Fixed
+00011060: 2063 7265 645f 7065 7263 656e 7469 6c65   cred_percentile
+00011070: 7320 3d20 6e75 6d70 792e 6172 7261 795b  s = numpy.array[
+00011080: 352c 315d 2920 666f 7220 7468 6520 756e  5,1]) for the un
+00011090: 636f 7272 656c 6174 6564 2047 6175 7373  correlated Gauss
+000110a0: 6961 6e20 6572 726f 7220 7072 6f70 6167  ian error propag
+000110b0: 6174 696f 6e20 270a 2020 2020 2020 2020  ation '.        
+000110c0: 2020 2020 2020 2020 2020 2020 2020 276f                'o
+000110d0: 6620 7468 6520 6472 6966 7420 736c 6f70  f the drift slop
+000110e0: 6520 6973 2075 7365 6420 666f 7220 6472  e is used for dr
+000110f0: 6966 745f 6d6f 6465 6c20 3d3d 2060 3372  ift_model == `3r
+00011100: 645f 6f72 6465 725f 706f 6c79 6e6f 6d69  d_order_polynomi
+00011110: 616c 602e 2729 0a20 2020 2020 2020 2065  al`.').        e
+00011120: 6c69 6620 6572 726f 725f 7072 6f70 6167  lif error_propag
+00011130: 6174 696f 6e20 3d3d 2027 756e 636f 7272  ation == 'uncorr
+00011140: 656c 6174 6564 2047 6175 7373 6961 6e27  elated Gaussian'
+00011150: 2061 6e64 2073 656c 662e 6472 6966 745f   and self.drift_
+00011160: 6d6f 6465 6c20 3d3d 2027 6669 7273 7420  model == 'first 
+00011170: 6f72 6465 7220 706f 6c79 6e6f 6d69 616c  order polynomial
+00011180: 273a 0a20 2020 2020 2020 2020 2020 2063  ':.            c
+00011190: 7265 6469 6269 6c69 7479 5f62 616e 6473  redibility_bands
+000111a0: 203d 2063 7265 645f 7065 7263 656e 7469   = cred_percenti
+000111b0: 6c65 730a 2020 2020 2020 2020 656c 6966  les.        elif
+000111c0: 2065 7272 6f72 5f70 726f 7061 6761 7469   error_propagati
+000111d0: 6f6e 203d 3d20 2765 7272 6f72 2062 6f75  on == 'error bou
+000111e0: 6e64 273a 0a20 2020 2020 2020 2020 2020  nd':.           
+000111f0: 2063 7265 6469 6269 6c69 7479 5f62 616e   credibility_ban
+00011200: 6473 203d 2063 7265 645f 7065 7263 656e  ds = cred_percen
+00011210: 7469 6c65 730a 2020 2020 2020 2020 656c  tiles.        el
+00011220: 6966 206e 6f74 2065 7272 6f72 5f70 726f  if not error_pro
+00011230: 7061 6761 7469 6f6e 203d 3d20 2773 756d  pagation == 'sum
+00011240: 6d61 7279 2073 7461 7469 7374 6963 7327  mary statistics'
+00011250: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00011260: 696e 7428 2745 5252 4f52 3a20 4e6f 2073  int('ERROR: No s
+00011270: 7569 7461 626c 6520 6572 726f 725f 7072  uitable error_pr
+00011280: 6f70 6167 6174 696f 6e20 6f70 7469 6f6e  opagation option
+00011290: 2064 6566 696e 6564 2e27 290a 2020 2020   defined.').    
+000112a0: 2020 2020 7365 6c66 2e77 696e 646f 775f      self.window_
+000112b0: 7369 7a65 203d 2077 696e 646f 775f 7369  size = window_si
+000112c0: 7a65 0a20 2020 2020 2020 2073 656c 662e  ze.        self.
+000112d0: 7769 6e64 6f77 5f73 6869 6674 203d 2077  window_shift = w
+000112e0: 696e 646f 775f 7368 6966 740a 2020 2020  indow_shift.    
+000112f0: 2020 2020 7365 6c66 2e64 6174 615f 7769      self.data_wi
+00011300: 6e64 6f77 203d 206e 702e 7a65 726f 7328  ndow = np.zeros(
+00011310: 7769 6e64 6f77 5f73 697a 6529 0a20 2020  window_size).   
+00011320: 2020 2020 2073 656c 662e 7469 6d65 5f77       self.time_w
+00011330: 696e 646f 7720 3d20 6e70 2e7a 6572 6f73  indow = np.zeros
+00011340: 2877 696e 646f 775f 7369 7a65 290a 2020  (window_size).  
+00011350: 2020 2020 2020 7365 6c66 2e6c 6f6f 705f        self.loop_
+00011360: 7261 6e67 6520 3d20 6e70 2e61 7261 6e67  range = np.arang
+00011370: 6528 302c 2073 656c 662e 6461 7461 5f73  e(0, self.data_s
+00011380: 697a 6520 2d20 7365 6c66 2e77 696e 646f  ize - self.windo
+00011390: 775f 7369 7a65 2c20 7365 6c66 2e77 696e  w_size, self.win
+000113a0: 646f 775f 7368 6966 7429 0a20 2020 2020  dow_shift).     
+000113b0: 2020 2073 656c 662e 736c 6f70 655f 7374     self.slope_st
+000113c0: 6f72 6167 6520 3d20 6e70 2e7a 6572 6f73  orage = np.zeros
+000113d0: 2828 352c 2073 656c 662e 6c6f 6f70 5f72  ((5, self.loop_r
+000113e0: 616e 6765 2e73 697a 6529 290a 2020 2020  ange.size)).    
+000113f0: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6c      self.noise_l
+00011400: 6576 656c 5f73 746f 7261 6765 203d 206e  evel_storage = n
+00011410: 702e 7a65 726f 7328 2835 2c20 7365 6c66  p.zeros((5, self
+00011420: 2e6c 6f6f 705f 7261 6e67 652e 7369 7a65  .loop_range.size
+00011430: 2929 0a20 2020 2020 2020 2069 6620 6372  )).        if cr
+00011440: 6561 7465 5f70 6c6f 7420 3d3d 2046 616c  eate_plot == Fal
+00011450: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011460: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00011470: 656c 662e 6c6f 6f70 5f72 616e 6765 2e73  elf.loop_range.s
+00011480: 697a 6529 3a0a 2020 2020 2020 2020 2020  ize):.          
+00011490: 2020 2020 2020 6966 2070 7269 6e74 5f70        if print_p
+000114a0: 726f 6772 6573 733a 0a20 2020 2020 2020  rogress:.       
+000114b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000114c0: 6e74 2827 4361 6c63 756c 6174 6520 4d41  nt('Calculate MA
+000114d0: 5020 7265 7369 6c69 656e 6365 2066 6f72  P resilience for
+000114e0: 2077 696e 646f 7720 2720 2b20 7374 7228   window ' + str(
+000114f0: 6920 2b20 3129 202b 2027 206f 6620 2720  i + 1) + ' of ' 
+00011500: 2b20 7374 7228 7365 6c66 2e6c 6f6f 705f  + str(self.loop_
+00011510: 7261 6e67 652e 7369 7a65 2920 2b20 272e  range.size) + '.
+00011520: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00011530: 2020 2073 656c 662e 7769 6e64 6f77 5f73     self.window_s
+00011540: 6869 6674 203d 2073 656c 662e 6c6f 6f70  hift = self.loop
+00011550: 5f72 616e 6765 5b69 5d0a 2020 2020 2020  _range[i].      
+00011560: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00011570: 6361 6c63 5f4d 4150 5f72 6573 696c 6965  calc_MAP_resilie
+00011580: 6e63 6528 6372 6564 5f70 6572 6365 6e74  nce(cred_percent
+00011590: 696c 6573 2c20 6572 726f 725f 7072 6f70  iles, error_prop
+000115a0: 6167 6174 696f 6e2c 2073 756d 6d61 7279  agation, summary
+000115b0: 5f77 696e 646f 775f 7369 7a65 2c0a 2020  _window_size,.  
 000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115e0: 2020 2020 2020 2020 2073 6967 6d61 5f6d           sigma_m
-000115f0: 756c 7469 706c 6573 2c20 7072 696e 745f  ultiples, print_
-00011600: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
-00011610: 2020 2020 2020 2020 2073 656c 662e 736c           self.sl
-00011620: 6f70 655f 7374 6f72 6167 655b 3a2c 2069  ope_storage[:, i
-00011630: 5d20 3d20 7365 6c66 2e64 7269 6674 5f73  ] = self.drift_s
-00011640: 6c6f 7065 0a20 2020 2020 2020 2020 2020  lope.           
-00011650: 2020 2020 2073 656c 662e 6e6f 6973 655f       self.noise_
-00011660: 6c65 7665 6c5f 7374 6f72 6167 655b 3a2c  level_storage[:,
-00011670: 2069 5d20 3d20 7365 6c66 2e6e 6f69 7365   i] = self.noise
-00011680: 5f6c 6576 656c 5f65 7374 696d 6174 650a  _level_estimate.
-00011690: 2020 2020 2020 2020 656c 6966 2063 7265          elif cre
-000116a0: 6174 655f 706c 6f74 3a0a 2020 2020 2020  ate_plot:.      
-000116b0: 2020 2020 2020 7072 696e 7428 2754 6865        print('The
-000116c0: 204d 4150 2070 6c6f 7420 6665 6174 7572   MAP plot featur
-000116d0: 6520 6973 206e 6f74 2069 6d70 6c65 6d65  e is not impleme
-000116e0: 6e74 6564 2079 6574 2e27 290a 2020 2020  nted yet.').    
-000116f0: 2020 2020 6966 2065 7272 6f72 5f70 726f      if error_pro
-00011700: 7061 6761 7469 6f6e 203d 3d20 2773 756d  pagation == 'sum
-00011710: 6d61 7279 2073 7461 7469 7374 6963 7327  mary statistics'
-00011720: 2061 6e64 206e 6f74 2066 6173 744d 4150   and not fastMAP
-00011730: 666c 6167 3a0a 2020 2020 2020 2020 2020  flag:.          
-00011740: 2020 7365 6c66 2e73 6c6f 7065 5f73 746f    self.slope_sto
-00011750: 7261 6765 203d 2073 756d 6d61 7279 5f73  rage = summary_s
-00011760: 7461 7469 7374 6963 735f 6865 6c70 6572  tatistics_helper
-00011770: 2873 656c 662e 736c 6f70 655f 7374 6f72  (self.slope_stor
-00011780: 6167 652c 2073 756d 6d61 7279 5f77 696e  age, summary_win
-00011790: 646f 775f 7369 7a65 2c20 7369 676d 615f  dow_size, sigma_
-000117a0: 6d75 6c74 6970 6c65 7329 0a20 2020 2020  multiples).     
-000117b0: 2020 2069 6620 7361 7665 3a0a 2020 2020     if save:.    
-000117c0: 2020 2020 2020 2020 6e70 2e73 6176 6528          np.save(
-000117d0: 736c 6f70 655f 7361 7665 5f6e 616d 652c  slope_save_name,
-000117e0: 2073 656c 662e 736c 6f70 655f 7374 6f72   self.slope_stor
-000117f0: 6167 6529 0a20 2020 2020 2020 2020 2020  age).           
-00011800: 206e 702e 7361 7665 286e 6f69 7365 5f6c   np.save(noise_l
-00011810: 6576 656c 5f73 6176 655f 6e61 6d65 2c20  evel_save_name, 
-00011820: 7365 6c66 2e6e 6f69 7365 5f6c 6576 656c  self.noise_level
-00011830: 5f73 746f 7261 6765 290a 0a0a 2020 2020  _storage)...    
-00011840: 6465 6620 5f70 7265 7061 7265 5f64 6174  def _prepare_dat
-00011850: 6128 7365 6c66 2c20 7072 696e 7462 6f6f  a(self, printboo
-00011860: 6c29 3a0a 2020 2020 2020 2020 2222 220a  l):.        """.
-00011870: 2020 2020 2020 2020 4865 6c70 6572 2066          Helper f
-00011880: 756e 6374 696f 6e20 746f 2063 616c 6375  unction to calcu
-00011890: 6c61 7465 2074 6865 2069 6e63 7265 6d65  late the increme
-000118a0: 6e74 7320 696e 2063 6173 6520 6f66 2061  nts in case of a
-000118b0: 2060 604c 616e 6765 7669 6e45 7374 696d   ``LangevinEstim
-000118c0: 6174 696f 6e60 6020 6f62 6a65 6374 2e0a  ation`` object..
-000118d0: 2020 2020 2020 2020 5468 6520 6060 7072          The ``pr
-000118e0: 696e 7462 6f6f 6c60 6020 7061 7261 6d65  intbool`` parame
-000118f0: 7465 7220 6973 206a 7573 7420 6120 706c  ter is just a pl
-00011900: 6163 6568 6f6c 6465 7220 666f 7220 7468  aceholder for th
-00011910: 6520 6f76 6572 6c6f 6164 6564 2066 756e  e overloaded fun
-00011920: 6374 696f 6e20 6f66 2074 6865 0a20 2020  ction of the.   
-00011930: 2020 2020 2060 6042 696e 6e69 6e67 4c61       ``BinningLa
-00011940: 6e67 6576 696e 4573 7469 6d61 7469 6f6e  ngevinEstimation
-00011950: 6060 2063 6c61 7373 2e0a 2020 2020 2020  `` class..      
-00011960: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00011970: 6c66 2e69 6e63 7265 6d65 6e74 7320 3d20  lf.increments = 
-00011980: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
-00011990: 5b31 3a5d 202d 2073 656c 662e 6461 7461  [1:] - self.data
-000119a0: 5f77 696e 646f 775b 3a2d 315d 0a0a 0a20  _window[:-1]... 
-000119b0: 2020 2064 6566 205f 6361 6c63 5f4d 4150     def _calc_MAP
-000119c0: 5f72 6573 696c 6965 6e63 6528 7365 6c66  _resilience(self
-000119d0: 2c20 6372 6564 5f70 6572 6365 6e74 696c  , cred_percentil
-000119e0: 6573 2c20 6572 726f 725f 7072 6f70 6167  es, error_propag
-000119f0: 6174 696f 6e2c 2073 756d 6d61 7279 5f77  ation, summary_w
-00011a00: 696e 646f 775f 7369 7a65 2c0a 2020 2020  indow_size,.    
+000115e0: 2020 2020 2020 2020 7369 676d 615f 6d75          sigma_mu
+000115f0: 6c74 6970 6c65 732c 2070 7269 6e74 5f64  ltiples, print_d
+00011600: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
+00011610: 2020 2020 2020 2020 7365 6c66 2e73 6c6f          self.slo
+00011620: 7065 5f73 746f 7261 6765 5b3a 2c20 695d  pe_storage[:, i]
+00011630: 203d 2073 656c 662e 6472 6966 745f 736c   = self.drift_sl
+00011640: 6f70 650a 2020 2020 2020 2020 2020 2020  ope.            
+00011650: 2020 2020 7365 6c66 2e6e 6f69 7365 5f6c      self.noise_l
+00011660: 6576 656c 5f73 746f 7261 6765 5b3a 2c20  evel_storage[:, 
+00011670: 695d 203d 2073 656c 662e 6e6f 6973 655f  i] = self.noise_
+00011680: 6c65 7665 6c5f 6573 7469 6d61 7465 0a20  level_estimate. 
+00011690: 2020 2020 2020 2065 6c69 6620 6372 6561         elif crea
+000116a0: 7465 5f70 6c6f 743a 0a20 2020 2020 2020  te_plot:.       
+000116b0: 2020 2020 2070 7269 6e74 2827 5468 6520       print('The 
+000116c0: 4d41 5020 706c 6f74 2066 6561 7475 7265  MAP plot feature
+000116d0: 2069 7320 6e6f 7420 696d 706c 656d 656e   is not implemen
+000116e0: 7465 6420 7965 742e 2729 0a20 2020 2020  ted yet.').     
+000116f0: 2020 2069 6620 6572 726f 725f 7072 6f70     if error_prop
+00011700: 6167 6174 696f 6e20 3d3d 2027 7375 6d6d  agation == 'summ
+00011710: 6172 7920 7374 6174 6973 7469 6373 2720  ary statistics' 
+00011720: 616e 6420 6e6f 7420 6661 7374 4d41 5066  and not fastMAPf
+00011730: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
+00011740: 2073 656c 662e 736c 6f70 655f 7374 6f72   self.slope_stor
+00011750: 6167 6520 3d20 7375 6d6d 6172 795f 7374  age = summary_st
+00011760: 6174 6973 7469 6373 5f68 656c 7065 7228  atistics_helper(
+00011770: 7365 6c66 2e73 6c6f 7065 5f73 746f 7261  self.slope_stora
+00011780: 6765 2c20 7375 6d6d 6172 795f 7769 6e64  ge, summary_wind
+00011790: 6f77 5f73 697a 652c 2073 6967 6d61 5f6d  ow_size, sigma_m
+000117a0: 756c 7469 706c 6573 290a 2020 2020 2020  ultiples).      
+000117b0: 2020 6966 2073 6176 653a 0a20 2020 2020    if save:.     
+000117c0: 2020 2020 2020 206e 702e 7361 7665 2873         np.save(s
+000117d0: 6c6f 7065 5f73 6176 655f 6e61 6d65 2c20  lope_save_name, 
+000117e0: 7365 6c66 2e73 6c6f 7065 5f73 746f 7261  self.slope_stora
+000117f0: 6765 290a 2020 2020 2020 2020 2020 2020  ge).            
+00011800: 6e70 2e73 6176 6528 6e6f 6973 655f 6c65  np.save(noise_le
+00011810: 7665 6c5f 7361 7665 5f6e 616d 652c 2073  vel_save_name, s
+00011820: 656c 662e 6e6f 6973 655f 6c65 7665 6c5f  elf.noise_level_
+00011830: 7374 6f72 6167 6529 0a0a 0a20 2020 2064  storage)...    d
+00011840: 6566 205f 7072 6570 6172 655f 6461 7461  ef _prepare_data
+00011850: 2873 656c 662c 2070 7269 6e74 626f 6f6c  (self, printbool
+00011860: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00011870: 2020 2020 2020 2048 656c 7065 7220 6675         Helper fu
+00011880: 6e63 7469 6f6e 2074 6f20 6361 6c63 756c  nction to calcul
+00011890: 6174 6520 7468 6520 696e 6372 656d 656e  ate the incremen
+000118a0: 7473 2069 6e20 6361 7365 206f 6620 6120  ts in case of a 
+000118b0: 6060 4c61 6e67 6576 696e 4573 7469 6d61  ``LangevinEstima
+000118c0: 7469 6f6e 6060 206f 626a 6563 742e 0a20  tion`` object.. 
+000118d0: 2020 2020 2020 2054 6865 2060 6070 7269         The ``pri
+000118e0: 6e74 626f 6f6c 6060 2070 6172 616d 6574  ntbool`` paramet
+000118f0: 6572 2069 7320 6a75 7374 2061 2070 6c61  er is just a pla
+00011900: 6365 686f 6c64 6572 2066 6f72 2074 6865  ceholder for the
+00011910: 206f 7665 726c 6f61 6465 6420 6675 6e63   overloaded func
+00011920: 7469 6f6e 206f 6620 7468 650a 2020 2020  tion of the.    
+00011930: 2020 2020 6060 4269 6e6e 696e 674c 616e      ``BinningLan
+00011940: 6765 7669 6e45 7374 696d 6174 696f 6e60  gevinEstimation`
+00011950: 6020 636c 6173 732e 0a20 2020 2020 2020  ` class..       
+00011960: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00011970: 662e 696e 6372 656d 656e 7473 203d 2073  f.increments = s
+00011980: 656c 662e 6461 7461 5f77 696e 646f 775b  elf.data_window[
+00011990: 313a 5d20 2d20 7365 6c66 2e64 6174 615f  1:] - self.data_
+000119a0: 7769 6e64 6f77 5b3a 2d31 5d0a 0a0a 2020  window[:-1]...  
+000119b0: 2020 6465 6620 5f63 616c 635f 4d41 505f    def _calc_MAP_
+000119c0: 7265 7369 6c69 656e 6365 2873 656c 662c  resilience(self,
+000119d0: 2063 7265 645f 7065 7263 656e 7469 6c65   cred_percentile
+000119e0: 732c 2065 7272 6f72 5f70 726f 7061 6761  s, error_propaga
+000119f0: 7469 6f6e 2c20 7375 6d6d 6172 795f 7769  tion, summary_wi
+00011a00: 6e64 6f77 5f73 697a 652c 0a20 2020 2020  ndow_size,.     
 00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 2020 2020 2020 7369 676d 615f 6d75          sigma_mu
-00011a30: 6c74 6970 6c65 732c 2070 7269 6e74 5f64  ltiples, print_d
-00011a40: 6574 6169 6c73 293a 0a20 2020 2020 2020  etails):.       
-00011a50: 2022 2222 0a20 2020 2020 2020 2048 656c   """.        Hel
-00011a60: 7065 7220 6675 6e63 7469 6f6e 2074 6861  per function tha
-00011a70: 7420 636f 6d70 7574 6573 2074 6865 204d  t computes the M
-00011a80: 4150 2065 7374 696d 6174 6573 206f 6620  AP estimates of 
-00011a90: 6472 6966 7420 736c 6f70 6520 3a6d 6174  drift slope :mat
-00011aa0: 683a 605c 6861 747b 5c7a 6574 617d 6020  h:`\hat{\zeta}` 
-00011ab0: 616e 6420 6e6f 6973 6520 6c65 7665 6c0a  and noise level.
-00011ac0: 2020 2020 2020 2020 3a6d 6174 683a 605c          :math:`\
-00011ad0: 6861 747b 5c73 6967 6d61 7d60 2077 6974  hat{\sigma}` wit
-00011ae0: 6820 636f 7272 6573 706f 6e64 696e 6720  h corresponding 
-00011af0: 636f 6e66 6964 656e 6365 2062 616e 6473  confidence bands
-00011b00: 2063 7265 6174 6564 2077 6974 6820 5769   created with Wi
-00011b10: 6c6b 7327 2074 6865 6f72 656d 2061 6e64  lks' theorem and
-00011b20: 0a20 2020 2020 2020 2047 6175 7373 6961  .        Gaussia
-00011b30: 6e20 7072 6f70 6167 6174 696f 6e20 6f66  n propagation of
-00011b40: 2075 6e65 7274 6169 6e74 7920 666f 7220   unertainty for 
-00011b50: 6120 6769 7665 6e20 6060 7769 6e64 6f77  a given ``window
-00011b60: 5f73 697a 6560 6020 616e 6420 6060 7769  _size`` and ``wi
-00011b70: 6e64 6f77 5f73 6869 6674 6060 2073 746f  ndow_shift`` sto
-00011b80: 7265 640a 2020 2020 2020 2020 696e 2074  red.        in t
-00011b90: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00011ba0: 2061 7474 7269 6275 7465 732e 0a20 2020   attributes..   
-00011bb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011bc0: 2073 656c 662e 6461 7461 5f77 696e 646f   self.data_windo
-00011bd0: 7720 3d20 6e70 2e72 6f6c 6c28 7365 6c66  w = np.roll(self
-00011be0: 2e64 6174 612c 2073 6869 6674 3d2d 2073  .data, shift=- s
-00011bf0: 656c 662e 7769 6e64 6f77 5f73 6869 6674  elf.window_shift
-00011c00: 295b 3a73 656c 662e 7769 6e64 6f77 5f73  )[:self.window_s
-00011c10: 697a 655d 0a20 2020 2020 2020 2073 656c  ize].        sel
-00011c20: 662e 7469 6d65 5f77 696e 646f 7720 3d20  f.time_window = 
-00011c30: 6e70 2e72 6f6c 6c28 7365 6c66 2e74 696d  np.roll(self.tim
-00011c40: 652c 2073 6869 6674 3d2d 2073 656c 662e  e, shift=- self.
-00011c50: 7769 6e64 6f77 5f73 6869 6674 295b 3a73  window_shift)[:s
-00011c60: 656c 662e 7769 6e64 6f77 5f73 697a 655d  elf.window_size]
-00011c70: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
-00011c80: 7265 7061 7265 5f64 6174 6128 7072 696e  repare_data(prin
-00011c90: 7462 6f6f 6c3d 7072 696e 745f 6465 7461  tbool=print_deta
-00011ca0: 696c 7329 0a20 2020 2020 2020 2073 656c  ils).        sel
-00011cb0: 662e 5f63 6f6d 7075 7465 5f4d 4150 5f65  f._compute_MAP_e
-00011cc0: 7374 696d 6174 6573 2870 7269 6e74 626f  stimates(printbo
-00011cd0: 6f6c 3d70 7269 6e74 5f64 6574 6169 6c73  ol=print_details
-00011ce0: 290a 2020 2020 2020 2020 6966 2070 7269  ).        if pri
-00011cf0: 6e74 5f64 6574 6169 6c73 3a0a 2020 2020  nt_details:.    
-00011d00: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
+00011a20: 2020 2020 2020 2073 6967 6d61 5f6d 756c         sigma_mul
+00011a30: 7469 706c 6573 2c20 7072 696e 745f 6465  tiples, print_de
+00011a40: 7461 696c 7329 3a0a 2020 2020 2020 2020  tails):.        
+00011a50: 2222 220a 2020 2020 2020 2020 4865 6c70  """.        Help
+00011a60: 6572 2066 756e 6374 696f 6e20 7468 6174  er function that
+00011a70: 2063 6f6d 7075 7465 7320 7468 6520 4d41   computes the MA
+00011a80: 5020 6573 7469 6d61 7465 7320 6f66 2064  P estimates of d
+00011a90: 7269 6674 2073 6c6f 7065 203a 6d61 7468  rift slope :math
+00011aa0: 3a60 5c68 6174 7b5c 7a65 7461 7d60 2061  :`\hat{\zeta}` a
+00011ab0: 6e64 206e 6f69 7365 206c 6576 656c 0a20  nd noise level. 
+00011ac0: 2020 2020 2020 203a 6d61 7468 3a60 5c68         :math:`\h
+00011ad0: 6174 7b5c 7369 676d 617d 6020 7769 7468  at{\sigma}` with
+00011ae0: 2063 6f72 7265 7370 6f6e 6469 6e67 2063   corresponding c
+00011af0: 6f6e 6669 6465 6e63 6520 6261 6e64 7320  onfidence bands 
+00011b00: 6372 6561 7465 6420 7769 7468 2057 696c  created with Wil
+00011b10: 6b73 2720 7468 656f 7265 6d20 616e 640a  ks' theorem and.
+00011b20: 2020 2020 2020 2020 4761 7573 7369 616e          Gaussian
+00011b30: 2070 726f 7061 6761 7469 6f6e 206f 6620   propagation of 
+00011b40: 756e 6572 7461 696e 7479 2066 6f72 2061  unertainty for a
+00011b50: 2067 6976 656e 2060 6077 696e 646f 775f   given ``window_
+00011b60: 7369 7a65 6060 2061 6e64 2060 6077 696e  size`` and ``win
+00011b70: 646f 775f 7368 6966 7460 6020 7374 6f72  dow_shift`` stor
+00011b80: 6564 0a20 2020 2020 2020 2069 6e20 7468  ed.        in th
+00011b90: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+00011ba0: 6174 7472 6962 7574 6573 2e0a 2020 2020  attributes..    
+00011bb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011bc0: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
+00011bd0: 203d 206e 702e 726f 6c6c 2873 656c 662e   = np.roll(self.
+00011be0: 6461 7461 2c20 7368 6966 743d 2d20 7365  data, shift=- se
+00011bf0: 6c66 2e77 696e 646f 775f 7368 6966 7429  lf.window_shift)
+00011c00: 5b3a 7365 6c66 2e77 696e 646f 775f 7369  [:self.window_si
+00011c10: 7a65 5d0a 2020 2020 2020 2020 7365 6c66  ze].        self
+00011c20: 2e74 696d 655f 7769 6e64 6f77 203d 206e  .time_window = n
+00011c30: 702e 726f 6c6c 2873 656c 662e 7469 6d65  p.roll(self.time
+00011c40: 2c20 7368 6966 743d 2d20 7365 6c66 2e77  , shift=- self.w
+00011c50: 696e 646f 775f 7368 6966 7429 5b3a 7365  indow_shift)[:se
+00011c60: 6c66 2e77 696e 646f 775f 7369 7a65 5d0a  lf.window_size].
+00011c70: 2020 2020 2020 2020 7365 6c66 2e5f 7072          self._pr
+00011c80: 6570 6172 655f 6461 7461 2870 7269 6e74  epare_data(print
+00011c90: 626f 6f6c 3d70 7269 6e74 5f64 6574 6169  bool=print_detai
+00011ca0: 6c73 290a 2020 2020 2020 2020 7365 6c66  ls).        self
+00011cb0: 2e5f 636f 6d70 7574 655f 4d41 505f 6573  ._compute_MAP_es
+00011cc0: 7469 6d61 7465 7328 7072 696e 7462 6f6f  timates(printboo
+00011cd0: 6c3d 7072 696e 745f 6465 7461 696c 7329  l=print_details)
+00011ce0: 0a20 2020 2020 2020 2069 6620 7072 696e  .        if prin
+00011cf0: 745f 6465 7461 696c 733a 0a20 2020 2020  t_details:.     
+00011d00: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
 00011d10: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00011d20: 5f5f 5f5f 5f5f 5f5f 5f27 290a 2020 2020  _________').    
-00011d30: 2020 2020 2020 2020 7072 696e 7428 2743          print('C
-00011d40: 616c 6375 6c61 7465 204d 4150 2064 7269  alculate MAP dri
-00011d50: 6674 2073 6c6f 7065 2127 290a 2020 2020  ft slope!').    
-00011d60: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
+00011d20: 5f5f 5f5f 5f5f 5f5f 2729 0a20 2020 2020  ________').     
+00011d30: 2020 2020 2020 2070 7269 6e74 2827 4361         print('Ca
+00011d40: 6c63 756c 6174 6520 4d41 5020 6472 6966  lculate MAP drif
+00011d50: 7420 736c 6f70 6521 2729 0a20 2020 2020  t slope!').     
+00011d60: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
 00011d70: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00011d80: 5f5f 5f5f 5f5f 5f5f 5f27 290a 2020 2020  _________').    
-00011d90: 2020 2020 6966 2073 656c 662e 6472 6966      if self.drif
-00011da0: 745f 6d6f 6465 6c20 3d3d 2027 3372 6420  t_model == '3rd 
-00011db0: 6f72 6465 7220 706f 6c79 6e6f 6d69 616c  order polynomial
-00011dc0: 273a 0a20 2020 2020 2020 2020 2020 2073  ':.            s
-00011dd0: 656c 662e 5f4d 4150 5f74 6869 7264 5f6f  elf._MAP_third_o
-00011de0: 7264 6572 5f70 6f6c 796e 6f6d 5f73 6c6f  rder_polynom_slo
-00011df0: 7065 5f69 6e5f 6669 7865 645f 706f 696e  pe_in_fixed_poin
-00011e00: 7428 290a 2020 2020 2020 2020 656c 6966  t().        elif
-00011e10: 2073 656c 662e 6472 6966 745f 6d6f 6465   self.drift_mode
-00011e20: 6c20 3d3d 2027 6c69 6e65 6172 206d 6f64  l == 'linear mod
-00011e30: 656c 273a 0a20 2020 2020 2020 2020 2020  el':.           
-00011e40: 2073 656c 662e 6472 6966 745f 736c 6f70   self.drift_slop
-00011e50: 655b 305d 203d 2073 656c 662e 4d41 505f  e[0] = self.MAP_
-00011e60: 7468 6574 615b 312c 2030 5d0a 2020 2020  theta[1, 0].    
-00011e70: 2020 2020 6966 2070 7269 6e74 5f64 6574      if print_det
-00011e80: 6169 6c73 3a0a 2020 2020 2020 2020 2020  ails:.          
-00011e90: 2020 7072 696e 7428 275f 5f5f 5f5f 2729    print('_____')
-00011ea0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00011eb0: 6e74 2827 446f 6e65 2127 290a 2020 2020  nt('Done!').    
-00011ec0: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
-00011ed0: 5f5f 5f5f 2729 0a20 2020 2020 2020 2073  ____').        s
-00011ee0: 656c 662e 5f64 6574 6572 6d69 6e65 5f63  elf._determine_c
-00011ef0: 6f6e 6669 6465 6e63 655f 6261 6e64 7328  onfidence_bands(
-00011f00: 7369 6752 6174 696f 3d63 7265 645f 7065  sigRatio=cred_pe
-00011f10: 7263 656e 7469 6c65 732c 2070 7269 6e74  rcentiles, print
-00011f20: 626f 6f6c 3d70 7269 6e74 5f64 6574 6169  bool=print_detai
-00011f30: 6c73 290a 2020 2020 2020 2020 6966 2065  ls).        if e
-00011f40: 7272 6f72 5f70 726f 7061 6761 7469 6f6e  rror_propagation
-00011f50: 203d 3d20 2765 7272 6f72 2062 6f75 6e64   == 'error bound
-00011f60: 273a 0a20 2020 2020 2020 2020 2020 2073  ':.            s
-00011f70: 656c 662e 5f63 6f6d 7075 7465 5f73 6c6f  elf._compute_slo
-00011f80: 7065 5f65 7272 6f72 5f6d 6172 6769 6e28  pe_error_margin(
-00011f90: 7072 696e 7462 6f6f 6c3d 7072 696e 745f  printbool=print_
-00011fa0: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
-00011fb0: 2065 6c69 6620 6572 726f 725f 7072 6f70   elif error_prop
-00011fc0: 6167 6174 696f 6e20 3d3d 2027 756e 636f  agation == 'unco
-00011fd0: 7272 656c 6174 6564 2047 6175 7373 6961  rrelated Gaussia
-00011fe0: 6e27 3a0a 2020 2020 2020 2020 2020 2020  n':.            
-00011ff0: 7365 6c66 2e5f 636f 6d70 7574 655f 736c  self._compute_sl
-00012000: 6f70 655f 6572 726f 7273 2870 7269 6e74  ope_errors(print
-00012010: 626f 6f6c 3d70 7269 6e74 5f64 6574 6169  bool=print_detai
-00012020: 6c73 290a 0a0a 2020 2020 6465 6620 5f63  ls)...    def _c
-00012030: 6f6d 7075 7465 5f4d 4150 5f65 7374 696d  ompute_MAP_estim
-00012040: 6174 6573 2873 656c 662c 2070 7269 6e74  ates(self, print
-00012050: 626f 6f6c 3d46 616c 7365 2c20 7072 696e  bool=False, prin
-00012060: 745f 7469 6d65 5f73 6361 6c65 5f69 6e66  t_time_scale_inf
-00012070: 6f20 3d20 4e6f 6e65 293a 0a20 2020 2020  o = None):.     
-00012080: 2020 2022 2222 0a20 2020 2020 2020 2048     """.        H
-00012090: 656c 7065 7220 6675 6e63 7469 6f6e 2074  elper function t
-000120a0: 6861 7420 6465 7465 726d 696e 6573 2074  hat determines t
-000120b0: 6865 2060 604d 4150 5f74 6865 7461 6060  he ``MAP_theta``
-000120c0: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-000120d0: 6d20 7072 696e 7462 6f6f 6c3a 2049 6620  m printbool: If 
-000120e0: 6060 5472 7565 6060 2061 2064 6574 6169  ``True`` a detai
-000120f0: 6c65 6420 6f75 7470 7574 2069 7320 7072  led output is pr
-00012100: 696e 7465 642e 0a20 2020 2020 2020 203a  inted..        :
-00012110: 7479 7065 2070 7269 6e74 626f 6f6c 3a20  type printbool: 
-00012120: 426f 6f6c 6561 6e0a 2020 2020 2020 2020  Boolean.        
-00012130: 2222 220a 2020 2020 2020 2020 6966 2070  """.        if p
-00012140: 7269 6e74 626f 6f6c 3a0a 2020 2020 2020  rintbool:.      
-00012150: 2020 2020 2020 7072 696e 7428 275f 5f5f        print('___
+00011d80: 5f5f 5f5f 5f5f 5f5f 2729 0a20 2020 2020  ________').     
+00011d90: 2020 2069 6620 7365 6c66 2e64 7269 6674     if self.drift
+00011da0: 5f6d 6f64 656c 203d 3d20 2733 7264 206f  _model == '3rd o
+00011db0: 7264 6572 2070 6f6c 796e 6f6d 6961 6c27  rder polynomial'
+00011dc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011dd0: 6c66 2e5f 4d41 505f 7468 6972 645f 6f72  lf._MAP_third_or
+00011de0: 6465 725f 706f 6c79 6e6f 6d5f 736c 6f70  der_polynom_slop
+00011df0: 655f 696e 5f66 6978 6564 5f70 6f69 6e74  e_in_fixed_point
+00011e00: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+00011e10: 7365 6c66 2e64 7269 6674 5f6d 6f64 656c  self.drift_model
+00011e20: 203d 3d20 276c 696e 6561 7220 6d6f 6465   == 'linear mode
+00011e30: 6c27 3a0a 2020 2020 2020 2020 2020 2020  l':.            
+00011e40: 7365 6c66 2e64 7269 6674 5f73 6c6f 7065  self.drift_slope
+00011e50: 5b30 5d20 3d20 7365 6c66 2e4d 4150 5f74  [0] = self.MAP_t
+00011e60: 6865 7461 5b31 2c20 305d 0a20 2020 2020  heta[1, 0].     
+00011e70: 2020 2069 6620 7072 696e 745f 6465 7461     if print_deta
+00011e80: 696c 733a 0a20 2020 2020 2020 2020 2020  ils:.           
+00011e90: 2070 7269 6e74 2827 5f5f 5f5f 5f27 290a   print('_____').
+00011ea0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011eb0: 7428 2744 6f6e 6521 2729 0a20 2020 2020  t('Done!').     
+00011ec0: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
+00011ed0: 5f5f 5f27 290a 2020 2020 2020 2020 7365  ___').        se
+00011ee0: 6c66 2e5f 6465 7465 726d 696e 655f 636f  lf._determine_co
+00011ef0: 6e66 6964 656e 6365 5f62 616e 6473 2873  nfidence_bands(s
+00011f00: 6967 5261 7469 6f3d 6372 6564 5f70 6572  igRatio=cred_per
+00011f10: 6365 6e74 696c 6573 2c20 7072 696e 7462  centiles, printb
+00011f20: 6f6f 6c3d 7072 696e 745f 6465 7461 696c  ool=print_detail
+00011f30: 7329 0a20 2020 2020 2020 2069 6620 6572  s).        if er
+00011f40: 726f 725f 7072 6f70 6167 6174 696f 6e20  ror_propagation 
+00011f50: 3d3d 2027 6572 726f 7220 626f 756e 6427  == 'error bound'
+00011f60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011f70: 6c66 2e5f 636f 6d70 7574 655f 736c 6f70  lf._compute_slop
+00011f80: 655f 6572 726f 725f 6d61 7267 696e 2870  e_error_margin(p
+00011f90: 7269 6e74 626f 6f6c 3d70 7269 6e74 5f64  rintbool=print_d
+00011fa0: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
+00011fb0: 656c 6966 2065 7272 6f72 5f70 726f 7061  elif error_propa
+00011fc0: 6761 7469 6f6e 203d 3d20 2775 6e63 6f72  gation == 'uncor
+00011fd0: 7265 6c61 7465 6420 4761 7573 7369 616e  related Gaussian
+00011fe0: 273a 0a20 2020 2020 2020 2020 2020 2073  ':.            s
+00011ff0: 656c 662e 5f63 6f6d 7075 7465 5f73 6c6f  elf._compute_slo
+00012000: 7065 5f65 7272 6f72 7328 7072 696e 7462  pe_errors(printb
+00012010: 6f6f 6c3d 7072 696e 745f 6465 7461 696c  ool=print_detail
+00012020: 7329 0a0a 0a20 2020 2064 6566 205f 636f  s)...    def _co
+00012030: 6d70 7574 655f 4d41 505f 6573 7469 6d61  mpute_MAP_estima
+00012040: 7465 7328 7365 6c66 2c20 7072 696e 7462  tes(self, printb
+00012050: 6f6f 6c3d 4661 6c73 652c 2070 7269 6e74  ool=False, print
+00012060: 5f74 696d 655f 7363 616c 655f 696e 666f  _time_scale_info
+00012070: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00012080: 2020 2222 220a 2020 2020 2020 2020 4865    """.        He
+00012090: 6c70 6572 2066 756e 6374 696f 6e20 7468  lper function th
+000120a0: 6174 2064 6574 6572 6d69 6e65 7320 7468  at determines th
+000120b0: 6520 6060 4d41 505f 7468 6574 6160 602e  e ``MAP_theta``.
+000120c0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000120d0: 2070 7269 6e74 626f 6f6c 3a20 4966 2060   printbool: If `
+000120e0: 6054 7275 6560 6020 6120 6465 7461 696c  `True`` a detail
+000120f0: 6564 206f 7574 7075 7420 6973 2070 7269  ed output is pri
+00012100: 6e74 6564 2e0a 2020 2020 2020 2020 3a74  nted..        :t
+00012110: 7970 6520 7072 696e 7462 6f6f 6c3a 2042  ype printbool: B
+00012120: 6f6f 6c65 616e 0a20 2020 2020 2020 2022  oolean.        "
+00012130: 2222 0a20 2020 2020 2020 2069 6620 7072  "".        if pr
+00012140: 696e 7462 6f6f 6c3a 0a20 2020 2020 2020  intbool:.       
+00012150: 2020 2020 2070 7269 6e74 2827 5f5f 5f5f       print('____
 00012160: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00012170: 5f5f 5f27 290a 2020 2020 2020 2020 2020  ___').          
-00012180: 2020 7072 696e 7428 2750 6572 666f 726d    print('Perform
-00012190: 204d 4150 2065 7374 696d 6174 696f 6e21   MAP estimation!
-000121a0: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
-000121b0: 7269 6e74 2827 5f5f 5f5f 5f5f 5f5f 5f5f  rint('__________
-000121c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 2729 0a20  ____________'). 
-000121d0: 2020 2020 2020 2070 6172 3020 3d20 6e70         par0 = np
-000121e0: 2e6f 6e65 7328 7365 6c66 2e6e 6469 6d29  .ones(self.ndim)
-000121f0: 0a20 2020 2020 2020 2073 656c 662e 4d41  .        self.MA
-00012200: 505f 7468 6574 6120 3d20 6e70 2e7a 6572  P_theta = np.zer
-00012210: 6f73 2828 7365 6c66 2e6e 6469 6d2c 2035  os((self.ndim, 5
-00012220: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
-00012230: 6c66 2e61 6e74 6943 5079 4f62 6a65 6374  lf.antiCPyObject
-00012240: 203d 3d20 274c 616e 6765 7669 6e45 7374   == 'LangevinEst
-00012250: 696d 6174 696f 6e27 3a0a 2020 2020 2020  imation':.      
-00012260: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
-00012270: 7061 7261 6c6c 656c 5f45 6e73 656d 626c  parallel_Ensembl
-00012280: 6553 616d 706c 6572 2873 656c 662e 6461  eSampler(self.da
-00012290: 7461 5f77 696e 646f 772c 2073 656c 662e  ta_window, self.
-000122a0: 6474 2c20 7365 6c66 2e64 7269 6674 5f6d  dt, self.drift_m
-000122b0: 6f64 656c 2c20 7365 6c66 2e64 6966 6675  odel, self.diffu
-000122c0: 7369 6f6e 5f6d 6f64 656c 2c0a 2020 2020  sion_model,.    
+00012170: 5f5f 2729 0a20 2020 2020 2020 2020 2020  __').           
+00012180: 2070 7269 6e74 2827 5065 7266 6f72 6d20   print('Perform 
+00012190: 4d41 5020 6573 7469 6d61 7469 6f6e 2127  MAP estimation!'
+000121a0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+000121b0: 696e 7428 275f 5f5f 5f5f 5f5f 5f5f 5f5f  int('___________
+000121c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f27 290a 2020  ___________').  
+000121d0: 2020 2020 2020 7061 7230 203d 206e 702e        par0 = np.
+000121e0: 6f6e 6573 2873 656c 662e 6e64 696d 290a  ones(self.ndim).
+000121f0: 2020 2020 2020 2020 7365 6c66 2e4d 4150          self.MAP
+00012200: 5f74 6865 7461 203d 206e 702e 7a65 726f  _theta = np.zero
+00012210: 7328 2873 656c 662e 6e64 696d 2c20 3529  s((self.ndim, 5)
+00012220: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00012230: 662e 616e 7469 4350 794f 626a 6563 7420  f.antiCPyObject 
+00012240: 3d3d 2027 4c61 6e67 6576 696e 4573 7469  == 'LangevinEsti
+00012250: 6d61 7469 6f6e 273a 0a20 2020 2020 2020  mation':.       
+00012260: 2020 2020 2073 656c 662e 696e 6974 5f70       self.init_p
+00012270: 6172 616c 6c65 6c5f 456e 7365 6d62 6c65  arallel_Ensemble
+00012280: 5361 6d70 6c65 7228 7365 6c66 2e64 6174  Sampler(self.dat
+00012290: 615f 7769 6e64 6f77 2c20 7365 6c66 2e64  a_window, self.d
+000122a0: 742c 2073 656c 662e 6472 6966 745f 6d6f  t, self.drift_mo
+000122b0: 6465 6c2c 2073 656c 662e 6469 6666 7573  del, self.diffus
+000122c0: 696f 6e5f 6d6f 6465 6c2c 0a20 2020 2020  ion_model,.     
 000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012300: 2e70 7269 6f72 5f74 7970 652c 2073 656c  .prior_type, sel
-00012310: 662e 7072 696f 725f 7261 6e67 652c 2073  f.prior_range, s
-00012320: 656c 662e 7363 616c 6573 290a 2020 2020  elf.scales).    
-00012330: 2020 2020 656c 6966 2073 656c 662e 616e      elif self.an
-00012340: 7469 4350 794f 626a 6563 7420 3d3d 2027  tiCPyObject == '
-00012350: 4e6f 6e4d 6172 6b6f 7645 7374 696d 6174  NonMarkovEstimat
-00012360: 696f 6e27 3a0a 2020 2020 2020 2020 2020  ion':.          
-00012370: 2020 7365 6c66 2e69 6e69 745f 7061 7261    self.init_para
-00012380: 6c6c 656c 5f45 6e73 656d 626c 6553 616d  llel_EnsembleSam
-00012390: 706c 6572 2873 656c 662e 6461 7461 5f77  pler(self.data_w
-000123a0: 696e 646f 772c 2073 656c 662e 585f 6472  indow, self.X_dr
-000123b0: 6966 745f 6d6f 6465 6c2c 2073 656c 662e  ift_model, self.
-000123c0: 595f 6472 6966 745f 6d6f 6465 6c2c 2073  Y_drift_model, s
-000123d0: 656c 662e 595f 6469 6666 7573 696f 6e5f  elf.Y_diffusion_
-000123e0: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
+000122f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012300: 7072 696f 725f 7479 7065 2c20 7365 6c66  prior_type, self
+00012310: 2e70 7269 6f72 5f72 616e 6765 2c20 7365  .prior_range, se
+00012320: 6c66 2e73 6361 6c65 7329 0a20 2020 2020  lf.scales).     
+00012330: 2020 2065 6c69 6620 7365 6c66 2e61 6e74     elif self.ant
+00012340: 6943 5079 4f62 6a65 6374 203d 3d20 274e  iCPyObject == 'N
+00012350: 6f6e 4d61 726b 6f76 4573 7469 6d61 7469  onMarkovEstimati
+00012360: 6f6e 273a 0a20 2020 2020 2020 2020 2020  on':.           
+00012370: 2073 656c 662e 696e 6974 5f70 6172 616c   self.init_paral
+00012380: 6c65 6c5f 456e 7365 6d62 6c65 5361 6d70  lel_EnsembleSamp
+00012390: 6c65 7228 7365 6c66 2e64 6174 615f 7769  ler(self.data_wi
+000123a0: 6e64 6f77 2c20 7365 6c66 2e58 5f64 7269  ndow, self.X_dri
+000123b0: 6674 5f6d 6f64 656c 2c20 7365 6c66 2e59  ft_model, self.Y
+000123c0: 5f64 7269 6674 5f6d 6f64 656c 2c20 7365  _drift_model, se
+000123d0: 6c66 2e59 5f64 6966 6675 7369 6f6e 5f6d  lf.Y_diffusion_m
+000123e0: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
 000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012400: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012410: 6c66 2e58 5f63 6f75 706c 696e 675f 7465  lf.X_coupling_te
-00012420: 726d 2c20 7365 6c66 2e59 5f6d 6f64 656c  rm, self.Y_model
-00012430: 2c20 7365 6c66 2e64 742c 2073 656c 662e  , self.dt, self.
-00012440: 7072 696f 725f 7479 7065 2c20 7365 6c66  prior_type, self
-00012450: 2e70 7269 6f72 5f72 616e 6765 2c0a 2020  .prior_range,.  
+00012400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012410: 662e 585f 636f 7570 6c69 6e67 5f74 6572  f.X_coupling_ter
+00012420: 6d2c 2073 656c 662e 595f 6d6f 6465 6c2c  m, self.Y_model,
+00012430: 2073 656c 662e 6474 2c20 7365 6c66 2e70   self.dt, self.p
+00012440: 7269 6f72 5f74 7970 652c 2073 656c 662e  rior_type, self.
+00012450: 7072 696f 725f 7261 6e67 652c 0a20 2020  prior_range,.   
 00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012480: 2020 2020 2073 656c 662e 7363 616c 6573       self.scales
-00012490: 2c20 7365 6c66 2e61 6374 6976 6174 655f  , self.activate_
-000124a0: 7469 6d65 5f73 6361 6c65 5f73 6570 6172  time_scale_separ
-000124b0: 6174 696f 6e5f 7072 696f 722c 0a20 2020  ation_prior,.   
+00012480: 2020 2020 7365 6c66 2e73 6361 6c65 732c      self.scales,
+00012490: 2073 656c 662e 6163 7469 7661 7465 5f74   self.activate_t
+000124a0: 696d 655f 7363 616c 655f 7365 7061 7261  ime_scale_separa
+000124b0: 7469 6f6e 5f70 7269 6f72 2c0a 2020 2020  tion_prior,.    
 000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124e0: 2020 2020 7365 6c66 2e74 696d 655f 7363      self.time_sc
-000124f0: 616c 655f 7365 7061 7261 7469 6f6e 5f66  ale_separation_f
-00012500: 6163 746f 722c 2073 656c 662e 736c 6f77  actor, self.slow
-00012510: 5f70 726f 6365 7373 2c20 7072 696e 745f  _process, print_
-00012520: 7469 6d65 5f73 6361 6c65 5f69 6e66 6f29  time_scale_info)
-00012530: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00012540: 3020 3d20 7365 6c66 2e6d 6178 5f6c 696b  0 = self.max_lik
-00012550: 656c 6968 6f6f 645f 7374 6172 7469 6e67  elihood_starting
-00012560: 5f67 7565 7373 6573 0a20 2020 2020 2020  _guesses.       
-00012570: 2072 6573 203d 206f 7074 696d 697a 652e   res = optimize.
-00012580: 6d69 6e69 6d69 7a65 2873 656c 662e 6e65  minimize(self.ne
-00012590: 675f 6c6f 675f 706f 7374 6572 696f 722c  g_log_posterior,
-000125a0: 2078 303d 7061 7230 2c0a 2020 2020 2020   x0=par0,.      
+000124e0: 2020 2073 656c 662e 7469 6d65 5f73 6361     self.time_sca
+000124f0: 6c65 5f73 6570 6172 6174 696f 6e5f 6661  le_separation_fa
+00012500: 6374 6f72 2c20 7365 6c66 2e73 6c6f 775f  ctor, self.slow_
+00012510: 7072 6f63 6573 732c 2070 7269 6e74 5f74  process, print_t
+00012520: 696d 655f 7363 616c 655f 696e 666f 290a  ime_scale_info).
+00012530: 2020 2020 2020 2020 2020 2020 7061 7230              par0
+00012540: 203d 2073 656c 662e 6d61 785f 6c69 6b65   = self.max_like
+00012550: 6c69 686f 6f64 5f73 7461 7274 696e 675f  lihood_starting_
+00012560: 6775 6573 7365 730a 2020 2020 2020 2020  guesses.        
+00012570: 7265 7320 3d20 6f70 7469 6d69 7a65 2e6d  res = optimize.m
+00012580: 696e 696d 697a 6528 7365 6c66 2e6e 6567  inimize(self.neg
+00012590: 5f6c 6f67 5f70 6f73 7465 7269 6f72 2c20  _log_posterior, 
+000125a0: 7830 3d70 6172 302c 0a20 2020 2020 2020  x0=par0,.       
 000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125c0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-000125d0: 733d 7b27 6d61 7869 7465 7227 3a20 3130  s={'maxiter': 10
-000125e0: 202a 2a20 352c 2027 6469 7370 273a 2046   ** 5, 'disp': F
-000125f0: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+000125c0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+000125d0: 3d7b 276d 6178 6974 6572 273a 2031 3020  ={'maxiter': 10 
+000125e0: 2a2a 2035 2c20 2764 6973 7027 3a20 4661  ** 5, 'disp': Fa
+000125f0: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
 00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 206d 6574 686f 643d 274e         method='N
-00012620: 656c 6465 722d 4d65 6164 2729 0a20 2020  elder-Mead').   
-00012630: 2020 2020 2073 656c 662e 4d41 505f 7468       self.MAP_th
-00012640: 6574 615b 3a2c 2030 5d20 3d20 7265 735b  eta[:, 0] = res[
-00012650: 2778 275d 0a20 2020 2020 2020 2069 6620  'x'].        if 
-00012660: 7072 696e 7462 6f6f 6c3a 0a20 2020 2020  printbool:.     
-00012670: 2020 2020 2020 2070 7269 6e74 2827 4d41         print('MA
-00012680: 5020 7468 6574 613a 2027 2c20 7365 6c66  P theta: ', self
-00012690: 2e4d 4150 5f74 6865 7461 290a 2020 2020  .MAP_theta).    
-000126a0: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
+00012610: 2020 2020 2020 6d65 7468 6f64 3d27 4e65        method='Ne
+00012620: 6c64 6572 2d4d 6561 6427 290a 2020 2020  lder-Mead').    
+00012630: 2020 2020 7365 6c66 2e4d 4150 5f74 6865      self.MAP_the
+00012640: 7461 5b3a 2c20 305d 203d 2072 6573 5b27  ta[:, 0] = res['
+00012650: 7827 5d0a 2020 2020 2020 2020 6966 2070  x'].        if p
+00012660: 7269 6e74 626f 6f6c 3a0a 2020 2020 2020  rintbool:.      
+00012670: 2020 2020 2020 7072 696e 7428 274d 4150        print('MAP
+00012680: 2074 6865 7461 3a20 272c 2073 656c 662e   theta: ', self.
+00012690: 4d41 505f 7468 6574 6129 0a20 2020 2020  MAP_theta).     
+000126a0: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
 000126b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000126c0: 5f5f 5f5f 5f27 290a 2020 2020 2020 2020  _____').        
-000126d0: 2020 2020 7072 696e 7428 2744 6f6e 6521      print('Done!
-000126e0: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
-000126f0: 7269 6e74 2827 5f5f 5f5f 5f5f 5f5f 5f5f  rint('__________
-00012700: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 2729 0a0a  ____________')..
-00012710: 2020 2020 6465 6620 5f63 6f6e 6669 6465      def _confide
-00012720: 6e63 655f 6865 6c70 6572 2873 656c 662c  nce_helper(self,
-00012730: 206d 6170 5f62 7063 695f 6269 7365 6374   map_bpci_bisect
-00012740: 696f 6e2c 2074 6865 7461 5f69 6e64 6578  ion, theta_index
-00012750: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012760: 2020 2020 2020 2048 656c 7065 7220 6675         Helper fu
-00012770: 6e63 7469 6f6e 2074 6f20 6669 6e64 2074  nction to find t
-00012780: 6865 2072 6f6f 7473 2061 7420 7468 6520  he roots at the 
-00012790: 626f 756e 6461 7269 6573 206f 6620 7468  boundaries of th
-000127a0: 6520 3144 2063 6f6e 6669 6465 6e63 6520  e 1D confidence 
-000127b0: 696e 7465 7276 616c 730a 2020 2020 2020  intervals.      
-000127c0: 2020 6f66 2074 6865 2060 6074 6865 7461    of the ``theta
-000127d0: 5f69 6e64 6578 6060 2d74 6820 6060 4d41  _index``-th ``MA
-000127e0: 505f 7468 6574 6160 6020 6573 7469 6d61  P_theta`` estima
-000127f0: 7465 2061 7420 6120 636f 6e66 6964 656e  te at a confiden
-00012800: 6365 206c 6576 656c 2067 6976 656e 2062  ce level given b
-00012810: 7920 7468 650a 2020 2020 2020 2020 6174  y the.        at
-00012820: 7472 6962 7574 6560 605f 7369 676d 6152  tribute``_sigmaR
-00012830: 6174 696f 6060 2e0a 0a20 2020 2020 2020  atio``...       
-00012840: 203a 7061 7261 6d20 6d61 705f 6270 6369   :param map_bpci
-00012850: 5f62 6973 6563 7469 6f6e 3a20 4465 7669  _bisection: Devi
-00012860: 6174 696f 6e20 6f66 2074 6865 2060 6074  ation of the ``t
-00012870: 6865 7461 5f69 6e64 6578 6060 2d74 6820  heta_index``-th 
-00012880: 7061 7261 6d65 7465 7220 7468 6174 2069  parameter that i
-00012890: 7320 7661 7269 6564 2062 790a 2020 2020  s varied by.    
+000126c0: 5f5f 5f5f 2729 0a20 2020 2020 2020 2020  ____').         
+000126d0: 2020 2070 7269 6e74 2827 446f 6e65 2127     print('Done!'
+000126e0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+000126f0: 696e 7428 275f 5f5f 5f5f 5f5f 5f5f 5f5f  int('___________
+00012700: 5f5f 5f5f 5f5f 5f5f 5f5f 5f27 290a 0a20  ___________').. 
+00012710: 2020 2064 6566 205f 636f 6e66 6964 656e     def _confiden
+00012720: 6365 5f68 656c 7065 7228 7365 6c66 2c20  ce_helper(self, 
+00012730: 6d61 705f 6270 6369 5f62 6973 6563 7469  map_bpci_bisecti
+00012740: 6f6e 2c20 7468 6574 615f 696e 6465 7829  on, theta_index)
+00012750: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012760: 2020 2020 2020 4865 6c70 6572 2066 756e        Helper fun
+00012770: 6374 696f 6e20 746f 2066 696e 6420 7468  ction to find th
+00012780: 6520 726f 6f74 7320 6174 2074 6865 2062  e roots at the b
+00012790: 6f75 6e64 6172 6965 7320 6f66 2074 6865  oundaries of the
+000127a0: 2031 4420 636f 6e66 6964 656e 6365 2069   1D confidence i
+000127b0: 6e74 6572 7661 6c73 0a20 2020 2020 2020  ntervals.       
+000127c0: 206f 6620 7468 6520 6060 7468 6574 615f   of the ``theta_
+000127d0: 696e 6465 7860 602d 7468 2060 604d 4150  index``-th ``MAP
+000127e0: 5f74 6865 7461 6060 2065 7374 696d 6174  _theta`` estimat
+000127f0: 6520 6174 2061 2063 6f6e 6669 6465 6e63  e at a confidenc
+00012800: 6520 6c65 7665 6c20 6769 7665 6e20 6279  e level given by
+00012810: 2074 6865 0a20 2020 2020 2020 2061 7474   the.        att
+00012820: 7269 6275 7465 6060 5f73 6967 6d61 5261  ribute``_sigmaRa
+00012830: 7469 6f60 602e 0a0a 2020 2020 2020 2020  tio``...        
+00012840: 3a70 6172 616d 206d 6170 5f62 7063 695f  :param map_bpci_
+00012850: 6269 7365 6374 696f 6e3a 2044 6576 6961  bisection: Devia
+00012860: 7469 6f6e 206f 6620 7468 6520 6060 7468  tion of the ``th
+00012870: 6574 615f 696e 6465 7860 602d 7468 2070  eta_index``-th p
+00012880: 6172 616d 6574 6572 2074 6861 7420 6973  arameter that is
+00012890: 2076 6172 6965 6420 6279 0a20 2020 2020   varied by.     
 000128a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128b0: 2020 2020 7468 6520 6269 7365 6374 696f      the bisectio
-000128c0: 6e20 616c 676f 7269 7468 6d20 696e 206f  n algorithm in o
-000128d0: 7264 6572 2074 6f20 6669 6e64 2074 6865  rder to find the
-000128e0: 2063 6f6e 6669 6465 6e63 6520 626f 756e   confidence boun
-000128f0: 6420 666f 7220 6120 6769 7665 6e0a 2020  d for a given.  
+000128b0: 2020 2074 6865 2062 6973 6563 7469 6f6e     the bisection
+000128c0: 2061 6c67 6f72 6974 686d 2069 6e20 6f72   algorithm in or
+000128d0: 6465 7220 746f 2066 696e 6420 7468 6520  der to find the 
+000128e0: 636f 6e66 6964 656e 6365 2062 6f75 6e64  confidence bound
+000128f0: 2066 6f72 2061 2067 6976 656e 0a20 2020   for a given.   
 00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 2020 2020 636f 6e66 6964 656e 6365        confidence
-00012920: 206c 6576 656c 2e0a 0a20 2020 2020 2020   level...       
-00012930: 203a 7479 7065 206d 6170 5f62 7063 695f   :type map_bpci_
-00012940: 6269 7365 6374 696f 6e3a 2066 6c6f 6174  bisection: float
-00012950: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012960: 7468 6574 615f 696e 6465 783a 2049 6e64  theta_index: Ind
-00012970: 6578 206f 6620 7468 6520 6060 4d41 505f  ex of the ``MAP_
-00012980: 7468 6574 6160 6020 6573 7469 6d61 7465  theta`` estimate
-00012990: 206f 6620 7768 6963 6820 7468 6520 636f   of which the co
-000129a0: 6e66 6964 656e 6365 2062 616e 6420 6973  nfidence band is
-000129b0: 2063 6f6d 7075 7465 642e 0a20 2020 2020   computed..     
-000129c0: 2020 203a 7479 7065 2074 6865 7461 5f69     :type theta_i
-000129d0: 6e64 6578 3a20 696e 740a 2020 2020 2020  ndex: int.      
-000129e0: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
-000129f0: 6576 203d 206e 702e 7a65 726f 7328 7365  ev = np.zeros(se
-00012a00: 6c66 2e6e 6469 6d29 0a20 2020 2020 2020  lf.ndim).       
-00012a10: 2064 6576 5b74 6865 7461 5f69 6e64 6578   dev[theta_index
-00012a20: 5d20 3d20 6d61 705f 6270 6369 5f62 6973  ] = map_bpci_bis
-00012a30: 6563 7469 6f6e 0a20 2020 2020 2020 2072  ection.        r
-00012a40: 6574 7572 6e20 2873 656c 662e 5f6f 7074  eturn (self._opt
-00012a50: 696d 756d 5f73 6f6c 7574 696f 6e0a 2020  imum_solution.  
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00012a70: 7365 6c66 2e6e 6567 5f6c 6f67 5f70 6f73  self.neg_log_pos
-00012a80: 7465 7269 6f72 2873 656c 662e 4d41 505f  terior(self.MAP_
-00012a90: 7468 6574 615b 3a2c 2030 5d20 2b20 6465  theta[:, 0] + de
-00012aa0: 7629 0a20 2020 2020 2020 2020 2020 2020  v).             
-00012ab0: 2020 202d 2028 6e70 2e6c 6f67 2873 656c     - (np.log(sel
-00012ac0: 662e 5f73 6967 6d61 5261 7469 6f29 2929  f._sigmaRatio)))
-00012ad0: 0a0a 0a20 2020 2064 6566 205f 6361 6c63  ...    def _calc
-00012ae0: 5f63 6f6e 6669 6465 6e63 655f 6261 6e64  _confidence_band
-00012af0: 2873 656c 662c 2070 7269 6e74 626f 6f6c  (self, printbool
-00012b00: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012b10: 2020 2020 2020 2048 656c 7065 7220 6675         Helper fu
-00012b20: 6e63 7469 6f6e 2074 6861 7420 6465 7465  nction that dete
-00012b30: 726d 696e 6573 2074 6865 2060 604d 4150  rmines the ``MAP
-00012b40: 5f74 6865 7461 6060 2063 6f6e 6669 6465  _theta`` confide
-00012b50: 6e63 6520 6261 6e64 2066 6f72 2061 2067  nce band for a g
-00012b60: 6976 656e 0a20 2020 2020 2020 2063 6f6e  iven.        con
-00012b70: 6669 6465 6e63 6520 6c65 7665 6c20 7374  fidence level st
-00012b80: 6f72 6564 2069 6e20 7468 6520 6174 7472  ored in the attr
-00012b90: 6962 7574 6520 6060 5f73 6967 6d61 5261  ibute ``_sigmaRa
-00012ba0: 7469 6f60 6020 6279 2062 6973 6563 7469  tio`` by bisecti
-00012bb0: 6f6e 206f 6620 7468 650a 2020 2020 2020  on of the.      
-00012bc0: 2020 6060 5f63 6f6e 6669 6465 6e63 655f    ``_confidence_
-00012bd0: 6865 6c70 6572 282e 2e2e 2960 6020 6d65  helper(...)`` me
-00012be0: 7468 6f64 2e0a 0a20 2020 2020 2020 203a  thod...        :
-00012bf0: 7061 7261 6d20 7072 696e 7462 6f6f 6c3a  param printbool:
-00012c00: 2044 6574 6572 6d69 6e65 7320 7768 6574   Determines whet
-00012c10: 6865 7220 6120 6465 7461 696c 6564 206f  her a detailed o
-00012c20: 7574 7075 7420 6973 2070 7269 6e74 6564  utput is printed
-00012c30: 206f 7220 6e6f 742e 0a20 2020 2020 2020   or not..       
-00012c40: 203a 7479 7065 2070 7269 6e74 626f 6f6c   :type printbool
-00012c50: 3a20 426f 6f6c 6561 6e0a 2020 2020 2020  : Boolean.      
-00012c60: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00012c70: 2070 7269 6e74 626f 6f6c 3a0a 2020 2020   printbool:.    
-00012c80: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
+00012910: 2020 2020 2063 6f6e 6669 6465 6e63 6520       confidence 
+00012920: 6c65 7665 6c2e 0a0a 2020 2020 2020 2020  level...        
+00012930: 3a74 7970 6520 6d61 705f 6270 6369 5f62  :type map_bpci_b
+00012940: 6973 6563 7469 6f6e 3a20 666c 6f61 740a  isection: float.
+00012950: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+00012960: 6865 7461 5f69 6e64 6578 3a20 496e 6465  heta_index: Inde
+00012970: 7820 6f66 2074 6865 2060 604d 4150 5f74  x of the ``MAP_t
+00012980: 6865 7461 6060 2065 7374 696d 6174 6520  heta`` estimate 
+00012990: 6f66 2077 6869 6368 2074 6865 2063 6f6e  of which the con
+000129a0: 6669 6465 6e63 6520 6261 6e64 2069 7320  fidence band is 
+000129b0: 636f 6d70 7574 6564 2e0a 2020 2020 2020  computed..      
+000129c0: 2020 3a74 7970 6520 7468 6574 615f 696e    :type theta_in
+000129d0: 6465 783a 2069 6e74 0a20 2020 2020 2020  dex: int.       
+000129e0: 2022 2222 0a0a 2020 2020 2020 2020 6465   """..        de
+000129f0: 7620 3d20 6e70 2e7a 6572 6f73 2873 656c  v = np.zeros(sel
+00012a00: 662e 6e64 696d 290a 2020 2020 2020 2020  f.ndim).        
+00012a10: 6465 765b 7468 6574 615f 696e 6465 785d  dev[theta_index]
+00012a20: 203d 206d 6170 5f62 7063 695f 6269 7365   = map_bpci_bise
+00012a30: 6374 696f 6e0a 2020 2020 2020 2020 7265  ction.        re
+00012a40: 7475 726e 2028 7365 6c66 2e5f 6f70 7469  turn (self._opti
+00012a50: 6d75 6d5f 736f 6c75 7469 6f6e 0a20 2020  mum_solution.   
+00012a60: 2020 2020 2020 2020 2020 2020 202d 2073               - s
+00012a70: 656c 662e 6e65 675f 6c6f 675f 706f 7374  elf.neg_log_post
+00012a80: 6572 696f 7228 7365 6c66 2e4d 4150 5f74  erior(self.MAP_t
+00012a90: 6865 7461 5b3a 2c20 305d 202b 2064 6576  heta[:, 0] + dev
+00012aa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012ab0: 2020 2d20 286e 702e 6c6f 6728 7365 6c66    - (np.log(self
+00012ac0: 2e5f 7369 676d 6152 6174 696f 2929 290a  ._sigmaRatio))).
+00012ad0: 0a0a 2020 2020 6465 6620 5f63 616c 635f  ..    def _calc_
+00012ae0: 636f 6e66 6964 656e 6365 5f62 616e 6428  confidence_band(
+00012af0: 7365 6c66 2c20 7072 696e 7462 6f6f 6c29  self, printbool)
+00012b00: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012b10: 2020 2020 2020 4865 6c70 6572 2066 756e        Helper fun
+00012b20: 6374 696f 6e20 7468 6174 2064 6574 6572  ction that deter
+00012b30: 6d69 6e65 7320 7468 6520 6060 4d41 505f  mines the ``MAP_
+00012b40: 7468 6574 6160 6020 636f 6e66 6964 656e  theta`` confiden
+00012b50: 6365 2062 616e 6420 666f 7220 6120 6769  ce band for a gi
+00012b60: 7665 6e0a 2020 2020 2020 2020 636f 6e66  ven.        conf
+00012b70: 6964 656e 6365 206c 6576 656c 2073 746f  idence level sto
+00012b80: 7265 6420 696e 2074 6865 2061 7474 7269  red in the attri
+00012b90: 6275 7465 2060 605f 7369 676d 6152 6174  bute ``_sigmaRat
+00012ba0: 696f 6060 2062 7920 6269 7365 6374 696f  io`` by bisectio
+00012bb0: 6e20 6f66 2074 6865 0a20 2020 2020 2020  n of the.       
+00012bc0: 2060 605f 636f 6e66 6964 656e 6365 5f68   ``_confidence_h
+00012bd0: 656c 7065 7228 2e2e 2e29 6060 206d 6574  elper(...)`` met
+00012be0: 686f 642e 0a0a 2020 2020 2020 2020 3a70  hod...        :p
+00012bf0: 6172 616d 2070 7269 6e74 626f 6f6c 3a20  aram printbool: 
+00012c00: 4465 7465 726d 696e 6573 2077 6865 7468  Determines wheth
+00012c10: 6572 2061 2064 6574 6169 6c65 6420 6f75  er a detailed ou
+00012c20: 7470 7574 2069 7320 7072 696e 7465 6420  tput is printed 
+00012c30: 6f72 206e 6f74 2e0a 2020 2020 2020 2020  or not..        
+00012c40: 3a74 7970 6520 7072 696e 7462 6f6f 6c3a  :type printbool:
+00012c50: 2042 6f6f 6c65 616e 0a20 2020 2020 2020   Boolean.       
+00012c60: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00012c70: 7072 696e 7462 6f6f 6c3a 0a20 2020 2020  printbool:.     
+00012c80: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
 00012c90: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00012ca0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00012cb0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00012cc0: 5f5f 5f5f 5f5f 2729 0a20 2020 2020 2020  ______').       
-00012cd0: 2020 2020 2070 7269 6e74 2827 436f 6d70       print('Comp
-00012ce0: 7574 6520 4261 7965 7369 616e 2063 6f6e  ute Bayesian con
-00012cf0: 6669 6465 6e63 6520 6261 6e64 7320 7769  fidence bands wi
-00012d00: 7468 2057 696c 6b73 c2b4 2074 6865 6f72  th Wilks.. theor
-00012d10: 656d 2127 290a 2020 2020 2020 2020 2020  em!').          
-00012d20: 2020 7072 696e 7428 275f 5f5f 5f5f 5f5f    print('_______
+00012cc0: 5f5f 5f5f 5f27 290a 2020 2020 2020 2020  _____').        
+00012cd0: 2020 2020 7072 696e 7428 2743 6f6d 7075      print('Compu
+00012ce0: 7465 2042 6179 6573 6961 6e20 636f 6e66  te Bayesian conf
+00012cf0: 6964 656e 6365 2062 616e 6473 2077 6974  idence bands wit
+00012d00: 6820 5769 6c6b 73c2 b420 7468 656f 7265  h Wilks.. theore
+00012d10: 6d21 2729 0a20 2020 2020 2020 2020 2020  m!').           
+00012d20: 2070 7269 6e74 2827 5f5f 5f5f 5f5f 5f5f   print('________
 00012d30: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00012d40: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00012d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00012d60: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00012d70: 5f6f 7074 696d 756d 5f73 6f6c 7574 696f  _optimum_solutio
-00012d80: 6e20 3d20 7365 6c66 2e6e 6567 5f6c 6f67  n = self.neg_log
-00012d90: 5f70 6f73 7465 7269 6f72 2873 656c 662e  _posterior(self.
-00012da0: 4d41 505f 7468 6574 615b 3a2c 2030 5d29  MAP_theta[:, 0])
-00012db0: 0a20 2020 2020 2020 204d 4150 5f43 4920  .        MAP_CI 
-00012dc0: 3d20 6e70 2e7a 6572 6f73 2828 7365 6c66  = np.zeros((self
-00012dd0: 2e6e 6469 6d2c 2032 2929 0a20 2020 2020  .ndim, 2)).     
-00012de0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00012df0: 6528 7365 6c66 2e6e 6469 6d29 3a0a 2020  e(self.ndim):.  
-00012e00: 2020 2020 2020 2020 2020 6966 2070 7269            if pri
-00012e10: 6e74 626f 6f6c 3a0a 2020 2020 2020 2020  ntbool:.        
-00012e20: 2020 2020 2020 2020 7072 696e 7428 2750          print('P
-00012e30: 6172 616d 6574 6572 2027 202b 2073 7472  arameter ' + str
-00012e40: 2869 202b 2031 2920 2b20 2720 3a20 2720  (i + 1) + ' : ' 
-00012e50: 2b20 7374 7228 7365 6c66 2e4d 4150 5f74  + str(self.MAP_t
-00012e60: 6865 7461 5b69 2c20 305d 2920 2b20 2720  heta[i, 0]) + ' 
-00012e70: 4250 4349 203a 2028 2027 290a 2020 2020  BPCI : ( ').    
-00012e80: 2020 2020 2020 2020 2320 6669 6e64 206c          # find l
-00012e90: 6f77 6572 2062 6f75 6e64 2066 6f72 2062  ower bound for b
-00012ea0: 6973 6563 7469 6f6e 2072 6f6f 7420 6669  isection root fi
-00012eb0: 6e64 696e 6720 616c 676f 7269 7468 6d0a  nding algorithm.
-00012ec0: 2020 2020 2020 2020 2020 2020 6d61 705f              map_
-00012ed0: 6270 6369 5f62 6973 6563 7469 6f6e 203d  bpci_bisection =
-00012ee0: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
-00012ef0: 7768 696c 6520 7365 6c66 2e5f 636f 6e66  while self._conf
-00012f00: 6964 656e 6365 5f68 656c 7065 7228 6d61  idence_helper(ma
-00012f10: 705f 6270 6369 5f62 6973 6563 7469 6f6e  p_bpci_bisection
-00012f20: 2c20 6929 203e 3d20 303a 0a20 2020 2020  , i) >= 0:.     
-00012f30: 2020 2020 2020 2020 2020 206d 6170 5f62             map_b
-00012f40: 7063 695f 6269 7365 6374 696f 6e20 2d3d  pci_bisection -=
-00012f50: 2031 2e0a 2020 2020 2020 2020 2020 2020   1..            
-00012f60: 2320 6220 6920 7320 6520 6320 7420 6920  # b i s e c t i 
-00012f70: 6f20 6e0a 2020 2020 2020 2020 2020 2020  o n.            
-00012f80: 4d41 505f 4349 5b69 2c20 305d 203d 206f  MAP_CI[i, 0] = o
-00012f90: 7074 696d 697a 652e 6269 7365 6374 2866  ptimize.bisect(f
-00012fa0: 3d73 656c 662e 5f63 6f6e 6669 6465 6e63  =self._confidenc
-00012fb0: 655f 6865 6c70 6572 2c20 613d 6d61 705f  e_helper, a=map_
-00012fc0: 6270 6369 5f62 6973 6563 7469 6f6e 2c20  bpci_bisection, 
-00012fd0: 623d 302e 2c0a 2020 2020 2020 2020 2020  b=0.,.          
+00012d50: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f27  _______________'
+00012d60: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00012d70: 6f70 7469 6d75 6d5f 736f 6c75 7469 6f6e  optimum_solution
+00012d80: 203d 2073 656c 662e 6e65 675f 6c6f 675f   = self.neg_log_
+00012d90: 706f 7374 6572 696f 7228 7365 6c66 2e4d  posterior(self.M
+00012da0: 4150 5f74 6865 7461 5b3a 2c20 305d 290a  AP_theta[:, 0]).
+00012db0: 2020 2020 2020 2020 4d41 505f 4349 203d          MAP_CI =
+00012dc0: 206e 702e 7a65 726f 7328 2873 656c 662e   np.zeros((self.
+00012dd0: 6e64 696d 2c20 3229 290a 2020 2020 2020  ndim, 2)).      
+00012de0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00012df0: 2873 656c 662e 6e64 696d 293a 0a20 2020  (self.ndim):.   
+00012e00: 2020 2020 2020 2020 2069 6620 7072 696e           if prin
+00012e10: 7462 6f6f 6c3a 0a20 2020 2020 2020 2020  tbool:.         
+00012e20: 2020 2020 2020 2070 7269 6e74 2827 5061         print('Pa
+00012e30: 7261 6d65 7465 7220 2720 2b20 7374 7228  rameter ' + str(
+00012e40: 6920 2b20 3129 202b 2027 203a 2027 202b  i + 1) + ' : ' +
+00012e50: 2073 7472 2873 656c 662e 4d41 505f 7468   str(self.MAP_th
+00012e60: 6574 615b 692c 2030 5d29 202b 2027 2042  eta[i, 0]) + ' B
+00012e70: 5043 4920 3a20 2820 2729 0a20 2020 2020  PCI : ( ').     
+00012e80: 2020 2020 2020 2023 2066 696e 6420 6c6f         # find lo
+00012e90: 7765 7220 626f 756e 6420 666f 7220 6269  wer bound for bi
+00012ea0: 7365 6374 696f 6e20 726f 6f74 2066 696e  section root fin
+00012eb0: 6469 6e67 2061 6c67 6f72 6974 686d 0a20  ding algorithm. 
+00012ec0: 2020 2020 2020 2020 2020 206d 6170 5f62             map_b
+00012ed0: 7063 695f 6269 7365 6374 696f 6e20 3d20  pci_bisection = 
+00012ee0: 2d31 0a20 2020 2020 2020 2020 2020 2077  -1.            w
+00012ef0: 6869 6c65 2073 656c 662e 5f63 6f6e 6669  hile self._confi
+00012f00: 6465 6e63 655f 6865 6c70 6572 286d 6170  dence_helper(map
+00012f10: 5f62 7063 695f 6269 7365 6374 696f 6e2c  _bpci_bisection,
+00012f20: 2069 2920 3e3d 2030 3a0a 2020 2020 2020   i) >= 0:.      
+00012f30: 2020 2020 2020 2020 2020 6d61 705f 6270            map_bp
+00012f40: 6369 5f62 6973 6563 7469 6f6e 202d 3d20  ci_bisection -= 
+00012f50: 312e 0a20 2020 2020 2020 2020 2020 2023  1..            #
+00012f60: 2062 2069 2073 2065 2063 2074 2069 206f   b i s e c t i o
+00012f70: 206e 0a20 2020 2020 2020 2020 2020 204d   n.            M
+00012f80: 4150 5f43 495b 692c 2030 5d20 3d20 6f70  AP_CI[i, 0] = op
+00012f90: 7469 6d69 7a65 2e62 6973 6563 7428 663d  timize.bisect(f=
+00012fa0: 7365 6c66 2e5f 636f 6e66 6964 656e 6365  self._confidence
+00012fb0: 5f68 656c 7065 722c 2061 3d6d 6170 5f62  _helper, a=map_b
+00012fc0: 7063 695f 6269 7365 6374 696f 6e2c 2062  pci_bisection, b
+00012fd0: 3d30 2e2c 0a20 2020 2020 2020 2020 2020  =0.,.           
 00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013000: 2061 7267 733d 2869 292c 2078 746f 6c3d   args=(i), xtol=
-00013010: 3165 2d33 290a 2020 2020 2020 2020 2020  1e-3).          
-00013020: 2020 2320 6669 6e64 2075 7070 6572 2062    # find upper b
-00013030: 6f75 6e64 2066 6f72 2062 6973 6563 7469  ound for bisecti
-00013040: 6f6e 2072 6f6f 7420 6669 6e64 696e 6720  on root finding 
-00013050: 616c 676f 7269 7468 6d0a 2020 2020 2020  algorithm.      
-00013060: 2020 2020 2020 6d61 705f 6270 6369 5f62        map_bpci_b
-00013070: 6973 6563 7469 6f6e 203d 2031 0a20 2020  isection = 1.   
-00013080: 2020 2020 2020 2020 2077 6869 6c65 2073           while s
-00013090: 656c 662e 5f63 6f6e 6669 6465 6e63 655f  elf._confidence_
-000130a0: 6865 6c70 6572 286d 6170 5f62 7063 695f  helper(map_bpci_
-000130b0: 6269 7365 6374 696f 6e2c 2069 2920 3e20  bisection, i) > 
-000130c0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-000130d0: 2020 206d 6170 5f62 7063 695f 6269 7365     map_bpci_bise
-000130e0: 6374 696f 6e20 2b3d 2031 2e0a 2020 2020  ction += 1..    
-000130f0: 2020 2020 2020 2020 2320 6220 6920 7320          # b i s 
-00013100: 6520 6320 7420 6920 6f20 6e0a 2020 2020  e c t i o n.    
-00013110: 2020 2020 2020 2020 4d41 505f 4349 5b69          MAP_CI[i
-00013120: 2c20 315d 203d 206f 7074 696d 697a 652e  , 1] = optimize.
-00013130: 6269 7365 6374 2866 3d73 656c 662e 5f63  bisect(f=self._c
-00013140: 6f6e 6669 6465 6e63 655f 6865 6c70 6572  onfidence_helper
-00013150: 2c20 613d 302e 2c20 623d 6d61 705f 6270  , a=0., b=map_bp
-00013160: 6369 5f62 6973 6563 7469 6f6e 2c0a 2020  ci_bisection,.  
+00013000: 6172 6773 3d28 6929 2c20 7874 6f6c 3d31  args=(i), xtol=1
+00013010: 652d 3329 0a20 2020 2020 2020 2020 2020  e-3).           
+00013020: 2023 2066 696e 6420 7570 7065 7220 626f   # find upper bo
+00013030: 756e 6420 666f 7220 6269 7365 6374 696f  und for bisectio
+00013040: 6e20 726f 6f74 2066 696e 6469 6e67 2061  n root finding a
+00013050: 6c67 6f72 6974 686d 0a20 2020 2020 2020  lgorithm.       
+00013060: 2020 2020 206d 6170 5f62 7063 695f 6269       map_bpci_bi
+00013070: 7365 6374 696f 6e20 3d20 310a 2020 2020  section = 1.    
+00013080: 2020 2020 2020 2020 7768 696c 6520 7365          while se
+00013090: 6c66 2e5f 636f 6e66 6964 656e 6365 5f68  lf._confidence_h
+000130a0: 656c 7065 7228 6d61 705f 6270 6369 5f62  elper(map_bpci_b
+000130b0: 6973 6563 7469 6f6e 2c20 6929 203e 2030  isection, i) > 0
+000130c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000130d0: 2020 6d61 705f 6270 6369 5f62 6973 6563    map_bpci_bisec
+000130e0: 7469 6f6e 202b 3d20 312e 0a20 2020 2020  tion += 1..     
+000130f0: 2020 2020 2020 2023 2062 2069 2073 2065         # b i s e
+00013100: 2063 2074 2069 206f 206e 0a20 2020 2020   c t i o n.     
+00013110: 2020 2020 2020 204d 4150 5f43 495b 692c         MAP_CI[i,
+00013120: 2031 5d20 3d20 6f70 7469 6d69 7a65 2e62   1] = optimize.b
+00013130: 6973 6563 7428 663d 7365 6c66 2e5f 636f  isect(f=self._co
+00013140: 6e66 6964 656e 6365 5f68 656c 7065 722c  nfidence_helper,
+00013150: 2061 3d30 2e2c 2062 3d6d 6170 5f62 7063   a=0., b=map_bpc
+00013160: 695f 6269 7365 6374 696f 6e2c 0a20 2020  i_bisection,.   
 00013170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2020 2020 2020 2061 7267 733d 2869           args=(i
-000131a0: 292c 2078 746f 6c3d 3165 2d33 290a 2020  ), xtol=1e-3).  
-000131b0: 2020 2020 2020 2020 2020 6966 2070 7269            if pri
-000131c0: 6e74 626f 6f6c 3a0a 2020 2020 2020 2020  ntbool:.        
-000131d0: 2020 2020 2020 2020 7072 696e 7428 7374          print(st
-000131e0: 7228 4d41 505f 4349 5b69 2c20 305d 2920  r(MAP_CI[i, 0]) 
-000131f0: 2b20 272c 2027 202b 2073 7472 284d 4150  + ', ' + str(MAP
-00013200: 5f43 495b 692c 2031 5d29 202b 2027 2927  _CI[i, 1]) + ')'
-00013210: 290a 2020 2020 2020 2020 6966 2070 7269  ).        if pri
-00013220: 6e74 626f 6f6c 3a0a 2020 2020 2020 2020  ntbool:.        
-00013230: 2020 2020 7072 696e 7428 275f 5f5f 5f5f      print('_____
+00013190: 2020 2020 2020 2020 6172 6773 3d28 6929          args=(i)
+000131a0: 2c20 7874 6f6c 3d31 652d 3329 0a20 2020  , xtol=1e-3).   
+000131b0: 2020 2020 2020 2020 2069 6620 7072 696e           if prin
+000131c0: 7462 6f6f 6c3a 0a20 2020 2020 2020 2020  tbool:.         
+000131d0: 2020 2020 2020 2070 7269 6e74 2873 7472         print(str
+000131e0: 284d 4150 5f43 495b 692c 2030 5d29 202b  (MAP_CI[i, 0]) +
+000131f0: 2027 2c20 2720 2b20 7374 7228 4d41 505f   ', ' + str(MAP_
+00013200: 4349 5b69 2c20 315d 2920 2b20 2729 2729  CI[i, 1]) + ')')
+00013210: 0a20 2020 2020 2020 2069 6620 7072 696e  .        if prin
+00013220: 7462 6f6f 6c3a 0a20 2020 2020 2020 2020  tbool:.         
+00013230: 2020 2070 7269 6e74 2827 5f5f 5f5f 5f5f     print('______
 00013240: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00013250: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00013260: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00013270: 5f5f 2729 0a20 2020 2020 2020 2020 2020  __').           
-00013280: 2070 7269 6e74 2827 446f 6e65 2127 290a   print('Done!').
-00013290: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000132a0: 7428 275f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  t('_____________
+00013270: 5f27 290a 2020 2020 2020 2020 2020 2020  _').            
+00013280: 7072 696e 7428 2744 6f6e 6521 2729 0a20  print('Done!'). 
+00013290: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000132a0: 2827 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ('______________
 000132b0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 000132c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000132d0: 5f5f 5f5f 5f5f 5f5f 5f5f 2729 0a20 2020  __________').   
-000132e0: 2020 2020 2072 6574 7572 6e20 4d41 505f       return MAP_
-000132f0: 4349 0a0a 0a20 2020 2064 6566 205f 6465  CI...    def _de
-00013300: 7465 726d 696e 655f 636f 6e66 6964 656e  termine_confiden
-00013310: 6365 5f62 616e 6473 2873 656c 662c 2073  ce_bands(self, s
-00013320: 6967 5261 7469 6f2c 2070 7269 6e74 626f  igRatio, printbo
-00013330: 6f6c 293a 0a20 2020 2020 2020 2022 2222  ol):.        """
-00013340: 0a20 2020 2020 2020 2048 656c 7065 7220  .        Helper 
-00013350: 6675 6e63 7469 6f6e 2074 6861 7420 6973  function that is
-00013360: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-00013370: 7465 2074 6865 2063 6f6e 6669 6465 6e63  te the confidenc
-00013380: 6520 6261 6e64 7320 666f 7220 7570 2074  e bands for up t
-00013390: 6f20 7477 6f20 6469 6666 6572 656e 740a  o two different.
-000133a0: 2020 2020 2020 2020 636f 6e66 6964 656e          confiden
-000133b0: 6365 206c 6576 656c 7320 6561 6368 206f  ce levels each o
-000133c0: 6620 7768 6963 6820 6973 2063 6f6d 7075  f which is compu
-000133d0: 7465 6420 7669 6120 7468 6520 6060 5f63  ted via the ``_c
-000133e0: 616c 635f 636f 6e66 6964 656e 6365 5f62  alc_confidence_b
-000133f0: 616e 6428 2e2e 2e29 6060 206d 6574 686f  and(...)`` metho
-00013400: 642e 0a0a 2020 2020 2020 2020 3a70 6172  d...        :par
-00013410: 616d 2073 6967 5261 7469 6f3a 2043 6f6e  am sigRatio: Con
-00013420: 7461 696e 7320 7468 6520 6669 7273 7420  tains the first 
-00013430: 616e 6420 7365 636f 6e64 2063 6f6e 6669  and second confi
-00013440: 6465 6e63 6520 6c65 7665 6c20 6561 6368  dence level each
-00013450: 206f 6620 7768 6963 6820 6973 2075 7365   of which is use
-00013460: 6420 746f 2064 6574 6572 6d69 6e65 0a20  d to determine. 
+000132d0: 5f5f 5f5f 5f5f 5f5f 5f27 290a 2020 2020  _________').    
+000132e0: 2020 2020 7265 7475 726e 204d 4150 5f43      return MAP_C
+000132f0: 490a 0a0a 2020 2020 6465 6620 5f64 6574  I...    def _det
+00013300: 6572 6d69 6e65 5f63 6f6e 6669 6465 6e63  ermine_confidenc
+00013310: 655f 6261 6e64 7328 7365 6c66 2c20 7369  e_bands(self, si
+00013320: 6752 6174 696f 2c20 7072 696e 7462 6f6f  gRatio, printboo
+00013330: 6c29 3a0a 2020 2020 2020 2020 2222 220a  l):.        """.
+00013340: 2020 2020 2020 2020 4865 6c70 6572 2066          Helper f
+00013350: 756e 6374 696f 6e20 7468 6174 2069 7320  unction that is 
+00013360: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+00013370: 6520 7468 6520 636f 6e66 6964 656e 6365  e the confidence
+00013380: 2062 616e 6473 2066 6f72 2075 7020 746f   bands for up to
+00013390: 2074 776f 2064 6966 6665 7265 6e74 0a20   two different. 
+000133a0: 2020 2020 2020 2063 6f6e 6669 6465 6e63         confidenc
+000133b0: 6520 6c65 7665 6c73 2065 6163 6820 6f66  e levels each of
+000133c0: 2077 6869 6368 2069 7320 636f 6d70 7574   which is comput
+000133d0: 6564 2076 6961 2074 6865 2060 605f 6361  ed via the ``_ca
+000133e0: 6c63 5f63 6f6e 6669 6465 6e63 655f 6261  lc_confidence_ba
+000133f0: 6e64 282e 2e2e 2960 6020 6d65 7468 6f64  nd(...)`` method
+00013400: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00013410: 6d20 7369 6752 6174 696f 3a20 436f 6e74  m sigRatio: Cont
+00013420: 6169 6e73 2074 6865 2066 6972 7374 2061  ains the first a
+00013430: 6e64 2073 6563 6f6e 6420 636f 6e66 6964  nd second confid
+00013440: 656e 6365 206c 6576 656c 2065 6163 6820  ence level each 
+00013450: 6f66 2077 6869 6368 2069 7320 7573 6564  of which is used
+00013460: 2074 6f20 6465 7465 726d 696e 650a 2020   to determine.  
 00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 2020 2020 2074 6865 2063 6f6e 6669         the confi
-00013490: 6465 6e63 6520 6261 6e64 7320 6f66 2074  dence bands of t
-000134a0: 6865 2060 604d 4150 5f74 6865 7461 6060  he ``MAP_theta``
-000134b0: 2065 7374 696d 6174 6573 2e0a 0a20 2020   estimates...   
-000134c0: 2020 2020 203a 7479 7065 2073 6967 5261       :type sigRa
-000134d0: 7469 6f3a 204f 6e65 2d64 696d 656e 7369  tio: One-dimensi
-000134e0: 6f6e 616c 206e 756d 7079 2061 7272 6179  onal numpy array
-000134f0: 206f 6620 666c 6f61 742e 0a0a 2020 2020   of float...    
-00013500: 2020 2020 3a70 6172 616d 2070 7269 6e74      :param print
-00013510: 626f 6f6c 3a20 4465 7465 726d 696e 6573  bool: Determines
-00013520: 2077 6865 7468 6572 2061 2064 6574 6169   whether a detai
-00013530: 6c65 6420 6f75 7470 7574 2069 7320 7072  led output is pr
-00013540: 696e 7465 6420 6f72 206e 6f74 2e0a 2020  inted or not..  
-00013550: 2020 2020 2020 3a74 7970 6520 7072 696e        :type prin
-00013560: 7462 6f6f 6c3a 2042 6f6f 6c65 616e 0a20  tbool: Boolean. 
-00013570: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013580: 2020 2069 6620 7369 6752 6174 696f 2e73     if sigRatio.s
-00013590: 697a 6520 3d3d 2032 3a0a 2020 2020 2020  ize == 2:.      
-000135a0: 2020 2020 2020 7365 6c66 2e4d 4150 5f43        self.MAP_C
-000135b0: 4920 3d20 6e70 2e7a 6572 6f73 2828 7365  I = np.zeros((se
-000135c0: 6c66 2e6e 6469 6d2c 2034 2929 0a20 2020  lf.ndim, 4)).   
-000135d0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
-000135e0: 6967 6d61 5261 7469 6f20 3d20 6e70 2e65  igmaRatio = np.e
-000135f0: 7870 282d 6370 792e 6368 6932 2e70 7066  xp(-cpy.chi2.ppf
-00013600: 2831 2d73 6967 5261 7469 6f5b 305d 2f31  (1-sigRatio[0]/1
-00013610: 3030 2e2c 3129 2f32 2e29 0a20 2020 2020  00.,1)/2.).     
-00013620: 2020 2020 2020 2073 656c 662e 4d41 505f         self.MAP_
-00013630: 4349 5b3a 2c20 303a 325d 203d 2073 656c  CI[:, 0:2] = sel
-00013640: 662e 5f63 616c 635f 636f 6e66 6964 656e  f._calc_confiden
-00013650: 6365 5f62 616e 6428 7072 696e 7462 6f6f  ce_band(printboo
-00013660: 6c3d 7072 696e 7462 6f6f 6c29 0a20 2020  l=printbool).   
-00013670: 2020 2020 2020 2020 2073 656c 662e 4d41           self.MA
-00013680: 505f 7468 6574 615b 3a2c 2031 5d20 3d20  P_theta[:, 1] = 
-00013690: 7365 6c66 2e4d 4150 5f74 6865 7461 5b3a  self.MAP_theta[:
-000136a0: 2c20 305d 202b 2073 656c 662e 4d41 505f  , 0] + self.MAP_
-000136b0: 4349 5b3a 2c20 305d 0a20 2020 2020 2020  CI[:, 0].       
-000136c0: 2020 2020 2073 656c 662e 4d41 505f 7468       self.MAP_th
-000136d0: 6574 615b 3a2c 2032 5d20 3d20 7365 6c66  eta[:, 2] = self
-000136e0: 2e4d 4150 5f74 6865 7461 5b3a 2c20 305d  .MAP_theta[:, 0]
-000136f0: 202b 2073 656c 662e 4d41 505f 4349 5b3a   + self.MAP_CI[:
-00013700: 2c20 315d 0a20 2020 2020 2020 2020 2020  , 1].           
-00013710: 2073 656c 662e 5f73 6967 6d61 5261 7469   self._sigmaRati
-00013720: 6f20 3d20 6e70 2e65 7870 282d 6370 792e  o = np.exp(-cpy.
-00013730: 6368 6932 2e70 7066 2831 2d73 6967 5261  chi2.ppf(1-sigRa
-00013740: 7469 6f5b 315d 2f31 3030 2e2c 3129 2f32  tio[1]/100.,1)/2
-00013750: 2e29 0a20 2020 2020 2020 2020 2020 2073  .).            s
-00013760: 656c 662e 4d41 505f 4349 5b3a 2c20 323a  elf.MAP_CI[:, 2:
-00013770: 345d 203d 2073 656c 662e 5f63 616c 635f  4] = self._calc_
-00013780: 636f 6e66 6964 656e 6365 5f62 616e 6428  confidence_band(
-00013790: 7072 696e 7462 6f6f 6c3d 7072 696e 7462  printbool=printb
-000137a0: 6f6f 6c29 0a20 2020 2020 2020 2020 2020  ool).           
-000137b0: 2073 656c 662e 4d41 505f 7468 6574 615b   self.MAP_theta[
-000137c0: 3a2c 2033 5d20 3d20 7365 6c66 2e4d 4150  :, 3] = self.MAP
-000137d0: 5f74 6865 7461 5b3a 2c20 305d 202b 2073  _theta[:, 0] + s
-000137e0: 656c 662e 4d41 505f 4349 5b3a 2c20 325d  elf.MAP_CI[:, 2]
-000137f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013800: 662e 4d41 505f 7468 6574 615b 3a2c 2034  f.MAP_theta[:, 4
-00013810: 5d20 3d20 7365 6c66 2e4d 4150 5f74 6865  ] = self.MAP_the
-00013820: 7461 5b3a 2c20 305d 202b 2073 656c 662e  ta[:, 0] + self.
-00013830: 4d41 505f 4349 5b3a 2c20 335d 0a20 2020  MAP_CI[:, 3].   
-00013840: 2020 2020 2065 6c69 6620 7369 6752 6174       elif sigRat
-00013850: 696f 2e73 697a 6520 3d3d 2031 3a0a 2020  io.size == 1:.  
-00013860: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
-00013870: 4150 5f43 4920 3d20 6e70 2e7a 6572 6f73  AP_CI = np.zeros
-00013880: 2828 7365 6c66 2e6e 6469 6d2c 2032 2929  ((self.ndim, 2))
-00013890: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000138a0: 662e 5f73 6967 6d61 5261 7469 6f20 3d20  f._sigmaRatio = 
-000138b0: 6e70 2e65 7870 282d 6370 792e 6368 6932  np.exp(-cpy.chi2
-000138c0: 2e70 7066 2831 2d73 6967 5261 7469 6f5b  .ppf(1-sigRatio[
-000138d0: 305d 2f31 3030 2e2c 2031 292f 322e 290a  0]/100., 1)/2.).
-000138e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000138f0: 2e4d 4150 5f43 495b 3a2c 2030 3a32 5d20  .MAP_CI[:, 0:2] 
-00013900: 3d20 7365 6c66 2e5f 6361 6c63 5f63 6f6e  = self._calc_con
-00013910: 6669 6465 6e63 655f 6261 6e64 2870 7269  fidence_band(pri
-00013920: 6e74 626f 6f6c 3d70 7269 6e74 626f 6f6c  ntbool=printbool
-00013930: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00013940: 6c66 2e4d 4150 5f74 6865 7461 5b3a 2c20  lf.MAP_theta[:, 
-00013950: 315d 203d 2073 656c 662e 4d41 505f 7468  1] = self.MAP_th
-00013960: 6574 615b 3a2c 2030 5d20 2b20 7365 6c66  eta[:, 0] + self
-00013970: 2e4d 4150 5f43 495b 3a2c 2030 5d0a 2020  .MAP_CI[:, 0].  
-00013980: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
-00013990: 4150 5f74 6865 7461 5b3a 2c20 325d 203d  AP_theta[:, 2] =
-000139a0: 2073 656c 662e 4d41 505f 7468 6574 615b   self.MAP_theta[
-000139b0: 3a2c 2030 5d20 2b20 7365 6c66 2e4d 4150  :, 0] + self.MAP
-000139c0: 5f43 495b 3a2c 2031 5d0a 2020 2020 2020  _CI[:, 1].      
-000139d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000139e0: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
-000139f0: 3a20 5468 6520 7369 6752 6174 696f 2061  : The sigRatio a
-00013a00: 7267 756d 656e 7420 6e65 6564 7320 6f6e  rgument needs on
-00013a10: 6520 6f72 2074 776f 206e 756d 7079 2061  e or two numpy a
-00013a20: 7272 6179 2065 6e74 7269 6573 2e27 290a  rray entries.').
-00013a30: 2020 2020 2020 2020 7365 6c66 2e6e 6f69          self.noi
-00013a40: 7365 5f6c 6576 656c 5f65 7374 696d 6174  se_level_estimat
-00013a50: 6520 3d20 7365 6c66 2e4d 4150 5f74 6865  e = self.MAP_the
-00013a60: 7461 5b2d 312c 203a 5d0a 0a20 2020 2064  ta[-1, :]..    d
-00013a70: 6566 205f 636f 6d70 7574 655f 736c 6f70  ef _compute_slop
-00013a80: 655f 6572 726f 7273 2873 656c 662c 2070  e_errors(self, p
-00013a90: 7269 6e74 626f 6f6c 293a 0a20 2020 2020  rintbool):.     
-00013aa0: 2020 2022 2222 0a20 2020 2020 2020 2048     """.        H
-00013ab0: 656c 7065 7220 6675 6e63 7469 6f6e 2074  elper function t
-00013ac0: 6861 7420 6465 7465 726d 696e 6573 2074  hat determines t
-00013ad0: 6865 2061 7379 6d6d 6574 7269 6320 6d61  he asymmetric ma
-00013ae0: 7267 696e 616c 2075 6e63 6572 7461 696e  rginal uncertain
-00013af0: 7469 6573 206f 6620 7468 6520 6060 4d41  ties of the ``MA
-00013b00: 505f 7468 6574 6160 6020 7669 6120 5769  P_theta`` via Wi
-00013b10: 6c6b 7327 2074 6865 6f72 656d 2e0a 2020  lks' theorem..  
-00013b20: 2020 2020 2020 5468 6520 6d65 7468 6f64        The method
-00013b30: 2079 6965 6c64 7320 7472 7573 7461 626c   yields trustabl
-00013b40: 6520 636f 6e66 6964 656e 6365 2062 616e  e confidence ban
-00013b50: 6473 2066 6f72 2074 6865 2064 7269 6674  ds for the drift
-00013b60: 2073 6c6f 7065 203a 6d61 7468 3a60 5c68   slope :math:`\h
-00013b70: 6174 7b5c 7a65 7461 7d60 2066 6f72 2074  at{\zeta}` for t
-00013b80: 6865 2066 6972 7374 206f 7264 6572 2070  he first order p
-00013b90: 6f6c 796e 6f6d 6961 6c0a 2020 2020 2020  olynomial.      
-00013ba0: 2020 6f66 2074 6865 204c 616e 6765 7669    of the Langevi
-00013bb0: 6e20 6571 7561 7469 6f6e 2e20 496e 2063  n equation. In c
-00013bc0: 6173 6520 6f66 2074 6865 2074 6869 7264  ase of the third
-00013bd0: 206f 7264 6572 2070 6f6c 796e 6f6d 6961   order polynomia
-00013be0: 6c20 6472 6966 742c 2074 6865 2075 6e63  l drift, the unc
-00013bf0: 6572 7461 696e 7479 206f 6620 7468 6520  ertainty of the 
-00013c00: 6472 6966 7420 6c6f 7065 203a 6d61 7468  drift lope :math
-00013c10: 3a60 5c68 6174 7b5c 7a65 7461 7d60 0a20  :`\hat{\zeta}`. 
-00013c20: 2020 2020 2020 2069 7320 6465 7465 726d         is determ
-00013c30: 696e 6564 2076 6961 2073 696d 706c 6520  ined via simple 
-00013c40: 4761 7573 7369 616e 2070 726f 7061 6761  Gaussian propaga
-00013c50: 7469 6f6e 206f 6620 756e 6365 7274 6169  tion of uncertai
-00013c60: 6e74 6965 732e 2053 6576 6572 616c 2061  nties. Several a
-00013c70: 7373 756d 7074 696f 6e73 206d 616b 6520  ssumptions make 
-00013c80: 7468 6520 636f 6e66 6964 656e 6365 2062  the confidence b
-00013c90: 616e 6473 2074 6f6f 0a20 2020 2020 2020  ands too.       
-00013ca0: 206f 7074 696d 6973 7469 632c 2069 2e65   optimistic, i.e
-00013cb0: 2e20 746f 6f20 6e61 7272 6f77 2e20 5468  . too narrow. Th
-00013cc0: 6520 6d6f 6465 6c20 7061 7261 6d65 7465  e model paramete
-00013cd0: 7273 2061 7265 2061 7373 756d 6564 2074  rs are assumed t
-00013ce0: 6f20 6265 2075 6e63 6f72 7265 6c61 7465  o be uncorrelate
-00013cf0: 6420 616e 6420 4761 7573 7369 616e 2064  d and Gaussian d
-00013d00: 6973 7472 6962 7574 6564 2e20 5468 6520  istributed. The 
-00013d10: 6d6f 6465 6c0a 2020 2020 2020 2020 7361  model.        sa
-00013d20: 6d70 6c65 2073 697a 6520 6f66 2074 6865  mple size of the
-00013d30: 204d 4150 2065 7374 696d 6174 6573 2069   MAP estimates i
-00013d40: 7320 6f6e 652e 2049 6620 7468 6973 2065  s one. If this e
-00013d50: 7272 6f72 2070 726f 7061 6761 7469 6f6e  rror propagation
-00013d60: 206f 7074 696f 6e20 6973 2063 686f 7365   option is chose
-00013d70: 6e20 666f 7220 7468 6520 7468 6972 6420  n for the third 
-00013d80: 6f72 6465 7220 6472 6966 7420 706f 6c79  order drift poly
-00013d90: 6e6f 6d69 616c 2c0a 2020 2020 2020 2020  nomial,.        
-00013da0: 7468 6520 636f 6e66 6964 656e 6365 206c  the confidence l
-00013db0: 6576 656c 7320 6172 6520 6669 7865 6420  evels are fixed 
-00013dc0: 746f 2063 7265 645f 7065 7263 656e 7469  to cred_percenti
-00013dd0: 6c65 7320 3d20 6e75 6d70 792e 6172 7261  les = numpy.arra
-00013de0: 7928 5b35 2c31 5d29 2074 6f20 7472 616e  y([5,1]) to tran
-00013df0: 7366 6f72 6d20 7468 6520 6d61 7267 696e  sform the margin
-00013e00: 616c 2063 6f6e 6669 6465 6e63 6520 6261  al confidence ba
-00013e10: 6e64 730a 2020 2020 2020 2020 6f66 2074  nds.        of t
-00013e20: 6865 2070 6172 616d 6574 6572 7320 696e  he parameters in
-00013e30: 746f 2065 7272 6f72 2076 6961 2066 6978  to error via fix
-00013e40: 6564 2074 7261 6e73 666f 726d 6174 696f  ed transformatio
-00013e50: 6e20 6661 6374 6f72 732c 2069 2e65 2e20  n factors, i.e. 
-00013e60: 312e 3936 2061 6e64 2032 2e35 3532 3520  1.96 and 2.5525 
-00013e70: 666f 7220 6861 6c66 2d73 6964 6564 2069  for half-sided i
-00013e80: 6e74 6572 7661 6c73 2e0a 2020 2020 2020  ntervals..      
-00013e90: 2020 4166 7465 7220 6572 726f 7220 7072    After error pr
-00013ea0: 6f70 6167 6174 696f 6e20 7468 6520 6472  opagation the dr
-00013eb0: 6966 7420 736c 6f70 6520 6572 726f 7220  ift slope error 
-00013ec0: 6973 2074 7261 6e73 666f 726d 6564 2062  is transformed b
-00013ed0: 6163 6b20 7669 6120 7468 6520 7361 6d65  ack via the same
-00013ee0: 2066 6163 746f 7273 2e20 5468 6520 6e6f   factors. The no
-00013ef0: 726d 616c 6c79 2073 6c69 6768 746c 7920  rmally slightly 
-00013f00: 6173 796d 6d65 7472 6963 2065 7272 6f72  asymmetric error
-00013f10: 0a20 2020 2020 2020 2062 6f75 6e64 7320  .        bounds 
-00013f20: 6172 6520 6d61 696e 7461 696e 6564 2061  are maintained a
-00013f30: 6e64 2074 7265 6174 6564 2061 7320 6966  nd treated as if
-00013f40: 2074 6865 7920 776f 756c 6420 6265 2068   they would be h
-00013f50: 616c 6620 636f 6e66 6964 656e 6365 2069  alf confidence i
-00013f60: 6e74 6572 7661 6c73 206f 6620 6120 4761  ntervals of a Ga
-00013f70: 7573 7369 616e 2e20 5468 6973 2066 6f72  ussian. This for
-00013f80: 6d61 6c6c 7920 6e6f 7420 636f 7272 6563  mally not correc
-00013f90: 742c 0a20 2020 2020 2020 2062 7574 206d  t,.        but m
-00013fa0: 6169 6e74 6169 6e73 2074 6865 2069 6e66  aintains the inf
-00013fb0: 6f72 6d61 7469 6f6e 2061 626f 7574 2061  ormation about a
-00013fc0: 7379 6d6d 6574 7279 206f 6620 7468 6520  symmetry of the 
-00013fd0: 6572 726f 7220 6261 6e64 7320 6f66 2074  error bands of t
-00013fe0: 6865 2057 696c 6b73 2720 7468 656f 7265  he Wilks' theore
-00013ff0: 6d20 6170 7072 6f78 696d 6174 696f 6e2e  m approximation.
-00014000: 0a20 2020 2020 2020 204f 6e6c 7920 696e  .        Only in
-00014010: 2074 6865 2072 6172 6520 6361 7365 206f   the rare case o
-00014020: 6620 6869 6768 2061 6d6f 756e 7473 206f  f high amounts o
-00014030: 6620 6461 7461 2070 6572 2077 696e 646f  f data per windo
-00014040: 772c 2074 6865 2063 6f6e 6669 6465 6e63  w, the confidenc
-00014050: 6520 6261 6e64 7320 636f 6d70 7574 6564  e bands computed
-00014060: 2062 7920 7468 6973 2070 726f 6365 6475   by this procedu
-00014070: 7265 206d 6967 6874 2062 650a 2020 2020  re might be.    
-00014080: 2020 2020 7472 7573 7477 6f72 7468 7920      trustworthy 
-00014090: 696e 2074 6865 2063 6173 6520 6f66 2061  in the case of a
-000140a0: 2074 6869 7264 206f 7264 6572 2070 6f6c   third order pol
-000140b0: 796e 6f6d 6961 6c20 6472 6966 7420 7465  ynomial drift te
-000140c0: 726d 2e20 5468 6973 2069 7373 7565 206d  rm. This issue m
-000140d0: 6967 6874 2062 6520 736f 6c76 6162 6c65  ight be solvable
-000140e0: 2062 7920 696e 7472 6f64 7563 696e 6720   by introducing 
-000140f0: 616e 2065 7374 696d 6174 650a 2020 2020  an estimate.    
-00014100: 2020 2020 6f66 2074 6865 2063 6f76 6172      of the covar
-00014110: 6961 6e63 6520 6d61 7472 6978 206f 6620  iance matrix of 
-00014120: 7468 6520 7061 7261 6d65 7465 7273 2069  the parameters i
-00014130: 6e20 6675 7475 7265 2e0a 0a20 2020 2020  n future...     
-00014140: 2020 203a 7061 7261 6d20 7072 696e 7462     :param printb
-00014150: 6f6f 6c3a 2044 6574 6572 6d69 6e65 7320  ool: Determines 
-00014160: 7768 6574 6865 7220 6120 6465 7461 696c  whether a detail
-00014170: 6564 206f 7574 7075 7420 6973 2070 7269  ed output is pri
-00014180: 6e74 6564 206f 7220 6e6f 742e 0a20 2020  nted or not..   
-00014190: 2020 2020 203a 7479 7065 2070 7269 6e74       :type print
-000141a0: 626f 6f6c 3a20 426f 6f6c 6561 6e0a 2020  bool: Boolean.  
-000141b0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000141c0: 2020 2069 6620 7072 696e 7462 6f6f 6c3a     if printbool:
-000141d0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000141e0: 6e74 2827 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  nt('____________
+00013480: 2020 2020 2020 7468 6520 636f 6e66 6964        the confid
+00013490: 656e 6365 2062 616e 6473 206f 6620 7468  ence bands of th
+000134a0: 6520 6060 4d41 505f 7468 6574 6160 6020  e ``MAP_theta`` 
+000134b0: 6573 7469 6d61 7465 732e 0a0a 2020 2020  estimates...    
+000134c0: 2020 2020 3a74 7970 6520 7369 6752 6174      :type sigRat
+000134d0: 696f 3a20 4f6e 652d 6469 6d65 6e73 696f  io: One-dimensio
+000134e0: 6e61 6c20 6e75 6d70 7920 6172 7261 7920  nal numpy array 
+000134f0: 6f66 2066 6c6f 6174 2e0a 0a20 2020 2020  of float...     
+00013500: 2020 203a 7061 7261 6d20 7072 696e 7462     :param printb
+00013510: 6f6f 6c3a 2044 6574 6572 6d69 6e65 7320  ool: Determines 
+00013520: 7768 6574 6865 7220 6120 6465 7461 696c  whether a detail
+00013530: 6564 206f 7574 7075 7420 6973 2070 7269  ed output is pri
+00013540: 6e74 6564 206f 7220 6e6f 742e 0a20 2020  nted or not..   
+00013550: 2020 2020 203a 7479 7065 2070 7269 6e74       :type print
+00013560: 626f 6f6c 3a20 426f 6f6c 6561 6e0a 2020  bool: Boolean.  
+00013570: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013580: 2020 6966 2073 6967 5261 7469 6f2e 7369    if sigRatio.si
+00013590: 7a65 203d 3d20 323a 0a20 2020 2020 2020  ze == 2:.       
+000135a0: 2020 2020 2073 656c 662e 4d41 505f 4349       self.MAP_CI
+000135b0: 203d 206e 702e 7a65 726f 7328 2873 656c   = np.zeros((sel
+000135c0: 662e 6e64 696d 2c20 3429 290a 2020 2020  f.ndim, 4)).    
+000135d0: 2020 2020 2020 2020 7365 6c66 2e5f 7369          self._si
+000135e0: 676d 6152 6174 696f 203d 206e 702e 6578  gmaRatio = np.ex
+000135f0: 7028 2d63 7079 2e63 6869 322e 7070 6628  p(-cpy.chi2.ppf(
+00013600: 312d 7369 6752 6174 696f 5b30 5d2f 3130  1-sigRatio[0]/10
+00013610: 302e 2c31 292f 322e 290a 2020 2020 2020  0.,1)/2.).      
+00013620: 2020 2020 2020 7365 6c66 2e4d 4150 5f43        self.MAP_C
+00013630: 495b 3a2c 2030 3a32 5d20 3d20 7365 6c66  I[:, 0:2] = self
+00013640: 2e5f 6361 6c63 5f63 6f6e 6669 6465 6e63  ._calc_confidenc
+00013650: 655f 6261 6e64 2870 7269 6e74 626f 6f6c  e_band(printbool
+00013660: 3d70 7269 6e74 626f 6f6c 290a 2020 2020  =printbool).    
+00013670: 2020 2020 2020 2020 7365 6c66 2e4d 4150          self.MAP
+00013680: 5f74 6865 7461 5b3a 2c20 315d 203d 2073  _theta[:, 1] = s
+00013690: 656c 662e 4d41 505f 7468 6574 615b 3a2c  elf.MAP_theta[:,
+000136a0: 2030 5d20 2b20 7365 6c66 2e4d 4150 5f43   0] + self.MAP_C
+000136b0: 495b 3a2c 2030 5d0a 2020 2020 2020 2020  I[:, 0].        
+000136c0: 2020 2020 7365 6c66 2e4d 4150 5f74 6865      self.MAP_the
+000136d0: 7461 5b3a 2c20 325d 203d 2073 656c 662e  ta[:, 2] = self.
+000136e0: 4d41 505f 7468 6574 615b 3a2c 2030 5d20  MAP_theta[:, 0] 
+000136f0: 2b20 7365 6c66 2e4d 4150 5f43 495b 3a2c  + self.MAP_CI[:,
+00013700: 2031 5d0a 2020 2020 2020 2020 2020 2020   1].            
+00013710: 7365 6c66 2e5f 7369 676d 6152 6174 696f  self._sigmaRatio
+00013720: 203d 206e 702e 6578 7028 2d63 7079 2e63   = np.exp(-cpy.c
+00013730: 6869 322e 7070 6628 312d 7369 6752 6174  hi2.ppf(1-sigRat
+00013740: 696f 5b31 5d2f 3130 302e 2c31 292f 322e  io[1]/100.,1)/2.
+00013750: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00013760: 6c66 2e4d 4150 5f43 495b 3a2c 2032 3a34  lf.MAP_CI[:, 2:4
+00013770: 5d20 3d20 7365 6c66 2e5f 6361 6c63 5f63  ] = self._calc_c
+00013780: 6f6e 6669 6465 6e63 655f 6261 6e64 2870  onfidence_band(p
+00013790: 7269 6e74 626f 6f6c 3d70 7269 6e74 626f  rintbool=printbo
+000137a0: 6f6c 290a 2020 2020 2020 2020 2020 2020  ol).            
+000137b0: 7365 6c66 2e4d 4150 5f74 6865 7461 5b3a  self.MAP_theta[:
+000137c0: 2c20 335d 203d 2073 656c 662e 4d41 505f  , 3] = self.MAP_
+000137d0: 7468 6574 615b 3a2c 2030 5d20 2b20 7365  theta[:, 0] + se
+000137e0: 6c66 2e4d 4150 5f43 495b 3a2c 2032 5d0a  lf.MAP_CI[:, 2].
+000137f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013800: 2e4d 4150 5f74 6865 7461 5b3a 2c20 345d  .MAP_theta[:, 4]
+00013810: 203d 2073 656c 662e 4d41 505f 7468 6574   = self.MAP_thet
+00013820: 615b 3a2c 2030 5d20 2b20 7365 6c66 2e4d  a[:, 0] + self.M
+00013830: 4150 5f43 495b 3a2c 2033 5d0a 2020 2020  AP_CI[:, 3].    
+00013840: 2020 2020 656c 6966 2073 6967 5261 7469      elif sigRati
+00013850: 6f2e 7369 7a65 203d 3d20 313a 0a20 2020  o.size == 1:.   
+00013860: 2020 2020 2020 2020 2073 656c 662e 4d41           self.MA
+00013870: 505f 4349 203d 206e 702e 7a65 726f 7328  P_CI = np.zeros(
+00013880: 2873 656c 662e 6e64 696d 2c20 3229 290a  (self.ndim, 2)).
+00013890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000138a0: 2e5f 7369 676d 6152 6174 696f 203d 206e  ._sigmaRatio = n
+000138b0: 702e 6578 7028 2d63 7079 2e63 6869 322e  p.exp(-cpy.chi2.
+000138c0: 7070 6628 312d 7369 6752 6174 696f 5b30  ppf(1-sigRatio[0
+000138d0: 5d2f 3130 302e 2c20 3129 2f32 2e29 0a20  ]/100., 1)/2.). 
+000138e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000138f0: 4d41 505f 4349 5b3a 2c20 303a 325d 203d  MAP_CI[:, 0:2] =
+00013900: 2073 656c 662e 5f63 616c 635f 636f 6e66   self._calc_conf
+00013910: 6964 656e 6365 5f62 616e 6428 7072 696e  idence_band(prin
+00013920: 7462 6f6f 6c3d 7072 696e 7462 6f6f 6c29  tbool=printbool)
+00013930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013940: 662e 4d41 505f 7468 6574 615b 3a2c 2031  f.MAP_theta[:, 1
+00013950: 5d20 3d20 7365 6c66 2e4d 4150 5f74 6865  ] = self.MAP_the
+00013960: 7461 5b3a 2c20 305d 202b 2073 656c 662e  ta[:, 0] + self.
+00013970: 4d41 505f 4349 5b3a 2c20 305d 0a20 2020  MAP_CI[:, 0].   
+00013980: 2020 2020 2020 2020 2073 656c 662e 4d41           self.MA
+00013990: 505f 7468 6574 615b 3a2c 2032 5d20 3d20  P_theta[:, 2] = 
+000139a0: 7365 6c66 2e4d 4150 5f74 6865 7461 5b3a  self.MAP_theta[:
+000139b0: 2c20 305d 202b 2073 656c 662e 4d41 505f  , 0] + self.MAP_
+000139c0: 4349 5b3a 2c20 315d 0a20 2020 2020 2020  CI[:, 1].       
+000139d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000139e0: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
+000139f0: 2054 6865 2073 6967 5261 7469 6f20 6172   The sigRatio ar
+00013a00: 6775 6d65 6e74 206e 6565 6473 206f 6e65  gument needs one
+00013a10: 206f 7220 7477 6f20 6e75 6d70 7920 6172   or two numpy ar
+00013a20: 7261 7920 656e 7472 6965 732e 2729 0a20  ray entries.'). 
+00013a30: 2020 2020 2020 2073 656c 662e 6e6f 6973         self.nois
+00013a40: 655f 6c65 7665 6c5f 6573 7469 6d61 7465  e_level_estimate
+00013a50: 203d 2073 656c 662e 4d41 505f 7468 6574   = self.MAP_thet
+00013a60: 615b 2d31 2c20 3a5d 0a0a 2020 2020 6465  a[-1, :]..    de
+00013a70: 6620 5f63 6f6d 7075 7465 5f73 6c6f 7065  f _compute_slope
+00013a80: 5f65 7272 6f72 7328 7365 6c66 2c20 7072  _errors(self, pr
+00013a90: 696e 7462 6f6f 6c29 3a0a 2020 2020 2020  intbool):.      
+00013aa0: 2020 2222 220a 2020 2020 2020 2020 4865    """.        He
+00013ab0: 6c70 6572 2066 756e 6374 696f 6e20 7468  lper function th
+00013ac0: 6174 2064 6574 6572 6d69 6e65 7320 7468  at determines th
+00013ad0: 6520 6173 796d 6d65 7472 6963 206d 6172  e asymmetric mar
+00013ae0: 6769 6e61 6c20 756e 6365 7274 6169 6e74  ginal uncertaint
+00013af0: 6965 7320 6f66 2074 6865 2060 604d 4150  ies of the ``MAP
+00013b00: 5f74 6865 7461 6060 2076 6961 2057 696c  _theta`` via Wil
+00013b10: 6b73 2720 7468 656f 7265 6d2e 0a20 2020  ks' theorem..   
+00013b20: 2020 2020 2054 6865 206d 6574 686f 6420       The method 
+00013b30: 7969 656c 6473 2074 7275 7374 6162 6c65  yields trustable
+00013b40: 2063 6f6e 6669 6465 6e63 6520 6261 6e64   confidence band
+00013b50: 7320 666f 7220 7468 6520 6472 6966 7420  s for the drift 
+00013b60: 736c 6f70 6520 3a6d 6174 683a 605c 6861  slope :math:`\ha
+00013b70: 747b 5c7a 6574 617d 6020 666f 7220 7468  t{\zeta}` for th
+00013b80: 6520 6669 7273 7420 6f72 6465 7220 706f  e first order po
+00013b90: 6c79 6e6f 6d69 616c 0a20 2020 2020 2020  lynomial.       
+00013ba0: 206f 6620 7468 6520 4c61 6e67 6576 696e   of the Langevin
+00013bb0: 2065 7175 6174 696f 6e2e 2049 6e20 6361   equation. In ca
+00013bc0: 7365 206f 6620 7468 6520 7468 6972 6420  se of the third 
+00013bd0: 6f72 6465 7220 706f 6c79 6e6f 6d69 616c  order polynomial
+00013be0: 2064 7269 6674 2c20 7468 6520 756e 6365   drift, the unce
+00013bf0: 7274 6169 6e74 7920 6f66 2074 6865 2064  rtainty of the d
+00013c00: 7269 6674 206c 6f70 6520 3a6d 6174 683a  rift lope :math:
+00013c10: 605c 6861 747b 5c7a 6574 617d 600a 2020  `\hat{\zeta}`.  
+00013c20: 2020 2020 2020 6973 2064 6574 6572 6d69        is determi
+00013c30: 6e65 6420 7669 6120 7369 6d70 6c65 2047  ned via simple G
+00013c40: 6175 7373 6961 6e20 7072 6f70 6167 6174  aussian propagat
+00013c50: 696f 6e20 6f66 2075 6e63 6572 7461 696e  ion of uncertain
+00013c60: 7469 6573 2e20 5365 7665 7261 6c20 6173  ties. Several as
+00013c70: 7375 6d70 7469 6f6e 7320 6d61 6b65 2074  sumptions make t
+00013c80: 6865 2063 6f6e 6669 6465 6e63 6520 6261  he confidence ba
+00013c90: 6e64 7320 746f 6f0a 2020 2020 2020 2020  nds too.        
+00013ca0: 6f70 7469 6d69 7374 6963 2c20 692e 652e  optimistic, i.e.
+00013cb0: 2074 6f6f 206e 6172 726f 772e 2054 6865   too narrow. The
+00013cc0: 206d 6f64 656c 2070 6172 616d 6574 6572   model parameter
+00013cd0: 7320 6172 6520 6173 7375 6d65 6420 746f  s are assumed to
+00013ce0: 2062 6520 756e 636f 7272 656c 6174 6564   be uncorrelated
+00013cf0: 2061 6e64 2047 6175 7373 6961 6e20 6469   and Gaussian di
+00013d00: 7374 7269 6275 7465 642e 2054 6865 206d  stributed. The m
+00013d10: 6f64 656c 0a20 2020 2020 2020 2073 616d  odel.        sam
+00013d20: 706c 6520 7369 7a65 206f 6620 7468 6520  ple size of the 
+00013d30: 4d41 5020 6573 7469 6d61 7465 7320 6973  MAP estimates is
+00013d40: 206f 6e65 2e20 4966 2074 6869 7320 6572   one. If this er
+00013d50: 726f 7220 7072 6f70 6167 6174 696f 6e20  ror propagation 
+00013d60: 6f70 7469 6f6e 2069 7320 6368 6f73 656e  option is chosen
+00013d70: 2066 6f72 2074 6865 2074 6869 7264 206f   for the third o
+00013d80: 7264 6572 2064 7269 6674 2070 6f6c 796e  rder drift polyn
+00013d90: 6f6d 6961 6c2c 0a20 2020 2020 2020 2074  omial,.        t
+00013da0: 6865 2063 6f6e 6669 6465 6e63 6520 6c65  he confidence le
+00013db0: 7665 6c73 2061 7265 2066 6978 6564 2074  vels are fixed t
+00013dc0: 6f20 6372 6564 5f70 6572 6365 6e74 696c  o cred_percentil
+00013dd0: 6573 203d 206e 756d 7079 2e61 7272 6179  es = numpy.array
+00013de0: 285b 352c 315d 2920 746f 2074 7261 6e73  ([5,1]) to trans
+00013df0: 666f 726d 2074 6865 206d 6172 6769 6e61  form the margina
+00013e00: 6c20 636f 6e66 6964 656e 6365 2062 616e  l confidence ban
+00013e10: 6473 0a20 2020 2020 2020 206f 6620 7468  ds.        of th
+00013e20: 6520 7061 7261 6d65 7465 7273 2069 6e74  e parameters int
+00013e30: 6f20 6572 726f 7220 7669 6120 6669 7865  o error via fixe
+00013e40: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
+00013e50: 2066 6163 746f 7273 2c20 692e 652e 2031   factors, i.e. 1
+00013e60: 2e39 3620 616e 6420 322e 3537 3520 666f  .96 and 2.575 fo
+00013e70: 7220 6861 6c66 2d73 6964 6564 2069 6e74  r half-sided int
+00013e80: 6572 7661 6c73 2e0a 2020 2020 2020 2020  ervals..        
+00013e90: 4166 7465 7220 6572 726f 7220 7072 6f70  After error prop
+00013ea0: 6167 6174 696f 6e20 7468 6520 6472 6966  agation the drif
+00013eb0: 7420 736c 6f70 6520 6572 726f 7220 6973  t slope error is
+00013ec0: 2074 7261 6e73 666f 726d 6564 2062 6163   transformed bac
+00013ed0: 6b20 7669 6120 7468 6520 7361 6d65 2066  k via the same f
+00013ee0: 6163 746f 7273 2e20 5468 6520 6e6f 726d  actors. The norm
+00013ef0: 616c 6c79 2073 6c69 6768 746c 7920 6173  ally slightly as
+00013f00: 796d 6d65 7472 6963 2065 7272 6f72 0a20  ymmetric error. 
+00013f10: 2020 2020 2020 2062 6f75 6e64 7320 6172         bounds ar
+00013f20: 6520 6d61 696e 7461 696e 6564 2061 6e64  e maintained and
+00013f30: 2074 7265 6174 6564 2061 7320 6966 2074   treated as if t
+00013f40: 6865 7920 776f 756c 6420 6265 2068 616c  hey would be hal
+00013f50: 6620 636f 6e66 6964 656e 6365 2069 6e74  f confidence int
+00013f60: 6572 7661 6c73 206f 6620 6120 4761 7573  ervals of a Gaus
+00013f70: 7369 616e 2e20 5468 6973 2066 6f72 6d61  sian. This forma
+00013f80: 6c6c 7920 6e6f 7420 636f 7272 6563 742c  lly not correct,
+00013f90: 0a20 2020 2020 2020 2062 7574 206d 6169  .        but mai
+00013fa0: 6e74 6169 6e73 2074 6865 2069 6e66 6f72  ntains the infor
+00013fb0: 6d61 7469 6f6e 2061 626f 7574 2061 7379  mation about asy
+00013fc0: 6d6d 6574 7279 206f 6620 7468 6520 6572  mmetry of the er
+00013fd0: 726f 7220 6261 6e64 7320 6f66 2074 6865  ror bands of the
+00013fe0: 2057 696c 6b73 2720 7468 656f 7265 6d20   Wilks' theorem 
+00013ff0: 6170 7072 6f78 696d 6174 696f 6e2e 0a20  approximation.. 
+00014000: 2020 2020 2020 204f 6e6c 7920 696e 2074         Only in t
+00014010: 6865 2072 6172 6520 6361 7365 206f 6620  he rare case of 
+00014020: 6869 6768 2061 6d6f 756e 7473 206f 6620  high amounts of 
+00014030: 6461 7461 2070 6572 2077 696e 646f 772c  data per window,
+00014040: 2074 6865 2063 6f6e 6669 6465 6e63 6520   the confidence 
+00014050: 6261 6e64 7320 636f 6d70 7574 6564 2062  bands computed b
+00014060: 7920 7468 6973 2070 726f 6365 6475 7265  y this procedure
+00014070: 206d 6967 6874 2062 650a 2020 2020 2020   might be.      
+00014080: 2020 7472 7573 7477 6f72 7468 7920 696e    trustworthy in
+00014090: 2074 6865 2063 6173 6520 6f66 2061 2074   the case of a t
+000140a0: 6869 7264 206f 7264 6572 2070 6f6c 796e  hird order polyn
+000140b0: 6f6d 6961 6c20 6472 6966 7420 7465 726d  omial drift term
+000140c0: 2e20 5468 6973 2069 7373 7565 206d 6967  . This issue mig
+000140d0: 6874 2062 6520 736f 6c76 6162 6c65 2062  ht be solvable b
+000140e0: 7920 696e 7472 6f64 7563 696e 6720 616e  y introducing an
+000140f0: 2065 7374 696d 6174 650a 2020 2020 2020   estimate.      
+00014100: 2020 6f66 2074 6865 2063 6f76 6172 6961    of the covaria
+00014110: 6e63 6520 6d61 7472 6978 206f 6620 7468  nce matrix of th
+00014120: 6520 7061 7261 6d65 7465 7273 2069 6e20  e parameters in 
+00014130: 6675 7475 7265 2e0a 0a20 2020 2020 2020  future...       
+00014140: 203a 7061 7261 6d20 7072 696e 7462 6f6f   :param printboo
+00014150: 6c3a 2044 6574 6572 6d69 6e65 7320 7768  l: Determines wh
+00014160: 6574 6865 7220 6120 6465 7461 696c 6564  ether a detailed
+00014170: 206f 7574 7075 7420 6973 2070 7269 6e74   output is print
+00014180: 6564 206f 7220 6e6f 742e 0a20 2020 2020  ed or not..     
+00014190: 2020 203a 7479 7065 2070 7269 6e74 626f     :type printbo
+000141a0: 6f6c 3a20 426f 6f6c 6561 6e0a 2020 2020  ol: Boolean.    
+000141b0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000141c0: 2069 6620 7072 696e 7462 6f6f 6c3a 0a20   if printbool:. 
+000141d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000141e0: 2827 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ('______________
 000141f0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00014200: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00014210: 5f5f 2729 0a20 2020 2020 2020 2020 2020  __').           
-00014220: 2070 7269 6e74 2827 436f 6d70 7574 6520   print('Compute 
-00014230: 6173 796d 6d65 7472 6963 2073 6c6f 7065  asymmetric slope
-00014240: 2063 6f6e 6669 6465 6e63 6520 696e 7465   confidence inte
-00014250: 7276 616c 732e 2729 0a20 2020 2020 2020  rvals.').       
-00014260: 2020 2020 2070 7269 6e74 2827 5f5f 5f5f       print('____
+00014210: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
+00014220: 7269 6e74 2827 436f 6d70 7574 6520 6173  rint('Compute as
+00014230: 796d 6d65 7472 6963 2073 6c6f 7065 2063  ymmetric slope c
+00014240: 6f6e 6669 6465 6e63 6520 696e 7465 7276  onfidence interv
+00014250: 616c 732e 2729 0a20 2020 2020 2020 2020  als.').         
+00014260: 2020 2070 7269 6e74 2827 5f5f 5f5f 5f5f     print('______
 00014270: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
 00014280: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00014290: 5f5f 5f5f 5f5f 5f5f 5f5f 2729 0a20 2020  __________').   
-000142a0: 2020 2020 2073 656c 662e 4d41 505f 736c       self.MAP_sl
-000142b0: 6f70 655f 6572 726f 7273 203d 206e 702e  ope_errors = np.
-000142c0: 7a65 726f 7328 3429 0a20 2020 2020 2020  zeros(4).       
-000142d0: 2074 6865 7461 5f65 7272 6f72 5f73 6967   theta_error_sig
-000142e0: 4c65 7665 6c31 203d 206e 702e 7a65 726f  Level1 = np.zero
-000142f0: 7328 2873 656c 662e 6e64 696d 2c20 3229  s((self.ndim, 2)
-00014300: 290a 2020 2020 2020 2020 7468 6574 615f  ).        theta_
-00014310: 6572 726f 725f 7369 674c 6576 656c 3220  error_sigLevel2 
-00014320: 3d20 6e70 2e7a 6572 6f73 2828 7365 6c66  = np.zeros((self
-00014330: 2e6e 6469 6d2c 2032 2929 0a20 2020 2020  .ndim, 2)).     
-00014340: 2020 2074 6865 7461 5f65 7272 6f72 5f73     theta_error_s
-00014350: 6967 4c65 7665 6c31 5b3a 2c20 305d 203d  igLevel1[:, 0] =
-00014360: 2073 656c 662e 4d41 505f 4349 5b3a 2c20   self.MAP_CI[:, 
-00014370: 305d 0a20 2020 2020 2020 2074 6865 7461  0].        theta
-00014380: 5f65 7272 6f72 5f73 6967 4c65 7665 6c31  _error_sigLevel1
-00014390: 5b3a 2c20 315d 203d 2073 656c 662e 4d41  [:, 1] = self.MA
-000143a0: 505f 4349 5b3a 2c20 315d 0a20 2020 2020  P_CI[:, 1].     
-000143b0: 2020 2074 6865 7461 5f65 7272 6f72 5f73     theta_error_s
-000143c0: 6967 4c65 7665 6c31 5b3a 2c20 305d 203d  igLevel1[:, 0] =
-000143d0: 2073 656c 662e 4d41 505f 4349 5b3a 2c20   self.MAP_CI[:, 
-000143e0: 305d 0a20 2020 2020 2020 2074 6865 7461  0].        theta
-000143f0: 5f65 7272 6f72 5f73 6967 4c65 7665 6c31  _error_sigLevel1
-00014400: 5b3a 2c20 315d 203d 2073 656c 662e 4d41  [:, 1] = self.MA
-00014410: 505f 4349 5b3a 2c20 315d 0a0a 2020 2020  P_CI[:, 1]..    
-00014420: 2020 2020 7468 6574 615f 6572 726f 725f      theta_error_
-00014430: 7369 674c 6576 656c 325b 3a2c 2030 5d20  sigLevel2[:, 0] 
-00014440: 3d20 7365 6c66 2e4d 4150 5f43 495b 3a2c  = self.MAP_CI[:,
-00014450: 2032 5d0a 2020 2020 2020 2020 7468 6574   2].        thet
-00014460: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
-00014470: 325b 3a2c 2031 5d20 3d20 7365 6c66 2e4d  2[:, 1] = self.M
-00014480: 4150 5f43 495b 3a2c 2033 5d0a 2020 2020  AP_CI[:, 3].    
-00014490: 2020 2020 7468 6574 615f 6572 726f 725f      theta_error_
-000144a0: 7369 674c 6576 656c 325b 3a2c 2030 5d20  sigLevel2[:, 0] 
-000144b0: 3d20 7365 6c66 2e4d 4150 5f43 495b 3a2c  = self.MAP_CI[:,
-000144c0: 2032 5d2f 322e 3535 3235 0a20 2020 2020   2]/2.5525.     
-000144d0: 2020 2074 6865 7461 5f65 7272 6f72 5f73     theta_error_s
-000144e0: 6967 4c65 7665 6c32 5b3a 2c20 315d 203d  igLevel2[:, 1] =
-000144f0: 2073 656c 662e 4d41 505f 4349 5b3a 2c20   self.MAP_CI[:, 
-00014500: 335d 2f32 2e35 3532 350a 0a20 2020 2020  3]/2.5525..     
-00014510: 2020 2023 2063 6f6d 7075 7465 2077 6f72     # compute wor
-00014520: 7374 2063 6173 6520 6c6f 7765 7220 626f  st case lower bo
-00014530: 756e 640a 2020 2020 2020 2020 6966 2073  und.        if s
-00014540: 656c 662e 6472 6966 745f 6d6f 6465 6c20  elf.drift_model 
-00014550: 3d3d 2027 3372 6420 6f72 6465 7220 706f  == '3rd order po
-00014560: 6c79 6e6f 6d69 616c 273a 0a20 2020 2020  lynomial':.     
-00014570: 2020 2020 2020 2064 6174 615f 7769 6e64         data_wind
-00014580: 6f77 5f65 7272 6f72 203d 206e 702e 7371  ow_error = np.sq
-00014590: 7274 2831 2e2f 2873 656c 662e 6461 7461  rt(1./(self.data
-000145a0: 5f77 696e 646f 772e 7369 7a65 2920 2a20  _window.size) * 
-000145b0: 6e70 2e76 6172 2873 656c 662e 6461 7461  np.var(self.data
-000145c0: 5f77 696e 646f 7729 290a 2020 2020 2020  _window)).      
-000145d0: 2020 2020 2020 585f 6572 726f 7220 3d20        X_error = 
-000145e0: 2832 202a 2073 656c 662e 4d41 505f 7468  (2 * self.MAP_th
-000145f0: 6574 615b 322c 2030 5d20 2b20 3620 2a20  eta[2, 0] + 6 * 
-00014600: 7365 6c66 2e66 6978 6564 5f70 6f69 6e74  self.fixed_point
-00014610: 5f65 7374 696d 6174 6520 2a0a 2020 2020  _estimate *.    
-00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2073 656c 662e 4d41 505f 7468 6574     self.MAP_thet
-00014640: 615b 332c 2030 5d29 202a 2064 6174 615f  a[3, 0]) * data_
-00014650: 7769 6e64 6f77 5f65 7272 6f72 0a20 2020  window_error.   
-00014660: 2020 2020 2020 2020 2070 6172 616d 315f           param1_
-00014670: 6572 726f 7220 3d20 3120 2a20 7468 6574  error = 1 * thet
-00014680: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
-00014690: 315b 312c 2030 5d0a 2020 2020 2020 2020  1[1, 0].        
-000146a0: 2020 2020 7061 7261 6d32 5f65 7272 6f72      param2_error
-000146b0: 203d 2032 202a 2073 656c 662e 6669 7865   = 2 * self.fixe
-000146c0: 645f 706f 696e 745f 6573 7469 6d61 7465  d_point_estimate
-000146d0: 202a 2074 6865 7461 5f65 7272 6f72 5f73   * theta_error_s
-000146e0: 6967 4c65 7665 6c31 5b32 2c20 305d 0a20  igLevel1[2, 0]. 
-000146f0: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00014700: 335f 6572 726f 7220 3d20 3320 2a20 7365  3_error = 3 * se
-00014710: 6c66 2e66 6978 6564 5f70 6f69 6e74 5f65  lf.fixed_point_e
-00014720: 7374 696d 6174 6520 2a2a 2032 202a 2074  stimate ** 2 * t
-00014730: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
-00014740: 7665 6c31 5b33 2c20 305d 0a20 2020 2020  vel1[3, 0].     
-00014750: 2020 2020 2020 2073 656c 662e 4d41 505f         self.MAP_
-00014760: 736c 6f70 655f 6572 726f 7273 5b30 5d20  slope_errors[0] 
-00014770: 3d20 6e70 2e73 7172 7428 7061 7261 6d31  = np.sqrt(param1
-00014780: 5f65 7272 6f72 2a2a 3220 2b20 7061 7261  _error**2 + para
-00014790: 6d32 5f65 7272 6f72 2a2a 3220 2b20 7061  m2_error**2 + pa
-000147a0: 7261 6d33 5f65 7272 6f72 2a2a 3220 2b20  ram3_error**2 + 
-000147b0: 585f 6572 726f 722a 2a32 290a 0a20 2020  X_error**2)..   
-000147c0: 2020 2020 2020 2020 2023 2063 6f6d 7075           # compu
-000147d0: 7465 2077 6f72 7374 2063 6173 6520 7570  te worst case up
-000147e0: 7065 7220 626f 756e 640a 2020 2020 2020  per bound.      
-000147f0: 2020 2020 2020 7061 7261 6d31 5f65 7272        param1_err
-00014800: 6f72 203d 2031 202a 2074 6865 7461 5f65  or = 1 * theta_e
-00014810: 7272 6f72 5f73 6967 4c65 7665 6c31 5b31  rror_sigLevel1[1
-00014820: 2c20 315d 0a20 2020 2020 2020 2020 2020  , 1].           
-00014830: 2070 6172 616d 325f 6572 726f 7220 3d20   param2_error = 
-00014840: 3220 2a20 7365 6c66 2e66 6978 6564 5f70  2 * self.fixed_p
-00014850: 6f69 6e74 5f65 7374 696d 6174 6520 2a20  oint_estimate * 
-00014860: 7468 6574 615f 6572 726f 725f 7369 674c  theta_error_sigL
-00014870: 6576 656c 315b 322c 2031 5d0a 2020 2020  evel1[2, 1].    
-00014880: 2020 2020 2020 2020 7061 7261 6d33 5f65          param3_e
-00014890: 7272 6f72 203d 2033 202a 2073 656c 662e  rror = 3 * self.
-000148a0: 6669 7865 645f 706f 696e 745f 6573 7469  fixed_point_esti
-000148b0: 6d61 7465 202a 2a20 3220 2a20 7468 6574  mate ** 2 * thet
-000148c0: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
-000148d0: 315b 332c 2031 5d0a 2020 2020 2020 2020  1[3, 1].        
-000148e0: 2020 2020 7365 6c66 2e4d 4150 5f73 6c6f      self.MAP_slo
-000148f0: 7065 5f65 7272 6f72 735b 315d 203d 206e  pe_errors[1] = n
-00014900: 702e 7371 7274 2870 6172 616d 315f 6572  p.sqrt(param1_er
-00014910: 726f 7220 2a2a 2032 202b 2070 6172 616d  ror ** 2 + param
-00014920: 325f 6572 726f 7220 2a2a 2032 202b 2070  2_error ** 2 + p
-00014930: 6172 616d 335f 6572 726f 7220 2a2a 2032  aram3_error ** 2
-00014940: 202b 2058 5f65 7272 6f72 2a2a 3229 0a0a   + X_error**2)..
-00014950: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00014960: 6d70 7574 6520 776f 7273 7420 6361 7365  mpute worst case
-00014970: 206c 6f77 6572 2062 6f75 6e64 0a20 2020   lower bound.   
-00014980: 2020 2020 2020 2020 2070 6172 616d 315f           param1_
-00014990: 6572 726f 7220 3d20 3120 2a20 7468 6574  error = 1 * thet
-000149a0: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
-000149b0: 325b 312c 2030 5d0a 2020 2020 2020 2020  2[1, 0].        
-000149c0: 2020 2020 7061 7261 6d32 5f65 7272 6f72      param2_error
-000149d0: 203d 2032 202a 2073 656c 662e 6669 7865   = 2 * self.fixe
-000149e0: 645f 706f 696e 745f 6573 7469 6d61 7465  d_point_estimate
-000149f0: 202a 2074 6865 7461 5f65 7272 6f72 5f73   * theta_error_s
-00014a00: 6967 4c65 7665 6c32 5b32 2c20 305d 0a20  igLevel2[2, 0]. 
-00014a10: 2020 2020 2020 2020 2020 2070 6172 616d             param
-00014a20: 335f 6572 726f 7220 3d20 3320 2a20 7365  3_error = 3 * se
-00014a30: 6c66 2e66 6978 6564 5f70 6f69 6e74 5f65  lf.fixed_point_e
-00014a40: 7374 696d 6174 6520 2a2a 2032 202a 2074  stimate ** 2 * t
-00014a50: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
-00014a60: 7665 6c32 5b33 2c20 305d 0a20 2020 2020  vel2[3, 0].     
-00014a70: 2020 2020 2020 2073 656c 662e 4d41 505f         self.MAP_
-00014a80: 736c 6f70 655f 6572 726f 7273 5b32 5d20  slope_errors[2] 
-00014a90: 3d20 6e70 2e73 7172 7428 7061 7261 6d31  = np.sqrt(param1
-00014aa0: 5f65 7272 6f72 202a 2a20 3220 2b20 7061  _error ** 2 + pa
-00014ab0: 7261 6d32 5f65 7272 6f72 202a 2a20 3220  ram2_error ** 2 
-00014ac0: 2b20 7061 7261 6d33 5f65 7272 6f72 202a  + param3_error *
-00014ad0: 2a20 3220 2b20 585f 6572 726f 722a 2a32  * 2 + X_error**2
-00014ae0: 2920 2a20 322e 3535 3235 0a0a 2020 2020  ) * 2.5525..    
-00014af0: 2020 2020 2020 2020 2320 636f 6d70 7574          # comput
-00014b00: 6520 776f 7273 7420 6361 7365 2075 7070  e worst case upp
-00014b10: 6572 2062 6f75 6e64 0a20 2020 2020 2020  er bound.       
-00014b20: 2020 2020 2070 6172 616d 315f 6572 726f       param1_erro
-00014b30: 7220 3d20 3120 2a20 7468 6574 615f 6572  r = 1 * theta_er
-00014b40: 726f 725f 7369 674c 6576 656c 325b 312c  ror_sigLevel2[1,
-00014b50: 2031 5d0a 2020 2020 2020 2020 2020 2020   1].            
-00014b60: 7061 7261 6d32 5f65 7272 6f72 203d 2032  param2_error = 2
-00014b70: 202a 2073 656c 662e 6669 7865 645f 706f   * self.fixed_po
-00014b80: 696e 745f 6573 7469 6d61 7465 202a 2074  int_estimate * t
-00014b90: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
-00014ba0: 7665 6c32 5b32 2c20 315d 0a20 2020 2020  vel2[2, 1].     
-00014bb0: 2020 2020 2020 2070 6172 616d 335f 6572         param3_er
-00014bc0: 726f 7220 3d20 3320 2a20 7365 6c66 2e66  ror = 3 * self.f
-00014bd0: 6978 6564 5f70 6f69 6e74 5f65 7374 696d  ixed_point_estim
-00014be0: 6174 6520 2a2a 2032 202a 2074 6865 7461  ate ** 2 * theta
-00014bf0: 5f65 7272 6f72 5f73 6967 4c65 7665 6c32  _error_sigLevel2
-00014c00: 5b33 2c20 315d 0a20 2020 2020 2020 2020  [3, 1].         
-00014c10: 2020 2073 656c 662e 4d41 505f 736c 6f70     self.MAP_slop
-00014c20: 655f 6572 726f 7273 5b33 5d20 3d20 6e70  e_errors[3] = np
-00014c30: 2e73 7172 7428 7061 7261 6d31 5f65 7272  .sqrt(param1_err
-00014c40: 6f72 202a 2a20 3220 2b20 7061 7261 6d32  or ** 2 + param2
-00014c50: 5f65 7272 6f72 202a 2a20 3220 2b20 7061  _error ** 2 + pa
-00014c60: 7261 6d33 5f65 7272 6f72 202a 2a20 3220  ram3_error ** 2 
-00014c70: 2b20 585f 6572 726f 722a 2a32 2920 2a20  + X_error**2) * 
-00014c80: 322e 3535 3235 0a0a 2020 2020 2020 2020  2.5525..        
-00014c90: 656c 6966 2073 656c 662e 6472 6966 745f  elif self.drift_
-00014ca0: 6d6f 6465 6c20 3d3d 2027 6c69 6e65 6172  model == 'linear
-00014cb0: 206d 6f64 656c 273a 0a20 2020 2020 2020   model':.       
-00014cc0: 2020 2020 2073 656c 662e 4d41 505f 736c       self.MAP_sl
-00014cd0: 6f70 655f 6572 726f 7273 203d 206e 702e  ope_errors = np.
-00014ce0: 6172 7261 7928 5b74 6865 7461 5f65 7272  array([theta_err
-00014cf0: 6f72 5f73 6967 4c65 7665 6c31 5b31 2c20  or_sigLevel1[1, 
-00014d00: 305d 2c20 7468 6574 615f 6572 726f 725f  0], theta_error_
-00014d10: 7369 674c 6576 656c 315b 312c 2031 5d2c  sigLevel1[1, 1],
-00014d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00014d50: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
-00014d60: 7665 6c32 5b31 2c20 305d 2c20 7468 6574  vel2[1, 0], thet
-00014d70: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
-00014d80: 325b 312c 2031 5d5d 290a 2020 2020 2020  2[1, 1]]).      
-00014d90: 2020 7365 6c66 2e64 7269 6674 5f73 6c6f    self.drift_slo
-00014da0: 7065 5b31 5d20 3d20 7365 6c66 2e64 7269  pe[1] = self.dri
-00014db0: 6674 5f73 6c6f 7065 5b30 5d20 2d20 2873  ft_slope[0] - (s
-00014dc0: 656c 662e 4d41 505f 736c 6f70 655f 6572  elf.MAP_slope_er
-00014dd0: 726f 7273 5b30 5d29 0a20 2020 2020 2020  rors[0]).       
-00014de0: 2073 656c 662e 6472 6966 745f 736c 6f70   self.drift_slop
-00014df0: 655b 325d 203d 2073 656c 662e 6472 6966  e[2] = self.drif
-00014e00: 745f 736c 6f70 655b 305d 202b 2028 7365  t_slope[0] + (se
-00014e10: 6c66 2e4d 4150 5f73 6c6f 7065 5f65 7272  lf.MAP_slope_err
-00014e20: 6f72 735b 315d 290a 2020 2020 2020 2020  ors[1]).        
-00014e30: 7365 6c66 2e64 7269 6674 5f73 6c6f 7065  self.drift_slope
-00014e40: 5b33 5d20 3d20 7365 6c66 2e64 7269 6674  [3] = self.drift
-00014e50: 5f73 6c6f 7065 5b30 5d20 2d20 2873 656c  _slope[0] - (sel
-00014e60: 662e 4d41 505f 736c 6f70 655f 6572 726f  f.MAP_slope_erro
-00014e70: 7273 5b32 5d29 0a20 2020 2020 2020 2073  rs[2]).        s
-00014e80: 656c 662e 6472 6966 745f 736c 6f70 655b  elf.drift_slope[
-00014e90: 345d 203d 2073 656c 662e 6472 6966 745f  4] = self.drift_
-00014ea0: 736c 6f70 655b 305d 202b 2028 7365 6c66  slope[0] + (self
-00014eb0: 2e4d 4150 5f73 6c6f 7065 5f65 7272 6f72  .MAP_slope_error
-00014ec0: 735b 335d 290a 2020 2020 2020 2020 6966  s[3]).        if
-00014ed0: 2070 7269 6e74 626f 6f6c 3a0a 2020 2020   printbool:.    
-00014ee0: 2020 2020 2020 2020 7072 696e 7428 274d          print('M
-00014ef0: 4150 5f73 6c6f 7065 5f65 7272 6f72 733a  AP_slope_errors:
-00014f00: 2027 2c20 7365 6c66 2e4d 4150 5f73 6c6f   ', self.MAP_slo
-00014f10: 7065 5f65 7272 6f72 7329 0a20 2020 2020  pe_errors).     
-00014f20: 2020 2020 2020 2070 7269 6e74 2827 6472         print('dr
-00014f30: 6966 745f 736c 6f70 6520 6172 7261 793a  ift_slope array:
-00014f40: 2027 2c20 7365 6c66 2e64 7269 6674 5f73   ', self.drift_s
-00014f50: 6c6f 7065 290a 2020 2020 2020 2020 2020  lope).          
-00014f60: 2020 7072 696e 7428 275f 5f5f 5f5f 2729    print('_____')
-00014f70: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00014f80: 6e74 2827 446f 6e65 2127 290a 2020 2020  nt('Done!').    
-00014f90: 2020 2020 2020 2020 7072 696e 7428 275f          print('_
-00014fa0: 5f5f 5f5f 2729 0a0a 2020 2020 6465 6620  ____')..    def 
-00014fb0: 5f63 6f6d 7075 7465 5f73 6c6f 7065 5f65  _compute_slope_e
-00014fc0: 7272 6f72 5f6d 6172 6769 6e28 7365 6c66  rror_margin(self
-00014fd0: 2c20 7072 696e 7462 6f6f 6c29 3a0a 2020  , printbool):.  
-00014fe0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014ff0: 2020 4865 6c70 6572 2066 756e 6374 696f    Helper functio
-00015000: 6e20 7468 6174 2064 6574 6572 6d69 6e65  n that determine
-00015010: 7320 7468 6520 7379 6d6d 6574 7269 6320  s the symmetric 
-00015020: 756e 6365 7274 6169 6e74 7920 6261 6e64  uncertainty band
-00015030: 7320 6f66 2074 6865 204d 4150 2073 6c6f  s of the MAP slo
-00015040: 7065 2065 7374 696d 6174 6573 2076 6961  pe estimates via
-00015050: 0a20 2020 2020 2020 2047 6175 7373 6961  .        Gaussia
-00015060: 6e20 7072 6f70 6167 6174 696f 6e20 6f66  n propagation of
-00015070: 2075 6e63 6572 7461 696e 7469 6573 2e20   uncertainties. 
-00015080: 5468 6520 756e 6465 726c 7969 6e67 206d  The underlying m
-00015090: 6172 6769 6e61 6c20 756e 6365 7274 6169  arginal uncertai
-000150a0: 6e74 6965 7320 6f66 2074 6865 2060 604d  nties of the ``M
-000150b0: 4150 5f74 6865 7461 6060 0a20 2020 2020  AP_theta``.     
-000150c0: 2020 2061 7265 2065 7374 696d 6174 6564     are estimated
-000150d0: 2076 6961 2057 696c 6b73 2720 7468 656f   via Wilks' theo
-000150e0: 7265 6d20 616e 6420 7468 6520 6869 6768  rem and the high
-000150f0: 6572 2064 6576 6961 7469 6f6e 206f 6620  er deviation of 
-00015100: 6561 6368 2065 7374 696d 6174 6564 2060  each estimated `
-00015110: 604d 4150 5f74 6865 7461 6060 2069 7320  `MAP_theta`` is 
-00015120: 696e 7465 7270 7265 7465 640a 2020 2020  interpreted.    
-00015130: 2020 2020 6173 2073 796d 6d65 7472 6963      as symmetric
-00015140: 2065 7272 6f72 2062 6f75 6e64 2e20 5468   error bound. Th
-00015150: 6520 6465 7669 6174 696f 6e73 2061 7265  e deviations are
-00015160: 2070 726f 7061 6761 7465 6420 696e 2074   propagated in t
-00015170: 6572 6d73 206f 6620 6572 726f 7220 626f  erms of error bo
-00015180: 756e 6473 2e0a 2020 2020 2020 2020 5468  unds..        Th
-00015190: 6520 6572 726f 7220 626f 756e 6420 6f66  e error bound of
-000151a0: 2074 6865 2066 6978 6564 2070 6f69 6e74   the fixed point
-000151b0: 2065 7374 696d 6174 6520 6973 2061 7373   estimate is ass
-000151c0: 756d 6564 2074 6f20 6265 2065 7175 616c  umed to be equal
-000151d0: 2074 6f20 6120 4761 7573 7369 616e 203a   to a Gaussian :
-000151e0: 6d61 7468 3a60 335c 7369 676d 6160 202d  math:`3\sigma` -
-000151f0: 636f 6e66 6964 656e 6365 0a20 2020 2020  confidence.     
-00015200: 2020 2062 616e 642e 0a20 2020 2020 2020     band..       
-00015210: 2054 6865 2065 7374 696d 6174 696f 6e20   The estimation 
-00015220: 7465 6e64 7320 746f 2062 6520 746f 6f20  tends to be too 
-00015230: 6f70 7469 6d69 7374 6963 2c20 692e 652e  optimistic, i.e.
-00015240: 2074 6865 2075 6e63 6572 7461 696e 7479   the uncertainty
-00015250: 2062 6f75 6e64 7320 6172 6520 746f 6f20   bounds are too 
-00015260: 6e61 7272 6f77 2e20 5468 6520 4d41 5020  narrow. The MAP 
-00015270: 6573 7469 6d61 7469 6f6e 2074 656e 6473  estimation tends
-00015280: 0a20 2020 2020 2020 2074 6f20 7661 7279  .        to vary
-00015290: 2074 6f20 7374 726f 6e67 2066 6f72 2073   to strong for s
-000152a0: 7562 7365 7175 656e 7420 7769 6e64 6f77  ubsequent window
-000152b0: 732e 2049 7420 6973 206f 6e6c 7920 7573  s. It is only us
-000152c0: 6566 756c 2069 6e20 7468 6520 7665 7279  eful in the very
-000152d0: 2072 6172 6520 6361 7365 206f 6620 7665   rare case of ve
-000152e0: 7279 2068 6967 6820 616d 6f75 6e74 7320  ry high amounts 
-000152f0: 6f66 0a20 2020 2020 2020 2073 7461 7469  of.        stati
-00015300: 6f6e 6172 7920 6461 7461 2070 6572 2077  onary data per w
-00015310: 696e 646f 772e 2049 7420 6973 2072 6563  indow. It is rec
-00015320: 6f6d 6d65 6e64 6564 2074 6f20 7573 6520  ommended to use 
-00015330: 7468 6520 7375 6d6d 6172 7920 7374 6174  the summary stat
-00015340: 6973 7469 6373 2075 6e63 6572 7461 696e  istics uncertain
-00015350: 7479 2062 616e 6473 2e0a 0a20 2020 2020  ty bands...     
-00015360: 2020 203a 7061 7261 6d20 7072 696e 7462     :param printb
-00015370: 6f6f 6c3a 2044 6574 6572 6d69 6e65 7320  ool: Determines 
-00015380: 7768 6574 6865 7220 6120 6465 7461 696c  whether a detail
-00015390: 6564 206f 7574 7075 7420 6973 2070 7269  ed output is pri
-000153a0: 6e74 6564 206f 7220 6e6f 742e 0a20 2020  nted or not..   
-000153b0: 2020 2020 203a 7479 7065 2070 7269 6e74       :type print
-000153c0: 626f 6f6c 3a20 426f 6f6c 6561 6e0a 2020  bool: Boolean.  
-000153d0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000153e0: 2020 2069 6620 7072 696e 7462 6f6f 6c3a     if printbool:
-000153f0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00015400: 6e74 2827 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  nt('____________
-00015410: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00015420: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00015430: 5f5f 2729 0a20 2020 2020 2020 2020 2020  __').           
-00015440: 2070 7269 6e74 2827 436f 6d70 7574 6520   print('Compute 
-00015450: 7379 6d6d 6574 7269 6320 736c 6f70 6520  symmetric slope 
-00015460: 6572 726f 7220 6d61 7267 696e 732e 2729  error margins.')
-00015470: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00015480: 6e74 2827 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  nt('____________
-00015490: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000154a0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-000154b0: 5f5f 2729 0a20 2020 2020 2020 2073 656c  __').        sel
-000154c0: 662e 6669 7865 645f 706f 696e 745f 6573  f.fixed_point_es
-000154d0: 7469 6d61 7465 203d 206e 702e 6d65 616e  timate = np.mean
-000154e0: 2873 656c 662e 6461 7461 5f77 696e 646f  (self.data_windo
-000154f0: 7729 0a20 2020 2020 2020 2064 6174 615f  w).        data_
-00015500: 7769 6e64 6f77 5f65 7272 6f72 203d 206e  window_error = n
-00015510: 702e 7371 7274 2831 2e20 2f20 2873 656c  p.sqrt(1. / (sel
-00015520: 662e 6461 7461 5f77 696e 646f 772e 7369  f.data_window.si
-00015530: 7a65 2920 2a20 6e70 2e76 6172 2873 656c  ze) * np.var(sel
-00015540: 662e 6461 7461 5f77 696e 646f 7729 2920  f.data_window)) 
-00015550: 2a20 322e 3535 3235 0a20 2020 2020 2020  * 2.5525.       
-00015560: 2058 5f65 7272 6f72 5f62 6f75 6e64 203d   X_error_bound =
-00015570: 2061 6273 2832 202a 2073 656c 662e 4d41   abs(2 * self.MA
-00015580: 505f 7468 6574 615b 322c 2030 5d20 2b20  P_theta[2, 0] + 
-00015590: 3620 2a20 7365 6c66 2e66 6978 6564 5f70  6 * self.fixed_p
-000155a0: 6f69 6e74 5f65 7374 696d 6174 6520 2a0a  oint_estimate *.
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2020 2073 656c 662e 4d41 505f 7468 6574     self.MAP_thet
-000155d0: 615b 332c 2030 5d29 202a 2064 6174 615f  a[3, 0]) * data_
-000155e0: 7769 6e64 6f77 5f65 7272 6f72 0a20 2020  window_error.   
-000155f0: 2020 2020 2073 656c 662e 4d41 505f 736c       self.MAP_sl
-00015600: 6f70 655f 6d61 7267 696e 203d 206e 702e  ope_margin = np.
-00015610: 7a65 726f 7328 3229 0a20 2020 2020 2020  zeros(2).       
-00015620: 2074 6865 7461 5f65 7272 6f72 5f73 6967   theta_error_sig
-00015630: 4c65 7665 6c31 203d 206e 702e 7a65 726f  Level1 = np.zero
-00015640: 7328 2873 656c 662e 6e64 696d 2c20 3229  s((self.ndim, 2)
-00015650: 290a 2020 2020 2020 2020 7468 6574 615f  ).        theta_
-00015660: 6572 726f 725f 7369 674c 6576 656c 3220  error_sigLevel2 
-00015670: 3d20 6e70 2e7a 6572 6f73 2828 7365 6c66  = np.zeros((self
-00015680: 2e6e 6469 6d2c 2032 2929 0a20 2020 2020  .ndim, 2)).     
-00015690: 2020 2074 6865 7461 5f65 7272 6f72 5f73     theta_error_s
-000156a0: 6967 4c65 7665 6c31 5b3a 2c20 305d 203d  igLevel1[:, 0] =
-000156b0: 2073 656c 662e 4d41 505f 4349 5b3a 2c20   self.MAP_CI[:, 
-000156c0: 305d 0a20 2020 2020 2020 2074 6865 7461  0].        theta
-000156d0: 5f65 7272 6f72 5f73 6967 4c65 7665 6c31  _error_sigLevel1
-000156e0: 5b3a 2c20 315d 203d 2073 656c 662e 4d41  [:, 1] = self.MA
-000156f0: 505f 4349 5b3a 2c20 315d 0a20 2020 2020  P_CI[:, 1].     
-00015700: 2020 2074 6865 7461 5f6d 6172 6769 6e31     theta_margin1
-00015710: 203d 206e 702e 6d61 7869 6d75 6d28 6e70   = np.maximum(np
-00015720: 2e61 6273 6f6c 7574 6528 7468 6574 615f  .absolute(theta_
-00015730: 6572 726f 725f 7369 674c 6576 656c 315b  error_sigLevel1[
-00015740: 313a 2c20 305d 292c 2074 6865 7461 5f65  1:, 0]), theta_e
-00015750: 7272 6f72 5f73 6967 4c65 7665 6c31 5b31  rror_sigLevel1[1
-00015760: 3a2c 2031 5d29 0a20 2020 2020 2020 2074  :, 1]).        t
-00015770: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
-00015780: 7665 6c32 5b3a 2c20 305d 203d 2073 656c  vel2[:, 0] = sel
-00015790: 662e 4d41 505f 4349 5b3a 2c20 325d 0a20  f.MAP_CI[:, 2]. 
-000157a0: 2020 2020 2020 2074 6865 7461 5f65 7272         theta_err
-000157b0: 6f72 5f73 6967 4c65 7665 6c32 5b3a 2c20  or_sigLevel2[:, 
-000157c0: 315d 203d 2073 656c 662e 4d41 505f 4349  1] = self.MAP_CI
-000157d0: 5b3a 2c20 335d 0a20 2020 2020 2020 2074  [:, 3].        t
-000157e0: 6865 7461 5f6d 6172 6769 6e32 203d 206e  heta_margin2 = n
-000157f0: 702e 6d61 7869 6d75 6d28 6e70 2e61 6273  p.maximum(np.abs
-00015800: 6f6c 7574 6528 7468 6574 615f 6572 726f  olute(theta_erro
-00015810: 725f 7369 674c 6576 656c 325b 313a 2c20  r_sigLevel2[1:, 
-00015820: 305d 292c 2074 6865 7461 5f65 7272 6f72  0]), theta_error
-00015830: 5f73 6967 4c65 7665 6c32 5b31 3a2c 2031  _sigLevel2[1:, 1
-00015840: 5d29 0a20 2020 2020 2020 2070 6172 616d  ]).        param
-00015850: 315f 6d61 7267 696e 203d 2031 202a 2074  1_margin = 1 * t
-00015860: 6865 7461 5f6d 6172 6769 6e31 5b30 5d0a  heta_margin1[0].
-00015870: 2020 2020 2020 2020 7061 7261 6d32 5f6d          param2_m
-00015880: 6172 6769 6e20 3d20 3220 2a20 6e70 2e61  argin = 2 * np.a
-00015890: 6273 6f6c 7574 6528 7365 6c66 2e66 6978  bsolute(self.fix
-000158a0: 6564 5f70 6f69 6e74 5f65 7374 696d 6174  ed_point_estimat
-000158b0: 6529 202a 2074 6865 7461 5f6d 6172 6769  e) * theta_margi
-000158c0: 6e31 5b31 5d0a 2020 2020 2020 2020 7061  n1[1].        pa
-000158d0: 7261 6d33 5f6d 6172 6769 6e20 3d20 3320  ram3_margin = 3 
-000158e0: 2a20 7365 6c66 2e66 6978 6564 5f70 6f69  * self.fixed_poi
-000158f0: 6e74 5f65 7374 696d 6174 6520 2a2a 2032  nt_estimate ** 2
-00015900: 202a 2074 6865 7461 5f6d 6172 6769 6e31   * theta_margin1
-00015910: 5b32 5d0a 2020 2020 2020 2020 7365 6c66  [2].        self
-00015920: 2e4d 4150 5f73 6c6f 7065 5f6d 6172 6769  .MAP_slope_margi
-00015930: 6e5b 305d 203d 2070 6172 616d 315f 6d61  n[0] = param1_ma
-00015940: 7267 696e 202b 2070 6172 616d 325f 6d61  rgin + param2_ma
-00015950: 7267 696e 202b 2070 6172 616d 335f 6d61  rgin + param3_ma
-00015960: 7267 696e 202b 2058 5f65 7272 6f72 5f62  rgin + X_error_b
-00015970: 6f75 6e64 0a20 2020 2020 2020 2070 6172  ound.        par
-00015980: 616d 315f 6d61 7267 696e 203d 2031 202a  am1_margin = 1 *
-00015990: 2074 6865 7461 5f6d 6172 6769 6e32 5b30   theta_margin2[0
-000159a0: 5d0a 2020 2020 2020 2020 7061 7261 6d32  ].        param2
-000159b0: 5f6d 6172 6769 6e20 3d20 3220 2a20 6e70  _margin = 2 * np
-000159c0: 2e61 6273 6f6c 7574 6528 7365 6c66 2e66  .absolute(self.f
-000159d0: 6978 6564 5f70 6f69 6e74 5f65 7374 696d  ixed_point_estim
-000159e0: 6174 6529 202a 2074 6865 7461 5f6d 6172  ate) * theta_mar
-000159f0: 6769 6e32 5b31 5d0a 2020 2020 2020 2020  gin2[1].        
-00015a00: 7061 7261 6d33 5f6d 6172 6769 6e20 3d20  param3_margin = 
-00015a10: 3320 2a20 7365 6c66 2e66 6978 6564 5f70  3 * self.fixed_p
-00015a20: 6f69 6e74 5f65 7374 696d 6174 6520 2a2a  oint_estimate **
-00015a30: 2032 202a 2074 6865 7461 5f6d 6172 6769   2 * theta_margi
-00015a40: 6e32 5b32 5d0a 2020 2020 2020 2020 7365  n2[2].        se
-00015a50: 6c66 2e4d 4150 5f73 6c6f 7065 5f6d 6172  lf.MAP_slope_mar
-00015a60: 6769 6e5b 315d 203d 2070 6172 616d 315f  gin[1] = param1_
-00015a70: 6d61 7267 696e 202b 2070 6172 616d 325f  margin + param2_
-00015a80: 6d61 7267 696e 202b 2070 6172 616d 335f  margin + param3_
-00015a90: 6d61 7267 696e 202b 2058 5f65 7272 6f72  margin + X_error
-00015aa0: 5f62 6f75 6e64 0a20 2020 2020 2020 2073  _bound.        s
-00015ab0: 656c 662e 6472 6966 745f 736c 6f70 655b  elf.drift_slope[
-00015ac0: 315d 203d 2073 656c 662e 6472 6966 745f  1] = self.drift_
-00015ad0: 736c 6f70 655b 305d 202d 2073 656c 662e  slope[0] - self.
-00015ae0: 4d41 505f 736c 6f70 655f 6d61 7267 696e  MAP_slope_margin
-00015af0: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
-00015b00: 2e64 7269 6674 5f73 6c6f 7065 5b32 5d20  .drift_slope[2] 
-00015b10: 3d20 7365 6c66 2e64 7269 6674 5f73 6c6f  = self.drift_slo
-00015b20: 7065 5b30 5d20 2b20 7365 6c66 2e4d 4150  pe[0] + self.MAP
-00015b30: 5f73 6c6f 7065 5f6d 6172 6769 6e5b 305d  _slope_margin[0]
-00015b40: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
-00015b50: 6966 745f 736c 6f70 655b 335d 203d 2073  ift_slope[3] = s
-00015b60: 656c 662e 6472 6966 745f 736c 6f70 655b  elf.drift_slope[
-00015b70: 305d 202d 2073 656c 662e 4d41 505f 736c  0] - self.MAP_sl
-00015b80: 6f70 655f 6d61 7267 696e 5b31 5d0a 2020  ope_margin[1].  
-00015b90: 2020 2020 2020 7365 6c66 2e64 7269 6674        self.drift
-00015ba0: 5f73 6c6f 7065 5b34 5d20 3d20 7365 6c66  _slope[4] = self
-00015bb0: 2e64 7269 6674 5f73 6c6f 7065 5b30 5d20  .drift_slope[0] 
-00015bc0: 2b20 7365 6c66 2e4d 4150 5f73 6c6f 7065  + self.MAP_slope
-00015bd0: 5f6d 6172 6769 6e5b 315d 0a20 2020 2020  _margin[1].     
-00015be0: 2020 2069 6620 7072 696e 7462 6f6f 6c3a     if printbool:
-00015bf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00015c00: 6e74 2827 4d41 505f 736c 6f70 655f 6d61  nt('MAP_slope_ma
-00015c10: 7267 696e 3a20 272c 2073 656c 662e 4d41  rgin: ', self.MA
-00015c20: 505f 736c 6f70 655f 6d61 7267 696e 290a  P_slope_margin).
-00015c30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00015c40: 7428 2764 7269 6674 5f73 6c6f 7065 2061  t('drift_slope a
-00015c50: 7272 6179 3a20 272c 2073 656c 662e 6472  rray: ', self.dr
-00015c60: 6966 745f 736c 6f70 6529 0a20 2020 2020  ift_slope).     
-00015c70: 2020 2020 2020 2070 7269 6e74 2827 5f5f         print('__
-00015c80: 5f5f 5f27 290a 2020 2020 2020 2020 2020  ___').          
-00015c90: 2020 7072 696e 7428 2744 6f6e 6521 2729    print('Done!')
-00015ca0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00015cb0: 6e74 2827 5f5f 5f5f 5f27 29              nt('_____')
+00014290: 5f5f 5f5f 5f5f 5f5f 2729 0a20 2020 2020  ________').     
+000142a0: 2020 2073 656c 662e 4d41 505f 736c 6f70     self.MAP_slop
+000142b0: 655f 6572 726f 7273 203d 206e 702e 7a65  e_errors = np.ze
+000142c0: 726f 7328 3429 0a20 2020 2020 2020 2074  ros(4).        t
+000142d0: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
+000142e0: 7665 6c31 203d 206e 702e 7a65 726f 7328  vel1 = np.zeros(
+000142f0: 2873 656c 662e 6e64 696d 2c20 3229 290a  (self.ndim, 2)).
+00014300: 2020 2020 2020 2020 7468 6574 615f 6572          theta_er
+00014310: 726f 725f 7369 674c 6576 656c 3220 3d20  ror_sigLevel2 = 
+00014320: 6e70 2e7a 6572 6f73 2828 7365 6c66 2e6e  np.zeros((self.n
+00014330: 6469 6d2c 2032 2929 0a0a 2020 2020 2020  dim, 2))..      
+00014340: 2020 7468 6574 615f 6572 726f 725f 7369    theta_error_si
+00014350: 674c 6576 656c 315b 3a2c 2030 5d20 3d20  gLevel1[:, 0] = 
+00014360: 7365 6c66 2e4d 4150 5f43 495b 3a2c 2030  self.MAP_CI[:, 0
+00014370: 5d2f 312e 3936 0a20 2020 2020 2020 2074  ]/1.96.        t
+00014380: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
+00014390: 7665 6c31 5b3a 2c20 315d 203d 2073 656c  vel1[:, 1] = sel
+000143a0: 662e 4d41 505f 4349 5b3a 2c20 315d 2f31  f.MAP_CI[:, 1]/1
+000143b0: 2e39 360a 0a20 2020 2020 2020 2074 6865  .96..        the
+000143c0: 7461 5f65 7272 6f72 5f73 6967 4c65 7665  ta_error_sigLeve
+000143d0: 6c32 5b3a 2c20 305d 203d 2073 656c 662e  l2[:, 0] = self.
+000143e0: 4d41 505f 4349 5b3a 2c20 325d 2f32 2e35  MAP_CI[:, 2]/2.5
+000143f0: 3735 0a20 2020 2020 2020 2074 6865 7461  75.        theta
+00014400: 5f65 7272 6f72 5f73 6967 4c65 7665 6c32  _error_sigLevel2
+00014410: 5b3a 2c20 315d 203d 2073 656c 662e 4d41  [:, 1] = self.MA
+00014420: 505f 4349 5b3a 2c20 335d 2f32 2e35 3735  P_CI[:, 3]/2.575
+00014430: 0a0a 2020 2020 2020 2020 2320 636f 6d70  ..        # comp
+00014440: 7574 6520 776f 7273 7420 6361 7365 206c  ute worst case l
+00014450: 6f77 6572 2062 6f75 6e64 0a20 2020 2020  ower bound.     
+00014460: 2020 2069 6620 7365 6c66 2e64 7269 6674     if self.drift
+00014470: 5f6d 6f64 656c 203d 3d20 2733 7264 206f  _model == '3rd o
+00014480: 7264 6572 2070 6f6c 796e 6f6d 6961 6c27  rder polynomial'
+00014490: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+000144a0: 7461 5f77 696e 646f 775f 6572 726f 7220  ta_window_error 
+000144b0: 3d20 6e70 2e73 7172 7428 312e 2f28 7365  = np.sqrt(1./(se
+000144c0: 6c66 2e64 6174 615f 7769 6e64 6f77 2e73  lf.data_window.s
+000144d0: 697a 6529 202a 206e 702e 7661 7228 7365  ize) * np.var(se
+000144e0: 6c66 2e64 6174 615f 7769 6e64 6f77 2929  lf.data_window))
+000144f0: 0a20 2020 2020 2020 2020 2020 2058 5f65  .            X_e
+00014500: 7272 6f72 203d 2028 3220 2a20 7365 6c66  rror = (2 * self
+00014510: 2e4d 4150 5f74 6865 7461 5b32 2c20 305d  .MAP_theta[2, 0]
+00014520: 202b 2036 202a 2073 656c 662e 6669 7865   + 6 * self.fixe
+00014530: 645f 706f 696e 745f 6573 7469 6d61 7465  d_point_estimate
+00014540: 202a 0a20 2020 2020 2020 2020 2020 2020   *.             
+00014550: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
+00014560: 4150 5f74 6865 7461 5b33 2c20 305d 2920  AP_theta[3, 0]) 
+00014570: 2a20 6461 7461 5f77 696e 646f 775f 6572  * data_window_er
+00014580: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+00014590: 7061 7261 6d31 5f65 7272 6f72 203d 2031  param1_error = 1
+000145a0: 202a 2074 6865 7461 5f65 7272 6f72 5f73   * theta_error_s
+000145b0: 6967 4c65 7665 6c31 5b31 2c20 305d 0a20  igLevel1[1, 0]. 
+000145c0: 2020 2020 2020 2020 2020 2070 6172 616d             param
+000145d0: 325f 6572 726f 7220 3d20 3220 2a20 7365  2_error = 2 * se
+000145e0: 6c66 2e66 6978 6564 5f70 6f69 6e74 5f65  lf.fixed_point_e
+000145f0: 7374 696d 6174 6520 2a20 7468 6574 615f  stimate * theta_
+00014600: 6572 726f 725f 7369 674c 6576 656c 315b  error_sigLevel1[
+00014610: 322c 2030 5d0a 2020 2020 2020 2020 2020  2, 0].          
+00014620: 2020 7061 7261 6d33 5f65 7272 6f72 203d    param3_error =
+00014630: 2033 202a 2073 656c 662e 6669 7865 645f   3 * self.fixed_
+00014640: 706f 696e 745f 6573 7469 6d61 7465 202a  point_estimate *
+00014650: 2a20 3220 2a20 7468 6574 615f 6572 726f  * 2 * theta_erro
+00014660: 725f 7369 674c 6576 656c 315b 332c 2030  r_sigLevel1[3, 0
+00014670: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00014680: 6c66 2e4d 4150 5f73 6c6f 7065 5f65 7272  lf.MAP_slope_err
+00014690: 6f72 735b 305d 203d 206e 702e 7371 7274  ors[0] = np.sqrt
+000146a0: 2870 6172 616d 315f 6572 726f 722a 2a32  (param1_error**2
+000146b0: 202b 2070 6172 616d 325f 6572 726f 722a   + param2_error*
+000146c0: 2a32 202b 2070 6172 616d 335f 6572 726f  *2 + param3_erro
+000146d0: 722a 2a32 202b 2058 5f65 7272 6f72 2a2a  r**2 + X_error**
+000146e0: 3229 202a 2031 2e39 360a 0a20 2020 2020  2) * 1.96..     
+000146f0: 2020 2020 2020 2023 2063 6f6d 7075 7465         # compute
+00014700: 2077 6f72 7374 2063 6173 6520 7570 7065   worst case uppe
+00014710: 7220 626f 756e 640a 2020 2020 2020 2020  r bound.        
+00014720: 2020 2020 7061 7261 6d31 5f65 7272 6f72      param1_error
+00014730: 203d 2031 202a 2074 6865 7461 5f65 7272   = 1 * theta_err
+00014740: 6f72 5f73 6967 4c65 7665 6c31 5b31 2c20  or_sigLevel1[1, 
+00014750: 315d 0a20 2020 2020 2020 2020 2020 2070  1].            p
+00014760: 6172 616d 325f 6572 726f 7220 3d20 3220  aram2_error = 2 
+00014770: 2a20 7365 6c66 2e66 6978 6564 5f70 6f69  * self.fixed_poi
+00014780: 6e74 5f65 7374 696d 6174 6520 2a20 7468  nt_estimate * th
+00014790: 6574 615f 6572 726f 725f 7369 674c 6576  eta_error_sigLev
+000147a0: 656c 315b 322c 2031 5d0a 2020 2020 2020  el1[2, 1].      
+000147b0: 2020 2020 2020 7061 7261 6d33 5f65 7272        param3_err
+000147c0: 6f72 203d 2033 202a 2073 656c 662e 6669  or = 3 * self.fi
+000147d0: 7865 645f 706f 696e 745f 6573 7469 6d61  xed_point_estima
+000147e0: 7465 202a 2a20 3220 2a20 7468 6574 615f  te ** 2 * theta_
+000147f0: 6572 726f 725f 7369 674c 6576 656c 315b  error_sigLevel1[
+00014800: 332c 2031 5d0a 2020 2020 2020 2020 2020  3, 1].          
+00014810: 2020 7365 6c66 2e4d 4150 5f73 6c6f 7065    self.MAP_slope
+00014820: 5f65 7272 6f72 735b 315d 203d 206e 702e  _errors[1] = np.
+00014830: 7371 7274 2870 6172 616d 315f 6572 726f  sqrt(param1_erro
+00014840: 7220 2a2a 2032 202b 2070 6172 616d 325f  r ** 2 + param2_
+00014850: 6572 726f 7220 2a2a 2032 202b 2070 6172  error ** 2 + par
+00014860: 616d 335f 6572 726f 7220 2a2a 2032 202b  am3_error ** 2 +
+00014870: 2058 5f65 7272 6f72 2a2a 3229 202a 2031   X_error**2) * 1
+00014880: 2e39 360a 0a20 2020 2020 2020 2020 2020  .96..           
+00014890: 2023 2063 6f6d 7075 7465 2077 6f72 7374   # compute worst
+000148a0: 2063 6173 6520 6c6f 7765 7220 626f 756e   case lower boun
+000148b0: 640a 2020 2020 2020 2020 2020 2020 7061  d.            pa
+000148c0: 7261 6d31 5f65 7272 6f72 203d 2031 202a  ram1_error = 1 *
+000148d0: 2074 6865 7461 5f65 7272 6f72 5f73 6967   theta_error_sig
+000148e0: 4c65 7665 6c32 5b31 2c20 305d 0a20 2020  Level2[1, 0].   
+000148f0: 2020 2020 2020 2020 2070 6172 616d 325f           param2_
+00014900: 6572 726f 7220 3d20 3220 2a20 7365 6c66  error = 2 * self
+00014910: 2e66 6978 6564 5f70 6f69 6e74 5f65 7374  .fixed_point_est
+00014920: 696d 6174 6520 2a20 7468 6574 615f 6572  imate * theta_er
+00014930: 726f 725f 7369 674c 6576 656c 325b 322c  ror_sigLevel2[2,
+00014940: 2030 5d0a 2020 2020 2020 2020 2020 2020   0].            
+00014950: 7061 7261 6d33 5f65 7272 6f72 203d 2033  param3_error = 3
+00014960: 202a 2073 656c 662e 6669 7865 645f 706f   * self.fixed_po
+00014970: 696e 745f 6573 7469 6d61 7465 202a 2a20  int_estimate ** 
+00014980: 3220 2a20 7468 6574 615f 6572 726f 725f  2 * theta_error_
+00014990: 7369 674c 6576 656c 325b 332c 2030 5d0a  sigLevel2[3, 0].
+000149a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000149b0: 2e4d 4150 5f73 6c6f 7065 5f65 7272 6f72  .MAP_slope_error
+000149c0: 735b 325d 203d 206e 702e 7371 7274 2870  s[2] = np.sqrt(p
+000149d0: 6172 616d 315f 6572 726f 7220 2a2a 2032  aram1_error ** 2
+000149e0: 202b 2070 6172 616d 325f 6572 726f 7220   + param2_error 
+000149f0: 2a2a 2032 202b 2070 6172 616d 335f 6572  ** 2 + param3_er
+00014a00: 726f 7220 2a2a 2032 202b 2058 5f65 7272  ror ** 2 + X_err
+00014a10: 6f72 2a2a 3229 202a 2032 2e35 3735 0a0a  or**2) * 2.575..
+00014a20: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00014a30: 6d70 7574 6520 776f 7273 7420 6361 7365  mpute worst case
+00014a40: 2075 7070 6572 2062 6f75 6e64 0a20 2020   upper bound.   
+00014a50: 2020 2020 2020 2020 2070 6172 616d 315f           param1_
+00014a60: 6572 726f 7220 3d20 3120 2a20 7468 6574  error = 1 * thet
+00014a70: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
+00014a80: 325b 312c 2031 5d0a 2020 2020 2020 2020  2[1, 1].        
+00014a90: 2020 2020 7061 7261 6d32 5f65 7272 6f72      param2_error
+00014aa0: 203d 2032 202a 2073 656c 662e 6669 7865   = 2 * self.fixe
+00014ab0: 645f 706f 696e 745f 6573 7469 6d61 7465  d_point_estimate
+00014ac0: 202a 2074 6865 7461 5f65 7272 6f72 5f73   * theta_error_s
+00014ad0: 6967 4c65 7665 6c32 5b32 2c20 315d 0a20  igLevel2[2, 1]. 
+00014ae0: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00014af0: 335f 6572 726f 7220 3d20 3320 2a20 7365  3_error = 3 * se
+00014b00: 6c66 2e66 6978 6564 5f70 6f69 6e74 5f65  lf.fixed_point_e
+00014b10: 7374 696d 6174 6520 2a2a 2032 202a 2074  stimate ** 2 * t
+00014b20: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
+00014b30: 7665 6c32 5b33 2c20 315d 0a20 2020 2020  vel2[3, 1].     
+00014b40: 2020 2020 2020 2073 656c 662e 4d41 505f         self.MAP_
+00014b50: 736c 6f70 655f 6572 726f 7273 5b33 5d20  slope_errors[3] 
+00014b60: 3d20 6e70 2e73 7172 7428 7061 7261 6d31  = np.sqrt(param1
+00014b70: 5f65 7272 6f72 202a 2a20 3220 2b20 7061  _error ** 2 + pa
+00014b80: 7261 6d32 5f65 7272 6f72 202a 2a20 3220  ram2_error ** 2 
+00014b90: 2b20 7061 7261 6d33 5f65 7272 6f72 202a  + param3_error *
+00014ba0: 2a20 3220 2b20 585f 6572 726f 722a 2a32  * 2 + X_error**2
+00014bb0: 2920 2a20 322e 3537 350a 0a20 2020 2020  ) * 2.575..     
+00014bc0: 2020 2065 6c69 6620 7365 6c66 2e64 7269     elif self.dri
+00014bd0: 6674 5f6d 6f64 656c 203d 3d20 276c 696e  ft_model == 'lin
+00014be0: 6561 7220 6d6f 6465 6c27 3a0a 2020 2020  ear model':.    
+00014bf0: 2020 2020 2020 2020 7365 6c66 2e4d 4150          self.MAP
+00014c00: 5f73 6c6f 7065 5f65 7272 6f72 7320 3d20  _slope_errors = 
+00014c10: 6e70 2e61 7272 6179 285b 7468 6574 615f  np.array([theta_
+00014c20: 6572 726f 725f 7369 674c 6576 656c 315b  error_sigLevel1[
+00014c30: 312c 2030 5d2c 2074 6865 7461 5f65 7272  1, 0], theta_err
+00014c40: 6f72 5f73 6967 4c65 7665 6c31 5b31 2c20  or_sigLevel1[1, 
+00014c50: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c80: 2020 7468 6574 615f 6572 726f 725f 7369    theta_error_si
+00014c90: 674c 6576 656c 325b 312c 2030 5d2c 2074  gLevel2[1, 0], t
+00014ca0: 6865 7461 5f65 7272 6f72 5f73 6967 4c65  heta_error_sigLe
+00014cb0: 7665 6c32 5b31 2c20 315d 5d29 0a20 2020  vel2[1, 1]]).   
+00014cc0: 2020 2020 2073 656c 662e 6472 6966 745f       self.drift_
+00014cd0: 736c 6f70 655b 315d 203d 2073 656c 662e  slope[1] = self.
+00014ce0: 6472 6966 745f 736c 6f70 655b 305d 202d  drift_slope[0] -
+00014cf0: 2028 7365 6c66 2e4d 4150 5f73 6c6f 7065   (self.MAP_slope
+00014d00: 5f65 7272 6f72 735b 305d 290a 2020 2020  _errors[0]).    
+00014d10: 2020 2020 7365 6c66 2e64 7269 6674 5f73      self.drift_s
+00014d20: 6c6f 7065 5b32 5d20 3d20 7365 6c66 2e64  lope[2] = self.d
+00014d30: 7269 6674 5f73 6c6f 7065 5b30 5d20 2b20  rift_slope[0] + 
+00014d40: 2873 656c 662e 4d41 505f 736c 6f70 655f  (self.MAP_slope_
+00014d50: 6572 726f 7273 5b31 5d29 0a20 2020 2020  errors[1]).     
+00014d60: 2020 2073 656c 662e 6472 6966 745f 736c     self.drift_sl
+00014d70: 6f70 655b 335d 203d 2073 656c 662e 6472  ope[3] = self.dr
+00014d80: 6966 745f 736c 6f70 655b 305d 202d 2028  ift_slope[0] - (
+00014d90: 7365 6c66 2e4d 4150 5f73 6c6f 7065 5f65  self.MAP_slope_e
+00014da0: 7272 6f72 735b 325d 290a 2020 2020 2020  rrors[2]).      
+00014db0: 2020 7365 6c66 2e64 7269 6674 5f73 6c6f    self.drift_slo
+00014dc0: 7065 5b34 5d20 3d20 7365 6c66 2e64 7269  pe[4] = self.dri
+00014dd0: 6674 5f73 6c6f 7065 5b30 5d20 2b20 2873  ft_slope[0] + (s
+00014de0: 656c 662e 4d41 505f 736c 6f70 655f 6572  elf.MAP_slope_er
+00014df0: 726f 7273 5b33 5d29 0a20 2020 2020 2020  rors[3]).       
+00014e00: 2069 6620 7072 696e 7462 6f6f 6c3a 0a20   if printbool:. 
+00014e10: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00014e20: 2827 4d41 505f 736c 6f70 655f 6572 726f  ('MAP_slope_erro
+00014e30: 7273 3a20 272c 2073 656c 662e 4d41 505f  rs: ', self.MAP_
+00014e40: 736c 6f70 655f 6572 726f 7273 290a 2020  slope_errors).  
+00014e50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00014e60: 2764 7269 6674 5f73 6c6f 7065 2061 7272  'drift_slope arr
+00014e70: 6179 3a20 272c 2073 656c 662e 6472 6966  ay: ', self.drif
+00014e80: 745f 736c 6f70 6529 0a20 2020 2020 2020  t_slope).       
+00014e90: 2020 2020 2070 7269 6e74 2827 5f5f 5f5f       print('____
+00014ea0: 5f27 290a 2020 2020 2020 2020 2020 2020  _').            
+00014eb0: 7072 696e 7428 2744 6f6e 6521 2729 0a20  print('Done!'). 
+00014ec0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00014ed0: 2827 5f5f 5f5f 5f27 290a 0a20 2020 2064  ('_____')..    d
+00014ee0: 6566 205f 636f 6d70 7574 655f 736c 6f70  ef _compute_slop
+00014ef0: 655f 6572 726f 725f 6d61 7267 696e 2873  e_error_margin(s
+00014f00: 656c 662c 2070 7269 6e74 626f 6f6c 293a  elf, printbool):
+00014f10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014f20: 2020 2020 2048 656c 7065 7220 6675 6e63       Helper func
+00014f30: 7469 6f6e 2074 6861 7420 6465 7465 726d  tion that determ
+00014f40: 696e 6573 2074 6865 2073 796d 6d65 7472  ines the symmetr
+00014f50: 6963 2075 6e63 6572 7461 696e 7479 2062  ic uncertainty b
+00014f60: 616e 6473 206f 6620 7468 6520 4d41 5020  ands of the MAP 
+00014f70: 736c 6f70 6520 6573 7469 6d61 7465 7320  slope estimates 
+00014f80: 7669 610a 2020 2020 2020 2020 4761 7573  via.        Gaus
+00014f90: 7369 616e 2070 726f 7061 6761 7469 6f6e  sian propagation
+00014fa0: 206f 6620 756e 6365 7274 6169 6e74 6965   of uncertaintie
+00014fb0: 732e 2054 6865 2075 6e64 6572 6c79 696e  s. The underlyin
+00014fc0: 6720 6d61 7267 696e 616c 2075 6e63 6572  g marginal uncer
+00014fd0: 7461 696e 7469 6573 206f 6620 7468 6520  tainties of the 
+00014fe0: 6060 4d41 505f 7468 6574 6160 600a 2020  ``MAP_theta``.  
+00014ff0: 2020 2020 2020 6172 6520 6573 7469 6d61        are estima
+00015000: 7465 6420 7669 6120 5769 6c6b 7327 2074  ted via Wilks' t
+00015010: 6865 6f72 656d 2061 6e64 2074 6865 2068  heorem and the h
+00015020: 6967 6865 7220 6465 7669 6174 696f 6e20  igher deviation 
+00015030: 6f66 2065 6163 6820 6573 7469 6d61 7465  of each estimate
+00015040: 6420 6060 4d41 505f 7468 6574 6160 6020  d ``MAP_theta`` 
+00015050: 6973 2069 6e74 6572 7072 6574 6564 0a20  is interpreted. 
+00015060: 2020 2020 2020 2061 7320 7379 6d6d 6574         as symmet
+00015070: 7269 6320 6572 726f 7220 626f 756e 642e  ric error bound.
+00015080: 2054 6865 2064 6576 6961 7469 6f6e 7320   The deviations 
+00015090: 6172 6520 7072 6f70 6167 6174 6564 2069  are propagated i
+000150a0: 6e20 7465 726d 7320 6f66 2065 7272 6f72  n terms of error
+000150b0: 2062 6f75 6e64 732e 0a20 2020 2020 2020   bounds..       
+000150c0: 2054 6865 2065 7272 6f72 2062 6f75 6e64   The error bound
+000150d0: 206f 6620 7468 6520 6669 7865 6420 706f   of the fixed po
+000150e0: 696e 7420 6573 7469 6d61 7465 2069 7320  int estimate is 
+000150f0: 6173 7375 6d65 6420 746f 2062 6520 6571  assumed to be eq
+00015100: 7561 6c20 746f 2061 2047 6175 7373 6961  ual to a Gaussia
+00015110: 6e20 3a6d 6174 683a 6033 5c73 6967 6d61  n :math:`3\sigma
+00015120: 6020 2d63 6f6e 6669 6465 6e63 650a 2020  ` -confidence.  
+00015130: 2020 2020 2020 6261 6e64 2e0a 2020 2020        band..    
+00015140: 2020 2020 5468 6520 6573 7469 6d61 7469      The estimati
+00015150: 6f6e 2074 656e 6473 2074 6f20 6265 2074  on tends to be t
+00015160: 6f6f 206f 7074 696d 6973 7469 632c 2069  oo optimistic, i
+00015170: 2e65 2e20 7468 6520 756e 6365 7274 6169  .e. the uncertai
+00015180: 6e74 7920 626f 756e 6473 2061 7265 2074  nty bounds are t
+00015190: 6f6f 206e 6172 726f 772e 2054 6865 204d  oo narrow. The M
+000151a0: 4150 2065 7374 696d 6174 696f 6e20 7465  AP estimation te
+000151b0: 6e64 730a 2020 2020 2020 2020 746f 2076  nds.        to v
+000151c0: 6172 7920 746f 2073 7472 6f6e 6720 666f  ary to strong fo
+000151d0: 7220 7375 6273 6571 7565 6e74 2077 696e  r subsequent win
+000151e0: 646f 7773 2e20 4974 2069 7320 6f6e 6c79  dows. It is only
+000151f0: 2075 7365 6675 6c20 696e 2074 6865 2076   useful in the v
+00015200: 6572 7920 7261 7265 2063 6173 6520 6f66  ery rare case of
+00015210: 2076 6572 7920 6869 6768 2061 6d6f 756e   very high amoun
+00015220: 7473 206f 660a 2020 2020 2020 2020 7374  ts of.        st
+00015230: 6174 696f 6e61 7279 2064 6174 6120 7065  ationary data pe
+00015240: 7220 7769 6e64 6f77 2e20 4974 2069 7320  r window. It is 
+00015250: 7265 636f 6d6d 656e 6465 6420 746f 2075  recommended to u
+00015260: 7365 2074 6865 2073 756d 6d61 7279 2073  se the summary s
+00015270: 7461 7469 7374 6963 7320 756e 6365 7274  tatistics uncert
+00015280: 6169 6e74 7920 6261 6e64 732e 0a0a 2020  ainty bands...  
+00015290: 2020 2020 2020 3a70 6172 616d 2070 7269        :param pri
+000152a0: 6e74 626f 6f6c 3a20 4465 7465 726d 696e  ntbool: Determin
+000152b0: 6573 2077 6865 7468 6572 2061 2064 6574  es whether a det
+000152c0: 6169 6c65 6420 6f75 7470 7574 2069 7320  ailed output is 
+000152d0: 7072 696e 7465 6420 6f72 206e 6f74 2e0a  printed or not..
+000152e0: 2020 2020 2020 2020 3a74 7970 6520 7072          :type pr
+000152f0: 696e 7462 6f6f 6c3a 2042 6f6f 6c65 616e  intbool: Boolean
+00015300: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00015310: 2020 2020 2020 6966 2070 7269 6e74 626f        if printbo
+00015320: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+00015330: 7072 696e 7428 275f 5f5f 5f5f 5f5f 5f5f  print('_________
+00015340: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00015350: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00015360: 5f5f 5f5f 5f27 290a 2020 2020 2020 2020  _____').        
+00015370: 2020 2020 7072 696e 7428 2743 6f6d 7075      print('Compu
+00015380: 7465 2073 796d 6d65 7472 6963 2073 6c6f  te symmetric slo
+00015390: 7065 2065 7272 6f72 206d 6172 6769 6e73  pe error margins
+000153a0: 2e27 290a 2020 2020 2020 2020 2020 2020  .').            
+000153b0: 7072 696e 7428 275f 5f5f 5f5f 5f5f 5f5f  print('_________
+000153c0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000153d0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+000153e0: 5f5f 5f5f 5f27 290a 2020 2020 2020 2020  _____').        
+000153f0: 7365 6c66 2e66 6978 6564 5f70 6f69 6e74  self.fixed_point
+00015400: 5f65 7374 696d 6174 6520 3d20 6e70 2e6d  _estimate = np.m
+00015410: 6561 6e28 7365 6c66 2e64 6174 615f 7769  ean(self.data_wi
+00015420: 6e64 6f77 290a 2020 2020 2020 2020 6461  ndow).        da
+00015430: 7461 5f77 696e 646f 775f 6572 726f 7220  ta_window_error 
+00015440: 3d20 6e70 2e73 7172 7428 312e 202f 2028  = np.sqrt(1. / (
+00015450: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
+00015460: 2e73 697a 6529 202a 206e 702e 7661 7228  .size) * np.var(
+00015470: 7365 6c66 2e64 6174 615f 7769 6e64 6f77  self.data_window
+00015480: 2929 202a 2032 2e35 3735 0a20 2020 2020  )) * 2.575.     
+00015490: 2020 2058 5f65 7272 6f72 5f62 6f75 6e64     X_error_bound
+000154a0: 203d 2061 6273 2832 202a 2073 656c 662e   = abs(2 * self.
+000154b0: 4d41 505f 7468 6574 615b 322c 2030 5d20  MAP_theta[2, 0] 
+000154c0: 2b20 3620 2a20 7365 6c66 2e66 6978 6564  + 6 * self.fixed
+000154d0: 5f70 6f69 6e74 5f65 7374 696d 6174 6520  _point_estimate 
+000154e0: 2a0a 2020 2020 2020 2020 2020 2020 2020  *.              
+000154f0: 2020 2020 2073 656c 662e 4d41 505f 7468       self.MAP_th
+00015500: 6574 615b 332c 2030 5d29 202a 2064 6174  eta[3, 0]) * dat
+00015510: 615f 7769 6e64 6f77 5f65 7272 6f72 0a20  a_window_error. 
+00015520: 2020 2020 2020 2073 656c 662e 4d41 505f         self.MAP_
+00015530: 736c 6f70 655f 6d61 7267 696e 203d 206e  slope_margin = n
+00015540: 702e 7a65 726f 7328 3229 0a20 2020 2020  p.zeros(2).     
+00015550: 2020 2074 6865 7461 5f65 7272 6f72 5f73     theta_error_s
+00015560: 6967 4c65 7665 6c31 203d 206e 702e 7a65  igLevel1 = np.ze
+00015570: 726f 7328 2873 656c 662e 6e64 696d 2c20  ros((self.ndim, 
+00015580: 3229 290a 2020 2020 2020 2020 7468 6574  2)).        thet
+00015590: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
+000155a0: 3220 3d20 6e70 2e7a 6572 6f73 2828 7365  2 = np.zeros((se
+000155b0: 6c66 2e6e 6469 6d2c 2032 2929 0a20 2020  lf.ndim, 2)).   
+000155c0: 2020 2020 2074 6865 7461 5f65 7272 6f72       theta_error
+000155d0: 5f73 6967 4c65 7665 6c31 5b3a 2c20 305d  _sigLevel1[:, 0]
+000155e0: 203d 2073 656c 662e 4d41 505f 4349 5b3a   = self.MAP_CI[:
+000155f0: 2c20 305d 0a20 2020 2020 2020 2074 6865  , 0].        the
+00015600: 7461 5f65 7272 6f72 5f73 6967 4c65 7665  ta_error_sigLeve
+00015610: 6c31 5b3a 2c20 315d 203d 2073 656c 662e  l1[:, 1] = self.
+00015620: 4d41 505f 4349 5b3a 2c20 315d 0a20 2020  MAP_CI[:, 1].   
+00015630: 2020 2020 2074 6865 7461 5f6d 6172 6769       theta_margi
+00015640: 6e31 203d 206e 702e 6d61 7869 6d75 6d28  n1 = np.maximum(
+00015650: 6e70 2e61 6273 6f6c 7574 6528 7468 6574  np.absolute(thet
+00015660: 615f 6572 726f 725f 7369 674c 6576 656c  a_error_sigLevel
+00015670: 315b 313a 2c20 305d 292c 2074 6865 7461  1[1:, 0]), theta
+00015680: 5f65 7272 6f72 5f73 6967 4c65 7665 6c31  _error_sigLevel1
+00015690: 5b31 3a2c 2031 5d29 0a20 2020 2020 2020  [1:, 1]).       
+000156a0: 2074 6865 7461 5f65 7272 6f72 5f73 6967   theta_error_sig
+000156b0: 4c65 7665 6c32 5b3a 2c20 305d 203d 2073  Level2[:, 0] = s
+000156c0: 656c 662e 4d41 505f 4349 5b3a 2c20 325d  elf.MAP_CI[:, 2]
+000156d0: 0a20 2020 2020 2020 2074 6865 7461 5f65  .        theta_e
+000156e0: 7272 6f72 5f73 6967 4c65 7665 6c32 5b3a  rror_sigLevel2[:
+000156f0: 2c20 315d 203d 2073 656c 662e 4d41 505f  , 1] = self.MAP_
+00015700: 4349 5b3a 2c20 335d 0a20 2020 2020 2020  CI[:, 3].       
+00015710: 2074 6865 7461 5f6d 6172 6769 6e32 203d   theta_margin2 =
+00015720: 206e 702e 6d61 7869 6d75 6d28 6e70 2e61   np.maximum(np.a
+00015730: 6273 6f6c 7574 6528 7468 6574 615f 6572  bsolute(theta_er
+00015740: 726f 725f 7369 674c 6576 656c 325b 313a  ror_sigLevel2[1:
+00015750: 2c20 305d 292c 2074 6865 7461 5f65 7272  , 0]), theta_err
+00015760: 6f72 5f73 6967 4c65 7665 6c32 5b31 3a2c  or_sigLevel2[1:,
+00015770: 2031 5d29 0a20 2020 2020 2020 2070 6172   1]).        par
+00015780: 616d 315f 6d61 7267 696e 203d 2031 202a  am1_margin = 1 *
+00015790: 2074 6865 7461 5f6d 6172 6769 6e31 5b30   theta_margin1[0
+000157a0: 5d0a 2020 2020 2020 2020 7061 7261 6d32  ].        param2
+000157b0: 5f6d 6172 6769 6e20 3d20 3220 2a20 6e70  _margin = 2 * np
+000157c0: 2e61 6273 6f6c 7574 6528 7365 6c66 2e66  .absolute(self.f
+000157d0: 6978 6564 5f70 6f69 6e74 5f65 7374 696d  ixed_point_estim
+000157e0: 6174 6529 202a 2074 6865 7461 5f6d 6172  ate) * theta_mar
+000157f0: 6769 6e31 5b31 5d0a 2020 2020 2020 2020  gin1[1].        
+00015800: 7061 7261 6d33 5f6d 6172 6769 6e20 3d20  param3_margin = 
+00015810: 3320 2a20 7365 6c66 2e66 6978 6564 5f70  3 * self.fixed_p
+00015820: 6f69 6e74 5f65 7374 696d 6174 6520 2a2a  oint_estimate **
+00015830: 2032 202a 2074 6865 7461 5f6d 6172 6769   2 * theta_margi
+00015840: 6e31 5b32 5d0a 2020 2020 2020 2020 7365  n1[2].        se
+00015850: 6c66 2e4d 4150 5f73 6c6f 7065 5f6d 6172  lf.MAP_slope_mar
+00015860: 6769 6e5b 305d 203d 2070 6172 616d 315f  gin[0] = param1_
+00015870: 6d61 7267 696e 202b 2070 6172 616d 325f  margin + param2_
+00015880: 6d61 7267 696e 202b 2070 6172 616d 335f  margin + param3_
+00015890: 6d61 7267 696e 202b 2058 5f65 7272 6f72  margin + X_error
+000158a0: 5f62 6f75 6e64 0a20 2020 2020 2020 2070  _bound.        p
+000158b0: 6172 616d 315f 6d61 7267 696e 203d 2031  aram1_margin = 1
+000158c0: 202a 2074 6865 7461 5f6d 6172 6769 6e32   * theta_margin2
+000158d0: 5b30 5d0a 2020 2020 2020 2020 7061 7261  [0].        para
+000158e0: 6d32 5f6d 6172 6769 6e20 3d20 3220 2a20  m2_margin = 2 * 
+000158f0: 6e70 2e61 6273 6f6c 7574 6528 7365 6c66  np.absolute(self
+00015900: 2e66 6978 6564 5f70 6f69 6e74 5f65 7374  .fixed_point_est
+00015910: 696d 6174 6529 202a 2074 6865 7461 5f6d  imate) * theta_m
+00015920: 6172 6769 6e32 5b31 5d0a 2020 2020 2020  argin2[1].      
+00015930: 2020 7061 7261 6d33 5f6d 6172 6769 6e20    param3_margin 
+00015940: 3d20 3320 2a20 7365 6c66 2e66 6978 6564  = 3 * self.fixed
+00015950: 5f70 6f69 6e74 5f65 7374 696d 6174 6520  _point_estimate 
+00015960: 2a2a 2032 202a 2074 6865 7461 5f6d 6172  ** 2 * theta_mar
+00015970: 6769 6e32 5b32 5d0a 2020 2020 2020 2020  gin2[2].        
+00015980: 7365 6c66 2e4d 4150 5f73 6c6f 7065 5f6d  self.MAP_slope_m
+00015990: 6172 6769 6e5b 315d 203d 2070 6172 616d  argin[1] = param
+000159a0: 315f 6d61 7267 696e 202b 2070 6172 616d  1_margin + param
+000159b0: 325f 6d61 7267 696e 202b 2070 6172 616d  2_margin + param
+000159c0: 335f 6d61 7267 696e 202b 2058 5f65 7272  3_margin + X_err
+000159d0: 6f72 5f62 6f75 6e64 0a20 2020 2020 2020  or_bound.       
+000159e0: 2073 656c 662e 6472 6966 745f 736c 6f70   self.drift_slop
+000159f0: 655b 315d 203d 2073 656c 662e 6472 6966  e[1] = self.drif
+00015a00: 745f 736c 6f70 655b 305d 202d 2073 656c  t_slope[0] - sel
+00015a10: 662e 4d41 505f 736c 6f70 655f 6d61 7267  f.MAP_slope_marg
+00015a20: 696e 5b30 5d0a 2020 2020 2020 2020 7365  in[0].        se
+00015a30: 6c66 2e64 7269 6674 5f73 6c6f 7065 5b32  lf.drift_slope[2
+00015a40: 5d20 3d20 7365 6c66 2e64 7269 6674 5f73  ] = self.drift_s
+00015a50: 6c6f 7065 5b30 5d20 2b20 7365 6c66 2e4d  lope[0] + self.M
+00015a60: 4150 5f73 6c6f 7065 5f6d 6172 6769 6e5b  AP_slope_margin[
+00015a70: 305d 0a20 2020 2020 2020 2073 656c 662e  0].        self.
+00015a80: 6472 6966 745f 736c 6f70 655b 335d 203d  drift_slope[3] =
+00015a90: 2073 656c 662e 6472 6966 745f 736c 6f70   self.drift_slop
+00015aa0: 655b 305d 202d 2073 656c 662e 4d41 505f  e[0] - self.MAP_
+00015ab0: 736c 6f70 655f 6d61 7267 696e 5b31 5d0a  slope_margin[1].
+00015ac0: 2020 2020 2020 2020 7365 6c66 2e64 7269          self.dri
+00015ad0: 6674 5f73 6c6f 7065 5b34 5d20 3d20 7365  ft_slope[4] = se
+00015ae0: 6c66 2e64 7269 6674 5f73 6c6f 7065 5b30  lf.drift_slope[0
+00015af0: 5d20 2b20 7365 6c66 2e4d 4150 5f73 6c6f  ] + self.MAP_slo
+00015b00: 7065 5f6d 6172 6769 6e5b 315d 0a20 2020  pe_margin[1].   
+00015b10: 2020 2020 2069 6620 7072 696e 7462 6f6f       if printboo
+00015b20: 6c3a 0a20 2020 2020 2020 2020 2020 2070  l:.            p
+00015b30: 7269 6e74 2827 4d41 505f 736c 6f70 655f  rint('MAP_slope_
+00015b40: 6d61 7267 696e 3a20 272c 2073 656c 662e  margin: ', self.
+00015b50: 4d41 505f 736c 6f70 655f 6d61 7267 696e  MAP_slope_margin
+00015b60: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00015b70: 696e 7428 2764 7269 6674 5f73 6c6f 7065  int('drift_slope
+00015b80: 2061 7272 6179 3a20 272c 2073 656c 662e   array: ', self.
+00015b90: 6472 6966 745f 736c 6f70 6529 0a20 2020  drift_slope).   
+00015ba0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00015bb0: 5f5f 5f5f 5f27 290a 2020 2020 2020 2020  _____').        
+00015bc0: 2020 2020 7072 696e 7428 2744 6f6e 6521      print('Done!
+00015bd0: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
+00015be0: 7269 6e74 2827 5f5f 5f5f 5f27 29         rint('_____')
```

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/non_markov_estimation.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/non_markov_estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
         :param noise_grid: Array on which the noise level :math:`\hat{\psi}` kernel density estimate is evaluated.
         :type noise_grid: One-dimensional numpy array of floats.
         :param OU_grid: Array on which the Ornstein Uhlenbeck (OU) parameter's kernel density estimate is evaluated.
         :type OU_grid: One-dimensional numpy array of floats.
         :param X_coupling_grid: Array on which the X coupling strength kernel density estimate is evaluated.
         :type X_coupling_grid: One-dimensional numpy array of floats.
         :param nburn: Number of data points at the beginning of the Markov chains which are discarded in terms of
-                        a burn in period. Usually the defaul is 200, set by the `perform_resilience_scan` method.
+                        a burn in period. Usually the default is 200, set by the `perform_resilience_scan` method.
         :type nburn: int
         :param n_joint_samples: Number of joint samples that are drawn from the estimated joint posterior
                         probability in order to calculate the drift slope estimate :math:`\zeta` and
                         corresponding credibility bands. Default is 50000.
         :type n_joint_samples: int
         :param n_slope_samples: Number of drift slope samples that are drawn from the estimated drift slope
                         posterior computed based on the sampling results of the joint posterior probability
@@ -841,16 +841,16 @@
             self.data_window, self.slow_trend = self.detrend(self.time_window, self.data_window,
                                                                   detrending_per_window, gauss_filter_mode,
                                                                   gauss_filter_sigma,gauss_filter_order,
                                                                   gauss_filter_cval, gauss_filter_truncate,
                                                                   plot_detrending)
         self._prepare_data(printbool=print_details)
         self.declare_MAP_starting_guesses(print_time_scale_info=print_time_scale_info)
-        self.compute_posterior_samples(print_AC_tau=print_AC_tau, ignore_AC_error=ignore_AC_error, nburn = nburn,
-                                       thinning_by=thinning_by, print_progress=print_progress,
+        self.compute_posterior_samples(print_AC_tau=print_AC_tau, ignore_AC_error=ignore_AC_error,
+                                       thinning_by=thinning_by, print_progress=print_progress, nburn = nburn,
                                        MCMC_parallelization_method=MCMC_parallelization_method,
                                        num_processes=num_processes, num_chop_chains=num_chop_chains,
                                        MCMC_AC_estimate=MCMC_AC_estimate)
         if self.drift_model == '3rd order polynomial' or self.drift_model == '3rd order odds correlated':
             self.joint_kernel_density_obj = cpy.gaussian_kde(self.theta_array, bw_method='silverman')
             self.joint_samples = self.joint_kernel_density_obj.resample(size=n_joint_samples)
             self.third_order_polynom_slope_in_fixed_point()
```

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/rocket_fast_resilience_estimation.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/rocket_fast_resilience_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,27 @@
                              MCMC_AC_estimate='standard', cred_percentiles=np.array([16, 1]), print_AC_tau=False, ignore_AC_error=False,
                              thinning_by=60, print_progress=False, print_details=False, print_time_scale_info = False, slope_save_name='default_save_slopes',
                              noise_level_save_name='default_save_noise', OU_param_save_name = 'default_save_OUparam',
                              X_coupling_save_name = 'default_save_Xcoupling', num_processes=None, save=True):
         """
         The function's structure to use is almost equivalent to ``perform_resilience_scan`` of the ``LangevinEstimation`` and the
         ``NonMarkovEstimation`` class. It initializes a multiprocessing pool to calculate several rolling windows simultaneously.
+
+        :param window_shift: The parameter can differ from the basic integer definition known from the ``LangevinEstimation`` and the
+                            ``NonMarkovEstimation`` classes. If a one-dimensional numpy array is given instead, its entries are
+                            interpreted as specific ``window_shift`` for the parallel workers. In that case only these explicitly
+                            given shifts are used to determine the estimates of the corresponding windows.
+        :type window_shift: int or one-dimensional numpy array.
         """
         self.window_size = window_size
-        self.window_shift = window_shift
-        self.loop_range = np.arange(0, self.data_size - self.window_size, self.window_shift, dtype=int)
+        if isinstance(window_shift, int):
+            self.window_shift = window_shift
+            self.loop_range = np.arange(0, self.data_size - self.window_size, self.window_shift, dtype=int)
+        elif window_shift.size != 1:
+            self.loop_range = np.array(window_shift)
         loop_range_size = self.loop_range.size
         self.slope_storage = mp.RawArray('d', 5 * loop_range_size)
         self.noise_level_storage = mp.RawArray('d', 5 * loop_range_size)
         self.data_window = np.zeros(window_size)
         self.time_window = np.zeros(window_size)
         self.increments = np.zeros(window_size - 1)
         self.nwalkers = nwalkers
```

### Comparing `antiCPy-0.0.8/antiCPy/early_warnings/drift_slope/summary_statistics_helper.py` & `antiCPy-0.0.8.post1/antiCPy/early_warnings/drift_slope/summary_statistics_helper.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_configs_helper/create_configs_helper.py` & `antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_configs_helper/create_configs_helper.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/trend_extrapolation/batched_cp_segment_fit.py` & `antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/batched_cp_segment_fit.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy/trend_extrapolation/cp_segment_fit.py` & `antiCPy-0.0.8.post1/antiCPy/trend_extrapolation/cp_segment_fit.py`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/antiCPy.egg-info/PKG-INFO` & `antiCPy-0.0.8.post1/antiCPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antiCPy
-Version: 0.0.8
+Version: 0.0.8.post1
 Summary: A package that provides tools to estimate resilience and noise level of a system as well as extrapolate possible transition times.
 Home-page: https://github.com/MartinHessler/antiCPy
 Author: Martin Heßler
 Author-email: m_hess23@wwu.de
 License: GPL
 Keywords: time series analysis,critical transitions,leading indicators
 Platform: any
```

### Comparing `antiCPy-0.0.8/antiCPy.egg-info/SOURCES.txt` & `antiCPy-0.0.8.post1/antiCPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antiCPy-0.0.8/setup.py` & `antiCPy-0.0.8.post1/setup.py`

 * *Files identical despite different names*

