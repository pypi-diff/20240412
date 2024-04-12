# Comparing `tmp/spectrum_fundamentals-0.5.0.tar.gz` & `tmp/spectrum_fundamentals-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.5.0.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.5.1.tar", max compression
```

## Comparing `spectrum_fundamentals-0.5.0.tar` & `spectrum_fundamentals-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1102 2023-12-18 17:27:05.800800 spectrum_fundamentals-0.5.0/LICENSE
--rw-r--r--   0        0        0     2611 2023-12-18 17:27:05.800800 spectrum_fundamentals-0.5.0/README.rst
--rw-r--r--   0        0        0     2464 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      938 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    11644 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1372 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     8544 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    13817 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14554 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    21687 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    22262 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0    13671 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2023-12-18 17:27:05.804801 spectrum_fundamentals-0.5.0/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 14:21:10.165602 spectrum_fundamentals-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2611 2024-04-12 14:21:10.165602 spectrum_fundamentals-0.5.1/README.rst
+-rw-r--r--   0        0        0     2464 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11644 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1377 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     8748 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    13817 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14495 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    21687 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22262 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0    15698 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.1/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.5.0/LICENSE` & `spectrum_fundamentals-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/README.rst` & `spectrum_fundamentals-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/pyproject.toml` & `spectrum_fundamentals-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.5.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamental functions, annotation pipeline and constants for oktoberfest"
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Initialize fundamentals."""
+
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/charge.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     elif isinstance(labels, (list, np.ndarray)):
         labels = np.array(labels)
     else:
         raise TypeError(
             f"Type of labels not understood. Only int, List[int] and np.ndarray are supported. Given: {type(labels)}."
         )
 
-    max_label = labels.max()
+    max_label = int(labels.max())
     if classes is None:
         classes = max_label
     if max_label > classes:
         raise ValueError(
             f"All labels must be smaller or equal to the number of classes. max_label: {max_label}, classes: {classes}"
         )
```

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,25 @@
     "K[305]": "K[UNIMOD:2016]",
     "K[214]": "K[UNIMOD:214]",
     "n[230]": "[UNIMOD:737]-",
     "n[305]": "[UNIMOD:2016]-",
     "n[214]": "[UNIMOD:214]-",
 }
 
+#######################
+# Xisearch constants #
+#######################
+
+XISEARCH_VAR_MODS = {
+    "ox": "[UNIMOD:35]",
+    "cm": "[UNIMOD:4]",
+    "dsso": "[UNIMOD:1896]",
+    "dsbu": "[UNIMOD:1884]",
+}
+
 ####################
 # MASS CALCULATION #
 ####################
 
 # initialize other masses
 PARTICLE_MASSES = {"PROTON": 1.007276467, "ELECTRON": 0.00054858}
```

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/fragments.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,28 +27,26 @@
 
 
 class FragmentsRatio(Metric):
     """Main to initialize a FragmentsRatio obj."""
 
     @staticmethod
     def count_with_ion_mask(
-        boolean_array: scipy.sparse.csr_matrix, ion_mask: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None
+        boolean_array: scipy.sparse.csr_matrix, ion_mask: Optional[Union[np.ndarray, scipy.sparse.spmatrix]] = None
     ) -> np.ndarray:
         """
         Count the number of ions.
 
         :param boolean_array: boolean array with True for observed/predicted peaks and \
                               False for missing observed/predicted peaks, array of length 174
         :param ion_mask: mask with 1s for the ions that should be counted and 0s for ions that should be ignored, \
                          integer array of length 174
         :return: number of observed/predicted peaks not masked by ion_mask
         """
         if ion_mask is None:
-            ion_mask = []
-        if len(ion_mask) == 0:
             ion_mask = scipy.sparse.csr_matrix(np.ones((174, 1)))
         else:
             ion_mask = scipy.sparse.csr_matrix(ion_mask).T
         return scipy.sparse.csr_matrix.dot(boolean_array, ion_mask).toarray().flatten()
 
     @staticmethod
     def count_observation_states(
```

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/percolator.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.0/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.5.1/spectrum_fundamentals/mod_string.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import difflib
 import re
 from itertools import repeat
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
-from .constants import MAXQUANT_VAR_MODS, MOD_MASSES, MOD_MASSES_SAGE, MOD_NAMES, MSFRAGGER_VAR_MODS, SPECTRONAUT_MODS
+import numpy as np
+import pandas as pd
+
+from .constants import (
+    MAXQUANT_VAR_MODS,
+    MOD_MASSES,
+    MOD_MASSES_SAGE,
+    MOD_NAMES,
+    MSFRAGGER_VAR_MODS,
+    SPECTRONAUT_MODS,
+    XISEARCH_VAR_MODS,
+)
 
 
 def sage_to_internal(sequences: List[str]) -> List[str]:
     """
     Convert mod string from sage to the internal format.
 
     This function converts sequences using the mass change of a modification in
@@ -50,26 +61,81 @@
         # Append the modified string to the 'modified_strings' list.
         modified_strings.append(modified_string)
 
     # Return the list of modified sequences.
     return modified_strings
 
 
-def internal_to_spectronaut(sequences: List[str]) -> List[str]:
+def xisearch_to_internal(
+    xl: str,
+    seq: str,
+    mod: str,
+    crosslinker_position: int,
+    mod_positions: str,
+):
+    """
+    Function to translate a xisearch modstring to the XL-Prosit format.
+
+    :param xl: type of crosslinker used. Can be 'DSSO' or 'DSBU'.
+    :param seq: unmodified peptide sequence
+    :param mod: all modifications of pep
+    :param crosslinker_position: crosslinker position of peptide
+    :param mod_positions: position of all modifications of peptide
+    :raises ValueError: if suplied type of crosslinker is unknown
+
+    :return: modified sequence
+    """
+
+    def add_mod_sequence(split_seq: List[str], mods: str, mod_positions: str):
+        """
+        Apply modifications.
+
+        :param split_seq: List containing the sequence characters
+        :param mods: String containing modifications
+        :param mod_positions: String containing positions of modifications
+        """
+        if mod_positions.lower() in ["", "nan", "null"]:
+            return
+
+        split_mod = mods.split(";")
+        split_mod_positions = mod_positions.split(";")
+
+        for mod, pos in zip(split_mod, split_mod_positions):
+            modification = XISEARCH_VAR_MODS.get(mod)
+            pos_mod = int(pos)
+            if modification:
+                split_seq[pos_mod - 1] += modification
+            else:
+                split_seq[pos_mod - 1] += f"({mod})"
+
+    # Check the crosslinker type and apply modification accordingly
+    modification = XISEARCH_VAR_MODS.get(xl.lower())
+    if modification is None:
+        raise ValueError(f"Unknown crosslinker type provided: {xl}. Only 'DSSO' and 'DSBU' are supported.")
+
+    split_seq = [x for x in seq]
+    add_mod_sequence(split_seq, mod, mod_positions)
+    split_seq[crosslinker_position - 1] += modification
+    return "".join(split_seq)
+
+
+def internal_to_spectronaut(sequences: Union[np.ndarray, pd.Series, List[str]]) -> List[str]:
     """
     Function to translate a modstring from the internal format to the spectronaut format.
 
     :param sequences: List[str] of sequences
     :return: List[str] of modified sequences
     """
     regex = re.compile("(%s)" % "|".join(map(re.escape, SPECTRONAUT_MODS.keys())))
     return [regex.sub(lambda mo: SPECTRONAUT_MODS[mo.string[mo.start() : mo.end()]], seq) for seq in sequences]
 
 
-def maxquant_to_internal(sequences: List[str], fixed_mods: Optional[Dict[str, str]] = None) -> List[str]:
+def maxquant_to_internal(
+    sequences: Union[np.ndarray, pd.Series, List[str]], fixed_mods: Optional[Dict[str, str]] = None
+) -> List[str]:
     """
     Function to translate a MaxQuant modstring to the Prosit format.
 
     :param sequences: List[str] of sequences
     :param fixed_mods: Optional dictionary of modifications with key aa and value mod, e.g. 'M': 'M(UNIMOD:35)'.
         Fixed modifications must be included in the variable modificatons dictionary.
         By default, i.e. if nothing is supplied to fixed_mods, carbamidomethylation on cystein will be included
@@ -112,15 +178,17 @@
                 key = f"{key}$"
 
         return replacements[key]
 
     return [regex.sub(find_replacement, seq).replace("_", "") for seq in sequences]
 
 
-def msfragger_to_internal(sequences: List[str], fixed_mods: Optional[Dict[str, str]] = None) -> List[str]:
+def msfragger_to_internal(
+    sequences: Union[np.ndarray, pd.Series, List[str]], fixed_mods: Optional[Dict[str, str]] = None
+) -> List[str]:
     """
     Function to translate a MSFragger modstring to the Prosit format.
 
     :param sequences: List[str] of sequences
     :param fixed_mods: Optional dictionary of modifications with key aa and value mod, e.g. 'M[147]': 'M(UNIMOD:35)'.
         Fixed modifications must be included in the variable modificatons dictionary.
         By default, i.e. if nothing is supplied to fixed_mods, carbamidomethylation on cystein will be included
```

### Comparing `spectrum_fundamentals-0.5.0/PKG-INFO` & `spectrum_fundamentals-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_fundamentals
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fundamental functions, annotation pipeline and constants for oktoberfest
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

