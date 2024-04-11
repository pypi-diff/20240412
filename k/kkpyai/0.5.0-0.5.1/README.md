# Comparing `tmp/kkpyai-0.5.0.tar.gz` & `tmp/kkpyai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.5.0.tar", max compression
+gzip compressed data, was "kkpyai-0.5.1.tar", max compression
```

## Comparing `kkpyai-0.5.0.tar` & `kkpyai-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.5.0/LICENSE
--rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.5.0/README.md
--rw-r--r--   0        0        0     9553 2024-04-11 19:25:17.524948 kkpyai-0.5.0/kkpyai/kktorch.py
--rw-r--r--   0        0        0      420 2024-04-11 19:08:10.389722 kkpyai-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 kkpyai-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.5.1/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.5.1/README.md
+-rw-r--r--   0        0        0     9541 2024-04-11 19:46:35.124583 kkpyai-0.5.1/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      420 2024-04-11 19:46:35.125843 kkpyai-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 kkpyai-0.5.1/PKG-INFO
```

### Comparing `kkpyai-0.5.0/LICENSE` & `kkpyai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.5.0/kkpyai/kktorch.py` & `kkpyai-0.5.1/kkpyai/kktorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch as tc
 import matplotlib.pyplot as plt
 import numpy as np
 
 
 # region globals
 
-def find_fastest_device():
+def find_fast_device():
     """
     - Apple Silicon uses Apple's own Metal Performance Shaders (MPS) instead of CUDA
     """
     if util.PLATFORM == 'Darwin':
         return 'mps' if tc.backends.mps.is_available() else 'cpu'
     if tc.cuda.is_available():
         return 'cuda'
@@ -31,20 +31,20 @@
 
 
 # region tensor ops
 
 class TensorFactory(Loggable):
     def __init__(self, device=None, dtype=tc.float32, requires_grad=False, logger=None):
         super().__init__(logger)
-        self.device = tc.device(device) if device else find_fastest_device()
+        self.device = tc.device(device) if device else find_fast_device()
         self.dtype = dtype
         self.requires_grad = requires_grad
 
     def init(self, device: str = '', dtype=tc.float32, requires_grad=False):
-        self.device = tc.device(device) if device else find_fastest_device()
+        self.device = tc.device(device) if device else find_fast_device()
         self.dtype = dtype
         self.requires_grad = requires_grad
 
     def ramp(self, size: typing.Union[list, tuple], start=1):
         """
         - ramp is easier to understand than random numbers
         - so they can come in handy for debugging and test-drive
@@ -92,15 +92,15 @@
 
 # region model
 
 
 class Model(Loggable):
     def __init__(self, model, lossfn_name='L1Loss', optm_name='SGD', learning_rate=0.01, device_name=None, logger=None):
         super().__init__(logger)
-        self.device = device_name or find_fastest_device()
+        self.device = device_name or find_fast_device()
         self.model = model.to(self.device)
         self.lossFunction = eval(f'tc.nn.{lossfn_name}()')
         self.optimizer = eval(f'tc.optim.{optm_name}(self.model.parameters(), lr={learning_rate})')
         self.plot = Plot()
 
     def set_lossfunction(self, lossfn_name='L1Loss'):
         """
```

