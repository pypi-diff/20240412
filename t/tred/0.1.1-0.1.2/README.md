# Comparing `tmp/tred-0.1.1.tar.gz` & `tmp/tred-0.1.2.tar.gz`

## Comparing `tred-0.1.1.tar` & `tred-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.1/requirements.txt
--rw-r--r--   0        0        0    18447 2020-02-02 00:00:00.000000 tred-0.1.1/examples/basic.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_m_transforms.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_tensor_ops.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_tensor_pca.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tred-0.1.1/tred/__init__.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_m_transforms.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_tensor_ops.py
--rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_tensor_pca.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tred-0.1.1/tred/_utils.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.1/LICENSE
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.1/README.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tred-0.1.2/requirements.txt
+-rw-r--r--   0        0        0    18447 2020-02-02 00:00:00.000000 tred-0.1.2/examples/basic.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tred-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_m_transforms.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_tensor_ops.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_tensor_pca.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tred-0.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tred-0.1.2/tred/__init__.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_m_transforms.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_tensor_ops.py
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_tensor_pca.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 tred-0.1.2/tred/_utils.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 tred-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tred-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tred-0.1.2/README.txt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tred-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tred-0.1.2/PKG-INFO
```

### Comparing `tred-0.1.1/examples/basic.ipynb` & `tred-0.1.2/examples/basic.ipynb`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tests/test_m_transforms.py` & `tred-0.1.2/tests/test_m_transforms.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tests/test_tensor_ops.py` & `tred-0.1.2/tests/test_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tests/test_tensor_pca.py` & `tred-0.1.2/tests/test_tensor_pca.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,44 +13,61 @@
     generate_transform_pair_from_matrix,
     generate_dctii_m_transform_pair,
     generate_dstii_m_transform_pair,
 )
 
 
 GLOBAL_SEED = 1
-RNG = np.random.default_rng(seed=GLOBAL_SEED)
+GLOBAL_RNG = np.random.default_rng(seed=GLOBAL_SEED)
+
+# various n, p, t sizes
+# ensure n > p, p > n inputs are tested
+TENSOR_SHAPES = [(4, 3, 2), (5, 7, 6), (2, 2, 6)]
+
+# test tiny, small, medium, and large numbers
+ELEMENT_SCALES = [10**i for i in range(-4, 5, 4)]
+
+# create a dictionary mapping each value of t found in TENSOR_SHAPES to an orthogonal
+# t x t matrix generated by scipy
+#
+# NOTE: This is done so that the _dummy_random_orthogonal_m_transform_generator function
+# below is deterministic; given the same value of t, it will return the same orthogonal
+# matrix M
+_T_LIST = [t for _, _, t in TENSOR_SHAPES]  # do not change this manually!
+M_MATRICES_DICT = {
+    t: M_mat
+    for t, M_mat in zip(
+        _T_LIST, [special_ortho_group.rvs(t, random_state=GLOBAL_RNG) for t in _T_LIST]
+    )
+}
 
 
 def _dummy_random_orthogonal_m_transform_generator(t):
-    """Let's test a m-transform defined by a random orthogonal matrix too!"""
-    M_mat = special_ortho_group.rvs(t, random_state=RNG)
+    """Generate a pair of m-transforms defined explicitly by an orthogonal matrix
+    Uses the M_MATRICES_DICT to find an appropriate matrix M corresponding to the input t
+    """
+    M_mat = M_MATRICES_DICT[t]
     M, Minv = generate_transform_pair_from_matrix(M_mat)
     return M, Minv
 
 
 def _dummy_default_transform_generator(t):
     """Return M=None, Minv=None to test default m-transform configuration"""
     return None, None
 
 
-# various n, p, t sizes
-# ensure n > p, p > n inputs are tested
-TENSOR_SHAPES = [(4, 3, 2), (5, 7, 6), (2, 2, 6)]
-
-# m transforms to suit the tensor sizes above
+# test various m transforms in the tred library to ensure they all produce reasonable
+# results when being used in tsvdm and TPCA
 TRANSFORM_FAMILY_GENERATORS = [
     _dummy_random_orthogonal_m_transform_generator,
     _dummy_default_transform_generator,
     generate_dctii_m_transform_pair,
     generate_dstii_m_transform_pair,
 ]
 
-# test tiny, small, medium, and large numbers
-ELEMENT_SCALES = [10**i for i in range(-4, 5, 4)]
-
 
 def _check_fitted_tpca_close(tpca1, tpca2, rtol, atol):
     """Check all of the fitted attributes of the two tpca classes
     NOTE: unused at the moment, but will likely be useful in future tests
     """
     assert_allclose(tpca1.n_, tpca2.n_, rtol=rtol, atol=atol)
     assert_allclose(tpca1.p_, tpca2.p_, rtol=rtol, atol=atol)
```

### Comparing `tred-0.1.1/tests/test_utils.py` & `tred-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tred/__init__.py` & `tred-0.1.2/tred/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 The `tred` module implements tensor decomposition methods such as tensor PCA and tensor 
 SVD. Most of the functionality in this module can be regarded as dimensionality reduction 
 strategies for order-3 datasets of size n, p, t, where p >> n > t. 
 """
 
+__version__ = "0.1.2"
+
 from ._m_transforms import (
     generate_transform_pair_from_matrix,
     generate_dstii_m_transform_pair,
     generate_dctii_m_transform_pair,
 )
 from ._tensor_ops import facewise_product, m_product
 from ._tensor_pca import generate_default_m_transform_pair, tsvdm, TPCA
```

### Comparing `tred-0.1.1/tred/_m_transforms.py` & `tred-0.1.2/tred/_m_transforms.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tred/_tensor_ops.py` & `tred-0.1.2/tred/_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tred/_tensor_pca.py` & `tred-0.1.2/tred/_tensor_pca.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/tred/_utils.py` & `tred-0.1.2/tred/_utils.py`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/.gitignore` & `tred-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/LICENSE` & `tred-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/README.txt` & `tred-0.1.2/README.txt`

 * *Files identical despite different names*

### Comparing `tred-0.1.1/pyproject.toml` & `tred-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tred"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Brendan Lu", email="brendannlu5@gmail.com" },
 ]
 description = "Dimensionality reduction techniques for order-3 tensors"
 readme = "README.txt"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tred-0.1.1/PKG-INFO` & `tred-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tred
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dimensionality reduction techniques for order-3 tensors
 Project-URL: Homepage, https://github.com/brendanlu/tred
 Project-URL: Issues, https://github.com/brendanlu/tred/issues
 Author-email: Brendan Lu <brendannlu5@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```
