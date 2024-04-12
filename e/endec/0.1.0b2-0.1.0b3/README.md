# Comparing `tmp/endec-0.1.0b2.tar.gz` & `tmp/endec-0.1.0b3.tar.gz`

## Comparing `endec-0.1.0b2.tar` & `endec-0.1.0b3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 endec-0.1.0b2/Cargo.toml
--rw-r--r--   0     1001      127     4333 2024-04-10 05:18:56.000000 endec-0.1.0b2/.github/workflows/build.yml
--rw-r--r--   0     1001      127      994 2024-04-10 05:18:56.000000 endec-0.1.0b2/.github/workflows/test.yml
--rw-r--r--   0     1001      127      685 2024-04-10 05:18:56.000000 endec-0.1.0b2/.gitignore
--rw-r--r--   0     1001      127     1064 2024-04-10 05:18:56.000000 endec-0.1.0b2/LICENSE
--rw-r--r--   0     1001      127     2356 2024-04-10 05:18:56.000000 endec-0.1.0b2/README.md
--rw-r--r--   0     1001      127      515 2024-04-10 05:18:56.000000 endec-0.1.0b2/endec.pyi
--rw-r--r--   0     1001      127       90 2024-04-10 05:18:56.000000 endec-0.1.0b2/python/endec/__init__.py
--rw-r--r--   0     1001      127     1075 2024-04-10 05:18:56.000000 endec-0.1.0b2/python/endec/exceptions.py
--rw-r--r--   0     1001      127      650 2024-04-10 05:18:56.000000 endec-0.1.0b2/renovate.json
--rw-r--r--   0     1001      127     4250 2024-04-10 05:18:56.000000 endec-0.1.0b2/src/lib.rs
--rw-r--r--   0     1001      127     4526 2024-04-10 05:18:56.000000 endec-0.1.0b2/tests/test_decode.py
--rw-r--r--   0     1001      127     1089 2024-04-10 05:18:56.000000 endec-0.1.0b2/tests/test_encode.py
--rw-r--r--   0     1001      127      294 2024-04-10 05:18:56.000000 endec-0.1.0b2/tests/test_iso2022jp.py
--rw-r--r--   0     1001      127      193 2024-04-10 05:18:56.000000 endec-0.1.0b2/tox.ini
--rw-r--r--   0     1001      127     8098 2024-04-10 05:18:56.000000 endec-0.1.0b2/Cargo.lock
--rw-r--r--   0     1001      127     1174 2024-04-10 05:18:56.000000 endec-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 endec-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      164 1970-01-01 00:00:00.000000 endec-0.1.0b3/Cargo.toml
+-rw-r--r--   0     1001      127     4333 2024-04-11 03:25:16.000000 endec-0.1.0b3/.github/workflows/build.yml
+-rw-r--r--   0     1001      127      994 2024-04-11 03:25:16.000000 endec-0.1.0b3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      685 2024-04-11 03:25:16.000000 endec-0.1.0b3/.gitignore
+-rw-r--r--   0     1001      127     1064 2024-04-11 03:25:16.000000 endec-0.1.0b3/LICENSE
+-rw-r--r--   0     1001      127     2356 2024-04-11 03:25:16.000000 endec-0.1.0b3/README.md
+-rw-r--r--   0     1001      127       92 2024-04-11 03:25:16.000000 endec-0.1.0b3/python/endec/__init__.py
+-rw-r--r--   0     1001      127      515 2024-04-11 03:25:16.000000 endec-0.1.0b3/python/endec/endec.pyi
+-rw-r--r--   0     1001      127     1060 2024-04-11 03:25:16.000000 endec-0.1.0b3/python/endec/exceptions.py
+-rw-r--r--   0     1001      127        0 2024-04-11 03:25:16.000000 endec-0.1.0b3/python/endec/py.typed
+-rw-r--r--   0     1001      127      745 2024-04-11 03:25:16.000000 endec-0.1.0b3/renovate.json
+-rw-r--r--   0     1001      127       86 2024-04-11 03:25:16.000000 endec-0.1.0b3/rust-toolchain.toml
+-rw-r--r--   0     1001      127     3004 2024-04-11 03:25:16.000000 endec-0.1.0b3/src/decode.rs
+-rw-r--r--   0     1001      127      967 2024-04-11 03:25:16.000000 endec-0.1.0b3/src/encode.rs
+-rw-r--r--   0     1001      127      433 2024-04-11 03:25:16.000000 endec-0.1.0b3/src/lib.rs
+-rw-r--r--   0     1001      127      301 2024-04-11 03:25:16.000000 endec-0.1.0b3/src/utils.rs
+-rw-r--r--   0     1001      127     4763 2024-04-11 03:25:16.000000 endec-0.1.0b3/tests/test_decode.py
+-rw-r--r--   0     1001      127     1089 2024-04-11 03:25:16.000000 endec-0.1.0b3/tests/test_encode.py
+-rw-r--r--   0     1001      127      294 2024-04-11 03:25:16.000000 endec-0.1.0b3/tests/test_iso2022jp.py
+-rw-r--r--   0     1001      127      193 2024-04-11 03:25:16.000000 endec-0.1.0b3/tox.ini
+-rw-r--r--   0     1001      127     8098 2024-04-11 03:25:16.000000 endec-0.1.0b3/Cargo.lock
+-rw-r--r--   0     1001      127     1203 2024-04-11 03:25:16.000000 endec-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 endec-0.1.0b3/PKG-INFO
```

### Comparing `endec-0.1.0b2/.github/workflows/build.yml` & `endec-0.1.0b3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/.github/workflows/test.yml` & `endec-0.1.0b3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/.gitignore` & `endec-0.1.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/LICENSE` & `endec-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/README.md` & `endec-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/endec.pyi` & `endec-0.1.0b3/python/endec/endec.pyi`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/python/endec/exceptions.py` & `endec-0.1.0b3/python/endec/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import TYPE_CHECKING, Optional
+    from typing import Optional
 
 
 class DecodeError(UnicodeError):
     encoding: str
     target: bytes
     reason: "Optional[str]"
```

### Comparing `endec-0.1.0b2/src/lib.rs` & `endec-0.1.0b3/src/decode.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,55 @@
 use std::borrow::Cow;
 
-use encoding_rs::{UTF_16BE, UTF_16LE, UTF_8};
-use pyo3::{
-    exceptions::PyLookupError,
-    prelude::*,
-    types::{PyBytes, PyString},
-};
-
-mod exceptions {
-    pyo3::import_exception!(endec.exceptions, EncodeError);
-    pyo3::import_exception!(endec.exceptions, DecodeError);
-}
-
-fn get_codec(name: &str) -> PyResult<&'static encoding_rs::Encoding> {
-    encoding_rs::Encoding::for_label(name.as_bytes()).ok_or(PyLookupError::new_err(format!(
-        "unknown encoding: {}",
-        name
-    )))
-}
+use encoding_rs::{UTF_16BE, UTF_16LE};
+use pyo3::exceptions::PyLookupError;
+use pyo3::prelude::*;
+use pyo3::types::PyString;
 
-#[pyfunction]
-#[pyo3(signature = (input_str, /, encoding = "utf-8", errors = "strict"))]
-fn encode(py: Python, input_str: &str, encoding: &str, errors: &str) -> PyResult<PyObject> {
-    let (out, used_encoding, has_unmappable) = get_codec(encoding)?.encode(input_str);
-    let convert_to_pybytes = || PyBytes::new(py, &out).into();
-
-    if !has_unmappable {
-        return Ok(convert_to_pybytes());
-    }
-
-    match errors {
-        "strict" => Err(exceptions::EncodeError::new_err((
-            used_encoding.name().to_owned(),
-            input_str.to_owned(),
-        ))),
-        "xmlcharrefreplace" => Ok(convert_to_pybytes()),
-        _ => Err(PyLookupError::new_err(format!(
-            "unknown error handler name '{}'",
-            errors
-        ))),
-    }
-}
+use crate::exceptions::DecodeError;
+use crate::utils::get_encoding_by_name;
 
 #[pyfunction]
 #[pyo3(signature = (input_bytes, /, encoding = "utf-8", errors = "strict", *, bom = "evaluate"))]
-fn decode<'py>(
+pub(crate) fn decode<'py>(
     py: Python<'py>,
     input_bytes: &'py [u8],
     encoding: &'py str,
     errors: &'py str,
     bom: &'py str,
-) -> PyResult<&'py PyString> {
-    let codec = get_codec(encoding)?;
+) -> PyResult<Bound<'py, PyString>> {
+    let codec = get_encoding_by_name(encoding)?;
 
     let mut evaluated_encoding = codec.name();
 
     let mut decode = || -> PyResult<(Cow<'py, str>, bool)> {
         match bom {
             "evaluate" => {
-                let (out, used_encoding, has_replaced) =
-                    if codec == UTF_8 || codec == UTF_16BE || codec == UTF_16LE {
-                        codec.decode(input_bytes)
-                    } else {
-                        let (out, has_replaced) = codec.decode_with_bom_removal(input_bytes);
-                        (out, codec, has_replaced)
-                    };
+                // only allow morphing for utf-16 in default evaluate mode
+                let (out, used_encoding, has_replaced) = if codec == UTF_16BE || codec == UTF_16LE {
+                    codec.decode(input_bytes)
+                } else {
+                    let (out, has_replaced) = codec.decode_with_bom_removal(input_bytes);
+                    (out, codec, has_replaced)
+                };
 
                 evaluated_encoding = used_encoding.name();
                 Ok((out, has_replaced))
             }
             "evaluateall" => {
                 let (out, used_encoding, has_replaced) = codec.decode(input_bytes);
                 evaluated_encoding = used_encoding.name();
                 Ok((out, has_replaced))
             }
             "strip" => Ok(codec.decode_with_bom_removal(input_bytes)),
             "ignore" => {
                 if errors == "strict" {
                     let out = codec
                         .decode_without_bom_handling_and_without_replacement(input_bytes)
-                        .ok_or(exceptions::DecodeError::new_err((
+                        .ok_or(DecodeError::new_err((
                             evaluated_encoding.to_owned(),
                             input_bytes.to_vec(),
                         )))?;
 
                     Ok((out, false))
                 } else {
                     // replace
@@ -100,15 +66,15 @@
     let out = match errors {
         "strict" => {
             let (out, has_replaced) = decode()?;
 
             if has_replaced {
                 // has replaced characters but strict mode was used
                 // TODO add reason in exception
-                return Err(exceptions::DecodeError::new_err((
+                return Err(DecodeError::new_err((
                     evaluated_encoding.to_owned(),
                     input_bytes.to_owned(),
                 )));
             }
 
             out
         }
@@ -117,16 +83,9 @@
             return Err(PyLookupError::new_err(format!(
                 "unknown error handler name '{}'",
                 errors
             )))
         }
     };
 
-    Ok(PyString::new(py, out.as_ref()))
-}
-
-#[pymodule]
-fn endec(_py: Python, module: &PyModule) -> PyResult<()> {
-    module.add_function(wrap_pyfunction!(encode, module)?)?;
-    module.add_function(wrap_pyfunction!(decode, module)?)?;
-    Ok(())
+    Ok(PyString::new_bound(py, out.as_ref()))
 }
```

### Comparing `endec-0.1.0b2/tests/test_decode.py` & `endec-0.1.0b3/tests/test_decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,31 @@
     assert endec.decode(b"\xff\xfetest", "utf-16", bom="evaluate") == "整瑳"
     assert endec.decode(b"\xfe\xfftest", "utf-16", bom="evaluate") == "瑥獴"
     assert endec.decode(b"\xff\xfeetts", "utf-16", bom="evaluate") == "瑥獴"
     assert endec.decode(b"\xef\xbb\xbftest", "utf-8", bom="evaluate") == "test"
 
 
 def test_decode_bom_evaluate_morph():
-    # evaluate should not morph other codecs other than utf-8, utf-16be, utf-16le
+    # evaluate should not morph other codecs other than utf-16be, utf-16le
+
+    # bom should default to evaluate
     assert endec.decode(b"\xff\xfetest", "latin1") == "ÿþtest"
+
+    with pytest.raises(DecodeError):
+        endec.decode(b"\xfe\xfftest", "utf-8")
+
+    # explicit bom kwargs
     assert endec.decode(b"\xff\xfetest", "latin1", bom="evaluate") == "ÿþtest"
 
+    with pytest.raises(DecodeError):
+        endec.decode(b"\xfe\xfftest", "utf-8", bom="evaluate")
+
 
 def test_decode_bom_evaluateall():
-    # evaluateall should morph other codecs other than utf-8, utf-16be, utf-16le
+    # evaluateall should morph other codecs other than utf-16be, utf-16le
 
     # morph to utf-16le
     assert endec.decode(b"\xff\xfetest", "latin1", bom="evaluateall") == "整瑳"
 
     # morph to utf-16be
     assert endec.decode(b"\xfe\xfftest", "latin1", bom="evaluateall") == "瑥獴"
```

### Comparing `endec-0.1.0b2/tests/test_encode.py` & `endec-0.1.0b3/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `endec-0.1.0b2/Cargo.lock` & `endec-0.1.0b3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "endec"
 version = "0.1.0"
```

### Comparing `endec-0.1.0b2/pyproject.toml` & `endec-0.1.0b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.2,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "endec"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Web-compatible encoding and decoding library"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Thitat Auareesuksakul", email = "flux@thitat.net" }]
 keywords = ["encoding_rs", "web", "codec"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -24,16 +24,17 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Utilities",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
-repository = "https://github.com/fluxth/endec"
+Repository = "https://github.com/fluxth/endec"
 
 [tool.maturin]
+module-name = "endec._endec"
 python-source = "python"
 features = ["pyo3/extension-module"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
```

### Comparing `endec-0.1.0b2/PKG-INFO` & `endec-0.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: endec
-Version: 0.1.0b2
+Version: 0.1.0b3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 Classifier: Topic :: Utilities
 License-File: LICENSE
 Summary: Web-compatible encoding and decoding library
 Keywords: encoding_rs,web,codec
 Author-email: Thitat Auareesuksakul <flux@thitat.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/fluxth/endec
+Project-URL: Repository, https://github.com/fluxth/endec
 
 # endec
 
 [![PyPI - Version](https://img.shields.io/pypi/v/endec)](https://pypi.org/project/endec/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/endec)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/fluxth/endec/build.yml)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/fluxth/endec/test.yml?label=tests)
```

