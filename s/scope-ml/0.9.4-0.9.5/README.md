# Comparing `tmp/scope_ml-0.9.4.tar.gz` & `tmp/scope_ml-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope_ml-0.9.4.tar", max compression
+gzip compressed data, was "scope_ml-0.9.5.tar", max compression
```

## Comparing `scope_ml-0.9.4.tar` & `scope_ml-0.9.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1082 2024-04-10 16:31:38.197965 scope_ml-0.9.4/LICENSE
--rw-r--r--   0        0        0     1427 2024-04-10 16:31:38.197965 scope_ml-0.9.4/README.md
--rw-r--r--   0        0        0    55490 2024-04-10 16:31:38.209965 scope_ml-0.9.4/config.defaults.yaml
--rw-r--r--   0        0        0     3527 2024-04-10 16:31:38.305965 scope_ml-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     2755 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/__init__.py
--rw-r--r--   0        0        0      597 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/_instantiate.py
--rwxr-xr-x   0        0        0    13601 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/fritz.py
--rw-r--r--   0        0        0      883 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/models.py
--rw-r--r--   0        0        0    21602 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/nn.py
--rwxr-xr-x   0        0        0   113350 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/scope_class.py
--rw-r--r--   0        0        0    45857 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/utils.py
--rw-r--r--   0        0        0    20264 2024-04-10 16:31:38.305965 scope_ml-0.9.4/scope/xgb.py
--rw-r--r--   0        0        0     4163 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/DNN_AL_mapper.json
--rw-r--r--   0        0        0     4163 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/XGB_AL_mapper.json
--rwxr-xr-x   0        0        0     4346 2024-04-10 16:31:38.305965 scope_ml-0.9.4/tools/analyze_logs.py
--rwxr-xr-x   0        0        0    11958 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/combine_preds.py
--rwxr-xr-x   0        0        0     4338 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/combine_preds_slurm.py
--rw-r--r--   0        0        0     3775 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/alertstats.py
--rw-r--r--   0        0        0     5460 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/external_xmatch.py
--rw-r--r--   0        0        0    12658 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/lcstats.py
--rw-r--r--   0        0        0    19686 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/periodsearch.py
--rw-r--r--   0        0        0        0 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/__init__.py
--rw-r--r--   0        0        0    29593 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aov.f90
--rw-r--r--   0        0        0      545 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aovconst.f90
--rw-r--r--   0        0        0     9369 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/aovsub.f90
--rw-r--r--   0        0        0      218 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/featureGeneration/pyaov/build.sh
--rw-r--r--   0        0        0     3983 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/fritz_mapper.json
--rwxr-xr-x   0        0        0    56855 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features.py
--rwxr-xr-x   0        0        0    12036 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features_job_submission.py
--rwxr-xr-x   0        0        0    20587 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/generate_features_slurm.py
--rwxr-xr-x   0        0        0    18037 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/get_features.py
--rwxr-xr-x   0        0        0    17448 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/get_quad_ids.py
--rw-r--r--   0        0        0     4334 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/golden_dataset_mapper.json
--rwxr-xr-x   0        0        0    28896 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/inference.py
--rw-r--r--   0        0        0       92 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/local_scope_radec.csv
--rw-r--r--   0        0        0       77 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/local_scope_ztfid.csv
--rwxr-xr-x   0        0        0     2652 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_inference_job_submission.py
--rwxr-xr-x   0        0        0     6811 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_inference_slurm.py
--rwxr-xr-x   0        0        0    12544 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/run_scope_local.py
--rwxr-xr-x   0        0        0    30136 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_download_classification.py
--rwxr-xr-x   0        0        0     6900 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_download_gcn_sources.py
--rwxr-xr-x   0        0        0     8254 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_manage_annotation.py
--rwxr-xr-x   0        0        0    34114 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_upload_classification.py
--rw-r--r--   0        0        0     3121 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/scope_upload_disagreements.py
--rwxr-xr-x   0        0        0     3873 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/taxonomy.py
--rwxr-xr-x   0        0        0     8018 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/train_algorithm_job_submission.py
--rwxr-xr-x   0        0        0     9212 2024-04-10 16:31:38.309965 scope_ml-0.9.4/tools/train_algorithm_slurm.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 scope_ml-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-12 18:19:40.971413 scope_ml-0.9.5/LICENSE
+-rw-r--r--   0        0        0     1427 2024-04-12 18:19:40.971413 scope_ml-0.9.5/README.md
+-rw-r--r--   0        0        0    55490 2024-04-12 18:19:40.983413 scope_ml-0.9.5/config.defaults.yaml
+-rw-r--r--   0        0        0     3527 2024-04-12 18:19:41.075414 scope_ml-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2755 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/_instantiate.py
+-rwxr-xr-x   0        0        0    13601 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/fritz.py
+-rw-r--r--   0        0        0      883 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/models.py
+-rw-r--r--   0        0        0    21602 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/nn.py
+-rwxr-xr-x   0        0        0   112988 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/scope_class.py
+-rw-r--r--   0        0        0    45911 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/utils.py
+-rw-r--r--   0        0        0    20264 2024-04-12 18:19:41.079414 scope_ml-0.9.5/scope/xgb.py
+-rw-r--r--   0        0        0     4163 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/DNN_AL_mapper.json
+-rw-r--r--   0        0        0     4163 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/XGB_AL_mapper.json
+-rwxr-xr-x   0        0        0     4346 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/analyze_logs.py
+-rwxr-xr-x   0        0        0    12139 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/combine_preds.py
+-rwxr-xr-x   0        0        0     4338 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/combine_preds_slurm.py
+-rw-r--r--   0        0        0     3775 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/alertstats.py
+-rw-r--r--   0        0        0     5460 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/external_xmatch.py
+-rw-r--r--   0        0        0    12658 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/lcstats.py
+-rw-r--r--   0        0        0    19686 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/periodsearch.py
+-rw-r--r--   0        0        0        0 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/pyaov/__init__.py
+-rw-r--r--   0        0        0    29593 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/pyaov/aov.f90
+-rw-r--r--   0        0        0      545 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/pyaov/aovconst.f90
+-rw-r--r--   0        0        0     9369 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/pyaov/aovsub.f90
+-rw-r--r--   0        0        0      218 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/featureGeneration/pyaov/build.sh
+-rw-r--r--   0        0        0     3983 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/fritz_mapper.json
+-rwxr-xr-x   0        0        0    56855 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/generate_features.py
+-rwxr-xr-x   0        0        0    12036 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/generate_features_job_submission.py
+-rwxr-xr-x   0        0        0    20587 2024-04-12 18:19:41.079414 scope_ml-0.9.5/tools/generate_features_slurm.py
+-rwxr-xr-x   0        0        0    18037 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/get_features.py
+-rwxr-xr-x   0        0        0    17448 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/get_quad_ids.py
+-rw-r--r--   0        0        0     4334 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/golden_dataset_mapper.json
+-rwxr-xr-x   0        0        0    28896 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/inference.py
+-rw-r--r--   0        0        0       92 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/local_scope_radec.csv
+-rw-r--r--   0        0        0       77 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/local_scope_ztfid.csv
+-rwxr-xr-x   0        0        0     2652 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/run_inference_job_submission.py
+-rwxr-xr-x   0        0        0     6811 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/run_inference_slurm.py
+-rwxr-xr-x   0        0        0    12544 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/run_scope_local.py
+-rwxr-xr-x   0        0        0    30136 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/scope_download_classification.py
+-rwxr-xr-x   0        0        0     6900 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/scope_download_gcn_sources.py
+-rwxr-xr-x   0        0        0     8254 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/scope_manage_annotation.py
+-rwxr-xr-x   0        0        0    34114 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/scope_upload_classification.py
+-rw-r--r--   0        0        0     3121 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/scope_upload_disagreements.py
+-rwxr-xr-x   0        0        0     3873 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/taxonomy.py
+-rwxr-xr-x   0        0        0     8018 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/train_algorithm_job_submission.py
+-rwxr-xr-x   0        0        0     9212 2024-04-12 18:19:41.083414 scope_ml-0.9.5/tools/train_algorithm_slurm.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 scope_ml-0.9.5/PKG-INFO
```

### Comparing `scope_ml-0.9.4/LICENSE` & `scope_ml-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/README.md` & `scope_ml-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/config.defaults.yaml` & `scope_ml-0.9.5/config.defaults.yaml`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/pyproject.toml` & `scope_ml-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 target-version = ['py39', 'py310', 'py311']
 skip-string-normalization = true
 
 [tool.poetry]
 name = "scope-ml"
-version = "0.9.4"
+version = "0.9.5"
 description = "SCoPe: ZTF Source Classification Project"
 readme = "README.md"
 authors = ["Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al."]
 maintainers = ["Brian F. Healy <healyb@umn.edu>"]
 license = "MIT"
 repository = "https://github.com/ZwickyTransientFacility/scope"
 documentation = "https://zwickytransientfacility.github.io/scope-docs/"
```

### Comparing `scope_ml-0.9.4/scope/__init__.py` & `scope_ml-0.9.5/scope/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import os
 import site
 
 # Below code adapted from https://github.com/skyportal/skyportal/blob/main/skyportal/__init__.py
 # 2022-10-18
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 if "dev" in __version__:
     # Append last commit date and hash to dev version information, if available
 
     import subprocess
     import os.path
```

### Comparing `scope_ml-0.9.4/scope/_instantiate.py` & `scope_ml-0.9.5/scope/_instantiate.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/scope/fritz.py` & `scope_ml-0.9.5/scope/fritz.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/scope/models.py` & `scope_ml-0.9.5/scope/models.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/scope/nn.py` & `scope_ml-0.9.5/scope/nn.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/scope/scope_class.py` & `scope_ml-0.9.5/scope/scope_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,58 +671,32 @@
         )
         parser.add_argument(
             "--plot",
             action="store_true",
             help="if set, generate/save diagnostic training plots",
         )
         parser.add_argument(
+            "--plot-model",
+            action="store_true",
+            help="if set, plot model architecture",
+        )
+        parser.add_argument(
             "--weights-only",
             action="store_true",
             help="if set and pre-trained model specified, load only weights",
         )
         parser.add_argument(
             "--skip-cv",
             action="store_true",
             help="if set, skip XGB cross-validation",
         )
 
         args, _ = parser.parse_known_args()
         self.train(**vars(args))
 
-    # args to add for ds.make (override config-specified values)
-    # threshold
-    # balance
-    # weight_per_class (test this to make sure it works as intended)
-    # scale_features
-    # test_size
-    # val_size
-    # random_state
-    # feature_stats
-    # batch_size
-    # shuffle_buffer_size
-    # epochs
-    # float_convert_types
-
-    # Args to add with descriptions (or references to tf docs)
-    # lr
-    # beta_1
-    # beta_2
-    # epsilon
-    # decay
-    # amsgrad
-    # momentum
-    # monitor
-    # patience
-    # callbacks
-    # run_eagerly
-    # pre_trained_model
-    # save
-    # plot
-    # weights_only
-
     def train(
         self,
         tag: str,
         path_dataset: Union[str, pathlib.Path] = None,
         algorithm: str = "dnn",
         gpu: Optional[int] = None,
         verbose: bool = False,
@@ -752,14 +726,15 @@
         monitor: str = "val_loss",
         patience: int = 20,
         callbacks: list = ["reduce_lr_on_plateau", "early_stopping"],
         run_eagerly: bool = False,
         pre_trained_model: str = None,
         save: bool = False,
         plot: bool = False,
+        plot_model: bool = False,
         weights_only: bool = False,
         skip_cv: bool = False,
         **kwargs,
     ):
         """Train classifier
 
         :param tag: classifier designation, refers to "class" in config.taxonomy (str)
@@ -793,14 +768,15 @@
         :param monitor: dnn monitor quantity (str)
         :param patience: dnn patience [in epochs] (int)
         :param callbacks: dnn callbacks (list)
         :param run_eagerly: dnn run_eagerly (bool)
         :param pre_trained_model: name of dnn pre-trained model to load, if any (str)
         :param save: if set, save trained model (bool)
         :param plot: if set, generate/save diagnostic training plots (bool)
+        :param plot_model: if set, plot model architecture (bool)
         :param weights_only: if set and pre-trained model specified, load only weights (bool)
         :param skip_cv: if set, skip XGB cross-validation (bool)
 
         :return:
         """
 
         import tensorflow as tf
@@ -1117,15 +1093,15 @@
                     beta_1=beta_1,
                     beta_2=beta_2,
                     epsilon=epsilon,
                     decay=decay,
                     amsgrad=amsgrad,
                 )
 
-            if plot:
+            if plot_model:
                 tf.keras.utils.plot_model(
                     classifier.model,
                     to_file=self.base_path / "DNN.pdf",
                     show_shapes=True,
                     show_dtype=False,
                     show_layer_names=False,
                     rankdir="TB",
```

### Comparing `scope_ml-0.9.4/scope/utils.py` & `scope_ml-0.9.5/scope/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     "split_dict",
     "sort_lightcurve",
 ]
 
 from astropy.io import fits
 import datetime
 import json
-import healpy as hp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pathlib
 from sklearn.model_selection import train_test_split
 import tensorflow as tf
 from tqdm.auto import tqdm
@@ -476,14 +475,17 @@
     save: Optional[Union[str, pathlib.Path]] = None,
 ):
     """Plot the RA/DEC Gaia density plot with a sample of objects over-plotted
 
     source: https://vlas.dev/post/gaia-dr2-hrd/
 
     """
+    # import healpy here to avoid windows issues
+    import healpy as hp
+
     # plot the H-R diagram for 1 M stars within 200 pc from the Sun
     plt.rc("text", usetex=True)
 
     # load the data
     hdulist = fits.open(path_gaia_density)
     hist = hdulist[1].data["srcdens"][np.argsort(hdulist[1].data["hpx8"])]
```

### Comparing `scope_ml-0.9.4/scope/xgb.py` & `scope_ml-0.9.5/scope/xgb.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/DNN_AL_mapper.json` & `scope_ml-0.9.5/tools/DNN_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/XGB_AL_mapper.json` & `scope_ml-0.9.5/tools/XGB_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/analyze_logs.py` & `scope_ml-0.9.5/tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/combine_preds.py` & `scope_ml-0.9.5/tools/combine_preds.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,46 +100,49 @@
     fields_xgb_dict = {
         fields_xgb[i]: field_paths_xgb[i] for i in range(len(fields_xgb))
     }
 
     if save:
         os.makedirs(path_to_preds / combined_preds_dirname, exist_ok=True)
 
-    done_fields = [
-        int(str(x).split("/")[-1].split(".")[0].split("_")[1])
-        for x in (path_to_preds / combined_preds_dirname).glob("field_*.parquet")
-    ]
-    fields_to_list = done_fields.copy()
-
-    if fields_to_exclude is not None:
-        fields_to_list.extend(fields_to_exclude)
-
-    fields_to_do = list(
-        set([int(x.split("_")[1]) for x in fields_dnn_dict.keys()]).difference(
-            fields_to_list
+    if dateobs is None:
+        done_fields = [
+            int(str(x).split("/")[-1].split(".")[0].split("_")[1])
+            for x in (path_to_preds / combined_preds_dirname).glob("field_*.parquet")
+        ]
+        fields_to_list = done_fields.copy()
+
+        if fields_to_exclude is not None:
+            fields_to_list.extend(fields_to_exclude)
+
+        fields_to_do = list(
+            set([int(x.split("_")[1]) for x in fields_dnn_dict.keys()]).difference(
+                fields_to_list
+            )
         )
-    )
-    fields_to_list.extend(fields_to_do)
+        fields_to_list.extend(fields_to_do)
 
-    # Use set to drop duplicate fields before sorting
-    fields_to_list = list(set(fields_to_list))
-    fields_to_list.sort()
-
-    if save:
-        # Write json file containing field list
-        with open(path_to_preds / combined_preds_dirname / "fields.json", "w") as f:
-            json.dump(fields_to_list, f)
+        # Use set to drop duplicate fields before sorting
+        fields_to_list = list(set(fields_to_list))
+        fields_to_list.sort()
+
+        if save:
+            # Write json file containing field list
+            with open(path_to_preds / combined_preds_dirname / "fields.json", "w") as f:
+                json.dump(fields_to_list, f)
+
+        # Reformat fields in field_N format to match filenames
+        fields_to_do = [f"field_{x}" for x in fields_to_do]
+    else:
+        fields_to_do = [x for x in fields_dnn_dict.keys()]
 
     preds_to_save = None
     counter = 0
     print(f"Processing {len(fields_to_do)} fields/files...")
 
-    # Reformat fields in field_N format to match filenames
-    fields_to_do = [f"field_{x}" for x in fields_to_do]
-
     for field in fields_dnn_dict.keys():
         if field in fields_to_do:
             if field in fields_xgb_dict.keys():
                 try:
                     dnn_preds = read_parquet(
                         fields_dnn_dict[field] / f"{field}.parquet"
                     )
```

### Comparing `scope_ml-0.9.4/tools/combine_preds_slurm.py` & `scope_ml-0.9.5/tools/combine_preds_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/alertstats.py` & `scope_ml-0.9.5/tools/featureGeneration/alertstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/external_xmatch.py` & `scope_ml-0.9.5/tools/featureGeneration/external_xmatch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/lcstats.py` & `scope_ml-0.9.5/tools/featureGeneration/lcstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/periodsearch.py` & `scope_ml-0.9.5/tools/featureGeneration/periodsearch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/pyaov/aov.f90` & `scope_ml-0.9.5/tools/featureGeneration/pyaov/aov.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/pyaov/aovconst.f90` & `scope_ml-0.9.5/tools/featureGeneration/pyaov/aovconst.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/featureGeneration/pyaov/aovsub.f90` & `scope_ml-0.9.5/tools/featureGeneration/pyaov/aovsub.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/fritz_mapper.json` & `scope_ml-0.9.5/tools/fritz_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/generate_features.py` & `scope_ml-0.9.5/tools/generate_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/generate_features_job_submission.py` & `scope_ml-0.9.5/tools/generate_features_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/generate_features_slurm.py` & `scope_ml-0.9.5/tools/generate_features_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/get_features.py` & `scope_ml-0.9.5/tools/get_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/get_quad_ids.py` & `scope_ml-0.9.5/tools/get_quad_ids.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/golden_dataset_mapper.json` & `scope_ml-0.9.5/tools/golden_dataset_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/inference.py` & `scope_ml-0.9.5/tools/inference.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/run_inference_job_submission.py` & `scope_ml-0.9.5/tools/run_inference_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/run_inference_slurm.py` & `scope_ml-0.9.5/tools/run_inference_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/run_scope_local.py` & `scope_ml-0.9.5/tools/run_scope_local.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/scope_download_classification.py` & `scope_ml-0.9.5/tools/scope_download_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/scope_download_gcn_sources.py` & `scope_ml-0.9.5/tools/scope_download_gcn_sources.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/scope_manage_annotation.py` & `scope_ml-0.9.5/tools/scope_manage_annotation.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/scope_upload_classification.py` & `scope_ml-0.9.5/tools/scope_upload_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/scope_upload_disagreements.py` & `scope_ml-0.9.5/tools/scope_upload_disagreements.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/taxonomy.py` & `scope_ml-0.9.5/tools/taxonomy.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/train_algorithm_job_submission.py` & `scope_ml-0.9.5/tools/train_algorithm_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/tools/train_algorithm_slurm.py` & `scope_ml-0.9.5/tools/train_algorithm_slurm.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.4/PKG-INFO` & `scope_ml-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-ml
-Version: 0.9.4
+Version: 0.9.5
 Summary: SCoPe: ZTF Source Classification Project
 Home-page: https://github.com/ZwickyTransientFacility/scope
 License: MIT
 Author: Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al.
 Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu
 Requires-Python: >=3.9,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scope-ml Version: 0.9.4 Summary: SCoPe: ZTF Source
+Metadata-Version: 2.1 Name: scope-ml Version: 0.9.5 Summary: SCoPe: ZTF Source
 Classification Project Home-page: https://github.com/ZwickyTransientFacility/
 scope License: MIT Author: Brian F. Healy, Michael W. Coughlin, Ashish A.
 Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A.
 Hillenbrand, Jan van Roestel, Paula Szkody et al. Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

