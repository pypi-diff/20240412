# Comparing `tmp/pystorm3-0.1.2.tar.gz` & `tmp/pystorm3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.2.tar", last modified: Thu Apr 11 12:33:35 2024, max compression
+gzip compressed data, was "pystorm3-0.1.3.tar", last modified: Thu Apr 11 14:29:33 2024, max compression
```

## Comparing `pystorm3-0.1.2.tar` & `pystorm3-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.048623 pystorm3-0.1.2/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.2/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:33:35.047623 pystorm3-0.1.2/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.2/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.2/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/signal_processing/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.2/pystorm/signal_processing/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     4742 2024-04-11 12:21:03.000000 pystorm3-0.1.2/pystorm/signal_processing/band_filter.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.2/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2647 2024-04-11 12:22:38.000000 pystorm3-0.1.2/pystorm/timefreq/hilbert.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2377 2024-04-10 16:09:04.000000 pystorm3-0.1.2/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       51 2024-04-10 16:00:40.000000 pystorm3-0.1.2/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    29490 2024-04-11 12:24:01.000000 pystorm3-0.1.2/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)      716 2024-04-11 12:18:49.000000 pystorm3-0.1.2/pystorm/utils/type_safety.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 12:33:30.000000 pystorm3-0.1.2/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      472 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 12:33:35.048623 pystorm3-0.1.2/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.2/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.3/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 14:29:33.425090 pystorm3-0.1.3/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.3/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.424090 pystorm3-0.1.3/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.3/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.424090 pystorm3-0.1.3/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.3/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4740 2024-04-11 14:15:21.000000 pystorm3-0.1.3/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.3/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2645 2024-04-11 14:15:13.000000 pystorm3-0.1.3/pystorm/timefreq/hilbert.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2560 2024-04-11 14:26:22.000000 pystorm3-0.1.3/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       24 2024-04-11 14:15:31.000000 pystorm3-0.1.3/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    30302 2024-04-11 14:27:51.000000 pystorm3-0.1.3/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 14:15:58.000000 pystorm3-0.1.3/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 14:29:33.425090 pystorm3-0.1.3/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      443 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 14:29:33.000000 pystorm3-0.1.3/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 14:29:33.425090 pystorm3-0.1.3/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.3/setup.py
```

### Comparing `pystorm3-0.1.2/LICENSE` & `pystorm3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.2/PKG-INFO` & `pystorm3-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.2/README.md` & `pystorm3-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.2/pystorm/signal_processing/band_filter.py` & `pystorm3-0.1.3/pystorm/signal_processing/band_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pystorm.utils.type_safety import ensure_numpy, ensure_torch
+from pystorm.utils.minitorch import ensure_numpy, ensure_torch
 from scipy.signal import firwin
 from math import ceil 
 from pystorm import minitorch as mnt
 
 def get_firwin(ntaps, centered_band, beta, fs):
     return firwin(ntaps, centered_band, window=("kaiser", beta), scale = True, pass_zero=False,fs=fs)
```

### Comparing `pystorm3-0.1.2/pystorm/timefreq/hilbert.py` & `pystorm3-0.1.3/pystorm/timefreq/hilbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pystorm.utils.type_safety import ensure_numpy, ensure_torch
+from pystorm.utils.minitorch import ensure_numpy, ensure_torch
 from pystorm.signal_processing import band_pass
 from pystorm import minitorch as mnt
 
 def get_hilbert_torch(signal, fs, pad_size = None, window_mask = None, device = "cpu"):
     signal = ensure_torch(signal).to(device)
     
     if window_mask is not None: # Foreshadowing Amplitude Envelope Correlation implementation
```

### Comparing `pystorm3-0.1.2/pystorm/timefreq/welch_psd.py` & `pystorm3-0.1.3/pystorm/timefreq/welch_psd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from pystorm.utils import minitorch as mnt
-from pystorm.utils.type_safety import ensure_torch, ensure_numpy
+from pystorm.utils.minitorch import ensure_numpy
 
 def welch_psd_source_space(time_series, fs, ker = None,window_length=2000, overlap = 0.5, device = "cpu"):
     if ker is None:
         return welch_psd_sensor_space(time_series, fs, window_length=window_length, overlap = overlap, device = device)
     nTime = time_series.shape[-1]
     Lwin = round(window_length/1000*fs)
     Loverlap = round(Lwin * overlap)
     Lwin = Lwin - Lwin%2
     Nwin = int((nTime - Loverlap)/(Lwin-Loverlap))
 
     freqs = mnt.rfftfreq(Lwin,1/fs).to(device)
-    ker_cuda = ensure_torch(ker).to(device).type(mnt.complex64)
-    sensor_cuda = ensure_torch(time_series).to(device)
+    if time_series.dtype == mnt.float32:
+        mnt.set_minitorch_default_dtype("float32")
+        print(mnt.__default_complex_dtype__)
+    ker_cuda = mnt.ensure_torch(ker, type_float=True).to(device).type(mnt.__default_complex_dtype__)
+    sensor_cuda = mnt.ensure_torch(time_series, type_float=True).to(device)
     hamming_window = (0.54 - 0.46 * mnt.cos(mnt.linspace(0,2*mnt.pi,Lwin))).to(device)
 
     win_noise_power_gain = (hamming_window**2).sum()
     scaling_term = (2/(win_noise_power_gain*fs)).sqrt()
     time_sequence = mnt.arange(0,Lwin, dtype = int)
 
     fft_blocks = 0
@@ -33,15 +36,15 @@
     nTime = time_series.shape[-1]
     Lwin = round(window_length/1000*fs)
     Loverlap = round(Lwin * overlap)
     Lwin = Lwin - Lwin%2
     Nwin = int((nTime - Loverlap)/(Lwin-Loverlap))
 
     freqs = mnt.rfftfreq(Lwin,1/fs).to(device)
-    sensor_cuda = ensure_torch(time_series).to(device)
+    sensor_cuda = mnt.ensure_torch(time_series).to(device)
     hamming_window = (0.54 - 0.46 * mnt.cos(mnt.linspace(0,2*mnt.pi,Lwin))).to(device)
 
     win_noise_power_gain = (hamming_window**2).sum()
     scaling_term = (2/(win_noise_power_gain*fs)).sqrt()
     time_sequence = mnt.arange(0,Lwin, dtype = int)
 
     fft_blocks = 0
```

### Comparing `pystorm3-0.1.2/pystorm/utils/minitorch.py` & `pystorm3-0.1.3/pystorm/utils/minitorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,69 @@
 from torchaudio.functional import convolve as tconvolve
 from torchaudio.functional import fftconvolve as tfftconvolve
 from torch import float16,float32,float64
 from torch import set_default_dtype
 pi = tpi
 
 __default_dtype__ = float64
+__default_complex_dtype__ = complex128
 set_default_dtype(__default_dtype__)
 def set_minitorch_default_dtype(default_type = "float64"):
-    global __default_dtype__
+    global __default_dtype__, __default_complex_dtype__
     if default_type == "float16":
         __default_dtype__ = float16
         print("Warning: Pytorch only supports FFT of signals whose length are powers of 2 in this float type")
     elif default_type == "float32":
         __default_dtype__ = float32
+        __default_complex_dtype__ = complex64
     else:
         __default_dtype__ = float64
+        __default_complex_dtype__ = complex128
     set_default_dtype(__default_dtype__)
     
 
+def ensure_torch(x, type_float = False):
+    try:
+        x = as_tensor(x)
+        if type_float:
+            x = x.type(__default_dtype__)
+    except:
+        try:
+            x = from_numpy(x)
+            if type_float:
+                x = x.type(__default_dtype__)
+        except:
+            pass
+    
+    if type_float:
+        try:
+            x = x.type(__default_dtype__)
+        except:
+            pass
+    return x
+
+def ensure_numpy(x):
+    
+    try:
+        x = x.detach()
+    except:
+        pass
+    
+    try:
+        x = x.to('cpu')
+    except:
+        pass
+    
+    try:
+        x = x.numpy()
+    except:
+        pass
+    
+    return x
+
 def eye(*args, **kwargs):
     """
     eye(n, m=None, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a 2-D tensor with ones on the diagonal and zeros elsewhere.
 
     Args:
```

### Comparing `pystorm3-0.1.2/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.3/pystorm3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
```

### Comparing `pystorm3-0.1.2/setup.py` & `pystorm3-0.1.3/setup.py`

 * *Files identical despite different names*

