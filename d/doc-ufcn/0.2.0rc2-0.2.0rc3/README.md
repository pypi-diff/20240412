# Comparing `tmp/doc-ufcn-0.2.0rc2.tar.gz` & `tmp/doc-ufcn-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-ufcn-0.2.0rc2.tar", last modified: Fri Mar  1 14:46:10 2024, max compression
+gzip compressed data, was "doc-ufcn-0.2.0rc3.tar", last modified: Fri Apr 12 16:25:21 2024, max compression
```

## Comparing `doc-ufcn-0.2.0rc2.tar` & `doc-ufcn-0.2.0rc3.tar`

### file list

```diff
@@ -1,49 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.984643 doc-ufcn-0.2.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    22162 2024-03-01 14:46:10.984643 doc-ufcn-0.2.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    21431 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-03-01 14:45:59.000000 doc-ufcn-0.2.0rc2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.980643 doc-ufcn-0.2.0rc2/doc_ufcn/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-01 14:45:59.000000 doc-ufcn-0.2.0rc2/doc_ufcn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/image.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/main.py
--rw-rw-rw-   0 root         (0) root         (0)     8821 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/prediction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.984643 doc-ufcn-0.2.0rc2/doc_ufcn/train/
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7109 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/evaluate.py
--rw-rw-rw-   0 root         (0) root         (0)    11206 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     5398 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-03-01 14:18:26.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/mlflow_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/normalization_params.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/predict.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.984643 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/
--rw-rw-rw-   0 root         (0) root         (0)     6880 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9836 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8020 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/object_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     8788 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     4479 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/training.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/training_pixel_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/doc_ufcn/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.980643 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22162 2024-03-01 14:46:10.000000 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1053 2024-03-01 14:46:10.000000 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 14:46:10.000000 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      285 2024-03-01 14:46:10.000000 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-01 14:46:10.000000 doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 14:46:10.984643 doc-ufcn-0.2.0rc2/hugging_face/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-01 14:45:59.000000 doc-ufcn-0.2.0rc2/hugging_face/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7282 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/hugging_face/app.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/hugging_face/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/hugging_face/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 14:46:10.988643 doc-ufcn-0.2.0rc2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1426 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-01 14:12:29.000000 doc-ufcn-0.2.0rc2/training-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22981 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    21500 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.566730 doc-ufcn-0.2.0rc3/ci/
+-rw-rw-rw-   0 root         (0) root         (0)     3037 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/ci/publish_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.566730 doc-ufcn-0.2.0rc3/doc_ufcn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 16:25:11.000000 doc-ufcn-0.2.0rc3/doc_ufcn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     6050 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/prediction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.570730 doc-ufcn-0.2.0rc3/doc_ufcn/train/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     7109 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/evaluate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11206 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5398 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/mlflow_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/normalization_params.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.570730 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     6880 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9836 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8020 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/object_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3891 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     8788 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/training_pixel_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/doc_ufcn/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22981 2024-04-12 16:25:21.000000 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-04-12 16:25:21.000000 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:25:21.000000 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-12 16:25:21.000000 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-12 16:25:21.000000 doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.570730 doc-ufcn-0.2.0rc3/hugging_face/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 16:25:11.000000 doc-ufcn-0.2.0rc3/hugging_face/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7282 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/hugging_face/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/hugging_face/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/hugging_face/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-12 14:41:48.000000 doc-ufcn-0.2.0rc3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 16:25:11.000000 doc-ufcn-0.2.0rc3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    19803 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     5284 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11129 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tests/test_prediction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:25:21.574730 doc-ufcn-0.2.0rc3/tools/
+-rwxrwxrwx   0 root         (0) root         (0)     2735 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tools/notify-slack.py
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2024-04-12 12:20:19.000000 doc-ufcn-0.2.0rc3/tools/training-csv-config.py
```

### Comparing `doc-ufcn-0.2.0rc2/LICENSE` & `doc-ufcn-0.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/PKG-INFO` & `doc-ufcn-0.2.0rc3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-Metadata-Version: 2.1
-Name: doc-ufcn
-Version: 0.2.0rc2
-Summary: Doc-UFCN
-Home-page: https://gitlab.com/teklia/dla/doc-ufcn
-Author: Mélodie Boillet
-Author-email: boillet@teklia.com
-Project-URL: Source, https://gitlab.teklia.com/dla/doc-ufcn/
-Project-URL: Tracker, https://gitlab.teklia.com/dla/doc-ufcn/issues/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: >= 3.10, < 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: training
-License-File: LICENSE
-
 # Doc-UFCN
 
 This Python 3 library contains a public implementation of Doc-UFCN, a fully convolutional network presented in the paper [Multiple Document Datasets Pre-training Improves Text Line Detection With Deep Neural Networks](https://teklia.com/research/publications/boillet2020/). This library has been developed by the original authors from [Teklia](https://teklia.com).
 
 The model is designed to run various Document Layout Analysis (DLA) tasks like the text line detection or page segmentation.
 
-![Model schema](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
+![Model schema](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
 
 This library can be used to train a model, fine-tune a model or directly apply a trained Doc-UFCN model to document images.
 
 ## Getting started
 
 To use Doc-UFCN in your own scripts, install it using pip:
 
@@ -100,16 +81,16 @@
 By default, only the detected polygons are returned, to return the four outputs, one can use:
 ```python
 detected_polygons, probabilities, mask, overlap = model.predict(
     image, raw_output=True, mask_output=True, overlap_output=True
 )
 ```
 
-![Mask of detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/mask.png)
-![Overlap with the detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/overlap.png)
+![Mask of detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/mask.png)
+![Overlap with the detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/overlap.png)
 
 ### Models
 
 We provide various open-source models, stored on [HuggingFace](https://huggingface.co/Teklia) and every model prefixed by `doc-ufcn-` is supported. For example, to download our [generic page detection model](https://huggingface.co/Teklia/doc-ufcn-generic-page) and load it, one can use:
 ```python
 from doc_ufcn import models
 from doc_ufcn.main import DocUFCN
@@ -320,15 +301,15 @@
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
+![image](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
 
 An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
 | `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
 | `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
@@ -398,8 +379,8 @@
 
 ## License
 
 This library is under the 3-Clause BSD License.
 
 ## Contact
 
-If you have any questions or suggestions, please contact [Mélodie Boillet](mailto:boillet@teklia.com).
+If you have any questions or suggestions, please contact [Mélodie Boillet and Teklia](mailto:team@teklia.com?cc=boillet@teklia.com&subject=Feedback%20on%20Doc-UFCN%3A%20).
```

### Comparing `doc-ufcn-0.2.0rc2/README.md` & `doc-ufcn-0.2.0rc3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,49 @@
+Metadata-Version: 2.1
+Name: doc-ufcn
+Version: 0.2.0rc3
+Summary: Doc-UFCN
+Author-email: Mélodie Boillet <boillet@teklia.com>
+Project-URL: Source, https://gitlab.teklia.com/dla/doc-ufcn/
+Project-URL: Tracker, https://gitlab.teklia.com/dla/doc-ufcn/issues/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: <3.11,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: huggingface-hub==0.20.2
+Requires-Dist: numpy==1.26.2
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: requests<3,>=2
+Requires-Dist: torch==2.1.0
+Provides-Extra: training
+Requires-Dist: imageio==2.27.0; extra == "training"
+Requires-Dist: matplotlib==3.8.1; extra == "training"
+Requires-Dist: mlflow==2.2.1; extra == "training"
+Requires-Dist: Shapely==2.0.3; extra == "training"
+Requires-Dist: teklia-toolbox==0.1.4; extra == "training"
+Requires-Dist: tensorboard==2.15.1; extra == "training"
+Requires-Dist: torchvision==0.16.0; extra == "training"
+Requires-Dist: tqdm==4.66.1; extra == "training"
+Provides-Extra: test
+Requires-Dist: scikit-image==0.22.0; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-lazy-fixtures==1.0.7; extra == "test"
+
 # Doc-UFCN
 
 This Python 3 library contains a public implementation of Doc-UFCN, a fully convolutional network presented in the paper [Multiple Document Datasets Pre-training Improves Text Line Detection With Deep Neural Networks](https://teklia.com/research/publications/boillet2020/). This library has been developed by the original authors from [Teklia](https://teklia.com).
 
 The model is designed to run various Document Layout Analysis (DLA) tasks like the text line detection or page segmentation.
 
-![Model schema](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
+![Model schema](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
 
 This library can be used to train a model, fine-tune a model or directly apply a trained Doc-UFCN model to document images.
 
 ## Getting started
 
 To use Doc-UFCN in your own scripts, install it using pip:
 
@@ -81,16 +116,16 @@
 By default, only the detected polygons are returned, to return the four outputs, one can use:
 ```python
 detected_polygons, probabilities, mask, overlap = model.predict(
     image, raw_output=True, mask_output=True, overlap_output=True
 )
 ```
 
-![Mask of detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/mask.png)
-![Overlap with the detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/overlap.png)
+![Mask of detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/mask.png)
+![Overlap with the detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/overlap.png)
 
 ### Models
 
 We provide various open-source models, stored on [HuggingFace](https://huggingface.co/Teklia) and every model prefixed by `doc-ufcn-` is supported. For example, to download our [generic page detection model](https://huggingface.co/Teklia/doc-ufcn-generic-page) and load it, one can use:
 ```python
 from doc_ufcn import models
 from doc_ufcn.main import DocUFCN
@@ -301,15 +336,15 @@
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
+![image](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
 
 An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
 | `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
 | `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
@@ -379,8 +414,8 @@
 
 ## License
 
 This library is under the 3-Clause BSD License.
 
 ## Contact
 
-If you have any questions or suggestions, please contact [Mélodie Boillet](mailto:boillet@teklia.com).
+If you have any questions or suggestions, please contact [Mélodie Boillet and Teklia](mailto:team@teklia.com?cc=boillet@teklia.com&subject=Feedback%20on%20Doc-UFCN%3A%20).
```

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/image.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/image.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/main.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/main.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/model.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/model.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/models.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/models.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/prediction.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/cli.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/cli.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/configuration.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/configuration.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/evaluate.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/evaluate.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/experiment.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/experiment.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/mask.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/mask.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/mlflow_utils.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/normalization_params.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/normalization_params.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/predict.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/predict.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/training.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/__init__.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/evaluation.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/object_metrics.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/object_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/pixel_metrics.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/prediction.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/preprocessing.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/training.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/training.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/train/utils/training_pixel_metrics.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/train/utils/training_pixel_metrics.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn/utils.py` & `doc-ufcn-0.2.0rc3/doc_ufcn/utils.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/PKG-INFO` & `doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: doc-ufcn
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Doc-UFCN
-Home-page: https://gitlab.com/teklia/dla/doc-ufcn
-Author: Mélodie Boillet
-Author-email: boillet@teklia.com
+Author-email: Mélodie Boillet <boillet@teklia.com>
 Project-URL: Source, https://gitlab.teklia.com/dla/doc-ufcn/
 Project-URL: Tracker, https://gitlab.teklia.com/dla/doc-ufcn/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Requires-Python: >= 3.10, < 3.11
+Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: training
 License-File: LICENSE
+Requires-Dist: huggingface-hub==0.20.2
+Requires-Dist: numpy==1.26.2
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: requests<3,>=2
+Requires-Dist: torch==2.1.0
+Provides-Extra: training
+Requires-Dist: imageio==2.27.0; extra == "training"
+Requires-Dist: matplotlib==3.8.1; extra == "training"
+Requires-Dist: mlflow==2.2.1; extra == "training"
+Requires-Dist: Shapely==2.0.3; extra == "training"
+Requires-Dist: teklia-toolbox==0.1.4; extra == "training"
+Requires-Dist: tensorboard==2.15.1; extra == "training"
+Requires-Dist: torchvision==0.16.0; extra == "training"
+Requires-Dist: tqdm==4.66.1; extra == "training"
+Provides-Extra: test
+Requires-Dist: scikit-image==0.22.0; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-lazy-fixtures==1.0.7; extra == "test"
 
 # Doc-UFCN
 
 This Python 3 library contains a public implementation of Doc-UFCN, a fully convolutional network presented in the paper [Multiple Document Datasets Pre-training Improves Text Line Detection With Deep Neural Networks](https://teklia.com/research/publications/boillet2020/). This library has been developed by the original authors from [Teklia](https://teklia.com).
 
 The model is designed to run various Document Layout Analysis (DLA) tasks like the text line detection or page segmentation.
 
-![Model schema](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
+![Model schema](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/UFCN.png)
 
 This library can be used to train a model, fine-tune a model or directly apply a trained Doc-UFCN model to document images.
 
 ## Getting started
 
 To use Doc-UFCN in your own scripts, install it using pip:
 
@@ -100,16 +116,16 @@
 By default, only the detected polygons are returned, to return the four outputs, one can use:
 ```python
 detected_polygons, probabilities, mask, overlap = model.predict(
     image, raw_output=True, mask_output=True, overlap_output=True
 )
 ```
 
-![Mask of detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/mask.png)
-![Overlap with the detected objects](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/resources/overlap.png)
+![Mask of detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/mask.png)
+![Overlap with the detected objects](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/resources/overlap.png)
 
 ### Models
 
 We provide various open-source models, stored on [HuggingFace](https://huggingface.co/Teklia) and every model prefixed by `doc-ufcn-` is supported. For example, to download our [generic page detection model](https://huggingface.co/Teklia/doc-ufcn-generic-page) and load it, one can use:
 ```python
 from doc_ufcn import models
 from doc_ufcn.main import DocUFCN
@@ -320,15 +336,15 @@
 
 ```shell
 pip install gradio
 ```
 The code was last tested with `gradio==3.18.0`.
 
 
-![image](https://gitlab.com/teklia/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
+![image](https://gitlab.teklia.com/dla/doc-ufcn/-/raw/main/hugging_face/resource/demo_doc_ufcn_hf.png)
 
 An example is available in the `huggingface/` folder. You need to create a YAML configuration file with the following parameters:
 
 | Parameter        | Description                                                                                                        | Default value                 |
 | ---------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
 | `title`          | Title of the app (supports Markdown)                                                                                                   |                           **Required**|
 | `description`    | Description of the app (supports Markdown)                                                                                           |                           **Required**|
@@ -398,8 +414,8 @@
 
 ## License
 
 This library is under the 3-Clause BSD License.
 
 ## Contact
 
-If you have any questions or suggestions, please contact [Mélodie Boillet](mailto:boillet@teklia.com).
+If you have any questions or suggestions, please contact [Mélodie Boillet and Teklia](mailto:team@teklia.com?cc=boillet@teklia.com&subject=Feedback%20on%20Doc-UFCN%3A%20).
```

### Comparing `doc-ufcn-0.2.0rc2/doc_ufcn.egg-info/SOURCES.txt` & `doc-ufcn-0.2.0rc3/doc_ufcn.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 LICENSE
-MANIFEST.in
 README.md
-VERSION
-requirements.txt
-setup.py
-training-requirements.txt
+pyproject.toml
+ci/publish_models.py
 doc_ufcn/__init__.py
 doc_ufcn/image.py
 doc_ufcn/main.py
 doc_ufcn/model.py
 doc_ufcn/models.py
 doc_ufcn/prediction.py
 doc_ufcn/utils.py
@@ -34,8 +31,18 @@
 doc_ufcn/train/utils/prediction.py
 doc_ufcn/train/utils/preprocessing.py
 doc_ufcn/train/utils/training.py
 doc_ufcn/train/utils/training_pixel_metrics.py
 hugging_face/__init__.py
 hugging_face/app.py
 hugging_face/config.py
-hugging_face/tools.py
+hugging_face/tools.py
+tests/__init__.py
+tests/conftest.py
+tests/test_image.py
+tests/test_main.py
+tests/test_mask.py
+tests/test_model.py
+tests/test_models.py
+tests/test_prediction.py
+tools/notify-slack.py
+tools/training-csv-config.py
```

### Comparing `doc-ufcn-0.2.0rc2/hugging_face/app.py` & `doc-ufcn-0.2.0rc3/hugging_face/app.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/hugging_face/config.py` & `doc-ufcn-0.2.0rc3/hugging_face/config.py`

 * *Files identical despite different names*

### Comparing `doc-ufcn-0.2.0rc2/hugging_face/tools.py` & `doc-ufcn-0.2.0rc3/hugging_face/tools.py`

 * *Files identical despite different names*

