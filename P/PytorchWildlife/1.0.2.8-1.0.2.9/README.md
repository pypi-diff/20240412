# Comparing `tmp/PytorchWildlife-1.0.2.8.tar.gz` & `tmp/PytorchWildlife-1.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PytorchWildlife-1.0.2.8.tar", last modified: Tue Apr  9 22:43:58 2024, max compression
+gzip compressed data, was "PytorchWildlife-1.0.2.9.tar", last modified: Fri Apr 12 00:51:23 2024, max compression
```

## Comparing `PytorchWildlife-1.0.2.8.tar` & `PytorchWildlife-1.0.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.069585 PytorchWildlife-1.0.2.8/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     1070 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/LICENSE
--rw-r--r--   0 zhongqimiao   (501) staff       (20)    20648 2024-04-09 22:43:58.069056 PytorchWildlife-1.0.2.8/PKG-INFO
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.050755 PytorchWildlife-1.0.2.8/PW_FT_classification/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       38 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PW_FT_classification/__init__.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     7449 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PW_FT_classification/main.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.051464 PytorchWildlife-1.0.2.8/PytorchWildlife/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)      315 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/__init__.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.060665 PytorchWildlife-1.0.2.8/PytorchWildlife/data/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       49 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/__init__.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     3764 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/datasets.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     5526 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/data/transforms.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.061142 PytorchWildlife-1.0.2.8/PytorchWildlife/models/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       54 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/__init__.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.061715 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       21 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/__init__.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.064648 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)      100 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/__init__.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     3162 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/amazon.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     5315 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/base_classifier.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     2297 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/opossum.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     2548 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/serengeti.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.065041 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       21 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/__init__.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.066205 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       56 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/__init__.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     6024 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/base_detector.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     1499 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/megadetector.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.067602 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       47 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/__init__.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     1874 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/misc.py
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     6670 2024-04-09 22:31:58.000000 PytorchWildlife-1.0.2.8/PytorchWildlife/utils/post_process.py
-drwxr-xr-x   0 zhongqimiao   (501) staff       (20)        0 2024-04-09 22:43:58.068049 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/
--rw-r--r--   0 zhongqimiao   (501) staff       (20)    20648 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/PKG-INFO
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     1098 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/SOURCES.txt
--rw-r--r--   0 zhongqimiao   (501) staff       (20)        1 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/dependency_links.txt
--rw-r--r--   0 zhongqimiao   (501) staff       (20)      148 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/requires.txt
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       37 2024-04-09 22:43:57.000000 PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/top_level.txt
--rw-r--r--   0 zhongqimiao   (501) staff       (20)    19803 2024-04-09 21:48:20.000000 PytorchWildlife-1.0.2.8/README.md
--rw-r--r--   0 zhongqimiao   (501) staff       (20)       38 2024-04-09 22:43:58.069643 PytorchWildlife-1.0.2.8/setup.cfg
--rw-r--r--   0 zhongqimiao   (501) staff       (20)     1432 2024-04-09 22:37:03.000000 PytorchWildlife-1.0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    20866 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:22.974611 PytorchWildlife-1.0.2.9/PW_FT_classification/
+-rw-rw-rw-   0        0        0       38 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PW_FT_classification/__init__.py
+-rw-rw-rw-   0        0        0     7627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PW_FT_classification/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:22.984142 PytorchWildlife-1.0.2.9/PytorchWildlife/
+-rw-rw-rw-   0        0        0      324 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.046106 PytorchWildlife-1.0.2.9/PytorchWildlife/data/
+-rw-rw-rw-   0        0        0       50 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/__init__.py
+-rw-rw-rw-   0        0        0     3884 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/datasets.py
+-rw-rw-rw-   0        0        0     5685 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/data/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.054540 PytorchWildlife-1.0.2.9/PytorchWildlife/models/
+-rw-rw-rw-   0        0        0       55 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.063002 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/
+-rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.117808 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/
+-rw-rw-rw-   0        0        0      103 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/__init__.py
+-rw-rw-rw-   0        0        0     3267 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/amazon.py
+-rw-rw-rw-   0        0        0     5470 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/base_classifier.py
+-rw-rw-rw-   0        0        0     2367 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/opossum.py
+-rw-rw-rw-   0        0        0     2627 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/serengeti.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.126222 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/
+-rw-rw-rw-   0        0        0       21 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.158140 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/
+-rw-rw-rw-   0        0        0       57 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/__init__.py
+-rw-rw-rw-   0        0        0     6648 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/base_detector.py
+-rw-rw-rw-   0        0        0     1546 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/megadetector.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.188442 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/
+-rw-rw-rw-   0        0        0       48 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-04-12 00:50:31.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/misc.py
+-rw-rw-rw-   0        0        0    10090 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/PytorchWildlife/utils/post_process.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:23.017998 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/
+-rw-rw-rw-   0        0        0    20866 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-04-12 00:51:22.000000 PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19962 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 00:51:23.190441 PytorchWildlife-1.0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2024-04-12 00:50:43.000000 PytorchWildlife-1.0.2.9/setup.py
```

### Comparing `PytorchWildlife-1.0.2.8/PKG-INFO` & `PytorchWildlife-1.0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,367 +1,337 @@
-Metadata-Version: 2.1
-Name: PytorchWildlife
-Version: 1.0.2.8
-Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
-Home-page: https://github.com/microsoft/CameraTraps/
-Author: Andres Hernandez, Zhongqi Miao
-Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
-License: MIT
-Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: torch==1.10.1
-Requires-Dist: torchvision==0.11.2
-Requires-Dist: torchaudio==0.10.1
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: Pillow==10.1.0
-Requires-Dist: supervision==0.16.0
-Requires-Dist: gradio==4.8.0
-Requires-Dist: ultralytics-yolov5
-Requires-Dist: chardet
-
-![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
-
-<div align="center"> 
-<font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
-<br>
-<hr>
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
-<a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
-<a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
-<!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
-<a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
-<a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
-<a href="https://discord.gg/TeEVxzaYtm"><img src="https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=Discord" /></a>
-<br><br>
-</div>
-
-
-## ✅ Update highlights (Version 1.0.2)
-- [x] Added Google Colab demos.
-- [x] Added Snapshot Serengeti classification model into the model zoo.
-- [x] Added Classification fine-tuning module.
-- [x] Added a Docker Image for ease of installation.
-
-## 🔥 Future highlights
-- [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
-- [ ] Direct Timelapse format outputs for both detection and classification.
-- [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
-- [ ] Direct LILA connection for more training/validation data.
-- [ ] More pretrained detection and classification models to expand the current model zoo.
-
-To check the full version of the roadmap with completed tasks and long term goals, please click [here!](roadmaps.md).
-
-## 🐾 Introduction
-
-At the core of our mission is the desire to create a harmonious space where conservation scientists from all over the globe can unite. Where they're able to share, grow, use datasets and deep learning architectures for wildlife conservation.
-We've been inspired by the potential and capabilities of Megadetector, and we deeply value its contributions to the community. As we forge ahead with Pytorch-Wildlife, under which Megadetector now resides, please know that we remain committed to supporting, maintaining, and developing Megadetector, ensuring its continued relevance, expansion, and utility.
-
-Pytorch-Wildlife is pip installable:
-```
-pip install PytorchWildlife
-```
-
-To use the newest version of MegaDetector with all the existing functionalities, you can use our [Hugging Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model with **Pytorch-Wildlife**. The weights will be automatically downloaded:
-```python
-from PytorchWildlife.models import detection as pw_detection
-detection_model = pw_detection.MegaDetectorV5()
-```
-
-For those interested in accessing the previous MegaDetector repository, which utilizes the same `MegaDetector v5` model weights and was primarily developed by Dan Morris during his time at Microsoft, please visit the [archive](https://github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that Dan Morris is actively maintaining.
-
->[!TIP]
->If you have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
-
-## 👋 Welcome to Pytorch-Wildlife Version 1.0
-
-**PyTorch-Wildlife** is a platform to create, modify, and share powerful AI conservation models. These models can be used for a variety of applications, including camera trap images, overhead images, underwater images, or bioacoustics. Your engagement with our work is greatly appreciated, and we eagerly await any feedback you may have.
-
-
-The **Pytorch-Wildlife** library allows users to directly load the `MegaDetector v5` model weights for animal detection. We've fully refactored our codebase, prioritizing ease of use in model deployment and expansion. In addition to `MegaDetector v5`, **Pytorch-Wildlife** also accommodates a range of classification weights, such as those derived from the Amazon Rainforest dataset and the Opossum classification dataset. Explore the codebase and functionalities of **Pytorch-Wildlife** through our interactive [HuggingFace web app](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or local [demos and notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo), designed to showcase the practical applications of our enhancements at [PyTorchWildlife](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md). You can find more information in our [documentation](https://cameratraps.readthedocs.io/en/latest/).
-
-👇 Here is a brief example on how to perform detection and classification on a single image using `PyTorch-wildlife`
-```python
-import torch
-from PytorchWildlife.models import detection as pw_detection
-from PytorchWildlife.models import classification as pw_classification
-
-img = torch.randn((3, 1280, 1280))
-
-# Detection
-detection_model = pw_detection.MegaDetectorV5() # Model weights are automatically downloaded.
-detection_result = detection_model.single_image_detection(img)
-
-#Classification
-classification_model = pw_classification.AI4GAmazonRainforest() # Model weights are automatically downloaded.
-classification_results = classification_model.single_image_classification(img)
-```
-
-## ⚙️ Install Pytorch-Wildlife
-```
-pip install PytorchWildlife
-```
-Please refer to our [installation guide](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) for more installation information.
-
-## 🕵️ Explore Pytorch-Wildlife and MegaDetector with our Demo User Interface
-
-If you want to directly try **Pytorch-Wildlife** with the AI models available, including `MegaDetector v5`, you can use our [**Gradio** interface](https://github.com/microsoft/CameraTraps/tree/main/demo). This interface allows users to directly load the `MegaDetector v5` model weights for animal detection. In addition, **Pytorch-Wildlife** also has two classification models in our initial version. One is trained from an Amazon Rainforest camera trap dataset and the other from a Galapagos opossum classification dataset (more details of these datasets will be published soon). To start, please follow the [installation instructions](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) on how to run the Gradio interface! We also provide multiple [**Jupyter** notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo) for demonstration.
-
-![image](https://microsoft.github.io/CameraTraps/assets/gradio_UI.png)
-
-
-## 🛠️ Core Features
-   What are the core components of Pytorch-Wildlife?
-![Pytorch-core-diagram](https://microsoft.github.io/CameraTraps/assets/Pytorch_Wildlife_core_figure.jpg)
-
-
-### 🌐 Unified Framework:
-  Pytorch-Wildlife integrates **four pivotal elements:**
-
-▪ Machine Learning Models<br>
-▪ Pre-trained Weights<br>
-▪ Datasets<br>
-▪ Utilities<br>
-
-### 👷 Our work:
-  In the provided graph, boxes outlined in red represent elements that will be added and remained fixed, while those in blue will be part of our development.
-
-
-### 🚀 Inaugural Model:
-  We're kickstarting with YOLO as our first available model, complemented by pre-trained weights from `MegaDetector v5`. This is the same `MegaDetector v5` model from the previous repository.
-
-
-### 📚 Expandable Repository:
-  As we move forward, our platform will welcome new models and pre-trained weights for camera traps and bioacoustic analysis. We're excited to host contributions from global researchers through a dedicated submission platform.
-
-
-### 📊 Datasets from LILA:
-  Pytorch-Wildlife will also incorporate the vast datasets hosted on LILA, making it a treasure trove for conservation research.
-
-
-### 🧰 Versatile Utilities:
-  Our set of utilities spans from visualization tools to task-specific utilities, many inherited from Megadetector.
-
-
-### 💻 User Interface Flexibility:
-  While we provide a foundational user interface, our platform is designed to inspire. We encourage researchers to craft and share their unique interfaces, and we'll list both existing and new UIs from other collaborators for the community's benefit.
-
-
-Let's shape the future of wildlife research, together! 🙌
-
-
-### 📈 Progress on core tasks
-
-<details>
-<summary> <font size="3"> ▪️ Packaging </font> </summary>
-
-- [ ] Animal detection fine-tuning<br>
-- [x] MegaDetectorV5 integration<br>
-- [ ] MegaDetectorV6 integration<br>
-- [x] User submitted weights<br>
-- [x] Animal classification fine-tuning<br>
-- [x] Amazon Rainforest classification<br>
-- [x] Amazon Opossum classification<br>
-- [ ] User submitted weights<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Utility Toolkit</font></summary>
-
-- [x] Visualization tools<br>
-- [x] MegaDetector utils<br>
-- [ ] User submitted utils<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Datasets</font></summary>
-
-- [ ] Animal Datasets<br>
-- [ ] LILA datasets<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Accessibility</font></summary>
-
-- [x] Basic user interface for demonstration<br>
-- [ ] UI Dev tools<br>
-- [ ] List of available UIs<br>
-</details><br>
-
-
-## 🖼️ Examples
-
-### Image detection using `MegaDetector v5`
-<img src="https://microsoft.github.io/CameraTraps/assets/animal_det_1.JPG" alt="animal_det_1" width="400"/><br>
-*Credits to Universidad de los Andes, Colombia.*
-
-### Image classification with `MegaDetector v5` and `AI4GAmazonRainforest`
-<img src="https://microsoft.github.io/CameraTraps/assets/animal_clas_1.png" alt="animal_clas_1" width="500"/><br>
-*Credits to Universidad de los Andes, Colombia.*
-
-### Opossum ID with `MegaDetector v5` and `AI4GOpossum`
-<img src="https://microsoft.github.io/CameraTraps/assets/opossum_det.png" alt="opossum_det" width="500"/><br>
-*Credits to the Agency for Regulation and Control of Biosecurity and Quarantine for Galápagos (ABG), Ecuador.*
-
-
-## 🤝 Contributing
-This project is open to your ideas and contributions. If you want to submit a pull request, we'll have some guidelines available soon.
-
-We have adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [us](zhongqimiao@microsoft.com) with any additional questions or comments.
-
-## License
-This repository is licensed with the [MIT license](https://github.com/Microsoft/dotnet/blob/main/LICENSE).
-
-
-## 👥 Existing Collaborators
-
-The extensive collaborative efforts of Megadetector have genuinely inspired us, and we deeply value its significant contributions to the community. As we continue to advance with Pytorch-Wildlife, our commitment to delivering technical support to our existing partners on MegaDetector remains the same.
-
-Here we list a few of the organizations that have used MegaDetector. We're only listing organizations who have given us permission to refer to them here or have posted publicly about their use of MegaDetector.
-
-<details>
-<summary><font size="3">👉 Full list of organizations</font></summary>
-
-(Newly Added) [TerrOïko](https://www.terroiko.fr/) ([OCAPI platform](https://www.terroiko.fr/ocapi))
-
-[Arizona Department of Environmental Quality](http://azdeq.gov/)
-
-[Blackbird Environmental](https://blackbirdenv.com/)
-
-[Camelot](https://camelotproject.org/)
-
-[Canadian Parks and Wilderness Society (CPAWS) Northern Alberta Chapter](https://cpawsnab.org/)
-
-[Conservation X Labs](https://conservationxlabs.com/)
-
-[Czech University of Life Sciences Prague](https://www.czu.cz/en)
-
-[EcoLogic Consultants Ltd.](https://www.consult-ecologic.com/)
-
-[Estación Biológica de Doñana](http://www.ebd.csic.es/inicio)
-
-[Idaho Department of Fish and Game](https://idfg.idaho.gov/)
-
-[Island Conservation](https://www.islandconservation.org/)
-
-[Myall Lakes Dingo Project](https://carnivorecoexistence.info/myall-lakes-dingo-project/)
-
-[Point No Point Treaty Council](https://pnptc.org/)
-
-[Ramat Hanadiv Nature Park](https://www.ramat-hanadiv.org.il/en/)
-
-[SPEA (Portuguese Society for the Study of Birds)](https://spea.pt/en/)
-
-[Synthetaic](https://www.synthetaic.com/)
-
-[Taronga Conservation Society](https://taronga.org.au/)
-
-[The Nature Conservancy in Wyoming](https://www.nature.org/en-us/about-us/where-we-work/united-states/wyoming/)
-
-[TrapTagger](https://wildeyeconservation.org/trap-tagger-about/)
-
-[Upper Yellowstone Watershed Group](https://www.upperyellowstone.org/)
-
-[Applied Conservation Macro Ecology Lab](http://www.acmelab.ca/), University of Victoria
-
-[Banff National Park Resource Conservation](https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation), Parks Canada(https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation)
-
-[Blumstein Lab](https://blumsteinlab.eeb.ucla.edu/), UCLA
-
-[Borderlands Research Institute](https://bri.sulross.edu/), Sul Ross State University
-
-[Capitol Reef National Park](https://www.nps.gov/care/index.htm) / Utah Valley University
-
-[Center for Biodiversity and Conservation](https://www.amnh.org/research/center-for-biodiversity-conservation), American Museum of Natural History
-
-[Centre for Ecosystem Science](https://www.unsw.edu.au/research/), UNSW Sydney
-
-[Cross-Cultural Ecology Lab](https://crossculturalecology.net/), Macquarie University
-
-[DC Cat Count](https://hub.dccatcount.org/), led by the Humane Rescue Alliance
-
-[Department of Fish and Wildlife Sciences](https://www.uidaho.edu/cnr/departments/fish-and-wildlife-sciences), University of Idaho
-
-[Department of Wildlife Ecology and Conservation](https://wec.ifas.ufl.edu/), University of Florida
-
-[Ecology and Conservation of Amazonian Vertebrates Research Group](https://www.researchgate.net/lab/Fernanda-Michalski-Lab-4), Federal University of Amapá
-
-[Gola Forest Programma](https://www.rspb.org.uk/our-work/conservation/projects/scientific-support-for-the-gola-forest-programme/), Royal Society for the Protection of Birds (RSPB)
-
-[Graeme Shannon's Research Group](https://wildliferesearch.co.uk/group-1), Bangor University
-
-[Hamaarag](https://hamaarag.org.il/), The Steinhardt Museum of Natural History, Tel Aviv University
-
-[Institut des Science de la Forêt Tempérée (ISFORT)](https://isfort.uqo.ca/), Université du Québec en Outaouais
-
-[Lab of Dr. Bilal Habib](https://bhlab.in/about), the Wildlife Institute of India
-
-[Mammal Spatial Ecology and Conservation Lab](https://labs.wsu.edu/dthornton/), Washington State University
-
-[McLoughlin Lab in Population Ecology](http://mcloughlinlab.ca/lab/), University of Saskatchewan
-
-[National Wildlife Refuge System, Southwest Region](https://www.fws.gov/about/region/southwest), U.S. Fish & Wildlife Service
-
-[Northern Great Plains Program](https://nationalzoo.si.edu/news/restoring-americas-prairie), Smithsonian
-
-[Quantitative Ecology Lab](https://depts.washington.edu/sefsqel/), University of Washington
-
-[Santa Monica Mountains Recreation Area](https://www.nps.gov/samo/index.htm), National Park Service
-
-[Seattle Urban Carnivore Project](https://www.zoo.org/seattlecarnivores), Woodland Park Zoo
-
-[Serra dos Órgãos National Park](https://www.icmbio.gov.br/parnaserradosorgaos/), ICMBio
-
-[Snapshot USA](https://emammal.si.edu/snapshot-usa), Smithsonian
-
-[Wildlife Coexistence Lab](https://wildlife.forestry.ubc.ca/), University of British Columbia
-
-[Wildlife Research](https://www.dfw.state.or.us/wildlife/research/index.asp), Oregon Department of Fish and Wildlife
-
-[Wildlife Division](https://www.michigan.gov/dnr/about/contact/wildlife), Michigan Department of Natural Resources
-
-Department of Ecology, TU Berlin
-
-Ghost Cat Analytics
-
-Protected Areas Unit, Canadian Wildlife Service
-
-[School of Natural Sciences](https://www.utas.edu.au/natural-sciences), University of Tasmania [(story)](https://www.utas.edu.au/about/news-and-stories/articles/2022/1204-innovative-camera-network-keeps-close-eye-on-tassie-wildlife)
-
-[Kenai National Wildlife Refuge](https://www.fws.gov/refuge/kenai), U.S. Fish & Wildlife Service [(story)](https://www.peninsulaclarion.com/sports/refuge-notebook-new-technology-increases-efficiency-of-refuge-cameras/)
-
-[Australian Wildlife Conservancy](https://www.australianwildlife.org/) [(blog](https://www.australianwildlife.org/cutting-edge-technology-delivering-efficiency-gains-in-conservation/), [blog)](https://www.australianwildlife.org/efficiency-gains-at-the-cutting-edge-of-technology/)
-
-[Felidae Conservation Fund](https://felidaefund.org/) [(WildePod platform)](https://wildepod.org/) [(blog post)](https://abhaykashyap.com/blog/ai-powered-camera-trap-image-annotation-system/)
-
-[Alberta Biodiversity Monitoring Institute (ABMI)](https://www.abmi.ca/home.html) [(WildTrax platform)](https://www.wildtrax.ca/) [(blog post)](https://wildcams.ca/blog/the-abmi-visits-the-zoo/)
-
-[Shan Shui Conservation Center](http://en.shanshui.org/) [(blog post)](https://mp.weixin.qq.com/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs) [(translated blog post)](https://mp-weixin-qq-com.translate.goog/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs&_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp)
-
-[Irvine Ranch Conservancy](http://www.irconservancy.org/) [(story)](https://www.ocregister.com/2022/03/30/ai-software-is-helping-researchers-focus-on-learning-about-ocs-wild-animals/)
-
-[Wildlife Protection Solutions](https://wildlifeprotectionsolutions.org/) [(story](https://customers.microsoft.com/en-us/story/1384184517929343083-wildlife-protection-solutions-nonprofit-ai-for-earth), [story)](https://www.enterpriseai.news/2023/02/20/ai-helps-wildlife-protection-solutions-safeguard-endangered-species/)
-
-[Road Ecology Center](https://roadecology.ucdavis.edu/), University of California, Davis [(Wildlife Observer Network platform)](https://wildlifeobserver.net/)
-
-[The Nature Conservancy in California](https://www.nature.org/en-us/about-us/where-we-work/united-states/california/) [(Animl platform)](https://github.com/tnc-ca-geo/animl-frontend)
-
-[San Diego Zoo Wildlife Alliance](https://science.sandiegozoo.org/) [(Animl R package)](https://github.com/conservationtechlab/animl)
-
-</details><br>
-
-
->[!IMPORTANT]
->If you would like to be added to this list or have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our Discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
-
+![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
+
+<div align="center"> 
+<font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
+<br>
+<hr>
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
+<a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
+<a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
+<!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
+<a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
+<a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
+<a href="https://discord.gg/TeEVxzaYtm"><img src="https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=Discord" /></a>
+<br><br>
+</div>
+
+
+## ✅ Update highlights (Version 1.0.2.9)
+- [x] Added Timelapse compatibility! Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo).
+- [x] Added Google Colab demos.
+- [x] Added Snapshot Serengeti classification model into the model zoo.
+- [x] Added Classification fine-tuning module.
+- [x] Added a Docker Image for ease of installation.
+
+## 🔥 Future highlights
+- [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
+- [ ] Direct Timelapse format outputs for both detection and classification.
+- [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
+- [ ] Direct LILA connection for more training/validation data.
+- [ ] More pretrained detection and classification models to expand the current model zoo.
+
+To check the full version of the roadmap with completed tasks and long term goals, please click [here!](roadmaps.md).
+
+## 🐾 Introduction
+
+At the core of our mission is the desire to create a harmonious space where conservation scientists from all over the globe can unite. Where they're able to share, grow, use datasets and deep learning architectures for wildlife conservation.
+We've been inspired by the potential and capabilities of Megadetector, and we deeply value its contributions to the community. As we forge ahead with Pytorch-Wildlife, under which Megadetector now resides, please know that we remain committed to supporting, maintaining, and developing Megadetector, ensuring its continued relevance, expansion, and utility.
+
+Pytorch-Wildlife is pip installable:
+```
+pip install PytorchWildlife
+```
+
+To use the newest version of MegaDetector with all the existing functionalities, you can use our [Hugging Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model with **Pytorch-Wildlife**. The weights will be automatically downloaded:
+```python
+from PytorchWildlife.models import detection as pw_detection
+detection_model = pw_detection.MegaDetectorV5()
+```
+
+For those interested in accessing the previous MegaDetector repository, which utilizes the same `MegaDetector v5` model weights and was primarily developed by Dan Morris during his time at Microsoft, please visit the [archive](https://github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that Dan Morris is actively maintaining.
+
+>[!TIP]
+>If you have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
+
+## 👋 Welcome to Pytorch-Wildlife Version 1.0
+
+**PyTorch-Wildlife** is a platform to create, modify, and share powerful AI conservation models. These models can be used for a variety of applications, including camera trap images, overhead images, underwater images, or bioacoustics. Your engagement with our work is greatly appreciated, and we eagerly await any feedback you may have.
+
+
+The **Pytorch-Wildlife** library allows users to directly load the `MegaDetector v5` model weights for animal detection. We've fully refactored our codebase, prioritizing ease of use in model deployment and expansion. In addition to `MegaDetector v5`, **Pytorch-Wildlife** also accommodates a range of classification weights, such as those derived from the Amazon Rainforest dataset and the Opossum classification dataset. Explore the codebase and functionalities of **Pytorch-Wildlife** through our interactive [HuggingFace web app](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or local [demos and notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo), designed to showcase the practical applications of our enhancements at [PyTorchWildlife](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md). You can find more information in our [documentation](https://cameratraps.readthedocs.io/en/latest/).
+
+👇 Here is a brief example on how to perform detection and classification on a single image using `PyTorch-wildlife`
+```python
+import torch
+from PytorchWildlife.models import detection as pw_detection
+from PytorchWildlife.models import classification as pw_classification
+
+img = torch.randn((3, 1280, 1280))
+
+# Detection
+detection_model = pw_detection.MegaDetectorV5() # Model weights are automatically downloaded.
+detection_result = detection_model.single_image_detection(img)
+
+#Classification
+classification_model = pw_classification.AI4GAmazonRainforest() # Model weights are automatically downloaded.
+classification_results = classification_model.single_image_classification(img)
+```
+
+## ⚙️ Install Pytorch-Wildlife
+```
+pip install PytorchWildlife
+```
+Please refer to our [installation guide](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) for more installation information.
+
+## 🕵️ Explore Pytorch-Wildlife and MegaDetector with our Demo User Interface
+
+If you want to directly try **Pytorch-Wildlife** with the AI models available, including `MegaDetector v5`, you can use our [**Gradio** interface](https://github.com/microsoft/CameraTraps/tree/main/demo). This interface allows users to directly load the `MegaDetector v5` model weights for animal detection. In addition, **Pytorch-Wildlife** also has two classification models in our initial version. One is trained from an Amazon Rainforest camera trap dataset and the other from a Galapagos opossum classification dataset (more details of these datasets will be published soon). To start, please follow the [installation instructions](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) on how to run the Gradio interface! We also provide multiple [**Jupyter** notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo) for demonstration.
+
+![image](https://microsoft.github.io/CameraTraps/assets/gradio_UI.png)
+
+
+## 🛠️ Core Features
+   What are the core components of Pytorch-Wildlife?
+![Pytorch-core-diagram](https://microsoft.github.io/CameraTraps/assets/Pytorch_Wildlife_core_figure.jpg)
+
+
+### 🌐 Unified Framework:
+  Pytorch-Wildlife integrates **four pivotal elements:**
+
+▪ Machine Learning Models<br>
+▪ Pre-trained Weights<br>
+▪ Datasets<br>
+▪ Utilities<br>
+
+### 👷 Our work:
+  In the provided graph, boxes outlined in red represent elements that will be added and remained fixed, while those in blue will be part of our development.
+
+
+### 🚀 Inaugural Model:
+  We're kickstarting with YOLO as our first available model, complemented by pre-trained weights from `MegaDetector v5`. This is the same `MegaDetector v5` model from the previous repository.
+
+
+### 📚 Expandable Repository:
+  As we move forward, our platform will welcome new models and pre-trained weights for camera traps and bioacoustic analysis. We're excited to host contributions from global researchers through a dedicated submission platform.
+
+
+### 📊 Datasets from LILA:
+  Pytorch-Wildlife will also incorporate the vast datasets hosted on LILA, making it a treasure trove for conservation research.
+
+
+### 🧰 Versatile Utilities:
+  Our set of utilities spans from visualization tools to task-specific utilities, many inherited from Megadetector.
+
+
+### 💻 User Interface Flexibility:
+  While we provide a foundational user interface, our platform is designed to inspire. We encourage researchers to craft and share their unique interfaces, and we'll list both existing and new UIs from other collaborators for the community's benefit.
+
+
+Let's shape the future of wildlife research, together! 🙌
+
+
+### 📈 Progress on core tasks
+
+<details>
+<summary> <font size="3"> ▪️ Packaging </font> </summary>
+
+- [ ] Animal detection fine-tuning<br>
+- [x] MegaDetectorV5 integration<br>
+- [ ] MegaDetectorV6 integration<br>
+- [x] User submitted weights<br>
+- [x] Animal classification fine-tuning<br>
+- [x] Amazon Rainforest classification<br>
+- [x] Amazon Opossum classification<br>
+- [ ] User submitted weights<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Utility Toolkit</font></summary>
+
+- [x] Visualization tools<br>
+- [x] MegaDetector utils<br>
+- [ ] User submitted utils<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Datasets</font></summary>
+
+- [ ] Animal Datasets<br>
+- [ ] LILA datasets<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Accessibility</font></summary>
+
+- [x] Basic user interface for demonstration<br>
+- [ ] UI Dev tools<br>
+- [ ] List of available UIs<br>
+</details><br>
+
+
+## 🖼️ Examples
+
+### Image detection using `MegaDetector v5`
+<img src="https://microsoft.github.io/CameraTraps/assets/animal_det_1.JPG" alt="animal_det_1" width="400"/><br>
+*Credits to Universidad de los Andes, Colombia.*
+
+### Image classification with `MegaDetector v5` and `AI4GAmazonRainforest`
+<img src="https://microsoft.github.io/CameraTraps/assets/animal_clas_1.png" alt="animal_clas_1" width="500"/><br>
+*Credits to Universidad de los Andes, Colombia.*
+
+### Opossum ID with `MegaDetector v5` and `AI4GOpossum`
+<img src="https://microsoft.github.io/CameraTraps/assets/opossum_det.png" alt="opossum_det" width="500"/><br>
+*Credits to the Agency for Regulation and Control of Biosecurity and Quarantine for Galápagos (ABG), Ecuador.*
+
+
+## 🤝 Contributing
+This project is open to your ideas and contributions. If you want to submit a pull request, we'll have some guidelines available soon.
+
+We have adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [us](zhongqimiao@microsoft.com) with any additional questions or comments.
+
+## License
+This repository is licensed with the [MIT license](https://github.com/Microsoft/dotnet/blob/main/LICENSE).
+
+
+## 👥 Existing Collaborators
+
+The extensive collaborative efforts of Megadetector have genuinely inspired us, and we deeply value its significant contributions to the community. As we continue to advance with Pytorch-Wildlife, our commitment to delivering technical support to our existing partners on MegaDetector remains the same.
+
+Here we list a few of the organizations that have used MegaDetector. We're only listing organizations who have given us permission to refer to them here or have posted publicly about their use of MegaDetector.
+
+<details>
+<summary><font size="3">👉 Full list of organizations</font></summary>
+
+(Newly Added) [TerrOïko](https://www.terroiko.fr/) ([OCAPI platform](https://www.terroiko.fr/ocapi))
+
+[Arizona Department of Environmental Quality](http://azdeq.gov/)
+
+[Blackbird Environmental](https://blackbirdenv.com/)
+
+[Camelot](https://camelotproject.org/)
+
+[Canadian Parks and Wilderness Society (CPAWS) Northern Alberta Chapter](https://cpawsnab.org/)
+
+[Conservation X Labs](https://conservationxlabs.com/)
+
+[Czech University of Life Sciences Prague](https://www.czu.cz/en)
+
+[EcoLogic Consultants Ltd.](https://www.consult-ecologic.com/)
+
+[Estación Biológica de Doñana](http://www.ebd.csic.es/inicio)
+
+[Idaho Department of Fish and Game](https://idfg.idaho.gov/)
+
+[Island Conservation](https://www.islandconservation.org/)
+
+[Myall Lakes Dingo Project](https://carnivorecoexistence.info/myall-lakes-dingo-project/)
+
+[Point No Point Treaty Council](https://pnptc.org/)
+
+[Ramat Hanadiv Nature Park](https://www.ramat-hanadiv.org.il/en/)
+
+[SPEA (Portuguese Society for the Study of Birds)](https://spea.pt/en/)
+
+[Synthetaic](https://www.synthetaic.com/)
+
+[Taronga Conservation Society](https://taronga.org.au/)
+
+[The Nature Conservancy in Wyoming](https://www.nature.org/en-us/about-us/where-we-work/united-states/wyoming/)
+
+[TrapTagger](https://wildeyeconservation.org/trap-tagger-about/)
+
+[Upper Yellowstone Watershed Group](https://www.upperyellowstone.org/)
+
+[Applied Conservation Macro Ecology Lab](http://www.acmelab.ca/), University of Victoria
+
+[Banff National Park Resource Conservation](https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation), Parks Canada(https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation)
+
+[Blumstein Lab](https://blumsteinlab.eeb.ucla.edu/), UCLA
+
+[Borderlands Research Institute](https://bri.sulross.edu/), Sul Ross State University
+
+[Capitol Reef National Park](https://www.nps.gov/care/index.htm) / Utah Valley University
+
+[Center for Biodiversity and Conservation](https://www.amnh.org/research/center-for-biodiversity-conservation), American Museum of Natural History
+
+[Centre for Ecosystem Science](https://www.unsw.edu.au/research/), UNSW Sydney
+
+[Cross-Cultural Ecology Lab](https://crossculturalecology.net/), Macquarie University
+
+[DC Cat Count](https://hub.dccatcount.org/), led by the Humane Rescue Alliance
+
+[Department of Fish and Wildlife Sciences](https://www.uidaho.edu/cnr/departments/fish-and-wildlife-sciences), University of Idaho
+
+[Department of Wildlife Ecology and Conservation](https://wec.ifas.ufl.edu/), University of Florida
+
+[Ecology and Conservation of Amazonian Vertebrates Research Group](https://www.researchgate.net/lab/Fernanda-Michalski-Lab-4), Federal University of Amapá
+
+[Gola Forest Programma](https://www.rspb.org.uk/our-work/conservation/projects/scientific-support-for-the-gola-forest-programme/), Royal Society for the Protection of Birds (RSPB)
+
+[Graeme Shannon's Research Group](https://wildliferesearch.co.uk/group-1), Bangor University
+
+[Hamaarag](https://hamaarag.org.il/), The Steinhardt Museum of Natural History, Tel Aviv University
+
+[Institut des Science de la Forêt Tempérée (ISFORT)](https://isfort.uqo.ca/), Université du Québec en Outaouais
+
+[Lab of Dr. Bilal Habib](https://bhlab.in/about), the Wildlife Institute of India
+
+[Mammal Spatial Ecology and Conservation Lab](https://labs.wsu.edu/dthornton/), Washington State University
+
+[McLoughlin Lab in Population Ecology](http://mcloughlinlab.ca/lab/), University of Saskatchewan
+
+[National Wildlife Refuge System, Southwest Region](https://www.fws.gov/about/region/southwest), U.S. Fish & Wildlife Service
+
+[Northern Great Plains Program](https://nationalzoo.si.edu/news/restoring-americas-prairie), Smithsonian
+
+[Quantitative Ecology Lab](https://depts.washington.edu/sefsqel/), University of Washington
+
+[Santa Monica Mountains Recreation Area](https://www.nps.gov/samo/index.htm), National Park Service
+
+[Seattle Urban Carnivore Project](https://www.zoo.org/seattlecarnivores), Woodland Park Zoo
+
+[Serra dos Órgãos National Park](https://www.icmbio.gov.br/parnaserradosorgaos/), ICMBio
+
+[Snapshot USA](https://emammal.si.edu/snapshot-usa), Smithsonian
+
+[Wildlife Coexistence Lab](https://wildlife.forestry.ubc.ca/), University of British Columbia
+
+[Wildlife Research](https://www.dfw.state.or.us/wildlife/research/index.asp), Oregon Department of Fish and Wildlife
+
+[Wildlife Division](https://www.michigan.gov/dnr/about/contact/wildlife), Michigan Department of Natural Resources
+
+Department of Ecology, TU Berlin
+
+Ghost Cat Analytics
+
+Protected Areas Unit, Canadian Wildlife Service
+
+[School of Natural Sciences](https://www.utas.edu.au/natural-sciences), University of Tasmania [(story)](https://www.utas.edu.au/about/news-and-stories/articles/2022/1204-innovative-camera-network-keeps-close-eye-on-tassie-wildlife)
+
+[Kenai National Wildlife Refuge](https://www.fws.gov/refuge/kenai), U.S. Fish & Wildlife Service [(story)](https://www.peninsulaclarion.com/sports/refuge-notebook-new-technology-increases-efficiency-of-refuge-cameras/)
+
+[Australian Wildlife Conservancy](https://www.australianwildlife.org/) [(blog](https://www.australianwildlife.org/cutting-edge-technology-delivering-efficiency-gains-in-conservation/), [blog)](https://www.australianwildlife.org/efficiency-gains-at-the-cutting-edge-of-technology/)
+
+[Felidae Conservation Fund](https://felidaefund.org/) [(WildePod platform)](https://wildepod.org/) [(blog post)](https://abhaykashyap.com/blog/ai-powered-camera-trap-image-annotation-system/)
+
+[Alberta Biodiversity Monitoring Institute (ABMI)](https://www.abmi.ca/home.html) [(WildTrax platform)](https://www.wildtrax.ca/) [(blog post)](https://wildcams.ca/blog/the-abmi-visits-the-zoo/)
+
+[Shan Shui Conservation Center](http://en.shanshui.org/) [(blog post)](https://mp.weixin.qq.com/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs) [(translated blog post)](https://mp-weixin-qq-com.translate.goog/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs&_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp)
+
+[Irvine Ranch Conservancy](http://www.irconservancy.org/) [(story)](https://www.ocregister.com/2022/03/30/ai-software-is-helping-researchers-focus-on-learning-about-ocs-wild-animals/)
+
+[Wildlife Protection Solutions](https://wildlifeprotectionsolutions.org/) [(story](https://customers.microsoft.com/en-us/story/1384184517929343083-wildlife-protection-solutions-nonprofit-ai-for-earth), [story)](https://www.enterpriseai.news/2023/02/20/ai-helps-wildlife-protection-solutions-safeguard-endangered-species/)
+
+[Road Ecology Center](https://roadecology.ucdavis.edu/), University of California, Davis [(Wildlife Observer Network platform)](https://wildlifeobserver.net/)
+
+[The Nature Conservancy in California](https://www.nature.org/en-us/about-us/where-we-work/united-states/california/) [(Animl platform)](https://github.com/tnc-ca-geo/animl-frontend)
+
+[San Diego Zoo Wildlife Alliance](https://science.sandiegozoo.org/) [(Animl R package)](https://github.com/conservationtechlab/animl)
+
+</details><br>
+
+
+>[!IMPORTANT]
+>If you would like to be added to this list or have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our Discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
+
```

#### html2text {}

```diff
@@ -1,41 +1,27 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.8 Summary: a PyTorch
-Collaborative Deep Learning Framework for Conservation. Home-page: https://
-github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
-Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
-Keywords:
-pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy Requires-Dist: torch==1.10.1
-Requires-Dist: torchvision==0.11.2 Requires-Dist: torchaudio==0.10.1 Requires-
-Dist: tqdm==4.66.1 Requires-Dist: Pillow==10.1.0 Requires-Dist:
-supervision==0.16.0 Requires-Dist: gradio==4.8.0 Requires-Dist: ultralytics-
-yolov5 Requires-Dist: chardet ![image](https://microsoft.github.io/CameraTraps/
-assets/Pytorch_Banner_transparentbk.png)
+![image](https://microsoft.github.io/CameraTraps/assets/
+Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
 _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
  _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
    _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
                    _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
-## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
-Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. - [x] Added a Docker Image for ease of
-installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
-model sizes for both optimized performance and low-budget devices like camera
-systems. - [ ] Direct Timelapse format outputs for both detection and
+## â Update highlights (Version 1.0.2.9) - [x] Added Timelapse compatibility!
+Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://
+github.com/microsoft/CameraTraps/tree/main/demo). - [x] Added Google Colab
+demos. - [x] Added Snapshot Serengeti classification model into the model zoo.
+- [x] Added Classification fine-tuning module. - [x] Added a Docker Image for
+ease of installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with
+multiple model sizes for both optimized performance and low-budget devices like
+camera systems. - [ ] Direct Timelapse format outputs for both detection and
 classification. - [ ] A detection model fine-tuning module to fine-tune your
 own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
 training/validation data. - [ ] More pretrained detection and classification
 models to expand the current model zoo. To check the full version of the
 roadmap with completed tasks and long term goals, please click [here!]
 (roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
 create a harmonious space where conservation scientists from all over the globe
```

### Comparing `PytorchWildlife-1.0.2.8/PW_FT_classification/main.py` & `PytorchWildlife-1.0.2.9/PW_FT_classification/main.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# %%
-# Importing libraries
-import os
-import yaml
-import typer
-from munch import Munch
-# %%
-import torch
-import pytorch_lightning as pl
-from pytorch_lightning.callbacks import ModelCheckpoint
-from pytorch_lightning.callbacks import LearningRateMonitor
-from pytorch_lightning.loggers import CSVLogger, CometLogger, TensorBoardLogger, WandbLogger
-# %%
-from src import algorithms
-from src import datasets
-# %%
-from src.utils import batch_detection_cropping
-from src.utils import data_splitting
-#app = typer.Typer()
-# %%
-#@app.command()
-def main(
-        config:str='./configs/Raw/Crop_res50_plain_082723.yaml',
-        project:str='Custom-classification',
-        gpus:str='0', 
-        logger_type:str='csv',
-        evaluate:str=None,
-        np_threads:str='32',
-        session:int=0,
-        seed:int=0,
-        dev:bool=False,
-        val:bool=False,
-        predict:bool=False,
-        predict_root:str=""
-    ):
-    """
-    Main function for training or evaluating a ResNet-50 model using PyTorch Lightning.
-    It loads configurations, initializes the model, logger, and other components based on provided arguments.
-
-    Args:
-        config (str): Path to the configuration file.
-        project (str): Name of the project for logging.
-        gpus (str): Comma-separated GPU ids for training.
-        logger_type (str): Type of logger to use (wandb, comet, tensorboard, csv).
-        evaluate (str): Path to the model checkpoint for evaluation.
-        np_threads (str): Number of numpy threads to use.
-        session (int): Session number for logging purposes.
-        seed (int): Random seed for reproducibility.
-        dev (bool): Development mode flag.
-        val (bool): Validation mode flag.
-        predict (bool): Prediction mode flag.
-        predict_root (str): Root directory for prediction outputs.
-    """
-
-    # GPU configuration: set up GPUs based on availability and user specification
-    gpus = gpus if torch.cuda.is_available() else None
-    gpus = [int(i) for i in gpus.split(',')]
-
-    # Environment variable setup for numpy multi-threading
-    os.environ["OMP_NUM_THREADS"] = str(np_threads)
-    os.environ["OPENBLAS_NUM_THREADS"] = str(np_threads)
-    os.environ["MKL_NUM_THREADS"] = str(np_threads)
-    os.environ["VECLIB_MAXIMUM_THREADS"] = str(np_threads)
-    os.environ["NUMEXPR_NUM_THREADS"] = str(np_threads)
-    # Load and set configurations from the YAML file
-    with open(config) as f:
-        conf = Munch(yaml.load(f, Loader=yaml.FullLoader))
-    conf.evaluate = evaluate
-    conf.val = val
-    conf.predict = predict
-    conf.predict_root = predict_root
-
-    # Set a global seed for reproducibility
-    pl.seed_everything(seed)
-
-    
-    # If the annotation directory does not have a data split, split the data first
-    if conf.split_data:
-        # Replace annotation dir from config with the directory containing the split files
-        conf.annotation_dir = os.path.dirname(conf.split_path)
-        # Split the data according to the split type
-        if conf.split_type == 'location':
-            data_splitting.split_by_location(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
-        elif conf.split_type == 'sequence':
-            data_splitting.split_by_seq(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
-        elif conf.split_type == 'random':
-            data_splitting.create_splits(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
-        else:
-            raise ValueError('Invalid split type: {}. Available options: random, location, sequence.'.format(conf.split_type))
-        
-    # Get the path to the annotation files
-    train_annotations = os.path.join(conf.dataset_root, 'train_annotations.csv')
-    test_annotations = os.path.join(conf.dataset_root, 'test_annotations.csv')
-    val_annotations = os.path.join(conf.dataset_root, 'val_annotations.csv')
-    # Split training data
-
-    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), train_annotations)
-    # Split validation and test data
-    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), val_annotations)
-    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), test_annotations)
-
-
-    # Dataset and algorithm loading based on the configuration
-    dataset = datasets.__dict__[conf.dataset_name](conf=conf)
-    learner = algorithms.__dict__[conf.algorithm](conf=conf,
-                            train_class_counts=dataset.train_class_counts, 
-                            id_to_labels=dataset.id_to_labels)
-
-    # Logger setup based on the specified logger type
-    log_folder = 'log_dev' if dev else 'log'
-    logger = None
-    if logger_type == 'csv':
-        logger = CSVLogger(
-            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
-            prefix=project,
-            name='{}_{}'.format(conf.algorithm, conf.conf_id),
-            version=session
-        )
-    elif logger_type == 'tensorboard':
-        logger = TensorBoardLogger(
-            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
-            prefix=project,
-            name='{}_{}'.format(conf.algorithm, conf.conf_id),
-            version=session
-        )
-    elif logger_type == 'comet':
-        logger = CometLogger(
-            api_key=os.environ.get("COMET_API_KEY"),
-            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
-            project_name=project, 
-            experiment_name='{}_{}_{}'.format(conf.algorithm, conf.conf_id, session),
-        )
-    elif logger_type == 'wandb':
-        logger = WandbLogger(
-            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
-            project=project,  
-            name='{}_{}_{}'.format(conf.algorithm, conf.conf_id, session),
-        )
-
-    # Callbacks for model checkpointing and learning rate monitoring
-    weights_folder = 'weights_dev' if dev else 'weights'
-    checkpoint_callback = ModelCheckpoint(
-        monitor='valid_mac_acc', mode='max', dirpath='./{}/{}/{}'.format(weights_folder, conf.log_dir, conf.algorithm),
-        save_top_k=1, filename='{}-{}'.format(conf.conf_id, session) + '-{epoch:02d}-{valid_mac_acc:.2f}', verbose=True
-    )
-
-    lr_monitor = LearningRateMonitor(logging_interval='step')
-
-    # Trainer configuration in PyTorch Lightning
-    trainer = pl.Trainer(
-        max_epochs=conf.num_epochs,
-        check_val_every_n_epoch=1, 
-        log_every_n_steps = conf.log_interval, 
-        accelerator='gpu',
-        devices=gpus,
-        logger=None if evaluate is not None else logger,
-        callbacks=[lr_monitor, checkpoint_callback],
-        strategy='ddp',
-        num_sanity_val_steps=0,
-        profiler=None
-    )
-    # Training, validation, or evaluation execution based on the mode
-    if evaluate is not None:
-        if val:
-            trainer.validate(learner, dataloaders=[dataset.val_dataloader()], ckpt_path=evaluate)
-        elif predict:
-            trainer.predict(learner, dataloaders=[dataset.predict_dataloader()], ckpt_path=evaluate)
-        else:
-            trainer.test(learner, dataloaders=[dataset.test_dataloader()], ckpt_path=evaluate)
-    else:
-        trainer.fit(learner, datamodule=dataset)
-# %%
-if __name__ == '__main__':
-    main()
-
-
-
-# %%
+# %%
+# Importing libraries
+import os
+import yaml
+import typer
+from munch import Munch
+# %%
+import torch
+import pytorch_lightning as pl
+from pytorch_lightning.callbacks import ModelCheckpoint
+from pytorch_lightning.callbacks import LearningRateMonitor
+from pytorch_lightning.loggers import CSVLogger, CometLogger, TensorBoardLogger, WandbLogger
+# %%
+from src import algorithms
+from src import datasets
+# %%
+from src.utils import batch_detection_cropping
+from src.utils import data_splitting
+#app = typer.Typer()
+# %%
+#@app.command()
+def main(
+        config:str='./configs/Raw/Crop_res50_plain_082723.yaml',
+        project:str='Custom-classification',
+        gpus:str='0', 
+        logger_type:str='csv',
+        evaluate:str=None,
+        np_threads:str='32',
+        session:int=0,
+        seed:int=0,
+        dev:bool=False,
+        val:bool=False,
+        predict:bool=False,
+        predict_root:str=""
+    ):
+    """
+    Main function for training or evaluating a ResNet-50 model using PyTorch Lightning.
+    It loads configurations, initializes the model, logger, and other components based on provided arguments.
+
+    Args:
+        config (str): Path to the configuration file.
+        project (str): Name of the project for logging.
+        gpus (str): Comma-separated GPU ids for training.
+        logger_type (str): Type of logger to use (wandb, comet, tensorboard, csv).
+        evaluate (str): Path to the model checkpoint for evaluation.
+        np_threads (str): Number of numpy threads to use.
+        session (int): Session number for logging purposes.
+        seed (int): Random seed for reproducibility.
+        dev (bool): Development mode flag.
+        val (bool): Validation mode flag.
+        predict (bool): Prediction mode flag.
+        predict_root (str): Root directory for prediction outputs.
+    """
+
+    # GPU configuration: set up GPUs based on availability and user specification
+    gpus = gpus if torch.cuda.is_available() else None
+    gpus = [int(i) for i in gpus.split(',')]
+
+    # Environment variable setup for numpy multi-threading
+    os.environ["OMP_NUM_THREADS"] = str(np_threads)
+    os.environ["OPENBLAS_NUM_THREADS"] = str(np_threads)
+    os.environ["MKL_NUM_THREADS"] = str(np_threads)
+    os.environ["VECLIB_MAXIMUM_THREADS"] = str(np_threads)
+    os.environ["NUMEXPR_NUM_THREADS"] = str(np_threads)
+    # Load and set configurations from the YAML file
+    with open(config) as f:
+        conf = Munch(yaml.load(f, Loader=yaml.FullLoader))
+    conf.evaluate = evaluate
+    conf.val = val
+    conf.predict = predict
+    conf.predict_root = predict_root
+
+    # Set a global seed for reproducibility
+    pl.seed_everything(seed)
+
+    
+    # If the annotation directory does not have a data split, split the data first
+    if conf.split_data:
+        # Replace annotation dir from config with the directory containing the split files
+        conf.annotation_dir = os.path.dirname(conf.split_path)
+        # Split the data according to the split type
+        if conf.split_type == 'location':
+            data_splitting.split_by_location(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
+        elif conf.split_type == 'sequence':
+            data_splitting.split_by_seq(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
+        elif conf.split_type == 'random':
+            data_splitting.create_splits(conf.split_path, conf.annotation_dir, conf.test_size, conf.val_size)
+        else:
+            raise ValueError('Invalid split type: {}. Available options: random, location, sequence.'.format(conf.split_type))
+        
+    # Get the path to the annotation files
+    train_annotations = os.path.join(conf.dataset_root, 'train_annotations.csv')
+    test_annotations = os.path.join(conf.dataset_root, 'test_annotations.csv')
+    val_annotations = os.path.join(conf.dataset_root, 'val_annotations.csv')
+    # Split training data
+
+    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), train_annotations)
+    # Split validation and test data
+    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), val_annotations)
+    batch_detection_cropping.batch_detection_cropping(conf.dataset_root, os.path.join(conf.dataset_root, "cropped_resized"), test_annotations)
+
+
+    # Dataset and algorithm loading based on the configuration
+    dataset = datasets.__dict__[conf.dataset_name](conf=conf)
+    learner = algorithms.__dict__[conf.algorithm](conf=conf,
+                            train_class_counts=dataset.train_class_counts, 
+                            id_to_labels=dataset.id_to_labels)
+
+    # Logger setup based on the specified logger type
+    log_folder = 'log_dev' if dev else 'log'
+    logger = None
+    if logger_type == 'csv':
+        logger = CSVLogger(
+            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
+            prefix=project,
+            name='{}_{}'.format(conf.algorithm, conf.conf_id),
+            version=session
+        )
+    elif logger_type == 'tensorboard':
+        logger = TensorBoardLogger(
+            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
+            prefix=project,
+            name='{}_{}'.format(conf.algorithm, conf.conf_id),
+            version=session
+        )
+    elif logger_type == 'comet':
+        logger = CometLogger(
+            api_key=os.environ.get("COMET_API_KEY"),
+            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
+            project_name=project, 
+            experiment_name='{}_{}_{}'.format(conf.algorithm, conf.conf_id, session),
+        )
+    elif logger_type == 'wandb':
+        logger = WandbLogger(
+            save_dir='./{}/{}/{}'.format(log_folder, conf.log_dir, conf.algorithm),
+            project=project,  
+            name='{}_{}_{}'.format(conf.algorithm, conf.conf_id, session),
+        )
+
+    # Callbacks for model checkpointing and learning rate monitoring
+    weights_folder = 'weights_dev' if dev else 'weights'
+    checkpoint_callback = ModelCheckpoint(
+        monitor='valid_mac_acc', mode='max', dirpath='./{}/{}/{}'.format(weights_folder, conf.log_dir, conf.algorithm),
+        save_top_k=1, filename='{}-{}'.format(conf.conf_id, session) + '-{epoch:02d}-{valid_mac_acc:.2f}', verbose=True
+    )
+
+    lr_monitor = LearningRateMonitor(logging_interval='step')
+
+    # Trainer configuration in PyTorch Lightning
+    trainer = pl.Trainer(
+        max_epochs=conf.num_epochs,
+        check_val_every_n_epoch=1, 
+        log_every_n_steps = conf.log_interval, 
+        accelerator='gpu',
+        devices=gpus,
+        logger=None if evaluate is not None else logger,
+        callbacks=[lr_monitor, checkpoint_callback],
+        strategy='ddp',
+        num_sanity_val_steps=0,
+        profiler=None
+    )
+    # Training, validation, or evaluation execution based on the mode
+    if evaluate is not None:
+        if val:
+            trainer.validate(learner, dataloaders=[dataset.val_dataloader()], ckpt_path=evaluate)
+        elif predict:
+            trainer.predict(learner, dataloaders=[dataset.predict_dataloader()], ckpt_path=evaluate)
+        else:
+            trainer.test(learner, dataloaders=[dataset.test_dataloader()], ckpt_path=evaluate)
+    else:
+        trainer.fit(learner, datamodule=dataset)
+# %%
+if __name__ == '__main__':
+    main()
+
+
+
+# %%
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/data/datasets.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/data/datasets.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-import os
-from glob import glob
-from PIL import Image
-import numpy as np
-import supervision as sv
-import torch
-from torch.utils.data import Dataset
-
-# Making the DetectionImageFolder class available for import from this module
-__all__ = [
-    "DetectionImageFolder",
-    ]
-
-
-class DetectionImageFolder(Dataset):
-    """
-    A PyTorch Dataset for loading images from a specified directory.
-    Each item in the dataset is a tuple containing the image data, 
-    the image's path, and the original size of the image.
-    """
-
-    def __init__(self, image_dir, transform=None, extension="JPG"):
-        """
-        Initializes the dataset.
-
-        Parameters:
-            image_dir (str): Path to the directory containing the images.
-            transform (callable, optional): Optional transform to be applied on the image.
-        """
-        self.image_dir = image_dir
-        # Listing and sorting all image files in the specified directory
-        self.images = sorted(glob(os.path.join(self.image_dir, "**/*." + extension),
-                                  recursive=True))
-        self.transform = transform
-
-    def __getitem__(self, idx):
-        """
-        Retrieves an image from the dataset.
-
-        Parameters:
-            idx (int): Index of the image to retrieve.
-
-        Returns:
-            tuple: Contains the image data, the image's path, and its original size.
-        """
-        # Get image filename and path
-        img_path = self.images[idx]
-
-        # Load and convert image to RGB
-        img = Image.open(img_path).convert("RGB")
-        img_size_ori = img.size[::-1]
-        
-        # Apply transformation if specified
-        if self.transform:
-            img = self.transform(img)
-
-        return img, img_path, torch.tensor(img_size_ori)
-    
-    def __len__(self):
-        """
-        Returns the total number of images in the dataset.
-
-        Returns:
-            int: Total number of images.
-        """
-        return len(self.images)
-
-
-class DetectionCrops(Dataset):
-
-    def __init__(self, detection_results, transform=None, path_head=None, animal_cls_id=0):
-
-        self.detection_results = detection_results
-        self.transform = transform
-        self.path_head = path_head
-        self.animal_cls_id = animal_cls_id # This determins which detection class id represents animals.
-        self.img_ids = []
-        self.xyxys = []
-
-        self.load_detection_results()
-
-    def load_detection_results(self):
-        for det in self.detection_results:
-            for xyxy, det_id in zip(det["detections"].xyxy, det["detections"].class_id):
-                # Only run recognition on animal detections
-                if det_id == self.animal_cls_id:
-                    self.img_ids.append(det["img_id"])
-                    self.xyxys.append(xyxy)
-
-    def __getitem__(self, idx):
-        """
-        Retrieves an image from the dataset.
-
-        Parameters:
-            idx (int): Index of the image to retrieve.
-
-        Returns:
-            tuple: Contains the image data and the image's path.
-        """
-
-        # Get image path and corresponding bbox xyxy for cropping
-        img_id = self.img_ids[idx]
-        xyxy = self.xyxys[idx]
-
-        img_path = os.path.join(self.path_head, img_id) if self.path_head else img_id
-        
-        # Load and crop image with supervision
-        img = sv.crop_image(np.array(Image.open(img_path).convert("RGB")),
-                            xyxy=xyxy)
-        
-        # Apply transformation if specified
-        if self.transform:
-            img = self.transform(Image.fromarray(img))
-
-        return img, img_path
-
-    def __len__(self):
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+import os
+from glob import glob
+from PIL import Image
+import numpy as np
+import supervision as sv
+import torch
+from torch.utils.data import Dataset
+
+# Making the DetectionImageFolder class available for import from this module
+__all__ = [
+    "DetectionImageFolder",
+    ]
+
+
+class DetectionImageFolder(Dataset):
+    """
+    A PyTorch Dataset for loading images from a specified directory.
+    Each item in the dataset is a tuple containing the image data, 
+    the image's path, and the original size of the image.
+    """
+
+    def __init__(self, image_dir, transform=None, extension="JPG"):
+        """
+        Initializes the dataset.
+
+        Parameters:
+            image_dir (str): Path to the directory containing the images.
+            transform (callable, optional): Optional transform to be applied on the image.
+        """
+        self.image_dir = image_dir
+        # Listing and sorting all image files in the specified directory
+        self.images = sorted(glob(os.path.join(self.image_dir, "**/*." + extension),
+                                  recursive=True))
+        self.transform = transform
+
+    def __getitem__(self, idx):
+        """
+        Retrieves an image from the dataset.
+
+        Parameters:
+            idx (int): Index of the image to retrieve.
+
+        Returns:
+            tuple: Contains the image data, the image's path, and its original size.
+        """
+        # Get image filename and path
+        img_path = self.images[idx]
+
+        # Load and convert image to RGB
+        img = Image.open(img_path).convert("RGB")
+        img_size_ori = img.size[::-1]
+        
+        # Apply transformation if specified
+        if self.transform:
+            img = self.transform(img)
+
+        return img, img_path, torch.tensor(img_size_ori)
+    
+    def __len__(self):
+        """
+        Returns the total number of images in the dataset.
+
+        Returns:
+            int: Total number of images.
+        """
+        return len(self.images)
+
+
+class DetectionCrops(Dataset):
+
+    def __init__(self, detection_results, transform=None, path_head=None, animal_cls_id=0):
+
+        self.detection_results = detection_results
+        self.transform = transform
+        self.path_head = path_head
+        self.animal_cls_id = animal_cls_id # This determins which detection class id represents animals.
+        self.img_ids = []
+        self.xyxys = []
+
+        self.load_detection_results()
+
+    def load_detection_results(self):
+        for det in self.detection_results:
+            for xyxy, det_id in zip(det["detections"].xyxy, det["detections"].class_id):
+                # Only run recognition on animal detections
+                if det_id == self.animal_cls_id:
+                    self.img_ids.append(det["img_id"])
+                    self.xyxys.append(xyxy)
+
+    def __getitem__(self, idx):
+        """
+        Retrieves an image from the dataset.
+
+        Parameters:
+            idx (int): Index of the image to retrieve.
+
+        Returns:
+            tuple: Contains the image data and the image's path.
+        """
+
+        # Get image path and corresponding bbox xyxy for cropping
+        img_id = self.img_ids[idx]
+        xyxy = self.xyxys[idx]
+
+        img_path = os.path.join(self.path_head, img_id) if self.path_head else img_id
+        
+        # Load and crop image with supervision
+        img = sv.crop_image(np.array(Image.open(img_path).convert("RGB")),
+                            xyxy=xyxy)
+        
+        # Apply transformation if specified
+        if self.transform:
+            img = self.transform(Image.fromarray(img))
+
+        return img, img_path
+
+    def __len__(self):
         return len(self.img_ids)
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/data/transforms.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/data/transforms.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-import numpy as np
-import torch
-from torchvision import transforms
-#from yolov5.utils.augmentations import letterbox
-import torchvision.transforms as T
-import torch.nn.functional as F
-from PIL import Image
-
-# Making the provided classes available for import from this module
-__all__ = [
-    "MegaDetector_v5_Transform",
-    "Classification_Inference_Transform"
-]
-
-
-def letterbox(im, new_shape=(640, 640), color=(114, 114, 114), auto=False, scaleFill=False, scaleup=True, stride=32):
-    """
-    Resize and pad an image to a desired shape while keeping the aspect ratio unchanged. 
-
-    This function is commonly used in object detection tasks to prepare images for models like YOLOv5. 
-    It resizes the image to fit into the new shape with the correct aspect ratio and then pads the rest.
-
-    Parameters:
-    im (PIL.Image.Image or torch.Tensor): The input image. It can be a PIL image or a PyTorch tensor.
-    new_shape (tuple, optional): The target size of the image, in the form (height, width). Defaults to (640, 640).
-    color (tuple, optional): The color used for padding. Defaults to (114, 114, 114).
-    auto (bool, optional): Adjust padding to ensure the padded image is a multiple of stride. Defaults to True.
-    scaleFill (bool, optional): If True, scales the image to fill the new shape, ignoring the aspect ratio. Defaults to False.
-    scaleup (bool, optional): Allow the function to scale up the image. Defaults to True.
-    stride (int, optional): The stride used in the model. The padding is adjusted to be a multiple of this stride. Defaults to 32.
-
-    Returns:
-    tuple: A tuple containing:
-        - The transformed image as a torch.Tensor.
-        - The scale ratios as a tuple (width_ratio, height_ratio).
-        - The padding applied as a tuple (width_padding, height_padding).
-    """
-
-    # Convert PIL Image to Torch Tensor
-
-    if isinstance(im, Image.Image):
-        im = T.ToTensor()(im)
-
-    # Original shape
-    shape = im.shape[1:]  # shape = [height, width]
-
-    # New shape
-    if isinstance(new_shape, int):
-        new_shape = (new_shape, new_shape)
-
-    # Scale ratio (new / old) and compute padding
-    r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
-    if not scaleup:
-        r = min(r, 1.0)
-
-    new_unpad = (int(round(shape[1] * r)), int(round(shape[0] * r)))
-    dw, dh = new_shape[1] - new_unpad[0], new_shape[0] - new_unpad[1]
-
-    if auto:
-        dw, dh = dw % stride, dh % stride
-    elif scaleFill:
-        dw, dh = 0, 0
-        new_unpad = new_shape
-        r = new_shape[1] / shape[1], new_shape[0] / shape[0]
-
-    dw /= 2
-    dh /= 2
-   
-    # Resize image
-    if shape[::-1] != new_unpad:
-        resize_transform = T.Resize(new_unpad[::-1], interpolation=T.InterpolationMode.BILINEAR,
-                                    antialias=False)
-        im = resize_transform(im)
-
-    # Pad image
-    padding = (int(round(dw - 0.1)), int(round(dw + 0.1)), int(round(dh + 0.1)), int(round(dh - 0.1)))
-    im = F.pad(im*255.0, padding, value=114)/255.0
-
-    return im
-
-class MegaDetector_v5_Transform:
-    """
-    A transformation class to preprocess images for the MegaDetector v5 model.
-    This includes resizing, transposing, and normalization operations.
-    This is a required transformation for the YoloV5 model.
-
-    """
-
-    def __init__(self, target_size=1280, stride=32):
-        """
-        Initializes the transform.
-
-        Args:
-            target_size (int): Desired size for the image's longest side after resizing.
-            stride (int): Stride value for resizing.
-        """
-        self.target_size = target_size
-        self.stride = stride
-
-    def __call__(self, np_img):
-        """
-        Applies the transformation on the provided image.
-
-        Args:
-            np_img (np.ndarray): Input image as a numpy array or PIL Image.
-
-        Returns:
-            torch.Tensor: Transformed image.
-        """
-        # Convert the image to a PyTorch tensor and normalize it
-        if isinstance(np_img, np.ndarray):
-            np_img = np_img.transpose((2, 0, 1))
-            np_img = np.ascontiguousarray(np_img)
-            np_img = torch.from_numpy(np_img).float()
-            np_img /= 255.0
-
-        # Resize and pad the image using a customized letterbox function. 
-        img = letterbox(np_img, new_shape=self.target_size, stride=self.stride, auto=False)
-
-        return img
-
-class Classification_Inference_Transform:
-    """
-    A transformation class to preprocess images for classification inference.
-    This includes resizing, normalization, and conversion to a tensor.
-    """
-    # Normalization constants
-    mean = [0.485, 0.456, 0.406]
-    std = [0.229, 0.224, 0.225]
-
-    def __init__(self, target_size=224):
-        """
-        Initializes the transform.
-
-        Args:
-            target_size (int): Desired size for the height and width after resizing.
-        """
-        # Define the sequence of transformations
-        self.trans = transforms.Compose([
-            transforms.Resize((target_size, target_size)),
-            transforms.ToTensor(),
-            transforms.Normalize(self.mean, self.std)
-        ])
-
-    def __call__(self, img):
-        """
-        Applies the transformation on the provided image.
-
-        Args:
-            img (PIL.Image.Image): Input image in PIL format.
-
-        Returns:
-            torch.Tensor: Transformed image.
-        """
-        img = self.trans(img)
-        return img
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+import numpy as np
+import torch
+from torchvision import transforms
+#from yolov5.utils.augmentations import letterbox
+import torchvision.transforms as T
+import torch.nn.functional as F
+from PIL import Image
+
+# Making the provided classes available for import from this module
+__all__ = [
+    "MegaDetector_v5_Transform",
+    "Classification_Inference_Transform"
+]
+
+
+def letterbox(im, new_shape=(640, 640), color=(114, 114, 114), auto=False, scaleFill=False, scaleup=True, stride=32):
+    """
+    Resize and pad an image to a desired shape while keeping the aspect ratio unchanged. 
+
+    This function is commonly used in object detection tasks to prepare images for models like YOLOv5. 
+    It resizes the image to fit into the new shape with the correct aspect ratio and then pads the rest.
+
+    Parameters:
+    im (PIL.Image.Image or torch.Tensor): The input image. It can be a PIL image or a PyTorch tensor.
+    new_shape (tuple, optional): The target size of the image, in the form (height, width). Defaults to (640, 640).
+    color (tuple, optional): The color used for padding. Defaults to (114, 114, 114).
+    auto (bool, optional): Adjust padding to ensure the padded image is a multiple of stride. Defaults to True.
+    scaleFill (bool, optional): If True, scales the image to fill the new shape, ignoring the aspect ratio. Defaults to False.
+    scaleup (bool, optional): Allow the function to scale up the image. Defaults to True.
+    stride (int, optional): The stride used in the model. The padding is adjusted to be a multiple of this stride. Defaults to 32.
+
+    Returns:
+    tuple: A tuple containing:
+        - The transformed image as a torch.Tensor.
+        - The scale ratios as a tuple (width_ratio, height_ratio).
+        - The padding applied as a tuple (width_padding, height_padding).
+    """
+
+    # Convert PIL Image to Torch Tensor
+
+    if isinstance(im, Image.Image):
+        im = T.ToTensor()(im)
+
+    # Original shape
+    shape = im.shape[1:]  # shape = [height, width]
+
+    # New shape
+    if isinstance(new_shape, int):
+        new_shape = (new_shape, new_shape)
+
+    # Scale ratio (new / old) and compute padding
+    r = min(new_shape[0] / shape[0], new_shape[1] / shape[1])
+    if not scaleup:
+        r = min(r, 1.0)
+
+    new_unpad = (int(round(shape[1] * r)), int(round(shape[0] * r)))
+    dw, dh = new_shape[1] - new_unpad[0], new_shape[0] - new_unpad[1]
+
+    if auto:
+        dw, dh = dw % stride, dh % stride
+    elif scaleFill:
+        dw, dh = 0, 0
+        new_unpad = new_shape
+        r = new_shape[1] / shape[1], new_shape[0] / shape[0]
+
+    dw /= 2
+    dh /= 2
+   
+    # Resize image
+    if shape[::-1] != new_unpad:
+        resize_transform = T.Resize(new_unpad[::-1], interpolation=T.InterpolationMode.BILINEAR,
+                                    antialias=False)
+        im = resize_transform(im)
+
+    # Pad image
+    padding = (int(round(dw - 0.1)), int(round(dw + 0.1)), int(round(dh + 0.1)), int(round(dh - 0.1)))
+    im = F.pad(im*255.0, padding, value=114)/255.0
+
+    return im
+
+class MegaDetector_v5_Transform:
+    """
+    A transformation class to preprocess images for the MegaDetector v5 model.
+    This includes resizing, transposing, and normalization operations.
+    This is a required transformation for the YoloV5 model.
+
+    """
+
+    def __init__(self, target_size=1280, stride=32):
+        """
+        Initializes the transform.
+
+        Args:
+            target_size (int): Desired size for the image's longest side after resizing.
+            stride (int): Stride value for resizing.
+        """
+        self.target_size = target_size
+        self.stride = stride
+
+    def __call__(self, np_img):
+        """
+        Applies the transformation on the provided image.
+
+        Args:
+            np_img (np.ndarray): Input image as a numpy array or PIL Image.
+
+        Returns:
+            torch.Tensor: Transformed image.
+        """
+        # Convert the image to a PyTorch tensor and normalize it
+        if isinstance(np_img, np.ndarray):
+            np_img = np_img.transpose((2, 0, 1))
+            np_img = np.ascontiguousarray(np_img)
+            np_img = torch.from_numpy(np_img).float()
+            np_img /= 255.0
+
+        # Resize and pad the image using a customized letterbox function. 
+        img = letterbox(np_img, new_shape=self.target_size, stride=self.stride, auto=False)
+
+        return img
+
+class Classification_Inference_Transform:
+    """
+    A transformation class to preprocess images for classification inference.
+    This includes resizing, normalization, and conversion to a tensor.
+    """
+    # Normalization constants
+    mean = [0.485, 0.456, 0.406]
+    std = [0.229, 0.224, 0.225]
+
+    def __init__(self, target_size=224):
+        """
+        Initializes the transform.
+
+        Args:
+            target_size (int): Desired size for the height and width after resizing.
+        """
+        # Define the sequence of transformations
+        self.trans = transforms.Compose([
+            transforms.Resize((target_size, target_size)),
+            transforms.ToTensor(),
+            transforms.Normalize(self.mean, self.std)
+        ])
+
+    def __call__(self, img):
+        """
+        Applies the transformation on the provided image.
+
+        Args:
+            img (PIL.Image.Image): Input image in PIL format.
+
+        Returns:
+            torch.Tensor: Transformed image.
+        """
+        img = self.trans(img)
+        return img
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/base_classifier.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/base_classifier.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-import numpy as np
-import torch
-import torch.nn as nn
-from torchvision.models.resnet import BasicBlock, Bottleneck, ResNet
-from torch.hub import load_state_dict_from_url
-from tqdm import tqdm
-from collections import OrderedDict
-
-# Making the PlainResNetInference class available for import from this module
-__all__ = ["PlainResNetInference"]
-
-
-class ResNetBackbone(ResNet):
-    """
-    Custom ResNet Backbone that extracts features from input images.
-    """
-    def _forward_impl(self, x):
-        # Following the ResNet structure to extract features
-        x = self.conv1(x)
-        x = self.bn1(x)
-        x = self.relu(x)
-        x = self.maxpool(x)
-
-        x = self.layer1(x)
-        x = self.layer2(x)
-        x = self.layer3(x)
-        x = self.layer4(x)
-
-        x = self.avgpool(x)
-        x = torch.flatten(x, 1)
-        return x
-
-
-class PlainResNetClassifier(nn.Module):
-    """
-    Basic ResNet Classifier that uses a custom ResNet backbone.
-    """
-    name = "PlainResNetClassifier"
-
-    def __init__(self, num_cls=1, num_layers=50):
-        super(PlainResNetClassifier, self).__init__()
-        self.num_cls = num_cls
-        self.num_layers = num_layers
-        self.feature = None
-        self.classifier = None
-        self.criterion_cls = None
-        # Initialize the network and weights
-        self.setup_net()
-
-    def setup_net(self):
-        """
-        Set up the ResNet classifier according to the specified number of layers.
-        """
-        kwargs = {}
-
-        if self.num_layers == 18:
-            block = BasicBlock
-            layers = [2, 2, 2, 2]
-            # ... [Missing weight URL definition for ResNet18]
-        elif self.num_layers == 50:
-            block = Bottleneck
-            layers = [3, 4, 6, 3]
-            # ... [Missing weight URL definition for ResNet50]
-        else:
-            raise Exception("ResNet Type not supported.")
-
-        self.feature = ResNetBackbone(block, layers, **kwargs)
-        self.classifier = nn.Linear(512 * block.expansion, self.num_cls)
-
-    def setup_criteria(self):
-        """
-        Setup the criterion for classification.
-        """
-        self.criterion_cls = nn.CrossEntropyLoss()
-
-    def feat_init(self):
-        """
-        Initialize the features using pretrained weights.
-        """
-        init_weights = self.pretrained_weights.get_state_dict(progress=True)
-        init_weights = OrderedDict({k.replace("module.", "").replace("feature.", ""): init_weights[k]
-                                    for k in init_weights})
-        self.feature.load_state_dict(init_weights, strict=False)
-        # Print missing and unused keys for debugging purposes
-        load_keys = set(init_weights.keys())
-        self_keys = set(self.feature.state_dict().keys())
-        missing_keys = self_keys - load_keys
-        unused_keys = load_keys - self_keys
-        print("missing keys:", sorted(list(missing_keys)))
-        print("unused_keys:", sorted(list(unused_keys)))
-
-
-class PlainResNetInference(nn.Module):
-    """
-    Inference module for the PlainResNet Classifier.
-    """
-    def __init__(self, num_cls=36, num_layers=50, weights=None, device="cpu", url=None):
-        super(PlainResNetInference, self).__init__()
-        self.device = device
-        self.net = PlainResNetClassifier(num_cls=num_cls, num_layers=num_layers)
-        if weights:
-            clf_weights = torch.load(weights, map_location=torch.device(self.device))
-        elif url:
-            clf_weights = load_state_dict_from_url(url, map_location=torch.device(self.device))
-        else:
-            raise Exception("Need weights for inference.")
-        self.load_state_dict(clf_weights["state_dict"], strict=True)
-        self.eval()
-        self.net.to(self.device)
-
-    def results_generation(self, logits, img_id, id_strip=None):
-        """
-        Process logits to produce final results. 
-
-        Args:
-            logits (torch.Tensor): Logits from the network.
-            img_id (str): image path.       
-            id_strip (str): stiping string for better image id saving.       
-
-        Returns:
-            dict: Dictionary containing the results.
-        """
-        pass
-
-    def forward(self, img):
-        feats = self.net.feature(img)
-        logits = self.net.classifier(feats)
-        return logits
-
-    def single_image_classification(self, img, img_id=None, id_strip=None):
-        logits = self.forward(img.unsqueeze(0).to(self.device))
-        return self.results_generation(logits.cpu(), [img_id], id_strip=id_strip)[0]
-
-    def batch_image_classification(self, dataloader, id_strip=None):
-        """
-        Process a batch of images for classification.
-        """
-        total_logits = []
-        total_paths = []
-
-        with tqdm(total=len(dataloader)) as pbar: 
-            for batch in dataloader:
-                imgs, paths = batch
-                imgs = imgs.to(self.device)
-                total_logits.append(self.forward(imgs))
-                total_paths.append(paths)
-                pbar.update(1)
-
-        total_logits = torch.cat(total_logits, dim=0).cpu()
-        total_paths = np.concatenate(total_paths, axis=0)
-
-        return self.results_generation(total_logits, total_paths, id_strip=id_strip)
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+import numpy as np
+import torch
+import torch.nn as nn
+from torchvision.models.resnet import BasicBlock, Bottleneck, ResNet
+from torch.hub import load_state_dict_from_url
+from tqdm import tqdm
+from collections import OrderedDict
+
+# Making the PlainResNetInference class available for import from this module
+__all__ = ["PlainResNetInference"]
+
+
+class ResNetBackbone(ResNet):
+    """
+    Custom ResNet Backbone that extracts features from input images.
+    """
+    def _forward_impl(self, x):
+        # Following the ResNet structure to extract features
+        x = self.conv1(x)
+        x = self.bn1(x)
+        x = self.relu(x)
+        x = self.maxpool(x)
+
+        x = self.layer1(x)
+        x = self.layer2(x)
+        x = self.layer3(x)
+        x = self.layer4(x)
+
+        x = self.avgpool(x)
+        x = torch.flatten(x, 1)
+        return x
+
+
+class PlainResNetClassifier(nn.Module):
+    """
+    Basic ResNet Classifier that uses a custom ResNet backbone.
+    """
+    name = "PlainResNetClassifier"
+
+    def __init__(self, num_cls=1, num_layers=50):
+        super(PlainResNetClassifier, self).__init__()
+        self.num_cls = num_cls
+        self.num_layers = num_layers
+        self.feature = None
+        self.classifier = None
+        self.criterion_cls = None
+        # Initialize the network and weights
+        self.setup_net()
+
+    def setup_net(self):
+        """
+        Set up the ResNet classifier according to the specified number of layers.
+        """
+        kwargs = {}
+
+        if self.num_layers == 18:
+            block = BasicBlock
+            layers = [2, 2, 2, 2]
+            # ... [Missing weight URL definition for ResNet18]
+        elif self.num_layers == 50:
+            block = Bottleneck
+            layers = [3, 4, 6, 3]
+            # ... [Missing weight URL definition for ResNet50]
+        else:
+            raise Exception("ResNet Type not supported.")
+
+        self.feature = ResNetBackbone(block, layers, **kwargs)
+        self.classifier = nn.Linear(512 * block.expansion, self.num_cls)
+
+    def setup_criteria(self):
+        """
+        Setup the criterion for classification.
+        """
+        self.criterion_cls = nn.CrossEntropyLoss()
+
+    def feat_init(self):
+        """
+        Initialize the features using pretrained weights.
+        """
+        init_weights = self.pretrained_weights.get_state_dict(progress=True)
+        init_weights = OrderedDict({k.replace("module.", "").replace("feature.", ""): init_weights[k]
+                                    for k in init_weights})
+        self.feature.load_state_dict(init_weights, strict=False)
+        # Print missing and unused keys for debugging purposes
+        load_keys = set(init_weights.keys())
+        self_keys = set(self.feature.state_dict().keys())
+        missing_keys = self_keys - load_keys
+        unused_keys = load_keys - self_keys
+        print("missing keys:", sorted(list(missing_keys)))
+        print("unused_keys:", sorted(list(unused_keys)))
+
+
+class PlainResNetInference(nn.Module):
+    """
+    Inference module for the PlainResNet Classifier.
+    """
+    def __init__(self, num_cls=36, num_layers=50, weights=None, device="cpu", url=None):
+        super(PlainResNetInference, self).__init__()
+        self.device = device
+        self.net = PlainResNetClassifier(num_cls=num_cls, num_layers=num_layers)
+        if weights:
+            clf_weights = torch.load(weights, map_location=torch.device(self.device))
+        elif url:
+            clf_weights = load_state_dict_from_url(url, map_location=torch.device(self.device))
+        else:
+            raise Exception("Need weights for inference.")
+        self.load_state_dict(clf_weights["state_dict"], strict=True)
+        self.eval()
+        self.net.to(self.device)
+
+    def results_generation(self, logits, img_id, id_strip=None):
+        """
+        Process logits to produce final results. 
+
+        Args:
+            logits (torch.Tensor): Logits from the network.
+            img_id (str): image path.       
+            id_strip (str): stiping string for better image id saving.       
+
+        Returns:
+            dict: Dictionary containing the results.
+        """
+        pass
+
+    def forward(self, img):
+        feats = self.net.feature(img)
+        logits = self.net.classifier(feats)
+        return logits
+
+    def single_image_classification(self, img, img_id=None, id_strip=None):
+        logits = self.forward(img.unsqueeze(0).to(self.device))
+        return self.results_generation(logits.cpu(), [img_id], id_strip=id_strip)[0]
+
+    def batch_image_classification(self, dataloader, id_strip=None):
+        """
+        Process a batch of images for classification.
+        """
+        total_logits = []
+        total_paths = []
+
+        with tqdm(total=len(dataloader)) as pbar: 
+            for batch in dataloader:
+                imgs, paths = batch
+                imgs = imgs.to(self.device)
+                total_logits.append(self.forward(imgs))
+                total_paths.append(paths)
+                pbar.update(1)
+
+        total_logits = torch.cat(total_logits, dim=0).cpu()
+        total_paths = np.concatenate(total_paths, axis=0)
+
+        return self.results_generation(total_logits, total_paths, id_strip=id_strip)
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/opossum.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/opossum.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-import torch
-from .base_classifier import PlainResNetInference
-
-__all__ = [
-    "AI4GOpossum"
-]
-
-
-class AI4GOpossum(PlainResNetInference):
-    """
-    Opossum Classifier that inherits from PlainResNetInference.
-    This classifier is specialized for distinguishing between Opossums and Non-opossums.
-    """
-    
-    # Image size for the Opossum classifier
-    IMAGE_SIZE = 224
-    
-    # Class names for prediction
-    CLASS_NAMES = {
-        0: "Non-opossum",
-        1: "Opossum"
-    }
-
-    def __init__(self, weights=None, device="cpu", pretrained=True):
-        """
-        Initialize the Opossum Classifier.
-
-        Args:
-            weights (str, optional): Path to the model weights. Defaults to None.
-            device (str, optional): Device for model inference. Defaults to "cpu".
-            pretrained (bool, optional): Whether to use pretrained weights. Defaults to True.
-        """
-
-        # If pretrained, use the provided URL to fetch the weights
-        if pretrained:
-            url = "https://zenodo.org/records/10023414/files/OpossumClassification_v0.0.0.ckpt?download=1"
-        else:
-            url = None
-
-        super(AI4GOpossum, self).__init__(weights=weights, device=device,
-                                          num_cls=1, num_layers=50, url=url)
-
-    def results_generation(self, logits, img_ids, id_strip=None):
-        """
-        Generate results for classification.
-
-        Args:
-            logits (torch.Tensor): Output tensor from the model.
-            img_id (list): List of image identifier.
-            id_strip (str): stiping string for better image id saving.       
-
-        Returns:
-            dict: Dictionary containing image ID, prediction, and confidence score.
-        """
-
-        probs = torch.sigmoid(logits)
-        preds = (probs > 0.5).squeeze(1).numpy().astype(int)
-
-        results = []
-        for pred, img_id, prob in zip(preds, img_ids, probs):
-            r = {"img_id": str(img_id).strip(id_strip)}
-            r["prediction"] = self.CLASS_NAMES[pred]
-            r["class_id"] = pred
-            r["confidence"] = prob.item() if pred == 1 else (1 - prob.item())
-            results.append(r)
-        
-        return results
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+import torch
+from .base_classifier import PlainResNetInference
+
+__all__ = [
+    "AI4GOpossum"
+]
+
+
+class AI4GOpossum(PlainResNetInference):
+    """
+    Opossum Classifier that inherits from PlainResNetInference.
+    This classifier is specialized for distinguishing between Opossums and Non-opossums.
+    """
+    
+    # Image size for the Opossum classifier
+    IMAGE_SIZE = 224
+    
+    # Class names for prediction
+    CLASS_NAMES = {
+        0: "Non-opossum",
+        1: "Opossum"
+    }
+
+    def __init__(self, weights=None, device="cpu", pretrained=True):
+        """
+        Initialize the Opossum Classifier.
+
+        Args:
+            weights (str, optional): Path to the model weights. Defaults to None.
+            device (str, optional): Device for model inference. Defaults to "cpu".
+            pretrained (bool, optional): Whether to use pretrained weights. Defaults to True.
+        """
+
+        # If pretrained, use the provided URL to fetch the weights
+        if pretrained:
+            url = "https://zenodo.org/records/10023414/files/OpossumClassification_v0.0.0.ckpt?download=1"
+        else:
+            url = None
+
+        super(AI4GOpossum, self).__init__(weights=weights, device=device,
+                                          num_cls=1, num_layers=50, url=url)
+
+    def results_generation(self, logits, img_ids, id_strip=None):
+        """
+        Generate results for classification.
+
+        Args:
+            logits (torch.Tensor): Output tensor from the model.
+            img_id (list): List of image identifier.
+            id_strip (str): stiping string for better image id saving.       
+
+        Returns:
+            dict: Dictionary containing image ID, prediction, and confidence score.
+        """
+
+        probs = torch.sigmoid(logits)
+        preds = (probs > 0.5).squeeze(1).numpy().astype(int)
+
+        results = []
+        for pred, img_id, prob in zip(preds, img_ids, probs):
+            r = {"img_id": str(img_id).strip(id_strip)}
+            r["prediction"] = self.CLASS_NAMES[pred]
+            r["class_id"] = pred
+            r["confidence"] = prob.item() if pred == 1 else (1 - prob.item())
+            results.append(r)
+        
+        return results
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/models/classification/resnet/serengeti.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/models/classification/resnet/serengeti.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-import torch
-from .base_classifier import PlainResNetInference
-
-__all__ = [
-    "AI4GSnapshotSerengeti"
-]
-
-
-class AI4GSnapshotSerengeti(PlainResNetInference):
-    """
-    Snapshot Serengeti Animal Classifier that inherits from PlainResNetInference.
-    This classifier is specialized for recognizing 9 different animals and has 1 'other' class.
-    """
-    
-    # Image size for the Opossum classifier
-    IMAGE_SIZE = 224
-    
-    # Class names for prediction
-    CLASS_NAMES = {
-        0: 'wildebeest',
-        1: 'guineafowl',
-        2: 'zebra',
-        3: 'buffalo',
-        4: 'gazellethomsons',
-        5: 'gazellegrants',
-        6: 'warthog',
-        7: 'impala',
-        8: 'hyenaspotted',
-        9: 'other'
-    }
-
-    def __init__(self, weights=None, device="cpu", pretrained=True):
-        """
-        Initialize the Amazon animal Classifier.
-
-        Args:
-            weights (str, optional): Path to the model weights. Defaults to None.
-            device (str, optional): Device for model inference. Defaults to "cpu".
-            pretrained (bool, optional): Whether to use pretrained weights. Defaults to True.
-        """
-
-        # If pretrained, use the provided URL to fetch the weights
-        if pretrained:
-            url = "https://zenodo.org/records/10456813/files/AI4GSnapshotSerengeti.ckpt?download=1"
-        else:
-            url = None
-
-        super(AI4GSnapshotSerengeti, self).__init__(weights=weights, device=device,
-                                                   num_cls=10, num_layers=18, url=url)
-
-    def results_generation(self, logits, img_ids, id_strip=None):
-        """
-        Generate results for classification.
-
-        Args:
-            logits (torch.Tensor): Output tensor from the model.
-            img_id (str): Image identifier.
-            id_strip (str): stiping string for better image id saving.       
-
-        Returns:
-            dict: Dictionary containing image ID, prediction, and confidence score.
-        """
-        
-        probs = torch.softmax(logits, dim=1)
-        preds = probs.argmax(dim=1)
-        confs = probs.max(dim=1)[0]
-
-        results = []
-        for pred, img_id, conf in zip(preds, img_ids, confs):
-            r = {"img_id": str(img_id).strip(id_strip)}
-            r["prediction"] = self.CLASS_NAMES[pred.item()]
-            r["class_id"] = pred.item()
-            r["confidence"] = conf.item()
-            results.append(r)
-        
-        return results
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+import torch
+from .base_classifier import PlainResNetInference
+
+__all__ = [
+    "AI4GSnapshotSerengeti"
+]
+
+
+class AI4GSnapshotSerengeti(PlainResNetInference):
+    """
+    Snapshot Serengeti Animal Classifier that inherits from PlainResNetInference.
+    This classifier is specialized for recognizing 9 different animals and has 1 'other' class.
+    """
+    
+    # Image size for the Opossum classifier
+    IMAGE_SIZE = 224
+    
+    # Class names for prediction
+    CLASS_NAMES = {
+        0: 'wildebeest',
+        1: 'guineafowl',
+        2: 'zebra',
+        3: 'buffalo',
+        4: 'gazellethomsons',
+        5: 'gazellegrants',
+        6: 'warthog',
+        7: 'impala',
+        8: 'hyenaspotted',
+        9: 'other'
+    }
+
+    def __init__(self, weights=None, device="cpu", pretrained=True):
+        """
+        Initialize the Amazon animal Classifier.
+
+        Args:
+            weights (str, optional): Path to the model weights. Defaults to None.
+            device (str, optional): Device for model inference. Defaults to "cpu".
+            pretrained (bool, optional): Whether to use pretrained weights. Defaults to True.
+        """
+
+        # If pretrained, use the provided URL to fetch the weights
+        if pretrained:
+            url = "https://zenodo.org/records/10456813/files/AI4GSnapshotSerengeti.ckpt?download=1"
+        else:
+            url = None
+
+        super(AI4GSnapshotSerengeti, self).__init__(weights=weights, device=device,
+                                                   num_cls=10, num_layers=18, url=url)
+
+    def results_generation(self, logits, img_ids, id_strip=None):
+        """
+        Generate results for classification.
+
+        Args:
+            logits (torch.Tensor): Output tensor from the model.
+            img_id (str): Image identifier.
+            id_strip (str): stiping string for better image id saving.       
+
+        Returns:
+            dict: Dictionary containing image ID, prediction, and confidence score.
+        """
+        
+        probs = torch.softmax(logits, dim=1)
+        preds = probs.argmax(dim=1)
+        confs = probs.max(dim=1)[0]
+
+        results = []
+        for pred, img_id, conf in zip(preds, img_ids, confs):
+            r = {"img_id": str(img_id).strip(id_strip)}
+            r["prediction"] = self.CLASS_NAMES[pred.item()]
+            r["class_id"] = pred.item()
+            r["confidence"] = conf.item()
+            results.append(r)
+        
+        return results
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/models/detection/yolov5/base_detector.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/models/detection/yolov5/base_detector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,169 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-""" YoloV5 base detector class. """
-
-# Importing basic libraries
-
-import numpy as np
-from tqdm import tqdm
-import supervision as sv
-import torch
-from torch.hub import load_state_dict_from_url
-from yolov5.utils.general import non_max_suppression, scale_coords
-
-class YOLOV5Base:
-    """
-    Base detector class for YOLO V5. This class provides utility methods for
-    loading the model, generating results, and performing single and batch image detections.
-    """
-    
-    # Placeholder class-level attributes to be defined in derived classes
-    IMAGE_SIZE = None
-    STRIDE = None
-    CLASS_NAMES = None
-    TRANSFORM = None
-
-    def __init__(self, weights=None, device="cpu", url=None):
-        """
-        Initialize the YOLO V5 detector.
-        
-        Args:
-            weights (str, optional): 
-                Path to the model weights. Defaults to None.
-            device (str, optional): 
-                Device for model inference. Defaults to "cpu".
-            url (str, optional): 
-                URL to fetch the model weights. Defaults to None.
-        """
-        self.model = None
-        self.device = device
-        self._load_model(weights, self.device, url)
-        self.model.to(self.device)
-
-    def _load_model(self, weights=None, device="cpu", url=None):
-        """
-        Load the YOLO V5 model weights.
-        
-        Args:
-            weights (str, optional): 
-                Path to the model weights. Defaults to None.
-            device (str, optional): 
-                Device for model inference. Defaults to "cpu".
-            url (str, optional): 
-                URL to fetch the model weights. Defaults to None.
-        Raises:
-            Exception: If weights are not provided.
-        """
-        if weights:
-            checkpoint = torch.load(weights, map_location=torch.device(device))
-        elif url:
-            checkpoint = load_state_dict_from_url(url, map_location=torch.device(self.device))
-        else:
-            raise Exception("Need weights for inference.")
-        self.model = checkpoint["model"].float().fuse().eval()  # Convert to FP32 model
-
-    def results_generation(self, preds, img_id, id_strip=None):
-        """
-        Generate results for detection based on model predictions.
-        
-        Args:
-            preds (numpy.ndarray): 
-                Model predictions.
-            img_id (str): 
-                Image identifier.
-            id_strip (str, optional): 
-                Strip specific characters from img_id. Defaults to None.
-
-        Returns:
-            dict: Dictionary containing image ID, detections, and labels.
-        """
-        results = {"img_id": str(img_id).strip(id_strip)}
-        results["detections"] = sv.Detections(
-            xyxy=preds[:, :4],
-            confidence=preds[:, 4],
-            class_id=preds[:, 5].astype(int)
-        )
-        results["labels"] = [
-            f"{self.CLASS_NAMES[class_id]} {confidence:0.2f}"
-            for _, _, confidence, class_id, _ in results["detections"]
-        ]
-        return results
-
-    def single_image_detection(self, img, img_size=None, img_path=None, conf_thres=0.2, id_strip=None):
-        """
-        Perform detection on a single image.
-        
-        Args:
-            img (torch.Tensor): 
-                Input image tensor.
-            img_size (tuple): 
-                Original image size.
-            img_path (str): 
-                Image path or identifier.
-            conf_thres (float, optional): 
-                Confidence threshold for predictions. Defaults to 0.2.
-            id_strip (str, optional): 
-                Characters to strip from img_id. Defaults to None.
-
-        Returns:
-            dict: Detection results.
-        """
-        if img_size is None:
-            img_size = img.permute((1, 2, 0)).shape # We need hwc instead of chw for coord scaling
-        preds = self.model(img.unsqueeze(0).to(self.device))[0]
-        preds = torch.cat(non_max_suppression(prediction=preds, conf_thres=conf_thres), axis=0)
-        preds[:, :4] = scale_coords([self.IMAGE_SIZE] * 2, preds[:, :4], img_size).round()
-        return self.results_generation(preds.cpu().numpy(), img_path, id_strip)
-
-    def batch_image_detection(self, dataloader, conf_thres=0.2, id_strip=None):
-        """
-        Perform detection on a batch of images.
-        
-        Args:
-            dataloader (DataLoader): 
-                DataLoader containing image batches.
-            conf_thres (float, optional): 
-                Confidence threshold for predictions. Defaults to 0.2.
-            id_strip (str, optional): 
-                Characters to strip from img_id. Defaults to None.
-
-        Returns:
-            list: List of detection results for all images.
-        """
-        results = []
-        total_preds = []
-        total_paths = []
-        total_img_sizes = []
-
-        with tqdm(total=len(dataloader)) as pbar: 
-            for batch in dataloader:
-                imgs, paths, sizes = batch
-                imgs = imgs.to(self.device)
-                total_preds.append(self.model(imgs)[0].detach().cpu())
-                total_paths.append(paths)
-                total_img_sizes.append(sizes.numpy())
-                pbar.update(1)
-
-        total_preds = [
-            non_max_suppression(prediction=pred.unsqueeze(0), conf_thres=conf_thres)[0].numpy()
-            for pred in torch.cat(total_preds, dim=0).cpu()
-        ]
-        total_paths = np.concatenate(total_paths, axis=0)
-        total_img_sizes = np.concatenate(total_img_sizes, axis=0)
-
-        # If there are size differences in the input images, use a for loop instead of matrix processing for scaling
-        for pred, size, path in zip(total_preds, total_img_sizes, total_paths):
-            pred[:, :4] = scale_coords([self.IMAGE_SIZE] * 2, pred[:, :4], size).round()
-            results.append(self.results_generation(pred, path, id_strip))
-
-        return results
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+""" YoloV5 base detector class. """
+
+# Importing basic libraries
+
+import numpy as np
+from tqdm import tqdm
+import supervision as sv
+import torch
+from torch.hub import load_state_dict_from_url
+from yolov5.utils.general import non_max_suppression, scale_coords
+
+class YOLOV5Base:
+    """
+    Base detector class for YOLO V5. This class provides utility methods for
+    loading the model, generating results, and performing single and batch image detections.
+    """
+    
+    # Placeholder class-level attributes to be defined in derived classes
+    IMAGE_SIZE = None
+    STRIDE = None
+    CLASS_NAMES = None
+    TRANSFORM = None
+
+    def __init__(self, weights=None, device="cpu", url=None):
+        """
+        Initialize the YOLO V5 detector.
+        
+        Args:
+            weights (str, optional): 
+                Path to the model weights. Defaults to None.
+            device (str, optional): 
+                Device for model inference. Defaults to "cpu".
+            url (str, optional): 
+                URL to fetch the model weights. Defaults to None.
+        """
+        self.model = None
+        self.device = device
+        self._load_model(weights, self.device, url)
+        self.model.to(self.device)
+
+    def _load_model(self, weights=None, device="cpu", url=None):
+        """
+        Load the YOLO V5 model weights.
+        
+        Args:
+            weights (str, optional): 
+                Path to the model weights. Defaults to None.
+            device (str, optional): 
+                Device for model inference. Defaults to "cpu".
+            url (str, optional): 
+                URL to fetch the model weights. Defaults to None.
+        Raises:
+            Exception: If weights are not provided.
+        """
+        if weights:
+            checkpoint = torch.load(weights, map_location=torch.device(device))
+        elif url:
+            checkpoint = load_state_dict_from_url(url, map_location=torch.device(self.device))
+        else:
+            raise Exception("Need weights for inference.")
+        self.model = checkpoint["model"].float().fuse().eval()  # Convert to FP32 model
+
+    def results_generation(self, preds, img_id, id_strip=None):
+        """
+        Generate results for detection based on model predictions.
+        
+        Args:
+            preds (numpy.ndarray): 
+                Model predictions.
+            img_id (str): 
+                Image identifier.
+            id_strip (str, optional): 
+                Strip specific characters from img_id. Defaults to None.
+
+        Returns:
+            dict: Dictionary containing image ID, detections, and labels.
+        """
+        results = {"img_id": str(img_id).strip(id_strip)}
+        results["detections"] = sv.Detections(
+            xyxy=preds[:, :4],
+            confidence=preds[:, 4],
+            class_id=preds[:, 5].astype(int)
+        )
+        results["labels"] = [
+            f"{self.CLASS_NAMES[class_id]} {confidence:0.2f}"
+            for _, _, confidence, class_id, _ in results["detections"]
+        ]
+        return results
+
+    def single_image_detection(self, img, img_size=None, img_path=None, conf_thres=0.2, id_strip=None):
+        """
+        Perform detection on a single image.
+        
+        Args:
+            img (torch.Tensor): 
+                Input image tensor.
+            img_size (tuple): 
+                Original image size.
+            img_path (str): 
+                Image path or identifier.
+            conf_thres (float, optional): 
+                Confidence threshold for predictions. Defaults to 0.2.
+            id_strip (str, optional): 
+                Characters to strip from img_id. Defaults to None.
+
+        Returns:
+            dict: Detection results.
+        """
+        if img_size is None:
+            img_size = img.permute((1, 2, 0)).shape # We need hwc instead of chw for coord scaling
+        preds = self.model(img.unsqueeze(0).to(self.device))[0]
+        preds = torch.cat(non_max_suppression(prediction=preds, conf_thres=conf_thres), axis=0)
+        preds[:, :4] = scale_coords([self.IMAGE_SIZE] * 2, preds[:, :4], img_size).round()
+        return self.results_generation(preds.cpu().numpy(), img_path, id_strip)
+
+    def batch_image_detection(self, dataloader, conf_thres=0.2, id_strip=None):
+        """
+        Perform detection on a batch of images.
+        
+        Args:
+            dataloader (DataLoader): 
+                DataLoader containing image batches.
+            conf_thres (float, optional): 
+                Confidence threshold for predictions. Defaults to 0.2.
+            id_strip (str, optional): 
+                Characters to strip from img_id. Defaults to None.
+
+        Returns:
+            list: List of detection results for all images.
+        """
+        results = []
+        total_preds = []
+        total_paths = []
+        total_img_sizes = []
+
+        with tqdm(total=len(dataloader)) as pbar: 
+            for batch in dataloader:
+                imgs, paths, sizes = batch
+                imgs = imgs.to(self.device)
+                total_preds.append(self.model(imgs)[0].detach().cpu())
+                total_paths.append(paths)
+                total_img_sizes.append(sizes.numpy())
+                pbar.update(1)
+
+        total_preds = [
+            non_max_suppression(prediction=pred.unsqueeze(0), conf_thres=conf_thres)[0].numpy()
+            for pred in torch.cat(total_preds, dim=0).cpu()
+        ]
+        total_paths = np.concatenate(total_paths, axis=0)
+        total_img_sizes = np.concatenate(total_img_sizes, axis=0)
+
+        # If there are size differences in the input images, use a for loop instead of matrix processing for scaling
+        for pred, size, path in zip(total_preds, total_img_sizes, total_paths):
+            original_coords = pred[:, :4].copy()
+            normalized_coords = []
+            pred[:, :4] = scale_coords([self.IMAGE_SIZE] * 2, pred[:, :4], size).round()
+            res = self.results_generation(pred, path, id_strip)
+            # Normalize the coordinates for timelapse compatibility
+            for coord in pred[:, :4]:
+                x1, y1, x2, y2 = coord
+                x1, y1, x2, y2 = x1 / size[1], y1 / size[0], x2 / size[1], y2 / size[0]
+                normalized_coords.append([x1, y1, x2, y2])
+            res["normalized_coords"] = normalized_coords
+            results.append(res)
+
+        return results
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife/utils/misc.py` & `PytorchWildlife-1.0.2.9/PytorchWildlife/utils/misc.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
-
-""" Miscellaneous functions."""
-
-import numpy as np
-from tqdm import tqdm
-import cv2
-from typing import Callable
-from supervision import VideoInfo, VideoSink, get_video_frames_generator
-
-__all__ = [
-    "process_video"
-]
-
-
-def process_video(
-    source_path: str,
-    target_path: str,
-    callback: Callable[[np.ndarray, int], np.ndarray],
-    target_fps: int = 1,
-    codec: str = "mp4v"
-) -> None:
-    """
-    Process a video frame-by-frame, applying a callback function to each frame and saving the results 
-    to a new video. This version includes a progress bar and allows codec selection.
-    
-    Args:
-        source_path (str): 
-            Path to the source video file.
-        target_path (str): 
-            Path to save the processed video.
-        callback (Callable[[np.ndarray, int], np.ndarray]): 
-            A function that takes a video frame and its index as input and returns the processed frame.
-        codec (str, optional): 
-            Codec used to encode the processed video. Default is "avc1".
-    """
-    source_video_info = VideoInfo.from_video_path(video_path=source_path)
-    
-    if source_video_info.fps > target_fps:
-        stride = int(source_video_info.fps / target_fps)
-        source_video_info.fps = target_fps
-    else:
-        stride = 1
-    
-    with VideoSink(target_path=target_path, video_info=source_video_info, codec=codec) as sink:
-        with tqdm(total=int(source_video_info.total_frames / stride)) as pbar: 
-            for index, frame in enumerate(
-                get_video_frames_generator(source_path=source_path, stride=stride)
-            ):
-                result_frame = callback(frame, index)
-                sink.write_frame(frame=cv2.cvtColor(result_frame, cv2.COLOR_RGB2BGR))
-                pbar.update(1)
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License.
+
+""" Miscellaneous functions."""
+
+import numpy as np
+from tqdm import tqdm
+import cv2
+from typing import Callable
+from supervision import VideoInfo, VideoSink, get_video_frames_generator
+
+__all__ = [
+    "process_video"
+]
+
+
+def process_video(
+    source_path: str,
+    target_path: str,
+    callback: Callable[[np.ndarray, int], np.ndarray],
+    target_fps: int = 1,
+    codec: str = "mp4v"
+) -> None:
+    """
+    Process a video frame-by-frame, applying a callback function to each frame and saving the results 
+    to a new video. This version includes a progress bar and allows codec selection.
+    
+    Args:
+        source_path (str): 
+            Path to the source video file.
+        target_path (str): 
+            Path to save the processed video.
+        callback (Callable[[np.ndarray, int], np.ndarray]): 
+            A function that takes a video frame and its index as input and returns the processed frame.
+        codec (str, optional): 
+            Codec used to encode the processed video. Default is "avc1".
+    """
+    source_video_info = VideoInfo.from_video_path(video_path=source_path)
+    
+    if source_video_info.fps > target_fps:
+        stride = int(source_video_info.fps / target_fps)
+        source_video_info.fps = target_fps
+    else:
+        stride = 1
+    
+    with VideoSink(target_path=target_path, video_info=source_video_info, codec=codec) as sink:
+        with tqdm(total=int(source_video_info.total_frames / stride)) as pbar: 
+            for index, frame in enumerate(
+                get_video_frames_generator(source_path=source_path, stride=stride)
+            ):
+                result_frame = callback(frame, index)
+                sink.write_frame(frame=cv2.cvtColor(result_frame, cv2.COLOR_RGB2BGR))
+                pbar.update(1)
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/PKG-INFO` & `PytorchWildlife-1.0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,367 +1,358 @@
-Metadata-Version: 2.1
-Name: PytorchWildlife
-Version: 1.0.2.8
-Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
-Home-page: https://github.com/microsoft/CameraTraps/
-Author: Andres Hernandez, Zhongqi Miao
-Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
-License: MIT
-Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: torch==1.10.1
-Requires-Dist: torchvision==0.11.2
-Requires-Dist: torchaudio==0.10.1
-Requires-Dist: tqdm==4.66.1
-Requires-Dist: Pillow==10.1.0
-Requires-Dist: supervision==0.16.0
-Requires-Dist: gradio==4.8.0
-Requires-Dist: ultralytics-yolov5
-Requires-Dist: chardet
-
-![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
-
-<div align="center"> 
-<font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
-<br>
-<hr>
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
-<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
-<a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
-<a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
-<!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
-<a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
-<a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
-<a href="https://discord.gg/TeEVxzaYtm"><img src="https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=Discord" /></a>
-<br><br>
-</div>
-
-
-## ✅ Update highlights (Version 1.0.2)
-- [x] Added Google Colab demos.
-- [x] Added Snapshot Serengeti classification model into the model zoo.
-- [x] Added Classification fine-tuning module.
-- [x] Added a Docker Image for ease of installation.
-
-## 🔥 Future highlights
-- [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
-- [ ] Direct Timelapse format outputs for both detection and classification.
-- [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
-- [ ] Direct LILA connection for more training/validation data.
-- [ ] More pretrained detection and classification models to expand the current model zoo.
-
-To check the full version of the roadmap with completed tasks and long term goals, please click [here!](roadmaps.md).
-
-## 🐾 Introduction
-
-At the core of our mission is the desire to create a harmonious space where conservation scientists from all over the globe can unite. Where they're able to share, grow, use datasets and deep learning architectures for wildlife conservation.
-We've been inspired by the potential and capabilities of Megadetector, and we deeply value its contributions to the community. As we forge ahead with Pytorch-Wildlife, under which Megadetector now resides, please know that we remain committed to supporting, maintaining, and developing Megadetector, ensuring its continued relevance, expansion, and utility.
-
-Pytorch-Wildlife is pip installable:
-```
-pip install PytorchWildlife
-```
-
-To use the newest version of MegaDetector with all the existing functionalities, you can use our [Hugging Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model with **Pytorch-Wildlife**. The weights will be automatically downloaded:
-```python
-from PytorchWildlife.models import detection as pw_detection
-detection_model = pw_detection.MegaDetectorV5()
-```
-
-For those interested in accessing the previous MegaDetector repository, which utilizes the same `MegaDetector v5` model weights and was primarily developed by Dan Morris during his time at Microsoft, please visit the [archive](https://github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that Dan Morris is actively maintaining.
-
->[!TIP]
->If you have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
-
-## 👋 Welcome to Pytorch-Wildlife Version 1.0
-
-**PyTorch-Wildlife** is a platform to create, modify, and share powerful AI conservation models. These models can be used for a variety of applications, including camera trap images, overhead images, underwater images, or bioacoustics. Your engagement with our work is greatly appreciated, and we eagerly await any feedback you may have.
-
-
-The **Pytorch-Wildlife** library allows users to directly load the `MegaDetector v5` model weights for animal detection. We've fully refactored our codebase, prioritizing ease of use in model deployment and expansion. In addition to `MegaDetector v5`, **Pytorch-Wildlife** also accommodates a range of classification weights, such as those derived from the Amazon Rainforest dataset and the Opossum classification dataset. Explore the codebase and functionalities of **Pytorch-Wildlife** through our interactive [HuggingFace web app](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or local [demos and notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo), designed to showcase the practical applications of our enhancements at [PyTorchWildlife](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md). You can find more information in our [documentation](https://cameratraps.readthedocs.io/en/latest/).
-
-👇 Here is a brief example on how to perform detection and classification on a single image using `PyTorch-wildlife`
-```python
-import torch
-from PytorchWildlife.models import detection as pw_detection
-from PytorchWildlife.models import classification as pw_classification
-
-img = torch.randn((3, 1280, 1280))
-
-# Detection
-detection_model = pw_detection.MegaDetectorV5() # Model weights are automatically downloaded.
-detection_result = detection_model.single_image_detection(img)
-
-#Classification
-classification_model = pw_classification.AI4GAmazonRainforest() # Model weights are automatically downloaded.
-classification_results = classification_model.single_image_classification(img)
-```
-
-## ⚙️ Install Pytorch-Wildlife
-```
-pip install PytorchWildlife
-```
-Please refer to our [installation guide](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) for more installation information.
-
-## 🕵️ Explore Pytorch-Wildlife and MegaDetector with our Demo User Interface
-
-If you want to directly try **Pytorch-Wildlife** with the AI models available, including `MegaDetector v5`, you can use our [**Gradio** interface](https://github.com/microsoft/CameraTraps/tree/main/demo). This interface allows users to directly load the `MegaDetector v5` model weights for animal detection. In addition, **Pytorch-Wildlife** also has two classification models in our initial version. One is trained from an Amazon Rainforest camera trap dataset and the other from a Galapagos opossum classification dataset (more details of these datasets will be published soon). To start, please follow the [installation instructions](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) on how to run the Gradio interface! We also provide multiple [**Jupyter** notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo) for demonstration.
-
-![image](https://microsoft.github.io/CameraTraps/assets/gradio_UI.png)
-
-
-## 🛠️ Core Features
-   What are the core components of Pytorch-Wildlife?
-![Pytorch-core-diagram](https://microsoft.github.io/CameraTraps/assets/Pytorch_Wildlife_core_figure.jpg)
-
-
-### 🌐 Unified Framework:
-  Pytorch-Wildlife integrates **four pivotal elements:**
-
-▪ Machine Learning Models<br>
-▪ Pre-trained Weights<br>
-▪ Datasets<br>
-▪ Utilities<br>
-
-### 👷 Our work:
-  In the provided graph, boxes outlined in red represent elements that will be added and remained fixed, while those in blue will be part of our development.
-
-
-### 🚀 Inaugural Model:
-  We're kickstarting with YOLO as our first available model, complemented by pre-trained weights from `MegaDetector v5`. This is the same `MegaDetector v5` model from the previous repository.
-
-
-### 📚 Expandable Repository:
-  As we move forward, our platform will welcome new models and pre-trained weights for camera traps and bioacoustic analysis. We're excited to host contributions from global researchers through a dedicated submission platform.
-
-
-### 📊 Datasets from LILA:
-  Pytorch-Wildlife will also incorporate the vast datasets hosted on LILA, making it a treasure trove for conservation research.
-
-
-### 🧰 Versatile Utilities:
-  Our set of utilities spans from visualization tools to task-specific utilities, many inherited from Megadetector.
-
-
-### 💻 User Interface Flexibility:
-  While we provide a foundational user interface, our platform is designed to inspire. We encourage researchers to craft and share their unique interfaces, and we'll list both existing and new UIs from other collaborators for the community's benefit.
-
-
-Let's shape the future of wildlife research, together! 🙌
-
-
-### 📈 Progress on core tasks
-
-<details>
-<summary> <font size="3"> ▪️ Packaging </font> </summary>
-
-- [ ] Animal detection fine-tuning<br>
-- [x] MegaDetectorV5 integration<br>
-- [ ] MegaDetectorV6 integration<br>
-- [x] User submitted weights<br>
-- [x] Animal classification fine-tuning<br>
-- [x] Amazon Rainforest classification<br>
-- [x] Amazon Opossum classification<br>
-- [ ] User submitted weights<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Utility Toolkit</font></summary>
-
-- [x] Visualization tools<br>
-- [x] MegaDetector utils<br>
-- [ ] User submitted utils<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Datasets</font></summary>
-
-- [ ] Animal Datasets<br>
-- [ ] LILA datasets<br>
-</details><br>
-
-<details>
-<summary><font size="3">▪️ Accessibility</font></summary>
-
-- [x] Basic user interface for demonstration<br>
-- [ ] UI Dev tools<br>
-- [ ] List of available UIs<br>
-</details><br>
-
-
-## 🖼️ Examples
-
-### Image detection using `MegaDetector v5`
-<img src="https://microsoft.github.io/CameraTraps/assets/animal_det_1.JPG" alt="animal_det_1" width="400"/><br>
-*Credits to Universidad de los Andes, Colombia.*
-
-### Image classification with `MegaDetector v5` and `AI4GAmazonRainforest`
-<img src="https://microsoft.github.io/CameraTraps/assets/animal_clas_1.png" alt="animal_clas_1" width="500"/><br>
-*Credits to Universidad de los Andes, Colombia.*
-
-### Opossum ID with `MegaDetector v5` and `AI4GOpossum`
-<img src="https://microsoft.github.io/CameraTraps/assets/opossum_det.png" alt="opossum_det" width="500"/><br>
-*Credits to the Agency for Regulation and Control of Biosecurity and Quarantine for Galápagos (ABG), Ecuador.*
-
-
-## 🤝 Contributing
-This project is open to your ideas and contributions. If you want to submit a pull request, we'll have some guidelines available soon.
-
-We have adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [us](zhongqimiao@microsoft.com) with any additional questions or comments.
-
-## License
-This repository is licensed with the [MIT license](https://github.com/Microsoft/dotnet/blob/main/LICENSE).
-
-
-## 👥 Existing Collaborators
-
-The extensive collaborative efforts of Megadetector have genuinely inspired us, and we deeply value its significant contributions to the community. As we continue to advance with Pytorch-Wildlife, our commitment to delivering technical support to our existing partners on MegaDetector remains the same.
-
-Here we list a few of the organizations that have used MegaDetector. We're only listing organizations who have given us permission to refer to them here or have posted publicly about their use of MegaDetector.
-
-<details>
-<summary><font size="3">👉 Full list of organizations</font></summary>
-
-(Newly Added) [TerrOïko](https://www.terroiko.fr/) ([OCAPI platform](https://www.terroiko.fr/ocapi))
-
-[Arizona Department of Environmental Quality](http://azdeq.gov/)
-
-[Blackbird Environmental](https://blackbirdenv.com/)
-
-[Camelot](https://camelotproject.org/)
-
-[Canadian Parks and Wilderness Society (CPAWS) Northern Alberta Chapter](https://cpawsnab.org/)
-
-[Conservation X Labs](https://conservationxlabs.com/)
-
-[Czech University of Life Sciences Prague](https://www.czu.cz/en)
-
-[EcoLogic Consultants Ltd.](https://www.consult-ecologic.com/)
-
-[Estación Biológica de Doñana](http://www.ebd.csic.es/inicio)
-
-[Idaho Department of Fish and Game](https://idfg.idaho.gov/)
-
-[Island Conservation](https://www.islandconservation.org/)
-
-[Myall Lakes Dingo Project](https://carnivorecoexistence.info/myall-lakes-dingo-project/)
-
-[Point No Point Treaty Council](https://pnptc.org/)
-
-[Ramat Hanadiv Nature Park](https://www.ramat-hanadiv.org.il/en/)
-
-[SPEA (Portuguese Society for the Study of Birds)](https://spea.pt/en/)
-
-[Synthetaic](https://www.synthetaic.com/)
-
-[Taronga Conservation Society](https://taronga.org.au/)
-
-[The Nature Conservancy in Wyoming](https://www.nature.org/en-us/about-us/where-we-work/united-states/wyoming/)
-
-[TrapTagger](https://wildeyeconservation.org/trap-tagger-about/)
-
-[Upper Yellowstone Watershed Group](https://www.upperyellowstone.org/)
-
-[Applied Conservation Macro Ecology Lab](http://www.acmelab.ca/), University of Victoria
-
-[Banff National Park Resource Conservation](https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation), Parks Canada(https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation)
-
-[Blumstein Lab](https://blumsteinlab.eeb.ucla.edu/), UCLA
-
-[Borderlands Research Institute](https://bri.sulross.edu/), Sul Ross State University
-
-[Capitol Reef National Park](https://www.nps.gov/care/index.htm) / Utah Valley University
-
-[Center for Biodiversity and Conservation](https://www.amnh.org/research/center-for-biodiversity-conservation), American Museum of Natural History
-
-[Centre for Ecosystem Science](https://www.unsw.edu.au/research/), UNSW Sydney
-
-[Cross-Cultural Ecology Lab](https://crossculturalecology.net/), Macquarie University
-
-[DC Cat Count](https://hub.dccatcount.org/), led by the Humane Rescue Alliance
-
-[Department of Fish and Wildlife Sciences](https://www.uidaho.edu/cnr/departments/fish-and-wildlife-sciences), University of Idaho
-
-[Department of Wildlife Ecology and Conservation](https://wec.ifas.ufl.edu/), University of Florida
-
-[Ecology and Conservation of Amazonian Vertebrates Research Group](https://www.researchgate.net/lab/Fernanda-Michalski-Lab-4), Federal University of Amapá
-
-[Gola Forest Programma](https://www.rspb.org.uk/our-work/conservation/projects/scientific-support-for-the-gola-forest-programme/), Royal Society for the Protection of Birds (RSPB)
-
-[Graeme Shannon's Research Group](https://wildliferesearch.co.uk/group-1), Bangor University
-
-[Hamaarag](https://hamaarag.org.il/), The Steinhardt Museum of Natural History, Tel Aviv University
-
-[Institut des Science de la Forêt Tempérée (ISFORT)](https://isfort.uqo.ca/), Université du Québec en Outaouais
-
-[Lab of Dr. Bilal Habib](https://bhlab.in/about), the Wildlife Institute of India
-
-[Mammal Spatial Ecology and Conservation Lab](https://labs.wsu.edu/dthornton/), Washington State University
-
-[McLoughlin Lab in Population Ecology](http://mcloughlinlab.ca/lab/), University of Saskatchewan
-
-[National Wildlife Refuge System, Southwest Region](https://www.fws.gov/about/region/southwest), U.S. Fish & Wildlife Service
-
-[Northern Great Plains Program](https://nationalzoo.si.edu/news/restoring-americas-prairie), Smithsonian
-
-[Quantitative Ecology Lab](https://depts.washington.edu/sefsqel/), University of Washington
-
-[Santa Monica Mountains Recreation Area](https://www.nps.gov/samo/index.htm), National Park Service
-
-[Seattle Urban Carnivore Project](https://www.zoo.org/seattlecarnivores), Woodland Park Zoo
-
-[Serra dos Órgãos National Park](https://www.icmbio.gov.br/parnaserradosorgaos/), ICMBio
-
-[Snapshot USA](https://emammal.si.edu/snapshot-usa), Smithsonian
-
-[Wildlife Coexistence Lab](https://wildlife.forestry.ubc.ca/), University of British Columbia
-
-[Wildlife Research](https://www.dfw.state.or.us/wildlife/research/index.asp), Oregon Department of Fish and Wildlife
-
-[Wildlife Division](https://www.michigan.gov/dnr/about/contact/wildlife), Michigan Department of Natural Resources
-
-Department of Ecology, TU Berlin
-
-Ghost Cat Analytics
-
-Protected Areas Unit, Canadian Wildlife Service
-
-[School of Natural Sciences](https://www.utas.edu.au/natural-sciences), University of Tasmania [(story)](https://www.utas.edu.au/about/news-and-stories/articles/2022/1204-innovative-camera-network-keeps-close-eye-on-tassie-wildlife)
-
-[Kenai National Wildlife Refuge](https://www.fws.gov/refuge/kenai), U.S. Fish & Wildlife Service [(story)](https://www.peninsulaclarion.com/sports/refuge-notebook-new-technology-increases-efficiency-of-refuge-cameras/)
-
-[Australian Wildlife Conservancy](https://www.australianwildlife.org/) [(blog](https://www.australianwildlife.org/cutting-edge-technology-delivering-efficiency-gains-in-conservation/), [blog)](https://www.australianwildlife.org/efficiency-gains-at-the-cutting-edge-of-technology/)
-
-[Felidae Conservation Fund](https://felidaefund.org/) [(WildePod platform)](https://wildepod.org/) [(blog post)](https://abhaykashyap.com/blog/ai-powered-camera-trap-image-annotation-system/)
-
-[Alberta Biodiversity Monitoring Institute (ABMI)](https://www.abmi.ca/home.html) [(WildTrax platform)](https://www.wildtrax.ca/) [(blog post)](https://wildcams.ca/blog/the-abmi-visits-the-zoo/)
-
-[Shan Shui Conservation Center](http://en.shanshui.org/) [(blog post)](https://mp.weixin.qq.com/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs) [(translated blog post)](https://mp-weixin-qq-com.translate.goog/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs&_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp)
-
-[Irvine Ranch Conservancy](http://www.irconservancy.org/) [(story)](https://www.ocregister.com/2022/03/30/ai-software-is-helping-researchers-focus-on-learning-about-ocs-wild-animals/)
-
-[Wildlife Protection Solutions](https://wildlifeprotectionsolutions.org/) [(story](https://customers.microsoft.com/en-us/story/1384184517929343083-wildlife-protection-solutions-nonprofit-ai-for-earth), [story)](https://www.enterpriseai.news/2023/02/20/ai-helps-wildlife-protection-solutions-safeguard-endangered-species/)
-
-[Road Ecology Center](https://roadecology.ucdavis.edu/), University of California, Davis [(Wildlife Observer Network platform)](https://wildlifeobserver.net/)
-
-[The Nature Conservancy in California](https://www.nature.org/en-us/about-us/where-we-work/united-states/california/) [(Animl platform)](https://github.com/tnc-ca-geo/animl-frontend)
-
-[San Diego Zoo Wildlife Alliance](https://science.sandiegozoo.org/) [(Animl R package)](https://github.com/conservationtechlab/animl)
-
-</details><br>
-
-
->[!IMPORTANT]
->If you would like to be added to this list or have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our Discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
-
+Metadata-Version: 2.1
+Name: PytorchWildlife
+Version: 1.0.2.9
+Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
+Home-page: https://github.com/microsoft/CameraTraps/
+Author: Andres Hernandez, Zhongqi Miao
+Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
+License: MIT
+Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
+
+<div align="center"> 
+<font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
+<br>
+<hr>
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://static.pepy.tech/badge/pytorchwildlife" /></a> 
+<a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/pyversions/PytorchWildlife" /></a> 
+<a href="https://huggingface.co/spaces/ai4g-biodiversity/pytorch-wildlife"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-blue" /></a>
+<a href="https://colab.research.google.com/drive/1rjqHrTMzEHkMualr4vB55dQWCsCKMNXi?usp=sharing"><img src="https://img.shields.io/badge/Colab-Demo-blue?logo=GoogleColab" /></a>
+<!-- <a href="https://colab.research.google.com/drive/16-OjFVQ6nopuP-gfqofYBBY00oIgbcr1?usp=sharing"><img src="https://img.shields.io/badge/Colab-Video detection-blue?logo=GoogleColab" /></a> -->
+<a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
+<a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
+<a href="https://discord.gg/TeEVxzaYtm"><img src="https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=Discord" /></a>
+<br><br>
+</div>
+
+
+## ✅ Update highlights (Version 1.0.2.9)
+- [x] Added Timelapse compatibility! Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo).
+- [x] Added Google Colab demos.
+- [x] Added Snapshot Serengeti classification model into the model zoo.
+- [x] Added Classification fine-tuning module.
+- [x] Added a Docker Image for ease of installation.
+
+## 🔥 Future highlights
+- [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
+- [ ] Direct Timelapse format outputs for both detection and classification.
+- [ ] A detection model fine-tuning module to fine-tune your own detection model for Pytorch-Wildlife.
+- [ ] Direct LILA connection for more training/validation data.
+- [ ] More pretrained detection and classification models to expand the current model zoo.
+
+To check the full version of the roadmap with completed tasks and long term goals, please click [here!](roadmaps.md).
+
+## 🐾 Introduction
+
+At the core of our mission is the desire to create a harmonious space where conservation scientists from all over the globe can unite. Where they're able to share, grow, use datasets and deep learning architectures for wildlife conservation.
+We've been inspired by the potential and capabilities of Megadetector, and we deeply value its contributions to the community. As we forge ahead with Pytorch-Wildlife, under which Megadetector now resides, please know that we remain committed to supporting, maintaining, and developing Megadetector, ensuring its continued relevance, expansion, and utility.
+
+Pytorch-Wildlife is pip installable:
+```
+pip install PytorchWildlife
+```
+
+To use the newest version of MegaDetector with all the existing functionalities, you can use our [Hugging Face interface](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or simply load the model with **Pytorch-Wildlife**. The weights will be automatically downloaded:
+```python
+from PytorchWildlife.models import detection as pw_detection
+detection_model = pw_detection.MegaDetectorV5()
+```
+
+For those interested in accessing the previous MegaDetector repository, which utilizes the same `MegaDetector v5` model weights and was primarily developed by Dan Morris during his time at Microsoft, please visit the [archive](https://github.com/microsoft/CameraTraps/blob/main/archive) directory, or you can visit this [forked repository](https://github.com/agentmorris/MegaDetector/tree/main) that Dan Morris is actively maintaining.
+
+>[!TIP]
+>If you have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
+
+## 👋 Welcome to Pytorch-Wildlife Version 1.0
+
+**PyTorch-Wildlife** is a platform to create, modify, and share powerful AI conservation models. These models can be used for a variety of applications, including camera trap images, overhead images, underwater images, or bioacoustics. Your engagement with our work is greatly appreciated, and we eagerly await any feedback you may have.
+
+
+The **Pytorch-Wildlife** library allows users to directly load the `MegaDetector v5` model weights for animal detection. We've fully refactored our codebase, prioritizing ease of use in model deployment and expansion. In addition to `MegaDetector v5`, **Pytorch-Wildlife** also accommodates a range of classification weights, such as those derived from the Amazon Rainforest dataset and the Opossum classification dataset. Explore the codebase and functionalities of **Pytorch-Wildlife** through our interactive [HuggingFace web app](https://huggingface.co/spaces/AndresHdzC/pytorch-wildlife) or local [demos and notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo), designed to showcase the practical applications of our enhancements at [PyTorchWildlife](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md). You can find more information in our [documentation](https://cameratraps.readthedocs.io/en/latest/).
+
+👇 Here is a brief example on how to perform detection and classification on a single image using `PyTorch-wildlife`
+```python
+import torch
+from PytorchWildlife.models import detection as pw_detection
+from PytorchWildlife.models import classification as pw_classification
+
+img = torch.randn((3, 1280, 1280))
+
+# Detection
+detection_model = pw_detection.MegaDetectorV5() # Model weights are automatically downloaded.
+detection_result = detection_model.single_image_detection(img)
+
+#Classification
+classification_model = pw_classification.AI4GAmazonRainforest() # Model weights are automatically downloaded.
+classification_results = classification_model.single_image_classification(img)
+```
+
+## ⚙️ Install Pytorch-Wildlife
+```
+pip install PytorchWildlife
+```
+Please refer to our [installation guide](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) for more installation information.
+
+## 🕵️ Explore Pytorch-Wildlife and MegaDetector with our Demo User Interface
+
+If you want to directly try **Pytorch-Wildlife** with the AI models available, including `MegaDetector v5`, you can use our [**Gradio** interface](https://github.com/microsoft/CameraTraps/tree/main/demo). This interface allows users to directly load the `MegaDetector v5` model weights for animal detection. In addition, **Pytorch-Wildlife** also has two classification models in our initial version. One is trained from an Amazon Rainforest camera trap dataset and the other from a Galapagos opossum classification dataset (more details of these datasets will be published soon). To start, please follow the [installation instructions](https://github.com/microsoft/CameraTraps/blob/main/INSTALLATION.md) on how to run the Gradio interface! We also provide multiple [**Jupyter** notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo) for demonstration.
+
+![image](https://microsoft.github.io/CameraTraps/assets/gradio_UI.png)
+
+
+## 🛠️ Core Features
+   What are the core components of Pytorch-Wildlife?
+![Pytorch-core-diagram](https://microsoft.github.io/CameraTraps/assets/Pytorch_Wildlife_core_figure.jpg)
+
+
+### 🌐 Unified Framework:
+  Pytorch-Wildlife integrates **four pivotal elements:**
+
+▪ Machine Learning Models<br>
+▪ Pre-trained Weights<br>
+▪ Datasets<br>
+▪ Utilities<br>
+
+### 👷 Our work:
+  In the provided graph, boxes outlined in red represent elements that will be added and remained fixed, while those in blue will be part of our development.
+
+
+### 🚀 Inaugural Model:
+  We're kickstarting with YOLO as our first available model, complemented by pre-trained weights from `MegaDetector v5`. This is the same `MegaDetector v5` model from the previous repository.
+
+
+### 📚 Expandable Repository:
+  As we move forward, our platform will welcome new models and pre-trained weights for camera traps and bioacoustic analysis. We're excited to host contributions from global researchers through a dedicated submission platform.
+
+
+### 📊 Datasets from LILA:
+  Pytorch-Wildlife will also incorporate the vast datasets hosted on LILA, making it a treasure trove for conservation research.
+
+
+### 🧰 Versatile Utilities:
+  Our set of utilities spans from visualization tools to task-specific utilities, many inherited from Megadetector.
+
+
+### 💻 User Interface Flexibility:
+  While we provide a foundational user interface, our platform is designed to inspire. We encourage researchers to craft and share their unique interfaces, and we'll list both existing and new UIs from other collaborators for the community's benefit.
+
+
+Let's shape the future of wildlife research, together! 🙌
+
+
+### 📈 Progress on core tasks
+
+<details>
+<summary> <font size="3"> ▪️ Packaging </font> </summary>
+
+- [ ] Animal detection fine-tuning<br>
+- [x] MegaDetectorV5 integration<br>
+- [ ] MegaDetectorV6 integration<br>
+- [x] User submitted weights<br>
+- [x] Animal classification fine-tuning<br>
+- [x] Amazon Rainforest classification<br>
+- [x] Amazon Opossum classification<br>
+- [ ] User submitted weights<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Utility Toolkit</font></summary>
+
+- [x] Visualization tools<br>
+- [x] MegaDetector utils<br>
+- [ ] User submitted utils<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Datasets</font></summary>
+
+- [ ] Animal Datasets<br>
+- [ ] LILA datasets<br>
+</details><br>
+
+<details>
+<summary><font size="3">▪️ Accessibility</font></summary>
+
+- [x] Basic user interface for demonstration<br>
+- [ ] UI Dev tools<br>
+- [ ] List of available UIs<br>
+</details><br>
+
+
+## 🖼️ Examples
+
+### Image detection using `MegaDetector v5`
+<img src="https://microsoft.github.io/CameraTraps/assets/animal_det_1.JPG" alt="animal_det_1" width="400"/><br>
+*Credits to Universidad de los Andes, Colombia.*
+
+### Image classification with `MegaDetector v5` and `AI4GAmazonRainforest`
+<img src="https://microsoft.github.io/CameraTraps/assets/animal_clas_1.png" alt="animal_clas_1" width="500"/><br>
+*Credits to Universidad de los Andes, Colombia.*
+
+### Opossum ID with `MegaDetector v5` and `AI4GOpossum`
+<img src="https://microsoft.github.io/CameraTraps/assets/opossum_det.png" alt="opossum_det" width="500"/><br>
+*Credits to the Agency for Regulation and Control of Biosecurity and Quarantine for Galápagos (ABG), Ecuador.*
+
+
+## 🤝 Contributing
+This project is open to your ideas and contributions. If you want to submit a pull request, we'll have some guidelines available soon.
+
+We have adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [us](zhongqimiao@microsoft.com) with any additional questions or comments.
+
+## License
+This repository is licensed with the [MIT license](https://github.com/Microsoft/dotnet/blob/main/LICENSE).
+
+
+## 👥 Existing Collaborators
+
+The extensive collaborative efforts of Megadetector have genuinely inspired us, and we deeply value its significant contributions to the community. As we continue to advance with Pytorch-Wildlife, our commitment to delivering technical support to our existing partners on MegaDetector remains the same.
+
+Here we list a few of the organizations that have used MegaDetector. We're only listing organizations who have given us permission to refer to them here or have posted publicly about their use of MegaDetector.
+
+<details>
+<summary><font size="3">👉 Full list of organizations</font></summary>
+
+(Newly Added) [TerrOïko](https://www.terroiko.fr/) ([OCAPI platform](https://www.terroiko.fr/ocapi))
+
+[Arizona Department of Environmental Quality](http://azdeq.gov/)
+
+[Blackbird Environmental](https://blackbirdenv.com/)
+
+[Camelot](https://camelotproject.org/)
+
+[Canadian Parks and Wilderness Society (CPAWS) Northern Alberta Chapter](https://cpawsnab.org/)
+
+[Conservation X Labs](https://conservationxlabs.com/)
+
+[Czech University of Life Sciences Prague](https://www.czu.cz/en)
+
+[EcoLogic Consultants Ltd.](https://www.consult-ecologic.com/)
+
+[Estación Biológica de Doñana](http://www.ebd.csic.es/inicio)
+
+[Idaho Department of Fish and Game](https://idfg.idaho.gov/)
+
+[Island Conservation](https://www.islandconservation.org/)
+
+[Myall Lakes Dingo Project](https://carnivorecoexistence.info/myall-lakes-dingo-project/)
+
+[Point No Point Treaty Council](https://pnptc.org/)
+
+[Ramat Hanadiv Nature Park](https://www.ramat-hanadiv.org.il/en/)
+
+[SPEA (Portuguese Society for the Study of Birds)](https://spea.pt/en/)
+
+[Synthetaic](https://www.synthetaic.com/)
+
+[Taronga Conservation Society](https://taronga.org.au/)
+
+[The Nature Conservancy in Wyoming](https://www.nature.org/en-us/about-us/where-we-work/united-states/wyoming/)
+
+[TrapTagger](https://wildeyeconservation.org/trap-tagger-about/)
+
+[Upper Yellowstone Watershed Group](https://www.upperyellowstone.org/)
+
+[Applied Conservation Macro Ecology Lab](http://www.acmelab.ca/), University of Victoria
+
+[Banff National Park Resource Conservation](https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation), Parks Canada(https://www.pc.gc.ca/en/pn-np/ab/banff/nature/conservation)
+
+[Blumstein Lab](https://blumsteinlab.eeb.ucla.edu/), UCLA
+
+[Borderlands Research Institute](https://bri.sulross.edu/), Sul Ross State University
+
+[Capitol Reef National Park](https://www.nps.gov/care/index.htm) / Utah Valley University
+
+[Center for Biodiversity and Conservation](https://www.amnh.org/research/center-for-biodiversity-conservation), American Museum of Natural History
+
+[Centre for Ecosystem Science](https://www.unsw.edu.au/research/), UNSW Sydney
+
+[Cross-Cultural Ecology Lab](https://crossculturalecology.net/), Macquarie University
+
+[DC Cat Count](https://hub.dccatcount.org/), led by the Humane Rescue Alliance
+
+[Department of Fish and Wildlife Sciences](https://www.uidaho.edu/cnr/departments/fish-and-wildlife-sciences), University of Idaho
+
+[Department of Wildlife Ecology and Conservation](https://wec.ifas.ufl.edu/), University of Florida
+
+[Ecology and Conservation of Amazonian Vertebrates Research Group](https://www.researchgate.net/lab/Fernanda-Michalski-Lab-4), Federal University of Amapá
+
+[Gola Forest Programma](https://www.rspb.org.uk/our-work/conservation/projects/scientific-support-for-the-gola-forest-programme/), Royal Society for the Protection of Birds (RSPB)
+
+[Graeme Shannon's Research Group](https://wildliferesearch.co.uk/group-1), Bangor University
+
+[Hamaarag](https://hamaarag.org.il/), The Steinhardt Museum of Natural History, Tel Aviv University
+
+[Institut des Science de la Forêt Tempérée (ISFORT)](https://isfort.uqo.ca/), Université du Québec en Outaouais
+
+[Lab of Dr. Bilal Habib](https://bhlab.in/about), the Wildlife Institute of India
+
+[Mammal Spatial Ecology and Conservation Lab](https://labs.wsu.edu/dthornton/), Washington State University
+
+[McLoughlin Lab in Population Ecology](http://mcloughlinlab.ca/lab/), University of Saskatchewan
+
+[National Wildlife Refuge System, Southwest Region](https://www.fws.gov/about/region/southwest), U.S. Fish & Wildlife Service
+
+[Northern Great Plains Program](https://nationalzoo.si.edu/news/restoring-americas-prairie), Smithsonian
+
+[Quantitative Ecology Lab](https://depts.washington.edu/sefsqel/), University of Washington
+
+[Santa Monica Mountains Recreation Area](https://www.nps.gov/samo/index.htm), National Park Service
+
+[Seattle Urban Carnivore Project](https://www.zoo.org/seattlecarnivores), Woodland Park Zoo
+
+[Serra dos Órgãos National Park](https://www.icmbio.gov.br/parnaserradosorgaos/), ICMBio
+
+[Snapshot USA](https://emammal.si.edu/snapshot-usa), Smithsonian
+
+[Wildlife Coexistence Lab](https://wildlife.forestry.ubc.ca/), University of British Columbia
+
+[Wildlife Research](https://www.dfw.state.or.us/wildlife/research/index.asp), Oregon Department of Fish and Wildlife
+
+[Wildlife Division](https://www.michigan.gov/dnr/about/contact/wildlife), Michigan Department of Natural Resources
+
+Department of Ecology, TU Berlin
+
+Ghost Cat Analytics
+
+Protected Areas Unit, Canadian Wildlife Service
+
+[School of Natural Sciences](https://www.utas.edu.au/natural-sciences), University of Tasmania [(story)](https://www.utas.edu.au/about/news-and-stories/articles/2022/1204-innovative-camera-network-keeps-close-eye-on-tassie-wildlife)
+
+[Kenai National Wildlife Refuge](https://www.fws.gov/refuge/kenai), U.S. Fish & Wildlife Service [(story)](https://www.peninsulaclarion.com/sports/refuge-notebook-new-technology-increases-efficiency-of-refuge-cameras/)
+
+[Australian Wildlife Conservancy](https://www.australianwildlife.org/) [(blog](https://www.australianwildlife.org/cutting-edge-technology-delivering-efficiency-gains-in-conservation/), [blog)](https://www.australianwildlife.org/efficiency-gains-at-the-cutting-edge-of-technology/)
+
+[Felidae Conservation Fund](https://felidaefund.org/) [(WildePod platform)](https://wildepod.org/) [(blog post)](https://abhaykashyap.com/blog/ai-powered-camera-trap-image-annotation-system/)
+
+[Alberta Biodiversity Monitoring Institute (ABMI)](https://www.abmi.ca/home.html) [(WildTrax platform)](https://www.wildtrax.ca/) [(blog post)](https://wildcams.ca/blog/the-abmi-visits-the-zoo/)
+
+[Shan Shui Conservation Center](http://en.shanshui.org/) [(blog post)](https://mp.weixin.qq.com/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs) [(translated blog post)](https://mp-weixin-qq-com.translate.goog/s/iOIQF3ckj0-rEG4yJgerYw?fbclid=IwAR0alwiWbe3udIcFvqqwm7y5qgr9hZpjr871FZIa-ErGUukZ7yJ3ZhgCevs&_x_tr_sl=auto&_x_tr_tl=en&_x_tr_hl=en&_x_tr_pto=wapp)
+
+[Irvine Ranch Conservancy](http://www.irconservancy.org/) [(story)](https://www.ocregister.com/2022/03/30/ai-software-is-helping-researchers-focus-on-learning-about-ocs-wild-animals/)
+
+[Wildlife Protection Solutions](https://wildlifeprotectionsolutions.org/) [(story](https://customers.microsoft.com/en-us/story/1384184517929343083-wildlife-protection-solutions-nonprofit-ai-for-earth), [story)](https://www.enterpriseai.news/2023/02/20/ai-helps-wildlife-protection-solutions-safeguard-endangered-species/)
+
+[Road Ecology Center](https://roadecology.ucdavis.edu/), University of California, Davis [(Wildlife Observer Network platform)](https://wildlifeobserver.net/)
+
+[The Nature Conservancy in California](https://www.nature.org/en-us/about-us/where-we-work/united-states/california/) [(Animl platform)](https://github.com/tnc-ca-geo/animl-frontend)
+
+[San Diego Zoo Wildlife Alliance](https://science.sandiegozoo.org/) [(Animl R package)](https://github.com/conservationtechlab/animl)
+
+</details><br>
+
+
+>[!IMPORTANT]
+>If you would like to be added to this list or have any questions regarding MegaDetector and Pytorch-Wildlife, please [email us](zhongqimiao@microsoft.com) or join us in our Discord channel: [![](https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=PytorchWildife)](https://discord.gg/TeEVxzaYtm)
+
```

#### html2text {}

```diff
@@ -1,41 +1,39 @@
-Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.8 Summary: a PyTorch
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9 Summary: a PyTorch
 Collaborative Deep Learning Framework for Conservation. Home-page: https://
 github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
 Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
 Keywords:
 pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy Requires-Dist: torch==1.10.1
-Requires-Dist: torchvision==0.11.2 Requires-Dist: torchaudio==0.10.1 Requires-
-Dist: tqdm==4.66.1 Requires-Dist: Pillow==10.1.0 Requires-Dist:
-supervision==0.16.0 Requires-Dist: gradio==4.8.0 Requires-Dist: ultralytics-
-yolov5 Requires-Dist: chardet ![image](https://microsoft.github.io/CameraTraps/
-assets/Pytorch_Banner_transparentbk.png)
+License-File: LICENSE ![image](https://microsoft.github.io/CameraTraps/assets/
+Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
 _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
  _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
    _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
                    _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
-## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
-Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. - [x] Added a Docker Image for ease of
-installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
-model sizes for both optimized performance and low-budget devices like camera
-systems. - [ ] Direct Timelapse format outputs for both detection and
+## â Update highlights (Version 1.0.2.9) - [x] Added Timelapse compatibility!
+Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://
+github.com/microsoft/CameraTraps/tree/main/demo). - [x] Added Google Colab
+demos. - [x] Added Snapshot Serengeti classification model into the model zoo.
+- [x] Added Classification fine-tuning module. - [x] Added a Docker Image for
+ease of installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with
+multiple model sizes for both optimized performance and low-budget devices like
+camera systems. - [ ] Direct Timelapse format outputs for both detection and
 classification. - [ ] A detection model fine-tuning module to fine-tune your
 own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
 training/validation data. - [ ] More pretrained detection and classification
 models to expand the current model zoo. To check the full version of the
 roadmap with completed tasks and long term goals, please click [here!]
 (roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
 create a harmonious space where conservation scientists from all over the globe
```

### Comparing `PytorchWildlife-1.0.2.8/PytorchWildlife.egg-info/SOURCES.txt` & `PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PytorchWildlife-1.0.2.8/README.md` & `PytorchWildlife-1.0.2.9/PytorchWildlife.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: PytorchWildlife
+Version: 1.0.2.9
+Summary: a PyTorch Collaborative Deep Learning Framework for Conservation.
+Home-page: https://github.com/microsoft/CameraTraps/
+Author: Andres Hernandez, Zhongqi Miao
+Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com
+License: MIT
+Keywords: pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![image](https://microsoft.github.io/CameraTraps/assets/Pytorch_Banner_transparentbk.png)
 
 <div align="center"> 
 <font size="6"> A Collaborative Deep Learning Framework for Conservation </font>
 <br>
 <hr>
 <a href="https://pypi.org/project/PytorchWildlife"><img src="https://img.shields.io/pypi/v/PytorchWildlife?color=limegreen" /></a> 
@@ -13,15 +34,16 @@
 <a href="https://cameratraps.readthedocs.io/en/latest/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=ReadtheDocs" /></a>
 <a href="https://github.com/microsoft/CameraTraps/blob/main/LICENSE"><img src="https://img.shields.io/pypi/l/PytorchWildlife" /></a>
 <a href="https://discord.gg/TeEVxzaYtm"><img src="https://img.shields.io/badge/any_text-Join_us!-blue?logo=discord&label=Discord" /></a>
 <br><br>
 </div>
 
 
-## ✅ Update highlights (Version 1.0.2)
+## ✅ Update highlights (Version 1.0.2.9)
+- [x] Added Timelapse compatibility! Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://github.com/microsoft/CameraTraps/tree/main/demo).
 - [x] Added Google Colab demos.
 - [x] Added Snapshot Serengeti classification model into the model zoo.
 - [x] Added Classification fine-tuning module.
 - [x] Added a Docker Image for ease of installation.
 
 ## 🔥 Future highlights
 - [ ] MegaDetectorV6 with multiple model sizes for both optimized performance and low-budget devices like camera systems.
```

#### html2text {}

```diff
@@ -1,25 +1,39 @@
-![image](https://microsoft.github.io/CameraTraps/assets/
+Metadata-Version: 2.1 Name: PytorchWildlife Version: 1.0.2.9 Summary: a PyTorch
+Collaborative Deep Learning Framework for Conservation. Home-page: https://
+github.com/microsoft/CameraTraps/ Author: Andres Hernandez, Zhongqi Miao
+Author-email: v-herandres@microsoft.com, zhongqimiao@microsoft.com License: MIT
+Keywords:
+pytorch_wildlife,pytorch,wildlife,megadetector,conservation,animal,detection,classification
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE ![image](https://microsoft.github.io/CameraTraps/assets/
 Pytorch_Banner_transparentbk.png)
            A Collaborative Deep Learning Framework for Conservation
 ===============================================================================
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_?_c_o_l_o_r_=_l_i_m_e_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/
 _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_y_t_o_r_c_h_w_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
  _P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_%_F_0_%_9_F_%_A_4_%_9_7_%_2_0_H_u_g_g_i_n_g_%_2_0_F_a_c_e_-
    _D_e_m_o_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_l_a_b_-_D_e_m_o_-_b_l_u_e_?_l_o_g_o_=_G_o_o_g_l_e_C_o_l_a_b_]
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_R_e_a_d_t_h_e_D_o_c_s_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_P_y_t_o_r_c_h_W_i_l_d_l_i_f_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_n_y___t_e_x_t_-
                    _J_o_i_n___u_s_!_-_b_l_u_e_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_D_i_s_c_o_r_d_]
 
-## â Update highlights (Version 1.0.2) - [x] Added Google Colab demos. - [x]
-Added Snapshot Serengeti classification model into the model zoo. - [x] Added
-Classification fine-tuning module. - [x] Added a Docker Image for ease of
-installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with multiple
-model sizes for both optimized performance and low-budget devices like camera
-systems. - [ ] Direct Timelapse format outputs for both detection and
+## â Update highlights (Version 1.0.2.9) - [x] Added Timelapse compatibility!
+Check the [Gradio interface](INSTALLATION.md) or [notebooks](https://
+github.com/microsoft/CameraTraps/tree/main/demo). - [x] Added Google Colab
+demos. - [x] Added Snapshot Serengeti classification model into the model zoo.
+- [x] Added Classification fine-tuning module. - [x] Added a Docker Image for
+ease of installation. ## ð¥ Future highlights - [ ] MegaDetectorV6 with
+multiple model sizes for both optimized performance and low-budget devices like
+camera systems. - [ ] Direct Timelapse format outputs for both detection and
 classification. - [ ] A detection model fine-tuning module to fine-tune your
 own detection model for Pytorch-Wildlife. - [ ] Direct LILA connection for more
 training/validation data. - [ ] More pretrained detection and classification
 models to expand the current model zoo. To check the full version of the
 roadmap with completed tasks and long term goals, please click [here!]
 (roadmaps.md). ## ð¾ Introduction At the core of our mission is the desire to
 create a harmonious space where conservation scientists from all over the globe
```

### Comparing `PytorchWildlife-1.0.2.8/setup.py` & `PytorchWildlife-1.0.2.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup, find_packages
-
-with open('README.md', encoding="utf8") as file:
-        long_description = file.read()
-setup(
-    name='PytorchWildlife',
-    version='1.0.2.8', 
-    packages=find_packages(),
-    url='https://github.com/microsoft/CameraTraps/',  
-    license='MIT',
-    author='Andres Hernandez, Zhongqi Miao',
-    author_email='v-herandres@microsoft.com, zhongqimiao@microsoft.com',  
-    description='a PyTorch Collaborative Deep Learning Framework for Conservation.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    install_requires=[
-        'numpy',
-        'torch==1.10.1',
-        'torchvision==0.11.2',
-        'torchaudio==0.10.1',
-        'tqdm==4.66.1',
-        'Pillow==10.1.0', 
-        'supervision==0.16.0',
-        'gradio==4.8.0',
-        'ultralytics-yolov5',
-        'chardet'
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',  
-        'Intended Audience :: Developers', 
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    keywords='pytorch_wildlife, pytorch, wildlife, megadetector, conservation, animal, detection, classification',
-    python_requires='>=3.8',
-)
+from setuptools import setup, find_packages
+
+with open('README.md', encoding="utf8") as file:
+        long_description = file.read()
+setup(
+    name='PytorchWildlife',
+    version='1.0.2.9', 
+    packages=find_packages(),
+    url='https://github.com/microsoft/CameraTraps/',  
+    license='MIT',
+    author='Andres Hernandez, Zhongqi Miao',
+    author_email='v-herandres@microsoft.com, zhongqimiao@microsoft.com',  
+    description='a PyTorch Collaborative Deep Learning Framework for Conservation.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    install_requires=[
+        'numpy',
+        'torch==1.10.1',
+        'torchvision==0.11.2',
+        'torchaudio==0.10.1',
+        'tqdm==4.66.1',
+        'Pillow==10.1.0', 
+        'supervision==0.16.0',
+        'gradio==4.8.0',
+        'ultralytics-yolov5',
+        'chardet'
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',  
+        'Intended Audience :: Developers', 
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+    ],
+    keywords='pytorch_wildlife, pytorch, wildlife, megadetector, conservation, animal, detection, classification',
+    python_requires='>=3.8',
+)
```

