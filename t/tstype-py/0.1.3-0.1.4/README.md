# Comparing `tmp/tstype_py-0.1.3.tar.gz` & `tmp/tstype_py-0.1.4.tar.gz`

## Comparing `tstype_py-0.1.3.tar` & `tstype_py-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 tstype_py-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     5162 2024-03-29 08:40:44.000000 tstype_py-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-03-29 08:40:44.000000 tstype_py-0.1.3/.gitignore
--rw-r--r--   0     1001      127     1278 2024-03-29 08:40:44.000000 tstype_py-0.1.3/README.md
--rw-r--r--   0     1001      127      218 2024-03-29 08:40:44.000000 tstype_py-0.1.3/example.py
--rw-r--r--   0     1001      127     1090 2024-03-29 08:40:44.000000 tstype_py-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127    10341 2024-03-29 08:40:44.000000 tstype_py-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127      389 2024-03-29 08:40:44.000000 tstype_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 tstype_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 tstype_py-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     5162 2024-04-12 03:09:39.000000 tstype_py-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-12 03:09:39.000000 tstype_py-0.1.4/.gitignore
+-rw-r--r--   0     1001      127     1290 2024-04-12 03:09:39.000000 tstype_py-0.1.4/README.md
+-rw-r--r--   0     1001      127      227 2024-04-12 03:09:39.000000 tstype_py-0.1.4/example.py
+-rw-r--r--   0     1001      127     1090 2024-04-12 03:09:39.000000 tstype_py-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127    10341 2024-04-12 03:09:39.000000 tstype_py-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127      389 2024-04-12 03:09:39.000000 tstype_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 tstype_py-0.1.4/PKG-INFO
```

### Comparing `tstype_py-0.1.3/.github/workflows/CI.yml` & `tstype_py-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `tstype_py-0.1.3/.gitignore` & `tstype_py-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tstype_py-0.1.3/README.md` & `tstype_py-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 Use `build_type_definition` to convert the JSON string back to the type definition string.
 
 ```
 Python 3.11.7 (main, Dec  4 2023, 18:10:11) [Clang 15.0.0 (clang-1500.1.0.2.5)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import tstype_py as ts
 >>> import json
->>> text = "string|Map<string,Map<number, Array<string | number>>>[][]"
+>>> text = "string|Record<string,Record<number, Array<string | number>>>[][]"
 >>> # parse a type definition string into a JSON object
 >>> json.loads(ts.parse_type_definition(text))
 {'Union': [{'Basic': 'string'}, {'Array': {'Array': {'Map': [{'Basic': 'string'}, {'Map': [{'Basic': 'number'}, {'Array': {'Union': [{'Basic': 'string'}, {'Basic': 'number'}]}}]}]}}}]}
 >>> # convert the JSON string back to the type definition string
 >>> ts.parse_type_definition(text)
 '{"Union":[{"Basic":"string"},{"Array":{"Array":{"Map":[{"Basic":"string"},{"Map":[{"Basic":"number"},{"Array":{"Union":[{"Basic":"string"},{"Basic":"number"}]}}]}]}}}]}'
 >>> ts.build_type_definition('{"Union":[{"Basic":"string"},{"Array":{"Array":{"Map":[{"Basic":"string"},{"Map":[{"Basic":"number"},{"Array":{"Union":[{"Basic":"string"},{"Basic":"number"}]}}]}]}}}]}')
-'Map<string, Map<number, string | number[]>>[][] | string'
+'Record<string, Record<number, string | number[]>>[][] | string'
 ```
```

### Comparing `tstype_py-0.1.3/src/lib.rs` & `tstype_py-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tstype_py-0.1.3/Cargo.lock` & `tstype_py-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -296,26 +296,26 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tstype-py"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
  "serde",
  "serde_json",
  "tstype-rs",
 ]
 
 [[package]]
 name = "tstype-rs"
-version = "0.1.3"
-source = "git+https://github.com/xxxbrian/tstype-rs#1c2ffecc418175c5e2b1301038a70658ca596b57"
+version = "0.1.4"
+source = "git+https://github.com/xxxbrian/tstype-rs#e3215c93c5dd8d0a4c651fbfdcbe39224b2f6c52"
 dependencies = [
  "regex",
  "serde",
  "serde_json",
 ]
 
 [[package]]
```

### Comparing `tstype_py-0.1.3/PKG-INFO` & `tstype_py-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tstype-py
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 Use `parse_type_definition` to parse a type definition string into a JSON string.
@@ -12,18 +12,18 @@
 Use `build_type_definition` to convert the JSON string back to the type definition string.
 
 ```
 Python 3.11.7 (main, Dec  4 2023, 18:10:11) [Clang 15.0.0 (clang-1500.1.0.2.5)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import tstype_py as ts
 >>> import json
->>> text = "string|Map<string,Map<number, Array<string | number>>>[][]"
+>>> text = "string|Record<string,Record<number, Array<string | number>>>[][]"
 >>> # parse a type definition string into a JSON object
 >>> json.loads(ts.parse_type_definition(text))
 {'Union': [{'Basic': 'string'}, {'Array': {'Array': {'Map': [{'Basic': 'string'}, {'Map': [{'Basic': 'number'}, {'Array': {'Union': [{'Basic': 'string'}, {'Basic': 'number'}]}}]}]}}}]}
 >>> # convert the JSON string back to the type definition string
 >>> ts.parse_type_definition(text)
 '{"Union":[{"Basic":"string"},{"Array":{"Array":{"Map":[{"Basic":"string"},{"Map":[{"Basic":"number"},{"Array":{"Union":[{"Basic":"string"},{"Basic":"number"}]}}]}]}}}]}'
 >>> ts.build_type_definition('{"Union":[{"Basic":"string"},{"Array":{"Array":{"Map":[{"Basic":"string"},{"Map":[{"Basic":"number"},{"Array":{"Union":[{"Basic":"string"},{"Basic":"number"}]}}]}]}}}]}')
-'Map<string, Map<number, string | number[]>>[][] | string'
+'Record<string, Record<number, string | number[]>>[][] | string'
 ```
```

