# Comparing `tmp/rjsonnet-0.5.3.tar.gz` & `tmp/rjsonnet-0.5.4.tar.gz`

## Comparing `rjsonnet-0.5.3.tar` & `rjsonnet-0.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 rjsonnet-0.5.3/Cargo.toml
--rw-r--r--   0      501       20      442 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/.github/dependabot.yml
--rw-r--r--   0      501       20     6611 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/.github/workflows/CI.yml
--rw-r--r--   0      501       20      646 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/.gitignore
--rw-r--r--   0      501       20     1086 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/LICENSE
--rw-r--r--   0      501       20     2142 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/README.md
--rw-r--r--   0      501       20       74 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/pyproject.toml
--rw-r--r--   0      501       20     1185 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/rjsonnet.pyi
--rw-r--r--   0      501       20    14889 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/src/lib.rs
--rw-r--r--   0      501       20      255 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/tests/test.jsonnet
--rw-r--r--   0      501       20     2691 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/tests/test_rjsonnet.py
--rw-r--r--   0      501       20    20065 2023-09-02 05:26:52.000000 rjsonnet-0.5.3/Cargo.lock
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 rjsonnet-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 rjsonnet-0.5.4/Cargo.toml
+-rw-r--r--   0      501       20      442 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/.github/dependabot.yml
+-rw-r--r--   0      501       20     6910 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      646 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/.gitignore
+-rw-r--r--   0      501       20     1086 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/LICENSE
+-rw-r--r--   0      501       20     2142 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/README.md
+-rw-r--r--   0      501       20     1185 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/rjsonnet.pyi
+-rw-r--r--   0      501       20    15151 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/src/lib.rs
+-rw-r--r--   0      501       20      255 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/tests/test.jsonnet
+-rw-r--r--   0      501       20     2966 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/tests/test_rjsonnet.py
+-rw-r--r--   0      501       20    21008 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/Cargo.lock
+-rw-r--r--   0      501       20       74 2024-04-12 13:55:39.000000 rjsonnet-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 rjsonnet-0.5.4/PKG-INFO
```

### Comparing `rjsonnet-0.5.3/.github/workflows/CI.yml` & `rjsonnet-0.5.4/.github/workflows/CI.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     tags: [ 'v*' ]
   pull_request:
 
 jobs:
   macos:
     runs-on: macos-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.9
       - uses: dtolnay/rust-toolchain@nightly
       - name: Build wheels - x86_64
         uses: messense/maturin-action@v1
         with:
           target: x86_64
@@ -32,27 +32,27 @@
           target: universal2-apple-darwin
           args: --release --out dist --features nightly
       - name: Install built wheel - universal2
         run: |
           pip install rjsonnet --no-index --find-links dist --force-reinstall
           cd tests && pytest
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos
           path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.9
           architecture: ${{ matrix.target }}
       - uses: dtolnay/rust-toolchain@nightly
       - name: Build wheels
         uses: messense/maturin-action@v1
         with:
@@ -60,27 +60,27 @@
           args: --release --out dist --features nightly
       - name: Install built wheel
         run: |
           pip install rjsonnet --no-index --find-links dist --force-reinstall
           pip install pytest
           cd tests && pytest
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-windows-${{ matrix.target }}
           path: dist
 
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [x86_64, i686]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Build wheels
       uses: messense/maturin-action@v1
       with:
         rust-toolchain: nightly
         target: ${{ matrix.target }}
@@ -89,66 +89,66 @@
     - name: Install built wheel
       if: matrix.target == 'x86_64'
       run: |
         pip install rjsonnet --no-index --find-links dist --force-reinstall
         pip install pytest
         cd tests && pytest
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-linux-${{ matrix.target }}
         path: dist
 
   linux-cross:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target: [aarch64, armv7, s390x, ppc64le]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Build wheels
       uses: messense/maturin-action@v1
       with:
         rust-toolchain: nightly
         target: ${{ matrix.target }}
         manylinux: auto
         args: --release --out dist --features nightly
-    - uses: uraimo/run-on-arch-action@v2.5.1
+    - uses: uraimo/run-on-arch-action@v2.7.1
       if: matrix.target != 'ppc64'
       name: Install built wheel
       with:
         arch: ${{ matrix.target }}
         distro: ubuntu20.04
         githubToken: ${{ github.token }}
         install: |
           apt-get update
           apt-get install -y --no-install-recommends python3 python3-pip
           pip3 install -U pip pytest
         run: |
           pip3 install rjsonnet --no-index --find-links dist/ --force-reinstall
           cd tests && pytest
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-linux-${{ matrix.target }}
         path: dist
 
   musllinux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         target:
           - x86_64-unknown-linux-musl
           - i686-unknown-linux-musl
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: 3.9
         architecture: x64
     - name: Build wheels
       uses: messense/maturin-action@v1
       with:
         rust-toolchain: nightly
@@ -158,75 +158,80 @@
     - name: Install built wheel
       if: matrix.target == 'x86_64-unknown-linux-musl'
       uses: addnab/docker-run-action@v3
       with:
         image: alpine:latest
         options: -v ${{ github.workspace }}:/io -w /io
         run: |
-          apk add py3-pip
-          pip3 install -U pip pytest
-          pip3 install rjsonnet --no-index --find-links /io/dist/ --force-reinstall
+          apk add py3-virtualenv
+          virtualenv .venv
+          source .venv/bin/activate
+          pip install pytest
+          pip install rjsonnet --no-index --find-links /io/dist/ --force-reinstall
           cd tests && python3 -m pytest
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-${{ matrix.target }}
         path: dist
 
   musllinux-cross:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         platform:
           - target: aarch64-unknown-linux-musl
             arch: aarch64
           - target: armv7-unknown-linux-musleabihf
             arch: armv7
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: 3.9
     - name: Build wheels
       uses: messense/maturin-action@v1
       with:
         rust-toolchain: nightly
         target: ${{ matrix.platform.target }}
         manylinux: musllinux_1_2
         args: --release --out dist --features nightly
-    - uses: uraimo/run-on-arch-action@v2.5.1
+    - uses: uraimo/run-on-arch-action@v2.7.1
       name: Install built wheel
       with:
         arch: ${{ matrix.platform.arch }}
         distro: alpine_latest
         githubToken: ${{ github.token }}
         install: |
-          apk add py3-pip
-          pip3 install -U pip pytest
+          apk add py3-virtualenv
         run: |
-          pip3 install rjsonnet --no-index --find-links dist/ --force-reinstall
+          virtualenv .venv
+          source .venv/bin/activate
+          pip install pytest
+          pip install rjsonnet --no-index --find-links dist/ --force-reinstall
           cd tests && python3 -m pytest
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-${{ matrix.platform.target }}
         path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ macos, windows, linux, linux-cross, musllinux, musllinux-cross ]
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: wheels
-      - uses: actions/setup-python@v4
+          pattern: wheels-*
+          merge-multiple: true
+      - uses: actions/setup-python@v5
         with:
-          python-version: 3.9
+          python-version: 3.12
       - name: Publish to PyPI
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
         run: |
           pip install --upgrade twine
           twine upload --skip-existing *
```

### Comparing `rjsonnet-0.5.3/.gitignore` & `rjsonnet-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rjsonnet-0.5.3/LICENSE` & `rjsonnet-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rjsonnet-0.5.3/README.md` & `rjsonnet-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `rjsonnet-0.5.3/rjsonnet.pyi` & `rjsonnet-0.5.4/rjsonnet.pyi`

 * *Files identical despite different names*

### Comparing `rjsonnet-0.5.3/src/lib.rs` & `rjsonnet-0.5.4/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -54,29 +54,31 @@
             });
             return Err(Error::new(ImportCallbackError(format!(
                 "import_callback error: {}",
                 err_msg
             ))));
         };
         let (resolved, content) =
-            Python::with_gil(|py| match self.callback.call(py, (base, path), None) {
-                Ok(obj) => obj.extract::<(String, Option<String>)>(py).map_err(|err| {
-                    let err_msg = err.to_string();
-                    err.restore(py);
-                    ImportCallbackError(format!("import_callback error: {}", err_msg))
-                }),
-                Err(err) => {
-                    let err_msg = err.to_string();
-                    err.restore(py);
-                    Err(ImportCallbackError(format!(
-                        "import_callback error: {}",
-                        err_msg
-                    )))
-                }
-            })?;
+            Python::with_gil(
+                |py| match self.callback.call_bound(py, (base, path), None) {
+                    Ok(obj) => obj.extract::<(String, Option<String>)>(py).map_err(|err| {
+                        let err_msg = err.to_string();
+                        err.restore(py);
+                        ImportCallbackError(format!("import_callback error: {}", err_msg))
+                    }),
+                    Err(err) => {
+                        let err_msg = err.to_string();
+                        err.restore(py);
+                        Err(ImportCallbackError(format!(
+                            "import_callback error: {}",
+                            err_msg
+                        )))
+                    }
+                },
+            )?;
         if let Some(content) = content {
             let resolved = SourcePath::new(SourceFile::new(PathBuf::from(resolved)));
             let mut out = self.out.borrow_mut();
             if !out.contains_key(&resolved) {
                 out.insert(resolved.clone(), content.into());
             }
             Ok(resolved)
@@ -94,33 +96,35 @@
 
     fn as_any(&self) -> &dyn Any {
         self
     }
 }
 
 fn pyobject_to_val(py: Python, obj: PyObject) -> PyResult<Val> {
-    return if let Ok(s) = obj.downcast::<PyString>(py) {
-        s.to_str().map(|s| Val::Str(StrValue::Flat(s.into())))
-    } else if let Ok(b) = obj.downcast::<PyBool>(py) {
+    return if let Ok(s) = obj.downcast_bound::<PyString>(py) {
+        s.as_gil_ref()
+            .to_str()
+            .map(|s| Val::Str(StrValue::Flat(s.into())))
+    } else if let Ok(b) = obj.downcast_bound::<PyBool>(py) {
         Ok(Val::Bool(b.is_true()))
-    } else if let Ok(f) = obj.downcast::<PyFloat>(py) {
+    } else if let Ok(f) = obj.downcast_bound::<PyFloat>(py) {
         Ok(Val::Num(f.value() as _))
     } else if let Ok(l) = obj.extract::<u64>(py) {
         Ok(Val::Num(l as _))
     } else if obj.is_none(py) {
         Ok(Val::Null)
-    } else if let Ok(seq) = obj.downcast::<PySequence>(py) {
+    } else if let Ok(seq) = obj.downcast_bound::<PySequence>(py) {
         let len = seq.len()?;
         let mut arr = Vec::with_capacity(len);
         for i in 0..len {
             let item = seq.get_item(i)?;
             arr.push(pyobject_to_val(py, item.into_py(py))?);
         }
         Ok(Val::Arr(ArrValue::eager(arr)))
-    } else if let Ok(d) = obj.downcast::<PyDict>(py) {
+    } else if let Ok(d) = obj.downcast_bound::<PyDict>(py) {
         let mut map = ObjValue::new_empty();
         for (k, v) in d {
             let k = k.extract::<String>()?;
             let v = pyobject_to_val(py, v.into_py(py))?;
             map.extend_field(k.into()).value(v);
         }
         Ok(Val::Obj(map))
@@ -134,23 +138,23 @@
 fn val_to_pyobject(py: Python, val: &Val, preserve_order: bool) -> PyObject {
     match val {
         Val::Bool(b) => b.into_py(py),
         Val::Null => py.None(),
         Val::Str(s) => s.clone().into_flat().into_py(py),
         Val::Num(n) => n.into_py(py),
         Val::Arr(a) => {
-            let arr = PyList::empty(py);
+            let arr = PyList::empty_bound(py);
             for item in a.iter() {
                 arr.append(val_to_pyobject(py, &item.unwrap(), preserve_order))
                     .unwrap();
             }
             arr.into_py(py)
         }
         Val::Obj(o) => {
-            let dict = PyDict::new(py);
+            let dict = PyDict::new_bound(py);
             for field in o.fields(preserve_order) {
                 let k = field.to_string();
                 let v = o
                     .get(field)
                     .unwrap()
                     .map(|x| val_to_pyobject(py, &x, preserve_order));
                 dict.set_item(k, v).unwrap();
@@ -174,15 +178,15 @@
 impl NativeCallbackHandler for JsonnetNativeCallbackHandler {
     fn call(&self, args: &[Val]) -> Result<Val, Error> {
         Python::with_gil(|py| {
             let args: Vec<_> = args
                 .iter()
                 .map(|v| val_to_pyobject(py, v, self.preserve_order))
                 .collect();
-            let err = match self.func.call(py, PyTuple::new(py, args), None) {
+            let err = match self.func.call_bound(py, PyTuple::new_bound(py, args), None) {
                 Ok(obj) => match pyobject_to_val(py, obj) {
                     Ok(val) => return Ok(val),
                     Err(err) => err,
                 },
                 Err(err) => err,
             };
             let err_msg = err.to_string();
@@ -256,29 +260,29 @@
                 },
             )
             .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
             tla_args.insert(name, TlaArg::Code(code));
         }
 
         if let Some(import_callback) = import_callback {
-            if !import_callback.as_ref(py).is_callable() {
+            if !import_callback.bind(py).is_callable() {
                 return Err(PyTypeError::new_err("import_callback must be callable"));
             }
             let import_resolver = PythonImportResolver {
                 callback: import_callback,
                 out: RefCell::new(HashMap::new()),
             };
             state.set_import_resolver(import_resolver);
         } else if let Some(jpathdir) = jpathdir {
             let import_resolver = FileImportResolver::new(jpathdir);
             state.set_import_resolver(import_resolver);
         }
 
         for (name, (args, func)) in native_callbacks.into_iter() {
-            let args = args.downcast::<PyTuple>(py)?;
+            let args = args.downcast_bound::<PyTuple>(py)?;
             let mut params = Vec::with_capacity(args.len());
             for arg in args {
                 let param = arg.extract::<String>()?;
                 params.push(param);
             }
             context_initializer.add_native(
                 name.clone(),
@@ -290,18 +294,20 @@
                         func,
                         preserve_order,
                     },
                 ),
             );
         }
 
+        let manifest_format = JsonFormat::cli(4, preserve_order);
+
         state.settings_mut().context_initializer = tb!(context_initializer);
         Ok(Self {
             state,
-            manifest_format: Box::new(JsonFormat::default()),
+            manifest_format: Box::new(manifest_format),
             trace_format: Box::new(trace_format),
             tla_args,
         })
     }
 
     fn evaluate_file(&self, filename: &str) -> Result<String, Error> {
         self.state
@@ -454,13 +460,13 @@
         .evaluate_snippet(filename, src)
         .map_err(|e| vm.error_to_pyerr(py, &e))?;
     Ok(result)
 }
 
 /// Python bindings to Rust jrsonnet crate
 #[pymodule]
-fn rjsonnet(_py: Python, m: &PyModule) -> PyResult<()> {
+fn rjsonnet(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     m.add_function(wrap_pyfunction!(evaluate_file, m)?)?;
     m.add_function(wrap_pyfunction!(evaluate_snippet, m)?)?;
     Ok(())
 }
```

### Comparing `rjsonnet-0.5.3/tests/test_rjsonnet.py` & `rjsonnet-0.5.4/tests/test_rjsonnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 
 import pytest
 import rjsonnet
 
 
 def import_callback(dir, rel):
@@ -102,7 +103,14 @@
 
     with pytest.raises(RuntimeError):
         rjsonnet.evaluate_file(
             "test.jsonnet",
             import_callback=import_callback_2,
             native_callbacks=native_callbacks,
         )
+
+def test_preserve_order():
+    code = "{c: 1, a: 2, b: 3}"
+    json_str = rjsonnet.evaluate_snippet("test", code, preserve_order=True)
+    # as of python 3.6 dicts are ordered, and the json 
+    obj = json.loads(json_str)
+    assert list(obj) == ['c', 'a', 'b']
```

### Comparing `rjsonnet-0.5.3/Cargo.lock` & `rjsonnet-0.5.4/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.8.3"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "once_cell",
  "version_check",
+ "zerocopy",
 ]
 
 [[package]]
 name = "annotate-snippets"
-version = "0.9.1"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3b9d411ecbaf79885c6df4d75fff75858d5995ff25385657a28af47e82f9c36"
+checksum = "ccaf7e9dfbb6ab22c82e473cd1a8a7bd313c19a5b7e40970f3d89ef5a5c9e81e"
 dependencies = [
  "unicode-width",
  "yansi-term",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
-version = "0.21.3"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "414dcefbc63d77c526a76b3afcf6fbb9b5e2791c19c3aa2297733208750c6e53"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -54,17 +55,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -118,34 +119,40 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jrsonnet-evaluator"
 version = "0.5.0-pre95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0951f206ee982ef3c61ed49c2779b3649858d2b7c6748943e4c7f36f6df55f9c"
 dependencies = [
@@ -251,79 +258,79 @@
 dependencies = [
  "jrsonnet-gcmodule",
  "peg",
 ]
 
 [[package]]
 name = "keccak"
-version = "0.1.4"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
+checksum = "ecc2af9a1119c51f12a14607e783cb977bde58bc069ff0c3da1095e635d70654"
 dependencies = [
  "cpufeatures",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.147"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "md5"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "490cc448043f947bae3cbee9c203358d62dbee0db12107a74be5c30ccfd09771"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -332,129 +339,138 @@
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "peg"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a07f2cafdc3babeebc087e499118343442b742cc7c31b4d054682cc598508554"
+checksum = "400bcab7d219c38abf8bd7cc2054eb9bbbd4312d66f6a5557d572a203f646f61"
 dependencies = [
  "peg-macros",
  "peg-runtime",
 ]
 
 [[package]]
 name = "peg-macros"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a90084dc05cf0428428e3d12399f39faad19b0909f64fb9170c9fdd6d9cd49b"
+checksum = "46e61cce859b76d19090f62da50a9fe92bab7c2a5f09e183763559a2ac392c90"
 dependencies = [
  "peg-runtime",
  "proc-macro2",
  "quote",
 ]
 
 [[package]]
 name = "peg-runtime"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fa00462b37ead6d11a82c9d568b26682d78e0477dc02d1966c013af80969739"
+checksum = "36bae92c60fa2398ce4678b98b2c4b5a7c61099961ca1fa305aec04a9ad28922"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.66"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rjsonnet"
-version = "0.5.3"
+version = "0.5.4"
 dependencies = [
  "jrsonnet-evaluator",
  "jrsonnet-gcmodule",
  "jrsonnet-parser",
  "jrsonnet-stdlib",
  "pyo3",
 ]
@@ -463,49 +479,49 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.29",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.105"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "693151e1ac27563d6dbcec9dee9fbd5da8539b20fa14ad3752b2e6d363ace360"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -518,28 +534,28 @@
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
 name = "sha1"
-version = "0.10.5"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
+checksum = "e3bf829a2d51ab4a5ddf1352d8470c140cadc8301b2ae1789db023f01cedd6ba"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.7"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+checksum = "793db75ad2bcafc3ffa7c68b215fee268f537982cd901d132f89c6343f3a3dc8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -550,17 +566,17 @@
 dependencies = [
  "digest",
  "keccak",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
@@ -601,72 +617,72 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.29"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c324c494eba9d92503e6f1ef2e6df781e78f6a7705a0202d9801b198807d518a"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.47"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97a802ec30afc17eee47b2855fc72e0c4cd62be9b4efe6591edde0ec5bd68d8f"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.47"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bb623b56e39ab7dcd4b1b98bb6c8f8d907ed255b18de254088016b27a8ee19b"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.29",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "typenum"
-version = "1.16.0"
+version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -762,7 +778,27 @@
 name = "yansi-term"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe5c30ade05e61656247b2e334a031dfd0cc466fadef865bdcdea8d537951bf1"
 dependencies = [
  "winapi",
 ]
+
+[[package]]
+name = "zerocopy"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
```

### Comparing `rjsonnet-0.5.3/PKG-INFO` & `rjsonnet-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rjsonnet
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python bindings to Rust jrsonnet crate
 Home-Page: https://github.com/messense/rjsonnet-py
 Author: messense <messense@icloud.com>
 Author-email: messense <messense@icloud.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/messense/rjsonnet-py.git
```

