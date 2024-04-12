# Comparing `tmp/dmri-commit-2.1.0.tar.gz` & `tmp/dmri-commit-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmri-commit-2.1.0.tar", last modified: Mon Jan 22 14:02:24 2024, max compression
+gzip compressed data, was "dmri-commit-2.2.0.tar", last modified: Fri Apr 12 14:59:34 2024, max compression
```

## Comparing `dmri-commit-2.1.0.tar` & `dmri-commit-2.2.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.766777 dmri-commit-2.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     4414 2023-12-06 11:14:27.000000 dmri-commit-2.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      154 2020-12-18 15:38:06.000000 dmri-commit-2.1.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1895 2024-01-22 14:02:24.766683 dmri-commit-2.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3829 2022-05-05 07:31:32.000000 dmri-commit-2.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.707767 dmri-commit-2.1.0/build/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.766256 dmri-commit-2.1.0/build/dmri_commit.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1895 2024-01-22 14:02:24.000000 dmri-commit-2.1.0/build/dmri_commit.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      759 2024-01-22 14:02:24.000000 dmri-commit-2.1.0/build/dmri_commit.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-01-22 14:02:24.000000 dmri-commit-2.1.0/build/dmri_commit.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      101 2024-01-22 14:02:24.000000 dmri-commit-2.1.0/build/dmri_commit.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2024-01-22 14:02:24.000000 dmri-commit-2.1.0/build/dmri_commit.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.745197 dmri-commit-2.1.0/commit/
--rwxrwxrwx   0 root         (0) root         (0)      120 2022-05-05 07:31:32.000000 dmri-commit-2.1.0/commit/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)  2459396 2023-08-03 07:16:07.000000 dmri-commit-2.1.0/commit/core.cpp
--rwxrwxrwx   0 root         (0) root         (0)    67239 2024-01-22 13:28:40.000000 dmri-commit-2.1.0/commit/core.pyx
--rwxrwxrwx   0 root         (0) root         (0)     2227 2024-01-22 10:47:10.000000 dmri-commit-2.1.0/commit/info.py
--rwxrwxrwx   0 root         (0) root         (0)     3084 2024-01-22 13:49:58.000000 dmri-commit-2.1.0/commit/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.747452 dmri-commit-2.1.0/commit/operator/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-12-18 15:38:06.000000 dmri-commit-2.1.0/commit/operator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-01-22 10:47:10.000000 dmri-commit-2.1.0/commit/operator/config.py
--rwxrwxrwx   0 root         (0) root         (0)     7030 2024-01-22 12:31:45.000000 dmri-commit-2.1.0/commit/operator/operator.pyx
--rwxrwxrwx   0 root         (0) root         (0)     1569 2024-01-22 10:47:10.000000 dmri-commit-2.1.0/commit/operator/operator.pyxbld
--rwxrwxrwx   0 root         (0) root         (0)     4367 2024-01-22 13:27:21.000000 dmri-commit-2.1.0/commit/operator/operator_noLUT.c
--rwxrwxrwx   0 root         (0) root         (0)    54731 2024-01-17 10:45:30.000000 dmri-commit-2.1.0/commit/operator/operator_withLUT.c
--rwxrwxrwx   0 root         (0) root         (0)     5580 2024-01-16 13:33:23.000000 dmri-commit-2.1.0/commit/proximals.pyx
--rwxrwxrwx   0 root         (0) root         (0)    14857 2024-01-22 10:47:10.000000 dmri-commit-2.1.0/commit/solvers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 14:02:24.765678 dmri-commit-2.1.0/commit/trk2dictionary/
--rwxrwxrwx   0 root         (0) root         (0)     1761 2023-09-14 13:16:19.000000 dmri-commit-2.1.0/commit/trk2dictionary/ProgressBar.h
--rwxrwxrwx   0 root         (0) root         (0)     1658 2023-12-06 11:14:27.000000 dmri-commit-2.1.0/commit/trk2dictionary/Vector.h
--rwxrwxrwx   0 root         (0) root         (0)  1349695 2023-08-03 07:16:09.000000 dmri-commit-2.1.0/commit/trk2dictionary/trk2dictionary.cpp
--rwxrwxrwx   0 root         (0) root         (0)    26846 2024-01-22 11:54:24.000000 dmri-commit-2.1.0/commit/trk2dictionary/trk2dictionary.pyx
--rwxrwxrwx   0 root         (0) root         (0)    32800 2024-01-22 12:08:00.000000 dmri-commit-2.1.0/commit/trk2dictionary/trk2dictionary_c.cpp
--rwxrwxrwx   0 root         (0) root         (0)      149 2024-01-22 14:02:24.767269 dmri-commit-2.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2838 2024-01-16 13:33:23.000000 dmri-commit-2.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.966951 dmri-commit-2.2.0/
+-rwxrwxrwx   0 root         (0) root         (0)     4414 2023-12-06 11:14:27.000000 dmri-commit-2.2.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      119 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)    10258 2024-04-12 14:59:34.966582 dmri-commit-2.2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3829 2022-05-05 07:31:32.000000 dmri-commit-2.2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.959551 dmri-commit-2.2.0/commit/
+-rwxrwxrwx   0 root         (0) root         (0)      252 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    92193 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/core.pyx
+-rwxrwxrwx   0 root         (0) root         (0)     3468 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.961647 dmri-commit-2.2.0/commit/operator/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-12-18 15:38:06.000000 dmri-commit-2.2.0/commit/operator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-10 08:28:40.000000 dmri-commit-2.2.0/commit/operator/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     7066 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/operator/operator.pyx
+-rwxrwxrwx   0 root         (0) root         (0)     1569 2024-04-10 08:28:40.000000 dmri-commit-2.2.0/commit/operator/operator.pyxbld
+-rwxrwxrwx   0 root         (0) root         (0)     4367 2024-04-10 08:28:40.000000 dmri-commit-2.2.0/commit/operator/operator_noLUT.c
+-rwxrwxrwx   0 root         (0) root         (0)    54731 2024-04-10 08:28:40.000000 dmri-commit-2.2.0/commit/operator/operator_withLUT.c
+-rwxrwxrwx   0 root         (0) root         (0)     5335 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/proximals.pyx
+-rwxrwxrwx   0 root         (0) root         (0)    17242 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/solvers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.963413 dmri-commit-2.2.0/commit/trk2dictionary/
+-rwxrwxrwx   0 root         (0) root         (0)     1761 2023-09-14 13:16:19.000000 dmri-commit-2.2.0/commit/trk2dictionary/ProgressBar.h
+-rwxrwxrwx   0 root         (0) root         (0)     1658 2023-12-06 11:14:27.000000 dmri-commit-2.2.0/commit/trk2dictionary/Vector.h
+-rwxrwxrwx   0 root         (0) root         (0)    30065 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/trk2dictionary/trk2dictionary.pyx
+-rwxrwxrwx   0 root         (0) root         (0)    32837 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/commit/trk2dictionary/trk2dictionary_c.cpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.966061 dmri-commit-2.2.0/dmri_commit.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    10258 2024-04-12 14:59:34.000000 dmri-commit-2.2.0/dmri_commit.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      671 2024-04-12 14:59:34.000000 dmri-commit-2.2.0/dmri_commit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-12 14:59:34.000000 dmri-commit-2.2.0/dmri_commit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       66 2024-04-12 14:59:34.000000 dmri-commit-2.2.0/dmri_commit.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2024-04-12 14:59:34.000000 dmri-commit-2.2.0/dmri_commit.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1670 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-12 14:59:34.967033 dmri-commit-2.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2178 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-12 14:59:34.965670 dmri-commit-2.2.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     6348 2024-04-12 14:56:53.000000 dmri-commit-2.2.0/tests/test_demo.py
```

### Comparing `dmri-commit-2.1.0/LICENSE` & `dmri-commit-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/README.md` & `dmri-commit-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/build/dmri_commit.egg-info/SOURCES.txt` & `dmri-commit-2.2.0/dmri_commit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
-./build/dmri_commit.egg-info/PKG-INFO
-./build/dmri_commit.egg-info/SOURCES.txt
-./build/dmri_commit.egg-info/dependency_links.txt
-./build/dmri_commit.egg-info/requires.txt
-./build/dmri_commit.egg-info/top_level.txt
 commit/__init__.py
-commit/core.cpp
 commit/core.pyx
-commit/info.py
 commit/models.py
 commit/proximals.pyx
 commit/solvers.py
 commit/operator/__init__.py
 commit/operator/config.py
 commit/operator/operator.pyx
 commit/operator/operator.pyxbld
 commit/operator/operator_noLUT.c
 commit/operator/operator_withLUT.c
 commit/trk2dictionary/ProgressBar.h
 commit/trk2dictionary/Vector.h
-commit/trk2dictionary/trk2dictionary.cpp
 commit/trk2dictionary/trk2dictionary.pyx
-commit/trk2dictionary/trk2dictionary_c.cpp
+commit/trk2dictionary/trk2dictionary_c.cpp
+dmri_commit.egg-info/PKG-INFO
+dmri_commit.egg-info/SOURCES.txt
+dmri_commit.egg-info/dependency_links.txt
+dmri_commit.egg-info/requires.txt
+dmri_commit.egg-info/top_level.txt
+tests/test_demo.py
```

### Comparing `dmri-commit-2.1.0/commit/models.py` & `dmri-commit-2.2.0/commit/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-import sys
+from Cython.Build.Inline import _get_build_extension
+from Cython.Build import cythonize
 from os import environ
 import os
-import pyximport
 from setuptools import Extension
-from Cython.Build.Inline import _get_build_extension
-from Cython.Build import cythonize
+import sys
+
 import numpy as np
+
 from amico.models import BaseModel, StickZeppelinBall as _StickZeppelinBall, CylinderZeppelinBall as _CylinderZeppelinBall
-from amico.util import ERROR
+import amico.util as util
+
+from dicelib.ui import setup_logger
+
+
+logger = setup_logger('models')
 
 try:
     sys.path.append(environ["WIP_MODEL"])
     extension = Extension(name='commitwipmodels',
                           language='c++',
                           sources=[os.environ['WIP_MODEL'] + '/commitwipmodels.pyx'],
                           extra_compile_args=['-w'])
@@ -40,22 +46,27 @@
     pass
 
 
 class StickZeppelinBall(_StickZeppelinBall):
     """Simulate the response functions according to the Stick-Zeppelin-Ball model.
     See the AMICO.model module for details.
     """
-    pass
+    def resample(self, in_path, idx_out, Ylm_out, doMergeB0, ndirs):
+        util.set_verbose(2)
+        return super().resample(in_path, idx_out, Ylm_out, doMergeB0, ndirs)
+
 
 
 class CylinderZeppelinBall(_CylinderZeppelinBall):
     """Simulate the response functions according to the Cylinder-Zeppelin-Ball model.
     See the AMICO.model module for details.
     """
-    pass
+    def resample(self, in_path, idx_out, Ylm_out, doMergeB0, ndirs):
+        util.set_verbose(2)
+        return super().resample(in_path, idx_out, Ylm_out, doMergeB0, ndirs)
 
 class VolumeFractions(BaseModel):
     """Implements a simple model where each compartment contributes only with
        its own volume fraction. This model has been created to test there
        ability to remove false positive fibers with COMMIT.
     """
     def __init__(self):
```

### Comparing `dmri-commit-2.1.0/commit/operator/operator.pyx` & `dmri-commit-2.2.0/commit/operator/operator.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 #cython: language_level=3, boundscheck=False, wraparound=False, profile=False
 
-import cython
 import numpy as np
-cimport numpy as np
+
+from dicelib.ui import setup_logger
 
 # Interfaces to actual C code performing the multiplications
 cdef extern void COMMIT_A(
     int _nF, int _n, int _nE, int _nV, int _nS, int _ndirs,
     double *_v_in, double *_v_out,
     unsigned int *_ICf, unsigned int *_ICv, unsigned short *_ICo, float *_ICl,
     unsigned int *_ECv, unsigned short *_ECo,
@@ -22,15 +22,15 @@
     unsigned int *_ICf, unsigned int *_ICv, unsigned short *_ICo, float *_ICl,
     unsigned int *_ECv, unsigned short *_ECo,
     unsigned int *_ISOv,
     float *_wmrSFP, float *_wmhSFP, float *_isoSFP,
     unsigned char *_ICthreadsT, unsigned int *_ECthreadsT, unsigned int *_ISOthreadsT
 ) nogil
 
-
+logger = setup_logger('operator')
 
 cdef class LinearOperator :
     """This class is a wrapper to the C code for performing marix-vector multiplications
     with the COMMIT linear operator A. The multiplications are done using C code
     that uses information from the DICTIONARY, KERNELS and THREADS data structures.
     """
     cdef int nS, nF, nR, nE, nT, nV, nI, n, ndirs
```

### Comparing `dmri-commit-2.1.0/commit/operator/operator.pyxbld` & `dmri-commit-2.2.0/commit/operator/operator.pyxbld`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/commit/operator/operator_noLUT.c` & `dmri-commit-2.2.0/commit/operator/operator_noLUT.c`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/commit/operator/operator_withLUT.c` & `dmri-commit-2.2.0/commit/operator/operator_withLUT.c`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/commit/proximals.pyx` & `dmri-commit-2.2.0/commit/proximals.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!python
 #cython: language_level=3, boundscheck=False, wraparound=False, profile=False
-cimport cython
-import numpy as np
-cimport numpy as np
+
 from libc.math cimport sqrt
 
+import numpy as np
+
+from dicelib.ui import setup_logger
+
+logger = setup_logger('proximals')
+
 
 cpdef non_negativity(double [::1] x, int compartment_start, int compartment_size):
     """
     POCS for the first orthant (non-negativity)
     """
     cdef:
         int i
@@ -22,18 +26,14 @@
     """
     Proximal of L1 norm
     """
     # NB: this preserves non-negativity
     cdef:
         int i
     for i in xrange(compartment_start, compartment_start+compartment_size):
-        # if x[i] <= lam:
-        #     x[i] = 0.0
-        # else:
-        #     x[i] = x[i] - lam
         if x[i] > lam:
             x[i] = x[i] - lam
         elif x[i] < -lam:
             x[i] = x[i] + lam
         else:
             x[i] = 0.0
     return np.asarray( x )
@@ -43,18 +43,14 @@
     """
     Proximal of weighted L1 norm
     """
     # NB: this preserves non-negativity
     cdef:
         int i
     for i in xrange(compartment_start, compartment_start+compartment_size):
-        # if x[i] <= lam:
-        #     x[i] = 0.0
-        # else:
-        #     x[i] = x[i] - lam
         if x[i] > w[i]*lam:
             x[i] = x[i] - w[i]*lam
         elif x[i] < -w[i]*lam:
             x[i] = x[i] + w[i]*lam
         else:
             x[i] = 0.0
     return np.asarray( x )
@@ -113,19 +109,14 @@
         int nG = group_size.size
         int N = 0
         int k = 0
         int i = 0
         int j = 0
         double wl, gNorm, x_i
 
-    k = x.size
-    for i in xrange(k):
-        if x[i] <= 0.0:
-            x[i] = 0.0
-
     if lam != 0:
         for k in xrange(nG) :
             N = group_size[k]
             gNorm = 0.0
             for i in xrange(j,j+N) :
                 x_i = x[group_idx[i]]
                 gNorm += x_i*x_i
```

### Comparing `dmri-commit-2.1.0/commit/solvers.py` & `dmri-commit-2.2.0/commit/solvers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,204 @@
-import numpy as np
-from math import sqrt
 import sys
-eps = np.finfo(float).eps
 
+from math import sqrt
+
+import numpy as np
+
+from dicelib.ui import setup_logger
+
+logger = setup_logger('solvers')
+eps = np.finfo(float).eps
 list_regularizers = [None, 'lasso', 'group_lasso', 'sparse_group_lasso']
 from commit.proximals import non_negativity, omega_group_lasso, prox_group_lasso, soft_thresholding, w_soft_thresholding, omega_sparse_group_lasso, omega_w_sparse_group_lasso
 # removed, for now, projection_onto_l2_ball
 
 
 def init_regularisation(regularisation_params):
     """
     Initialize the regularisation parameters.
 
     References:
         [1] Jenatton et al. - 'Proximal Methods for Hierarchical Sparse Coding'
     """
 
+    # check if regularisations are in the list
+    if regularisation_params['regIC'] not in list_regularizers or regularisation_params['regEC'] not in list_regularizers or regularisation_params['regISO'] not in list_regularizers:
+        logger.error('Regularisation not in the list')
+    
+    startIC  = regularisation_params.get('startIC')
+    sizeIC   = regularisation_params.get('sizeIC')
+    startEC  = regularisation_params.get('startEC')
+    sizeEC   = regularisation_params.get('sizeEC')
+    startISO = regularisation_params.get('startISO')
+    sizeISO  = regularisation_params.get('sizeISO')
+
+    # create array with al coeff_weights for weighted version of 'lasso'
+    all_coeff_weights = np.ones(sizeIC+sizeEC+sizeISO, dtype=np.float64)
+    if regularisation_params.get('dictIC_params') is not None and "coeff_weights" in regularisation_params['dictIC_params'].keys():
+        all_coeff_weights[startIC:(startIC+sizeIC)] = regularisation_params['dictIC_params']["coeff_weights"]
+    if regularisation_params.get('dictEC_params') is not None and "coeff_weights" in regularisation_params['dictEC_params'].keys():
+        all_coeff_weights[startEC:(startEC+sizeEC)] = regularisation_params['dictEC_params']["coeff_weights"]
+    if regularisation_params.get('dictISO_params') is not None and "coeff_weights" in regularisation_params['dictISO_params'].keys():
+        all_coeff_weights[startISO:(startISO+sizeISO)] = regularisation_params['dictISO_params']["coeff_weights"]
+
     ############################
     # INTRACELLULAR COMPARTMENT#
     ############################
 
-    # check if regularisations are in the list
-    if regularisation_params['regIC'] not in list_regularizers or regularisation_params['regEC'] not in list_regularizers or regularisation_params['regISO'] not in list_regularizers:
-        raise ValueError('Regularisation not in the list')
-
-    startIC = regularisation_params.get('startIC')
-    sizeIC = regularisation_params.get('sizeIC')
     dictIC_params = regularisation_params.get('dictIC_params')
 
     if regularisation_params['regIC'] is None:
         omegaIC = lambda x: 0.0
         if regularisation_params.get('nnIC')==True:
             proxIC = lambda x, _: non_negativity(x,startIC,sizeIC)
         else:
             proxIC = lambda x, _: x
 
     elif regularisation_params['regIC'] == 'lasso':
         lambdaIC = regularisation_params['lambdaIC']
         # check if weights are provided
-        if dictIC_params is not None:
-            if "weightsIC" in dictIC_params.keys():
-                w = dictIC_params["weightsIC"]
-                omegaIC = lambda x: lambdaIC * np.linalg.norm(w[startIC:sizeIC]*x[startIC:sizeIC],1)
-                if regularisation_params.get('nnIC'):
-                    proxIC = lambda x, scaling: non_negativity(w_soft_thresholding(x,w,scaling*lambdaIC,startIC,sizeIC),startIC,sizeIC)
-                else:
-                    proxIC = lambda x, _: non_negativity(x,startIC,sizeIC)
+        if dictIC_params is not None and "coeff_weights" in dictIC_params.keys():
+            # w = dictIC_params["coeff_weights"]
+            omegaIC = lambda x: lambdaIC * np.linalg.norm(all_coeff_weights[startIC:sizeIC]*x[startIC:sizeIC],1)
+            if regularisation_params.get('nnIC'):
+                proxIC = lambda x, scaling: non_negativity(w_soft_thresholding(x,all_coeff_weights,scaling*lambdaIC,startIC,sizeIC),startIC,sizeIC)
+            else:
+                proxIC = lambda x, scaling: w_soft_thresholding(x,all_coeff_weights,scaling*lambdaIC,startIC,sizeIC)
         else:
             omegaIC = lambda x: lambdaIC * np.linalg.norm(x[startIC:sizeIC],1)
             if regularisation_params.get('nnIC'):
                 proxIC = lambda x, scaling: non_negativity(soft_thresholding(x,scaling*lambdaIC,startIC,sizeIC),startIC,sizeIC)
             else:
-                proxIC = lambda x, _: non_negativity(x,startIC,sizeIC)
-
+                proxIC = lambda x, scaling: soft_thresholding(x,scaling*lambdaIC,startIC,sizeIC)
 
     # elif regularisation_params['regIC'] == 'smoothness':
     #     lambdaIC = regularisation_params.get('lambdaIC')
     #     omegaIC = lambda x: lambdaIC * np.linalg.norm(x[startIC:sizeIC])
     #     proxIC  = lambda x: projection_onto_l2_ball(x, lambdaIC, startIC, sizeIC)
 
     elif regularisation_params['regIC'] == 'group_lasso':
         if not len(dictIC_params["group_idx"]) == len(dictIC_params['group_weights']):
-            raise ValueError('Number of groups and weights do not match')
+            logger.error('Number of groups and weights do not match')
 
         lambda_group_IC = regularisation_params['lambdaIC']
 
         # convert to new data structure (needed for faster access)
         N = np.sum([g.size for g in dictIC_params["group_idx"]])
         groupIdxIC = np.zeros( (N,), dtype=np.int32 )
         groupSizeIC = np.zeros( (dictIC_params["group_idx"].size,), dtype=np.int32 )
         pos = 0
         for i, g in enumerate(dictIC_params["group_idx"]) :
             groupSizeIC[i] = g.size
             groupIdxIC[pos:(pos+g.size)] = g[:]
             pos += g.size
 
         omegaIC = lambda x: omega_group_lasso( x, groupIdxIC, groupSizeIC, dictIC_params['group_weights'], lambda_group_IC )
-        #TODO: verify if COMMIT2 results are better than before
         if regularisation_params.get('nnIC'):
             proxIC = lambda x, scaling: non_negativity(prox_group_lasso(x,groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC),startIC,sizeIC)
         else:
             proxIC = lambda x, scaling: prox_group_lasso(x,groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC)
   
     elif regularisation_params['regIC'] == 'sparse_group_lasso':
         if not len(dictIC_params["group_idx"]) == len(dictIC_params['group_weights']):
-            raise ValueError('Number of groups and weights do not match')
+            logger.error('Number of groups and weights do not match')
 
         lambdaIC = regularisation_params['lambdaIC'][0]
         lambda_group_IC = regularisation_params['lambdaIC'][1]
 
         # convert to new data structure (needed for faster access)
         N = np.sum([g.size for g in dictIC_params["group_idx"]])
         groupIdxIC  = np.zeros( (N,), dtype=np.int32 )
         groupSizeIC = np.zeros( (dictIC_params["group_idx"].size,), dtype=np.int32 )
         pos = 0
         for i, g in enumerate(dictIC_params["group_idx"]) :
             groupSizeIC[i] = g.size
             groupIdxIC[pos:(pos+g.size)] = g[:]
             pos += g.size
 
-        if "weightsIC" in dictIC_params.keys():
-            w = dictIC_params["weightsIC"]
-            omegaIC = lambda x: omega_w_sparse_group_lasso( x, w, groupIdxIC, groupSizeIC, dictIC_params['group_weights'], lambdaIC, lambda_group_IC)
+        if "coeff_weights" in dictIC_params.keys():
+            # w = dictIC_params["coeff_weights"]
+            omegaIC = lambda x: omega_w_sparse_group_lasso( x, all_coeff_weights, groupIdxIC, groupSizeIC, dictIC_params['group_weights'], lambdaIC, lambda_group_IC)
 
             if regularisation_params.get('nnIC'):
-                proxIC = lambda x, scaling: non_negativity(prox_group_lasso(w_soft_thresholding(x,w,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC), startIC,sizeIC)
+                proxIC = lambda x, scaling: non_negativity(prox_group_lasso(w_soft_thresholding(x,all_coeff_weights,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC), startIC,sizeIC)
             else:
-                proxIC = lambda x, scaling: prox_group_lasso(w_soft_thresholding(x,w,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC)
+                proxIC = lambda x, scaling: prox_group_lasso(w_soft_thresholding(x,all_coeff_weights,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC)
         else:
             omegaIC = lambda x: omega_sparse_group_lasso( x, groupIdxIC, groupSizeIC, dictIC_params['group_weights'], lambdaIC, lambda_group_IC)
 
             if regularisation_params.get('nnIC'):
                 proxIC = lambda x, scaling: non_negativity(prox_group_lasso(soft_thresholding(x,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC), startIC,sizeIC)
             else:
                 proxIC = lambda x, scaling: prox_group_lasso(soft_thresholding(x,scaling*lambdaIC,startIC,sizeIC),groupIdxIC,groupSizeIC,dictIC_params['group_weights'],scaling*lambda_group_IC)
 
 
     ###########################
     # EXTRCELLULAR COMPARTMENT#
     ###########################
 
-    startEC = regularisation_params.get('startEC')
-    sizeEC  = regularisation_params.get('sizeEC')
+    dictEC_params = regularisation_params.get('dictEC_params')
 
     if regularisation_params['regEC'] is None:
         omegaEC = lambda x: 0.0
         if regularisation_params.get('nnEC')==True:
             proxEC = lambda x, _: non_negativity(x,startEC,sizeEC)
         else:
             proxEC = lambda x, _: x
 
     elif regularisation_params['regEC'] == 'lasso':
         lambdaEC = regularisation_params.get('lambdaEC')
-        omegaEC = lambda x: lambdaEC * np.linalg.norm(x[startEC:(startEC+sizeEC)],1)
-        if regularisation_params.get('nnEC'):
-            proxEC = lambda x, scaling: non_negativity(soft_thresholding(x,scaling*lambdaEC,startEC,sizeEC),startEC,sizeEC)
+        # check if weights are provided
+        if dictEC_params is not None and "coeff_weights" in dictEC_params.keys():
+            omegaEC = lambda x: lambdaEC * np.linalg.norm(all_coeff_weights[startEC:sizeEC]*x[startEC:sizeEC],1)
+            if regularisation_params.get('nnEC'):
+                proxEC = lambda x, scaling: non_negativity(w_soft_thresholding(x,all_coeff_weights,scaling*lambdaEC,startEC,sizeEC),startEC,sizeEC)
+            else:
+                proxEC = lambda x, scaling: w_soft_thresholding(x,all_coeff_weights,scaling*lambdaEC,startEC,sizeEC)
         else:
-            proxEC = lambda x, scaling: soft_thresholding(x,scaling*lambdaEC,startEC,sizeEC)
+            omegaEC = lambda x: lambdaEC * np.linalg.norm(x[startEC:(startEC+sizeEC)],1)
+            if regularisation_params.get('nnEC'):
+                proxEC = lambda x, scaling: non_negativity(soft_thresholding(x,scaling*lambdaEC,startEC,sizeEC),startEC,sizeEC)
+            else:
+                proxEC = lambda x, scaling: soft_thresholding(x,scaling*lambdaEC,startEC,sizeEC)
 
     # elif regularisation_params['regIC'] == 'smoothness':
     #     lambdaEC = regularisation_params.get('lambdaEC')
     #     omegaEC = lambda x: lambdaEC * np.linalg.norm(x[startEC:(startEC+sizeEC)])
     #     proxEC  = lambda x: projection_onto_l2_ball(x, lambdaEC, startEC, sizeEC)
 
+
     ########################
     # ISOTROPIC COMPARTMENT#
     ########################
 
-    startISO = regularisation_params.get('startISO')
-    sizeISO  = regularisation_params.get('sizeISO')
+    dictISO_params = regularisation_params.get('dictISO_params')
 
     if regularisation_params['regISO'] is None:
         omegaISO = lambda x: 0.0
         if regularisation_params.get('nnISO')==True:
             proxISO = lambda x, _: non_negativity(x,startISO,sizeISO)
         else:
             proxISO  = lambda x, _: x
 
     elif regularisation_params['regISO'] == 'lasso':
         lambdaISO = regularisation_params.get('lambdaISO')
-        omegaISO = lambda x: lambdaISO * np.linalg.norm(x[startISO:(startISO+sizeISO)],1)
-        if regularisation_params.get('nnISO'):
-            proxISO  = lambda x, scaling: non_negativity(soft_thresholding(x,scaling*lambdaISO,startISO,sizeISO),startISO,sizeISO)
+        # check if weights are provided
+        if dictISO_params is not None and "coeff_weights" in dictISO_params.keys():
+            omegaISO = lambda x: lambdaISO * np.linalg.norm(all_coeff_weights[startISO:sizeISO]*x[startISO:sizeISO],1)
+            if regularisation_params.get('nnISO'):
+                proxISO = lambda x, scaling: non_negativity(w_soft_thresholding(x,all_coeff_weights,scaling*lambdaISO,startISO,sizeISO),startISO,sizeISO)
+            else:
+                proxISO = lambda x, scaling: w_soft_thresholding(x,all_coeff_weights,scaling*lambdaISO,startISO,sizeISO)
         else:
-            proxISO  = lambda x, scaling: soft_thresholding(x,scaling*lambdaISO,startISO,sizeISO)
+            omegaISO = lambda x: lambdaISO * np.linalg.norm(x[startISO:(startISO+sizeISO)],1)
+            if regularisation_params.get('nnISO'):
+                proxISO  = lambda x, scaling: non_negativity(soft_thresholding(x,scaling*lambdaISO,startISO,sizeISO),startISO,sizeISO)
+            else:
+                proxISO  = lambda x, scaling: soft_thresholding(x,scaling*lambdaISO,startISO,sizeISO)
 
     # elif regularisation_params['regISO'] == 'group_lasso':
     #     lambdaISO = regularisation_params.get('lambdaISO')
     #     omegaISO = lambda x: lambdaISO * np.linalg.norm(x[startISO:(startISO+sizeISO)])
     #     proxISO  = lambda x: projection_onto_l2_ball(x, lambdaISO, startISO, sizeISO)
 
     omega = lambda x: omegaIC(x) + omegaEC(x) + omegaISO(x)
@@ -184,15 +215,15 @@
         omega = lambda x: 0.0
     else:
         omega, _ = init_regularisation(regularisation)
 
     return 0.5*np.linalg.norm(A.dot(x)-y)**2 + omega(x)
 
 
-def solve(y, A, At, tol_fun=1e-4, tol_x=1e-6, max_iter=1000, verbose=True, x0=None, regularisation=None, confidence_array=None):
+def solve(y, A, At, tol_fun=1e-4, tol_x=1e-6, max_iter=1000, verbose=True, x0  =None, regularisation=None, confidence_array=None):
     """
     Solve the regularised least squares problem
 
         argmin_x 0.5*|| sqrt(W) ( Ax-y ) ||_2^2 + Omega(x)
 
     with the Omega described by 'regularisation' and W is the confidence_array
 
@@ -254,21 +285,21 @@
     # Step size computation
     if sqrt_W is not None:
         L = ( np.linalg.norm( sqrt_W * A.dot(grad) ) / np.linalg.norm(grad) )**2
     else:
         L = ( np.linalg.norm( A.dot(grad) ) / np.linalg.norm(grad) )**2
     step_size = 1.9 / L
     # Main loop
-    if verbose :
+    if verbose==4 :
         print()
         print( "      |  1/2||Ax-y||^2      Omega      |  Cost function    Abs error      Rel error    |      Abs x          Rel x    " )
         print( "------|--------------------------------|-----------------------------------------------|------------------------------" )
     iter = 1
     while True :
-        if verbose :
+        if verbose==4 :
             print( "%4d  |" % iter, end="" )
             sys.stdout.flush()
 
         # Smooth step
         x = xhat - step_size*grad
 
         # Non-smooth step
@@ -305,15 +336,15 @@
             curr_obj = 0.5 * res_norm**2 + reg_term_x
 
         # Global stopping criterion
         abs_obj = abs(curr_obj - prev_obj)
         rel_obj = abs_obj / curr_obj
         abs_x   = np.linalg.norm(x - prev_x)
         rel_x   = abs_x / ( np.linalg.norm(x) + eps )
-        if verbose :
+        if verbose==4 :
             print( "  %13.7e  %13.7e  |  %13.7e  %13.7e  %13.7e  |  %13.7e  %13.7e" % ( 0.5 * res_norm**2, reg_term_x, curr_obj, abs_obj, rel_obj, abs_x, rel_x ) )
 
         if abs_obj < eps :
             criterion = "Absolute tolerance on the objective"
             break
         elif rel_obj < tol_fun :
             criterion = "Relative tolerance on the objective"
@@ -343,22 +374,22 @@
         # Update variables
         iter += 1
         prev_obj = curr_obj
         prev_x = x.copy()
         told = t
         qfval = 0.5 * np.linalg.norm(res)**2
 
-    if verbose :
+    if verbose==4 :
         print( "< Stopping criterion: %s >" % criterion )
 
     opt_details = {}
     opt_details['residual'] = 0.5*res_norm**2
     opt_details['regterm'] = reg_term_x
     opt_details['cost_function'] = curr_obj
     opt_details['abs_cost'] = abs_obj
     opt_details['rel_cost'] = rel_obj
     opt_details['abs_x'] = abs_x
-    opt_details['rel _x'] = rel_x
+    opt_details['rel_x'] = rel_x
     opt_details['iterations'] = iter
     opt_details['stopping_criterion'] = criterion
 
     return x, opt_details
```

### Comparing `dmri-commit-2.1.0/commit/trk2dictionary/ProgressBar.h` & `dmri-commit-2.2.0/commit/trk2dictionary/ProgressBar.h`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/commit/trk2dictionary/Vector.h` & `dmri-commit-2.2.0/commit/trk2dictionary/Vector.h`

 * *Files identical despite different names*

### Comparing `dmri-commit-2.1.0/commit/trk2dictionary/trk2dictionary.pyx` & `dmri-commit-2.2.0/commit/trk2dictionary/trk2dictionary.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 #!python
 # cython: language_level=3, c_string_type=str, c_string_encoding=ascii, boundscheck=False, wraparound=False, profile=False
-import numpy as np
-cimport numpy as np
+
 from libc.stdlib cimport malloc, free
+from libcpp cimport bool
+cimport numpy as np
+
 import nibabel
-from dicelib.clustering import run_clustering
-from dicelib.ui import _in_notebook
+import numpy as np
 
 import os
 from os.path import join, exists, splitext, dirname, isdir, isfile
 from os import makedirs, remove
-import time
+
 import amico
+
+from dicelib.clustering import run_clustering
+from dicelib.ui import _in_notebook
+from dicelib.ui import ProgressBar, setup_logger
+from dicelib import ui
+from dicelib.utils import format_time
+
 import pickle
-from amico.util import LOG, NOTE, WARNING, ERROR
+
 from pkg_resources import get_distribution
+
 import shutil
 
-from libcpp cimport bool
+import time
+
+ 
+logger = setup_logger('trk2dictionary')
 
 # Interface to actual C code
 cdef extern from "trk2dictionary_c.cpp":
     int trk2dictionary(
         char* filename_tractogram, int data_offset, int Nx, int Ny, int Nz, float Px, float Py, float Pz, int n_count, int n_scalars,
         int n_properties, float fiber_shiftX, float fiber_shiftY, float fiber_shiftZ, float min_seg_len, float min_fiber_len,  float max_fiber_len,
         float* ptrPEAKS, int Np, float vf_THR, int ECix, int ECiy, int ECiz,
@@ -40,28 +52,32 @@
     """ Concatenate binary file """
     with open( outfilename, "wb" ) as outfile:
         for fname in infilename:
             with open( fname, 'rb' ) as inFile:
                 shutil.copyfileobj( inFile, outfile )
                 remove( fname )
 
-cpdef compute_tdi( np.uint32_t[::1] v, np.float32_t[::1] l, int nx, int ny, int nz ):
+cpdef compute_tdi( np.uint32_t[::1] v, np.float32_t[::1] l, int nx, int ny, int nz, int verbose):
     cdef np.float32_t [::1] tdi = np.zeros( nx*ny*nz, dtype=np.float32 )
-    cdef int i
-    for i in xrange(v.size):
-        tdi[ v[i] ] += l[i]
+    cdef unsigned long long i=0
+    with ProgressBar(total=v.size, disable=(verbose in [0, 1, 3]), hide_on_exit=True) as pbar:
+
+        for i in range(v.size):
+            tdi[ v[i] ] += l[i]
+            pbar.update()
+
     return tdi
 
 
 cpdef run( filename_tractogram=None, path_out=None, filename_peaks=None, filename_mask=None, filename_ISO=None,
             do_intersect=True, fiber_shift=0, min_seg_len=1e-3, min_fiber_len=0.0, max_fiber_len=250.0,
             vf_THR=0.1, peaks_use_affine=False, flip_peaks=[False,False,False], blur_clust_groupby=None,
             blur_clust_thr=0, blur_spacing=0.25, blur_core_extent=0.0, blur_gauss_extent=0.0,
             blur_gauss_min=0.1, blur_apply_to=None, TCK_ref_image=None, ndirs=500, n_threads=-1,
-            keep_temp=False, verbose=2
+            keep_temp=False, verbose=3
             ):
     """Perform the conversion of a tractoram to the sparse data-structure internally
     used by COMMIT to perform the matrix-vector multiplications with the operator A
     during the inversion of the linear system.
 
     Parameters
     ----------
@@ -144,58 +160,60 @@
         Number of threads. If nothing is specified, the value used is the number of CPUs available
         in the system (default : -1).
 
     keep_temp: boolean
         If True, the temporary files are not deleted (default : False).
 
     verbose: int
-        Verbosity level (default : 2).
+        The verbosity level (0: only errors, 1: errors and warnings, 2: errors, warnings and info, 3: errors, warnings, info and progress bars, 4: errors, warnings, info, progress bars and debug)
     """
 
+    ui.set_verbose('trk2dictionary' ,verbose)
+
     # check the value of ndirs
     if not amico.lut.is_valid(ndirs):
-        ERROR( 'Unsupported value for ndirs.\nNote: Supported values for ndirs are [500 (default), 1000, 1500, 2000, 2500, 3000, 3500, 4000, 4500, 5000, 5500, 6000, 6500, 7000, 7500, 8000, 8500, 9000, 9500, 10000, 32761]' )
+        logger.error( 'Unsupported value for ndirs.\nNote: Supported values for ndirs are [500 (default), 1000, 1500, 2000, 2500, 3000, 3500, 4000, 4500, 5000, 5500, 6000, 6500, 7000, 7500, 8000, 8500, 9000, 9500, 10000, 32761]' )
 
     # check conflicts of fiber_shift
     if np.isscalar(fiber_shift) :
         fiber_shiftX = fiber_shift
         fiber_shiftY = fiber_shift
         fiber_shiftZ = fiber_shift
     elif len(fiber_shift) == 3 :
         fiber_shiftX = fiber_shift[0]
         fiber_shiftY = fiber_shift[1]
         fiber_shiftZ = fiber_shift[2]
     else :
-        ERROR( '"fiber_shift" must be a scalar or a vector with 3 elements' )
+        logger.error( '"fiber_shift" must be a scalar or a vector with 3 elements' )
 
     # check for invalid parameters in the blur
     if blur_core_extent < 0 :
-        ERROR( 'The extent of the core must be non-negative' )
+        logger.error( 'The extent of the core must be non-negative' )
 
     if blur_gauss_extent < 0 :
-        ERROR( 'The extent of the blur must be non-negative' )
+        logger.error( 'The extent of the blur must be non-negative' )
 
     if blur_gauss_extent > 0 or blur_core_extent > 0:
         if blur_spacing <= 0 :
-            ERROR( 'The grid spacing of the blur must be positive' )
+            logger.error( 'The grid spacing of the blur must be positive' )
 
     tic = time.time()
-    LOG( '\n-> Creating the dictionary from tractogram:' )
+    logger.info( 'Creating data structure from tractogram' )
 
-    LOG( '\n   * Configuration:' )
-    print( f'\t- Segment position = {"COMPUTE INTERSECTIONS" if do_intersect else "CENTROID"}' )
-    print( f'\t- Coordinates shift in X = {fiber_shiftX:.3f} (voxel-size units)' )
-    print( f'\t- Coordinates shift in Y = {fiber_shiftY:.3f} (voxel-size units)' )
-    print( f'\t- Coordinates shift in Z = {fiber_shiftZ:.3f} (voxel-size units)' )
+    logger.subinfo( 'Configuration:', indent_char='*', indent_lvl=1 )
+    logger.subinfo( f'Segment position = {"COMPUTE INTERSECTIONS" if do_intersect else "CENTROID"}', indent_lvl=2, indent_char='-' )
+    logger.subinfo( f'Coordinates shift in X = {fiber_shiftX:.3f} (voxel-size units)', indent_lvl=2, indent_char='-' )
+    logger.subinfo( f'Coordinates shift in Y = {fiber_shiftY:.3f} (voxel-size units)', indent_lvl=2, indent_char='-' )
+    logger.subinfo( f'Coordinates shift in Z = {fiber_shiftZ:.3f} (voxel-size units)', indent_lvl=2, indent_char='-' )
     if min_seg_len >= 1e-3:
-        print( f'\t- Min segment len  = {min_seg_len:.3f} mm' )
+        logger.subinfo( f'Min segment len    = {min_seg_len:.3f} mm', indent_lvl=2, indent_char='-' )
     else:
-        print( f'\t- Min segment len  = {min_seg_len:.2e} mm' )
-    print( f'\t- Min streamline len    = {min_fiber_len:.2f} mm' )
-    print( f'\t- Max streamline len    = {max_fiber_len:.2f} mm' )
+        logger.subinfo( f'Min segment len    = {min_seg_len:.2e} mm', indent_lvl=2, indent_char='-' )
+    logger.subinfo( f'Min streamline len = {min_fiber_len:.2f} mm', indent_lvl=2, indent_char='-' )
+    logger.subinfo( f'Max streamline len = {max_fiber_len:.2f} mm', indent_lvl=2, indent_char='-' )
 
     # check blur params
     cdef :
         double [:] blurRho
         double [:] blurAngle
         double [:] blurWeights
         bool [:] blurApplyTo
@@ -226,120 +244,121 @@
             for i in xrange(nReplicas):
                 if blurRho[i] <= blur_core_extent :
                     blurWeights[i] = 1.0
                 else:
                     blurWeights[i] = np.exp( -(blurRho[i] - blur_core_extent)**2 / (2.0*blur_sigma**2) )
 
     if nReplicas == 1 :
-        print( '\t- Do not blur streamlines' )
+        logger.subinfo( 'Do not blur streamlines', indent_lvl=2, indent_char='-' )
     else :
-        print( '\t- Blur streamlines:' )
-        print( f'\t\t- core extent  = {blur_core_extent:.3f}' )
-        print( f'\t\t- gauss extent = {blur_gauss_extent:.3f} (sigma = {blur_sigma:.3f})' )
-        print( f'\t\t- grid spacing = {blur_spacing:.3f}' )
-        print( f'\t\t- weights = [ {np.min(blurWeights):.3f} ... {np.max(blurWeights):.3f} ]' )
+        logger.subinfo( 'Blur streamlines:', indent_lvl=2, indent_char='-' )
+        logger.subinfo( f'core extent  = {blur_core_extent:.3f}', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'gauss extent = {blur_gauss_extent:.3f} (sigma = {blur_sigma:.3f})', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'grid spacing = {blur_spacing:.3f}' , indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'weights = [ {np.min(blurWeights):.3f} ... {np.max(blurWeights):.3f} ]', indent_lvl=3, indent_char='-' )
 
     if min_seg_len < 0 :
-        ERROR( '"min_seg_len" must be >= 0' )
+        logger.error( '"min_seg_len" must be >= 0' )
     if min_fiber_len < 0 :
-        ERROR( '"min_fiber_len" must be >= 0' )
+        logger.error( '"min_fiber_len" must be >= 0' )
     if max_fiber_len < min_fiber_len :
-        ERROR( '"max_fiber_len" must be >= "min_fiber_len"' )
+        logger.error( '"max_fiber_len" must be >= "min_fiber_len"' )
 
     if filename_tractogram is None:
-        ERROR( '"filename_tractogram" not defined' )
+        logger.error( '"filename_tractogram" not defined' )
 
     if path_out is None:
         path_out = dirname(filename_tractogram)
         if path_out == '':
             path_out = '.'
         if not isdir(path_out):
-            ERROR( '"path_out" cannot be inferred from "filename_tractogram"' )
+            logger.error( '"path_out" cannot be inferred from "filename_tractogram"' )
         path_out = join(path_out,'COMMIT')
 
     # create output path
-    print( f'\t- Output written to "{path_out}"' )
+    logger.subinfo( f'Output written to "{path_out}"', indent_char='-', indent_lvl=2 )
     if not exists( path_out ):
         makedirs( path_out )
 
     path_temp = join(path_out, 'temp')
-    print( f'\t- Temporary files written to "{path_temp}"' )
+    logger.subinfo( f'Temporary files written to "{path_temp}"', indent_char='-', indent_lvl=2 )
 
     if exists(path_temp):
         shutil.rmtree(path_temp, ignore_errors=True)
     makedirs(path_temp, exist_ok=True)
 
     if n_threads == 0 or n_threads > 255 :
-        ERROR( 'Number of n_threads must be between 1 and 255' )
+        logger.error( 'Number of n_threads must be between 1 and 255' )
 
     if n_threads == -1 :
         # Set to the number of CPUs in the system
         try :
             n_threads = os.cpu_count()
         except :
             n_threads = 1
 
-    print( f'\t- Using parallel computation with {n_threads} threads' )
+    logger.subinfo( f'Using parallel computation with {n_threads} threads', indent_char='-', indent_lvl=2 )
 
     if np.isscalar(blur_clust_thr):
         blur_clust_thr = np.array( [blur_clust_thr] )
 
     if blur_clust_thr[0]> 0:
-        LOG( '\n   * Running tractogram clustering:' )
-        print( f'\t- Input tractogram "{filename_tractogram}"' )
-        print( f'\t- Clustering threshold = {blur_clust_thr[0]}' )
+        logger.subinfo( 'Reducing streamlines redundancy:', indent_char='*', indent_lvl=1)
+        logger.subinfo( f'Input tractogram "{filename_tractogram}"', indent_lvl=2, indent_char='-' )
         input_hdr = nibabel.streamlines.load( filename_tractogram, lazy_load=True ).header
         input_n_count = int(input_hdr['count'])
 
         extension = splitext(filename_tractogram)[1]
 
         if filename_mask is None and TCK_ref_image is None:
             if extension == ".tck":
-                ERROR( 'TCK files do not contain information about the geometry. Use "TCK_ref_image" for that' )
+                logger.error( 'TCK files do not contain information about the geometry. Use "TCK_ref_image" for that' )
             else:
-                ERROR( 'Unknown file extension. Use "filename_mask" or "TCK_ref_image" for that' )
+                logger.error( 'Unknown file extension. Use "filename_mask" or "TCK_ref_image" for that' )
 
         input_tractogram = os.path.basename(filename_tractogram)[:len(os.path.basename(filename_tractogram))-4]
-        filename_out = join( path_temp, f'{input_tractogram}_clustered_thr_{float(blur_clust_thr[0])}.tck' )
+        filename_out = join( path_out, f'{input_tractogram}_clustered_thr_{float(blur_clust_thr[0])}.tck' )
 
         if blur_clust_groupby:
-            file_assignments = join( path_temp, f'{input_tractogram}_clustered_thr_{blur_clust_thr[0]}_assignments.txt' )
             hdr = nibabel.streamlines.load( filename_tractogram, lazy_load=True ).header
             temp_idx = np.arange(int(hdr['count']))
-            path_streamline_idx = join( path_temp,"streamline_idx.npy")
-            np.save( path_streamline_idx, temp_idx )
-            idx_centroids = run_clustering(file_name_in=filename_tractogram, output_folder=path_temp, atlas=blur_clust_groupby,
-                            clust_thr=blur_clust_thr[0], save_assignments=file_assignments,
-                            temp_idx=path_streamline_idx, n_threads=n_threads, force=True, verbose=verbose)
+            log_list = []
+            subinfo = logger.subinfo(f'Clustering with threshold = {blur_clust_thr[0]}', indent_lvl=2, indent_char='-', with_progress=verbose>2)
+            with ProgressBar(disable=verbose<3, hide_on_exit=True, subinfo=subinfo, log_list=log_list) as pbar:
+                idx_centroids = run_clustering(tractogram_in=filename_tractogram, tractogram_out=filename_out,
+                                            temp_folder=path_temp, atlas=blur_clust_groupby, clust_thr=blur_clust_thr[0],
+                                            n_threads=n_threads, keep_temp_files=True, force=True, verbose=1, log_list=log_list)
         else:
-            idx_centroids = run_clustering(file_name_in=filename_tractogram, output_folder=path_temp, clust_thr=blur_clust_thr[0],
-                            force=True, verbose=verbose)
+            logger.subinfo(f'Clustering with threshold = {blur_clust_thr[0]}', indent_lvl=2, indent_char='-', with_progress=verbose>2)
+            with ProgressBar(disable=verbose<3, hide_on_exit=True, subinfo=True) as pbar:
+                idx_centroids = run_clustering(tractogram_in=filename_tractogram, tractogram_out=filename_out,
+                                            temp_folder=path_temp, clust_thr=blur_clust_thr[0],
+                                            keep_temp_files=True, force=True, verbose=1)
         filename_tractogram = filename_out
 
 
-
     # Load data from files
-    LOG( '\n   * Loading data:' )
+    logger.subinfo( 'Loading data:', indent_char='*', indent_lvl=1 )
     cdef short [:] htable = amico.lut.load_precomputed_hash_table(ndirs)
     cdef short* ptrHashTable = &htable[0]
 
     # Streamlines from tractogram
-    print( '\t- Tractogram' )
+    logger.subinfo( 'Tractogram:', indent_lvl=2, indent_char='-' )
 
     if not exists(filename_tractogram):
-        ERROR( f'Tractogram file not found: {filename_tractogram}' )
+        logger.error( f'Tractogram file not found: {filename_tractogram}' )
     extension = splitext(filename_tractogram)[1]
     if extension != ".trk" and extension != ".tck":
-        ERROR( 'Invalid input file: only .trk and .tck are supported' )
+        logger.error( 'Invalid input file: only .trk and .tck are supported' )
 
     hdr = nibabel.streamlines.load( filename_tractogram, lazy_load=True ).header
 
 
     if extension == ".trk":
-        print ( f'\t\t- geometry taken from "{filename_tractogram}"' )
+        logger.subinfo ( f'geometry taken from "{filename_tractogram}"', indent_lvl=3, indent_char='-' )
         Nx = int(hdr['dimensions'][0])
         Ny = int(hdr['dimensions'][1])
         Nz = int(hdr['dimensions'][2])
         Px = hdr['voxel_sizes'][0]
         Py = hdr['voxel_sizes'][1]
         Pz = hdr['voxel_sizes'][2]
 
@@ -351,46 +370,50 @@
     else:
         if TCK_ref_image is None:
             if filename_peaks is not None:
                 TCK_ref_image = filename_peaks
             elif filename_mask is not None:
                 TCK_ref_image = filename_mask
             else:
-                ERROR( 'TCK files do not contain information about the geometry. Use "TCK_ref_image" for that' )
-        print ( f'\t\t- geometry taken from "{TCK_ref_image}"' )
+                logger.error( 'TCK files do not contain information about the geometry. Use "TCK_ref_image" for that' )
+        logger.subinfo ( f'geometry taken from "{TCK_ref_image}"', indent_lvl=3, indent_char='-' )
 
         niiREF = nibabel.load( TCK_ref_image )
         niiREF_hdr = _get_header( niiREF )
         Nx = niiREF.shape[0]
         Ny = niiREF.shape[1]
         Nz = niiREF.shape[2]
         Px = niiREF_hdr['pixdim'][1]
         Py = niiREF_hdr['pixdim'][2]
         Pz = niiREF_hdr['pixdim'][3]
         data_offset = int(hdr['_offset_data'])
         n_count = int(hdr['count'])
         n_scalars = 0
         n_properties = 0
 
-    print( f'\t\t- {Nx} x {Ny} x {Nz}' )
-    print( f'\t\t- {Px:.4f} x {Py:.4f} x {Pz:.4f}' )
+    if n_threads > n_count:
+        logger.warning( 'Reducing the number of threads to the number of streamlines' )
+        n_threads = n_count
+
+    logger.subinfo( f'{Nx} x {Ny} x {Nz}', indent_lvl=3, indent_char='-' )
+    logger.subinfo( f'{Px:.4f} x {Py:.4f} x {Pz:.4f}', indent_lvl=3, indent_char='-' )
     if blur_clust_thr[0]> 0:
-        print( f'\t\t- {input_n_count} streamlines' )
+        logger.subinfo( f'{input_n_count} streamlines', indent_lvl=3, indent_char='-' )
     else:
-        print( f'\t\t- {n_count} streamlines' )
+        logger.subinfo( f'{n_count} streamlines', indent_lvl=3, indent_char='-' )
     if Nx >= 2**16 or Nz >= 2**16 or Nz >= 2**16 :
-        ERROR( 'The max dim size is 2^16 voxels' )
+        logger.error( 'The max dim size is 2^16 voxels' )
 
     # check copmpatibility between blurApplyTo and number of streamlines
     if blur_apply_to is None:
         blur_apply_to = np.repeat([True], n_count)
     else :
         if blur_apply_to.size != n_count :
-            ERROR( '"blur_apply_to" must have one value per streamline' )
-        print( f'\t\t\t- {sum(blur_apply_to)} blurred streamlines' )
+            logger.error( '"blur_apply_to" must have one value per streamline' )
+        logger.subinfo( f'{sum(blur_apply_to)} blurred streamlines', indent_lvl=3, indent_char='-' )
     blurApplyTo = blur_apply_to
 
     # get toVOXMM matrix (remove voxel scaling from affine) in case of TCK
     cdef float [:] toVOXMM
     cdef float* ptrToVOXMM
     if extension == ".tck":
         M = _get_affine( niiREF ).copy()
@@ -398,26 +421,26 @@
         toVOXMM = np.ravel(np.linalg.inv(M)).astype('<f4')
         ptrToVOXMM = &toVOXMM[0]
 
     # white-matter mask
     cdef float* ptrMASK
     cdef float [:, :, ::1] niiMASK_img
     if filename_mask is not None :
-        print( '\t- Filtering mask' )
+        logger.subinfo( 'Filtering mask:', indent_lvl=2, indent_char='-' )
         niiMASK = nibabel.load( filename_mask )
         niiMASK_hdr = _get_header( niiMASK )
-        print( f'\t\t- {niiMASK.shape[0]} x {niiMASK.shape[1]} x {niiMASK.shape[2]}' )
-        print( f'\t\t- {niiMASK_hdr["pixdim"][1]:.4f} x {niiMASK_hdr["pixdim"][2]:.4f} x {niiMASK_hdr["pixdim"][3]:.4f}' )
-        if ( Nx!=niiMASK.shape[0] or Ny!=niiMASK.shape[1] or Nz!=niiMASK.shape[2] or
+        logger.subinfo( f'{niiMASK.shape[0]} x {niiMASK.shape[1]} x {niiMASK.shape[2]}', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'{niiMASK_hdr["pixdim"][1]:.4f} x {niiMASK_hdr["pixdim"][2]:.4f} x {niiMASK_hdr["pixdim"][3]:.4f}', indent_lvl=3, indent_char='-' )
+        if ( Nx!=niiMASK.shape[0] or Ny!=niiMASK.shape[1] or Nz!=niiMASK.shape[2] or 
             abs(Px-niiMASK_hdr['pixdim'][1])>1e-3 or abs(Py-niiMASK_hdr['pixdim'][2])>1e-3 or abs(Pz-niiMASK_hdr['pixdim'][3])>1e-3 ) :
-            WARNING( 'Dataset does not have the same geometry as the tractogram' )
+            logger.warning( 'Dataset does not have the same geometry as the tractogram' )
         niiMASK_img = np.ascontiguousarray( np.asanyarray( niiMASK.dataobj ).astype(np.float32) )
         ptrMASK  = &niiMASK_img[0,0,0]
     else :
-        print( '\t- No mask specified to filter IC compartments' )
+        logger.subinfo( 'No mask specified to filter IC compartments', indent_lvl=2, indent_char='-' )
         ptrMASK = NULL
 
     # peaks file for EC contributions
     cdef float* ptrPEAKS
     cdef float [:, :, :, ::1] niiPEAKS_img
     cdef int Np
     cdef double [:,:, :,::1] niiTDI_img = np.ascontiguousarray( np.zeros((n_threads,Nx,Ny,Nz),dtype=np.float64) )
@@ -425,62 +448,62 @@
     for i in range(n_threads):
         ptrTDI[i] = &niiTDI_img[i,0,0,0]
 
     cdef double [:, ::1] peaksAffine
     cdef double* ptrPeaksAffine
 
     if filename_peaks is not None :
-        print( '\t- EC orientations' )
+        logger.subinfo( 'EC orientations:', indent_lvl=2, indent_char='-' )
         niiPEAKS = nibabel.load( filename_peaks )
         niiPEAKS_hdr = _get_header( niiPEAKS )
-        print( f'\t\t- {niiPEAKS.shape[0]} x {niiPEAKS.shape[1]} x {niiPEAKS.shape[2]} x {niiPEAKS.shape[3]}' )
-        print( f'\t\t- {niiPEAKS_hdr["pixdim"][1]:.4f} x {niiPEAKS_hdr["pixdim"][2]:.4f} x {niiPEAKS_hdr["pixdim"][3]:.4f}' )
-
-        print( f'\t\t- ignoring peaks < {vf_THR:.2f} * MaxPeak' )
-        print( f'\t\t- {"" if peaks_use_affine else "not "}using affine matrix' )
-        print( f'\t\t- flipping axes : [ x={flip_peaks[0]}, y={flip_peaks[1]}, z={flip_peaks[2]} ]' )
+        logger.subinfo( f'{niiPEAKS.shape[0]} x {niiPEAKS.shape[1]} x {niiPEAKS.shape[2]} x {niiPEAKS.shape[3]}', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'{niiPEAKS_hdr["pixdim"][1]:.4f} x {niiPEAKS_hdr["pixdim"][2]:.4f} x {niiPEAKS_hdr["pixdim"][3]:.4f}', indent_lvl=3, indent_char='-' )
+        
+        logger.subinfo( f'ignoring peaks < {vf_THR:.2f} * MaxPeak', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'{"" if peaks_use_affine else "not "}using affine matrix', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'flipping axes : [ x={flip_peaks[0]}, y={flip_peaks[1]}, z={flip_peaks[2]} ]', indent_lvl=3, indent_char='-' )
         if ( Nx!=niiPEAKS.shape[0] or Ny!=niiPEAKS.shape[1] or Nz!=niiPEAKS.shape[2] or
             abs(Px-niiPEAKS_hdr['pixdim'][1])>1e-3 or abs(Py-niiPEAKS_hdr['pixdim'][2])>1e-3 or abs(Pz-niiPEAKS_hdr['pixdim'][3])>1e-3 ) :
-            WARNING( "Dataset does not have the same geometry as the tractogram" )
+            logger.warning( "Dataset does not have the same geometry as the tractogram" )
         if niiPEAKS.shape[3] % 3 :
-            ERROR( 'PEAKS dataset must have 3*k volumes' )
+            logger.error( 'PEAKS dataset must have 3*k volumes' )
         if vf_THR < 0 or vf_THR > 1 :
-            ERROR( '"vf_THR" must be between 0 and 1' )
+            logger.error( '"vf_THR" must be between 0 and 1' )
         niiPEAKS_img = np.ascontiguousarray( np.asanyarray( niiPEAKS.dataobj ).astype(np.float32) )
         ptrPEAKS = &niiPEAKS_img[0,0,0,0]
         Np = niiPEAKS.shape[3]/3
 
         # affine matrix to rotate gradien directions (if required)
         if peaks_use_affine :
             peaksAffine = np.ascontiguousarray( niiPEAKS.affine[:3,:3].T )
         else :
             peaksAffine = np.ascontiguousarray( np.eye(3) )
         ptrPeaksAffine = &peaksAffine[0,0]
     else :
-        print( '\t- No dataset specified for EC compartments' )
+        logger.subinfo( 'No dataset specified for EC compartments', indent_lvl=2, indent_char='-' )
         Np = 0
         ptrPEAKS = NULL
         ptrPeaksAffine = NULL
     
     # ISO map for isotropic compartment
     cdef float* ptrISO
     cdef float [:, :, ::1] niiISO_img
     if filename_ISO is not None :
-        print( '\t- Restricted ISO map' )
+        logger.subinfo( 'Restricted ISO map', indent_lvl=2, indent_char='-' )
         niiISO = nibabel.load( filename_ISO )
         niiISO_hdr = _get_header( niiISO )
-        print( f'\t\t- {niiISO.shape[0]} x {niiISO.shape[1]} x {niiISO.shape[2]}' )
-        print( f'\t\t- {niiISO_hdr["pixdim"][1]:.4f} x {niiISO_hdr["pixdim"][2]:.4f} x {niiISO_hdr["pixdim"][3]:.4f}' )
+        logger.subinfo( f'{niiISO.shape[0]} x {niiISO.shape[1]} x {niiISO.shape[2]}', indent_lvl=3, indent_char='-' )
+        logger.subinfo( f'{niiISO_hdr["pixdim"][1]:.4f} x {niiISO_hdr["pixdim"][2]:.4f} x {niiISO_hdr["pixdim"][3]:.4f}', indent_lvl=3, indent_char='-' )
         if ( Nx!=niiISO.shape[0] or Ny!=niiISO.shape[1] or Nz!=niiISO.shape[2] or
             abs(Px-niiISO_hdr['pixdim'][1])>1e-3 or abs(Py-niiISO_hdr['pixdim'][2])>1e-3 or abs(Pz-niiISO_hdr['pixdim'][3])>1e-3 ) :
-            WARNING( 'Dataset does not have the same geometry as the tractogram' )
+            logger.warning( 'Dataset does not have the same geometry as the tractogram' )
         niiISO_img = np.ascontiguousarray( np.asanyarray( niiISO.dataobj ).astype(np.float32) )
         ptrISO  = &niiISO_img[0,0,0]
     else :
-        print( '\t- No ISO map specified, using tdi' )
+        logger.subinfo( 'No ISO map specified, using tdi', indent_lvl=2, indent_char='-' )
         ptrISO = NULL
 
     # write dictionary information info file
     dictionary_info = {}
     dictionary_info['filename_tractogram'] = filename_tractogram
     if blur_clust_thr[0]> 0:
         idx_centroids = np.array(idx_centroids, dtype=np.uint32)
@@ -513,109 +536,112 @@
     ret = trk2dictionary( filename_tractogram, data_offset,
         Nx, Ny, Nz, Px, Py, Pz, n_count, n_scalars, n_properties,
         fiber_shiftX, fiber_shiftY, fiber_shiftZ, min_seg_len, min_fiber_len, max_fiber_len,
         ptrPEAKS, Np, vf_THR, -1 if flip_peaks[0] else 1, -1 if flip_peaks[1] else 1, -1 if flip_peaks[2] else 1,
         ptrMASK, ptrISO, ptrTDI, path_temp, 1 if do_intersect else 0, ptrPeaksAffine,
         nReplicas, &blurRho[0], &blurAngle[0], &blurWeights[0], &blurApplyTo[0], ptrToVOXMM, ptrHashTable, n_threads, verbose if not _in_notebook() else 0 );
     if ret == 0 :
-        WARNING( 'DICTIONARY not generated' )
+        logger.warning( 'DICTIONARY not generated' )
         return None
 
     # Concatenate files together
+    logger.subinfo( 'Saving data structure', indent_char='*', indent_lvl=1, with_progress=True )
     cdef int discarded = 0
-    for j in range(n_threads-1):
-        path_IC_f = path_temp + f'/dictionary_IC_f_{j+1}.dict'
-        kept = np.fromfile( path_temp + f'/dictionary_TRK_kept_{j}.dict', dtype=np.uint8 )
-        IC_f = np.fromfile( path_temp + f'/dictionary_IC_f_{j+1}.dict', dtype=np.uint32 )
-        discarded += np.count_nonzero(kept==0)
-        IC_f -= discarded
-        IC_f_save = np.memmap( path_IC_f, dtype="uint32", mode='w+', shape=IC_f.shape )
-        IC_f_save[:] = IC_f[:]
-        IC_f_save.flush()
-        del IC_f_save
-        # np.save( path_out + f'/dictionary_IC_f_{j+1}.dict', IC_f, allow_pickle=True)
-
-    fileout = path_out + '/dictionary_TRK_kept.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_TRK_kept_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_TRK_norm.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_TRK_norm_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_TRK_len.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_TRK_len_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_TRK_lenTot.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_TRK_lenTot_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_IC_f.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_IC_f_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_IC_v.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_IC_v_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_IC_o.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_IC_o_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
-    fileout = path_out + '/dictionary_IC_len.dict'
-    dict_list = []
-    for j in range(n_threads):
-        dict_list += [ path_temp + f'/dictionary_IC_len_{j}.dict' ]
-    cat_function( dict_list, fileout )
-
+    with ProgressBar(disable=verbose<3, hide_on_exit=True, subinfo=True) as pbar:
+        for j in range(n_threads-1):
+            path_IC_f = path_temp + f'/dictionary_IC_f_{j+1}.dict'
+            kept = np.fromfile( path_temp + f'/dictionary_TRK_kept_{j}.dict', dtype=np.uint8 )
+            IC_f = np.fromfile( path_temp + f'/dictionary_IC_f_{j+1}.dict', dtype=np.uint32 )
+            discarded += np.count_nonzero(kept==0)
+            IC_f -= discarded
+            IC_f_save = np.memmap( path_IC_f, dtype="uint32", mode='w+', shape=IC_f.shape )
+            IC_f_save[:] = IC_f[:]
+            IC_f_save.flush()
+            del IC_f_save
+            # np.save( path_out + f'/dictionary_IC_f_{j+1}.dict', IC_f, allow_pickle=True)
+
+        fileout = path_out + '/dictionary_TRK_kept.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_TRK_kept_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_TRK_norm.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_TRK_norm_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_TRK_len.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_TRK_len_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_TRK_lenTot.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_TRK_lenTot_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_IC_f.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_IC_f_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_IC_v.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_IC_v_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_IC_o.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_IC_o_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+        fileout = path_out + '/dictionary_IC_len.dict'
+        dict_list = []
+        for j in range(n_threads):
+            dict_list += [ path_temp + f'/dictionary_IC_len_{j}.dict' ]
+        cat_function( dict_list, fileout )
+
+
+        # save TDI and MASK maps
+        if TCK_ref_image is not None:
+            TDI_affine = _get_affine( niiREF )
+        elif filename_mask is not None :
+            TDI_affine = _get_affine( niiMASK )
+        elif filename_peaks is not None :
+            TDI_affine = _get_affine( niiPEAKS )
+        else :
+            TDI_affine = np.diag( [Px, Py, Pz, 1] )
 
     # save TDI and MASK maps
-    if TCK_ref_image is not None:
-        TDI_affine = _get_affine( niiREF )
-    elif filename_mask is not None :
-        TDI_affine = _get_affine( niiMASK )
-    elif filename_peaks is not None :
-        TDI_affine = _get_affine( niiPEAKS )
-    else :
-        TDI_affine = np.diag( [Px, Py, Pz, 1] )
-
+    logger.subinfo( 'Saving TDI and MASK maps', indent_char='*', indent_lvl=1 )
     v = np.fromfile( join(path_out, 'dictionary_IC_v.dict'),   dtype=np.uint32 )
     l = np.fromfile( join(path_out, 'dictionary_IC_len.dict'), dtype=np.float32 )
 
     cdef np.float32_t [::1] niiTDI_mem = np.zeros( Nx*Ny*Nz, dtype=np.float32 )
-    niiTDI_mem = compute_tdi( v, l, Nx, Ny, Nz )
+    niiTDI_mem = compute_tdi( v, l, Nx, Ny, Nz, verbose )
     niiTDI_img_save = np.reshape( niiTDI_mem, (Nx,Ny,Nz), order='F' )
 
     niiTDI = nibabel.Nifti1Image( niiTDI_img_save, TDI_affine )
     niiTDI_hdr = _get_header( niiTDI )
     niiTDI_hdr['descrip'] = f'Created with COMMIT {get_distribution("dmri-commit").version}'
     nibabel.save( niiTDI, join(path_out,'dictionary_tdi.nii.gz') )
 
     if filename_mask is not None :
         niiMASK = nibabel.Nifti1Image( niiMASK_img, TDI_affine )
     else :
-        niiMASK = nibabel.Nifti1Image( (np.asarray(niiTDI_img)>0).astype(np.float32), TDI_affine )
+        niiMASK = nibabel.Nifti1Image( (np.asarray(niiTDI_img_save)>0).astype(np.float32), TDI_affine )
 
     niiMASK_hdr = _get_header( niiMASK )
     niiMASK_hdr['descrip'] = niiTDI_hdr['descrip']
     nibabel.save( niiMASK, join(path_out,'dictionary_mask.nii.gz') )
 
     if not keep_temp:
         shutil.rmtree(path_temp)
 
-
-    LOG( f'\n   [ {time.time() - tic:.1f} seconds ]' )
+    logger.info( f'[ {format_time(time.time() - tic)} ]' )
```

### Comparing `dmri-commit-2.1.0/commit/trk2dictionary/trk2dictionary_c.cpp` & `dmri-commit-2.2.0/commit/trk2dictionary/trk2dictionary_c.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -72,18 +72,18 @@
 float*          ptrISO;
 float           fiberShiftXmm, fiberShiftYmm, fiberShiftZmm;
 bool            doIntersect;
 float           minSegLen, minFiberLen, maxFiberLen;
 
 // Threads variables
 vector<thread>  threads;
-vector<unsigned int>    totICSegments; 
-vector<unsigned int>    totFibers;
-unsigned int            totECVoxels = 0;
-unsigned int            totECSegments = 0;
+vector<unsigned long int>   totICSegments; 
+vector<unsigned int>        totFibers;
+unsigned int                totECVoxels = 0;
+unsigned int                totECSegments = 0;
 
 // progressbar verbosity
 int verbosity = 0;
 
 // --- Functions Definitions ----
 bool rayBoxIntersection( Vector<double>& origin, Vector<double>& direction, Vector<double>& vmin, Vector<double>& vmax, double & t);
 void fiberForwardModel( float fiber[3][MAX_FIB_LEN], unsigned int pts, int nReplicas, double* ptrBlurRho, double* ptrBlurAngle, double* ptrBlurWeights, bool doApplyBlur, short* ptrHashTable, vector<Vector<double>>& P );
@@ -229,18 +229,18 @@
 
 
 
     // ==========================================
     //          Parallel IC compartments
     // ==========================================
 
-    printf( "\n   \033[0;32m* Exporting IC compartments:\033[0m\n" );
+    printf( "   * Exporting IC compartments:\033[0m\n" );
     // unsigned int width = 25;
     // PROGRESS = new ProgressBar( (unsigned int) n_count, (unsigned int) width);
-    if (verbosity > 0)
+    if (verbosity > 2)
     {
         PROGRESS->reset((unsigned int) n_count);
         PROGRESS->setPrefix("     ");
     }
     // ---- Original ------
     for( int i = 0; i<threads_count; i++ ){
         threads.push_back( thread( ICSegments, str_filename, isTRK, n_count, nReplicas, n_scalars, n_properties, ptrToVOXMM,
@@ -249,39 +249,39 @@
     }
 
 
     for( int i = 0; i<threads_count; i++ ) {
         threads[i].join();
     }
 
-    if (verbosity > 0)
+    if (verbosity > 2)
         PROGRESS->close();
 
-    printf( "     [ %d streamlines kept, %d segments in total ]\n", std::accumulate(totFibers.begin(), totFibers.end(), 0), std::accumulate( totICSegments.begin(), totICSegments.end(), 0) );
+    printf( "      [ %d streamlines kept, %ld segments in total ]\n", std::accumulate(totFibers.begin(), totFibers.end(), 0), std::accumulate( totICSegments.begin(), totICSegments.end(), 0) );
     totFibers.clear();
     threads.clear();
 
     // ==========================================
     //          Parallel EC compartments
     // ==========================================
 
-    printf( "\n   \033[0;32m* Exporting EC compartments:\033[0m\n" );
+    printf( "   * Exporting EC compartments:\033[0m\n" );
 
     int EC = ECSegments( ptrPEAKS, Np, vf_THR, ECix, ECiy, ECiz, ptrTDI, ptrHashTable, path_out, ptrPeaksAffine, threads_count );
 
-    printf("     [ %d voxels, %d segments ]\n", totECVoxels, totECSegments );
+    printf("      [ %d voxels, %d segments ]\n", totECVoxels, totECSegments );
 
     /*=========================*/
     /*     Restricted ISO compartments     */
     /*=========================*/
-    printf( "\n   \033[0;32m* Exporting ISO compartments:\033[0m\n" );
+    printf( "   * Exporting ISO compartments:\033[0m\n" );
 
     int totISO = ISOcompartments(ptrTDI, path_out, threads_count);
 
-    printf("     [ %d voxels ]\n", totISO );
+    printf("      [ %d voxels ]\n", totISO );
 
     return 1;
 
 }
 
 
 int ECSegments(float* ptrPEAKS, int Np, float vf_THR, int ECix, int ECiy, int ECiz,
@@ -453,21 +453,22 @@
 
 int ICSegments( char* str_filename, int isTRK, int n_count, int nReplicas, int n_scalars, int n_properties, float* ptrToVOXMM, double* ptrTDI, double* ptrBlurRho, 
 double* ptrBlurAngle, double* ptrBlurWeights, bool* ptrBlurApplyTo, short* ptrHashTable, char* path_out, 
 unsigned long long int offset, int idx, unsigned int startpos, unsigned int endpos ) 
 {
 
     // Variables definition
-    float           fiber[3][MAX_FIB_LEN] = {0} ;
-    float           fiberNorm;   // normalization
-    unsigned int    N, v, tempTotFibers, temp_totICSegments;
-    unsigned short  o;
-    unsigned char   kept;
-    string          filename;
-    string          OUTPUT_path(path_out);
+    float               fiber[3][MAX_FIB_LEN] = {0} ;
+    float               fiberNorm;   // normalization
+    unsigned int        N, v, tempTotFibers;
+    unsigned long int   temp_totICSegments;
+    unsigned short      o;
+    unsigned char       kept;
+    string              filename;
+    string              OUTPUT_path(path_out);
 
     unsigned int sumFibers = startpos;
 
     map<segKey,float>::iterator it;
     map<segInVoxKey,float> FiberNorm;
     map<segInVoxKey,float>::iterator itNorm;
 
@@ -519,15 +520,15 @@
         if ( FiberSegments.size() > 0 )
         {
             if ( FiberLen > minFiberLen && FiberLen < maxFiberLen )
             {
                 // add segments to files
                 for (it=FiberSegments.begin(); it!=FiberSegments.end(); it++)
                 {
-                    // NB: plese note inverted ordering for 'v'
+                    // NB: please note inverted ordering for 'v'
                     v = it->first.x + dim.x * ( it->first.y + dim.y * it->first.z );
                     o = it->first.o;       
 
                     fwrite( &sumFibers,      4, 1, pDict_IC_f );
                     fwrite( &v,              4, 1, pDict_IC_v );
                     fwrite( &o,              2, 1, pDict_IC_o );
                     fwrite( &(it->second),   4, 1, pDict_IC_len );       
@@ -556,15 +557,15 @@
 
         }
 
         fwrite( &kept, 1, 1, pDict_TRK_kept );
         totFibers[idx] = tempTotFibers;
         totICSegments[idx] = temp_totICSegments;
 
-        if (verbosity > 0)
+        if (verbosity > 2)
         {
             if (idx == 0)
             {
                 incr_new = std::accumulate(totFibers.begin(), totFibers.end(), 0);
                 for(int i=incr_old; i<incr_new; i++)
                     PROGRESS->inc();
                 incr_old = incr_new;
```

### Comparing `dmri-commit-2.1.0/setup.py` & `dmri-commit-2.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
+
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
-import os
 
 # name of the package
 package_name = 'commit'
 
 def get_extensions():
     # Cython extension to create the sparse data structure from a tractogram
     # for the computation of matrix-vector multiplications
@@ -24,17 +25,18 @@
                  
     return [trk2dictionary, core, proximals]
 
 class CustomBuildExtCommand(build_ext):
     """ build_ext command to use when numpy headers are needed. """
     def run(self):
         # Now that the requirements are installed, get everything from numpy
+        from multiprocessing import cpu_count
+
         from Cython.Build import cythonize
         from numpy import get_include
-        from multiprocessing import cpu_count
 
         # Add everything requires for build
         self.swig_opts = None
         self.include_dirs = [get_include()]
         self.distribution.ext_modules[:] = cythonize( self.distribution.ext_modules, build_dir='build' )
 
         # if not specified via '-j N' option, set compilation using max number of cores
@@ -42,33 +44,16 @@
             self.parallel = cpu_count()
         print( f'Parallel compilation using {self.parallel} threads' )
 
         # Call original build_ext command
         build_ext.finalize_options(self)
         build_ext.run(self)
 
-# import details from {package_name}/info.py
-import sys
-sys.path.insert(0, f'./{package_name}/')
-import info
-
 # create the 'build' directory
 if not os.path.exists('build'):
     os.makedirs('build')
 
 # install the package
 setup(
-    name=info.NAME,
-    version=info.VERSION,
-    description=info.DESCRIPTION,
-    long_description=info.LONG_DESCRIPTION,
-    author=info.AUTHOR,
-    author_email=info.AUTHOR_EMAIL,
-    url=info.URL,
-    license=info.LICENSE,
-    packages=[f'{package_name}', f'{package_name}.operator'],
     cmdclass={'build_ext': CustomBuildExtCommand},
-    ext_modules=get_extensions(),
-    setup_requires=['Cython>=0.29', 'numpy>=1.12', 'wheel'],
-    install_requires=['setuptools>=46.1', 'Cython>=0.29', 'numpy>=1.12', 'scipy>=1.0', 'dipy>=1.0', 'dmri-dicelib>=1.0.3', 'dmri-amico>=2.0.1'],
-    package_data={f'{package_name}.operator': ["*.*"]}
+    ext_modules=get_extensions()
 )
```

