# Comparing `tmp/neurobench-1.0.2.tar.gz` & `tmp/neurobench-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurobench-1.0.2.tar", max compression
+gzip compressed data, was "neurobench-1.0.3.tar", max compression
```

## Comparing `neurobench-1.0.2.tar` & `neurobench-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11357 2024-01-15 21:04:23.558633 neurobench-1.0.2/LICENSE
--rw-r--r--   0        0        0     7378 2024-01-26 16:43:52.081333 neurobench-1.0.2/README.rst
--rw-r--r--   0        0        0        0 2024-01-15 21:04:23.558989 neurobench-1.0.2/neurobench/__init__.py
--rw-r--r--   0        0        0       24 2024-01-15 21:04:23.559368 neurobench-1.0.2/neurobench/benchmarks/__init__.py
--rw-r--r--   0        0        0     5374 2024-01-24 16:02:08.536075 neurobench-1.0.2/neurobench/benchmarks/benchmark.py
--rw-r--r--   0        0        0     3028 2024-01-24 16:02:08.536189 neurobench-1.0.2/neurobench/benchmarks/hooks.py
--rw-r--r--   0        0        0     4806 2024-01-24 16:02:08.536564 neurobench-1.0.2/neurobench/benchmarks/static_metrics.py
--rw-r--r--   0        0        0    13202 2024-01-24 16:02:08.536815 neurobench-1.0.2/neurobench/benchmarks/workload_metrics.py
--rw-r--r--   0        0        0     5272 2024-01-24 16:02:08.537002 neurobench-1.0.2/neurobench/datasets/MSWC_IncrementalLoader.py
--rw-r--r--   0        0        0    10645 2024-01-26 16:43:54.374415 neurobench-1.0.2/neurobench/datasets/MSWC_dataset.py
--rw-r--r--   0        0        0     3779 2024-01-24 16:02:08.537550 neurobench-1.0.2/neurobench/datasets/WISDM.py
--rw-r--r--   0        0        0     1012 2024-01-24 16:02:08.537977 neurobench-1.0.2/neurobench/datasets/__init__.py
--rw-r--r--   0        0        0      804 2024-01-15 21:04:23.560148 neurobench-1.0.2/neurobench/datasets/dataset.py
--rw-r--r--   0        0        0     9971 2024-01-24 16:02:08.538146 neurobench-1.0.2/neurobench/datasets/dvs_gesture.py
--rw-r--r--   0        0        0     8977 2024-01-24 16:02:08.538788 neurobench-1.0.2/neurobench/datasets/mackey_glass.py
--rw-r--r--   0        0        0     6433 2024-01-24 16:02:08.539400 neurobench-1.0.2/neurobench/datasets/megapixel_automotive.py
--rw-r--r--   0        0        0    13242 2024-01-24 16:02:08.539992 neurobench-1.0.2/neurobench/datasets/primate_reaching.py
--rw-r--r--   0        0        0     2488 2024-01-24 16:02:08.540344 neurobench-1.0.2/neurobench/datasets/speech_commands.py
--rw-r--r--   0        0        0     5298 2024-01-24 16:02:08.540481 neurobench-1.0.2/neurobench/datasets/utils.py
--rw-r--r--   0        0        0      316 2024-01-15 21:04:23.564739 neurobench-1.0.2/neurobench/models/__init__.py
--rw-r--r--   0        0        0     4052 2024-01-24 16:02:09.338292 neurobench-1.0.2/neurobench/models/model.py
--rw-r--r--   0        0        0     1687 2024-01-24 16:02:09.338690 neurobench-1.0.2/neurobench/models/snntorch_models.py
--rw-r--r--   0        0        0      821 2024-01-24 16:02:09.338988 neurobench-1.0.2/neurobench/models/torch_model.py
--rw-r--r--   0        0        0        0 2024-01-24 16:02:09.339052 neurobench-1.0.2/neurobench/models/utils.py
--rw-r--r--   0        0        0       28 2024-01-24 16:02:09.339275 neurobench-1.0.2/neurobench/postprocessing/__init__.py
--rw-r--r--   0        0        0     1557 2024-01-24 16:02:09.339454 neurobench-1.0.2/neurobench/postprocessing/postprocessor.py
--rw-r--r--   0        0        0      344 2024-01-24 16:02:09.339889 neurobench-1.0.2/neurobench/preprocessing/__init__.py
--rw-r--r--   0        0        0     3056 2024-01-24 16:02:09.340501 neurobench-1.0.2/neurobench/preprocessing/mfcc.py
--rw-r--r--   0        0        0      876 2024-01-24 16:02:09.340964 neurobench-1.0.2/neurobench/preprocessing/preprocessor.py
--rw-r--r--   0        0        0     5949 2024-01-24 16:02:09.341536 neurobench-1.0.2/neurobench/preprocessing/speech2spikes.py
--rw-r--r--   0        0        0    11752 2024-01-24 16:02:09.341912 neurobench-1.0.2/neurobench/utils.py
--rw-r--r--   0        0        0     1061 2024-01-26 18:03:39.978772 neurobench-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 neurobench-1.0.2/setup.py
--rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 neurobench-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-15 21:04:23.558633 neurobench-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7378 2024-03-04 19:47:02.911313 neurobench-1.0.3/README.rst
+-rw-r--r--   0        0        0        0 2024-01-15 21:04:23.558989 neurobench-1.0.3/neurobench/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-12 15:27:09.486417 neurobench-1.0.3/neurobench/benchmarks/__init__.py
+-rw-r--r--   0        0        0     6585 2024-04-12 15:27:09.486824 neurobench-1.0.3/neurobench/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     3005 2024-04-12 15:27:09.487120 neurobench-1.0.3/neurobench/benchmarks/hooks.py
+-rw-r--r--   0        0        0     4845 2024-04-12 15:27:09.487487 neurobench-1.0.3/neurobench/benchmarks/static_metrics.py
+-rw-r--r--   0        0        0    13711 2024-04-12 15:27:09.487832 neurobench-1.0.3/neurobench/benchmarks/workload_metrics.py
+-rw-r--r--   0        0        0     5704 2024-04-12 15:27:09.488252 neurobench-1.0.3/neurobench/datasets/MSWC_IncrementalLoader.py
+-rw-r--r--   0        0        0    11325 2024-04-12 15:27:09.488613 neurobench-1.0.3/neurobench/datasets/MSWC_dataset.py
+-rw-r--r--   0        0        0     3773 2024-04-12 15:27:09.488852 neurobench-1.0.3/neurobench/datasets/WISDM.py
+-rw-r--r--   0        0        0     1088 2024-04-12 15:27:09.489528 neurobench-1.0.3/neurobench/datasets/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-12 15:27:09.490179 neurobench-1.0.3/neurobench/datasets/dataset.py
+-rw-r--r--   0        0        0    10055 2024-04-12 15:27:09.490468 neurobench-1.0.3/neurobench/datasets/dvs_gesture.py
+-rw-r--r--   0        0        0     9110 2024-04-12 15:27:09.490732 neurobench-1.0.3/neurobench/datasets/mackey_glass.py
+-rw-r--r--   0        0        0     6501 2024-04-12 15:27:09.491234 neurobench-1.0.3/neurobench/datasets/megapixel_automotive.py
+-rw-r--r--   0        0        0    13965 2024-04-12 15:27:09.491549 neurobench-1.0.3/neurobench/datasets/primate_reaching.py
+-rw-r--r--   0        0        0     2705 2024-04-12 15:27:09.492250 neurobench-1.0.3/neurobench/datasets/speech_commands.py
+-rw-r--r--   0        0        0     5469 2024-04-12 15:27:09.492651 neurobench-1.0.3/neurobench/datasets/utils.py
+-rw-r--r--   0        0        0      346 2024-04-12 15:27:09.496469 neurobench-1.0.3/neurobench/models/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-12 15:27:09.496822 neurobench-1.0.3/neurobench/models/model.py
+-rw-r--r--   0        0        0     1674 2024-04-12 15:27:09.497247 neurobench-1.0.3/neurobench/models/snntorch_models.py
+-rw-r--r--   0        0        0      818 2024-04-12 15:27:09.497877 neurobench-1.0.3/neurobench/models/torch_model.py
+-rw-r--r--   0        0        0        0 2024-01-24 16:02:09.339052 neurobench-1.0.3/neurobench/models/utils.py
+-rw-r--r--   0        0        0       29 2024-04-12 15:27:09.498538 neurobench-1.0.3/neurobench/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-12 15:27:09.498864 neurobench-1.0.3/neurobench/postprocessing/postprocessor.py
+-rw-r--r--   0        0        0      374 2024-04-12 15:27:09.499414 neurobench-1.0.3/neurobench/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-12 15:27:09.500043 neurobench-1.0.3/neurobench/preprocessing/mfcc.py
+-rw-r--r--   0        0        0      952 2024-04-12 15:27:09.500718 neurobench-1.0.3/neurobench/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0     6655 2024-04-12 15:27:09.501175 neurobench-1.0.3/neurobench/preprocessing/speech2spikes.py
+-rw-r--r--   0        0        0    12063 2024-04-12 15:27:09.501569 neurobench-1.0.3/neurobench/utils.py
+-rw-r--r--   0        0        0     1115 2024-04-12 15:28:56.137992 neurobench-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 neurobench-1.0.3/setup.py
+-rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 neurobench-1.0.3/PKG-INFO
```

### Comparing `neurobench-1.0.2/LICENSE` & `neurobench-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.2/README.rst` & `neurobench-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.2/neurobench/benchmarks/benchmark.py` & `neurobench-1.0.3/neurobench/benchmarks/benchmark.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,107 @@
 import sys
 from contextlib import redirect_stdout
 from tqdm import tqdm
 
 from . import static_metrics, workload_metrics
 
-class Benchmark():
-    """ Top-level benchmark class for running benchmarks.
-    """
+# workload metrics which require hooks
+requires_hooks = ["activation_sparsity", "number_neuron_updates", "synaptic_operations"]
+
+
+class Benchmark:
+    """Top-level benchmark class for running benchmarks."""
+
     def __init__(self, model, dataloader, preprocessors, postprocessors, metric_list):
         """
         Args:
             model: A NeuroBenchModel.
             dataloader: A PyTorch DataLoader.
             preprocessors: A list of NeuroBenchPreProcessors.
             postprocessors: A list of NeuroBenchPostProcessors.
-            metric_list: A list of lists of strings of metrics to run. 
+            metric_list: A list of lists of strings of metrics to run.
                 First item is static metrics, second item is data metrics.
         """
 
-        self.model = model 
-        self.dataloader = dataloader # dataloader not dataset
+        self.model = model
+        self.dataloader = dataloader  # dataloader not dataset
         self.preprocessors = preprocessors
         self.postprocessors = postprocessors
 
         self.static_metrics = {m: getattr(static_metrics, m) for m in metric_list[0]}
-        self.workload_metrics = {m: getattr(workload_metrics, m) for m in metric_list[1]}
-
-    def run(self, quiet=False, verbose: bool = False, 
-            dataloader=None, preprocessors=None, postprocessors=None):
-        """ Runs batched evaluation of the benchmark.
+        self.workload_metrics = {
+            m: getattr(workload_metrics, m) for m in metric_list[1]
+        }
+
+    def run(
+        self,
+        quiet=False,
+        verbose: bool = False,
+        dataloader=None,
+        preprocessors=None,
+        postprocessors=None,
+        device=None,
+    ):
+        """
+        Runs batched evaluation of the benchmark.
 
         Args:
             dataloader (optional): override DataLoader for this run.
             preprocessors (optional): override preprocessors for this run.
             postprocessors (optional): override postprocessors for this run.
             quiet (bool, default=False): If True, output is suppressed.
             verbose (bool, default=False): If True, metrics for each bach will be printed.
                                            If False (default), metrics are accumulated and printed after all batches are processed.
+            device (optional): use device for this run (e.g. 'cuda' or 'cpu').
 
         Returns:
             results: A dictionary of results.
+
         """
         with redirect_stdout(None if quiet else sys.stdout):
             print("Running benchmark")
 
             # Static metrics
             results = {}
             for m in self.static_metrics.keys():
                 results[m] = self.static_metrics[m](self.model)
 
             # add hooks to the model
-            workload_metrics.detect_activations_connections(self.model)
+            if any([m in requires_hooks for m in self.workload_metrics.keys()]):
+                workload_metrics.detect_activations_connections(self.model)
 
             dataloader = dataloader if dataloader is not None else self.dataloader
-            preprocessors = preprocessors if preprocessors is not None else self.preprocessors
-            postprocessors = postprocessors if postprocessors is not None else self.postprocessors
+            preprocessors = (
+                preprocessors if preprocessors is not None else self.preprocessors
+            )
+            postprocessors = (
+                postprocessors if postprocessors is not None else self.postprocessors
+            )
 
             # Init/re-init stateful data metrics
             for m in self.workload_metrics.keys():
-                if isinstance(self.workload_metrics[m],type) and issubclass(self.workload_metrics[m], workload_metrics.AccumulatedMetric):
+                if isinstance(self.workload_metrics[m], type) and issubclass(
+                    self.workload_metrics[m], workload_metrics.AccumulatedMetric
+                ):
                     self.workload_metrics[m] = self.workload_metrics[m]()
-                elif isinstance(self.workload_metrics[m], workload_metrics.AccumulatedMetric): # new benchmark run, reset metric state
+                elif isinstance(
+                    self.workload_metrics[m], workload_metrics.AccumulatedMetric
+                ):  # new benchmark run, reset metric state
                     self.workload_metrics[m].reset()
 
             dataset_len = len(dataloader.dataset)
 
+            if device is not None:
+                self.model.net.to(device)
+
             batch_num = 0
             for data in tqdm(dataloader, total=len(dataloader), disable=quiet):
+                if device is not None:
+                    data = (data[0].to(device), data[1].to(device))
+
                 batch_size = data[0].size(0)
 
                 # convert data to tuple
                 if type(data) is not tuple:
                     data = tuple(data)
 
                 # Preprocessing data
@@ -86,36 +117,54 @@
                 # Data metrics
                 batch_results = {}
                 for m in self.workload_metrics.keys():
                     batch_results[m] = self.workload_metrics[m](self.model, preds, data)
 
                 for m, v in batch_results.items():
                     # AccumulatedMetrics are computed after all batches complete
-                    if isinstance(self.workload_metrics[m], workload_metrics.AccumulatedMetric):
+                    if isinstance(
+                        self.workload_metrics[m], workload_metrics.AccumulatedMetric
+                    ):
                         continue
                     # otherwise accumulate via mean
                     else:
-                        assert isinstance(v, float) or isinstance(v, int), "Data metric must return float or int to be accumulated"
+                        assert isinstance(v, float) or isinstance(
+                            v, int
+                        ), "Data metric must return float or int to be accumulated"
                         if m not in results:
                             results[m] = v * batch_size / dataset_len
                         else:
                             results[m] += v * batch_size / dataset_len
 
                 # delete hook contents
                 self.model.reset_hooks()
 
                 if verbose:
                     for m in self.workload_metrics.keys():
-                        if isinstance(self.workload_metrics[m], workload_metrics.AccumulatedMetric):
+                        if isinstance(
+                            self.workload_metrics[m], workload_metrics.AccumulatedMetric
+                        ):
                             results[m] = self.workload_metrics[m].compute()
-                    print(f'\nBatch num {batch_num + 1}/{len(dataloader)}')
+                    print(f"\nBatch num {batch_num + 1}/{len(dataloader)}")
                     print(results)
 
                 batch_num += 1
 
             # compute AccumulatedMetrics after all batches if they are not calculated at every iteration
             if not verbose:
                 for m in self.workload_metrics.keys():
-                    if isinstance(self.workload_metrics[m], workload_metrics.AccumulatedMetric):
+                    if isinstance(
+                        self.workload_metrics[m], workload_metrics.AccumulatedMetric
+                    ):
                         results[m] = self.workload_metrics[m].compute()
 
+        # close hooks
+        for hook in self.model.activation_hooks:
+            hook.reset()
+            hook.close()
+        for hook in self.model.connection_hooks:
+            hook.reset()
+            hook.close()
+        self.model.activation_hooks = []
+        self.model.connection_hooks = []
+
         return results
```

### Comparing `neurobench-1.0.2/neurobench/benchmarks/hooks.py` & `neurobench-1.0.3/neurobench/benchmarks/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,88 +1,96 @@
 import snntorch as snn
-class ActivationHook():
-    """ Hook class for an activation layer in a NeuroBenchModel.
+
+
+class ActivationHook:
+    """
+    Hook class for an activation layer in a NeuroBenchModel.
 
     Output of the activation layer in each forward pass will be stored.
+
     """
 
     def __init__(self, layer, connection_layer=None, prev_act_layer_hook=None):
-        """ Initializes the class.
-        
+        """
+        Initializes the class.
+
         A forward hook is registered for the activation layer.
 
         Args:
             layer: The activation layer which is a PyTorch nn.Module.
+
         """
         self.activation_outputs = []
         self.activation_inputs = []
         if layer is not None:
             self.hook = layer.register_forward_hook(self.hook_fn)
             self.hook_pre = layer.register_forward_pre_hook(self.pre_hook_fn)
         else:
             self.hook = None
             self.hook_pre = None
 
-        self.layer = layer # the activation layer
-  
+        self.layer = layer  # the activation layer
+
         # Check if the layer is a spiking layer (SpikingNeuron is the superclass of all snnTorch spiking layers)
         self.spiking = isinstance(layer, snn.SpikingNeuron)
 
     def pre_hook_fn(self, layer, input):
-        """Hook function that will be called before each forward pass of 
-        the activation layer.
+        """
+        Hook function that will be called before each forward pass of the activation
+        layer.
 
-        Each input of the activation layer will be stored. 
+        Each input of the activation layer will be stored.
 
         Args:
-            layer: The registered layer 
+            layer: The registered layer
             input: Input of the registered layer
+
         """
         self.activation_inputs.append(input)
 
     def hook_fn(self, layer, input, output):
-        """Hook function that will be called after each forward pass of 
-        the activation layer.
+        """
+        Hook function that will be called after each forward pass of the activation
+        layer.
 
-        Each output of the activation layer will be stored. 
+        Each output of the activation layer will be stored.
 
         Args:
-            layer: The registered layer 
+            layer: The registered layer
             input: Input of the registered layer
             output: Output of the registered layer
+
         """
         if self.spiking:
             self.activation_outputs.append(output[0])
-            
 
         else:
             self.activation_outputs.append(output)
+
     def empty_hook(self):
-        """Deletes the contents of the hooks, but keeps the hook registered.
-        """
+        """Deletes the contents of the hooks, but keeps the hook registered."""
         self.activation_outputs = []
         self.activation_inputs = []
 
     def reset(self):
-        """ Resets the stored activation outputs and inputs
-        """
+        """Resets the stored activation outputs and inputs."""
         self.activation_outputs = []
         self.activation_inputs = []
 
     def close(self):
-        """ Remove the registered hook.
-        """
+        """Remove the registered hook."""
         if self.hook:
             self.hook.remove()
         if self.hook_pre:
             self.hook_pre.remove()
 
-class LayerHook():
+
+class LayerHook:
     def __init__(self, layer) -> None:
-        self.layer = layer 
+        self.layer = layer
         self.inputs = []
         if layer is not None:
             self.hook = layer.register_forward_pre_hook(self.hook_fn)
         else:
             self.hook = None
 
     def hook_fn(self, module, input):
```

### Comparing `neurobench-1.0.2/neurobench/benchmarks/static_metrics.py` & `neurobench-1.0.3/neurobench/benchmarks/static_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 import torch
 import snntorch as snn
+
 # static metrics, only require model
 
+
 def parameter_count(model):
-    """ Number of parameters in the model.
+    """
+    Number of parameters in the model.
 
     Args:
         model: A NeuroBenchModel.
     Returns:
         int: Number of parameters.
+
     """
     return sum(p.numel() for p in model.__net__().parameters())
 
+
 def footprint(model):
-    """ Memory footprint of the model.
+    """
+    Memory footprint of the model.
 
     Args:
         model: A NeuroBenchModel.
     Returns:
         float: Model size in bytes.
+
     """
     # Count the number of parameters and multiply by the size of each parameter in bytes
     param_size = 0
     for param in model.__net__().parameters():
         param_size += param.numel() * param.element_size()
 
     # Count the number of buffers and multiply by the size of each buffer in bytes
     buffer_size = 0
     for buffer in model.__net__().buffers():
         buffer_size += buffer.numel() * buffer.element_size()
 
     # Return the sum of the parameters and buffers
     return param_size + buffer_size
 
+
 def connection_sparsity(model):
-    """ Sparsity of model connections between layers. Based on number of zeros 
+    """Sparsity of model connections between layers. Based on number of zeros
     in supported layers, other layers are not taken into account in the computation:
     Supported layers:
     Linear
     Conv1d, Conv2d, Conv3d
     RNN, RNNBase, RNNCell
     LSTM, LSTMBase, LSTMCell
     GRU, GRUBase, GRUCell
@@ -46,89 +54,96 @@
     Args:
         model: A NeuroBenchModel.
     Returns:
         float: Connection sparsity, rounded to 3 decimals.
     """
 
     def get_nr_zeros_weights(module):
-        """ Get the number of zeros in a module's weights.
+        """
+        Get the number of zeros in a module's weights.
 
         Args:
             module: A torch.nn.Module.
         Returns:
             int: Number of zeros in the module's weights.
+
         """
         children = list(module.children())
-        regular_layers = (torch.nn.Linear, torch.nn.Conv1d, torch.nn.Conv2d, torch.nn.Conv3d)
-        recurr_layers  = (torch.nn.RNNBase)
-        recurr_cells   = (torch.nn.RNNCellBase)
-        if len(children) == 0: # it is a leaf
+        regular_layers = (
+            torch.nn.Linear,
+            torch.nn.Conv1d,
+            torch.nn.Conv2d,
+            torch.nn.Conv3d,
+        )
+        recurr_layers = torch.nn.RNNBase
+        recurr_cells = torch.nn.RNNCellBase
+        if len(children) == 0:  # it is a leaf
             # print(module)
             if isinstance(module, regular_layers):
                 count_zeros = torch.sum(module.weight == 0)
                 count_weights = module.weight.numel()
                 return count_zeros, count_weights
-            
+
             elif isinstance(module, recurr_layers):
                 attribute_names = []
-                for i in range(module.num_layers): 
-                    param_names = ['weight_ih_l{}{}', 'weight_hh_l{}{}']
+                for i in range(module.num_layers):
+                    param_names = ["weight_ih_l{}{}", "weight_hh_l{}{}"]
                     if module.bias:
-                        param_names += ['bias_ih_l{}{}', 'bias_hh_l{}{}']
-                    if module.proj_size > 0: # it is lstm
-                        param_names += ['weight_hr_l{}{}']
+                        param_names += ["bias_ih_l{}{}", "bias_hh_l{}{}"]
+                    if module.proj_size > 0:  # it is lstm
+                        param_names += ["weight_hr_l{}{}"]
 
-                    attribute_names += [x.format(i, '') for x in param_names]
+                    attribute_names += [x.format(i, "") for x in param_names]
                     if module.bidirectional:
-                        suffix = '_reverse'
+                        suffix = "_reverse"
                         attribute_names += [x.format(i, suffix) for x in param_names]
 
                 count_zeros = 0
                 count_weights = 0
                 for attr in attribute_names:
                     attr_val = getattr(module, attr)
                     count_zeros += torch.sum(attr_val == 0)
-                    count_weights += attr_val.numel() 
+                    count_weights += attr_val.numel()
 
                 return count_zeros, count_weights
-            
+
             elif isinstance(module, recurr_cells):
-                attribute_names = ['weight_ih', 'weight_hh']
+                attribute_names = ["weight_ih", "weight_hh"]
                 if module.bias:
-                    attribute_names += ['bias_ih', 'bias_hh']
-   
+                    attribute_names += ["bias_ih", "bias_hh"]
+
                 count_zeros = 0
                 count_weights = 0
                 for attr in attribute_names:
                     attr_val = getattr(module, attr)
                     count_zeros += torch.sum(attr_val == 0)
-                    count_weights += attr_val.numel() 
+                    count_weights += attr_val.numel()
 
                 return count_zeros, count_weights
 
             elif isinstance(module, snn.SpikingNeuron):
-                return 0, 0 # it is a neuromorphic neuron layer
+                return 0, 0  # it is a neuromorphic neuron layer
             else:
                 # print('Module type: ', module, 'not found.')
-                return 0,0
-        
+                return 0, 0
+
         else:
             count_zeros = 0
             count_weights = 0
             for child in children:
                 child_zeros, child_weights = get_nr_zeros_weights(child)
                 count_zeros += child_zeros
                 count_weights += child_weights
             return count_zeros, count_weights
+
     # Pull the layers from the model's network
     layers = model.__net__().children()
     # For each layer, count where the weights are zero
     count_zeros = 0
     count_weights = 0
     for module in layers:
         zeros, weights = get_nr_zeros_weights(module)
         count_zeros += zeros
         count_weights += weights
 
     # Return the ratio of zeros to weights, rounded to 4 decimals
     return round((count_zeros / count_weights).item(), 4)
-
```

### Comparing `neurobench-1.0.2/neurobench/benchmarks/workload_metrics.py` & `neurobench-1.0.3/neurobench/benchmarks/workload_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,341 +1,399 @@
 import torch
 import numpy as np
 from ..utils import check_shape, make_binary_copy, single_layer_MACs
 from .hooks import ActivationHook, LayerHook
 
+
 class AccumulatedMetric:
-    """ Abstract class for a metric which must save state between batches.
-    """
+    """Abstract class for a metric which must save state between batches."""
 
     def __init__(self):
-        """ Initialize metric.
-        """
-        raise NotImplementedError("Subclasses of AccumulatedMetric should implement __init__")
-    
+        """Initialize metric."""
+        raise NotImplementedError(
+            "Subclasses of AccumulatedMetric should implement __init__"
+        )
+
     def __call__(self, model, preds, data):
-        """ Process this batch of data.
+        """
+        Process this batch of data.
 
         Args:
             model: A NeuroBenchModel.
             preds: A torch tensor of model predictions.
             data: A tuple of data and labels.
         Returns:
             result: the accumulated metric as of this batch.
+
         """
-        raise NotImplementedError("Subclasses of AccumulatedMetric should implement __call__")
+        raise NotImplementedError(
+            "Subclasses of AccumulatedMetric should implement __call__"
+        )
 
     def compute(self):
-        """ Compute the metric score using all accumulated data.
+        """
+        Compute the metric score using all accumulated data.
 
         Returns:
             result: the final accumulated metric.
+
         """
-        raise NotImplementedError("Subclasses of AccumulatedMetric should implement compute")
+        raise NotImplementedError(
+            "Subclasses of AccumulatedMetric should implement compute"
+        )
 
     def reset(self):
-        """ Reset the metric state.
+        """
+        Reset the metric state.
+
+        This is called when the benchmark is run again, e.g. on the FSCIL task the
+        benchmark     is run at the end of each session.
 
-        This is called when the benchmark is run again, e.g. on the FSCIL task the benchmark
-            is run at the end of each session.
         """
-        raise NotImplementedError("Subclasses of AccumulatedMetric should implement reset")
+        raise NotImplementedError(
+            "Subclasses of AccumulatedMetric should implement reset"
+        )
 
 
 # dynamic metrics, require model, model predictions, and labels
 
+
 def detect_activations_connections(model):
-    """Register hooks or other operations that should be called before running a benchmark.
-    """
+    """Register hooks or other operations that should be called before running a
+    benchmark."""
     for hook in model.activation_hooks:
         hook.reset()
         hook.close()
     for hook in model.connection_hooks:
         hook.reset()
         hook.close()
     model.activation_hooks = []
     model.connection_hooks = []
-    
+
     supported_layers = model.supported_layers
-    
+
     # recurrent_supported_layers = (torch.nn.RNNBase)
     # recurr_cell_supported_layers = (torch.nn.RNNCellBase)
 
     act_layers = model.activation_layers()
     # Registered activation hooks
     for layer in act_layers:
         model.activation_hooks.append(ActivationHook(layer))
 
     con_layers = model.connection_layers()
     for flat_layer in con_layers:
         if isinstance(flat_layer, supported_layers):
             model.connection_hooks.append(LayerHook(flat_layer))
 
-    
 
 def activation_sparsity(model, preds, data):
-    """ Sparsity of model activations.
-    
+    """
+    Sparsity of model activations.
+
     Calculated as the number of zero activations over the total number
     of activations, over all layers, timesteps, samples in data.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
         data: A tuple of data and labels.
     Returns:
         float: Activation sparsity.
+
     """
     # TODO: for a spiking model, based on number of spikes over all timesteps over all samples from all layers
     #       Standard FF ANN depends on activation function, ReLU can introduce sparsity.
     total_spike_num, total_neuro_num = 0, 0
     for hook in model.activation_hooks:
-        for spikes in hook.activation_outputs:  # do we need a function rather than a member
-            spike_num, neuro_num = torch.count_nonzero(spikes).item(), torch.numel(spikes)
+        for (
+            spikes
+        ) in hook.activation_outputs:  # do we need a function rather than a member
+            spike_num, neuro_num = torch.count_nonzero(spikes).item(), torch.numel(
+                spikes
+            )
             total_spike_num += spike_num
             total_neuro_num += neuro_num
 
-    sparsity = (total_neuro_num - total_spike_num) / total_neuro_num if total_neuro_num != 0 else 0.0
+    sparsity = (
+        (total_neuro_num - total_spike_num) / total_neuro_num
+        if total_neuro_num != 0
+        else 0.0
+    )
     return sparsity
-    
+
+
 def number_neuron_updates(model, preds, data):
-    """ Number of times each neuron type is updated.
+    """
+    Number of times each neuron type is updated.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
         data: A tuple of data and labels.
     Returns:
         dict: key is neuron type, value is number of updates.
+
     """
     # check_shape(preds, data[1])
-    macs = 0
 
     update_dict = {}
-    for hook in model.activation_hooks: 
-        for spikes_batch in hook.activation_inputs:  
-            for spikes in spikes_batch: 
-                nr_updates = torch.count_nonzero(spikes) 
+    for hook in model.activation_hooks:
+        for spikes_batch in hook.activation_inputs:
+            for spikes in spikes_batch:
+                nr_updates = torch.count_nonzero(spikes)
                 if str(type(hook.layer)) not in update_dict:
                     update_dict[str(type(hook.layer))] = 0
                 update_dict[str(type(hook.layer))] += int(nr_updates)
     # print formatting
-    print('Number of updates for:')
+    print("Number of updates for:")
     for key in update_dict:
-        print(key, ':',update_dict[key])
+        print(key, ":", update_dict[key])
     return update_dict
 
+
 def classification_accuracy(model, preds, data):
-    """ Classification accuracy of the model predictions.
+    """
+    Classification accuracy of the model predictions.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
         data: A tuple of data and labels.
     Returns:
         float: Classification accuracy.
+
     """
     check_shape(preds, data[1])
     equal = torch.eq(preds, data[1])
     return torch.mean(equal.float()).item()
 
+
 def MSE(model, preds, data):
-    """ Mean squared error of the model predictions.
+    """
+    Mean squared error of the model predictions.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
         data: A tuple of data and labels.
     Returns:
         float: Mean squared error.
+
     """
     check_shape(preds, data[1])
-    return torch.mean((preds - data[1])**2).item()
+    return torch.mean((preds - data[1]) ** 2).item()
+
 
 def sMAPE(model, preds, data):
-    """ Symmetric mean absolute percentage error of the model predictions.
+    """
+    Symmetric mean absolute percentage error of the model predictions.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
         data: A tuple of data and labels.
     Returns:
         float: Symmetric mean absolute percentage error.
+
     """
     check_shape(preds, data[1])
-    smape = 200*torch.mean(torch.abs(preds - data[1])/(torch.abs(preds)+torch.abs(data[1])))
+    smape = 200 * torch.mean(
+        torch.abs(preds - data[1]) / (torch.abs(preds) + torch.abs(data[1]))
+    )
     return torch.nan_to_num(smape, nan=200.0).item()
 
+
 class synaptic_operations(AccumulatedMetric):
-    """ Number of synaptic operations 
-    
-    MACs for ANN
-    ACs for SNN
+    """
+    Number of synaptic operations.
+
+    MACs for ANN ACs for SNN
+
     """
 
     def __init__(self):
         self.MAC = 0
-        self.AC  = 0
+        self.AC = 0
         self.total_synops = 0
         self.total_samples = 0
 
     def reset(self):
         self.MAC = 0
-        self.AC  = 0
+        self.AC = 0
         self.total_synops = 0
         self.total_samples = 0
 
     def __call__(self, model, preds, data):
-        """ Multiply-accumulates (MACs) of the model forward.
+        """
+        Multiply-accumulates (MACs) of the model forward.
 
         Args:
             model: A NeuroBenchModel.
             preds: A tensor of model predictions.
             data: A tuple of data and labels.
             inputs: A tensor of model inputs.
         Returns:
             float: Multiply-accumulates.
+
         """
         for hook in model.connection_hooks:
-            inputs = hook.inputs # copy of the inputs, delete hooks after
+            inputs = hook.inputs  # copy of the inputs, delete hooks after
             for spikes in inputs:
                 # spikes is batch, features, see snntorchmodel wrappper
                 # for single_in in spikes:
                 if len(spikes) == 1:
                     spikes = spikes[0]
                 hook.hook.remove()
                 operations, spiking = single_layer_MACs(spikes, hook.layer)
-                total_ops,_ = single_layer_MACs(spikes, hook.layer, total=True)
+                total_ops, _ = single_layer_MACs(spikes, hook.layer, total=True)
                 self.total_synops += total_ops
                 if spiking:
                     self.AC += operations
                 else:
                     self.MAC += operations
                 hook.register_hook()
         # ops_per_sample = ops / data[0].size(0)
         self.total_samples += data[0].size(0)
         return self.compute()
-    
+
     def compute(self):
         if self.total_samples == 0:
-            return {'Effective_MACs': 0, 'Effective_ACs': 0, 'Dense': 0}
-        ac = self.AC/self.total_samples
-        mac = self.MAC/self.total_samples
-        total_synops = self.total_synops/self.total_samples
-        return {'Effective_MACs': mac, 'Effective_ACs': ac, 'Dense': total_synops}
-    
+            return {"Effective_MACs": 0, "Effective_ACs": 0, "Dense": 0}
+        ac = self.AC / self.total_samples
+        mac = self.MAC / self.total_samples
+        total_synops = self.total_synops / self.total_samples
+        return {"Effective_MACs": mac, "Effective_ACs": ac, "Dense": total_synops}
+
 
 class r2(AccumulatedMetric):
-    """ R2 Score of the model predictions.
+    """
+    R2 Score of the model predictions.
 
     Currently implemented for 2D output only.
+
     """
 
     def __init__(self):
-        """ Initalize metric state.
+        """
+        Initalize metric state.
 
         Must hold memory of all labels seen so far.
+
         """
         self.x_sum_squares = 0.0
         self.y_sum_squares = 0.0
-        
-        self.x_labels = torch.tensor([])
-        self.y_labels = torch.tensor([])
+
+        self.x_labels = None
+        self.y_labels = None
 
     def reset(self):
-        """ Reset metric state.
-        """
+        """Reset metric state."""
         self.x_sum_squares = 0.0
         self.y_sum_squares = 0.0
-        
+
         self.x_labels = torch.tensor([])
         self.y_labels = torch.tensor([])
 
     def __call__(self, model, preds, data):
         """
         Args:
             model: A NeuroBenchModel.
             preds: A tensor of model predictions.
             data: A tuple of data and labels.
         Returns:
             float: R2 Score.
         """
         check_shape(preds, data[1])
-        self.x_sum_squares += torch.sum((data[1][:, 0] - preds[:, 0])**2).item()
-        self.y_sum_squares += torch.sum((data[1][:, 1] - preds[:, 1])**2).item()
-        self.x_labels = torch.cat((self.x_labels, data[1][:, 0]))
-        self.y_labels = torch.cat((self.y_labels, data[1][:, 1]))
+        self.x_sum_squares += torch.sum((data[1][:, 0] - preds[:, 0]) ** 2).item()
+        self.y_sum_squares += torch.sum((data[1][:, 1] - preds[:, 1]) ** 2).item()
+
+        if self.x_labels is None:
+            self.x_labels = data[1][:, 0]
+            self.y_labels = data[1][:, 1]
+        else:
+            self.x_labels = torch.cat((self.x_labels, data[1][:, 0]))
+            self.y_labels = torch.cat((self.y_labels, data[1][:, 1]))
 
         return self.compute()
 
     def compute(self):
-        """ Compute r2 score using accumulated data
-        """
-        x_denom = self.x_labels.var(correction=0)*len(self.x_labels)
-        y_denom = self.y_labels.var(correction=0)*len(self.y_labels)
+        """Compute r2 score using accumulated data."""
+        x_denom = self.x_labels.var(correction=0) * len(self.x_labels)
+        y_denom = self.y_labels.var(correction=0) * len(self.y_labels)
 
-        x_r2 = 1 - (self.x_sum_squares/ x_denom)
-        y_r2 = 1 - (self.y_sum_squares/ y_denom)
+        x_r2 = 1 - (self.x_sum_squares / x_denom)
+        y_r2 = 1 - (self.y_sum_squares / y_denom)
 
         r2 = (x_r2 + y_r2) / 2
 
         return r2.item()
 
+
 class COCO_mAP(AccumulatedMetric):
-    """ COCO mean average precision.
+    """
+    COCO mean average precision.
 
     Measured for event data based on Perot2020, Supplementary B (https://arxiv.org/abs/2009.13436)
         - Skips first 0.5s of each sequence
         - Bounding boxes with diagonal size smaller than 60 pixels are ignored
+
     """
 
     def __init__(self):
-        """ Initalize metric state.
-        """
+        """Initalize metric state."""
         from metavision_ml.metrics.coco_eval import CocoEvaluator
         from collections import defaultdict
 
         self.dt_detections = defaultdict(list)
         self.gt_detections = defaultdict(list)
-        self.evaluator = CocoEvaluator(classes=['background'] + ["pedestrian", "two wheeler", "car"], height=360, width=640)
+        self.evaluator = CocoEvaluator(
+            classes=["background"] + ["pedestrian", "two wheeler", "car"],
+            height=360,
+            width=640,
+        )
 
     def reset(self):
-        """ Reset metric state.
-        """
+        """Reset metric state."""
         self.dt_detections = defaultdict(list)
         self.gt_detections = defaultdict(list)
-        self.evaluator = CocoEvaluator(classes=['background'] + ["pedestrian", "two wheeler", "car"], height=360, width=640)
+        self.evaluator = CocoEvaluator(
+            classes=["background"] + ["pedestrian", "two wheeler", "car"],
+            height=360,
+            width=640,
+        )
 
     def __call__(self, model, preds, data):
-        """ Accumulate predictions and ground truth detections over batches.
+        """
+        Accumulate predictions and ground truth detections over batches.
 
         Args:
             model: A NeuroBenchModel.
             preds: A tensor of model predictions.
             data: A tuple of data and labels.
         Returns:
             float: COCO mean average precision.
+
         """
         from metavision_ml.data import box_processing as box_api
         from metavision_sdk_core import EventBbox
 
         targets = data[1]
         video_infos = data[2]["video_infos"]
         frame_is_labeled = data[2]["frame_is_labeled"]
         skip_us = 500000
 
         for t in range(len(targets)):
             for i in range(len(targets[t])):
                 gt_boxes = targets[t][i]
-                
+
                 pred = preds[t][i]
 
                 video_info, tbin_start, _ = video_infos[i]
 
-                if video_info.padding or frame_is_labeled[t, i] == False:
+                if video_info.padding or frame_is_labeled[t, i] is False:
                     continue
 
                 name = video_info.path
                 if name not in self.dt_detections:
                     self.dt_detections[name] = [np.zeros((0), dtype=box_api.EventBbox)]
                 if name not in self.gt_detections:
                     self.gt_detections[name] = [np.zeros((0), dtype=box_api.EventBbox)]
@@ -344,34 +402,40 @@
 
                 if ts < skip_us:
                     continue
 
                 if isinstance(gt_boxes, torch.Tensor):
                     gt_boxes = gt_boxes.cpu().numpy()
                 if gt_boxes.dtype == np.float32:
-                    gt_boxes = box_api.box_vectors_to_bboxes(gt_boxes[:, :4], gt_boxes[:, 4], ts=ts)
-
-                if pred['boxes'] is not None and len(pred['boxes']) > 0:
-                    boxes = pred['boxes'].cpu().data.numpy()
-                    labels = pred['labels'].cpu().data.numpy()
-                    scores = pred['scores'].cpu().data.numpy()
-                    dt_boxes = box_api.box_vectors_to_bboxes(boxes, labels, scores, ts=ts)
+                    gt_boxes = box_api.box_vectors_to_bboxes(
+                        gt_boxes[:, :4], gt_boxes[:, 4], ts=ts
+                    )
+
+                if pred["boxes"] is not None and len(pred["boxes"]) > 0:
+                    boxes = pred["boxes"].cpu().data.numpy()
+                    labels = pred["labels"].cpu().data.numpy()
+                    scores = pred["scores"].cpu().data.numpy()
+                    dt_boxes = box_api.box_vectors_to_bboxes(
+                        boxes, labels, scores, ts=ts
+                    )
                     self.dt_detections[name].append(dt_boxes)
                 else:
                     self.dt_detections[name].append(np.zeros((0), dtype=EventBbox))
 
                 if len(gt_boxes):
                     gt_boxes["t"] = ts
                     self.gt_detections[name].append(gt_boxes)
                 else:
                     self.gt_detections[name].append(np.zeros((0), dtype=EventBbox))
 
-        return 0.0 # too heavy to compute every iteration
+        return 0.0  # too heavy to compute every iteration
 
     def compute(self):
-        """ Compute COCO mAP using accumulated data.
-        """
+        """Compute COCO mAP using accumulated data."""
         print("Computing COCO mAP.")
         for key in self.gt_detections:
-            self.evaluator.partial_eval([np.concatenate(self.gt_detections[key])], [np.concatenate(self.dt_detections[key])])
+            self.evaluator.partial_eval(
+                [np.concatenate(self.gt_detections[key])],
+                [np.concatenate(self.dt_detections[key])],
+            )
         coco_kpi = self.evaluator.accumulate()
-        return coco_kpi['mean_ap']
+        return coco_kpi["mean_ap"]
```

### Comparing `neurobench-1.0.2/neurobench/datasets/MSWC_IncrementalLoader.py` & `neurobench-1.0.3/neurobench/datasets/MSWC_IncrementalLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,110 +8,150 @@
 import numpy as np
 import torch
 from torch.utils.data import IterableDataset
 
 from neurobench.datasets.MSWC_dataset import MSWC, MSWC_query
 
 
-def get_indices_per_class(languages, root, samples_per_class: int, support_query_split: Optional[Tuple[int, int]] = None) -> Union[Dict[int, List[int]], Dict[int, Tuple[List[int], List[int]]]]:
+def get_indices_per_class(
+    languages,
+    root,
+    samples_per_class: int,
+    support_query_split: Optional[Tuple[int, int]] = None,
+) -> Union[Dict[int, List[int]], Dict[int, Tuple[List[int], List[int]]]]:
     indices_per_lang = {}
     for lang in languages:
         indices_per_lang[lang] = {}
         indices_per_class = indices_per_lang[lang]
         dataset = MSWC(root=root, subset="evaluation", language=lang)
 
         # Ordering samples index per class using the fact that all samples from one class are indexed together
         for i in range(len(dataset) // samples_per_class):
-            label = dataset[i*samples_per_class][1]
-            indices_per_class[label] = list(range(i * samples_per_class, (i + 1) * samples_per_class))
+            label = dataset[i * samples_per_class][1]
+            indices_per_class[label] = list(
+                range(i * samples_per_class, (i + 1) * samples_per_class)
+            )
 
         if support_query_split is not None:
             n_support, n_query = support_query_split
 
             for key in indices_per_class.keys():
-                indices_per_class[key] = (indices_per_class[key][:n_support], indices_per_class[key][n_support:n_support+n_query])
+                indices_per_class[key] = (
+                    indices_per_class[key][:n_support],
+                    indices_per_class[key][n_support : n_support + n_query],
+                )
         del dataset
 
     return indices_per_lang
 
 
 class IncrementalFewShot(IterableDataset):
-
-    def __init__(self,
-                 k_shot: int,
-                 root: str,
-                 inc_languages: list = ['fa', 'eo', 'pt', 'eu', 'pl', 'cy', 'nl', 'ru', 'es', 'it'],
-                 query_shots: int = -1,
-                 support_query_split: Optional[Tuple[int, int]] = None):
-        """Dataset for few shot learning.
+    def __init__(
+        self,
+        k_shot: int,
+        root: str,
+        inc_languages: list = [
+            "fa",
+            "eo",
+            "pt",
+            "eu",
+            "pl",
+            "cy",
+            "nl",
+            "ru",
+            "es",
+            "it",
+        ],
+        query_shots: int = -1,
+        support_query_split: Optional[Tuple[int, int]] = None,
+    ):
+        """
+        Dataset for few shot learning.
 
         Args:
             k_shot (int, optional): Number of samples per class in the support set.
             root (str): Path of the folder where to find the dataset language folders.
-            inc_languages (List[str], optional): List of languages 2 letters names to use as incremental sessions. 
+            inc_languages (List[str], optional): List of languages 2 letters names to use as incremental sessions.
             query_shots (Optional[int]): Number of samples per class in the query set. If not set, query_shots is set to k_shot. Defaults to -1.
             support_query_split (Optional[Tuple[int, int]], optional): Create non-overlapping support and query pools of given number of samples per class. Defaults to None.
+
         """
 
         self.support_query_split = support_query_split
-        self.samples_per_class = 200 # Number of samples per class to use. Used to simplify samples class indexing as the used dataset is ordered (class_0_sample_0, c0s1, c0s2, c1s0, c1s1, c1s2, ...).
-        self.indices_per_lang = get_indices_per_class(inc_languages, root, self.samples_per_class, self.support_query_split)
+        self.samples_per_class = 200  # Number of samples per class to use. Used to simplify samples class indexing as the used dataset is ordered (class_0_sample_0, c0s1, c0s2, c1s0, c1s1, c1s2, ...).
+        self.indices_per_lang = get_indices_per_class(
+            inc_languages, root, self.samples_per_class, self.support_query_split
+        )
 
-        self.n_way = 10 # Number of classes in the support and support sets. Fixed based on the dataset
+        self.n_way = 10  # Number of classes in the support and support sets. Fixed based on the dataset
         self.k_shot = k_shot
         self.query_shots = query_shots if query_shots != -1 else k_shot
 
         self.languages = inc_languages
         self.root = root
 
     def __iter__(self):
-        """Get a batch of samples for a k-shot n-way task.
+        """
+        Get a batch of samples for a k-shot n-way task.
 
         Returns:
             tuple[List[tuple[Tensor, Tensor]], Dataset, List[int]]: The support as a list of all shots, the query as a Dataset object and the list of cumulative query classes.
+
         """
 
         cumulative_classes = {}
         self.cumulative_query = []
 
         for lang in random.sample(self.languages, len(self.languages)):
             dataset = MSWC(root=self.root, subset="evaluation", language=lang)
 
-            support_classes = random.sample(sorted(self.indices_per_lang[lang].keys()), self.n_way)
+            support_classes = random.sample(
+                sorted(self.indices_per_lang[lang].keys()), self.n_way
+            )
             cumulative_classes[lang] = support_classes
 
             # Yields iterative sessions
             out = self._inner_iter(lang, dataset, support_classes, cumulative_classes)
             del dataset
             yield out
 
     def _inner_iter(self, language, dataset, support_classes, cumulative_classes):
         for class_index in cumulative_classes[language]:
-            query_indices = np.random.choice(self.indices_per_lang[language][class_index][1], self.query_shots, replace=False)
-
-            self.cumulative_query += [(dataset[j][3], class_index, dataset[j][2]) for j in query_indices]
+            query_indices = np.random.choice(
+                self.indices_per_lang[language][class_index][1],
+                self.query_shots,
+                replace=False,
+            )
+
+            self.cumulative_query += [
+                (dataset[j][3], class_index, dataset[j][2]) for j in query_indices
+            ]
 
         query_set = MSWC_query(self.cumulative_query)
 
         X_train_samples = [[] for _ in range(self.k_shot)]
         y_train_samples = [[] for _ in range(self.k_shot)]
 
         # For every class
         for class_index in support_classes:
-            support_indices = np.random.choice(self.indices_per_lang[language][class_index][0], self.k_shot, replace=False)
+            support_indices = np.random.choice(
+                self.indices_per_lang[language][class_index][0],
+                self.k_shot,
+                replace=False,
+            )
 
             # For every (support) shot/sample
             for j, index in enumerate(support_indices):
                 data, real_class, _, _ = dataset[index]
                 y_train_samples[j].append(real_class)
                 X_train_samples[j].append(data)
-            
+
         support = []
         for x, y in zip(X_train_samples, y_train_samples):
-            shot = (torch.stack(x),torch.tensor(y, dtype=torch.long))
+            shot = (torch.stack(x), torch.tensor(y, dtype=torch.long))
             support.append(shot)
 
         query_classes = []
         for lang_class in cumulative_classes.values():
             query_classes.extend(lang_class)
 
         out = (support, query_set, query_classes)
```

### Comparing `neurobench-1.0.2/neurobench/datasets/WISDM.py` & `neurobench-1.0.3/neurobench/datasets/WISDM.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,98 +2,116 @@
 from torch.utils.data import DataLoader, TensorDataset
 import os
 import gdown
 import numpy as np
 import torch
 
 
-def create_directory(directory_path):
-    if os.path.exists(directory_path):
-        return None
-    else:
-        try:
-            os.makedirs(directory_path)
-        except:
-            # in case another machine created the path meanwhile! :(
-            return None
-        return directory_path
-
-
 def convert_to_tensor(x, y):
     return torch.tensor(x, dtype=torch.float), torch.tensor(y, dtype=torch.long)
 
 
 class WISDM(LightningDataModule):
     def __init__(self, path: str = "path/to/file", batch_size: int = 256):
         super().__init__()
         self.ds_test = None
         self.ds_val = None
         self.ds_train = None
         self.batch_size = batch_size
 
-        (x_train, x_val, x_test, y_train, y_val,
-         y_test) = self.load_wisdm2_data(path)
+        (x_train, x_val, x_test, y_train, y_val, y_test) = self.load_wisdm2_data(path)
         self.train_dataset = convert_to_tensor(x_train, np.argmax(y_train, axis=-1))
         self.val_dataset = convert_to_tensor(x_val, np.argmax(y_val, axis=-1))
         self.test_dataset = convert_to_tensor(x_test, np.argmax(y_test, axis=-1))
 
         self.num_inputs = next(iter(self.train_dataset))[0].shape[1]
         self.num_steps = next(iter(self.train_dataset))[0].shape[0]
         self.num_outputs = len(np.unique(np.argmax(y_train, axis=-1)))
 
     @staticmethod
     def load_wisdm2_data(path):
-
         if path.endswith(".npz"):
             file_path = path
             dir_path = os.path.split(file_path)[0]
         else:
-            file_path = os.path.join(path, 'watch_subset2_40.npz')
+            file_path = os.path.join(path, "watch_subset2_40.npz")
             dir_path = path
 
         if not os.path.exists(dir_path) or not os.path.isfile(file_path):
-            create_directory(directory_path=dir_path)
+            os.makedirs(dir_path, exist_ok=True)
             url = "https://drive.google.com/drive/folders/1WCN-XwLM_D2nOTZLY00iGwEJLwDQaUCv"
             gdown.download_folder(url, quiet=True, use_cookies=False, output=dir_path)
 
         data = np.load(file_path)
-        return (data['arr_0'], data['arr_1'], data['arr_2'], data['arr_3'], data['arr_4'], data['arr_5'])
+        return (
+            data["arr_0"],
+            data["arr_1"],
+            data["arr_2"],
+            data["arr_3"],
+            data["arr_4"],
+            data["arr_5"],
+        )
 
     def setup(self, stage: str):
         match stage:
-            case 'fit':
+            case "fit":
                 x_train, y_train = self.train_dataset
                 x_val, y_val = self.val_dataset
                 x_test, y_test = self.test_dataset
                 self.ds_train = TensorDataset(x_train, y_train)
                 self.ds_val = TensorDataset(x_val, y_val)
                 self.ds_test = TensorDataset(x_test, y_test)
 
-            case 'test':
+            case "test":
                 x_test, y_test = self.test_dataset
                 self.ds_test = TensorDataset(x_test, y_test)
 
-            case 'predict':
+            case "predict":
                 x_test, y_test = self.test_dataset
                 self.ds_test = TensorDataset(x_test, y_test)
 
     def train_dataloader(self):
-        return DataLoader(self.ds_train, batch_size=self.batch_size, shuffle=True, num_workers=8, drop_last=False,
-                          persistent_workers=True)
+        return DataLoader(
+            self.ds_train,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=8,
+            drop_last=False,
+            persistent_workers=True,
+        )
 
     def val_dataloader(self):
-        return DataLoader(self.ds_val, batch_size=self.batch_size, num_workers=8, shuffle=False, drop_last=False,
-                          persistent_workers=True)
+        return DataLoader(
+            self.ds_val,
+            batch_size=self.batch_size,
+            num_workers=8,
+            shuffle=False,
+            drop_last=False,
+            persistent_workers=True,
+        )
 
     def test_dataloader(self):
-        return DataLoader(self.ds_test, batch_size=self.batch_size, num_workers=8, shuffle=False, drop_last=False,
-                          persistent_workers=True)
+        return DataLoader(
+            self.ds_test,
+            batch_size=self.batch_size,
+            num_workers=8,
+            shuffle=False,
+            drop_last=False,
+            persistent_workers=True,
+        )
 
     def predict_dataloader(self):
-        return DataLoader(self.ds_test, batch_size=self.batch_size, num_workers=8, shuffle=False, drop_last=False,
-                          persistent_workers=True)
-
-    def teardown(self, stage: str):
-        ...
+        return DataLoader(
+            self.ds_test,
+            batch_size=self.batch_size,
+            num_workers=8,
+            shuffle=False,
+            drop_last=False,
+            persistent_workers=True,
+        )
 
     def __len__(self):
-        return self.train_dataset[0].shape[0] + self.val_dataset[0].shape[0] + self.test_dataset[0].shape[0]
+        return (
+            self.train_dataset[0].shape[0]
+            + self.val_dataset[0].shape[0]
+            + self.test_dataset[0].shape[0]
+        )
```

### Comparing `neurobench-1.0.2/neurobench/datasets/__init__.py` & `neurobench-1.0.3/neurobench/datasets/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 from .dataset import *
 from .utils import *
 from ..utils import _lazy_import
 
+
 def SpeechCommands(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".speech_commands", "SpeechCommands")(*args, **kwargs)
+    return _lazy_import("neurobench.datasets", ".speech_commands", "SpeechCommands")(
+        *args, **kwargs
+    )
+
 
 def PrimateReaching(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".primate_reaching", "PrimateReaching")(*args, **kwargs)
+    return _lazy_import("neurobench.datasets", ".primate_reaching", "PrimateReaching")(
+        *args, **kwargs
+    )
+
 
 def Gen4DetectionDataLoader(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".megapixel_automotive", "Gen4DetectionDataLoader")(*args, **kwargs)
+    return _lazy_import(
+        "neurobench.datasets", ".megapixel_automotive", "Gen4DetectionDataLoader"
+    )(*args, **kwargs)
+
 
 def DVSGesture(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".dvs_gesture", "DVSGesture")(*args, **kwargs)
+    return _lazy_import("neurobench.datasets", ".dvs_gesture", "DVSGesture")(
+        *args, **kwargs
+    )
+
 
 def MackeyGlass(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".mackey_glass", "MackeyGlass")(*args, **kwargs)
+    return _lazy_import("neurobench.datasets", ".mackey_glass", "MackeyGlass")(
+        *args, **kwargs
+    )
+
 
 def WISDM(*args, **kwargs):
     return _lazy_import("neurobench.datasets", ".WISDM", "WISDM")(*args, **kwargs)
 
+
 def MSWC(*args, **kwargs):
     return _lazy_import("neurobench.datasets", ".MSWC_dataset", "MSWC")(*args, **kwargs)
-
```

### Comparing `neurobench-1.0.2/neurobench/datasets/dataset.py` & `neurobench-1.0.3/neurobench/datasets/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from torch.utils.data import Dataset
 
+
 class NeuroBenchDataset(Dataset):
     """
-    Abstract class for NeuroBench datasets. Individual datasets are responsible
-    for collating and splitting data. The top-level benchmark expects that the
-    dataset is wrapped into a DataLoader.
+    Abstract class for NeuroBench datasets.
+
+    Individual datasets are responsible for collating and splitting data. The top-level
+    benchmark expects that the dataset is wrapped into a DataLoader.
+
     """
+
     def __init__(self):
-        """ Init dataset.
-        """
-        raise NotImplementedError("Subclasses of NeuroBenchDataset should implement __init__")
+        """Init dataset."""
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchDataset should implement __init__"
+        )
 
     def __len__(self):
-        """ Returns length of dataset.
-        """
-        raise NotImplementedError("Subclasses of NeuroBenchDataset should implement __len__")
+        """Returns length of dataset."""
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchDataset should implement __len__"
+        )
 
     def __getitem__(self, idx):
-        """ Returns a sample from the dataset.
-        """
-        raise NotImplementedError("Subclasses of NeuroBenchDataset should implement __getitem__")
+        """Returns a sample from the dataset."""
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchDataset should implement __getitem__"
+        )
```

### Comparing `neurobench-1.0.2/neurobench/datasets/dvs_gesture.py` & `neurobench-1.0.3/neurobench/datasets/dvs_gesture.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,35 +13,40 @@
 
 # make animation
 from matplotlib.animation import FuncAnimation
 
 
 class DVSGesture(NeuroBenchDataset):
     """
-    Installs DVSGesture Dataset with individual events in each file,
-    if not yet installed, else pass the path of the tonic DVSGesture install.
+    Installs DVSGesture Dataset with individual events in each file, if not yet
+    installed, else pass the path of the tonic DVSGesture install.
 
     Data information:
     - Event rate: 1MHz -> dt 1e-6
     - Sample length: 1.7 seconds
     - Default timestep for frames: 5 ms
 
     For possible preprocessing functions, see:
     https://docs.prophesee.ai/stable/tutorials/ml/data_processing/event_preprocessing.html?highlight=metavision_ml%20preprocessing
+
     """
+
     def __init__(
         self, path, split="testing", data_type="frames", preprocessing="stack"
     ):
-        """ Initialization will load in data from path if possible, else will download dataset into path. 
-        
+        """
+        Initialization will load in data from path if possible, else will download
+        dataset into path.
+
         Args:
             path (str): Path of DVS Gesture dataset folder if applicable, else the destination of DVS Gesture dataset.
             split (str): Return testing or training data.
             data_type (str): If 'frames', returns frames with preprocessing applied; else returns raw events.
             preprocessing (str): Preprocessing to get frames from raw events.
+
         """
         # download or load data
         if split == "training":
             self.dataset = tonic_DVSGesture(save_to=path)
         else:
             self.dataset = tonic_DVSGesture(save_to=path, train=False)
 
@@ -52,30 +57,34 @@
 
         # sample parameters:
         self._deltat = 5000  # DVS is in microseconds -> deltat = 5ms
         self._T = 1700  # in ms, sample time is 1.7 sec
         self.random_window = False
 
     def __len__(self):
-        """ Returns the number of samples in the dataset.
+        """
+        Returns the number of samples in the dataset.
 
         Returns:
             int: The number of samples in the dataset.
+
         """
         return len(self.filenames)
 
     def __getitem__(self, idx):
-        """ Getter method for test data in the DataLoader.
+        """
+        Getter method for test data in the DataLoader.
 
         Args:
             idx (int): Index of the sample.
 
         Returns:
             sample (tensor): Individual data sample, which can be a sequence of frames or raw data.
             target (tensor): Corresponding gesture label.
+
         """
         structured_array = self.dataset[idx][0]
 
         # label = torch.nn.functional.one_hot(torch.tensor(self.dataset[idx][1]), num_classes=11)
         label = torch.tensor(self.dataset[idx][1])
 
         # get data
@@ -136,139 +145,150 @@
         """
         Sets sample parameters used if frames are created from events.
 
         Args:
             delta_t (int): Time steps to stack events into frames (in milliseconds).
             length (int): Length in milliseconds of each sample.
             random_window (bool): If True, the sample will be a random time window of length within the gesture.
+
         """
         self._deltat = delta_t * 1000  # convert to microseconds
         self._T = length
         self.random_window = random_window
 
 
 def stack_preprocessing(
     xypt, delta_t=5000, tbins=200, h_og=128, w_og=128, channels=3, display_frame=False
 ):
     """
-    Applies stack preprocessing to events. If at least one event has occurred at (x,y) in delta_t corresponding channel 
-    (pos or neg) will be 1, else zero.
+    Applies stack preprocessing to events. If at least one event has occurred at (x,y)
+    in delta_t corresponding channel (pos or neg) will be 1, else zero.
 
     Args:
         delta_t (int): Time steps to stack events into frames (in milliseconds).
         tbins (int): Number of frames required.
         h_og (int): Number of pixels in height.
         w_og (int): Number of pixels in width.
         channels (int): Number of channels in each frame (default 3 for plotting purposes).
         display_frame (bool): If True, will create an animation to visualize event frames.
+
     """
     frames = np.zeros((tbins, channels, h_og, w_og))
     for frame in frames:
         # delete prev neg times
         xypt_new = xypt[xypt[:, 3] >= 0]
         xypt = xypt_new
 
         # change timestamps
         xypt[:, 3] = xypt[:, 3] - delta_t
 
         xypt_sub = xypt[xypt[:, 3] <= 0]  # events for the current frame
-        pos_pol = np.unique(xypt_sub[xypt_sub[:, 2] == True][:, :2], axis=0)
-        neg_pol = np.unique(xypt_sub[xypt_sub[:, 2] == False][:, :2], axis=0)
+        pos_pol = np.unique(xypt_sub[xypt_sub[:, 2] is True][:, :2], axis=0)
+        neg_pol = np.unique(xypt_sub[xypt_sub[:, 2] is False][:, :2], axis=0)
 
         frame[0, :, :][pos_pol[:, 0], pos_pol[:, 1]] = 1
         frame[1, :, :][neg_pol[:, 0], neg_pol[:, 1]] = 1
 
     if display_frame:
-        frame = frame.astype(float) / np.max(frame) 
+        frame = frame.astype(float) / np.max(frame)
 
         animation = FuncAnimation(
-            fig, update, frames=tbins, fargs=(frames,), interval=delta_t/1000
-        )  
+            fig, update, frames=tbins, fargs=(frames,), interval=delta_t / 1000
+        )
         animation.save("test.gif")
-        plt.suptitle('Stack preprocessing')
+        plt.suptitle("Stack preprocessing")
         plt.show()
 
     return frames
 
 
-def histogram_difference_preprocessing(xypt, delta_t=5000, tbins=200, h_og=128, w_og=128, channels=3, display_frame=False):
+def histogram_difference_preprocessing(
+    xypt, delta_t=5000, tbins=200, h_og=128, w_og=128, channels=3, display_frame=False
+):
     """
-    Applies histogram preprocessing to events. For every positive (pos) or negative (neg) event that has occurred 
-    at (x,y) in delta_t, 1 will be added to (x,y) in the corresponding channel (pos or neg).
+    Applies histogram preprocessing to events. For every positive (pos) or negative
+    (neg) event that has occurred at (x,y) in delta_t, 1 will be added to (x,y) in the
+    corresponding channel (pos or neg).
 
     Args:
         delta_t (int): Time steps to stack events into frames (in milliseconds).
         tbins (int): Number of frames required.
         h_og (int): Number of pixels in height.
         w_og (int): Number of pixels in width.
         channels (int): Number of channels in each frame (default 3 for plotting purposes).
         display_frame (bool): If True, will create an animation to visualize event frames.
+
     """
     histogram = np.zeros((tbins, channels, h_og, w_og))
     for frame in histogram:
         # delete prev neg times
         xypt_new = xypt[xypt[:, 3] >= 0]
         xypt = xypt_new
 
         # change timestamps
         xypt[:, 3] = xypt[:, 3] - delta_t
 
         xypt_sub = xypt[xypt[:, 3] <= 0]  # events for the current frame
-        pos_pol, pos_count = np.unique(xypt_sub[xypt_sub[:, 2] == True][:, :2], axis=0, return_counts=True)
-        neg_pol, neg_count = np.unique(xypt_sub[xypt_sub[:, 2] == False][:, :2], axis=0, return_counts=True)
-        
+        pos_pol, pos_count = np.unique(
+            xypt_sub[xypt_sub[:, 2] is True][:, :2], axis=0, return_counts=True
+        )
+        neg_pol, neg_count = np.unique(
+            xypt_sub[xypt_sub[:, 2] is False][:, :2], axis=0, return_counts=True
+        )
+
         counts_dict = {}
 
         # Update counts from the positives
         for value, count in zip(pos_pol, pos_count):
             counts_dict[tuple(value)] = counts_dict.get(tuple(value), 0) + count
 
         # Update counts from the negatives
         for value, count in zip(neg_pol, neg_count):
             counts_dict[tuple(value)] = counts_dict.get(tuple(value), 0) - count
 
         # Convert the dictionary into a NumPy array
         array_data = [[*key, value] for key, value in counts_dict.items()]
         result_array = np.array(array_data)
-        pos_pol = result_array[result_array[:,2]>0]
-        neg_pol = result_array[result_array[:,2]<0]
-        frame[0, :, :][pos_pol[:, 0], pos_pol[:, 1]] = pos_pol[:,2]
-        frame[1, :, :][neg_pol[:, 0], neg_pol[:, 1]] = -neg_pol[:,2] # avoid clipping between [0,1]
+        pos_pol = result_array[result_array[:, 2] > 0]
+        neg_pol = result_array[result_array[:, 2] < 0]
+        frame[0, :, :][pos_pol[:, 0], pos_pol[:, 1]] = pos_pol[:, 2]
+        frame[1, :, :][neg_pol[:, 0], neg_pol[:, 1]] = -neg_pol[
+            :, 2
+        ]  # avoid clipping between [0,1]
 
     if display_frame:
-        frame = frame.astype(float) / np.max(frame) 
-        
+        frame = frame.astype(float) / np.max(frame)
+
         animation = FuncAnimation(
             fig, update, frames=tbins, fargs=(histogram,), interval=5
-        )  
+        )
         animation.save("waving_hand.gif", fps=1 / (5e-3))
-        
-        plt.suptitle('Histogram difference method')
+
+        plt.suptitle("Histogram difference method")
         plt.show()
 
     return histogram
 
 
 fig, ax = plt.subplots()
 
 
 def update(frame, frames):
-    """
-    Helper function for animation. 
-    """
+    """Helper function for animation."""
     ax.clear()
     image = frames[frame].transpose(1, 2, 0)
 
     ax.imshow(image, cmap="brg")  # You can adjust the colormap as needed
     ax.set_title(f"Frame {frame}")
 
 
 if __name__ == "__main__":
     path = os.curdir
     dataset = DVSGesture(
         os.path.join(path, "data/dvs_gesture"),
-        split="testing", preprocessing="histo_diff"
+        split="testing",
+        preprocessing="histo_diff",
     )
 
     dataloader = DataLoader(dataset, batch_size=16, shuffle=True)
     for local_batch, local_labels in dataloader:
         print(local_batch[0].shape, local_labels.shape)
```

### Comparing `neurobench-1.0.2/neurobench/datasets/mackey_glass.py` & `neurobench-1.0.3/neurobench/datasets/mackey_glass.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,63 +3,64 @@
 import torch
 import os
 from jitcdde import y, t, jitcdde_lyap
 from .utils import download_url
 from urllib.error import URLError
 import tarfile
 
-'''
+"""
 The jitcdde package used to generate the MackeyGlass time-series can vary based 
 on platform, due to lower level integration solvers. In order to ensure that you
 are using the same data as the authors, please use the downloaded version, which
 will be automatically downloaded.
 
 https://huggingface.co/datasets/NeuroBench/mackey_glass
-'''
+"""
 
 
 class MackeyGlass(Dataset):
-    """ Dataset for the Mackey-Glass task.
-    """
+    """Dataset for the Mackey-Glass task."""
 
-    def __init__(self,
-                 file_path=None,
-                 tau=17,
-                 lyaptime=197,
-                 constant_past=0.7206597,
-                 nmg=10,
-                 beta=0.2,
-                 gamma=0.1,
-                 pts_per_lyaptime=75,
-                 traintime=10.,
-                 testtime=10.,
-                 start_offset=0.,
-                 seed_id=0,
-                 bin_window=1,
-                 download=True
-                 ):
+    def __init__(
+        self,
+        file_path=None,
+        tau=17,
+        lyaptime=197,
+        constant_past=0.7206597,
+        nmg=10,
+        beta=0.2,
+        gamma=0.1,
+        pts_per_lyaptime=75,
+        traintime=10.0,
+        testtime=10.0,
+        start_offset=0.0,
+        seed_id=0,
+        bin_window=1,
+        download=True,
+    ):
         """
         Initializes the Mackey-Glass dataset.
 
         Args:
             file_path (str): path to .npy file containing Mackey-Glass time-series. If this is provided, then tau, lyaptime, constant_past, nmg, beta, gamma are ignored.
             tau (float): parameter of the Mackey-Glass equation
             lyaptime (float): Lyapunov time of the time-series
             constant_past (float): initial condition for the solver
             nmg (float): parameter of the Mackey-Glass equation
             beta (float): parameter of the Mackey-Glass equation
             gamma (float): parameter of the Mackey-Glass equation
             pts_per_lyaptime (int): number of points to sample per one Lyapunov time
             traintime (float): number of Lyapunov times to be used for training a model
-            testtime (float): number of Lyapunov times to be used for testing a model            
+            testtime (float): number of Lyapunov times to be used for testing a model
             start_offset (int): added offset in number of points to shift the timeseries forward
             seed_id (int): seed for generating function solution
             bin_window (int): number of points forming lookback window for each prediction
             download (bool): If True, downloads the dataset from the internet and puts it in root
                                  directory. If dataset is already downloaded, it will not be downloaded again.
+
         """
 
         super().__init__()
 
         # Parameters
         self.tau = tau
         self.lyaptime = lyaptime
@@ -76,27 +77,33 @@
 
         self.start_offset = start_offset
         self.seed_id = seed_id
 
         self.bin_window = bin_window
 
         # Total time to simulate the system
-        self.maxtime = self.traintime + self.testtime + (self.lyaptime / self.pts_per_lyaptime)
+        self.maxtime = (
+            self.traintime + self.testtime + (self.lyaptime / self.pts_per_lyaptime)
+        )
 
         # Discrete-time versions of the continuous times specified above
         self.traintime_pts = round(traintime * self.pts_per_lyaptime)
         self.testtime_pts = round(testtime * self.pts_per_lyaptime)
-        self.maxtime_pts = self.traintime_pts + self.testtime_pts + 1  # eval one past the end
+        self.maxtime_pts = (
+            self.traintime_pts + self.testtime_pts + 1
+        )  # eval one past the end
 
         # Specify the system using the provided parameters
         self.mackeyglass_specification = [
-            self.beta * y(0, t - self.tau) / (1 + y(0, t - self.tau) ** self.nmg) - self.gamma * y(0)]
+            self.beta * y(0, t - self.tau) / (1 + y(0, t - self.tau) ** self.nmg)
+            - self.gamma * y(0)
+        ]
 
         self.file_path = file_path
-        self.url = 'https://huggingface.co/datasets/NeuroBench/mackey_glass/resolve/main/data.tar.gz'
+        self.url = "https://huggingface.co/datasets/NeuroBench/mackey_glass/resolve/main/data.tar.gz"
 
         if download and not os.path.exists(self.file_path):
             print("downloading ....")
             self.download()
         # Load or generate time-series
         if os.path.exists(self.file_path) is not None:
             self.load_data(self.file_path)
@@ -106,117 +113,137 @@
         # Generate train/test indices
         self.split_data()
 
     def download(self):
         """Download the Mackey Glass data if it doesn't exist already."""
 
         if os.path.exists(self.file_path):
-            print(f"The dataset already exists!")
+            print("The dataset already exists!")
             return
 
         os.makedirs(os.path.dirname(self.file_path), exist_ok=True)
 
         # download file
         file_path = f"{os.path.dirname(self.file_path)}/data.tar.gz"
         try:
             print(f"Downloading {self.url}")
             download_url(self.url, file_path)
         except URLError as error:
             print(f"Failed to download (trying next):\n{error}")
         finally:
             print("Unzipping file...")
-            with tarfile.open(file_path, 'r:gz') as tar:
+            with tarfile.open(file_path, "r:gz") as tar:
                 for member in tar.getmembers():
                     if member.isfile():  # Check if it's a file
                         # Remove the directory path from the member's name
                         member.name = os.path.basename(member.name)
                         tar.extract(member, path=os.path.dirname(file_path))
             print()
 
     def load_data(self, file):
         all_data = np.load(file)
 
-        self.mackeyglass_soln = all_data[int(self.start_offset): int(self.start_offset + self.maxtime_pts)]
+        self.mackeyglass_soln = all_data[
+            int(self.start_offset) : int(self.start_offset + self.maxtime_pts)
+        ]
 
         self.mackeyglass_soln = torch.tensor(self.mackeyglass_soln, dtype=torch.float64)
         self.mackeyglass_soln = self.mackeyglass_soln.unsqueeze(dim=-1)
 
         # pad the soln with preceding zeroes for lookback window
         self.mackeyglass_soln = torch.cat(
-            (torch.zeros((self.bin_window - 1, 1), dtype=torch.float64), self.mackeyglass_soln), 0)
+            (
+                torch.zeros((self.bin_window - 1, 1), dtype=torch.float64),
+                self.mackeyglass_soln,
+            ),
+            0,
+        )
 
     def generate_data(self):
-        """ Generate time-series using the provided parameters of the equation.
-        """
+        """Generate time-series using the provided parameters of the equation."""
         np.random.seed(self.seed_id)
 
         # Create the equation object based on the settings
         self.DDE = jitcdde_lyap(self.mackeyglass_specification)
         # self.DDE.set_integration_parameters(atol=1e-17, rtol=1e-17, min_step=1e-17) # TODO: comment this out later after testing
         self.DDE.constant_past([self.constant_past])
         self.DDE.step_on_discontinuities()
 
         ##
-        ## Generate data from the Mackey-Glass system
+        # Generate data from the Mackey-Glass system
         ##
         self.mackeyglass_soln = torch.zeros((self.maxtime_pts, 1), dtype=torch.float64)
         lyaps = torch.zeros((self.maxtime_pts, 1), dtype=torch.float64)
         lyaps_weights = torch.zeros((self.maxtime_pts, 1), dtype=torch.float64)
         count = 0
 
         offset = self.start_offset * self.lyaptime / self.pts_per_lyaptime
 
-        for time in torch.linspace(self.DDE.t + offset, self.DDE.t + offset + self.maxtime, steps=self.maxtime_pts,
-                                   dtype=torch.float64):
+        for time in torch.linspace(
+            self.DDE.t + offset,
+            self.DDE.t + offset + self.maxtime,
+            steps=self.maxtime_pts,
+            dtype=torch.float64,
+        ):
             value, lyap, weight = self.DDE.integrate(time.item())
             self.mackeyglass_soln[count, 0] = value[0]
             lyaps[count, 0] = lyap[0]
             lyaps_weights[count, 0] = weight
             count += 1
 
         # Total variance of the generated Mackey-Glass time-series
         self.total_var = torch.var(self.mackeyglass_soln[:, 0], True)
 
         # Estimate Lyapunov exponent
         self.lyap_exp = ((lyaps.T @ lyaps_weights) / lyaps_weights.sum()).item()
 
         # pad the soln with preceding zeroes for lookback window
         self.mackeyglass_soln = torch.cat(
-            (torch.zeros((self.bin_window - 1, 1), dtype=torch.float64), self.mackeyglass_soln), 0)
+            (
+                torch.zeros((self.bin_window - 1, 1), dtype=torch.float64),
+                self.mackeyglass_soln,
+            ),
+            0,
+        )
 
     def split_data(self):
-        """ Generate training and testing indices.
-        """
+        """Generate training and testing indices."""
         self.ind_train = torch.arange(0, self.traintime_pts)
         self.ind_test = torch.arange(self.traintime_pts, self.maxtime_pts - 1)
 
     def __len__(self):
-        """ Returns number of samples in dataset.
+        """
+        Returns number of samples in dataset.
 
         Returns:
             int: number of samples in dataset
+
         """
         return len(self.mackeyglass_soln) - 1
 
     def __getitem__(self, idx):
-        """ Getter method for dataset.
+        """
+        Getter method for dataset.
 
         Args:
             idx (int or tensor): index(s) of sample(s) to return
 
         Returns:
             sample (tensor): individual data sample, shape=(timestamps, features)=(1,1)
             target (tensor): corresponding next state of the system, shape=(label,)=(1,)
+
         """
         # using Subset with list of indices
         if isinstance(idx, list) or (isinstance(idx, torch.Tensor) and idx.ndim > 0):
             # return in format (batch, bin_window, feature)
-            data = [self.mackeyglass_soln[i:i + self.bin_window, :] for i in idx]
+            data = [self.mackeyglass_soln[i : i + self.bin_window, :] for i in idx]
             sample = torch.stack(data)
 
         # idx is an integer
         else:
-            sample = self.mackeyglass_soln[idx:idx + self.bin_window, :]
+            sample = self.mackeyglass_soln[idx : idx + self.bin_window, :]
 
-        target = self.mackeyglass_soln[idx + self.bin_window, :]  # add to account for pre-padding
+        target = self.mackeyglass_soln[
+            idx + self.bin_window, :
+        ]  # add to account for pre-padding
 
         return sample, target
```

### Comparing `neurobench-1.0.2/neurobench/datasets/megapixel_automotive.py` & `neurobench-1.0.3/neurobench/datasets/megapixel_automotive.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,115 +8,128 @@
 import torch
 
 """
 The following files in the precomputed dataset test folder do not have 
 corresponding label files, for now they are skipped.
 """
 skip_files = [
-    'moorea_2019-06-17_test_01_000_1769500000_1829500000.h5',
-    'moorea_2019-06-14_000_549500000_609500000.h5',
-    'moorea_2019-06-14_000_1220500000_1280500000.h5',
-    'moorea_2019-06-26_test_02_000_1708500000_1768500000.h5',
+    "moorea_2019-06-17_test_01_000_1769500000_1829500000.h5",
+    "moorea_2019-06-14_000_549500000_609500000.h5",
+    "moorea_2019-06-14_000_1220500000_1280500000.h5",
+    "moorea_2019-06-26_test_02_000_1708500000_1768500000.h5",
 ]
 
+
 def create_class_lookup(wanted_keys=[]):
-    """Source code modified from metavision_ml.data.box_processing.create_class_lookup to avoid
-    having extraneous label map json file.
-    """
-    label_dic = {0: "pedestrian", 1: "two wheeler", 2: "car", 
-                  3: "truck", 4: "bus", 5: "traffic sign", 
-                  6: "traffic light"}
+    """Source code modified from metavision_ml.data.box_processing.create_class_lookup
+    to avoid having extraneous label map json file."""
+    label_dic = {
+        0: "pedestrian",
+        1: "two wheeler",
+        2: "car",
+        3: "truck",
+        4: "bus",
+        5: "traffic sign",
+        6: "traffic light",
+    }
 
     # we take maximum class id + 1 because of class id 0
     size = max(label_dic.keys()) + 1
 
     # check that all wanted classes are inside the dataset
     classes = label_dic.values()
     if wanted_keys:
-        assert any(item != 'empty' for item in wanted_keys)
+        assert any(item != "empty" for item in wanted_keys)
         for key in wanted_keys:
             assert key in classes, "key '{}' not found in the dataset".format(key)
     else:
         # we filter out 'empty' because this is used to annotate empty frames
-        wanted_keys = [label for label in classes if label != 'empty']
+        wanted_keys = [label for label in classes if label != "empty"]
 
     wanted_map = {label: idx for idx, label in enumerate(wanted_keys)}
     class_lookup = np.full(size, -1)
     for src_idx in range(size):
         if src_idx not in label_dic:
             continue
         src_label = label_dic[src_idx]
         if src_label not in wanted_keys:
             continue
         class_lookup[src_idx] = wanted_map[src_label] + 1
     return class_lookup
 
+
 class Gen4DetectionDataLoader(SequentialDataLoader):
-    """NeuroBench DataLoader for Gen4 pre-computed dataset
+    """
+    NeuroBench DataLoader for Gen4 pre-computed dataset.
 
-    The default parameters are set for the Gen4 Histograms dataset, which can be downloaded from
+    The default parameters are set for the Gen4 Histograms dataset, which can be
+    downloaded from
     https://docs.prophesee.ai/stable/datasets.html#precomputed-datasets
     but you can change that easily by downloading one of the other pre-computed datasets and
     changing the preprocess_function_name and channels parameters accordingly.
 
     Once downloaded, extract the zip folder and set the dataset_path parameter to the path of the extracted folder.
+
     """
+
     def __init__(
         self,
         dataset_path="data/Gen 4 Histograms",
         split="testing",
         batch_size: int = 4,
         num_tbins: int = 12,
         preprocess_function_name="histo",
         delta_t=50000,
         channels=2,  # histograms have two channels
         height=360,
         width=640,
         max_incr_per_pixel=5,
         class_selection=["pedestrian", "two wheeler", "car"],
-        num_workers=4
+        num_workers=4,
     ):
-        """ Initializes the Gen4DetectionDataLoader dataloader.
+        """
+        Initializes the Gen4DetectionDataLoader dataloader.
 
         Args:
             dataset_path: path to the dataset folder
             split: split to use, can be 'training', 'validation' or 'testing'
             batch_size: batch size
             num_tbins: number of time bins in a mini batch
             preprocess_function_name: name of the preprocessing function to use, 'histo' by default. Can be that are listed under https://docs.prophesee.ai/stable/api/python/ml/preprocessing.html
             delta_t: time interval between two consecutive frames
             channels: number of channels in the input data, 2 by default for histograms
             height: height of the input data
             width: width of the input data
             max_incr_per_pixel: maximum number of events per pixel
             class_selection: list of classes to use
             num_workers: number of workers for the dataloader
+
         """
 
         self.dataset_path = Path(dataset_path)
         self.files_train = glob.glob(str(self.dataset_path / "train" / "*.h5"))
         self.files_val = glob.glob(str(self.dataset_path / "val" / "*.h5"))
         self.files_test = glob.glob(str(self.dataset_path / "test" / "*.h5"))
 
         # patch to remove files without labels
         for file in self.files_test:
-            if file.split('/')[-1] in skip_files:
+            if file.split("/")[-1] in skip_files:
                 self.files_test.remove(file)
 
         self.split = split
         self.data = {
             "training": self.files_train,
             "validation": self.files_val,
             "testing": self.files_test,
         }[split]
         self.channels = channels
         self.height = height
         self.width = width
         self.class_selection = class_selection
-        
+
         # class_lookup = box_api.create_class_lookup(label_map_path, class_selection)
         class_lookup = create_class_lookup(class_selection)
 
         self.kw_args = dict(
             delta_t=delta_t,
             preprocess_function_name=preprocess_function_name,
             array_dim=[num_tbins, channels, height, width],
@@ -130,33 +143,36 @@
             num_workers=num_workers,
             padding=True,
             preprocess_kwargs={"max_incr_per_pixel": max_incr_per_pixel},
         )
         super().__init__(self.data, **self.kw_args)
 
     def __next__(self):
-        """ Override the metavision dataloader to reformat data.
+        """
+        Override the metavision dataloader to reformat data.
 
         Errata: note that labels do not fit the usual format of tensor with batch as first dimension,
         since the number of boxes per frame is variable.
 
         Returns:
             inputs (tensor): sample data, shape (batch, timesteps, channels, height, width)
             labels (list[list[bboxes]]): labels of the shape (timesteps, batch, num bounding boxes)
             kwargs (dict): dictionary of metadata with keys 'mask_keep_memory', 'frame_is_labeled', 'video_infos'
 
         """
         data_dict = super().__next__()
 
         inputs = data_dict["inputs"]
-        inputs = inputs.permute(1, 0, 2, 3, 4) # batch, timesteps, channels, height, width
+        inputs = inputs.permute(
+            1, 0, 2, 3, 4
+        )  # batch, timesteps, channels, height, width
 
         # list of list of bboxes, shape (timesteps, batch, num bbox)
         # where bbox is structured np array
         labels_bboxes = data_dict["labels"]
 
         del data_dict["inputs"]
         del data_dict["labels"]
 
         kwargs = data_dict
 
-        return inputs, labels_bboxes, kwargs
+        return inputs, labels_bboxes, kwargs
```

### Comparing `neurobench-1.0.2/neurobench/datasets/primate_reaching.py` & `neurobench-1.0.3/neurobench/datasets/primate_reaching.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,68 +16,85 @@
 
 # The spikes recorded in the Primate Reaching datasets have an interval of 4ms.
 SAMPLING_RATE = 4e-3
 
 
 class PrimateReaching(NeuroBenchDataset):
     """
-        Dataset for the Primate Reaching Task
+    Dataset for the Primate Reaching Task.
 
-        The Dataset can be downloaded from the following website:
-        https://zenodo.org/record/583331
+    The Dataset can be downloaded from the following website:
+    https://zenodo.org/record/583331
 
-        For this task, the following files are selected:
-        1. indy_20170131_02.mat
-        2. indy_20160630_01.mat
-        3. indy_20160622_01.mat
-        4. loco_20170301_05.mat
-        5. loco_20170215_02.mat
-        6. loco_20170210_03.mat
+    For this task, the following files are selected:
+    1. indy_20170131_02.mat
+    2. indy_20160630_01.mat
+    3. indy_20160622_01.mat
+    4. loco_20170301_05.mat
+    5. loco_20170215_02.mat
+    6. loco_20170210_03.mat
 
-        The description of the structure of the dataset can be found on the website
-        in the section: Variable names.
+    The description of the structure of the dataset can be found on the website
+    in the section: Variable names.
+
+    Once these .mat files are downloaded, store them in the same directory.
 
-        Once these .mat files are downloaded, store them in the same directory.
     """
+
     url = "https://zenodo.org/record/583331/files/"
 
     md5s = {
         "indy_20170131_02.mat": "2790b1c869564afaa7772dbf9e42d784",
         "indy_20160630_01.mat": "197413a5339630ea926cbd22b8b43338",
         "indy_20160622_01.mat": "c33d5fff31320d709d23fe445561fb6e",
         "loco_20170301_05.mat": "47342da09f9c950050c9213c3df38ea3",
         "loco_20170215_02.mat": "739b70762d838f3a1f358733c426bb02",
         "loco_20170210_03.mat": "4cae63b58c4cb9c8abd44929216c703b",
     }
 
-    def __init__(self, file_path, filename, num_steps, train_ratio=0.8,
-                 biological_delay=0, spike_sorting=False, stride=0.004, bin_width=0.028,
-                 max_segment_length=2000, split_num=1, remove_segments_inactive=False, 
-                 download=True):
-
-        """
-            Initialises the Dataset for the Primate Reaching Task.
+    def __init__(
+        self,
+        file_path,
+        filename,
+        num_steps,
+        train_ratio=0.8,
+        label_series=False,
+        biological_delay=0,
+        spike_sorting=False,
+        stride=0.004,
+        bin_width=0.028,
+        max_segment_length=2000,
+        split_num=1,
+        remove_segments_inactive=False,
+        download=True,
+    ):
+        """
+        Initialises the Dataset for the Primate Reaching Task.
+
+        Args:
+            file_path (str): The path to the directory storing the matlab files.
+            filename (str): The name of the file that will be loaded.
+            num_steps (int): Number of consecutive timesteps that are included per sample.
+                             In the real-time case, this should be 1.
+            train_ratio (float): ratio for how the dataset will be split into training/(val+test) set.
+                                 Default is 0.8 (80% of data is training).
+            label_series (bool): Whether the labels are series or not. Useful for training with multiple
+                                 timesteps. Default is False.
+            biological_delay (int): How many steps of delay is to be applied to the dataset. Default is 0
+                                    i.e. no delay applied.
+            spike_sorting (bool): Apply spike sorting for processing raw spike data. Default is False.
+            stride (float):  How many steps are taken when moving the bin_window. Default is 0.004 (4ms).
+            bin_width (float): The size of the bin_window. Default is 0.028 (28ms).
+            max_segment_length: Define the upper limits of a segment. Default is 2000 data points (8s)
+            split_num (int): The number of chunks to break the timeseries into. Default is 1 (no splits).
+            remove_segments_inactive (bool): Whether to remove segments longer than max_segment_length,
+                                             which represent subject inactivity. Default is False.
+            download (bool): If True, downloads the dataset from the internet and puts it in root
+                             directory. If dataset is already downloaded, it will not be downloaded again.
 
-            Args:
-                file_path (str): The path to the directory storing the matlab files.
-                filename (str): The name of the file that will be loaded.
-                num_steps (int): number of timesteps the data will be split into.
-                train_ratio (float): ratio for how the dataset will be split into training/(val+test) set.
-                                     Default is 0.8 (80% of data is training).
-                biological_delay (int): How many steps of delay is to be applied to the dataset. Default is 0
-                                        i.e. no delay applied.
-                spike_sorting (bool): Apply spike sorting for processing raw spike data. Default is False.
-                stride (float):  How many steps are taken when moving the bin_window. Default is 0.004 (4ms).
-                bin_width (float): The size of the bin_window. Default is 0.028 (28ms).
-                max_segment_length: Define the upper limits of a segment. Default is 2000 data points (8s)
-                split_num (int): The number of chunks to break the timeseries into. Default is 1 (no splits).
-                remove_segments_inactive (bool): Whether to remove segments longer than max_segment_length,
-                                                 which represent subject inactivity. Default is False.
-                download (bool): If True, downloads the dataset from the internet and puts it in root 
-                                 directory. If dataset is already downloaded, it will not be downloaded again.
         """
         self.url = "https://zenodo.org/record/583331/files/"
 
         self.md5s = {
             "indy_20170131_02.mat": "2790b1c869564afaa7772dbf9e42d784",
             "indy_20160630_01.mat": "197413a5339630ea926cbd22b8b43338",
             "indy_20160622_01.mat": "c33d5fff31320d709d23fe445561fb6e",
@@ -87,37 +104,39 @@
         }
 
         # The samples and labels of the dataset
         self.samples = None
         self.labels = None
 
         # used for input data file management
-        self.filename = filename if filename[-4:] == '.mat' else filename + ".mat"
+        self.filename = filename if filename[-4:] == ".mat" else filename + ".mat"
         self.file_path = os.path.join(file_path, self.filename)
 
         if download:
             self.download()
-        
+
         # test filepath
         assert os.path.exists(self.file_path)
 
         # related to processing of spike data
         self.spike_sorting = spike_sorting
         self.delay = biological_delay
         self.stride = stride
         self.bin_width = bin_width
         self.num_steps = num_steps
         self.train_ratio = train_ratio
+        self.label_series = label_series
         self.ratio = int(np.round(self.bin_width / SAMPLING_RATE))
 
         # test parameters
         assert self.delay >= 0
         assert self.stride >= SAMPLING_RATE
-        assert self.bin_width >= SAMPLING_RATE, \
-            "The binning window has to be greater than the sampling size (i.e. 0.004s)"
+        assert (
+            self.bin_width >= SAMPLING_RATE
+        ), "The binning window has to be greater than the sampling size (i.e. 0.004s)"
         assert self.num_steps >= 1
         assert 0 <= self.train_ratio <= 1
 
         # Defines the beginning and end of each segment.
         self.start_end_indices = None
         self.time_segments = None
 
@@ -131,88 +150,91 @@
         self.ind_train, self.ind_val, self.ind_test = [], [], []
 
         if "indy" in filename:
             self.input_feature_size = 96
         elif "loco" in filename:
             self.input_feature_size = 192
         else:
-            raise ValueError("Unexpected filename. Filename should be of either indy or loco")
-    
+            raise ValueError(
+                "Unexpected filename. Filename should be of either indy or loco"
+            )
+
         self.load_data()
 
         if self.delay > 0:
             self.apply_delay()
 
         if remove_segments_inactive and self.max_segment_length > 0:
             self.valid_segments = self.remove_segments_by_length()
         else:
             self.valid_segments = np.arange(self.time_segments.shape[0])
-        
+
         self.split_data()
 
     def __len__(self):
         return len(self.ind_train) + len(self.ind_test) + len(self.ind_val)
-    
+
     def __getitem__(self, idx):
-        """
-            Getter method of the dataloader
-        """
+        """Getter method of the dataloader."""
         # compute indices of congruent binning windows
         mask = idx - np.arange(self.num_steps) * self.ratio
-        return self.samples[:, mask].transpose(0, 1), self.labels[:, idx]
-    
+        if self.label_series:
+            samples = self.samples[:, mask].transpose(0, 1)
+            labels = self.labels[:, mask].transpose(0, 1)
+            return samples, labels
+        else:
+            return self.samples[:, mask].transpose(0, 1), self.labels[:, idx]
+
     def _check_exists(self, file_path, md5) -> bool:
-        return check_integrity(file_path, md5) 
-    
-    
+        return check_integrity(file_path, md5)
+
     def download(self):
         """Download the Primate Reaching data if it doesn't exist already."""
         md5 = self.md5s[self.filename]
-        
+
         if self._check_exists(self.file_path, md5):
             return
 
         os.makedirs(os.path.dirname(self.file_path), exist_ok=True)
-        
+
         # download file
         url = f"{self.url}{self.filename}"
         try:
             print(f"Downloading {url}")
             download_url(url, self.file_path, md5=md5)
         except URLError as error:
             print(f"Failed to download (trying next):\n{error}")
         finally:
             print()
-        
+
     def load_data(self):
-        """
-            Load the data from the matlab file and spike data 
-            if spike data has been processed and stored already
-        """
+        """Load the data from the matlab file and spike data if spike data has been
+        processed and stored already."""
         # Assume input is the original dataset, instead of the reconstructed one
         print(f"Loading {self.filename}")
         dataset = h5py.File(self.file_path, "r")
 
         # extract data from datafile
-        spikes = dataset["spikes"][()]  # Get the reference object's locations in the HDF5/mat file
+        spikes = dataset["spikes"][
+            ()
+        ]  # Get the reference object's locations in the HDF5/mat file
         cursor_pos = dataset["cursor_pos"][()]
         target_pos = dataset["target_pos"][()]
         t = np.squeeze(dataset["t"][()])
         new_t = np.arange(t[0] - self.bin_width, t[-1], SAMPLING_RATE)
 
         # Define the segments' start & end indices
         self.start_end_indices = np.array(self.get_flag_index(target_pos))
         self.time_segments = np.array(self.split_into_segments(self.start_end_indices))
 
         spike_train = np.zeros((*spikes.shape, len(new_t)), dtype=np.int8)
 
         # iterate over hdf5 dataframe and preprocess data
         for row_idx, row in enumerate(spikes):
             for col_idx, element in enumerate(row):
-
                 # get indices of spikes and convert data to spike train
                 if isinstance(element, np.ndarray):
                     bins, _ = np.histogram(element, bins=new_t.squeeze())
                 else:
                     bins, _ = np.histogram(dataset[element][()], bins=new_t.squeeze())
 
                 # histogram is assigns spikes to lower bound of binning window, therefor increment by one to shift to
@@ -229,85 +251,99 @@
             spike_train = spike_train.transpose()
         else:
             # combine units into channels
             spike_train = np.bitwise_or.reduce(spike_train, axis=0)
 
         # use convolution to compute binning window
         if self.ratio != 1:
-            binned_spike_train = convolve2d(spike_train, np.ones((1, self.ratio)), mode='valid')
+            binned_spike_train = convolve2d(
+                spike_train, np.ones((1, self.ratio)), mode="valid"
+            )
         else:
             binned_spike_train = spike_train
 
         # Dimensions: (channels x timesteps)
         self.samples = torch.from_numpy(binned_spike_train).float()
         # Dimensions: (nr_features x timesteps)
         self.labels = torch.from_numpy(cursor_pos).float()
 
         # convert position to velocity
         self.labels = torch.gradient(self.labels, dim=1)[0]
-    
+
     def apply_delay(self):
-        """
-            shift the labels by the delay to account for the biological delay between spikes and movement onset
-        """
+        """Shift the labels by the delay to account for the biological delay between
+        spikes and movement onset."""
         # Dimension: No_of_Channels*No_of_Records
-        self.samples = self.samples[:, :-self.delay]
-        self.labels = self.labels[:, self.delay:]
+        self.samples = self.samples[:, : -self.delay]
+        self.labels = self.labels[:, self.delay :]
 
     def split_data(self):
-        """
-            Split segments into training/validation/test set
-        """
+        """Split segments into training/validation/test set."""
         # This is No. of chunks
         split_num = self.split_num
         total_segments = self.time_segments.shape[0]
-        sub_length = int(total_segments / split_num)  # This is no of segments in each chunk
+        sub_length = int(
+            total_segments / split_num
+        )  # This is no of segments in each chunk
         stride = int(self.stride / SAMPLING_RATE)
         # print(total_segments, sub_length)
 
         train_len = math.floor(self.train_ratio * sub_length)
         val_len = math.floor((sub_length - train_len) / 2)
 
         offset = int(np.round(self.bin_width / SAMPLING_RATE)) * self.num_steps
 
         # split the data into 4 equal parts
         # for each part, split the data according to training, testing and validation split
         for split_no in range(split_num):
             for i in range(sub_length):
                 # Each segment's Dimension is: No_of_Probes * No_of_Recording
                 if i < train_len and i in self.valid_segments:
-                    self.ind_train += list(np.arange(offset + self.time_segments[split_no * sub_length + i, 0],
-                                                     self.time_segments[split_no * sub_length + i, 1], stride))
+                    self.ind_train += list(
+                        np.arange(
+                            offset + self.time_segments[split_no * sub_length + i, 0],
+                            self.time_segments[split_no * sub_length + i, 1],
+                            stride,
+                        )
+                    )
                 elif train_len <= i < train_len + val_len and i in self.valid_segments:
-                    self.ind_val += list(np.arange(offset + self.time_segments[split_no * sub_length + i, 0],
-                                                   self.time_segments[split_no * sub_length + i, 1], stride))
+                    self.ind_val += list(
+                        np.arange(
+                            offset + self.time_segments[split_no * sub_length + i, 0],
+                            self.time_segments[split_no * sub_length + i, 1],
+                            stride,
+                        )
+                    )
                 elif i in self.valid_segments:
-                    self.ind_test += list(np.arange(offset + self.time_segments[split_no * sub_length + i, 0],
-                                                    self.time_segments[split_no * sub_length + i, 1], stride))
+                    self.ind_test += list(
+                        np.arange(
+                            offset + self.time_segments[split_no * sub_length + i, 0],
+                            self.time_segments[split_no * sub_length + i, 1],
+                            stride,
+                        )
+                    )
 
     def remove_segments_by_length(self):
-        """
-            remove the segments where its duration exceeds the limit set by
-            max_segment_length
-        """
-        return np.nonzero(self.time_segments[:, 1] - self.time_segments[:, 0] < self.max_segment_length)[0]
+        """Remove the segments where its duration exceeds the limit set by
+        max_segment_length."""
+        return np.nonzero(
+            self.time_segments[:, 1] - self.time_segments[:, 0]
+            < self.max_segment_length
+        )[0]
 
     @staticmethod
     def split_into_segments(indices):
-        """
-            Combine the start and end index into a NumPy array.
-        """
+        """Combine the start and end index into a NumPy array."""
         start_end = np.array([indices[:-1], indices[1:]])
 
         return np.transpose(start_end)
 
     @staticmethod
     def get_flag_index(target_pos):
-        """
-            Find where each segment begins and ends
-        """
-        target_diff = np.diff(target_pos, axis=1, append=target_pos[:, -1].reshape(2, 1))
+        """Find where each segment begins and ends."""
+        target_diff = np.diff(
+            target_pos, axis=1, append=target_pos[:, -1].reshape(2, 1)
+        )
 
         indices = np.nonzero(np.sum(np.abs(target_diff), axis=0))[0]
 
         return indices
-
```

### Comparing `neurobench-1.0.2/neurobench/datasets/speech_commands.py` & `neurobench-1.0.3/neurobench/datasets/speech_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,96 @@
 import torch
 import os
 from glob import glob
 from torchaudio.datasets import SPEECHCOMMANDS
 from .dataset import NeuroBenchDataset
 
+
 class SpeechCommands(NeuroBenchDataset, SPEECHCOMMANDS):
-    """ Speech commands dataset v0.02 with 35 keywords.
+    """
+    Speech commands dataset v0.02 with 35 keywords.
 
     Wraps the torchaudio SPEECHCOMMANDS dataset.
+
     """
 
-    def __init__(self, path, subset:str=None, truncate_or_pad_to_1s=True, ):
-        """ Initializes the SpeechCommands dataset.
+    def __init__(
+        self,
+        path,
+        subset: str = None,
+        truncate_or_pad_to_1s=True,
+    ):
+        """
+        Initializes the SpeechCommands dataset.
 
         Args:
             path (str): path to the root directory of the dataset
             subset (str, optional): one of "training", "validation", or "testing". Defaults to None.
             truncate_or_pad_to_1s (bool, optional): whether to truncate or pad samples to 1s. Defaults to True.
+
         """
         os.makedirs(path, exist_ok=True)
         SPEECHCOMMANDS.__init__(self, path, download=True, subset=subset)
         self.truncate_or_pad_to_1s = truncate_or_pad_to_1s
 
         # convert labels to indices
-        self.labels = sorted(glob("*/", root_dir=os.path.join(path, "SpeechCommands", "speech_commands_v0.02")))
+        self.labels = sorted(
+            glob(
+                "*/",
+                root_dir=os.path.join(path, "SpeechCommands", "speech_commands_v0.02"),
+            )
+        )
         # subtract 1 to account for _background_noise_
-        self.labels = {key[:-1]: idx-1 for idx, key in enumerate(self.labels)}
+        self.labels = {key[:-1]: idx - 1 for idx, key in enumerate(self.labels)}
 
     def __getitem__(self, idx):
-        """ Getter method for dataset.
+        """
+        Getter method for dataset.
 
-        Args:  
+        Args:
             idx (int): index of sample to return
         Returns:
             waveform (torch.Tensor): waveform of audio sample
             label (torch.Tensor): label index of audio sample
+
         """
-        waveform, sample_rate, label, speaker_id, utterance_num =  SPEECHCOMMANDS.__getitem__(self, idx)
+        (
+            waveform,
+            sample_rate,
+            label,
+            speaker_id,
+            utterance_num,
+        ) = SPEECHCOMMANDS.__getitem__(self, idx)
         if self.truncate_or_pad_to_1s:
             if waveform.shape[0] > sample_rate:
                 waveform = waveform[:sample_rate]
             else:
                 temp_waveform = torch.zeros((sample_rate,))
-                temp_waveform[:waveform.numel()] = waveform
+                temp_waveform[: waveform.numel()] = waveform
                 waveform = temp_waveform
 
         waveform = waveform.unsqueeze(-1)
         label = self.label_to_index(label)
 
         return waveform, label
-    
+
     def label_to_index(self, label):
-        """ Converts a label to an index.
+        """
+        Converts a label to an index.
 
-        Args: 
+        Args:
             label (str): label of audio sample
-        Returns:   
+        Returns:
             torch.Tensor: index of label
+
         """
         return torch.tensor(self.labels[label])
 
     def __len__(self):
-        """ Returns number of samples in dataset.
+        """
+        Returns number of samples in dataset.
 
         Returns:
             int: number of samples in dataset
+
         """
-        return SPEECHCOMMANDS.__len__(self)
+        return SPEECHCOMMANDS.__len__(self)
```

### Comparing `neurobench-1.0.2/neurobench/datasets/utils.py` & `neurobench-1.0.3/neurobench/datasets/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,36 +55,44 @@
             if not chunk:
                 continue
 
             fh.write(chunk)
             pbar.update(len(chunk))
 
 
-def _urlretrieve(url, filename, chunk_size=1024*32):
-    with urllib.request.urlopen(urllib.request.Request(url, headers={"User-Agent": USER_AGENT})) as response:
-        _save_response_content(iter(lambda: response.read(chunk_size), b""), filename, length=response.length)
+def _urlretrieve(url, filename, chunk_size=1024 * 32):
+    with urllib.request.urlopen(
+        urllib.request.Request(url, headers={"User-Agent": USER_AGENT})
+    ) as response:
+        _save_response_content(
+            iter(lambda: response.read(chunk_size), b""),
+            filename,
+            length=response.length,
+        )
 
 
 def _get_redirect_url(url, max_hops=3):
     initial_url = url
     headers = {"Method": "HEAD", "User-Agent": USER_AGENT}
 
     for _ in range(max_hops + 1):
-        with urllib.request.urlopen(urllib.request.Request(url, headers=headers)) as response:
+        with urllib.request.urlopen(
+            urllib.request.Request(url, headers=headers)
+        ) as response:
             if response.url == url or response.url is None:
                 return url
 
             url = response.url
     else:
         raise RecursionError(
             f"Request to {initial_url} exceeded {max_hops} redirects. The last redirect points to {url}."
         )
 
 
-def calculate_md5(fpath, chunk_size=1024*1024):
+def calculate_md5(fpath, chunk_size=1024 * 1024):
     # Setting the `usedforsecurity` flag does not change anything about the functionality, but indicates that we are
     # not using the MD5 checksum for cryptography. This enables its usage in restricted environments like FIPS.
     if sys.version_info >= (3, 9):
         md5 = hashlib.md5(usedforsecurity=False)
     else:
         md5 = hashlib.md5()
     with open(fpath, "rb") as f:
@@ -102,21 +110,23 @@
         return False
     if md5 is None:
         return True
     return check_md5(fpath, md5)
 
 
 def download_url(url, file_path, md5=None, max_redirect_hops=3):
-    """Download a file from a url and place it in root.
+    """
+    Download a file from a url and place it in root.
 
     Args:
         url (str): URL to download file from
         file_path (str): Full path to the file to be downloaded.
         md5 (str, optional): MD5 checksum of the download. If None, do not check
         max_redirect_hops (int, optional): Maximum number of redirect hops allowed
+
     """
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
     # check if file is already present locally
     if check_integrity(file_path, md5):
         print("Using downloaded and verified file: " + file_path)
         return
@@ -132,15 +142,20 @@
     # download the file
     try:
         print("Downloading " + url + " to " + file_path)
         _urlretrieve(url, file_path)
     except (urllib.error.URLError, OSError) as e:  # type: ignore[attr-defined]
         if url[:5] == "https":
             url = url.replace("https:", "http:")
-            print("Failed download. Trying https -> http instead. Downloading " + url + " to " + file_path)
+            print(
+                "Failed download. Trying https -> http instead. Downloading "
+                + url
+                + " to "
+                + file_path
+            )
             _urlretrieve(url, file_path)
         else:
             raise e
 
     # check integrity of downloaded file
     if not check_integrity(file_path, md5):
         raise RuntimeError("File not found or corrupted.")
```

### Comparing `neurobench-1.0.2/neurobench/models/model.py` & `neurobench-1.0.3/neurobench/models/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,113 +2,125 @@
 import torch
 from neurobench.benchmarks.hooks import ActivationHook
 
 from neurobench.utils import activation_modules
 
 
 class NeuroBenchModel:
-    """ Abstract class for NeuroBench models. Individual model frameworks are
-    responsible for defining model inference.
+    """
+    Abstract class for NeuroBench models.
+
+    Individual model frameworks are responsible for defining model inference.
+
     """
 
     def __init__(self, net):
-        """ Init using a trained network
-        
+        """
+        Init using a trained network.
+
         Args:
             net: A trained network
+
         """
         self.activation_modules = activation_modules()
         self.activation_hooks = []
         self.connection_hooks = []
         self.first_layer = None
 
-        self.supported_layers = (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, 
-                        torch.nn.Conv3d, torch.nn.RNNBase, torch.nn.RNNCellBase,)
-
+        self.supported_layers = (
+            torch.nn.Linear,
+            torch.nn.Conv2d,
+            torch.nn.Conv1d,
+            torch.nn.Conv3d,
+            torch.nn.RNNBase,
+            torch.nn.RNNCellBase,
+        )
 
     def __call__(self, batch):
-        """ Includes the whole pipeline from data to inference (output should be same format as targets).
+        """
+        Includes the whole pipeline from data to inference (output should be same format
+        as targets).
 
         Args:
             batch: A batch of data to run inference on
+
         """
-        raise NotImplementedError("Subclasses of NeuroBenchModel should implement __call__")
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchModel should implement __call__"
+        )
 
     def __net__(self):
-        """ Returns the underlying network
-        """
-        raise NotImplementedError("Subclasses of NeuroBenchModel should implement __net__")
+        """Returns the underlying network."""
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchModel should implement __net__"
+        )
 
     def set_first_layer(self, layer):
-        """ Sets the first layer of the network
-        """
+        """Sets the first layer of the network."""
         self.first_layer = layer
-        
+
     def add_activation_module(self, activaton_module):
-        """ Add a cutomized activaton_module that can be detected after running the preprocessing pipeline for detecting activation functions
-        """
+        """Add a cutomized activaton_module that can be detected after running the
+        preprocessing pipeline for detecting activation functions."""
         self.activation_modules.append(activaton_module)
 
     def activation_layers(self):
-        """ Retrieve all the activaton layers of the underlying network (including spiking neuron layers)
-        """
+        """Retrieve all the activaton layers of the underlying network (including
+        spiking neuron layers)"""
+
         def check_if_activation(module):
             for activation_module in self.activation_modules:
                 if isinstance(module, activation_module):
                     return True
 
         def get_activation_layers(parent):
-            """ Returns all the neuro layers
-            """
+            """Returns all the neuro layers."""
             layers = []
             children = parent.children()
             for child in children:
                 if check_if_activation(child):
                     # is an activation module
                     layers.append(child)
                 else:
                     if len(list(child.children())) != 0:
                         # not an activation module and has nested submodules
                         children_layers = get_activation_layers(child)
                         layers.extend(children_layers)
-            
+
             return layers
 
-        
         root = self.__net__()
         layers = get_activation_layers(root)
         return layers
 
     def connection_layers(self):
-        """ Retrieve all the connection layers of the underlying network (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, torch.nn.Conv3d)
-        """
+        """Retrieve all the connection layers of the underlying network
+        (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, torch.nn.Conv3d)"""
         supported_layers = self.supported_layers
-        
+
         def get_connection_layers(parent):
-            """ Returns all the connection layers
-            """
+            """Returns all the connection layers."""
             connection_layers = []
             children = parent.children()
             for child in children:
                 grand_children = list(child.children())
-                if len(grand_children) == 0:  # leaf child  
+                if len(grand_children) == 0:  # leaf child
                     if isinstance(child, supported_layers):
-                            connection_layers.append(child)
+                        connection_layers.append(child)
 
                 else:
                     children_layers = get_connection_layers(child)
                     connection_layers.extend(children_layers)
-            
+
             return connection_layers
-        
+
         root = self.__net__()
         connection_layers = get_connection_layers(root)
         return connection_layers
-    
+
     def reset_hooks(self):
-        """ Resets all the hooks (activation hooks and connection hooks)
-        """
+        """Resets all the hooks (activation hooks and connection hooks)"""
         for hook in self.activation_hooks:
             hook.reset()
 
         for hook in self.connection_hooks:
             hook.reset()
```

### Comparing `neurobench-1.0.2/neurobench/models/snntorch_models.py` & `neurobench-1.0.3/neurobench/models/snntorch_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 import torch
 
 import snntorch as snn
 from snntorch import utils
 
 from .model import NeuroBenchModel
 
+
 class SNNTorchModel(NeuroBenchModel):
-    """ The SNNTorch class wraps the forward pass of the SNNTorch framework and ensures that spikes are in the correct 
-    format for downstream NeuroBench components.
-    """
+    """The SNNTorch class wraps the forward pass of the SNNTorch framework and ensures
+    that spikes are in the correct format for downstream NeuroBench components."""
+
     def __init__(self, net):
-        """ Init using a trained network.
+        """
+        Init using a trained network.
 
         Args:
             net: A trained SNNTorch network.
+
         """
         super().__init__(net)
-        
+
         self.net = net
         self.net.eval()
 
         # add snntorch neuron layers as activation modules
         self.add_activation_module(snn.SpikingNeuron)
 
     def __call__(self, data):
-        """ Executes the forward pass of SNNTorch models on data that follows the
-        NeuroBench specification. Ensures spikes are compatible with downstream
-        components.
+        """
+        Executes the forward pass of SNNTorch models on data that follows the NeuroBench
+        specification. Ensures spikes are compatible with downstream components.
 
         Args:
             data: A PyTorch tensor of shape (batch, timesteps, ...)
 
         Returns:
             spikes: A PyTorch tensor of shape (batch, timesteps, ...)
+
         """
         spikes = []
         # utils.reset(self.net) does not seem to delete all traces for the synaptic neuron model
-        if hasattr(self.net, 'reset'):
+        if hasattr(self.net, "reset"):
             self.net.reset()
         else:
             utils.reset(self.net)
         spikes = []
 
         # Data is expected to be shape (batch, timestep, features*)
         for step in range(data.shape[1]):
             spk_out, _ = self.net(data[:, step, ...])
             spikes.append(spk_out)
         spikes = torch.stack(spikes).transpose(0, 1)
         return spikes
 
     def __net__(self):
-        """ Returns the underlying network.
-        """
+        """Returns the underlying network."""
         return self.net
```

### Comparing `neurobench-1.0.2/neurobench/models/torch_model.py` & `neurobench-1.0.3/neurobench/models/torch_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import torch
 from .model import NeuroBenchModel
 
+
 class TorchModel(NeuroBenchModel):
-    """ The TorchModel class wraps an nn.Module.
-    """
+    """The TorchModel class wraps an nn.Module."""
+
     def __init__(self, net):
-        """ Initializes the TorchModel class.
+        """
+        Initializes the TorchModel class.
 
         Args:
             net: A PyTorch nn.Module.
+
         """
         super().__init__(net)
-        
+
         self.net = net
         self.net.eval()
 
     def __call__(self, batch):
-        """ Wraps forward pass of torch.nn model.
+        """
+        Wraps forward pass of torch.nn model.
 
         Args:
             batch: A PyTorch tensor of shape (batch, timesteps, features*)
 
         Returns:
             preds: either a tensor to be compared with targets or passed to
                 NeuroBenchPostProcessors.
+
         """
         return self.net(batch)
 
     def __net__(self):
-        """ Returns the underlying network.
-        """
-        return self.net
+        """Returns the underlying network."""
+        return self.net
```

### Comparing `neurobench-1.0.2/neurobench/postprocessing/postprocessor.py` & `neurobench-1.0.3/neurobench/postprocessing/postprocessor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 import torch
 
-class NeuroBenchPostProcessor():
-    """ Abstract class for NeuroBench postprocessors. Postprocessors take the spiking
-    output from the models and provide several methods of combining them.
-    Individual postprocessors are responsible for implementing init and call 
-    functions.
+
+class NeuroBenchPostProcessor:
+    """
+    Abstract class for NeuroBench postprocessors.
+
+    Postprocessors take the spiking output from the models and provide several methods
+    of combining them. Individual postprocessors are responsible for implementing init
+    and call functions.
+
     """
 
     def __init__(self, args):
-        """ Initialize postprocessor with any parameters needed
+        """
+        Initialize postprocessor with any parameters needed.
 
         Args:
             args: A dictionary of arguments for the postprocessor
+
         """
-        raise NotImplementedError("Subclasses of NeuroBenchPostProcessor should implement __init__")
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchPostProcessor should implement __init__"
+        )
 
     def __call__(self, spikes):
-        """ Process tensor of spiking data of format (batch, timesteps, ...) to 
-        match spikes to ground truth
+        """
+        Process tensor of spiking data of format (batch, timesteps, ...) to match spikes
+        to ground truth.
 
         Args:
             spikes: A torch tensor of spikes output by a NeuroBenchModel of
                 shape (batch, timestep, ...)
+
         """
-        raise NotImplementedError("Subclasses of NeuroBenchPostProcessor should implement __call__")
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchPostProcessor should implement __call__"
+        )
 
 
 def choose_max_count(spikes):
-    """ Returns the class with the highest spike count over the sample
+    """
+    Returns the class with the highest spike count over the sample.
 
     Args:
         spikes: A torch tensor of spikes of shape (batch, timestep, classes)
+
     """
     # Sum across time and return index with highest count
-    return spikes.sum(1).argmax(1) 
+    return spikes.sum(1).argmax(1)
+
 
 def aggregate(spikes):
-    """ Returns the aggregated spikes
+    """
+    Returns the aggregated spikes.
 
     Args:
         spikes: A torch tensor of spikes of shape (batch, timestep, classes)
-    
+
     Returns:
         spikes: A torch tensor of spikes of shape (batch, classes)
+
     """
-    return spikes.sum(1)
+    return spikes.sum(1)
```

### Comparing `neurobench-1.0.2/neurobench/preprocessing/mfcc.py` & `neurobench-1.0.3/neurobench/preprocessing/mfcc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from . import NeuroBenchPreProcessor
 from torchaudio.transforms import MFCC
 import torch
 
 
 class MFCCPreProcessor(NeuroBenchPreProcessor):
-    """ Does MFCC computation on dataset using torchaudio.transforms.MFCC.
-    Call expects loaded .wav data and targets as a tuple (data, targets).
-    Expects sample_rate to be the same for all samples in data.
     """
+    Does MFCC computation on dataset using torchaudio.transforms.MFCC.
+
+    Call expects loaded .wav data and targets as a tuple (data, targets). Expects
+    sample_rate to be the same for all samples in data.
+
+    """
+
     def __init__(
         self,
         sample_rate: int = 16000,
         n_mfcc: int = 40,
         dct_type: int = 2,
         norm: str = "ortho",
         log_mels: bool = False,
         melkwargs: dict = None,
-        device = None,
+        device=None,
     ):
         super(NeuroBenchPreProcessor).__init__()
         """
         Args:
             sample_rate (int, optional): Sample rate of the audio signal. (Default: 16000)
             n_mfcc (int, optional): Number of MFCC coefficients to retain. (Default: 40)
             dct_type (int, optional): Type of DCT (discrete cosine transform) to use. (Default: 2)
@@ -44,22 +48,24 @@
             melkwargs=self.melkwargs,
         )
 
         if device:
             self.mfcc = self.mfcc.to(device)
 
     def __call__(self, dataset):
-        """ Executes the MFCC computation on the dataset.
+        """
+        Executes the MFCC computation on the dataset.
 
         Args:
             dataset (tuple): A tuple of (data, targets).
 
         Returns:
             results: mfcc applied on data
             targets: targets from dataset
+
         """
         self.dataset_validity_check(dataset)
 
         data = dataset[0]
         targets = dataset[1]
         if len(dataset) == 3:
             kwargs = dataset[2]
@@ -68,26 +74,27 @@
 
         if isinstance(data, list):
             data = torch.vstack(data)
 
         # Data is expected in (batch, timesteps, features) format
         if data.dim() == 2:
             data.permute(1, 0)
-        
+
         elif data.dim() == 3:
             data = data.permute(0, 2, 1)
 
         self.results = self.mfcc(data)
 
         if kwargs:
             return self.results, targets, kwargs
         return self.results, targets
 
     @staticmethod
     def dataset_validity_check(dataset):
-        """ Checks if dataset is a tuple with length two.
-        """
+        """Checks if dataset is a tuple with length two."""
         if not isinstance(dataset, tuple):
             raise TypeError("Expected dataset to be tuple")
 
         if not len(dataset) == 2 and not len(dataset) == 3:
-            raise ValueError("Dataset tuple should have values as (data, targets), or (data, targets, kwargs)")
+            raise ValueError(
+                "Dataset tuple should have values as (data, targets), or (data, targets, kwargs)"
+            )
```

### Comparing `neurobench-1.0.2/neurobench/preprocessing/preprocessor.py` & `neurobench-1.0.3/neurobench/preprocessing/preprocessor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,32 @@
-class NeuroBenchPreProcessor():
-    """ Abstract class for NeuroBench pre-processors. Individual pre-processors are
-    responsible for implementing init and call functions.
+class NeuroBenchPreProcessor:
+    """
+    Abstract class for NeuroBench pre-processors.
+
+    Individual pre-processors are responsible for implementing init and call functions.
+
     """
 
     def __init__(self, args):
-        """ Initialize pre-processor with any parameters needed
+        """
+        Initialize pre-processor with any parameters needed.
 
         Args:
             args: Any arguments needed for pre-processing.
+
         """
-        raise NotImplementedError("Subclasses of NeuroBenchPreProcessor should implement __init__")
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchPreProcessor should implement __init__"
+        )
 
     def __call__(self, dataset):
-        """ Process dataset of format (data, targets), or (data, targets, kwargs) to prepare for model inference
+        """
+        Process dataset of format (data, targets), or (data, targets, kwargs) to prepare
+        for model inference.
 
         Args:
             dataset: A tuple of (data, targets) or (data, targets, kwargs) where data is a PyTorch tensor of shape (batch, timesteps, ...)
+
         """
-        raise NotImplementedError("Subclasses of NeuroBenchPreProcessor should implement __call__")
+        raise NotImplementedError(
+            "Subclasses of NeuroBenchPreProcessor should implement __call__"
+        )
```

### Comparing `neurobench-1.0.2/neurobench/preprocessing/speech2spikes.py` & `neurobench-1.0.3/neurobench/preprocessing/speech2spikes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """
-Speech2Spikes License
-Copyright © 2023 Accenture. 
+Speech2Spikes License Copyright © 2023 Accenture.
 
-Speech2Spikes is made available under a proprietary license that permits using, 
-copying, sharing, and making derivative works from Speech2Spikes and its source 
-code for academics/non-commercial purposes only, as long as the above copyright 
+Speech2Spikes is made available under a proprietary license that permits using,
+copying, sharing, and making derivative works from Speech2Spikes and its source
+code for academics/non-commercial purposes only, as long as the above copyright
 notice and this permission notice are included in all copies of the software.
 
-All distribution of Speech2Spikes in any form (source or executable), including 
-any derivative works that you create or to which you contribute, must be under 
-the terms of this license. You must inform recipients that any form of 
-Speech2Spikes and its derivatives is governed by the terms of this license, and 
-how they can obtain a copy of this license and a copy of the source code of 
-Speech2Spikes. You may not attempt to alter or restrict the recipients’ rights 
-in any form. If you are interested to use Speech2Spikes and/or develop 
-derivatives for commercial purposes, licenses can be purchased from Accenture, 
+All distribution of Speech2Spikes in any form (source or executable), including
+any derivative works that you create or to which you contribute, must be under
+the terms of this license. You must inform recipients that any form of
+Speech2Spikes and its derivatives is governed by the terms of this license, and
+how they can obtain a copy of this license and a copy of the source code of
+Speech2Spikes. You may not attempt to alter or restrict the recipients’ rights
+in any form. If you are interested to use Speech2Spikes and/or develop
+derivatives for commercial purposes, licenses can be purchased from Accenture,
 please contact neuromorphic_inquiries@accenture.com for more information.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER 
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-You agree to indemnify and hold Accenture harmless from and against all 
-liabilities, claims and suits and to pay all costs and expenses thereby 
-incurred, including reasonable legal fees and court courts, arising out of, 
-caused by or in any way connected with your use of Speech2Spikes. 
+You agree to indemnify and hold Accenture harmless from and against all
+liabilities, claims and suits and to pay all costs and expenses thereby
+incurred, including reasonable legal fees and court courts, arising out of,
+caused by or in any way connected with your use of Speech2Spikes.
 
 The original code can be found at:
 https://github.com/Accenture/speech2spikes
+
 """
 
 from .preprocessor import NeuroBenchPreProcessor
-
 import torch
 import torchaudio
 
 
 def tensor_to_events(batch, threshold=1, device=None):
-    """ Converts a batch of continuous signals to binary spikes via delta modulation
+    """Converts a batch of continuous signals to binary spikes via delta modulation
     (https://en.wikipedia.org/wiki/Delta_modulation).
 
     Args:
         batch (Tensor): PyTorch tensor of shape (..., timesteps).
         threshold (float): The difference between the residual and signal that
             will be considered an increase or decrease. Defaults to 1.
         device (torch.device, optional): A torch.Device used by PyTorch for the
@@ -66,82 +65,102 @@
             batch[..., t] - levels < -threshold
         ).to(torch.int8)
         levels += events[..., t] * threshold
     return events
 
 
 class S2SPreProcessor(NeuroBenchPreProcessor):
-    """ The SpikeEncoder class manages the conversion from raw audio into spikes
-    and stores the required conversion parameters.
-    """
-    def __init__(self, device=None, transpose=True):
+    """The SpikeEncoder class manages the conversion from raw audio into spikes and
+    stores the required conversion parameters."""
+
+    def __init__(self, device=None, transpose=True, log_offset=1e-6):
         """
         Args:
             device (torch.device, optional): A torch.Device used by PyTorch for the
                 computation. Defaults to None.
+            transpose (bool, optional): Whether to transpose the input tensor before processing.
+                If the input tensor is of shape (batch, channels, timesteps), this should be true.
+            log_offset (float, optional): A small value added to the MelSpectrogram before log is applied
         """
         self.device = device
         self.transpose = transpose
-        self._default_spec_kwargs = {
+        self.log_offset = log_offset
+        self.spec_kwargs = {
             "sample_rate": 16000,
             "n_mels": 20,
             "n_fft": 512,
             "f_min": 20,
             "f_max": 4000,
             "hop_length": 80,
         }
         self.threshold = 1
-        self.transform = torchaudio.transforms.MelSpectrogram(
-            **self._default_spec_kwargs
-        ).to(device)
+        self.transform = torchaudio.transforms.MelSpectrogram(**self.spec_kwargs).to(
+            device
+        )
 
     def __call__(self, batch):
-        """ Converts raw audio data to spikes using Speech2Spikes algorithm
+        """Converts raw audio data to spikes using Speech2Spikes algorithm
         (https://doi.org/10.1145/3584954.3584995)
 
         Args:
             batch: A tuple of data and corresponding targets (data_tensor, targets)
 
         Returns:
             tensors: PyTorch int8 tensor of shape (batch, timesteps, ...)
             targets: A tensor of corresponding targets.
 
         TODO:
             Add support for cumulative sum of features
         """
+        timesteps = batch[0].shape[1]
+
         tensors = batch[0]
         targets = batch[1]
         if len(batch) == 3:
             kwargs = batch[2]
         else:
             kwargs = None
 
         # Tensors will be batch, timestep, channels and need to be transposed
-        
+
         if self.transpose:
             tensors = tensors.transpose(1, 2)
         tensors = self.transform(tensors)
+        if self.log_offset:
+            tensors = tensors + self.log_offset
         tensors = torch.log(tensors)
-        tensors = tensor_to_events(tensors, threshold=self.threshold, device=self.device)
-        tensors = tensors.transpose(1, 3).squeeze() # Transpose back to timestep last
-        
+        tensors = tensor_to_events(
+            tensors, threshold=self.threshold, device=self.device
+        )
+        tensors = tensors.transpose(
+            1, 3
+        ).squeeze()  # Transpose back to batch, timestep, channel
+
+        # torchaudio seems to return one extra timestep, get rid of the zero timestep
+        if tensors.shape[1] == (timesteps / self.spec_kwargs["hop_length"] + 1):
+            tensors = tensors[:, 1:, :]
+
         if kwargs:
             return tensors, targets, kwargs
         else:
             return tensors, targets
 
     def configure(self, threshold=1, **spec_kwargs):
-        """ Allows the user to configure parameters of the S2S class and the
-        MelSpectrogram transform from torchaudio.
+        """
+        Allows the user to configure parameters of the S2S class and the MelSpectrogram
+        transform from torchaudio.
 
         Go to (https://pytorch.org/audio/main/generated/torchaudio.transforms.MelSpectrogram.html)
         for more information on the available transform parameters.
 
         Args:
             threshold (float): The difference between the residual and signal that
                 will be considered an increase or decrease. Defaults to 1.
             **spec_kwargs: Keyword arguments passed to torchaudio's MelSpectrogram.
+
         """
         self.threshold = threshold
 
-        spec_kwargs = {**self._default_spec_kwargs, **spec_kwargs}
-        self.transform = torchaudio.transforms.MelSpectrogram(**spec_kwargs).to(self.device)
+        self.spec_kwargs = {**self.spec_kwargs, **spec_kwargs}
+        self.transform = torchaudio.transforms.MelSpectrogram(**self.spec_kwargs).to(
+            self.device
+        )
```

### Comparing `neurobench-1.0.2/neurobench/utils.py` & `neurobench-1.0.3/neurobench/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,52 @@
 def _lazy_import(package_name, module_name, class_name):
     module = import_module(module_name, package=package_name)
     return getattr(module, class_name)
 
 
 def activation_modules():
     """
-    The activation layers that can be auto-deteced. Every activation layer can only be included once.
+    The activation layers that can be auto-deteced.
+
+    Every activation layer can only be included once.
+
     """
-    return list(set([nn.ReLU,
-                     nn.Sigmoid,
-                     ]))
+    return list(
+        set(
+            [
+                nn.ReLU,
+                nn.Sigmoid,
+            ]
+        )
+    )
 
 
 def check_shape(preds, labels):
-    """ Checks that the shape of the predictions and labels are the same.
-    """
+    """Checks that the shape of the predictions and labels are the same."""
     if preds.shape != labels.shape:
         raise ValueError("preds and labels must have the same shape")
 
 
 def make_binary_copy(layer, all_ones=False):
-    """ Makes a binary copy of the layer. All non 0 entries are made 1.
-        If all_ones is True, then all entries are made 1.
+    """
+    Makes a binary copy of the layer.
+
+    All non 0 entries are made 1. If all_ones is True, then all entries are made 1.
+
     """
     layer_copy = copy.deepcopy(layer)
 
-    stateless_layers = (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, torch.nn.Conv3d)
+    stateless_layers = (
+        torch.nn.Linear,
+        torch.nn.Conv2d,
+        torch.nn.Conv1d,
+        torch.nn.Conv3d,
+    )
     # recurrent_layers = (torch.nn.RNNBase)
-    recurrent_cells = (torch.nn.RNNCellBase)
+    recurrent_cells = torch.nn.RNNCellBase
 
     if isinstance(layer, stateless_layers):
         weights = layer_copy.weight.data
         weights[weights != 0] = int(1)
         if all_ones:
             weights[weights == 0] = int(1)
 
@@ -46,19 +61,18 @@
             biases[biases != 0] = int(1)
             if all_ones:
                 biases[biases == 0] = int(1)
             layer_copy.bias.data = biases
 
         layer_copy.weight.data = weights
 
-
     elif isinstance(layer, recurrent_cells):
-        attribute_names = ['weight_ih', 'weight_hh']
+        attribute_names = ["weight_ih", "weight_hh"]
         if layer.bias:
-            attribute_names += ['bias_ih', 'bias_hh']
+            attribute_names += ["bias_ih", "bias_hh"]
         # if layer.proj_size > 0: # it is lstm
         # 	attribute_names += ['weight_hr']
 
         for attr in attribute_names:
             with torch.no_grad():
                 attr_val = getattr(layer_copy, attr)
                 attr_val[attr_val != 0] = int(1)
@@ -66,91 +80,97 @@
                     attr_val[attr_val == 0] = int(1)
                 setattr(layer_copy, attr, attr_val)
 
     return layer_copy
 
 
 def make_ones_copy(layer):
-    """ Makes a ones copy of the layer. All entries are made 1.
+    """
+    Makes a ones copy of the layer.
+
+    All entries are made 1.
+
     """
     layer_copy = copy.deepcopy(layer)
 
-    stateless_layers = (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, torch.nn.Conv3d)
+    stateless_layers = (
+        torch.nn.Linear,
+        torch.nn.Conv2d,
+        torch.nn.Conv1d,
+        torch.nn.Conv3d,
+    )
     # recurrent_layers = (torch.nn.RNNBase)
-    recurrent_cells = (torch.nn.RNNCellBase)
+    recurrent_cells = torch.nn.RNNCellBase
 
     if isinstance(layer, stateless_layers):
         weights = layer_copy.weight.data
         weights[weights != 0] = int(1)
         weights[weights == 0] = int(1)
 
         if layer.bias is not None:
             biases = layer_copy.bias.data
             biases[biases != 0] = int(1)
             biases[biases == 0] = int(1)
             layer_copy.bias.data = biases
 
         layer_copy.weight.data = weights
 
-
     elif isinstance(layer, recurrent_cells):
-        attribute_names = ['weight_ih', 'weight_hh']
+        attribute_names = ["weight_ih", "weight_hh"]
         if layer.bias:
-            attribute_names += ['bias_ih', 'bias_hh']
+            attribute_names += ["bias_ih", "bias_hh"]
         # if layer.proj_size > 0: # it is lstm
         # 	attribute_names += ['weight_hr']
 
         for attr in attribute_names:
             with torch.no_grad():
                 attr_val = getattr(layer_copy, attr)
                 attr_val[attr_val != 0] = int(1)
                 attr_val[attr_val == 0] = int(1)
                 setattr(layer_copy, attr, attr_val)
 
     return layer_copy
 
 
 def cylce_tuple(tup):
-    """ Returns a copy of the tuple with binary elements
-    """
+    """Returns a copy of the tuple with binary elements."""
     tup_copy = []
     for t in tup:
         if isinstance(t, tuple):
             tup_copy.append(cylce_tuple(t))
         elif t is not None:
             t = t.detach().clone()
             t[t != 0] = 1
             tup_copy.append(t)
     return tuple(tup_copy)
 
 
 def cylce_tuple_ones(tup):
-    """ Returns a copy of the tuple with ones elements
-    """
+    """Returns a copy of the tuple with ones elements."""
     tup_copy = []
     for t in tup:
         if isinstance(t, tuple):
             tup_copy.append(cylce_tuple(t))
         elif t is not None:
             t = t.detach().clone()
             t[t != 0] = 1
             t[t == 0] = 1
             tup_copy.append(t)
     return tuple(tup_copy)
 
 
 def binary_inputs(inputs, all_ones=False):
-    """ Returns a copy of the inputs with binary elements, all ones if all_ones is True"""
+    """Returns a copy of the inputs with binary elements, all ones if all_ones is
+    True."""
     in_states = True  # assume that input is tuple of inputs and states. If not, then set to False
     spiking = False
 
     with torch.no_grad():
         # TODO: should change this code block so that all inputs get cloned
         if isinstance(inputs, tuple):
-
             # input is first element, rest is hidden states
             test_ins = inputs[0]
 
             # NOTE: this only checks first input as everything else can be seen as hidden states in rnn block
             if len(test_ins[(test_ins != 0) & (test_ins != 1) & (test_ins != -1)]) == 0:
                 spiking = True
             if not all_ones:
@@ -167,67 +187,77 @@
             inputs[inputs != 0] = 1
             if all_ones:
                 inputs[inputs == 0] = 1
     return inputs, spiking, in_states
 
 
 def single_layer_MACs(inputs, layer, total=False):
-    """ Computes the MACs for a single layer.
-        returns effective operations if total=False, else total operations (including zero operations)
-        Supported layers: Linear, Conv1d, Conv2d, Conv3d, RNNCellBase, LSTMCell, GRUCell
+    """
+    Computes the MACs for a single layer.
+
+    returns effective operations if total=False, else total operations (including zero operations)
+    Supported layers: Linear, Conv1d, Conv2d, Conv3d, RNNCellBase, LSTMCell, GRUCell
+
     """
     macs = 0
 
     # copy input
     inputs, spiking, in_states = binary_inputs(inputs, all_ones=total)
 
-    stateless_layers = (torch.nn.Linear, torch.nn.Conv2d, torch.nn.Conv1d, torch.nn.Conv3d)
-    recurrent_layers = (torch.nn.RNNBase)
-    recurrent_cells = (torch.nn.RNNCellBase)
+    stateless_layers = (
+        torch.nn.Linear,
+        torch.nn.Conv2d,
+        torch.nn.Conv1d,
+        torch.nn.Conv3d,
+    )
+    recurrent_layers = torch.nn.RNNBase
+    recurrent_cells = torch.nn.RNNCellBase
 
     if isinstance(layer, stateless_layers):
         # then multiply the binary layer with the diagonal matrix to get the MACs
         layer_bin = make_binary_copy(layer, all_ones=total)
 
         # bias is not considered as a synaptic operation
         # in the future you can change this parameter to include bias
         bias = False
         if layer_bin.bias is not None and not bias:
             # suppress the bias to zero
             layer_bin.bias.data = torch.zeros_like(layer_bin.bias.data)
 
         nr_updates = layer_bin(
-            inputs)  # this returns the number of MACs for every output neuron: if spiking neurons only AC
+            inputs
+        )  # this returns the number of MACs for every output neuron: if spiking neurons only AC
         macs = nr_updates.sum()
 
-
     elif isinstance(layer, recurrent_layers):
         layer_bin = make_binary_copy(layer, all_ones=total)
         attribute_names = []
         for i in range(layer.num_layers):
-            param_names = ['weight_ih_l{}{}', 'weight_hh_l{}{}']
+            param_names = ["weight_ih_l{}{}", "weight_hh_l{}{}"]
             if layer.bias:
-                param_names += ['bias_ih_l{}{}', 'bias_hh_l{}{}']
+                param_names += ["bias_ih_l{}{}", "bias_hh_l{}{}"]
             if layer.proj_size > 0:  # it is lstm
-                param_names += ['weight_hr_l{}{}']
+                param_names += ["weight_hr_l{}{}"]
 
-            attribute_names += [x.format(i, '') for x in param_names]
+            attribute_names += [x.format(i, "") for x in param_names]
             if layer.bidirectional:
-                suffix = '_reverse'
+                suffix = "_reverse"
                 attribute_names += [x.format(i, suffix) for x in param_names]
-        raise 'This layer is not yet supported by NeuroBench.'
+        raise "This layer is not yet supported by NeuroBench."
         return 0
     elif isinstance(layer, recurrent_cells):
         # NOTE: sigmoid and tanh will never change a non-zero value to zero or vice versa
         # NOTE: these activation functions are currently NOT included in NeuroBench
         # if no explicit states are passed to recurrent layers, then h and c are initialized to zero (pytorch convention)
         layer_bin = make_binary_copy(layer, all_ones=total)
         # transpose from batches, timesteps, features to features, batches
         # print(layer_bin.weight_ih.shape)
-        out_ih = torch.matmul(layer_bin.weight_ih, inputs[0].transpose(0, -1))  # accounts for i,f,g,o
+        out_ih = torch.matmul(
+            layer_bin.weight_ih, inputs[0].transpose(0, -1)
+        )  # accounts for i,f,g,o
         out_hh = torch.zeros_like(out_ih)
 
         biases = 0
         bias_ih = 0
         bias_hh = 0
         # out matrices are now features, batches
         if layer_bin.bias:
@@ -243,15 +273,17 @@
             # o = sigmoid(Wio*x + bio + Who*h + bho)
 
             # c = f*c + i*g
             # h = o*tanh(c)
 
             # inputs = (x,(h,c))
             if in_states:
-                out_hh = torch.matmul(layer_bin.weight_hh, inputs[1][0].transpose(0, -1))
+                out_hh = torch.matmul(
+                    layer_bin.weight_hh, inputs[1][0].transpose(0, -1)
+                )
 
             # out_ih[out_ih!=0] = 1
             # out_hh[out_hh!=0] = 1
 
             out = out_ih + out_hh
 
             ifgo_macs = out.sum()  # accounts for i,f,g,o WITHOUT biases
@@ -296,22 +328,28 @@
             out_hh_n = out_hh.reshape(3, -1)[2, :] + bias_hh.reshape(3, -1)[2, :]
             r = rzn[0, :]  # get r
             z = rzn[1, :]
 
             r[r != 0] = 1
             out_hh_n[out_hh_n != 0] = 1
 
-            n_hh_term_macs = r * out_hh_n  # elementwise_multiplication to find macs ofr*(Whn*h + bhn) specifically
+            n_hh_term_macs = (
+                r * out_hh_n
+            )  # elementwise_multiplication to find macs ofr*(Whn*h + bhn) specifically
             n_hh_term_macs[n_hh_term_macs != 0] = 1
             macs += n_hh_term_macs.sum()
 
             # note hh part of n is already binarized, does not influence calculation of macs for n
-            n = out_hh.reshape(3, -1)[2, :] + bias_ih.reshape(3, -1)[2, :] + n_hh_term_macs
+            n = (
+                out_hh.reshape(3, -1)[2, :]
+                + bias_ih.reshape(3, -1)[2, :]
+                + n_hh_term_macs
+            )
             n[n != 0] = 1
-            z_a = (1 - z)
+            z_a = 1 - z
             # only do this now because affects z_a
             z[z != 0] = 1
             z_a[z_a != 0] = 1
             t_1 = z_a * n
             t_2 = z * inputs[1]
 
             t_1[t_1 != 0] = 1
```

### Comparing `neurobench-1.0.2/pyproject.toml` & `neurobench-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurobench"
-version = "1.0.2"
+version = "1.0.3"
 description = "Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing"
 authors = ["NeuroBench Team <neurobench@googlegroups.com>"]
 readme = "README.rst"
 exclude = ["docs", "tests", "neurobench/examples"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -28,15 +28,19 @@
 pytest-cov = "^4.1.0"
 jitcdde = "^1.8.1"
 pytorch-lightning = "^1.4.0"
 gdown = "^4.7.1"
 librosa = "^0.10.1"
 sphinx = "^7.2.5"
 sphinx-rtd-theme = "^1.3.0"
+pre-commit = "*"
 
 [tool.poetry.extras]
 mackey-glass = ["jitcdde"]
 nehar = ["pytorch-lightning", "gdown"]
 
+[tool.black]
+exclude = '/examples/'
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `neurobench-1.0.2/setup.py` & `neurobench-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 extras_require = \
 {'mackey-glass': ['jitcdde>=1.8.1,<2.0.0'],
  'nehar': ['pytorch-lightning>=1.4.0,<2.0.0', 'gdown>=4.7.1,<5.0.0']}
 
 setup_kwargs = {
     'name': 'neurobench',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing',
     'long_description': "============\nIntroduction\n============\n\nA harness for running evaluations on\n`NeuroBench <https://neurobench.ai>`__ algorithm benchmarks.\n\nNeuroBench is a community-driven project, and we welcome further\ndevelopment from the community. If you are interested in developing\nextensions to features, programming frameworks, or metrics and tasks,\nplease see the `Contributing Guidelines <https://neurobench.readthedocs.io/en/latest/contributing.html>`__.\n\nNeuroBench Structure\n---------------------\n\nNeuroBench contains the following sections:\n\n.. list-table:: \n   :widths: 20 60\n\n   * - **Section**\n     - **Description**\n   * - `neurobench.benchmarks <https://neurobench.readthedocs.io/en/latest/neurobench.benchmarks.html>`__\n     - Neurobench benchmarks, including data metrics and static metrics\n   * - `neurobench.datasets <https://neurobench.readthedocs.io/en/latest/neurobench.datasets.html>`__\n     - Neurobench benchmark datasets\n   * - `neurobench.models <https://neurobench.readthedocs.io/en/latest/neurobench.models.html>`__\n     - Neurobench framework for Torch and SNNTorch models\n   * - `neurobench.preprocessing <https://neurobench.readthedocs.io/en/latest/neurobench.preprocessing.html>`__\n     - Pre-processing of data, conversion to spikes\n   * - `neurobench.postprocessing <https://neurobench.readthedocs.io/en/latest/neurobench.postprocessing.html>`__\n     - Post-processors take the spiking output from the models and provide several methods of combining them\n\nInstallation\n------------\n\nInstall from PyPI:\n\n::\n\n   pip install neurobench\n\nBenchmarks\n----------\n\nThe following benchmarks are currently available:\n\nv1.0 benchmarks\n~~~~~~~~~~~~~~~\n- Keyword Few-shot Class-incremental Learning (FSCIL)\n- Event Camera Object Detection\n- Non-human Primate (NHP) Motor Prediction\n- Chaotic Function Prediction\n\nAdditional benchmarks\n~~~~~~~~~~~~~~~~~~~~~\n- DVS Gesture Recognition\n- Google Speech Commands (GSC) Classification\n- Neuromorphic Human Activity Recognition (HAR)\n\nGetting started\n---------------\n\nExample benchmark scripts can be found under the ``neurobench/examples`` folder. \n(`https://github.com/NeuroBench/neurobench/tree/main/neurobench/examples/ <https://github.com/NeuroBench/neurobench/tree/main/neurobench/examples/>`__)\n\nIn general, the design flow for using the framework is as follows:\n\n1. Train a network using the train split from a particular dataset.\n2. Wrap the network in a ``NeuroBenchModel``.\n3. Pass the model, evaluation split dataloader, pre-/post-processors,\n   and a list of metrics to the ``Benchmark`` and ``run()``.\n\nDocumentation for the framework interfaces can found in the `API Overview <https://neurobench.readthedocs.io/en/latest/api.html>`__.\n\nDevelopment\n-----------\n\nIf you clone the repo directly for development, `poetry <https://pypi.org/project/poetry/>`__ \ncan be used to maintain a virtualenv consistent with a deployment environment. In the\nroot directory run:\n\n::\n\n   pip install poetry\n   poetry install\n\nPoetry requires python >=3.9. Installation should not take more than a few minutes.\n\nEnd-to-end examples can be run from the poetry environment. As a demo, try the \nGoogle Speech Commands keyword classification benchmark:\n\n::\n\n   # ANN Benchmark Example\n   poetry run python neurobench/examples/gsc/benchmark_ann.py\n   \n   # Expected results:\n   # {'footprint': 109228, 'connection_sparsity': 0.0,\n   # 'classification_accuracy': 0.8653339397251905, 'activation_sparsity': 0.3854464619019532, \n   # 'synaptic_operations': {'Effective_MACs': 1749994.1556565198, 'Effective_ACs': 0.0, 'Dense': 1902179.0}}\n\n\n   # SNN Benchmark Example\n   poetry run python neurobench/examples/gsc/benchmark_snn.py\n   \n   # Expected results:\n   # {'footprint': 583900, 'connection_sparsity': 0.0,\n   # 'classification_accuracy': 0.8484325295196562, 'activation_sparsity': 0.9675956131759854, \n   # 'synaptic_operations': {'Effective_MACs': 0.0, 'Effective_ACs': 3556689.9895502045, 'Dense': 29336955.0}}\n\nThese demos should download the dataset, then run in a couple minutes. Other baseline result scripts and notebook\ntutorials are available in the ``neurobench/examples`` folder.\n\nDevelopers\n----------\n\nNeuroBench is a collaboration between industry and academic engineers\nand researchers. This framework is currently maintained by `Jason\nYik <https://www.linkedin.com/in/jasonlyik/>`__, `Noah\nPacik-Nelson <https://www.linkedin.com/in/noah-pacik-nelson/>`__, and\n`Korneel Van den\nBerghe <https://www.linkedin.com/in/korneel-van-den-berghe/>`__, and\nthere have been technical contributions from many others. A\nnon-exhaustive list includes Gregor Lenz, Denis Kleyko, Younes\nBouhadjar, Paul Hueber, Vincent Sun, Biyan Zhou, George Vathakkattil\nJoseph, Douwe den Blanken, Maxime Fabre, Shenqi Wang, Guangzhi Tang,\nAnurag Kumar Mishra, Soikat Hasan Ahmed, Benedetto Leto, Aurora Micheli,\nTao Sun.\n\nContributing\n------------\n\nIf you are interested in helping to build this framework, please see the\n`Contribution Guidelines <https://neurobench.readthedocs.io/en/latest/contributing.html>`__.\n\nCitation\n--------\n\nIf you use this framework in your research, please cite the following\npreprint article:\n\n::\n\n   @misc{yik2024neurobench,\n      title={NeuroBench: A Framework for Benchmarking Neuromorphic Computing Algorithms and Systems}, \n      author={Jason Yik and Korneel Van den Berghe and Douwe den Blanken and Younes Bouhadjar and Maxime Fabre and Paul Hueber and Denis Kleyko and Noah Pacik-Nelson and Pao-Sheng Vincent Sun and Guangzhi Tang and Shenqi Wang and Biyan Zhou and Soikat Hasan Ahmed and George Vathakkattil Joseph and Benedetto Leto and Aurora Micheli and Anurag Kumar Mishra and Gregor Lenz and Tao Sun and Zergham Ahmed and Mahmoud Akl and Brian Anderson and Andreas G. Andreou and Chiara Bartolozzi and Arindam Basu and Petrut Bogdan and Sander Bohte and Sonia Buckley and Gert Cauwenberghs and Elisabetta Chicca and Federico Corradi and Guido de Croon and Andreea Danielescu and Anurag Daram and Mike Davies and Yigit Demirag and Jason Eshraghian and Tobias Fischer and Jeremy Forest and Vittorio Fra and Steve Furber and P. Michael Furlong and William Gilpin and Aditya Gilra and Hector A. Gonzalez and Giacomo Indiveri and Siddharth Joshi and Vedant Karia and Lyes Khacef and James C. Knight and Laura Kriener and Rajkumar Kubendran and Dhireesha Kudithipudi and Yao-Hong Liu and Shih-Chii Liu and Haoyuan Ma and Rajit Manohar and Josep Maria Margarit-Taulé and Christian Mayr and Konstantinos Michmizos and Dylan Muir and Emre Neftci and Thomas Nowotny and Fabrizio Ottati and Ayca Ozcelikkale and Priyadarshini Panda and Jongkil Park and Melika Payvand and Christian Pehle and Mihai A. Petrovici and Alessandro Pierro and Christoph Posch and Alpha Renner and Yulia Sandamirskaya and Clemens JS Schaefer and André van Schaik and Johannes Schemmel and Samuel Schmidgall and Catherine Schuman and Jae-sun Seo and Sadique Sheik and Sumit Bam Shrestha and Manolis Sifalakis and Amos Sironi and Matthew Stewart and Kenneth Stewart and Terrence C. Stewart and Philipp Stratmann and Jonathan Timcheck and Nergis Tömen and Gianvito Urgese and Marian Verhelst and Craig M. Vineyard and Bernhard Vogginger and Amirreza Yousefzadeh and Fatima Tuz Zohora and Charlotte Frenkel and Vijay Janapa Reddi},\n      year={2024},\n      eprint={2304.04640},\n      archivePrefix={arXiv},\n      primaryClass={cs.AI}\n   }\n",
     'author': 'NeuroBench Team',
     'author_email': 'neurobench@googlegroups.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `neurobench-1.0.2/PKG-INFO` & `neurobench-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurobench
-Version: 1.0.2
+Version: 1.0.3
 Summary: Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing
 Author: NeuroBench Team
 Author-email: neurobench@googlegroups.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

