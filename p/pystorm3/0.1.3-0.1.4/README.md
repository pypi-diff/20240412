# Comparing `tmp/pystorm3-0.1.3.tar.gz` & `tmp/pystorm3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.3.tar", last modified: Thu Apr 11 14:29:33 2024, max compression
+gzip compressed data, was "pystorm3-0.1.4.tar", last modified: Fri Apr 12 12:56:45 2024, max compression
```

## Comparing `pystorm3-0.1.3.tar` & `pystorm3-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.3/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 14:29:33.425090 pystorm3-0.1.3/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.3/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.424090 pystorm3-0.1.3/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.3/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.424090 pystorm3-0.1.3/pystorm/signal_processing/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.3/pystorm/signal_processing/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     4740 2024-04-11 14:15:21.000000 pystorm3-0.1.3/pystorm/signal_processing/band_filter.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.3/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2645 2024-04-11 14:15:13.000000 pystorm3-0.1.3/pystorm/timefreq/hilbert.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2560 2024-04-11 14:26:22.000000 pystorm3-0.1.3/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       24 2024-04-11 14:15:31.000000 pystorm3-0.1.3/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    30302 2024-04-11 14:27:51.000000 pystorm3-0.1.3/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 14:15:58.000000 pystorm3-0.1.3/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      443 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 14:29:33.425090 pystorm3-0.1.3/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.3/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.403517 pystorm3-0.1.4/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.4/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-12 12:56:45.403517 pystorm3-0.1.4/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.4/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.402517 pystorm3-0.1.4/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1074 2024-04-12 11:34:02.000000 pystorm3-0.1.4/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.402517 pystorm3-0.1.4/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      652 2024-04-12 12:13:01.000000 pystorm3-0.1.4/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     9436 2024-04-12 12:55:55.000000 pystorm3-0.1.4/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.402517 pystorm3-0.1.4/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      761 2024-04-12 11:20:10.000000 pystorm3-0.1.4/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     6902 2024-04-12 12:55:13.000000 pystorm3-0.1.4/pystorm/timefreq/analytical_signal.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4414 2024-04-12 12:54:52.000000 pystorm3-0.1.4/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.402517 pystorm3-0.1.4/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      409 2024-04-12 11:26:22.000000 pystorm3-0.1.4/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    34849 2024-04-12 12:22:18.000000 pystorm3-0.1.4/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-12 10:10:30.000000 pystorm3-0.1.4/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-12 12:56:45.403517 pystorm3-0.1.4/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-12 12:56:45.000000 pystorm3-0.1.4/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      453 2024-04-12 12:56:45.000000 pystorm3-0.1.4/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-12 12:56:45.000000 pystorm3-0.1.4/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-12 12:56:45.000000 pystorm3-0.1.4/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-12 12:56:45.000000 pystorm3-0.1.4/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-12 12:56:45.403517 pystorm3-0.1.4/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.4/setup.py
```

### Comparing `pystorm3-0.1.3/LICENSE` & `pystorm3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.3/PKG-INFO` & `pystorm3-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.3/README.md` & `pystorm3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.3/pystorm/utils/minitorch.py` & `pystorm3-0.1.4/pystorm/utils/minitorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,204 @@
 """
-A module that serves as lightweight pytorch.
+A module that serves as a lightweight pytorch++ (also has some numpy<->pytorch conversion utils, and some torchaudio functions).
 
-The intent is to possibly minimize RAM usage from functions that would be executed by multiple processes in parallel on the GPU.
+It is intended to be a quality-of-life module that groups most pytorch-related functions that are used repeatedly within the package and to possibly minimize GPU RAM usage from imports when executing jobs with multiple processes running on the GPU in parallel.
+
+The functions are 'copied' and not just imported to have their original docstrings available.
 """
 
-from torch.fft import rfft as trfft
-from torch.fft import rfftfreq as trfftfreq 
-from torch.fft import fft as tfft
-from torch.fft import ifft as tifft
-from torch.fft import fftfreq as tfftfreq 
-from torch import cat as tcat
-from torch import linspace as tlinspace
-from torch import pi as tpi
-from torch import arange as tarange
-from torch import zeros as tzeros
-from torch import zeros_like as  tzeros_like
-from torch import ones_like as  tones_like
-from torch import ones as tones
-from torch import as_tensor as tas_tensor
-from torch import from_numpy as tfrom_numpy
+from torch.fft import rfft as _rfft
+from torch.fft import rfftfreq as _rfftfreq 
+from torch.fft import fft as _fft
+from torch.fft import ifft as _ifft
+from torch.fft import fftfreq as _fftfreq 
+from torch import cat as _cat
+from torch import linspace as _linspace
+from torch import pi as _pi
+from torch import arange as _arange
+from torch import zeros as _zeros
+from torch import zeros_like as  _zeros_like
+from torch import ones_like as  _ones_like
+from torch import ones as _ones
+from torch import as_tensor as _as_tensor
+from torch import from_numpy as _from_numpy
 from torch import complex64, complex128
-from torch import cos as tcos
-from torch import eye as teye
-from torch import argwhere as targwhere
-from torchaudio.functional import convolve as tconvolve
-from torchaudio.functional import fftconvolve as tfftconvolve
+from torch import cos as _cos
+from torch import eye as _eye
+from torch import argwhere as _argwhere
+from torchaudio.functional import convolve as _convolve
+from torchaudio.functional import fftconvolve as _fftconvolve
 from torch import float16,float32,float64
 from torch import set_default_dtype
-pi = tpi
-
+from numpy import ndarray as _ndarray
+from torch import Tensor as _Tensor
+pi = _pi
+__all__=[
+        "rfft","rfftfreq","fft","ifft","fftfreq","convolve","fftconvolve",
+        "linspace","arange","argwhere",
+        "cat","zeros","ones","zeros_like","ones_like","eye",
+        "as_tensor","from_numpy","ensure_numpy","ensure_torch",
+        "cos","pi",
+        "float16","float32","float64","complex64","complex128",
+        "set_minitorch_default_dtype","__default_dtype__","__default_complex_dtype__"
+]
 __default_dtype__ = float64
 __default_complex_dtype__ = complex128
 set_default_dtype(__default_dtype__)
-def set_minitorch_default_dtype(default_type = "float64"):
+def set_minitorch_default_dtype(default_type: str = "float64"):
+    """ This function allows for specifying a floating point precision (and its matching complex precision). Default is float64 and complex128.
+
+        Args: 
+            None
+        Keyword Args: 
+            default_type: str     
+                String that specifies the default floating point type of the pytorch backend
+        Returns: 
+            None
+
+    """
+
     global __default_dtype__, __default_complex_dtype__
     if default_type == "float16":
         __default_dtype__ = float16
         print("Warning: Pytorch only supports FFT of signals whose length are powers of 2 in this float type")
     elif default_type == "float32":
         __default_dtype__ = float32
         __default_complex_dtype__ = complex64
     else:
         __default_dtype__ = float64
         __default_complex_dtype__ = complex128
     set_default_dtype(__default_dtype__)
     
 
-def ensure_torch(x, type_float = False):
+def ensure_torch(x, type_float: bool = False, type_complex: bool = False):
+    """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype').
+    
+        Args: 
+            x: list/numpy array/torch tensor/primitive type that can be contained in a torch tensor (e.g., float, int, bool)
+                Input variable.
+        Keyword Args: 
+            type_float: bool          
+                Specifies whether to set the type of the tensor.
+            type_complex: bool        
+                Specifies if the type of the tensor is meant to be complex
+        Returns:
+            x: Torch tensor
+                The input ensured to be a torch tensor.
+
+    """
+    dtype_setting = __default_dtype__
+    if type_complex:
+        dtype_setting = __default_complex_dtype__
+    if isinstance(x, _Tensor):
+        if not type_float:
+            return x
+        try:
+            x = x.type(dtype_setting)
+            return x
+        except:
+            pass
     try:
-        x = as_tensor(x)
+        x = _as_tensor(x)
         if type_float:
-            x = x.type(__default_dtype__)
+            x = x.type(dtype_setting)
+        return x
     except:
         try:
-            x = from_numpy(x)
+            x = _from_numpy(x)
             if type_float:
-                x = x.type(__default_dtype__)
+                x = x.type(dtype_setting)
+            return x
         except:
             pass
+    return x
+
+
+def _ensure_torch(x, type_float: bool = False, type_complex: bool = False):
+    """ This function ensures that the variable is a torch tensor. It optionally also ensures that it is of the default type (as set by 'set_minitorch_default_dtype'). Differs from 'ensure_torch' by returning False if it could not cast it as a tensor instead of returning the input.
     
-    if type_float:
+        Args: 
+            x: list/numpy array/torch tensor/primitive type that can be contained in a torch tensor (e.g., float, int, bool)
+                Input variable.
+        Keyword Args: 
+            type_float: bool          
+                Specifies whether to set the type of the tensor.
+            type_complex: bool        
+                Specifies if the type of the tensor is meant to be complex
+        Returns:
+            casting_success: bool
+                Boolean that specifies if casting succeeded or not. 
+            x: Torch tensor
+                The input ensured to be a torch tensor.
+
+    """
+    dtype_setting = __default_dtype__
+    if type_complex:
+        dtype_setting = __default_complex_dtype__
+    if isinstance(x, _Tensor):
+        if not type_float:
+            return True, x
         try:
-            x = x.type(__default_dtype__)
+            x = x.type(dtype_setting)
+            return True, x
         except:
             pass
-    return x
+    try:
+        x = _as_tensor(x)
+        if type_float:
+            x = x.type(dtype_setting)
+        return True, x
+    except:
+        try:
+            x = _from_numpy(x)
+            if type_float:
+                x = x.type(dtype_setting)
+            return True, x
+        except:
+            pass
+    return False, x
 
 def ensure_numpy(x):
+    """ This function ensures that the variable is a numpy array. 
     
+        Args: 
+            x: list/numpy array/torch tensor/primitive type that can be contained in a numpy array (e.g., float, int, bool)
+                Input variable.
+        Keyword Args: 
+            None
+        Returns: 
+            x: numpy array (or original variable if casting failed)                 
+                The input ensured to be a numpy array.
+
+    """ 
+    if isinstance(x, _ndarray):
+        return x
     try:
         x = x.detach()
     except:
         pass
     
     try:
-        x = x.to('cpu')
+        x = x.cpu()
     except:
         pass
     
     try:
         x = x.numpy()
     except:
-        pass
-    
+        # Handle the case where it's a list
+        try:
+            is_torch_now, x = _ensure_torch(x)
+            if is_torch_now: # Avoids infinite loop if for some reason casting fails
+                x = ensure_numpy(x)
+                return x
+            else:
+                return x
+        except:
+            pass
     return x
 
 def eye(*args, **kwargs):
     """
     eye(n, m=None, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a 2-D tensor with ones on the diagonal and zeros elsewhere.
@@ -107,15 +219,15 @@
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
 
     Returns:
         Tensor: A 2-D tensor with ones on the diagonal and zeros elsewhere
         """
-    return teye(*args,**kwargs)
+    return _eye(*args,**kwargs)
 
 def zeros(*args, **kwargs):
     """
     zeros(*size, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a tensor filled with the scalar value `0`, with the shape defined
     by the variable argument :attr:`size`.
@@ -133,15 +245,15 @@
         device (:class:`torch.device`, optional): the desired device of returned tensor.
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_tensor_type`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
             """
-    return tzeros(*args,**kwargs)
+    return _zeros(*args,**kwargs)
 
 def ones(*args, **kwargs):
     """
     ones(*size, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a tensor filled with the scalar value `1`, with the shape defined
     by the variable argument :attr:`size`.
@@ -159,15 +271,15 @@
         device (:class:`torch.device`, optional): the desired device of returned tensor.
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_tensor_type`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
         """
-    return tones(*args,**kwargs)
+    return _ones(*args,**kwargs)
 
 def cat(*args, **kwargs):
     """
     cat(tensors, dim=0, *, out=None) -> Tensor
 
     Concatenates the given sequence of :attr:`seq` tensors in the given dimension.
     All tensors must either have the same shape (except in the concatenating
@@ -187,15 +299,15 @@
             Non-empty tensors provided must have the same shape, except in the
             cat dimension.
         dim (int, optional): the dimension over which the tensors are concatenated
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return tcat(*args,**kwargs)
+    return _cat(*args,**kwargs)
 
 def arange(*args, **kwargs):
     """
     arange(start=0, end, step=1, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a 1-D tensor of size :math:`\left\lceil \frac{\text{end} - \text{start}}{\text{step}} \right\rceil`
     with values from the interval ``[start, end)`` taken with common difference
@@ -227,15 +339,15 @@
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_tensor_type`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
 
     """
-    return tarange(*args,**kwargs)
+    return _arange(*args,**kwargs)
 
 def linspace(*args, **kwargs):
     """
     linspace(start, end, steps, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Creates a one-dimensional tensor of size :attr:`steps` whose values are evenly
     spaced from :attr:`start` to :attr:`end`, inclusive. That is, the value are:
@@ -266,15 +378,15 @@
         device (:class:`torch.device`, optional): the desired device of returned tensor.
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_tensor_type`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
     """
-    return tlinspace(*args,**kwargs)
+    return _linspace(*args,**kwargs)
 
 def ones_like(*args, **kwargs):
     """
     ones_like(input, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format) -> Tensor
 
     Returns a tensor filled with the scalar value `1`, with the same size as
     :attr:`input`. ``torch.ones_like(input)`` is equivalent to
@@ -297,15 +409,15 @@
             Default: if ``None``, defaults to the device of :attr:`input`.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
         memory_format (:class:`torch.memory_format`, optional): the desired memory format of
             returned Tensor. Default: ``torch.preserve_format``.
 
     """
-    return tones_like(*args,**kwargs)
+    return _ones_like(*args,**kwargs)
 
 def zeros_like(*args, **kwargs):
     """
     zeros_like(input, *, dtype=None, layout=None, device=None, requires_grad=False, memory_format=torch.preserve_format) -> Tensor
 
     Returns a tensor filled with the scalar value `0`, with the same size as
     :attr:`input`. ``torch.zeros_like(input)`` is equivalent to
@@ -328,15 +440,15 @@
             Default: if ``None``, defaults to the device of :attr:`input`.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
         memory_format (:class:`torch.memory_format`, optional): the desired memory format of
             returned Tensor. Default: ``torch.preserve_format``.
 
     """
-    return tzeros_like(*args,**kwargs)
+    return _zeros_like(*args,**kwargs)
 
 def as_tensor(*args,**kwargs):
     """
     as_tensor(data, dtype=None, device=None) -> Tensor
 
     Converts :attr:`data` into a tensor, sharing data and preserving autograd
     history if possible.
@@ -360,15 +472,15 @@
         dtype (:class:`torch.dtype`, optional): the desired data type of returned tensor.
             Default: if ``None``, infers data type from :attr:`data`.
         device (:class:`torch.device`, optional): the device of the constructed tensor. If None and data is a tensor
             then the device of data is used. If None and data is not a tensor then
             the result tensor is constructed on the current device.
 
     """
-    return tas_tensor(*args,**kwargs)
+    return _as_tensor(*args,**kwargs)
 
 
 def from_numpy(*args,**kwargs):
     """
         
     from_numpy(ndarray) -> Tensor
 
@@ -383,15 +495,15 @@
     ``numpy.int64``, ``numpy.int32``, ``numpy.int16``, ``numpy.int8``, ``numpy.uint8``,
     and ``bool``.
 
     .. warning::
         Writing to a tensor created from a read-only NumPy array is not supported and will result in undefined behavior.
 
     """
-    return tfrom_numpy(*args,**kwargs)
+    return _from_numpy(*args,**kwargs)
 
 def rfft(*args,**kwargs):
     """
     rfft(input, n=None, dim=-1, norm=None, *, out=None) -> Tensor
 
     Computes the one dimensional Fourier transform of real-valued :attr:`input`.
 
@@ -421,15 +533,15 @@
             the exact inverse.
 
             Default is ``"backward"`` (no normalization).
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return trfft(*args,**kwargs)
+    return _rfft(*args,**kwargs)
     
 def rfftfreq(*args,**kwargs):
     """
     rfftfreq(n, d=1.0, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Computes the sample frequencies for :func:`~torch.fft.rfft` with a signal of size :attr:`n`.
 
@@ -461,15 +573,15 @@
         device (:class:`torch.device`, optional): the desired device of returned tensor.
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_tensor_type`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
     """
-    return trfftfreq(*args,**kwargs)
+    return _rfftfreq(*args,**kwargs)
 
 def cos(*args,**kwargs):
     """
         
     cos(input, *, out=None) -> Tensor
 
     Returns a new tensor with the cosine  of the elements of :attr:`input`.
@@ -479,15 +591,15 @@
 
     Args:
         input (Tensor): the input tensor.
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return tcos(*args,**kwargs)
+    return _cos(*args,**kwargs)
 
 
 def fft(*args,**kwargs):
     """  
     fft(input, n=None, dim=-1, norm=None, *, out=None) -> Tensor
 
     Computes the one dimensional discrete Fourier transform of :attr:`input`.
@@ -522,15 +634,15 @@
             the exact inverse.
 
             Default is ``"backward"`` (no normalization).
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return tfft(*args,**kwargs)
+    return _fft(*args,**kwargs)
 
 def ifft(*args,**kwargs):
     """
     ifft(input, n=None, dim=-1, norm=None, *, out=None) -> Tensor
 
     Computes the one dimensional inverse discrete Fourier transform of :attr:`input`.
 
@@ -556,15 +668,15 @@
             the exact inverse.
 
             Default is ``"backward"`` (normalize by ``1/n``).
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return tifft(*args,**kwargs)
+    return _ifft(*args,**kwargs)
 
 def fftfreq(*args,**kwargs):
     """
     fftfreq(n, d=1.0, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Computes the discrete Fourier Transform sample frequencies for a signal of size :attr:`n`.
 
@@ -599,15 +711,15 @@
             Default: if ``None``, uses the current device for the default tensor type
             (see :func:`torch.set_default_device`). :attr:`device` will be the CPU
             for CPU tensor types and the current CUDA device for CUDA tensor types.
         requires_grad (bool, optional): If autograd should record operations on the
             returned tensor. Default: ``False``.
 
     """
-    return tfftfreq(*args,**kwargs)
+    return _fftfreq(*args,**kwargs)
 
 
 def convolve(*args, **kwargs):
     r"""
     Convolves inputs along their last dimension using the direct method.
     Note that, in contrast to :meth:`torch.nn.functional.conv1d`, which actually applies the valid cross-correlation
     operator, this function applies the true `convolution`_ operator.
@@ -630,15 +742,15 @@
     Returns:
         torch.Tensor: Result of convolving ``x`` and ``y``, with shape `(..., L)`, where
         the leading dimensions match those of ``x`` and `L` is dictated by ``mode``.
 
     .. _convolution:
         https://en.wikipedia.org/wiki/Convolution
     """
-    return tconvolve(*args,**kwargs)
+    return _convolve(*args,**kwargs)
 
     
 def fftconvolve(*args, **kwargs):
     r"""
     Convolves inputs along their last dimension using FFT. For inputs with large last dimensions, this function
     is generally much faster than :meth:`convolve`.
     Note that, in contrast to :meth:`torch.nn.functional.conv1d`, which actually applies the valid cross-correlation
@@ -663,15 +775,15 @@
     Returns:
         torch.Tensor: Result of convolving ``x`` and ``y``, with shape `(..., L)`, where
         the leading dimensions match those of ``x`` and `L` is dictated by ``mode``.
 
     .. _convolution:
         https://en.wikipedia.org/wiki/Convolution
     """
-    return tfftconvolve(*args,**kwargs)
+    return _fftconvolve(*args,**kwargs)
 
 
 def argwhere(*args, **kwargs):
     """
     argwhere(input) -> Tensor
 
     Returns a tensor containing the indices of all non-zero elements of
@@ -688,8 +800,8 @@
 
         When :attr:`input` is on CUDA, this function causes host-device synchronization.
 
     Args:
         {input}
 
     """
-    return targwhere(*args,**kwargs)
+    return _argwhere(*args,**kwargs)
```

### Comparing `pystorm3-0.1.3/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.4/pystorm3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.3/setup.py` & `pystorm3-0.1.4/setup.py`

 * *Files identical despite different names*

