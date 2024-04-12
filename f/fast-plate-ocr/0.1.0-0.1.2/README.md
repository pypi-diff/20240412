# Comparing `tmp/fast_plate_ocr-0.1.0.tar.gz` & `tmp/fast_plate_ocr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_plate_ocr-0.1.0.tar", max compression
+gzip compressed data, was "fast_plate_ocr-0.1.2.tar", max compression
```

## Comparing `fast_plate_ocr-0.1.0.tar` & `fast_plate_ocr-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-10 03:43:12.706250 fast_plate_ocr-0.1.0/LICENSE
--rw-r--r--   0        0        0    12060 2024-04-10 03:43:12.706250 fast_plate_ocr-0.1.0/README.md
--rw-r--r--   0        0        0      140 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/__init__.py
--rw-r--r--   0        0        0      802 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/cli.py
--rw-r--r--   0        0        0     2665 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/onnx_converter.py
--rw-r--r--   0        0        0     6300 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/train.py
--rw-r--r--   0        0        0     1773 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/valid.py
--rw-r--r--   0        0        0     4344 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/visualize_augmentation.py
--rw-r--r--   0        0        0     2662 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/cli/visualize_predictions.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/common/__init__.py
--rw-r--r--   0        0        0     1235 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/common/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/config.py
--rw-r--r--   0        0        0     3536 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/hub.py
--rw-r--r--   0        0        0     7557 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/onnx_inference.py
--rw-r--r--   0        0        0     2726 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/process.py
--rw-r--r--   0        0        0      752 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/inference/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/py.typed
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/data/__init__.py
--rw-r--r--   0        0        0      804 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/data/augmentation.py
--rw-r--r--   0        0        0     1615 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/__init__.py
--rw-r--r--   0        0        0     1452 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/config.py
--rw-r--r--   0        0        0     2601 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/custom.py
--rw-r--r--   0        0        0     2400 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/layer_blocks.py
--rw-r--r--   0        0        0     2709 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/models.py
--rw-r--r--   0        0        0        0 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/utilities/__init__.py
--rw-r--r--   0        0        0      900 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/utilities/backend_utils.py
--rw-r--r--   0        0        0     5345 2024-04-10 03:43:12.718250 fast_plate_ocr-0.1.0/fast_plate_ocr/train/utilities/utils.py
--rw-r--r--   0        0        0     3549 2024-04-10 03:43:12.722250 fast_plate_ocr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14119 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/LICENSE
+-rw-r--r--   0        0        0    12182 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/README.md
+-rw-r--r--   0        0        0      140 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/__init__.py
+-rw-r--r--   0        0        0      802 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/cli.py
+-rw-r--r--   0        0        0     2665 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/onnx_converter.py
+-rw-r--r--   0        0        0     6300 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/train.py
+-rw-r--r--   0        0        0     1773 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/valid.py
+-rw-r--r--   0        0        0     4344 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_augmentation.py
+-rw-r--r--   0        0        0     2662 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_predictions.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/common/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/common/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/config.py
+-rw-r--r--   0        0        0     3548 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/hub.py
+-rw-r--r--   0        0        0     7684 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/onnx_inference.py
+-rw-r--r--   0        0        0     2726 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/process.py
+-rw-r--r--   0        0        0      752 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/inference/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/py.typed
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/augmentation.py
+-rw-r--r--   0        0        0     1615 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/__init__.py
+-rw-r--r--   0        0        0     1452 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/config.py
+-rw-r--r--   0        0        0     2601 2024-04-12 21:02:17.369462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/custom.py
+-rw-r--r--   0        0        0     2400 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/layer_blocks.py
+-rw-r--r--   0        0        0     2709 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/models.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/backend_utils.py
+-rw-r--r--   0        0        0     5345 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/utils.py
+-rw-r--r--   0        0        0     3858 2024-04-12 21:02:17.373462 fast_plate_ocr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14474 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.2/PKG-INFO
```

### Comparing `fast_plate_ocr-0.1.0/LICENSE` & `fast_plate_ocr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/README.md` & `fast_plate_ocr-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
 - **ONNX Runtime Inference**: **Fast** and **optimized** inference with ONNX runtime ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
 - **Model HUB**: Access to a collection of pre-trained models ready for inference 🌟
 
 ### Available Models
 
-|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                      Dataset                                                      | Accuracy<sup>[2]</sup> |              Dataset              |
-|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
-| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
+|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
+|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
+| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
 
-_<sup>[1]</sup>Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
+_<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
 _<sup>[2]</sup> Accuracy is what we refer as plate_acc. See metrics section._
 
 
 <details>
   <summary>Reproduce results.</summary>
@@ -54,21 +54,21 @@
 
   ```python
   from fast_plate_ocr import ONNXPlateRecognizer
 
   m = ONNXPlateRecognizer("argentinian-plates-cnn-model")
   m.benchmark()
   ```
-* Calculate Model accuracy
+* Calculate Model accuracy:
 
   ```shell
   pip install fast-plate-ocr[train]
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_cnn_ocr_config.yaml
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_cnn_ocr.keras
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_benchmark.zip
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_cnn_ocr_config.yaml
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_cnn_ocr.keras
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_benchmark.zip
   unzip arg_plate_benchmark.zip
   fast_plate_ocr valid \
       -m arg_cnn_ocr.keras \
       --config-file arg_cnn_ocr_config.yaml \
       --annotations benchmark/annotations.csv
   ```
 
@@ -118,14 +118,16 @@
 <details>
   <summary>benchmark demo</summary>
 
 ![Benchmark demo](https://github.com/ankandrew/fast-plate-ocr/blob/ac3d110c58f62b79072e3a7af15720bb52a45e4e/extra/benchmark_demo.gif?raw=true)
 
 </details>
 
+Make sure to check out the [docs](https://ankandrew.github.io/fast-plate-ocr) for more information.
+
 ### CLI
 
 <img src="https://github.com/ankandrew/fast-plate-ocr/blob/ac3d110c58f62b79072e3a7af15720bb52a45e4e/extra/cli_screenshot.png?raw=true" alt="CLI">
 
 To train or use the CLI tool, you'll need to install:
 
 ```shell
@@ -151,15 +153,15 @@
     pad_char: '_'
     # Image height which is fed to the model.
     img_height: 70
     # Image width which is fed to the model.
     img_width: 140
     ```
 2. A labeled dataset,
-   see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_dataset.zip)
+   see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)
    for the expected data format.
 3. Run train script:
     ```shell
     # You can set the backend to either TensorFlow, JAX or PyTorch
     # (just make sure it is installed)
     !KERAS_BACKEND=tensorflow fast_plate_ocr train \
         --annotations path_to_the_train.csv \
@@ -251,16 +253,16 @@
 	--output-path arg_cnn_ocr.onnx \
 	--opset 18 \
 	--config-file arg_cnn_ocr_config.yaml
 ```
 
 ### Keras Backend
 
-To train the model, you can install the ML Framework you like the most. Keras 3 has
-support for TensorFlow, JAX and PyTorch backends.
+To train the model, you can install the ML Framework you like the most. **Keras 3** has
+support for **TensorFlow**, **JAX** and **PyTorch** backends.
 
 To change the Keras backend you can either:
 
 1. Export `KERAS_BACKEND` environment variable, i.e. to use JAX for training:
     ```shell
     KERAS_BACKEND=jax fast_plate_ocr train --config-file ...
     ```
@@ -268,15 +270,15 @@
 
 _Note: You will probably need to install your desired framework for training._
 
 ### Model Architecture
 
 The current model architecture is quite simple but effective.
 See [cnn_ocr_model](https://github.com/ankandrew/cnn-ocr-lp/blob/e59b738bad86d269c82101dfe7a3bef49b3a77c7/fast_plate_ocr/train/model/models.py#L23-L23)
-the code.
+for implementation details.
 
 The model output consists of several heads. Each head represents the prediction of a character of the
 plate. If the plate consists of 7 characters at most (`max_plate_slots=7`), then the model would have 7 heads.
 
 Example of Argentinian plates:
 
 ![Model head](https://raw.githubusercontent.com/ankandrew/fast-plate-ocr/4a7dd34c9803caada0dc50a33b59487b63dd4754/extra/FCN.png)
@@ -293,16 +295,14 @@
   score 0.
 * **cat_acc**: Calculates how many characters of the plate were correctly classified. Example if the correct label is
   `ABC123` and `ABC133` is predicted, it will not give a precision of 0% like plate_acc (not completely
   classified correctly), but 83.3% (5/6).
 * **top_3_k**: Calculates how often the true character is found in the top-3 predictions (the 3 with the highest
   probability).
 
-_Metrics are defined in this [custom.py](fast_plate_ocr/train/model/custom.py) module._
-
 ### Contributing
 
 Contributions to the repo are greatly appreciated. Whether it's bug fixes, feature enhancements, or new models,
 your contributions are warmly welcomed.
 
 To start contributing or to begin development, you can follow these steps:
 
@@ -322,8 +322,8 @@
 If you want to train a model and share it, we'll add it to the HUB 🚀
 
 ### TODO
 
 - [ ] Expand model zoo.
 - [ ] Use synthetic image plates.
 - [ ] Finish and push TorchServe files.
-
+- [ ] Use Google docstring style
```

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/cli.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/onnx_converter.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/onnx_converter.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/train.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/train.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/valid.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/valid.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/visualize_augmentation.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/cli/visualize_predictions.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/cli/visualize_predictions.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/common/utils.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/common/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/inference/config.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/inference/hub.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 from fast_plate_ocr.inference.utils import safe_write
 
 BASE_URL: str = "https://github.com/ankandrew/cnn-ocr-lp/releases/download"
 
 AVAILABLE_ONNX_MODELS: dict[str, tuple[str, str]] = {
     "argentinian-plates-cnn-model": (
-        f"{BASE_URL}/v1.0/arg_cnn_ocr.onnx",
-        f"{BASE_URL}/v1.0/arg_cnn_ocr_config.yaml",
+        f"{BASE_URL}/arg-plates/arg_cnn_ocr.onnx",
+        f"{BASE_URL}/arg-plates/arg_cnn_ocr_config.yaml",
     )
 }
 """Available ONNX models for doing inference."""
 
 MODEL_CACHE_DIR: pathlib.Path = pathlib.Path.home() / ".cache" / "fast-plate-ocr"
 """Default location where models will be stored."""
```

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/inference/onnx_inference.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/onnx_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,29 +63,33 @@
     def __init__(
         self,
         hub_ocr_model: Literal["argentinian-plates-cnn-model"] | None = None,
         device: Literal["gpu", "cpu", "auto"] = "auto",
         sess_options: ort.SessionOptions | None = None,
         model_path: str | os.PathLike[str] | None = None,
         config_path: str | os.PathLike[str] | None = None,
-    ):
+    ) -> None:
         """
         Initializes the ONNXPlateRecognizer with the specified OCR model and inference device.
 
         The current OCR models available from the HUB are:
 
-        - 'argentinian-plates-cnn-model': OCR for Argentinian license plates.
+        - `argentinian-plates-cnn-model`: OCR for Argentinian license plates.
 
-        :param hub_ocr_model: Name of the OCR model to use from the HUB.
-        :param device: Device type for inference. Should be one of ('cpu', 'gpu', 'auto'). If
-         'auto' mode, the device will be deduced from `onnxruntime.get_available_providers()`.
-        :param sess_options: Advanced session options for ONNX Runtime.
-        :param model_path: Path to ONNX model file to use (In case you want to use a custom one).
-        :param config_path: Path to config file to use (In case you want to use a custom one).
-        :return: None.
+        Args:
+            hub_ocr_model: Name of the OCR model to use from the HUB.
+            device: Device type for inference. Should be one of ('cpu', 'gpu', 'auto'). If
+                'auto' mode, the device will be deduced from
+                `onnxruntime.get_available_providers()`.
+            sess_options: Advanced session options for ONNX Runtime.
+            model_path: Path to ONNX model file to use (In case you want to use a custom one).
+            config_path: Path to config file to use (In case you want to use a custom one).
+
+        Returns:
+            None.
         """
         self.logger = logging.getLogger(__name__)
 
         if device == "gpu":
             self.provider = ["CUDAExecutionProvider"]
         elif device == "cpu":
             self.provider = ["CPUExecutionProvider"]
@@ -115,18 +119,19 @@
         self.logger.info("Using ONNX Runtime with %s.", self.provider[0])
 
     def benchmark(self, n_iter: int = 10_000, include_processing: bool = False) -> None:
         """
         Benchmark time taken to run the OCR model. This reports the average inference time and the
         throughput in plates per second.
 
-        :param n_iter: The number of iterations to run the benchmark. This determines how many times
-         the inference will be executed to compute the average performance metrics.
-        :param include_processing: Indicates whether the benchmark should include preprocessing and
-         postprocessing times in the measurement.
+        Args:
+            n_iter: The number of iterations to run the benchmark. This determines how many times
+                the inference will be executed to compute the average performance metrics.
+            include_processing: Indicates whether the benchmark should include preprocessing and
+                postprocessing times in the measurement.
         """
         cum_time = 0.0
         x = np.random.randint(
             0, 256, size=(1, self.config["img_height"], self.config["img_width"], 1), dtype=np.uint8
         )
         for _ in range(n_iter):
             with measure_time() as time_taken:
@@ -151,22 +156,25 @@
         self,
         source: str | list[str] | npt.NDArray | list[npt.NDArray],
         return_confidence: bool = False,
     ) -> tuple[list[str], npt.NDArray] | list[str]:
         """
         Performs OCR to recognize license plate characters from an image or a list of images.
 
-        :param source: The path(s) to the image(s), a numpy array representing an image or a list
-         of NumPy arrays. If a numpy array is provided, it is expected to already be in grayscale
-         format, with shape (H, W) or (H, W, 1). A list of numpy arrays with different image sizes
-         may also be provided.
-        :param return_confidence: Whether to return confidence scores along with plate predictions.
-        :return: A list of plates for each input image. If `return_confidence` is True, a numpy
-         array is returned with the shape (N, plate_slots), where N is the batch size and each
-         plate_slot is the confidence for the recognized license plate character.
+        Args:
+            source: The path(s) to the image(s), a numpy array representing an image or a list
+                of NumPy arrays. If a numpy array is provided, it is expected to already be in
+                grayscale format, with shape `(H, W) `or `(H, W, 1)`. A list of numpy arrays with
+                different image sizes may also be provided.
+            return_confidence: Whether to return confidence scores along with plate predictions.
+
+        Returns:
+            A list of plates for each input image. If `return_confidence` is True, a numpy
+                array is returned with the shape `(N, plate_slots)`, where N is the batch size and
+                each plate slot is the confidence for the recognized license plate character.
         """
         x = _load_image_from_source(source)
         # Preprocess
         x = preprocess_image(x, self.config["img_height"], self.config["img_width"])
         # Run model
         y: list[npt.NDArray] = self.model.run(None, {"input": x})
         # Postprocess model output
```

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/inference/process.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/process.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/inference/utils.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/inference/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/data/augmentation.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/data/dataset.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/config.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/custom.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/custom.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/layer_blocks.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/layer_blocks.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/model/models.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/model/models.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/utilities/backend_utils.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/backend_utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/fast_plate_ocr/train/utilities/utils.py` & `fast_plate_ocr-0.1.2/fast_plate_ocr/train/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.0/pyproject.toml` & `fast_plate_ocr-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "fast-plate-ocr"
-version = "0.1.0"
+version = "0.1.2"
 description = "Fast & Lightweight OCR for vehicle license plates."
 authors = ["ankandrew <61120139+ankandrew@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/ankandrew/fast-plate-ocr/"
+documentation = "https://ankandrew.github.io/fast-plate-ocr"
 keywords = ["plate-recognition", "license-plate-recognition", "license-plate-ocr"]
 license = "MIT"
 classifiers = [
     "Typing :: Typed",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
@@ -43,37 +44,43 @@
 pandas = { version   = "*", optional = true }
 pydantic = { version = "^2.0.0", optional = true }
 tensorboard = { version = "*", optional = true }
 tensorflow = { version = "*", optional = true }
 tf2onnx = { version = "*", optional = true }
 torch = { version = "*", optional = true }
 
+# Optional packages for creating the docs
+mkdocs-material = { version = "*", optional = true }
+mkdocstrings = {version = "*", extras = ["python"], optional = true}
+mike = { version = "*", optional = true }
+
 [tool.poetry.extras]
 inference_gpu = ["onnxruntime-gpu"]
 train = [
     "albumentations",
     "click",
     "keras",
     "matplotlib",
     "pandas",
     "pydantic",
     "tensorboard",
     "tensorflow",
     "tf2onnx",
     "torch",
 ]
+docs = ["mkdocs-material", "mkdocstrings", "mike"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "*"
-ruff = "^0.3.1"
+ruff = "*"
 pandas-stubs = "^2.2.0.240218"
-pylint = "^3.1.0"
+pylint = "*"
 types-pyyaml = "^6.0.12.20240311"
 
 [tool.poetry.scripts]
 fast_plate_ocr = "fast_plate_ocr.cli.cli:main_cli"
 
 [tool.ruff]
 line-length = 100
```

### Comparing `fast_plate_ocr-0.1.0/PKG-INFO` & `fast_plate_ocr-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-plate-ocr
-Version: 0.1.0
+Version: 0.1.2
 Summary: Fast & Lightweight OCR for vehicle license plates.
 Home-page: https://github.com/ankandrew/fast-plate-ocr/
 License: MIT
 Keywords: plate-recognition,license-plate-recognition,license-plate-ocr
 Author: ankandrew
 Author-email: 61120139+ankandrew@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -20,33 +20,38 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Provides-Extra: docs
 Provides-Extra: inference-gpu
 Provides-Extra: train
 Requires-Dist: albumentations ; extra == "train"
 Requires-Dist: click ; extra == "train"
 Requires-Dist: keras (>=3.1.1) ; extra == "train"
 Requires-Dist: matplotlib ; extra == "train"
+Requires-Dist: mike ; extra == "docs"
+Requires-Dist: mkdocs-material ; extra == "docs"
+Requires-Dist: mkdocstrings[python] ; extra == "docs"
 Requires-Dist: numpy (>=1.17)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: onnxruntime-gpu (>=1.4.0) ; (sys_platform != "darwin") and (extra == "inference-gpu")
 Requires-Dist: opencv-python
 Requires-Dist: pandas ; extra == "train"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0) ; extra == "train"
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: rich
 Requires-Dist: tensorboard ; extra == "train"
 Requires-Dist: tensorflow ; extra == "train"
 Requires-Dist: tf2onnx ; extra == "train"
 Requires-Dist: torch ; extra == "train"
 Requires-Dist: tqdm
+Project-URL: Documentation, https://ankandrew.github.io/fast-plate-ocr
 Project-URL: Repository, https://github.com/ankandrew/fast-plate-ocr/
 Description-Content-Type: text/markdown
 
 ## Fast & Lightweight License Plate OCR
 
 [![Actions status](https://github.com/ankandrew/fast-plate-ocr/actions/workflows/main.yaml/badge.svg)](https://github.com/ankandrew/fast-plate-ocr/actions)
 [![Keras 3](https://img.shields.io/badge/Keras-3-red?logo=keras&logoColor=red&labelColor=white)](https://keras.io/keras_3/)
@@ -75,19 +80,19 @@
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
 - **ONNX Runtime Inference**: **Fast** and **optimized** inference with ONNX runtime ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
 - **Model HUB**: Access to a collection of pre-trained models ready for inference 🌟
 
 ### Available Models
 
-|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                      Dataset                                                      | Accuracy<sup>[2]</sup> |              Dataset              |
-|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
-| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
+|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
+|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
+| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
 
-_<sup>[1]</sup>Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
+_<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
 _<sup>[2]</sup> Accuracy is what we refer as plate_acc. See metrics section._
 
 
 <details>
   <summary>Reproduce results.</summary>
@@ -102,21 +107,21 @@
 
   ```python
   from fast_plate_ocr import ONNXPlateRecognizer
 
   m = ONNXPlateRecognizer("argentinian-plates-cnn-model")
   m.benchmark()
   ```
-* Calculate Model accuracy
+* Calculate Model accuracy:
 
   ```shell
   pip install fast-plate-ocr[train]
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_cnn_ocr_config.yaml
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_cnn_ocr.keras
-  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_benchmark.zip
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_cnn_ocr_config.yaml
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_cnn_ocr.keras
+  curl -LO https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_benchmark.zip
   unzip arg_plate_benchmark.zip
   fast_plate_ocr valid \
       -m arg_cnn_ocr.keras \
       --config-file arg_cnn_ocr_config.yaml \
       --annotations benchmark/annotations.csv
   ```
 
@@ -166,14 +171,16 @@
 <details>
   <summary>benchmark demo</summary>
 
 ![Benchmark demo](https://github.com/ankandrew/fast-plate-ocr/blob/ac3d110c58f62b79072e3a7af15720bb52a45e4e/extra/benchmark_demo.gif?raw=true)
 
 </details>
 
+Make sure to check out the [docs](https://ankandrew.github.io/fast-plate-ocr) for more information.
+
 ### CLI
 
 <img src="https://github.com/ankandrew/fast-plate-ocr/blob/ac3d110c58f62b79072e3a7af15720bb52a45e4e/extra/cli_screenshot.png?raw=true" alt="CLI">
 
 To train or use the CLI tool, you'll need to install:
 
 ```shell
@@ -199,15 +206,15 @@
     pad_char: '_'
     # Image height which is fed to the model.
     img_height: 70
     # Image width which is fed to the model.
     img_width: 140
     ```
 2. A labeled dataset,
-   see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/v1.0/arg_plate_dataset.zip)
+   see [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)
    for the expected data format.
 3. Run train script:
     ```shell
     # You can set the backend to either TensorFlow, JAX or PyTorch
     # (just make sure it is installed)
     !KERAS_BACKEND=tensorflow fast_plate_ocr train \
         --annotations path_to_the_train.csv \
@@ -299,16 +306,16 @@
 	--output-path arg_cnn_ocr.onnx \
 	--opset 18 \
 	--config-file arg_cnn_ocr_config.yaml
 ```
 
 ### Keras Backend
 
-To train the model, you can install the ML Framework you like the most. Keras 3 has
-support for TensorFlow, JAX and PyTorch backends.
+To train the model, you can install the ML Framework you like the most. **Keras 3** has
+support for **TensorFlow**, **JAX** and **PyTorch** backends.
 
 To change the Keras backend you can either:
 
 1. Export `KERAS_BACKEND` environment variable, i.e. to use JAX for training:
     ```shell
     KERAS_BACKEND=jax fast_plate_ocr train --config-file ...
     ```
@@ -316,15 +323,15 @@
 
 _Note: You will probably need to install your desired framework for training._
 
 ### Model Architecture
 
 The current model architecture is quite simple but effective.
 See [cnn_ocr_model](https://github.com/ankandrew/cnn-ocr-lp/blob/e59b738bad86d269c82101dfe7a3bef49b3a77c7/fast_plate_ocr/train/model/models.py#L23-L23)
-the code.
+for implementation details.
 
 The model output consists of several heads. Each head represents the prediction of a character of the
 plate. If the plate consists of 7 characters at most (`max_plate_slots=7`), then the model would have 7 heads.
 
 Example of Argentinian plates:
 
 ![Model head](https://raw.githubusercontent.com/ankandrew/fast-plate-ocr/4a7dd34c9803caada0dc50a33b59487b63dd4754/extra/FCN.png)
@@ -341,16 +348,14 @@
   score 0.
 * **cat_acc**: Calculates how many characters of the plate were correctly classified. Example if the correct label is
   `ABC123` and `ABC133` is predicted, it will not give a precision of 0% like plate_acc (not completely
   classified correctly), but 83.3% (5/6).
 * **top_3_k**: Calculates how often the true character is found in the top-3 predictions (the 3 with the highest
   probability).
 
-_Metrics are defined in this [custom.py](fast_plate_ocr/train/model/custom.py) module._
-
 ### Contributing
 
 Contributions to the repo are greatly appreciated. Whether it's bug fixes, feature enhancements, or new models,
 your contributions are warmly welcomed.
 
 To start contributing or to begin development, you can follow these steps:
 
@@ -370,9 +375,9 @@
 If you want to train a model and share it, we'll add it to the HUB 🚀
 
 ### TODO
 
 - [ ] Expand model zoo.
 - [ ] Use synthetic image plates.
 - [ ] Finish and push TorchServe files.
-
+- [ ] Use Google docstring style
```

