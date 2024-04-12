# Comparing `tmp/efficient_ocr-0.0.5.tar.gz` & `tmp/efficient_ocr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficient_ocr-0.0.5.tar", last modified: Tue Sep 12 14:36:21 2023, max compression
+gzip compressed data, was "efficient_ocr-0.1.0.tar", last modified: Mon Nov 20 15:51:00 2023, max compression
```

## Comparing `efficient_ocr-0.0.5.tar` & `efficient_ocr-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.804548 efficient_ocr-0.0.5/
--rw-rw-rw-   0        0        0    11558 2023-08-02 23:33:03.000000 efficient_ocr-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1462 2023-09-12 14:36:21.803551 efficient_ocr-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-08-02 23:33:03.000000 efficient_ocr-0.0.5/README.md
--rw-rw-rw-   0        0        0      788 2023-09-12 14:36:21.828556 efficient_ocr-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2067 2023-09-12 14:34:51.000000 efficient_ocr-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.489521 efficient_ocr-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.537520 efficient_ocr-0.0.5/src/efficient_ocr/
--rw-rw-rw-   0        0        0      118 2023-08-06 15:11:35.000000 efficient_ocr-0.0.5/src/efficient_ocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.640516 efficient_ocr-0.0.5/src/efficient_ocr/detection/
--rw-rw-rw-   0        0        0       76 2023-08-03 15:17:36.000000 efficient_ocr-0.0.5/src/efficient_ocr/detection/__init__.py
--rw-rw-rw-   0        0        0     2512 2023-08-14 20:58:59.000000 efficient_ocr-0.0.5/src/efficient_ocr/detection/detector.py
--rw-rw-rw-   0        0        0    13988 2023-09-07 22:21:06.000000 efficient_ocr-0.0.5/src/efficient_ocr/detection/linemodel.py
--rw-rw-rw-   0        0        0    20392 2023-09-08 19:15:35.000000 efficient_ocr-0.0.5/src/efficient_ocr/detection/localizermodel.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.668552 efficient_ocr-0.0.5/src/efficient_ocr/model/
--rw-rw-rw-   0        0        0       20 2023-08-15 15:18:04.000000 efficient_ocr-0.0.5/src/efficient_ocr/model/__init__.py
--rw-rw-rw-   0        0        0    20483 2023-09-08 19:20:05.000000 efficient_ocr-0.0.5/src/efficient_ocr/model/effocr.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.721547 efficient_ocr-0.0.5/src/efficient_ocr/recognition/
--rw-rw-rw-   0        0        0      112 2023-09-05 12:38:42.000000 efficient_ocr-0.0.5/src/efficient_ocr/recognition/__init__.py
--rw-rw-rw-   0        0        0     6490 2023-09-08 15:01:34.000000 efficient_ocr-0.0.5/src/efficient_ocr/recognition/infer_recognize.py
--rw-rw-rw-   0        0        0    43352 2023-09-05 20:42:03.000000 efficient_ocr-0.0.5/src/efficient_ocr/recognition/recognizermodel.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.762553 efficient_ocr-0.0.5/src/efficient_ocr/utils/
--rw-rw-rw-   0        0        0      765 2023-08-25 19:33:07.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/__init__.py
--rw-rw-rw-   0        0        0     5059 2023-09-12 14:30:10.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/default_config.py
--rw-rw-rw-   0        0        0     1338 2023-08-25 19:33:07.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/misc.py
--rw-rw-rw-   0        0        0      817 2023-09-05 20:38:20.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/onnx.py
--rw-rw-rw-   0        0        0    22849 2023-08-07 05:09:23.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/ops.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.797552 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/
--rw-rw-rw-   0        0        0      156 2023-08-14 21:16:32.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/__init__.py
--rw-rw-rw-   0        0        0     9992 2023-08-06 15:11:35.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/custom_schedulers.py
--rw-rw-rw-   0        0        0    13091 2023-08-10 18:41:52.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/datasets.py
--rw-rw-rw-   0        0        0     1441 2023-08-06 15:11:35.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/encoders.py
--rw-rw-rw-   0        0        0    15181 2023-08-10 18:41:52.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/samplers.py
--rw-rw-rw-   0        0        0    12816 2023-08-10 18:41:52.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/synth_crops.py
--rw-rw-rw-   0        0        0    12141 2023-08-07 00:31:49.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/transforms.py
--rw-rw-rw-   0        0        0     3777 2023-08-03 19:07:45.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/text.py
--rw-rw-rw-   0        0        0     3113 2023-09-05 20:04:53.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/transforms.py
--rw-rw-rw-   0        0        0     3463 2023-09-05 12:38:42.000000 efficient_ocr-0.0.5/src/efficient_ocr/utils/yolo.py
-drwxrwxrwx   0        0        0        0 2023-09-12 14:36:21.606520 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/
--rw-rw-rw-   0        0        0     1462 2023-09-12 14:36:21.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-09-12 14:36:21.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-12 14:36:21.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-14 20:11:06.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      208 2023-09-12 14:36:21.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-09-12 14:36:21.000000 efficient_ocr-0.0.5/src/efficient_ocr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.357023 efficient_ocr-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-08-02 23:33:03.000000 efficient_ocr-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    12322 2023-11-20 15:51:00.355021 efficient_ocr-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10875 2023-11-10 18:43:04.000000 efficient_ocr-0.1.0/README.md
+-rw-rw-rw-   0        0        0      788 2023-11-20 15:51:00.361021 efficient_ocr-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2061 2023-11-20 15:49:47.000000 efficient_ocr-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.179021 efficient_ocr-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.213020 efficient_ocr-0.1.0/src/efficient_ocr/
+-rw-rw-rw-   0        0        0      118 2023-08-06 15:11:35.000000 efficient_ocr-0.1.0/src/efficient_ocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.281020 efficient_ocr-0.1.0/src/efficient_ocr/detection/
+-rw-rw-rw-   0        0        0       76 2023-08-03 15:17:36.000000 efficient_ocr-0.1.0/src/efficient_ocr/detection/__init__.py
+-rw-rw-rw-   0        0        0     2512 2023-08-14 20:58:59.000000 efficient_ocr-0.1.0/src/efficient_ocr/detection/detector.py
+-rw-rw-rw-   0        0        0    16781 2023-11-10 19:08:10.000000 efficient_ocr-0.1.0/src/efficient_ocr/detection/linemodel.py
+-rw-rw-rw-   0        0        0    22810 2023-09-19 21:43:28.000000 efficient_ocr-0.1.0/src/efficient_ocr/detection/localizermodel.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.287019 efficient_ocr-0.1.0/src/efficient_ocr/model/
+-rw-rw-rw-   0        0        0       20 2023-08-15 15:18:04.000000 efficient_ocr-0.1.0/src/efficient_ocr/model/__init__.py
+-rw-rw-rw-   0        0        0    21401 2023-11-10 22:02:44.000000 efficient_ocr-0.1.0/src/efficient_ocr/model/effocr.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.298020 efficient_ocr-0.1.0/src/efficient_ocr/recognition/
+-rw-rw-rw-   0        0        0      112 2023-09-05 12:38:42.000000 efficient_ocr-0.1.0/src/efficient_ocr/recognition/__init__.py
+-rw-rw-rw-   0        0        0     6490 2023-11-10 18:45:37.000000 efficient_ocr-0.1.0/src/efficient_ocr/recognition/infer_recognize.py
+-rw-rw-rw-   0        0        0    45805 2023-11-20 15:48:41.000000 efficient_ocr-0.1.0/src/efficient_ocr/recognition/recognizermodel.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.325022 efficient_ocr-0.1.0/src/efficient_ocr/utils/
+-rw-rw-rw-   0        0        0      765 2023-08-25 19:33:07.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/__init__.py
+-rw-rw-rw-   0        0        0     5237 2023-11-10 21:29:30.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/default_config.py
+-rw-rw-rw-   0        0        0     1338 2023-08-25 19:33:07.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/misc.py
+-rw-rw-rw-   0        0        0      817 2023-09-05 20:38:20.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/onnx.py
+-rw-rw-rw-   0        0        0    23346 2023-09-13 13:22:50.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/ops.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.350020 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/
+-rw-rw-rw-   0        0        0      156 2023-08-14 21:16:32.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/__init__.py
+-rw-rw-rw-   0        0        0     9992 2023-08-06 15:11:35.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/custom_schedulers.py
+-rw-rw-rw-   0        0        0    13091 2023-08-10 18:41:52.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/datasets.py
+-rw-rw-rw-   0        0        0     1441 2023-08-06 15:11:35.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/encoders.py
+-rw-rw-rw-   0        0        0    15181 2023-08-10 18:41:52.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/samplers.py
+-rw-rw-rw-   0        0        0    12816 2023-08-10 18:41:52.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/synth_crops.py
+-rw-rw-rw-   0        0        0    12319 2023-11-20 15:48:41.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/transforms.py
+-rw-rw-rw-   0        0        0     3777 2023-08-03 19:07:45.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/text.py
+-rw-rw-rw-   0        0        0     3145 2023-11-20 15:48:41.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/transforms.py
+-rw-rw-rw-   0        0        0     3463 2023-09-05 12:38:42.000000 efficient_ocr-0.1.0/src/efficient_ocr/utils/yolo.py
+drwxrwxrwx   0        0        0        0 2023-11-20 15:51:00.267020 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/
+-rw-rw-rw-   0        0        0    12322 2023-11-20 15:51:00.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-11-20 15:51:00.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-20 15:51:00.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-14 20:11:06.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      208 2023-11-20 15:51:00.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-11-20 15:51:00.000000 efficient_ocr-0.1.0/src/efficient_ocr.egg-info/top_level.txt
```

### Comparing `efficient_ocr-0.0.5/LICENSE` & `efficient_ocr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/setup.cfg` & `efficient_ocr-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/setup.py` & `efficient_ocr-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 pkg_name = 'efficient_ocr'
 libinfo_py = os.path.join('src', pkg_name, '__init__.py')
 libinfo_content = open(libinfo_py, 'r', encoding='utf8').readlines()
 # version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][0]
 # exec(version_line)  # gives __version__
 
 setup(name         = "efficient_ocr",
-      version      = "0.0.5",
+      version      = "0.1.0",
       author       = "Tom Bryan, Abhishek Arora, Jacob Carlson",
       author_email = "bryanptom@gmail.com",
       license      = "Apache-2.0",
       url          = "https://github.com/dell-research-harvard/efficient_ocr",
       package_dir  = {"": "src"},
       packages     = find_packages("src"),
       description  = "Efficient OCR",
@@ -53,8 +53,8 @@
         'kornia',
         'pytorch_metric_learning',
         'transformers',
         'albumentations',
         'wandb'
       ],
       include_package_data=True
-      )
+)
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/detection/detector.py` & `efficient_ocr-0.1.0/src/efficient_ocr/detection/detector.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/detection/linemodel.py` & `efficient_ocr-0.1.0/src/efficient_ocr/detection/linemodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # import mmcv
 import torch
 import numpy as np
 import torchvision
 import cv2
 from math import floor, ceil
 import yolov5
-from huggingface_hub import snapshot_download
+from huggingface_hub import hf_hub_download
 from collections import defaultdict
 import subprocess
 
 from ..utils import letterbox, yolov8_non_max_suppression, initialize_onnx_model
 from ..utils import DEFAULT_MEAN, DEFAULT_STD
 from ..utils import create_yolo_training_data
 from ..utils import get_path, dictmerge, dir_is_empty
@@ -20,18 +20,40 @@
 
 
     def __init__(self, config):
 
         self.config = config
 
         if self.config['Line']['hf_repo_id'] is not None:
-            snapshot_download(
-                repo_id=self.config['Line']['hf_repo_id'], 
-                local_dir=self.config['Line']['model_dir'],
-                local_dir_use_symlinks=False)
+            
+            os.makedirs(self.config['Line']['model_dir'], exist_ok=True)
+            
+            # Parse out provided repo_id
+            repo_id = self.config['Line']['hf_repo_id'].strip('/')
+            # split on slashes
+            
+            if len(repo_id.split('/')) == 2:
+                fn_prefix = ''
+                fn = 'line.pt' if self.config['Line']['model_backend'] == 'yolov5' else 'line.onnx'
+
+            elif len(repo_id.split('/')) < 2:
+                raise ValueError('hf_repo_id must be in the format owner/repo_name, for example: dell-research-harvard/effocr_en')
+            else:
+                if repo_id.endswith('pt') or repo_id.endswith('onnx'):
+                    fn = '/'.join(repo_id.split('/')[2:])
+                    fn_prefix = ''
+                else:
+                    fn_prefix = '/'.join(repo_id.split('/')[2:]) + '/' # Careful, order matters here
+                    fn = 'line.pt' if self.config['Line']['model_backend'] == 'yolov5' else 'line.onnx'
+                repo_id = '/'.join(repo_id.split('/')[:2])
+
+            if not os.path.exists(os.path.join(self.config['Line']['model_dir'], fn_prefix + fn)):
+                hf_hub_download(repo_id = self.config['Line']['hf_repo_id'], 
+                                filename = fn_prefix + fn, 
+                                local_dir = self.config['Line']['model_dir']) 
             
         self.initialize_model()
 
 
     def __call__(self, imgs):
         """Wraps the run method, allowing the object to be called directly
 
@@ -265,46 +287,69 @@
         
         if kwargs:
             config = dictmerge(config, kwargs)
 
         os.makedirs(self.config['Line']['model_dir'], exist_ok=True)
             
         # Create yolo training data from coco
-        yaml_loc = create_yolo_training_data(
-            data_json, data_dir, target='line', 
-            output_dir=self.config["Line"]["model_dir"], 
-            char_only=self.config["Global"]["char_only"])
+        if self.config['Line']['training']['training_data_dir'] is None:
+            yaml_loc = create_yolo_training_data(
+                data_json, data_dir, target='line_detection', 
+                output_dir=self.config["Line"]["model_dir"], 
+                char_only=self.config["Global"]["char_only"])
+        elif os.path.isfile(os.path.join(self.config['Line']['training']['training_data_dir'], 'data.yaml')):
+            yaml_loc = os.path.join(self.config['Line']['training']['training_data_dir'], 'data.yaml')
+        else:
+            raise ValueError('Could not find training data yaml file! Please specify a valid training_data_dir in the config file (containing a data.yaml file) or a valid data_json.')
         
         train_weights = get_path(self.config['Line']['model_dir'], ext="pt")
 
         if self.config['Global']['hf_token_for_upload'] is None:
-            subprocess.run([
+            print(' '.join([
+                "yolov5", "train",
+                "--imgsz", str(self.config['Line']['training']['input_shape'][0]),
+                "--data", yaml_loc,
+                "--weights", train_weights if train_weights is not None else 'yolov5s.pt',
+                "--epochs", str(self.config['Line']['training']['epochs']),
+                "--batch_size", str(self.config['Line']['training']['batch_size']),
+                "--device", self.config['Line']['training']['device'],
+                "--project", self.config['Line']['model_dir'],
+                "--name", "trained_line_det"]))
+            p = subprocess.Popen(' '.join([
                 "yolov5", "train",
                 "--imgsz", str(self.config['Line']['training']['input_shape'][0]),
                 "--data", yaml_loc,
                 "--weights", train_weights if train_weights is not None else 'yolov5s.pt',
                 "--epochs", str(self.config['Line']['training']['epochs']),
                 "--batch_size", str(self.config['Line']['training']['batch_size']),
-                "--device", self.config['Line']['device'],
+                "--device", self.config['Line']['training']['device'],
                 "--project", self.config['Line']['model_dir'],
-                "--name", "trained"])
+                "--name", "trained_line_det"]), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1, shell=True)
         else:
             assert self.config['Global']['hf_username_for_upload'] is not None
-            subprocess.run(" ".join([
+            p = subprocess.Popen(" ".join([
                 "huggingface-cli", "login", "--token", self.config['Global']['hf_token_for_upload'], 
                 "&&",
                 "yolov5", "train",
                 "--imgsz", str(self.config['Line']['training']['input_shape'][0]),
                 "--data", yaml_loc,
                 "--weights", train_weights if train_weights is not None else 'yolov5s.pt',
                 "--epochs", str(self.config['Line']['training']['epochs']),
                 "--batch_size", str(self.config['Line']['training']['batch_size']),
-                "--device", self.config['Line']['device'],
+                "--device", self.config['Line']['training']['device'],
                 "--project", self.config['Line']['model_dir'],
-                "--name", "trained",
+                "--name", "trained_line_det",
                 "--hf_model_id", os.path.join(self.config['Global']['hf_username_for_upload'], 
                                               os.path.basename(self.config['Line']['model_dir'])),
                 "--hf_token", self.config['Global']['hf_token_for_upload'],
-                "--hf_private"]), shell=True)
-                        
+                "--hf_private"]), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1, shell=True)
+
+        # Stream the output to the console as we train
+        for line in iter(p.stdout.readline, ''):
+            if len(line) > 0:
+                print(line.decode('utf-8').strip('\n'))
+            elif not line:
+                break
+        p.wait()
+
         self.initialize_model()
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/detection/localizermodel.py` & `efficient_ocr-0.1.0/src/efficient_ocr/detection/localizermodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import yolov5
 import numpy as np
 from collections import defaultdict
 import threading
 import torch
 import queue
-from huggingface_hub import snapshot_download
+from huggingface_hub import hf_hub_download
 import multiprocessing
 import subprocess
 from math import floor, ceil
 import torchvision.ops.boxes as bops
 # from mmdet.apis import init_detector, inference_detector
 
 
@@ -115,19 +115,41 @@
 
 
     def __init__(self, config):
 
         self.config = config
 
         if self.config['Localizer']['hf_repo_id'] is not None:
-            snapshot_download(
-                repo_id=self.config['Localizer']['hf_repo_id'], 
-                local_dir=self.config['Localizer']['model_dir'],
-                local_dir_use_symlinks=False)
             
+            os.makedirs(self.config['Localizer']['model_dir'], exist_ok=True)
+            
+            # Parse out provided repo_id
+            repo_id = self.config['Localizer']['hf_repo_id'].strip('/')
+            # split on slashes
+            
+            if len(repo_id.split('/')) == 2:
+                fn_prefix = ''
+                fn = 'localizer.pt' if self.config['Localizer']['model_backend'] == 'yolov5' else 'localizer.onnx'
+
+            elif len(repo_id.split('/')) < 2:
+                raise ValueError('hf_repo_id must be in the format owner/repo_name, for example: dell-research-harvard/effocr_en')
+            else:
+                if repo_id.endswith('pt') or repo_id.endswith('onnx'):
+                    fn = '/'.join(repo_id.split('/')[2:])
+                    fn_prefix = ''
+                else:
+                    fn_prefix = '/'.join(repo_id.split('/')[2:]) + '/' # Careful, order matters here
+                    fn = 'localizer.pt' if self.config['Localizer']['model_backend'] == 'yolov5' else 'localizer.onnx'
+                repo_id = '/'.join(repo_id.split('/')[:2])
+
+            if not os.path.exists(os.path.join(self.config['Localizer']['model_dir'], fn_prefix + fn)):
+                hf_hub_download(repo_id = self.config['Localizer']['hf_repo_id'], 
+                                filename = fn_prefix + fn, 
+                                local_dir = self.config['Localizer']['model_dir'])          
+        
         self.initialize_model()
 
 
     def initialize_model(self):
         """Initializes the model based on the model backend
 
         Returns:
@@ -282,15 +304,15 @@
             thread.start()
         
         for thread in threads:
             thread.join()
 
         # Get the results from the output queue
         side_dists  = {bbox_idx: {'l_dists': [None] * len(line_results[bbox_idx]), 'r_dists': [None] * len(line_results[bbox_idx])} for bbox_idx in line_results.keys()}
-        print('Got localizer results')
+
         while not output_queue.empty():
             bbox_idx, im_idx, preds = output_queue.get()
             
             im = line_results[bbox_idx][im_idx][0]
             if self.config['Localizer']['model_backend'] == 'onnx':  
                 preds = [torch.from_numpy(pred) for pred in preds]
                 preds = [yolov8_non_max_suppression(
@@ -415,46 +437,61 @@
         
         if kwargs:
             config = dictmerge(config, kwargs)
 
         os.makedirs(self.config['Localizer']['model_dir'], exist_ok=True)
 
         # Create yolo training data from coco
-        yaml_loc = create_yolo_training_data(
-            data_json, data_dir, target='localizer', 
-            output_dir=self.config["Localizer"]["model_dir"], 
-            char_only=self.config["Global"]["char_only"])
+        if self.config['Localizer']['training']['training_data_dir'] is None:
+            yaml_loc = create_yolo_training_data(
+                data_json, data_dir, target='localizer', 
+                output_dir=self.config["Localizer"]["model_dir"], 
+                char_only=self.config["Global"]["char_only"])
+        elif os.path.isfile(os.path.join(self.config['Localizer']['training']['training_data_dir'], 'data.yaml')):
+            yaml_loc = os.path.join(self.config['Localizer']['training']['training_data_dir'], 'data.yaml')
+        else:
+            raise ValueError('Could not find training data yaml file! Please specify a valid training_data_dir in the config file (containing a data.yaml file) or a valid data_json.')
         
         train_weights = get_path(self.config['Localizer']['model_dir'], ext="pt")
 
+        # Switching these all to subprocess.Popen calls to allow for streaming of outputs to the console in notebooks (esp colab)
         if self.config['Global']['hf_token_for_upload'] is None:
-            subprocess.run([
+            p = subprocess.Popen(' '.join([
                 "yolov5", "train",
                 "--imgsz", str(self.config['Localizer']['training']['input_shape'][0]),
                 "--data", yaml_loc,
                 "--weights", train_weights if train_weights is not None else 'yolov5s.pt',
                 "--epochs", str(self.config['Localizer']['training']['epochs']),
                 "--batch_size", str(self.config['Localizer']['training']['batch_size']),
-                "--device", self.config['Localizer']['device'],
+                "--device", self.config['Localizer']['training']['device'],
                 "--project", self.config['Localizer']['model_dir'],
-                "--name", "trained"])
+                "--name", "trained_localizer"]), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1, shell=True)
+            
         else:
-            assert self.config['Global']['hf_username_for_upload'] is not None
-            subprocess.run(" ".join([
+            assert self.config['Global']['hf_username_for_upload'] is not None, 'Must specify hf_username_for_upload in config file!'
+            subprocess.Popen(" ".join([
                 "huggingface-cli", "login", "--token", self.config['Global']['hf_token_for_upload'], 
                 "&&",
                 "yolov5", "train",
                 "--imgsz", str(self.config['Localizer']['training']['input_shape'][0]),
                 "--data", yaml_loc,
                 "--weights", train_weights if train_weights is not None else 'yolov5s.pt',
                 "--epochs", str(self.config['Localizer']['training']['epochs']),
                 "--batch_size", str(self.config['Localizer']['training']['batch_size']),
-                "--device", self.config['Localizer']['device'],
+                "--device", self.config['Localizer']['training']['device'],
                 "--project", self.config['Localizer']['model_dir'],
-                "--name", "trained",
+                "--name", "trained_localizer",
                 "--hf_model_id", os.path.join(self.config['Global']['hf_username_for_upload'], 
                                               os.path.basename(self.config['Localizer']['model_dir'])),
                 "--hf_token", self.config['Global']['hf_token_for_upload'],
-                "--hf_private"]), shell=True)
+                "--hf_private"]), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=1, shell=True)
+            
+        # Stream the output to the console as we train
+        for line in iter(p.stdout.readline, ''):
+            if len(line) > 0:
+                print(line.decode('utf-8').strip('\n'))
+            elif not line:
+                break
+        p.wait()
                         
         self.initialize_model()
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/model/effocr.py` & `efficient_ocr-0.1.0/src/efficient_ocr/model/effocr.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,16 +97,29 @@
             self.config['Localizer']['model_dir'] = f"./{os.path.basename(self.config['Localizer']['hf_repo_id'])}"
         if self.config['Recognizer']['char']['hf_repo_id'] is not None and self.config['Recognizer']['char']['model_dir'] == "./char_model":
             self.config['Recognizer']['char']['model_dir'] = f"./{os.path.basename(self.config['Recognizer']['char']['hf_repo_id'])}"
         if self.config['Recognizer']['word']['hf_repo_id'] is not None and self.config['Recognizer']['word']['model_dir'] == "./word_model":
             self.config['Recognizer']['word']['model_dir'] = f"./{os.path.basename(self.config['Recognizer']['word']['hf_repo_id'])}"
         
         ## subset init
+        if self.config['Global']['single_model_training'] is not None:
+            to_train = self.config['Global']['single_model_training']
+            if to_train == 'line_detector':
+                self.line_model = self._initialize_line()
+            elif to_train == 'localizer':
+                self.localizer_model = self._initialize_localizer()
+            elif to_train == 'word_recognizer':
+                self.word_model = self._initialize_word_recognizer()
+            elif to_train == 'char_recognizer':
+                self.char_model = self._initialize_char_recognizer()
+            else:
+                raise ValueError('single_model_training must be one of: line_detector, localizer, word_recognizer, char_recognizer')
 
-        if self.config['Global']['char_only'] and self.config['Global']['recognition_only']:
+        ## full init
+        elif self.config['Global']['char_only'] and self.config['Global']['recognition_only']:
             self.char_model = self._initialize_char_recognizer()
         elif self.config['Global']['recognition_only']:
             self.word_model = self._initialize_word_recognizer()
             self.char_model = self._initialize_char_recognizer()
         elif self.config['Global']['char_only']:
             self.char_model = self._initialize_char_recognizer()
             if not self.config['Global']['skip_line_detection']:
@@ -154,28 +167,27 @@
                 full_text = '\n'.join([results[bbox_idx][i]['char_preds'] for i in range(len(results[bbox_idx]))])
             full_results[bbox_idx] = EffOCRResult(full_text, results[bbox_idx])
 
         return full_results
 
 
     def train(self, target = None, **kwargs):
-        
         if isinstance(target, str):
             target = [target]
         elif target is None and self.config['Global']['char_only']:
             target = ['line_detector', 'localizer', 'char_recognizer']
         elif target is None and self.config['Global']['recognition_only']:
             target = ['word_recognizer', 'char_recognizer']
         elif target is None and self.config['Global']['skip_line_detection']:
             target = ['localizer', 'word_recognizer', 'char_recognizer']
         elif target is None:
             target = ['line_detector', 'localizer', 'word_recognizer', 'char_recognizer']
         elif not isinstance(target, list):
             raise ValueError('target must be a single training procedure or a list of training procedures')
-
+            
         for t in target:
             print(f"\n\n*** TRAINING: {t} ***\n\n")
             if t not in self.training_funcs.keys():
                 raise ValueError('target must be one of {}'.format(self.training_funcs.keys()))
             else:
                 self.training_funcs[t](**kwargs)
 
@@ -189,18 +201,20 @@
 
 
     def _train_word_recognizer(self, **kwargs):
         self.word_model.train(self.data_json, self.data_dir, **kwargs)
 
 
     def _train_char_recognizer(self, **kwargs):
+        print(self.data_json)
+        print(self.data_dir)
         self.char_model.train(self.data_json, self.data_dir, **kwargs)
 
     
-    def infer(self, imgs, make_coco_annotations=None, visualize=None, save_crops = None, **kwargs):
+    def infer(self, imgs, make_coco_annotations=None, visualize=None, save_crops = None, to_display = None, **kwargs):
         '''
         Inference pipeline has five steps:
         1. Loading and formatting images
         2. Line Detection
         3. Word and Character Detection
         4. Word Recognition
         5. Character Recognition
@@ -382,15 +396,16 @@
 
         if make_coco_annotations is not None or visualize is not None or save_crops is not None:
             make_coco_from_effocr_result(final_results, imgs, save_path=make_coco_annotations if isinstance(make_coco_annotations, str) else "./data/coco_annotations.json")
 
         if visualize is not None:
             visualize_effocr_result(imgs, 
                                     annotations_path = make_coco_annotations if isinstance(make_coco_annotations, str) else "./data/coco_annotations.json",
-                                    save_path = visualize if isinstance(visualize, str) else "./data/visualized_effocr_result.jpg")
+                                    save_path = visualize if isinstance(visualize, str) else "./data/visualized_effocr_result.jpg",
+                                    to_display = to_display)
                                     # skip_lines = self.config['Global']['skip_line_detection'], char_only = self.config['Global']['char_only']
 
 
         return final_results
     
 
     def infer_simple(self, imgs):
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/recognition/infer_recognize.py` & `efficient_ocr-0.1.0/src/efficient_ocr/recognition/infer_recognize.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/recognition/recognizermodel.py` & `efficient_ocr-0.1.0/src/efficient_ocr/recognition/recognizermodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,43 +153,71 @@
         self.config = config
         self.type = type
         self.transform = get_transform(type, self.config['Recognizer'][self.type]['training']['imsize'])
         self.initialize_model()
 
 
     def initialize_model(self):
-
+        print('Initializing model...')
         if not self.config['Recognizer'][self.type]['hf_repo_id'] is None:
 
             print(f"Loading (HF) pretrained {self.type} recognizer model!")
 
-            for fn in ['ref.txt', 'ref.index']:
-                hf_hub_download(
-                    repo_id=self.config['Recognizer'][self.type]['hf_repo_id'],
-                    filename=fn,
-                    local_dir=self.config['Recognizer'][self.type]['model_dir'],
-                    local_dir_use_symlinks=False,
-                    token=self.config['Global']['hf_token_for_upload']
-                )
+            # Allow users to append to the huggingface hub repo any inner folders they need to naviagte
+            # Works because hf hub repos will always be owner/repo_name, so anything after is a path
+                
+            # remove any leading or trailing slashes
+            repo_id = self.config['Recognizer'][self.type]['hf_repo_id'].strip('/')
+            # split on slashes
+            if len(repo_id.split('/')) == 2:
+                fn_prefix = ''
+            elif len(repo_id.split('/')) < 2:
+                raise ValueError('hf_repo_id must be in the format owner/repo_name, for example: dell-research-harvard/effocr_en')
+            else:
+                if self.config['Recognizer'][self.type]['model_backend'] == 'timm':
+                    raise ValueError('huggingface models loaded by timm must follow standard conventions. Interior files are not allowed. See https://huggingface.co/docs/timm/hf_hub')
+                else:
+                    fn_prefix = '/'.join(repo_id.split('/')[2:]) + '/' # Careful, order matters here
+                    repo_id = '/'.join(repo_id.split('/')[:2])
+
+            if self.config['Recognizer'][self.type]['model_backend'] == 'timm':
+                model_suffix = '.pth'
+            elif self.config['Recognizer'][self.type]['model_backend'] == 'onnx':
+                model_suffix = '.onnx'
+
 
+            for fn in ['ref.txt', 'ref.index']:    
+                if not os.path.exists(os.path.join(self.config['Recognizer'][self.type]['model_dir'], fn_prefix + fn)):            
+                    hf_hub_download(
+                        repo_id=repo_id,
+                        filename=fn_prefix+fn,
+                        local_dir=self.config['Recognizer'][self.type]['model_dir'],
+                        local_dir_use_symlinks=False,
+                        token=self.config['Global']['hf_token_for_upload']
+                    )
+            
+            self.config['Recognizer'][self.type]['model_dir'] = os.path.join(self.config['Recognizer'][self.type]['model_dir'], fn_prefix)
             self.index = faiss.read_index(get_path(self.config['Recognizer'][self.type]['model_dir'], ext="index"))
 
             with open(get_path(self.config['Recognizer'][self.type]['model_dir'], "txt"), 'r') as f:
                 self.candidates = f.read().splitlines()
 
             if self.type == 'word':
                 self.candidates = [ord_str_to_word(candidate) for candidate in self.candidates]
 
             if self.config['Recognizer'][self.type]['model_backend'] == 'timm':
                 self.model = timm.create_model(f"hf-hub:{self.config['Recognizer'][self.type]['hf_repo_id']}", num_classes=0, pretrained=True)
                 self.save_model(self.config['Recognizer'][self.type]["model_dir"], self.model, "pretrained", False)
                 self.input_name = None
             elif self.config['Recognizer'][self.type]['model_backend'] == 'onnx':
                 self.model, self.input_name, _ = initialize_onnx_model(
-                    get_path(self.config['Recognizer'][self.type]['model_dir'], ext="onnx"), 
+                    hf_hub_download(repo_id=repo_id,
+                        filename=fn_prefix + 'enc_best' + model_suffix,
+                        local_dir=self.config['Recognizer'][self.type]['model_dir'],
+                        local_dir_use_symlinks=False), 
                     self.config['Recognizer'][self.type])
 
         elif not get_path(self.config['Recognizer'][self.type]['model_dir'], ext="index") is None:
         
             print(f"Loading (local) pretrained {self.type} recognizer model!")
 
             self.index = faiss.read_index(get_path(self.config['Recognizer'][self.type]['model_dir'], ext="index"))
@@ -210,21 +238,20 @@
 
             elif self.config['Recognizer'][self.type]['model_backend'] == 'onnx':
                 self.model, self.input_name, _ = initialize_onnx_model(
                     get_path(self.config['Recognizer'][self.type]['model_dir'], ext="onnx"), 
                     self.config['Recognizer'][self.type])
 
         else:
-
             self.index = None
             self.candidates = None
             self.model = timm.create_model(self.config['Recognizer'][self.type]['timm_model_name'], num_classes=0, pretrained=True)
             self.input_name = None
         
-        if self.config['Recognizer'][self.type]['model_backend'] == 'timm':
+        if self.config['Recognizer'][self.type]['model_backend'] == 'timm' and self.index is not None:
             self.model.eval()
             self.model.to(self.config['Recognizer'][self.type]['device'])
             self.knn_func = FaissKNN(index_init_fn=faiss.IndexFlatIP, reset_before=False, reset_after=False)
             self.infm = InferenceModel(self.model, knn_func=self.knn_func, data_device='cpu')
             self.infm.load_knn_func(get_path(self.config['Recognizer'][self.type]['model_dir'], ext="index"))
 
 
@@ -276,16 +303,17 @@
 
         if kwargs:
             config = dictmerge(config, kwargs)
 
         if not self.config['Recognizer'][self.type]['model_backend'] == 'timm':
             raise NotImplementedError('Training is only supported for timm models')
         
-        assert self.config['Recognizer'][self.type]['training']['render_dict'] is not None
-        assert self.config['Recognizer'][self.type]['training']['font_dir_path'] is not None
+        if not os.path.isdir(self.config['Recognizer'][self.type]['training']["ready_to_go_data_dir_path"]):
+            assert self.config['Recognizer'][self.type]['training']['render_dict'] is not None
+            assert self.config['Recognizer'][self.type]['training']['font_dir_path'] is not None
         
         os.makedirs(self.config['Recognizer'][self.type]["model_dir"], exist_ok=True)
         self.model.to('cuda' if torch.cuda.is_available() else 'cpu')
 
         ## Create training data from input coco if not already created
         self._get_training_data(data_json, data_dir)
        
@@ -297,19 +325,21 @@
         self.initialize_model()
 
 
     def _get_training_data(self, data_json, data_dir):
         """
         Transcriptions are currently being passed along with file names
         """
+        if not os.path.exists(self.config['Recognizer'][self.type]['training']["ready_to_go_data_dir_path"]):
+            self.config['Recognizer'][self.type]['training']["ready_to_go_data_dir_path"] = \
+                os.path.join(self.config['Recognizer'][self.type]["model_dir"], "ready_to_go_training_data")
 
-        self.config['Recognizer'][self.type]['training']["ready_to_go_data_dir_path"] = \
-            os.path.join(self.config['Recognizer'][self.type]["model_dir"], "ready_to_go_training_data")
-
-        if not os.path.exists(os.path.join(self.config['Recognizer'][self.type]["model_dir"], "ready_to_go_training_data")):
+        
+        if not os.path.exists(os.path.join(self.config['Recognizer'][self.type]["model_dir"], "ready_to_go_training_data")) and \
+            not os.path.exists(self.config['Recognizer'][self.type]['training']["ready_to_go_data_dir_path"]):
 
             # extract important metadata
 
             cat_catid_dict = {entry["name"]:entry["id"] for entry in data_json["categories"]}
             imageid_filename_dict = {x["id"]:x["file_name"] for x in data_json["images"]}
 
             try:
@@ -583,16 +613,18 @@
                 if not scheduler is None:
                     scheduler.step()
                     ###Log on wandb
                     if not self.config['Global']["wandb_project"] is None:
                         wandb.log({f"train/{self.type}/lr": scheduler.get_last_lr()[0]})
 
         ## test with best encoder
-
-        self.model.load_state_dict(torch.load(os.path.join(self.config['Recognizer'][self.type]["model_dir"], "best.pth")))
+        if self.datapara == False:
+            self.model.load_state_dict(torch.load(os.path.join(self.config['Recognizer'][self.type]["model_dir"], "best.pth")))
+        else:
+            self.model.module.load_state_dict(torch.load(os.path.join(self.config['Recognizer'][self.type]["model_dir"], "best.pth")))
 
         self.save_ref_index(render_dataset, self.model, self.config['Recognizer'][self.type]["model_dir"])
 
         if self.config['Recognizer'][self.type]['training']["test_at_end"]:
             print("Testing on test set...")
             self.tester_knn(test_dataset, render_dataset, self.model, "test", log=not self.config['Global']["wandb_project"] is None)
             print("Test set testing complete.")
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/__init__.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/default_config.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/default_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 
 DEFAULT_CONFIG = {
     'Global': {
         'char_only': False,
         'recognition_only': False,
         'skip_line_detection': False,
+        'single_model_training': None,
         'wandb_project': None,
         'hf_username_for_upload': None,
         'hf_token_for_upload': None,
         'min_word_sim': 0.8
     },
     'Recognizer': {
         'char': {
@@ -117,36 +118,40 @@
         'vertical': False,
         'hf_repo_id': None,
         'mmdet_config': None,
         'num_cores': None,
         'providers': None,
         'visualize': None,
         'training': {
+            'training_data_dir': None,
             'batch_size': 16,
             'conf_thresh': 0.25,
             'epochs': 10,
             'input_shape': [640, 640],
             'iou_thresh': 0.1,
             'max_det': 200,
+            'device': 'cpu'
         }
     },
     'Line': {
         'model_dir': './line_model',
         'model_backend': 'yolov5',
         'device': 'cpu',
         'hf_repo_id': None,
         'num_cores': None,
         'onnx': None,
         'providers': None,
         'visualize': None,
         'training': {
+            'training_data_dir': None,
             'batch_size': 16,
             'conf_thresh': 0.2,
             'epochs': 10,
             'input_shape': [640, 640],
             'iou_thresh': 0.15,
             'max_det': 200,
             'min_seg_ratio': 2,
+            'device': 'cpu'
         }
     },
 }
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/misc.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/onnx.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/ops.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -410,15 +410,18 @@
                 coco['annotations'].append(char_anno)
 
     if save_path is not None:
         with open(save_path, 'w') as f:
             json.dump(coco, f, indent=4)
 
 
-def visualize_effocr_result(imgs, annotations_path, save_path):
+def visualize_effocr_result(imgs, annotations_path, save_path, to_display = 'full'):
+    if to_display is None:
+        to_display = 'full'
+        
     with open(annotations_path, 'r') as infile:
         coco = json.load(infile)
 
     for img_idx, img in enumerate(imgs):
         img_coco = coco['images'][img_idx]
 
         # Create a blank white canvas with height and width 3x the original image's
@@ -463,23 +466,34 @@
                 elif anno['category_id'] == cat_mapping['word']:
                     cv2.rectangle(word_canvas, (x0, y0), (x0 + x1, y0 + y1), (0, 255, ), 1)
                 elif anno['category_id'] == cat_mapping['char']:
                     cv2.rectangle(char_canvas, (x0, y0), (x0 + x1, y0 + y1), (255, 0, 0), 1)
 
         # Paste the three canvases into the main canvas, with the top height at (1.5 image height) and top corners evenly spaced, starting at .5 image width
         # Scale down all three images to 2/3 of their original size
-        line_canvas = cv2.resize(line_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
-        word_canvas = cv2.resize(word_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
-        char_canvas = cv2.resize(char_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
+        line_canvas_ = cv2.resize(line_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
+        word_canvas_ = cv2.resize(word_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
+        char_canvas_ = cv2.resize(char_canvas, (2 * img_coco['width'] // 3, 2 * img_coco['height'] // 3))
         y_top = int(1.5 * img_coco['height'])
         x_left = int(.25 * img_coco['width'])
-        canvas[y_top:y_top + line_canvas.shape[0], x_left : x_left + line_canvas.shape[1]] = line_canvas
+        canvas[y_top:y_top + line_canvas_.shape[0], x_left : x_left + line_canvas_.shape[1]] = line_canvas_
         x_left = int(1.166 * img_coco['width'])
-        canvas[y_top:y_top + word_canvas.shape[0], x_left : x_left + word_canvas.shape[1]] = word_canvas
+        canvas[y_top:y_top + word_canvas_.shape[0], x_left : x_left + word_canvas_.shape[1]] = word_canvas_
         x_left = int(2.083 * img_coco['width'])
-        canvas[y_top:y_top + char_canvas.shape[0], x_left : x_left + char_canvas.shape[1]] = char_canvas
+        canvas[y_top:y_top + char_canvas_.shape[0], x_left : x_left + char_canvas_.shape[1]] = char_canvas_
 
+        if to_display == 'full':
+            to_save = canvas
+        elif to_display == 'line':
+            to_save = line_canvas
+        elif to_display == 'word':
+            to_save = word_canvas
+        elif to_display == 'char':
+            to_save = char_canvas
+        else:
+            raise ValueError('to_display must be one of "full", "line", "word", or "char"')
+        
         # Save the canvas to the save_path
         if save_path.endswith('png') or save_path.endswith('jpg'):
-            cv2.imwrite(save_path, canvas)
+            cv2.imwrite(save_path, to_save)
         else:
-            cv2.imwrite(os.path.join(save_path, str(img_idx) + '.png'), canvas)
+            cv2.imwrite(os.path.join(save_path, str(img_idx) + '.png'), to_save)
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/custom_schedulers.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/custom_schedulers.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/datasets.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/datasets.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/encoders.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/encoders.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/samplers.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/samplers.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/synth_crops.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/synth_crops.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/recognition/transforms.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/recognition/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
     def __call__(self, image):
 
         _, h, w = image.size()
         new_w =[int(w*p) for p in self.pcts]        
         
-        return T.Resize((h, np.random.choice(new_w)))(image)
+        return T.Resize((h, np.random.choice(new_w)), antialias = True)(image)
 
 
 class TransformLoader:
 
 
     def __init__(self, loader, transform):
         self.loader = loader
@@ -159,17 +159,17 @@
 
     w, h = pil_img.size
     larger_side = max([w, h])
     height_larger = larger_side == h 
     aspect_ratio = w / h if height_larger else h / w
     
     if height_larger:
-        patch_resizer = T.Resize((targetsize, (int(aspect_ratio*targetsize) // patchsize) * patchsize))
+        patch_resizer = T.Resize((targetsize, (int(aspect_ratio*targetsize) // patchsize) * patchsize), antialias=True)
     else:
-        patch_resizer = T.Resize(((int(aspect_ratio*targetsize) // patchsize) * patchsize, targetsize))
+        patch_resizer = T.Resize(((int(aspect_ratio*targetsize) // patchsize) * patchsize, targetsize), antialias=True)
 
     return patch_resizer(pil_img)
 
 
 def color_shift(im):
     color = list(np.random.random(size=3))
     im[0, :, :][im[0, :, :] >= 0.8] = color[0]
@@ -198,15 +198,15 @@
             T.RandomApply([T.ColorJitter(brightness=0.5, contrast=0.3, saturation=0.3, hue=0.3)], p=0.5),
             T.ToPILImage(),
             lambda x: Image.fromarray(A.GaussNoise(var_limit=(10.0, 150.0), mean=0, p=0.25)(image=np.array(x))["image"]),
             T.RandomApply([T.GaussianBlur(15, sigma=(1, 15))], p=0.3),
             T.RandomGrayscale(p=0.2),
             CharMedianPad(override=(255,255,255)),
             T.ToTensor(),
-            T.Resize((size, size)),
+            T.Resize((size, size), antialias=True),
             T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
         ])
     elif char_trans_version == 1: # suggested for japanese
         return T.Compose([
             T.ToTensor(),
             T.RandomApply([T.RandomAffine(degrees=0, translate=(0.1, 0.1), scale=(0.9, 1.1), fill=1)], p=0.7) if latin_suggested_augs \
                 else T.RandomApply([T.RandomAffine(degrees=0, translate=(0.2, 0.2), scale=(0.8, 1), fill=1)], p=0.7),
@@ -215,15 +215,15 @@
             T.RandomApply([random_erode_dilate], p=0.5) if latin_suggested_augs else lambda x: x,
             T.ToPILImage(),
             lambda x: Image.fromarray(A.GaussNoise(var_limit=(10.0, 150.0), mean=0, p=0.25)(image=np.array(x))["image"]),
             T.RandomApply([T.GaussianBlur(11, sigma=(0.1, 2.0))], p=0.3), # T.RandomApply([T.GaussianBlur(15, sigma=(1, 4))], p=0.3)
             T.RandomGrayscale(p=0.2),
             CharMedianPad(override=(255,255,255)),
             T.ToTensor(),
-            T.Resize((size, size)),
+            T.Resize((size, size), antialias=True),
             T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
         ])
     else:
         raise NotImplementedError
 
 
 def create_render_transform(high_blur, size=224,normalize=True,resize_pad=True):
@@ -257,49 +257,49 @@
         lambda x: Image.fromarray(A.GaussNoise(var_limit=(10.0, 150.0), mean=0, p=0.8)(image=np.array(x))["image"]),
         blur_transform(high_blur),
         T.RandomGrayscale(p=0.2),
         MedianPad(random_pad=True) if resize_pad else lambda x: x,
         # CharMedianPad(override=(255,255,255)) if resize_pad else lambda x: x,
         T.ToTensor(),
         ###We also want to blow up the image. So will first expand it to 2x and then resize to 224 (21-04:1307)
-        T.Resize((size*4, size*4) if resize_pad else lambda x: x),
-        T.Resize((size, size) if resize_pad else lambda x: x),
+        T.Resize((size*4, size*4) if resize_pad else lambda x: x, antialias=True),
+        T.Resize((size, size) if resize_pad else lambda x: x, antialias=True),
         T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD) if normalize else lambda x: x,
     ])
 
 
 def create_paired_transform(size=224):
     return T.Compose([
         T.ToTensor(),
         T.ToPILImage(),
         MedianPad(),
         T.ToTensor(),
-        T.Resize((size, size)),
+        T.Resize((size, size), antialias=True),
         T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
     ])
 
 
 def create_paired_transform_char(size=224):
     return T.Compose([
         CharMedianPad(override=(255,255,255)),
         T.ToTensor(),
-        T.Resize((size, size)),
+        T.Resize((size, size), antialias=True),
         T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
     ])
 
 
 def create_inference_transform(size=224):
     return T.Compose([
         T.ToTensor(),
         T.ToPILImage(),
         CharMedianPad(override=(255,255,255)),
-        T.Resize((size, size)),
+        T.Resize((size, size), antialias=True),
     ])
 
 
 def create_inference_transform_char(size=224):
     return T.Compose([
         CharMedianPad(),
-        T.Resize((size, size)),
+        T.Resize((size, size), antialias=True),
         ##Convert to pil image
     ])
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/text.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/text.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/transforms.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 
 def get_transform(type='char', size=224):
 
     if type == 'char':
         return T.Compose([
             MedianPad(override=(255,255,255)),
             T.ToTensor(),
-            T.Resize((size, size)),
+            T.Resize((size, size), antialias=True),
             T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
             lambda x: x.unsqueeze(0)
         ])
     elif type == 'word':
         return T.Compose([
             MedianPadWord(aspect_cutoff=0),
             T.ToTensor(),
-            T.Resize((size, size)),
+            T.Resize((size, size), antialias=True),
             T.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD),
             lambda x: x.unsqueeze(0)
         ])
     else:
         raise ValueError('Unknown type for recognizer: {}'.format(type))
```

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr/utils/yolo.py` & `efficient_ocr-0.1.0/src/efficient_ocr/utils/yolo.py`

 * *Files identical despite different names*

### Comparing `efficient_ocr-0.0.5/src/efficient_ocr.egg-info/SOURCES.txt` & `efficient_ocr-0.1.0/src/efficient_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

