# Comparing `tmp/approx_umap-0.1.1.tar.gz` & `tmp/approx_umap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approx_umap-0.1.1.tar", max compression
+gzip compressed data, was "approx_umap-0.1.2.tar", max compression
```

## Comparing `approx_umap-0.1.1.tar` & `approx_umap-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.1.1/LICENSE
--rw-r--r--   0        0        0     2116 2024-04-10 06:57:58.332889 approx_umap-0.1.1/README.md
--rw-r--r--   0        0        0       46 2024-04-03 16:17:03.972887 approx_umap-0.1.1/approx_umap/__init__.py
--rw-r--r--   0        0        0     5399 2024-04-03 16:58:35.915758 approx_umap-0.1.1/approx_umap/approx_umap.py
--rw-r--r--   0        0        0      639 2024-04-10 07:21:45.707931 approx_umap-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 approx_umap-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-03 17:09:04.702968 approx_umap-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2116 2024-04-12 11:32:14.902620 approx_umap-0.1.2/README.md
+-rw-r--r--   0        0        0       46 2024-04-12 11:31:51.625854 approx_umap-0.1.2/approx_umap/__init__.py
+-rw-r--r--   0        0        0     5512 2024-04-12 11:34:31.791489 approx_umap-0.1.2/approx_umap/approx_umap.py
+-rw-r--r--   0        0        0      710 2024-04-12 11:36:38.157165 approx_umap-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 approx_umap-0.1.2/PKG-INFO
```

### Comparing `approx_umap-0.1.1/LICENSE` & `approx_umap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `approx_umap-0.1.1/README.md` & `approx_umap-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,12 +51,12 @@
 
 ```bibtex
 @inproceedings{approx-umap2024,
     title = {Approximate UMAP allows for high-rate online visualization of high-dimensional data streams},
     author = {Peter Wassenaar and Pierre Guetschel and Michael Tangermann},
     year = {2024},
     month = {September},
-    booktitle = {8th Graz Brain-Computer Interface Conference},
+    booktitle = {9th Graz Brain-Computer Interface Conference},
     address = {Graz, Austria},
     url = {https://arxiv.org/abs/2404.04001},
 }
 ```
```

### Comparing `approx_umap-0.1.1/approx_umap/approx_umap.py` & `approx_umap-0.1.2/approx_umap/approx_umap.py`

 * *Files 9% similar despite different names*

```diff
@@ -120,14 +120,16 @@
                                      Values cannot be infinite.
 
         Returns
         -------
         X_new : array, shape (n_samples, n_components)
             Approximate embedding of the new data in low-dimensional space.
         """
-        neigh_dist, neigh_ind = self._knn.kneighbors(X, return_distance=True)
+        n_neighbors = min(self._knn.n_neighbors, self.embedding_.shape[0])
+        neigh_dist, neigh_ind = self._knn.kneighbors(
+            X, n_neighbors=n_neighbors, return_distance=True)
         neigh_emb = self.embedding_[neigh_ind]
         epsilon = 1e-8
         neigh_sim = 1 / (neigh_dist + epsilon)
         emb = np.sum(neigh_sim[:, :, None] / neigh_sim.sum(axis=1)[:, None, None] * neigh_emb,
                      axis=1)
         return emb
```

### Comparing `approx_umap-0.1.1/pyproject.toml` & `approx_umap-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approx-umap"
-version = "0.1.1"
+version = "0.1.2"
 description = "Modification of the UMAP algorithm to allow for fast approximate projections of new data points."
 authors = [
     "Pierre Guetschel <pierre.guetschel@donders.ru.nl>",
     "Peter Wassenaar <peter.wassenaar@ru.nl>",
 ]
 readme = "README.md"
 packages = [{ include = "approx_umap" }]
@@ -17,10 +17,14 @@
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 
 
+
+[tool.poetry.group.parametric_umap.dependencies]
+tensorflow = "^2.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `approx_umap-0.1.1/PKG-INFO` & `approx_umap-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approx-umap
-Version: 0.1.1
+Version: 0.1.2
 Summary: Modification of the UMAP algorithm to allow for fast approximate projections of new data points.
 Home-page: https://github.com/PierreGtch/approx-umap
 License: BSD-3-Clause
 Author: Pierre Guetschel
 Author-email: pierre.guetschel@donders.ru.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -68,12 +68,12 @@
 
 ```bibtex
 @inproceedings{approx-umap2024,
     title = {Approximate UMAP allows for high-rate online visualization of high-dimensional data streams},
     author = {Peter Wassenaar and Pierre Guetschel and Michael Tangermann},
     year = {2024},
     month = {September},
-    booktitle = {8th Graz Brain-Computer Interface Conference},
+    booktitle = {9th Graz Brain-Computer Interface Conference},
     address = {Graz, Austria},
     url = {https://arxiv.org/abs/2404.04001},
 }
 ```
```

