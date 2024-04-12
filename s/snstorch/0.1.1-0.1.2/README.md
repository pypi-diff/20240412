# Comparing `tmp/snstorch-0.1.1.tar.gz` & `tmp/snstorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snstorch-0.1.1.tar", last modified: Thu Feb  8 21:50:27 2024, max compression
+gzip compressed data, was "snstorch-0.1.2.tar", last modified: Fri Apr 12 20:30:54 2024, max compression
```

## Comparing `snstorch-0.1.1.tar` & `snstorch-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-02-08 21:50:27.439282 snstorch-0.1.1/
--rw-rw-r--   0 will      (1000) will      (1000)    11343 2024-01-31 00:24:02.000000 snstorch-0.1.1/LICENSE
--rw-rw-r--   0 will      (1000) will      (1000)      952 2024-02-08 21:50:27.439282 snstorch-0.1.1/PKG-INFO
--rw-rw-r--   0 will      (1000) will      (1000)       10 2023-12-21 20:42:31.000000 snstorch-0.1.1/README.md
--rw-rw-r--   0 will      (1000) will      (1000)       38 2024-02-08 21:50:27.439282 snstorch-0.1.1/setup.cfg
--rw-rw-r--   0 will      (1000) will      (1000)     1214 2024-02-08 21:49:50.000000 snstorch-0.1.1/setup.py
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-02-08 21:50:27.439282 snstorch-0.1.1/snstorch/
--rw-rw-r--   0 will      (1000) will      (1000)        0 2024-01-30 20:51:35.000000 snstorch-0.1.1/snstorch/__init__.py
--rw-rw-r--   0 will      (1000) will      (1000)     6749 2024-02-08 19:56:21.000000 snstorch-0.1.1/snstorch/modules.py
-drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-02-08 21:50:27.439282 snstorch-0.1.1/snstorch.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      952 2024-02-08 21:50:27.000000 snstorch-0.1.1/snstorch.egg-info/PKG-INFO
--rw-rw-r--   0 will      (1000) will      (1000)      226 2024-02-08 21:50:27.000000 snstorch-0.1.1/snstorch.egg-info/SOURCES.txt
--rw-rw-r--   0 will      (1000) will      (1000)        1 2024-02-08 21:50:27.000000 snstorch-0.1.1/snstorch.egg-info/dependency_links.txt
--rw-rw-r--   0 will      (1000) will      (1000)        6 2024-02-08 21:50:27.000000 snstorch-0.1.1/snstorch.egg-info/requires.txt
--rw-rw-r--   0 will      (1000) will      (1000)        9 2024-02-08 21:50:27.000000 snstorch-0.1.1/snstorch.egg-info/top_level.txt
+drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-04-12 20:30:54.562149 snstorch-0.1.2/
+-rw-rw-r--   0 will      (1000) will      (1000)    11343 2024-01-31 00:24:02.000000 snstorch-0.1.2/LICENSE
+-rw-rw-r--   0 will      (1000) will      (1000)      952 2024-04-12 20:30:54.562149 snstorch-0.1.2/PKG-INFO
+-rw-rw-r--   0 will      (1000) will      (1000)       10 2023-12-21 20:42:31.000000 snstorch-0.1.2/README.md
+-rw-rw-r--   0 will      (1000) will      (1000)       38 2024-04-12 20:30:54.562149 snstorch-0.1.2/setup.cfg
+-rw-rw-r--   0 will      (1000) will      (1000)     1214 2024-04-12 20:30:06.000000 snstorch-0.1.2/setup.py
+drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-04-12 20:30:54.562149 snstorch-0.1.2/snstorch/
+-rw-rw-r--   0 will      (1000) will      (1000)        0 2024-01-30 20:51:35.000000 snstorch-0.1.2/snstorch/__init__.py
+-rw-rw-r--   0 will      (1000) will      (1000)     7066 2024-03-01 21:23:05.000000 snstorch-0.1.2/snstorch/modules.py
+drwxrwxr-x   0 will      (1000) will      (1000)        0 2024-04-12 20:30:54.562149 snstorch-0.1.2/snstorch.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)      952 2024-04-12 20:30:54.000000 snstorch-0.1.2/snstorch.egg-info/PKG-INFO
+-rw-rw-r--   0 will      (1000) will      (1000)      226 2024-04-12 20:30:54.000000 snstorch-0.1.2/snstorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 will      (1000) will      (1000)        1 2024-04-12 20:30:54.000000 snstorch-0.1.2/snstorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 will      (1000) will      (1000)        6 2024-04-12 20:30:54.000000 snstorch-0.1.2/snstorch.egg-info/requires.txt
+-rw-rw-r--   0 will      (1000) will      (1000)        9 2024-04-12 20:30:54.000000 snstorch-0.1.2/snstorch.egg-info/top_level.txt
```

### Comparing `snstorch-0.1.1/LICENSE` & `snstorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snstorch-0.1.1/PKG-INFO` & `snstorch-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: snstorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/wnourse05/SNSTorch
 Author: William Nourse
 Author-email: nourse@case.edu
 License: Apache v2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `snstorch-0.1.1/setup.py` & `snstorch-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme_file_contents():
     with open('README.md') as f:
         data = f.read()
     return data
 
 setup(
     name='snstorch',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     url='https://github.com/wnourse05/SNSTorch',
     license='Apache v2.0',
     author='William Nourse',
     author_email='nourse@case.edu',
     description='',
     long_description='',
```

### Comparing `snstorch-0.1.1/snstorch/modules.py` & `snstorch-0.1.2/snstorch/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 import torch.nn as nn
 import torch.autograd.profiler as profiler
 import torch.jit as jit
 from typing import List
 
-class NonSpikingLayer(jit.ScriptModule):
+
+class NonSpikingLayer(nn.Module):
     def __init__(self, size, params=None, generator=None, device=None, dtype=torch.float32,
                  ):
         super().__init__()
         if device is None:
             device = 'cpu'
         self.params = nn.ParameterDict({
             'tau': nn.Parameter(torch.rand(size, dtype=dtype, generator=generator).to(device)),
@@ -16,64 +17,67 @@
             'rest': nn.Parameter(torch.zeros(size, dtype=dtype).to(device)),
             'bias': nn.Parameter(torch.rand(size, dtype=dtype, generator=generator).to(device)),
             'init': nn.Parameter(torch.rand(size, dtype=dtype, generator=generator).to(device))
         })
         if params is not None:
             self.params.update(params)
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self, x, state):
         # if state is None:
         #     state = self.params['init']
         # with profiler.record_function("NEURAL UPDATE"):
         state = state + self.params['tau'] * (-self.params['leak'] * (state - self.params['rest']) + self.params['bias'] + x)
             # state += new_state
         # if x is not None:
         #     state += self.params['tau']*x
         return state
 
-class ClampActivation(jit.ScriptModule):
+
+class ClampActivation(nn.Module):
     def __init__(self):
         super().__init__()
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self, x):
         return torch.clamp(x,0,1)
 
-class PiecewiseActivation(jit.ScriptModule):
+
+class PiecewiseActivation(nn.Module):
     def __init__(self, min_val=0, max_val=1):
         super().__init__()
         self.min_val = min_val
         self.inv_range = 1/(max_val-min_val)
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self,x):
         # with profiler.record_function("PIECEWISE SIGMOID"):
             # x -= self.min_val
             # x *= self.inv_range
             # x.clamp_(0,1)
         return torch.clamp((x - self.min_val) * self.inv_range, 0, 1)
         # return x
         # return torch.clamp((x-self.min_val)/self.range,0,1)
 
-class NonSpikingChemicalSynapseLinear(jit.ScriptModule):
+
+class NonSpikingChemicalSynapseLinear(nn.Module):
     def __init__(self, size_pre, size_post, params=None, activation=ClampActivation, device=None,
                  dtype=torch.float32, generator=None):
         super().__init__()
         if device is None:
             device = 'cpu'
         self.params = nn.ParameterDict({
             'conductance': nn.Parameter(torch.rand([size_post,size_pre],dtype=dtype, generator=generator).to(device)),
             'reversal': nn.Parameter((2*torch.rand([size_post,size_pre], generator=generator)-1).to(device))
         })
         if params is not None:
             self.params.update(params)
         self.activation = activation()
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self, state_pre, state_post):
         # with profiler.record_function("LINEAR SYNAPSE"):
         activated_pre = self.activation(state_pre)
         if state_pre.dim() > 1:
             conductance = self.params['conductance'] * activated_pre.unsqueeze(1)
         else:
             conductance = self.params['conductance'] * activated_pre
@@ -82,27 +86,33 @@
             right = state_post * torch.sum(conductance, dim=2)
         else:
             left = torch.sum(conductance * self.params['reversal'],dim=1)
             right = state_post*torch.sum(conductance,dim=1)
         out = left-right
         return out
 
-class NonSpikingChemicalSynapseConv(jit.ScriptModule):
+
+class NonSpikingChemicalSynapseConv(nn.Module):
     def __init__(self, in_channels, out_channels, kernel_size, conv_dim=2, params=None, stride=1, padding=0, dilation=1, groups=1,
                  padding_mode='zeros', device=None, dtype=None, activation=ClampActivation, generator=None):
         super().__init__()
         if conv_dim == 1:
             conv = nn.Conv1d
         elif conv_dim == 2:
             conv = nn.Conv2d
         elif conv_dim == 3:
             conv = nn.Conv3d
         else:
             raise ValueError('Convolution dimension must be 1, 2, or 3')
-
+        if device is None:
+            device = 'cpu'
+        if dtype is None:
+            dtype = torch.float32
+        self.dtype = dtype
+        self.device = device
         self.conv_left = conv(in_channels,out_channels,kernel_size, stride=stride, padding=padding, dilation=dilation,
                               groups=groups, padding_mode=padding_mode, bias=False, device=device, dtype=dtype)
         self.conv_right = conv(in_channels,out_channels,kernel_size, stride=stride, padding=padding, dilation=dilation,
                                groups=groups, padding_mode=padding_mode, bias=False, device=device, dtype=dtype)
         # remove the weights so they don't show up when calling parameters()
         shape = self.conv_right.weight.shape
         # del self.conv_left.weight
@@ -110,41 +120,47 @@
 
         self.params = nn.ParameterDict({
             'conductance': nn.Parameter(torch.randn(shape, generator=generator, dtype=dtype).to(device)),
             'reversal': nn.Parameter((2*torch.randn(shape, generator=generator, dtype=dtype)-1).to(device))
         })
         if params is not None:
             self.params.update(params)
-        conductance = torch.clamp(self.params['conductance'], min=0)
-        left = torch.zeros(shape, dtype=dtype, device=device)
-        right = torch.zeros(shape, dtype=dtype, device=device)
-        left[0,0,:,:] = (conductance * self.params['reversal']).to(device)
-        right[0,0,:,:] = conductance
-        self.conv_left.weight.data = nn.Parameter(left.to(device))
-        self.conv_right.weight.data = nn.Parameter(right.to(device))
+        self.setup()
+
         self.act = activation()
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self,x, state_post):
         # with profiler.record_function("CONV SYNAPSE"):
         x_unsqueezed = self.act(x).unsqueeze(0).unsqueeze(0)
         out = self.conv_left(x_unsqueezed) - self.conv_right(x_unsqueezed)*state_post
         return out
 
-class NonSpikingChemicalSynapseElementwise(jit.ScriptModule):
+    def setup(self):
+        conductance = torch.clamp(self.params['conductance'], min=0)
+        shape = self.conv_right.weight.shape
+        left = torch.zeros(shape, dtype=self.dtype, device=self.device)
+        right = torch.zeros(shape, dtype=self.dtype, device=self.device)
+        left[0, 0, :, :] = (conductance * self.params['reversal']).to(self.device)
+        right[0, 0, :, :] = conductance
+        self.conv_left.weight.data = nn.Parameter(left.to(self.device), requires_grad=False)
+        self.conv_right.weight.data = nn.Parameter(right.to(self.device), requires_grad=False)
+
+
+class NonSpikingChemicalSynapseElementwise(nn.Module):
     def __init__(self, params=None, device=None, dtype=torch.float32, generator=None, activation=ClampActivation()):
         super().__init__()
         if device is None:
             device = 'cpu'
         self.act = activation
         self.params = nn.ParameterDict({
             'conductance': nn.Parameter(torch.rand(1, device=device, dtype=dtype, generator=generator).to(device)),
             'reversal': nn.Parameter(2*torch.rand(1, device=device, dtype=dtype, generator=generator).to(device)-1)
         })
         if params is not None:
             self.params.update(params)
 
-    @jit.script_method
+    # @jit.script_method
     def forward(self, x, state_post):
         # with profiler.record_function("ELEMENTWISE SYNAPSE"):
         out = self.params['conductance']*self.act(x) * (self.params['reversal'] - state_post)
         return out
```

### Comparing `snstorch-0.1.1/snstorch.egg-info/PKG-INFO` & `snstorch-0.1.2/snstorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: snstorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/wnourse05/SNSTorch
 Author: William Nourse
 Author-email: nourse@case.edu
 License: Apache v2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

