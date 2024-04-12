# Comparing `tmp/qiskit-ionq-0.5.0.dev5.tar.gz` & `tmp/qiskit-ionq-0.5.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ionq-0.5.0.dev5.tar", last modified: Thu Feb 29 21:14:16 2024, max compression
+gzip compressed data, was "qiskit-ionq-0.5.1.dev0.tar", last modified: Fri Apr 12 19:37:12 2024, max compression
```

## Comparing `qiskit-ionq-0.5.0.dev5.tar` & `qiskit-ionq-0.5.1.dev0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.003820 qiskit-ionq-0.5.0.dev5/.eggs/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.003820 qiskit-ionq-0.5.0.dev5/.eggs/pytest_runner-6.0.1-py3.11.egg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.003820 qiskit-ionq-0.5.0.dev5/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/qiskit_ionq/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_gates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 21:14:15.000000 qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 21:14:16.007820 qiskit-ionq-0.5.0.dev5/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-29 21:14:08.000000 qiskit-ionq-0.5.0.dev5/test/test_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 19:37:11.000000 qiskit-ionq-0.5.1.dev0/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.405914 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/.eggs/pytest_runner-6.0.1-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.409914 qiskit-ionq-0.5.1.dev0/qiskit_ionq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:37:12.000000 qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:12.413914 qiskit-ionq-0.5.1.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-12 19:37:05.000000 qiskit-ionq-0.5.1.dev0/test/test_mock.py
```

### Comparing `qiskit-ionq-0.5.0.dev5/LICENSE.txt` & `qiskit-ionq-0.5.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/PKG-INFO` & `qiskit-ionq-0.5.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.5.0.dev5
+Version: 0.5.1.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
```

### Comparing `qiskit-ionq-0.5.0.dev5/README.md` & `qiskit-ionq-0.5.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/__init__.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/constants.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/exceptions.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 class IonQRetriableError(IonQError):
     """Errors that do not indicate a failure related to the request, and can be retried."""
 
     def __init__(self, cause):
         self._cause = cause
-        super().__init__(getattr(cause, 'message', 'Unknown error'))
+        super().__init__(getattr(cause, "message", "Unknown error"))
 
 
 # pylint: disable=no-member
 
 
 # https://support.cloudflare.com/hc/en-us/articles/115003014512-4xx-Client-Error
 # "Cloudflare will generate and serve a 409 response for a Error 1001: DNS Resolution Error."
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/helpers.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,45 +292,44 @@
                 sizes.append(size)
 
             labels.append(label)
 
     return sizes, labels
 
 
-def compress_dict_to_metadata_string(metadata_dict):  # pylint: disable=invalid-name
+def compress_to_metadata_string(metadata):  # pylint: disable=invalid-name
     """
-    Convert a dict to a compact string format (dumped, gzipped, base64 encoded)
+    Convert a metadata object to a compact string format (dumped, gzipped, base64 encoded)
     for storing in IonQ API metadata
 
     Parameters:
-        metadata_dict (dict): a dict with metadata relevant to building the results
-            object on a returned job.
+        metadata (dict or list): a dict or list of dicts with metadata relevant
+            to building the results object on a returned job.
 
     Returns:
         str: encoded string
 
     """
-    serialized = json.dumps(metadata_dict)
+    serialized = json.dumps(metadata)
     compressed = gzip.compress(serialized.encode("utf-8"))
     encoded = base64.b64encode(compressed)
-    encoded_string = encoded.decode()
-    return encoded_string
+    return encoded.decode()
 
 
-def decompress_metadata_string_to_dict(input_string):  # pylint: disable=invalid-name
+def decompress_metadata_string(input_string):  # pylint: disable=invalid-name
     """
     Convert compact string format (dumped, gzipped, base64 encoded) from
-    IonQ API metadata back into a dict relevant to building the results object
-    on a returned job.
+    IonQ API metadata back into a dict or list of dicts relevant to building
+    the results object on a returned job.
 
     Parameters:
         input_string (str): compressed string format of metadata dict
 
     Returns:
-        dict: decompressed metadata dict
+        dict or list: decompressed metadata dict or list of dicts
     """
     if input_string is None:
         return None
     encoded = input_string.encode()
     decoded = base64.b64decode(encoded)
     decompressed = gzip.decompress(decoded)
     return json.loads(decompressed)
@@ -350,60 +349,80 @@
 
     Returns:
         str: A string / JSON-serialized dictionary with IonQ API compatible values.
     """
     passed_args = passed_args or {}
     extra_query_params = extra_query_params or {}
     extra_metadata = extra_metadata or {}
-    ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(circuit, backend.gateset())
-    creg_sizes, clbit_labels = get_register_sizes_and_labels(circuit.cregs)
-    qreg_sizes, qubit_labels = get_register_sizes_and_labels(circuit.qregs)
-    qiskit_header = compress_dict_to_metadata_string(
+    ionq_circs = []
+    multi_circuit = False
+    if isinstance(circuit, (list, tuple)):
+        multi_circuit = True
+        for circ in circuit:
+            ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(circ, backend.gateset())
+            ionq_circs.append((ionq_circ, meas_map))
+    else:
+        ionq_circs, _, meas_map = qiskit_circ_to_ionq_circ(circuit, backend.gateset())
+        circuit = [circuit]
+
+    metadata_list = [
         {
-            "memory_slots": circuit.num_clbits,  # int
-            "global_phase": circuit.global_phase,  # float
-            "n_qubits": circuit.num_qubits,  # int
-            "name": circuit.name,  # str
+            "memory_slots": circ.num_clbits,  # int
+            "global_phase": circ.global_phase,  # float
+            "n_qubits": circ.num_qubits,  # int
+            "name": circ.name,  # str
             # list of [str, int] tuples cardinality memory_slots
-            "creg_sizes": creg_sizes,
+            "creg_sizes": get_register_sizes_and_labels(circ.cregs)[0],
             # list of [str, int] tuples cardinality memory_slots
-            "clbit_labels": clbit_labels,
+            "clbit_labels": get_register_sizes_and_labels(circ.cregs)[1],
             # list of [str, int] tuples cardinality num_qubits
-            "qreg_sizes": qreg_sizes,
+            "qreg_sizes": get_register_sizes_and_labels(circ.qregs)[0],
             # list of [str, int] tuples cardinality num_qubits
-            "qubit_labels": qubit_labels,
+            "qubit_labels": get_register_sizes_and_labels(circ.qregs)[1],
+            # custom metadata from the circuits
+            **({"metadata": circ.metadata} if circ.metadata else {}),
         }
+        for circ in circuit
+    ]
+
+    qiskit_header = compress_to_metadata_string(
+        metadata_list if multi_circuit else metadata_list[0]
     )
 
     target = backend.name()[5:] if backend.name().startswith("ionq") else backend.name()
     if target == "qpu":
         target = "qpu.harmony"  # todo default to cheapest available option
         warnings.warn(
             "The ionq_qpu backend is deprecated. Defaulting to ionq_qpu.harmony.",
             DeprecationWarning,
             stacklevel=2,
         )
     ionq_json = {
         "target": target,
         "shots": passed_args.get("shots"),
-        "name": circuit.name,
+        "name": ", ".join([c.name for c in circuit]),
         "input": {
             "format": "ionq.circuit.v0",
             "gateset": backend.gateset(),
-            "qubits": circuit.num_qubits,
-            "circuit": ionq_circ,
+            "qubits": max(c.num_qubits for c in circuit),
         },
-        "registers": {"meas_mapped": meas_map} if meas_map else {},
         # store a couple of things we'll need later for result formatting
         "metadata": {
             "shots": str(passed_args.get("shots")),
             "sampler_seed": str(passed_args.get("sampler_seed")),
             "qiskit_header": qiskit_header,
         },
     }
+    if multi_circuit:
+        ionq_json["input"]["circuits"] = [
+            {"circuit": c, "registers": {"meas_mapped": m}} for c, m in ionq_circs
+        ]
+    else:
+        ionq_json["input"]["circuit"] = ionq_circs
+        ionq_json["registers"] = {"meas_mapped": meas_map} if meas_map else {}
     if target == "simulator":
         ionq_json["noise"] = {
             "model": passed_args.get("noise_model") or backend.options.noise_model,
             "seed": backend.options.sampler_seed,
         }
     ionq_json.update(extra_query_params)
     # merge circuit and extra metadata
@@ -461,11 +480,11 @@
 
         return "unknown"
 
 
 __all__ = [
     "qiskit_to_ionq",
     "qiskit_circ_to_ionq_circ",
-    "compress_dict_to_metadata_string",
-    "decompress_metadata_string_to_dict",
+    "compress_to_metadata_string",
+    "decompress_metadata_string",
     "get_user_agent",
 ]
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_backend.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,49 +190,41 @@
 
         return ionq_client.IonQClient(token, url, self._provider.custom_headers)
 
     # pylint: disable=missing-type-doc,missing-param-doc,arguments-differ,arguments-renamed
     def run(self, circuit, **kwargs):
         """Create and run a job on an IonQ Backend.
 
-        .. NOTE::
-
-            IonQ backends do not support multi-experiment jobs.
-            If ``circuit`` is provided as a list with more than one element
-            then this method will raise out with a RuntimeError.
-
         Args:
             circuit (:class:`QuantumCircuit <qiskit.circuit.QuantumCircuit>`):
                 A Qiskit QuantumCircuit object.
 
         Returns:
             IonQJob: A reference to the job that was submitted.
-
-        Raises:
-            RuntimeError: If a multi-experiment circuit was provided.
         """
-        if isinstance(circuit, (list, tuple)):
-            if len(circuit) > 1:
-                raise RuntimeError("Multi-experiment jobs are not supported!")
-            circuit = circuit[0]
-
-        if not self.has_valid_mapping(circuit):
+        if not all(
+            (
+                self.has_valid_mapping(circ)
+                for circ in (circuit if isinstance(circuit, list) else [circuit])
+            )
+        ):
             warnings.warn(
-                f"Circuit {circuit.name} is not measuring any qubits",
+                "Circuit is not measuring any qubits",
                 UserWarning,
                 stacklevel=2,
             )
 
         for kwarg in kwargs:
             if not hasattr(self.options, kwarg):
                 warnings.warn(
                     f"Option {kwarg} is not used by this backend",
                     UserWarning,
                     stacklevel=2,
                 )
+
         if "shots" not in kwargs:
             kwargs["shots"] = self.options.shots
         # TODO: Should we merge the two maps, or warn if both are set?
         if "job_settings" not in kwargs:
             kwargs["job_settings"] = self.options.job_settings
         elif self.options.job_settings is not None:
             warnings.warn(
@@ -390,20 +382,22 @@
             NoneType: None
         """
         return None
 
     def gateset(self):
         return self._gateset
 
-    def __init__(self, provider, name="ionq_simulator", gateset="qis"):
+    def __init__(self, provider, name="simulator", gateset="qis"):
         """Base class for interfacing with an IonQ backend"""
         self._gateset = gateset
         config = BackendConfiguration.from_dict(
             {
-                "backend_name": name,
+                "backend_name": (
+                    "ionq_" + name if not name.startswith("ionq_") else name
+                ),
                 "backend_version": "0.0.1",
                 "simulator": True,
                 "local": False,
                 "coupling_map": None,
                 "description": "IonQ simulator",
                 "basis_gates": GATESET_MAP[gateset],
                 "memory": False,
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_client.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Basic API Client for IonQ's REST API"""
 
+import json
+from collections import OrderedDict
 from typing import Optional
 from warnings import warn
 import requests
 
 from retry import retry
 
 from . import exceptions
@@ -90,15 +92,18 @@
             IonQRetriableError: When a retriable error occurs during the request.
 
         Returns:
             Response: A requests.Response object.
         """
         try:
             res = requests.get(
-                req_path, params=params, headers=headers, timeout=timeout
+                req_path,
+                params=params,
+                headers=headers,
+                timeout=timeout,
             )
         except requests.exceptions.RequestException as req_exc:
             raise IonQRetriableError(req_exc) from req_exc
 
         return res
 
     @retry(exceptions=IonQRetriableError, tries=5)
@@ -262,11 +267,12 @@
                 )
             )
             params.update(extra_query_params)
 
         req_path = self.make_path("jobs", job_id, "results")
         res = self._get_with_retry(req_path, headers=self.api_headers, params=params)
         exceptions.IonQAPIError.raise_for_status(res)
-        return res.json()
+        # Use json.loads with object_pairs_hook to maintain order of JSON keys
+        return json.loads(res.text, object_pairs_hook=OrderedDict)
 
 
 __all__ = ["IonQClient"]
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_gates.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,20 @@
              |MS(ϴ,0)|
         q_1: ┤       ├-
              └───────┘
     **Matrix representation:**
 
     .. math::
 
-       MS(\phi_0, _\phi_1, \theta) q_0, q_1 =
+       MS(\phi_0, \phi_1, \theta) =
             \begin{pmatrix}
-                cos{\theta*\pi} & 0 & 0 & -i*e^{-i*2*\pi(\phi_0+\phi_1)}*sin{\theta*\pi} \\
-                0 & cos{\theta*\pi} & -i*e^{-i*2*\pi(\phi_0-\phi_1)}*sin{\theta*\pi} & 0 \\
-                0 & -i*e^{i*2*\pi(\phi_0-\phi_1)}*sin(\theta*\pi) & cos{\theta*\pi} & 0 \\
-                -i*e^{i*2*\pi(\phi_0+\phi_1)}*sin{\theta*\pi} & 0 & 0 & cos{\theta*\pi}
+                cos(\theta*\pi) & 0 & 0 & -i*e^{-i*2*\pi(\phi_0+\phi_1)}*sin(\theta*\pi) \\
+                0 & cos(\theta*\pi) & -i*e^{i*2*\pi(\phi_0-\phi_1)}*sin(\theta*\pi) & 0 \\
+                0 & -i*e^{-i*2*\pi(\phi_0-\phi_1)}*sin(\theta*\pi) & cos(\theta*\pi) & 0 \\
+                -i*e^{i*2*\pi(\phi_0+\phi_1)}*sin(\theta*\pi) & 0 & 0 & cos(\theta*\pi)
             \end{pmatrix}
     """
 
     def __init__(
         self,
         phi0: ParameterValueType,
         phi1: ParameterValueType,
@@ -136,16 +136,16 @@
         theta = self.params[2]
         diag = numpy.cos(math.pi * theta)
         sin = numpy.sin(math.pi * theta)
 
         return numpy.array(
             [
                 [diag, 0, 0, sin * -1j * cmath.exp(-1j * 2 * math.pi * (phi0 + phi1))],
-                [0, diag, sin * -1j * cmath.exp(-1j * 2 * math.pi * (phi0 - phi1)), 0],
-                [0, sin * -1j * cmath.exp(1j * 2 * math.pi * (phi0 - phi1)), diag, 0],
+                [0, diag, sin * -1j * cmath.exp(1j * 2 * math.pi * (phi0 - phi1)), 0],
+                [0, sin * -1j * cmath.exp(-1j * 2 * math.pi * (phi0 - phi1)), diag, 0],
                 [sin * -1j * cmath.exp(1j * 2 * math.pi * (phi0 + phi1)), 0, 0, diag],
             ],
             dtype=dtype,
         )
 
 
 class ZZGate(Gate):
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_job.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 import warnings
 import numpy as np
 
 from qiskit.providers import JobV1, jobstatus
 from qiskit.providers.exceptions import JobTimeoutError
 from .ionq_result import IonQResult as Result
-from .helpers import decompress_metadata_string_to_dict
+from .helpers import decompress_metadata_string
 
 
 from . import constants, exceptions
 
 
 def map_output(data, clbits, num_qubits):
     """Map histogram according to measured bits"""
@@ -123,15 +123,15 @@
 
         rand_values = rand.choice(outcomes, shots, p=weights)
 
         sampled.update(
             {key: np.count_nonzero(rand_values == key) for key in output_probs}
         )
 
-    # Build counts.
+    # Build counts
     counts = {}
     for key, val in output_probs.items():
         bits = bin(int(key))[2:].rjust(num_qubits, "0")
         hex_bits = hex(int(bits, 2))
         count = sampled[key] if use_sampler else round(val * shots)
         counts[hex_bits] = count
     # build probs
@@ -143,18 +143,14 @@
 
     return counts, probabilities
 
 
 class IonQJob(JobV1):
     """Representation of a Job that will run on an IonQ backend.
 
-    .. IMPORTANT::
-       IonQ backends do not support multi-experiment jobs.  Attempting to
-       submit a multi-experiment job will raise an exception.
-
     It is not recommended to create Job instances directly, but rather use the
     :meth:`run <IonQBackend.run>` and :meth:`retrieve_job <IonQBackend.retrieve_job>`
     methods on sub-class instances of IonQBackend to create and retrieve jobs
     (both methods return a job instance).
 
     Attributes:
         circuit(:mod:`QuantumCircuit <qiskit.QuantumCircuit>`): A possibly ``None``
@@ -176,24 +172,22 @@
         self._result = None
         self._status = None
         self._execution_time = None
         self._metadata = {}
 
         if passed_args is not None:
             self.extra_query_params = passed_args.pop("extra_query_params", {})
-            self.extra_metadata = {
-                **passed_args.pop("extra_metadata", {}),
-                **(circuit.metadata or {}),
-            }
+            self.extra_metadata = passed_args.pop("extra_metadata", {})
             self._passed_args = passed_args
         else:
             self.extra_query_params = {}
             self.extra_metadata = {}
             self._passed_args = {"shots": 1024, "sampler_seed": None}
 
+        # Handle both single and list of circuits
         if circuit is not None:
             self.circuit = circuit
             self._status = jobstatus.JobStatus.INITIALIZING
         else:  # retrieve existing job
             self.circuit = None
             self._status = jobstatus.JobStatus.INITIALIZING
             self._job_id = job_id
@@ -345,19 +339,19 @@
                 f"Qiskit has no JobStatus named '{status_enum}'"
             ) from ex
 
         if self._status in jobstatus.JOB_FINAL_STATES:
             self._save_metadata(response)
 
         if self._status == jobstatus.JobStatus.DONE:
-            self._num_qubits = response.get("qubits")
+            self._num_circuits = response.get("circuits", 1)
+            self._children = response.get("children", [])
+            self._num_qubits = response.get("qubits", 0)
             default_map = list(range(self._num_qubits))
-            self._clbits = (response.get("registers") or {}).get(
-                "meas_mapped", default_map
-            )
+            self._clbits = response.get("registers", {}).get("meas_mapped", default_map)
             self._execution_time = response.get("execution_time") / 1000
 
         if self._status == jobstatus.JobStatus.ERROR:
             failure = response.get("failure") or {}
             failure_type = failure.get("code", "")
             failure_message = failure.get("error", "")
             error_message = (
@@ -406,47 +400,66 @@
         success = self._status == jobstatus.JobStatus.DONE
         metadata = self._metadata.get("metadata", {})
         sampler_seed = (
             int(metadata.get("sampler_seed", ""))
             if metadata.get("sampler_seed", "").isdigit()
             else None
         )
-        qiskit_header = decompress_metadata_string_to_dict(
-            metadata.get("qiskit_header", None)
+        qiskit_header = decompress_metadata_string(metadata.get("qiskit_header", None))
+        if not isinstance(qiskit_header, list):
+            qiskit_header = [qiskit_header]
+        shots = (
+            int(metadata.get("shots", 1024))
+            if str(metadata.get("shots", "1024")).isdigit()
+            else 1024
         )
-
-        shots = int(metadata.get("shots") if metadata.get("shots").isdigit() else 1024)
-        job_result = {
-            "data": {},
-            "shots": shots,
-            "header": qiskit_header or {},
-            "success": success,
-        }
-        if self._status == jobstatus.JobStatus.DONE:
-            (counts, probabilities) = _build_counts(
-                data,
-                self._num_qubits,
-                self._clbits,
-                shots,
-                use_sampler=is_ideal_simulator,
-                sampler_seed=sampler_seed,
-            )
-            job_result["data"] = {
-                "counts": counts,
-                "probabilities": probabilities,
-                # Qiskit/experiments relies on this being present in this location in the
-                # ExperimentData class.
-                "metadata": qiskit_header or {},
+        job_result = [
+            {
+                "data": {},
+                "shots": shots,
+                "header": qiskit_header[i] or {},
+                "success": success,
             }
+            for i in range(self._num_circuits)
+        ]
+        if self._status == jobstatus.JobStatus.DONE:
+            # to handle ionq returning different data structures for single and multiple circuits
+            if self._num_circuits > 1:
+                data = list(data.values())
+            else:
+                data = [data]
+            for i in range(self._num_circuits):
+                (counts, probabilities) = _build_counts(
+                    data[i],
+                    qiskit_header[i].get("n_qubits", self._num_qubits),
+                    range(
+                        sum(
+                            creg[1]
+                            for creg in qiskit_header[i].get(
+                                "creg_sizes", [["meas", len(self._clbits)]]
+                            )
+                        )
+                    ),
+                    shots,
+                    use_sampler=is_ideal_simulator,
+                    sampler_seed=sampler_seed,
+                )
+                job_result[i]["data"] = {
+                    "counts": counts,
+                    "probabilities": probabilities,
+                    # Qiskit/experiments relies on this being present in this location in the
+                    # ExperimentData class.
+                    "metadata": qiskit_header[i] or {},
+                }
 
         # Create a qiskit result to express the IonQ job result data.
         backend = self.backend()
         return Result.from_dict(
             {
-                "results": [job_result],
+                "results": job_result,
                 "job_id": self.job_id(),
                 "backend_name": backend_name,
                 "backend_version": backend_version,
                 "qobj_id": metadata.get("qobj_id"),
                 "success": success,
                 "time_taken": self._execution_time,
             }
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_provider.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provider for interacting with IonQ backends"""
 
 import logging
 import os
+from dotenv import dotenv_values
 
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.providers.providerutils import filter_backends
 
 from . import ionq_backend
 
 logger = logging.getLogger(__name__)
@@ -50,19 +51,27 @@
         token (str): IonQ API access token.
         url (str, optional): IonQ API url. Defaults to ``None``.
 
     Returns:
         dict[str]: A dict with "token" and "url" keys, for use by a client.
     """
     env_token = (
-        os.environ.get("QISKIT_IONQ_API_TOKEN")
-        or os.environ.get("IONQ_API_TOKEN")
-        or os.environ.get("IONQ_API_KEY")
+        dotenv_values().get("QISKIT_IONQ_API_TOKEN")  # first check for dotenv values
+        or dotenv_values().get("IONQ_API_KEY")
+        or dotenv_values().get("IONQ_API_TOKEN")
+        or os.getenv("QISKIT_IONQ_API_TOKEN")  # then check for global env values
+        or os.getenv("IONQ_API_KEY")
+        or os.getenv("IONQ_API_TOKEN")
+    )
+    env_url = (
+        dotenv_values().get("QISKIT_IONQ_API_URL")
+        or dotenv_values().get("IONQ_API_URL")
+        or os.getenv("QISKIT_IONQ_API_URL")
+        or os.getenv("IONQ_API_URL")
     )
-    env_url = os.environ.get("QISKIT_IONQ_API_URL") or os.environ.get("IONQ_API_URL")
     return {
         "token": token or env_token,
         "url": url or env_url or "https://api.ionq.co/v0.3",
     }
 
 
 class IonQProvider:
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/ionq_result.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/ionq_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq/version.py` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 import os
 import pathlib
 import subprocess
 from typing import List
 
 pkg_parent = pathlib.Path(__file__).parent.parent.absolute()
 
-# major, minor, micro
-VERSION_INFO = ".".join(map(str, (0, 5, 0, "dev5")))
+# major, minor, patch
+VERSION_INFO = ".".join(map(str, (0, 5, 1, "dev0")))
 
 
 def _minimal_ext_cmd(cmd: List[str]) -> bytes:
     # construct minimal environment
     env = {
         "LANGUAGE": "C",  # LANGUAGE is used on win32
         "LANG": "C",
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/PKG-INFO` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.5.0.dev5
+Version: 0.5.1.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
```

### Comparing `qiskit-ionq-0.5.0.dev5/qiskit_ionq.egg-info/SOURCES.txt` & `qiskit-ionq-0.5.1.dev0/qiskit_ionq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/setup.py` & `qiskit-ionq-0.5.1.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/test/test_exceptions.py` & `qiskit-ionq-0.5.1.dev0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.5.0.dev5/test/test_mock.py` & `qiskit-ionq-0.5.1.dev0/test/test_mock.py`

 * *Files identical despite different names*

