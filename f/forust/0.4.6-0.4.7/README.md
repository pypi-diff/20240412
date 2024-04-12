# Comparing `tmp/forust-0.4.6.tar.gz` & `tmp/forust-0.4.7.tar.gz`

## Comparing `forust-0.4.6.tar` & `forust-0.4.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0      501       20      593 2024-03-24 17:40:12.000000 forust-0.4.6/Cargo.toml
--rw-r--r--   0      501       20     6951 2024-03-24 17:39:31.000000 forust-0.4.6/.github/workflows/CI.yml
--rw-r--r--   0      501       20      964 2024-03-24 17:39:31.000000 forust-0.4.6/.github/workflows/cargo-build-publish.yml
--rw-r--r--   0      501       20      733 2024-03-24 17:39:31.000000 forust-0.4.6/.github/workflows/docs.yml
--rw-r--r--   0      501       20      268 2024-03-24 17:39:31.000000 forust-0.4.6/.gitignore
--rw-r--r--   0      501       20      431 2024-03-24 17:39:31.000000 forust-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0      501       20     3533 2024-03-24 17:39:31.000000 forust-0.4.6/CONTRIBUTING.md
--rw-r--r--   0      501       20    11341 2024-03-24 17:39:31.000000 forust-0.4.6/LICENSE
--rw-r--r--   0      501       20     7350 2024-03-24 17:39:31.000000 forust-0.4.6/README.md
--rw-r--r--   0      501       20     5468 2024-03-24 17:39:31.000000 forust-0.4.6/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   513904 2024-03-24 17:41:12.000000 forust-0.4.6/dist/forust-0.4.6-cp312-cp312-macosx_10_12_x86_64.whl
--rw-r--r--   0      501       20    16121 2024-03-24 17:39:31.000000 forust-0.4.6/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2024-03-24 17:39:31.000000 forust-0.4.6/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2024-03-24 17:39:31.000000 forust-0.4.6/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2024-03-24 17:39:31.000000 forust-0.4.6/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2563 2024-03-24 17:39:31.000000 forust-0.4.6/rs-example.md
--rw-r--r--   0      501       20     1271 2024-03-24 17:39:31.000000 forust-0.4.6/scripts/make_resources.py
--rw-r--r--   0      501       20      370 2024-03-24 17:39:31.000000 forust-0.4.6/scripts/remove-optional-deps.py
--rw-r--r--   0      501       20       53 2024-03-24 17:39:31.000000 forust-0.4.6/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2024-03-24 17:39:31.000000 forust-0.4.6/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5647 2024-03-24 17:39:31.000000 forust-0.4.6/src/binning.rs
--rw-r--r--   0      501       20      248 2024-03-24 17:39:31.000000 forust-0.4.6/src/constraints.rs
--rw-r--r--   0      501       20    10051 2024-03-24 17:39:31.000000 forust-0.4.6/src/data.rs
--rw-r--r--   0      501       20      945 2024-03-24 17:39:31.000000 forust-0.4.6/src/errors.rs
--rw-r--r--   0      501       20    56880 2024-03-24 17:39:31.000000 forust-0.4.6/src/gradientbooster.rs
--rw-r--r--   0      501       20      881 2024-03-24 17:39:31.000000 forust-0.4.6/src/grower.rs
--rw-r--r--   0      501       20     9977 2024-03-24 17:39:31.000000 forust-0.4.6/src/histogram.rs
--rw-r--r--   0      501       20      384 2024-03-24 17:39:31.000000 forust-0.4.6/src/lib.rs
--rw-r--r--   0      501       20     8933 2024-03-24 17:39:31.000000 forust-0.4.6/src/metric.rs
--rw-r--r--   0      501       20     6863 2024-03-24 17:39:31.000000 forust-0.4.6/src/node.rs
--rw-r--r--   0      501       20     5956 2024-03-24 17:39:31.000000 forust-0.4.6/src/objective.rs
--rw-r--r--   0      501       20     4195 2024-03-24 17:39:31.000000 forust-0.4.6/src/partial_dependence.rs
--rw-r--r--   0      501       20     2923 2024-03-24 17:39:31.000000 forust-0.4.6/src/sampler.rs
--rw-r--r--   0      501       20     8072 2024-03-24 17:39:31.000000 forust-0.4.6/src/shapley.rs
--rw-r--r--   0      501       20    41163 2024-03-24 17:39:31.000000 forust-0.4.6/src/splitter.rs
--rw-r--r--   0      501       20    33349 2024-03-24 17:39:31.000000 forust-0.4.6/src/tree.rs
--rw-r--r--   0      501       20    35433 2024-03-24 17:39:31.000000 forust-0.4.6/src/utils.rs
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 forust-0.4.6/py-forust/Cargo.toml
--rw-r--r--   0      501       20      685 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/.gitignore
--rw-r--r--   0      501       20     7350 2024-03-24 17:40:12.000000 forust-0.4.6/py-forust/README.md
--rw-r--r--   0      501       20     1634 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/docs/index.md
--rw-r--r--   0      501       20    54682 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/forust/__init__.py
--rw-r--r--   0      501       20     1870 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/forust/serialize.py
--rw-r--r--   0      501       20     1192 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/mkdocs.yml
--rw-r--r--   0      501       20    16022 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/src/lib.rs
--rw-r--r--   0      501       20    55097 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/tests/test_booster.py
--rw-r--r--   0      501       20     1318 2024-03-24 17:39:31.000000 forust-0.4.6/py-forust/tests/test_serailze.py
--rw-r--r--   0      501       20    15147 2024-03-24 17:40:40.000000 forust-0.4.6/py-forust/Cargo.lock
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 forust-0.4.6/pyproject.toml
--rw-r--r--   0      501       20     1870 2024-03-24 17:39:31.000000 forust-0.4.6/forust/serialize.py
--rw-r--r--   0      501       20    54682 2024-03-24 17:39:31.000000 forust-0.4.6/forust/__init__.py
--rw-r--r--   0        0        0     8353 1970-01-01 00:00:00.000000 forust-0.4.6/PKG-INFO
+-rw-r--r--   0     1001      127      593 2024-04-12 16:25:13.000000 forust-0.4.7/Cargo.toml
+-rw-r--r--   0     1001      127     6951 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      964 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/cargo-build-publish.yml
+-rw-r--r--   0     1001      127      733 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127      268 2024-04-12 16:24:35.000000 forust-0.4.7/.gitignore
+-rw-r--r--   0     1001      127      431 2024-04-12 16:24:35.000000 forust-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     3533 2024-04-12 16:24:35.000000 forust-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0     1001      127    11341 2024-04-12 16:24:35.000000 forust-0.4.7/LICENSE
+-rw-r--r--   0     1001      127     7350 2024-04-12 16:24:35.000000 forust-0.4.7/README.md
+-rw-r--r--   0     1001      127     5468 2024-04-12 16:24:35.000000 forust-0.4.7/benches/forust_benchmarks.rs
+-rw-r--r--   0     1001      127   566309 2024-04-12 16:26:38.000000 forust-0.4.7/dist/forust-0.4.7-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+-rw-r--r--   0     1001      127    16121 2024-04-12 16:24:35.000000 forust-0.4.7/resources/pdp_plot_age.png
+-rw-r--r--   0     1001      127    10758 2024-04-12 16:24:35.000000 forust-0.4.7/resources/pdp_plot_age_mono.png
+-rw-r--r--   0     1001      127    57018 2024-04-12 16:24:35.000000 forust-0.4.7/resources/titanic.csv
+-rw-r--r--   0     1001      127   655700 2024-04-12 16:24:35.000000 forust-0.4.7/resources/tree-image-crop.png
+-rw-r--r--   0     1001      127     2563 2024-04-12 16:24:35.000000 forust-0.4.7/rs-example.md
+-rw-r--r--   0     1001      127     1271 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/make_resources.py
+-rw-r--r--   0     1001      127      370 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/remove-optional-deps.py
+-rw-r--r--   0     1001      127       53 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/run-python-tests.ps1
+-rw-r--r--   0     1001      127       53 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/run-python-tests.sh
+-rw-r--r--   0     1001      127     5647 2024-04-12 16:24:35.000000 forust-0.4.7/src/binning.rs
+-rw-r--r--   0     1001      127      248 2024-04-12 16:24:35.000000 forust-0.4.7/src/constraints.rs
+-rw-r--r--   0     1001      127    10051 2024-04-12 16:24:35.000000 forust-0.4.7/src/data.rs
+-rw-r--r--   0     1001      127      945 2024-04-12 16:24:35.000000 forust-0.4.7/src/errors.rs
+-rw-r--r--   0     1001      127    57204 2024-04-12 16:24:35.000000 forust-0.4.7/src/gradientbooster.rs
+-rw-r--r--   0     1001      127      881 2024-04-12 16:24:35.000000 forust-0.4.7/src/grower.rs
+-rw-r--r--   0     1001      127     9977 2024-04-12 16:24:35.000000 forust-0.4.7/src/histogram.rs
+-rw-r--r--   0     1001      127      384 2024-04-12 16:24:35.000000 forust-0.4.7/src/lib.rs
+-rw-r--r--   0     1001      127     8933 2024-04-12 16:24:35.000000 forust-0.4.7/src/metric.rs
+-rw-r--r--   0     1001      127     6863 2024-04-12 16:24:35.000000 forust-0.4.7/src/node.rs
+-rw-r--r--   0     1001      127     5956 2024-04-12 16:24:35.000000 forust-0.4.7/src/objective.rs
+-rw-r--r--   0     1001      127     4195 2024-04-12 16:24:35.000000 forust-0.4.7/src/partial_dependence.rs
+-rw-r--r--   0     1001      127     2923 2024-04-12 16:24:35.000000 forust-0.4.7/src/sampler.rs
+-rw-r--r--   0     1001      127     8072 2024-04-12 16:24:35.000000 forust-0.4.7/src/shapley.rs
+-rw-r--r--   0     1001      127    41163 2024-04-12 16:24:35.000000 forust-0.4.7/src/splitter.rs
+-rw-r--r--   0     1001      127    33600 2024-04-12 16:24:35.000000 forust-0.4.7/src/tree.rs
+-rw-r--r--   0     1001      127    35433 2024-04-12 16:24:35.000000 forust-0.4.7/src/utils.rs
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 forust-0.4.7/py-forust/Cargo.toml
+-rw-r--r--   0     1001      127      685 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/.gitignore
+-rw-r--r--   0     1001      127     7350 2024-04-12 16:25:13.000000 forust-0.4.7/py-forust/README.md
+-rw-r--r--   0     1001      127     1634 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/docs/index.md
+-rw-r--r--   0     1001      127    55983 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/forust/__init__.py
+-rw-r--r--   0     1001      127     1870 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/forust/serialize.py
+-rw-r--r--   0     1001      127     1192 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/mkdocs.yml
+-rw-r--r--   0     1001      127    16405 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/src/lib.rs
+-rw-r--r--   0     1001      127    55742 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/tests/test_booster.py
+-rw-r--r--   0     1001      127     1318 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/tests/test_serailze.py
+-rw-r--r--   0     1001      127    15147 2024-04-12 16:25:59.000000 forust-0.4.7/py-forust/Cargo.lock
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 forust-0.4.7/pyproject.toml
+-rw-r--r--   0     1001      127    55983 2024-04-12 16:24:35.000000 forust-0.4.7/forust/__init__.py
+-rw-r--r--   0     1001      127     1870 2024-04-12 16:24:35.000000 forust-0.4.7/forust/serialize.py
+-rw-r--r--   0        0        0     8353 1970-01-01 00:00:00.000000 forust-0.4.7/PKG-INFO
```

### Comparing `forust-0.4.6/Cargo.toml` & `forust-0.4.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.4.6"
+version = "0.4.7"
 edition = "2021"
 authors = [ "James Inlow <james.d.inlow@gmail.com>",]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.4.6/.github/workflows/CI.yml` & `forust-0.4.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/.github/workflows/cargo-build-publish.yml` & `forust-0.4.7/.github/workflows/cargo-build-publish.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/.github/workflows/docs.yml` & `forust-0.4.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/CONTRIBUTING.md` & `forust-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/LICENSE` & `forust-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/README.md` & `forust-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.6"
+forust-ml = "0.4.7"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.6" ``` ## Usage For details on all of the methods and their respective
+"0.4.7" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

### Comparing `forust-0.4.6/benches/forust_benchmarks.rs` & `forust-0.4.7/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/resources/pdp_plot_age.png` & `forust-0.4.7/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/resources/pdp_plot_age_mono.png` & `forust-0.4.7/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/resources/titanic.csv` & `forust-0.4.7/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/resources/tree-image-crop.png` & `forust-0.4.7/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/rs-example.md` & `forust-0.4.7/rs-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.4.6"
+forust-ml = "0.4.7"
 polars = "0.28"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.4.6/scripts/make_resources.py` & `forust-0.4.7/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/binning.rs` & `forust-0.4.7/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/data.rs` & `forust-0.4.7/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/errors.rs` & `forust-0.4.7/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/gradientbooster.rs` & `forust-0.4.7/src/gradientbooster.rs`

 * *Files 1% similar despite different names*

```diff
@@ -739,14 +739,22 @@
             {
                 *p_ += val;
             }
         });
         init_preds
     }
 
+    /// Predict the leaf Indexes, this returns a vector of length N records * N Trees
+    pub fn predict_leaf_indices(&self, data: &Matrix<f64>) -> Vec<usize> {
+        self.get_prediction_trees()
+            .iter()
+            .flat_map(|tree| tree.predict_leaf_indices(data, &self.missing))
+            .collect()
+    }
+
     /// Predict the contributions matrix for the provided dataset.
     pub fn predict_contributions(
         &self,
         data: &Matrix<f64>,
         method: ContributionsMethod,
         parallel: bool,
     ) -> Vec<f64> {
```

### Comparing `forust-0.4.6/src/grower.rs` & `forust-0.4.7/src/grower.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/histogram.rs` & `forust-0.4.7/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/metric.rs` & `forust-0.4.7/src/metric.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/node.rs` & `forust-0.4.7/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/objective.rs` & `forust-0.4.7/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/partial_dependence.rs` & `forust-0.4.7/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/sampler.rs` & `forust-0.4.7/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/shapley.rs` & `forust-0.4.7/src/shapley.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/splitter.rs` & `forust-0.4.7/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/src/tree.rs` & `forust-0.4.7/src/tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -389,20 +389,20 @@
                     contribs,
                     weights,
                     missing,
                 )
             })
     }
 
-    fn predict_row(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> f64 {
+    fn predict_leaf(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> &Node {
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
             if node.is_leaf {
-                return node.weight_value as f64;
+                return node;
             } else {
                 node_idx = node.get_child_idx(data.get(row, node.split_feature), missing);
             }
         }
     }
 
     pub fn predict_row_from_row_slice(&self, row: &[f64], missing: &f64) -> f64 {
@@ -416,33 +416,40 @@
             }
         }
     }
 
     fn predict_single_threaded(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
         data.index
             .iter()
-            .map(|i| self.predict_row(data, *i, missing))
+            .map(|i| self.predict_leaf(data, *i, missing).weight_value as f64)
             .collect()
     }
 
     fn predict_parallel(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
         data.index
             .par_iter()
-            .map(|i| self.predict_row(data, *i, missing))
+            .map(|i| self.predict_leaf(data, *i, missing).weight_value as f64)
             .collect()
     }
 
     pub fn predict(&self, data: &Matrix<f64>, parallel: bool, missing: &f64) -> Vec<f64> {
         if parallel {
             self.predict_parallel(data, missing)
         } else {
             self.predict_single_threaded(data, missing)
         }
     }
 
+    pub fn predict_leaf_indices(&self, data: &Matrix<f64>, missing: &f64) -> Vec<usize> {
+        data.index
+            .par_iter()
+            .map(|i| self.predict_leaf(data, *i, missing).num)
+            .collect()
+    }
+
     pub fn value_partial_dependence(&self, feature: usize, value: f64, missing: &f64) -> f64 {
         tree_partial_dependence(self, 0, feature, value, 1.0, missing)
     }
     fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
         let node = &self.nodes[i];
         let mut w = node.weight_value as f64;
         if !node.is_leaf {
```

### Comparing `forust-0.4.6/src/utils.rs` & `forust-0.4.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/.gitignore` & `forust-0.4.7/py-forust/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/README.md` & `forust-0.4.7/py-forust/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.6"
+forust-ml = "0.4.7"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.6" ``` ## Usage For details on all of the methods and their respective
+"0.4.7" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

### Comparing `forust-0.4.6/py-forust/docs/index.md` & `forust-0.4.7/py-forust/docs/index.md`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/forust/__init__.py` & `forust-0.4.7/py-forust/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,22 @@
         rows: int,
         cols: int,
         method: str,
         parallel: bool = True,
     ) -> np.ndarray:
         """method"""
 
+    def predict_leaf_indices(
+        self,
+        flat_data: np.ndarray,
+        rows: int,
+        cols: int,
+    ) -> np.ndarray:
+        """method"""
+
     def value_partial_dependence(
         self,
         feature: int,
         value: float,
     ) -> float:
         """pass"""
 
@@ -694,29 +702,52 @@
                 - "ProbabilityChange": This method is only valid when the objective type is set to "LogLoss". This method will calculate contributions as the change in a records probability of being 1 moving from a parent node to a child node. The sum of the returned contributions matrix, will be equal to the probability a record will be 1. For example, given a model, `model.predict_contributions(X, method="ProbabilityChange") == 1 / (1 + np.exp(-model.predict(X)))`
             parallel (Union[bool, None], optional): Optionally specify if the predict
                 function should run in parallel on multiple threads. If `None` is
                 passed, the `parallel` attribute of the booster will be used.
                 Defaults to `None`.
 
         Returns:
-            np.ndarray: Returns a numpy array of the predictions.
+            np.ndarray: Returns a numpy array of the predicted contributions.
         """
         features_, flat_data, rows, cols = _convert_input_frame(X)
         self._validate_features(features_)
         parallel_ = self.parallel if parallel is None else parallel
 
         contributions = self.booster.predict_contributions(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
             method=CONTRIBUTION_METHODS.get(method, method),
             parallel=parallel_,
         )
         return np.reshape(contributions, (rows, cols + 1))
 
+    def predict_leaf_indices(self, X: FrameLike) -> np.ndarray:
+        """Predict the leaf indices for each tree. This will be the node ID number, this can be used to identify the leaf node a record will fall into for each row, this could be paired directly with the `trees_to_dataframe` output. The data returned will be a matrix, where each column corresponds to a tree, thus the data will be of the shape (rows in X, prediction_iteration)
+
+        Args:
+            X (FrameLike): Either a pandas DataFrame, or a 2 dimensional numpy array.
+
+        Returns:
+            np.ndarray: Returns a numpy array of the predicted leaf indices..
+        """
+        features_, flat_data, rows, cols = _convert_input_frame(X)
+        self._validate_features(features_)
+        leaf_indices = self.booster.predict_leaf_indices(
+            flat_data=flat_data,
+            rows=rows,
+            cols=cols,
+        )
+        n_trees = (
+            self.number_of_trees
+            if self.prediction_iteration is None
+            else self.prediction_iteration
+        )
+        return np.reshape(leaf_indices, (rows, n_trees), order="F")
+
     def set_prediction_iteration(self, iteration: int):
         """Set the iteration that should be used when predicting. If `early_stopping_rounds`
         has been set, this will default to the best iteration, otherwise all of the trees
         will be used.
 
         Args:
             iteration (int): Iteration number to use, this will use all trees, up to this
```

### Comparing `forust-0.4.6/py-forust/forust/serialize.py` & `forust-0.4.7/py-forust/forust/serialize.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/mkdocs.yml` & `forust-0.4.7/py-forust/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/src/lib.rs` & `forust-0.4.7/py-forust/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,26 @@
         let method_ = to_value_error(serde_plain::from_str(method))?;
         Ok(self
             .booster
             .predict_contributions(&data, method_, parallel)
             .into_pyarray(py))
     }
 
+    pub fn predict_leaf_indices<'py>(
+        &self,
+        py: Python<'py>,
+        flat_data: PyReadonlyArray1<f64>,
+        rows: usize,
+        cols: usize,
+    ) -> PyResult<&'py PyArray1<usize>> {
+        let flat_data = flat_data.as_slice()?;
+        let data = Matrix::new(flat_data, rows, cols);
+        Ok(self.booster.predict_leaf_indices(&data).into_pyarray(py))
+    }
+
     pub fn calculate_feature_importance(
         &self,
         method: &str,
         normalize: bool,
     ) -> PyResult<HashMap<usize, f32>> {
         let method_ = to_value_error(serde_plain::from_str(method))?;
         Ok(self
```

### Comparing `forust-0.4.6/py-forust/tests/test_booster.py` & `forust-0.4.7/py-forust/tests/test_booster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1641,14 +1641,31 @@
         parameters,
         scoring=lambda est, X, y: roc_auc_score(y, est.predict(X)),
     )
     clf.fit(X, y)
     assert len(clf.cv_results_["mean_test_score"]) > 0
 
 
+def test_leaf_preds(X_y):
+    X, y = X_y
+    fmod = GradientBooster()
+    # We should be able to use the leaf predictions matrix, and the model dump
+    # to actually generate the predictions.
+    fmod.fit(X, y)
+    nodes = fmod.get_node_lists()
+    initial_preds = np.repeat(fmod.base_score, y.shape)
+    leaf_preds = fmod.predict_leaf_indices(X)
+    for i, tree in enumerate(nodes):
+        node_map = {node.num: node.weight_value for node in tree}
+        tree_preds = np.array([node_map[tv] for tv in leaf_preds[:, i]])
+        initial_preds += tree_preds
+    real_preds = fmod.predict(X)
+    assert np.allclose(real_preds, initial_preds)
+
+
 # All save and load methods
 @pytest.mark.parametrize(
     "load_func,save_func",
     [(unpickle_booster, pickle_booster), (load_booster, save_booster)],
 )
 class TestSaveLoadFunctions:
     def test_early_stopping_rounds(
```

### Comparing `forust-0.4.6/py-forust/tests/test_serailze.py` & `forust-0.4.7/py-forust/tests/test_serailze.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/py-forust/Cargo.lock` & `forust-0.4.7/py-forust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 name = "arc-swap"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -55,29 +55,29 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "forust-ml"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
  "log",
  "rand",
  "rayon",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -90,17 +90,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
@@ -128,17 +128,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
@@ -242,15 +242,15 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-forust"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
  "forust-ml",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-log",
  "serde",
@@ -329,17 +329,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -441,17 +441,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -467,17 +467,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `forust-0.4.6/pyproject.toml` & `forust-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/forust/serialize.py` & `forust-0.4.7/forust/serialize.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.6/forust/__init__.py` & `forust-0.4.7/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,22 @@
         rows: int,
         cols: int,
         method: str,
         parallel: bool = True,
     ) -> np.ndarray:
         """method"""
 
+    def predict_leaf_indices(
+        self,
+        flat_data: np.ndarray,
+        rows: int,
+        cols: int,
+    ) -> np.ndarray:
+        """method"""
+
     def value_partial_dependence(
         self,
         feature: int,
         value: float,
     ) -> float:
         """pass"""
 
@@ -694,29 +702,52 @@
                 - "ProbabilityChange": This method is only valid when the objective type is set to "LogLoss". This method will calculate contributions as the change in a records probability of being 1 moving from a parent node to a child node. The sum of the returned contributions matrix, will be equal to the probability a record will be 1. For example, given a model, `model.predict_contributions(X, method="ProbabilityChange") == 1 / (1 + np.exp(-model.predict(X)))`
             parallel (Union[bool, None], optional): Optionally specify if the predict
                 function should run in parallel on multiple threads. If `None` is
                 passed, the `parallel` attribute of the booster will be used.
                 Defaults to `None`.
 
         Returns:
-            np.ndarray: Returns a numpy array of the predictions.
+            np.ndarray: Returns a numpy array of the predicted contributions.
         """
         features_, flat_data, rows, cols = _convert_input_frame(X)
         self._validate_features(features_)
         parallel_ = self.parallel if parallel is None else parallel
 
         contributions = self.booster.predict_contributions(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
             method=CONTRIBUTION_METHODS.get(method, method),
             parallel=parallel_,
         )
         return np.reshape(contributions, (rows, cols + 1))
 
+    def predict_leaf_indices(self, X: FrameLike) -> np.ndarray:
+        """Predict the leaf indices for each tree. This will be the node ID number, this can be used to identify the leaf node a record will fall into for each row, this could be paired directly with the `trees_to_dataframe` output. The data returned will be a matrix, where each column corresponds to a tree, thus the data will be of the shape (rows in X, prediction_iteration)
+
+        Args:
+            X (FrameLike): Either a pandas DataFrame, or a 2 dimensional numpy array.
+
+        Returns:
+            np.ndarray: Returns a numpy array of the predicted leaf indices..
+        """
+        features_, flat_data, rows, cols = _convert_input_frame(X)
+        self._validate_features(features_)
+        leaf_indices = self.booster.predict_leaf_indices(
+            flat_data=flat_data,
+            rows=rows,
+            cols=cols,
+        )
+        n_trees = (
+            self.number_of_trees
+            if self.prediction_iteration is None
+            else self.prediction_iteration
+        )
+        return np.reshape(leaf_indices, (rows, n_trees), order="F")
+
     def set_prediction_iteration(self, iteration: int):
         """Set the iteration that should be used when predicting. If `early_stopping_rounds`
         has been set, this will default to the best iteration, otherwise all of the trees
         will be used.
 
         Args:
             iteration (int): Iteration number to use, this will use all trees, up to this
```

### Comparing `forust-0.4.6/PKG-INFO` & `forust-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: forust
-Version: 0.4.6
+Version: 0.4.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.21
 Requires-Dist: pandas >=1.3
 Requires-Dist: maturin ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
@@ -50,15 +50,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.6"
+forust-ml = "0.4.7"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: forust Version: 0.4.6 Classifier: Programming
+Metadata-Version: 2.3 Name: forust Version: 0.4.7 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.21 Requires-Dist: pandas >=1.3 Requires-Dist: maturin
 ; extra == 'dev' Requires-Dist: pytest ; extra == 'dev' Requires-Dist: seaborn
 ; extra == 'dev' Requires-Dist: xgboost ==1.6.1 ; extra == 'dev' Requires-Dist:
 scikit-learn ; extra == 'dev' Requires-Dist: mkdocs-material ==9.* ; extra ==
 'dev' Requires-Dist: mkdocstrings[python] ==0.22.0 ; extra == 'dev' Requires-
@@ -28,15 +28,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.6" ``` ## Usage For details on all of the methods and their respective
+"0.4.7" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

