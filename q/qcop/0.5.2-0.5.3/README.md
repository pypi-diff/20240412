# Comparing `tmp/qcop-0.5.2.tar.gz` & `tmp/qcop-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcop-0.5.2.tar", max compression
+gzip compressed data, was "qcop-0.5.3.tar", max compression
```

## Comparing `qcop-0.5.2.tar` & `qcop-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-04-10 16:39:47.807119 qcop-0.5.2/LICENSE
--rw-r--r--   0        0        0     7283 2024-04-10 16:39:47.807119 qcop-0.5.2/README.md
--rw-r--r--   0        0        0     1818 2024-04-10 16:39:47.807119 qcop-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      248 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/__init__.py
--rw-r--r--   0        0        0      360 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/__init__.py
--rw-r--r--   0        0        0    12380 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/base.py
--rw-r--r--   0        0        0     1487 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/file.py
--rw-r--r--   0        0        0    11141 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/geometric.py
--rw-r--r--   0        0        0     2111 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/qcengine.py
--rw-r--r--   0        0        0     4662 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/terachem.py
--rw-r--r--   0        0        0     7899 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/utils.py
--rw-r--r--   0        0        0     4122 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/adapters/xtb.py
--rw-r--r--   0        0        0     3639 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/exceptions.py
--rw-r--r--   0        0        0     3134 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/main.py
--rw-r--r--   0        0        0        0 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/py.typed
--rw-r--r--   0        0        0     3363 2024-04-10 16:39:47.811118 qcop-0.5.2/qcop/utils.py
--rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-11 22:35:46.722615 qcop-0.5.3/LICENSE
+-rw-r--r--   0        0        0     7283 2024-04-11 22:35:46.722615 qcop-0.5.3/README.md
+-rw-r--r--   0        0        0     1832 2024-04-11 22:35:46.726615 qcop-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      248 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/__init__.py
+-rw-r--r--   0        0        0    12380 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/base.py
+-rw-r--r--   0        0        0     1487 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/file.py
+-rw-r--r--   0        0        0    11141 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/geometric.py
+-rw-r--r--   0        0        0     2111 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/qcengine.py
+-rw-r--r--   0        0        0     4662 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/terachem.py
+-rw-r--r--   0        0        0     8709 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/utils.py
+-rw-r--r--   0        0        0     4419 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/adapters/xtb.py
+-rw-r--r--   0        0        0     3639 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/exceptions.py
+-rw-r--r--   0        0        0     3134 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/main.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/py.typed
+-rw-r--r--   0        0        0     3363 2024-04-11 22:35:46.726615 qcop-0.5.3/qcop/utils.py
+-rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 qcop-0.5.3/PKG-INFO
```

### Comparing `qcop-0.5.2/LICENSE` & `qcop-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/README.md` & `qcop-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/pyproject.toml` & `qcop-0.5.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qcop"
-version = "0.5.2"
+version = "0.5.3"
 description = "A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,14 +26,15 @@
 mypy = "^1.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 ruff = "^0.0.272"
 isort = "^5.12.0"
 pytest-mock = "^3.11.1"
 geometric = "^1.0.1"
+xtb = "^22.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `qcop-0.5.2/qcop/adapters/base.py` & `qcop-0.5.3/qcop/adapters/base.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/adapters/file.py` & `qcop-0.5.3/qcop/adapters/file.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/adapters/geometric.py` & `qcop-0.5.3/qcop/adapters/geometric.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/adapters/qcengine.py` & `qcop-0.5.3/qcop/adapters/qcengine.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/adapters/terachem.py` & `qcop-0.5.3/qcop/adapters/terachem.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/adapters/utils.py` & `qcop-0.5.3/qcop/adapters/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import logging
 import os
 import platform
 import shutil
 import subprocess
+import sys
 import tempfile
 from contextlib import contextmanager
 from io import StringIO
 from pathlib import Path
 from time import time
 from typing import Callable, List, Optional, Union
 
@@ -175,14 +176,43 @@
     try:
         yield (logger, logs_string)
     finally:
         # Remove the handler when done
         logger.removeHandler(handler)
 
 
+@contextmanager
+def capture_sys_stdout():
+    """Capture stdout from a program that bypasses the sys.stdout object.
+
+    Useful for capturing logs written by C/C++ libraries such as xtb.
+    """
+    # Create a pipe to capture output
+    r, w = os.pipe()
+
+    # Save the original stdout and stderr file descriptors
+    stdout_fd = sys.stdout.fileno()
+    old_stdout = os.dup(stdout_fd)
+
+    # Redirect stdout and stderr to the write end of the pipe
+    os.dup2(w, stdout_fd)
+    try:
+        yield r  # Allow code to be executed within the context manager block
+    finally:
+        # Restore stdout and stderr
+        os.dup2(old_stdout, stdout_fd)
+
+        # Close the duplicated fds
+        os.close(old_stdout)
+        os.close(w)
+
+        # Close the read ends of the pipe
+        os.close(r)
+
+
 def construct_provenance(
     program: str,
     version: Optional[str],
     scratch_dir: Path,
     wall_time: float,
 ) -> Provenance:
     """Construct a provenance object for a calculation.
```

### Comparing `qcop-0.5.2/qcop/adapters/xtb.py` & `qcop-0.5.3/qcop/adapters/xtb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Adaptor for xtb-python package.
 
 Great overview of how to implement this adaptor:
 https://github.com/grimme-lab/xtb-python/blob/main/xtb/qcschema/harness.py
 """
 
 import importlib
-from pathlib import Path
+import os
 from typing import Callable, Optional, Tuple
 
 import numpy as np
 from qcio import CalcType, ProgramInput, SinglePointResults, Wavefunction
 from qcio.constants import ELEMENTS
 
 from qcop.exceptions import (
     AdapterInputError,
     ExternalProgramError,
     ProgramNotFoundError,
 )
 
 from .base import ProgramAdapter
+from .utils import capture_sys_stdout
 
 
 class XTBAdapter(ProgramAdapter):
     """Adapter for xtb-python."""
 
     supported_calctypes = [CalcType.energy, CalcType.gradient]
     program = "xtb"
@@ -49,15 +50,15 @@
 
         Args:
             stdout: The stdout from the program.
 
         Returns:
             The program version.
         """
-        return self.xtb.__version__
+        return importlib.metadata.version(self.program)
 
     @staticmethod
     def _ensure_xtb():
         try:
             xtb = importlib.import_module("xtb")
             # xtb import structure is screwed up so I have to do this too
             importlib.import_module("xtb.interface")
@@ -90,36 +91,40 @@
             atomic_numbers = np.array(
                 [ELEMENTS[sym] for sym in inp_obj.molecule.symbols]
             )
             calc = self.xtb.interface.Calculator(
                 getattr(self.xtb.interface.Param, inp_obj.model.method),
                 atomic_numbers,
                 inp_obj.molecule.geometry,
+                inp_obj.molecule.charge,
+                # From https://github.com/grimme-lab/xtb-python/blob/a32309a43e5a6572b033814eacf396328a2a36ed/xtb/qcschema/harness.py#L126 # noqa: E501
+                inp_obj.molecule.multiplicity - 1,
             )
+            calc.set_verbosity(self.xtb.libxtb.VERBOSITY_FULL)  # all logs
+
             # Set Keywords
             for key, value in inp_obj.keywords.items():
                 # TODO: Need to handle external_charges and solvent
                 getattr(calc, f"set_{key}")(value)
 
-            # Always set verbosity high
-            calc.set_verbosity(self.xtb.libxtb.VERBOSITY_FULL)
-            logs = "logs.out"
-            calc.set_output(logs)
-
-            # Perform Calculation
-            res = calc.singlepoint()
-            # Collect logs
-            stdout = Path(logs).read_text()
+            # Capture logs
+            with capture_sys_stdout() as r_pipe:
+                res = calc.singlepoint()
+                # Not sure what this does but it's in the xtb-python docs
+                calc.release_output()
+                stdout = os.read(r_pipe, 100000).decode()
+
         except self.xtb.interface.XTBException as e:
             raise ExternalProgramError("Something went wrong with xtb-python.") from e
-        else:
-            # Collect results
-            # TODO: Collect other results like
-            results = SinglePointResults(
-                energy=res.get_energy(),
-                gradient=res.get_gradient(),
-                scf_dipole_moment=res.get_dipole(),
-                wavefunction=Wavefunction(
-                    scf_eigenvalues_a=res.get_orbital_eigenvalues(),
-                ),
-            )
+
+        # Collect results
+        # TODO: Collect other results xtb produces
+        results = SinglePointResults(
+            energy=res.get_energy(),
+            gradient=res.get_gradient(),
+            scf_dipole_moment=res.get_dipole(),
+            wavefunction=Wavefunction(
+                scf_eigenvalues_a=res.get_orbital_eigenvalues(),
+            ),
+        )
+
         return results, stdout
```

### Comparing `qcop-0.5.2/qcop/exceptions.py` & `qcop-0.5.3/qcop/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/main.py` & `qcop-0.5.3/qcop/main.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/qcop/utils.py` & `qcop-0.5.3/qcop/utils.py`

 * *Files identical despite different names*

### Comparing `qcop-0.5.2/PKG-INFO` & `qcop-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcop
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for operating Quantum Chemistry programs using qcio standardized data structures. Compatible with TeraChem, psi4, QChem, NWChem, ORCA, Molpro, geomeTRIC and many more.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

