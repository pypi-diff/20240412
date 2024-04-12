# Comparing `tmp/rlbot_flatbuffers-0.3.1.tar.gz` & `tmp/rlbot_flatbuffers-0.3.2.tar.gz`

## Comparing `rlbot_flatbuffers-0.3.1.tar` & `rlbot_flatbuffers-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.1/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/LICENSE
--rw-r--r--   0     1001      127      479 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/README.md
--rw-r--r--   0     1001      127    60169 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/build.rs
--rw-r--r--   0     1001      127      182 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/README.md
--rw-r--r--   0     1001      127      401 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/comms.fbs
--rw-r--r--   0     1001      127     1932 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/event.fbs
--rwxr-xr-x   0     1001      127  6681832 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc
--rw-r--r--   0     1001      127  3488256 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc.exe
--rw-r--r--   0     1001      127  6896752 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc_mac
--rw-r--r--   0     1001      127     1281 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/gamestate.fbs
--rw-r--r--   0     1001      127     5824 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/matchstart.fbs
--rw-r--r--   0     1001      127     1162 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/rendering.fbs
--rw-r--r--   0     1001      127     6296 2024-04-03 02:47:52.000000 rlbot_flatbuffers-0.3.1/flatbuffers-schema/rlbot.fbs
--rw-r--r--   0     1001      127     4770 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/src/lib.rs
--rw-r--r--   0     1001      127    12644 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/Cargo.lock
--rw-r--r--   0     1001      127      418 2024-04-03 02:47:51.000000 rlbot_flatbuffers-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/LICENSE
+-rw-r--r--   0     1001      127      479 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/README.md
+-rw-r--r--   0     1001      127    60199 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/build.rs
+-rw-r--r--   0     1001      127      182 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/README.md
+-rw-r--r--   0     1001      127      401 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/comms.fbs
+-rw-r--r--   0     1001      127     1932 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/event.fbs
+-rwxr-xr-x   0     1001      127  6681832 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc
+-rw-r--r--   0     1001      127  3488256 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc.exe
+-rw-r--r--   0     1001      127  6896752 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc_mac
+-rw-r--r--   0     1001      127     1281 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/gamestate.fbs
+-rw-r--r--   0     1001      127     5824 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/matchstart.fbs
+-rw-r--r--   0     1001      127     1162 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/rendering.fbs
+-rw-r--r--   0     1001      127     6296 2024-04-12 01:00:42.000000 rlbot_flatbuffers-0.3.2/flatbuffers-schema/rlbot.fbs
+-rw-r--r--   0     1001      127     4770 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      127    12644 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/Cargo.lock
+-rw-r--r--   0     1001      127      418 2024-04-12 01:00:41.000000 rlbot_flatbuffers-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 rlbot_flatbuffers-0.3.2/PKG-INFO
```

### Comparing `rlbot_flatbuffers-0.3.1/Cargo.toml` & `rlbot_flatbuffers-0.3.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlbot-flatbuffers-py"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 description = "A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers"
 repository = "https://github.com/VirxEC/rlbot-flatbuffers-py"
 license = "MIT"
 readme = "README.md"
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore", ".gitmodules"]
 publish = false
```

### Comparing `rlbot_flatbuffers-0.3.1/LICENSE` & `rlbot_flatbuffers-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/build.rs` & `rlbot_flatbuffers-0.3.2/build.rs`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     }
 
     fn write_string(&mut self, s: String) {
         self.file_contents.push(Cow::Owned(s));
     }
 
     fn generate_struct_definition(&mut self) {
-        self.write_str("#[pyclass(module = \"rlbot_flatbuffers\", get_all, set_all)]");
+        self.write_str("#[pyclass(module = \"rlbot_flatbuffers\", subclass, get_all, set_all)]");
 
         if self.types.is_empty() {
             self.write_str("#[derive(Debug, Default, Clone)]");
             self.write_string(format!("pub struct {} {{}}", self.struct_name));
             self.write_str("");
             return;
         }
@@ -1092,15 +1092,15 @@
         if self.bind_type == PythonBindType::Enum {
             self.write_string(format!("        let flat_t = flat::{name}::from(self);"));
         } else {
             self.write_string(format!("        let flat_t = flat::{name}::from_gil(py, self);"));
         }
 
         if self.has_complex_pack {
-            self.write_str("        let size = flat_t.get_size();");
+            self.write_str("        let size = flat_t.get_size().next_power_of_two();");
             self.write_str("");
             self.write_str("        let mut builder = FlatBufferBuilder::with_capacity(size);");
             self.write_str("        let offset = flat_t.pack(&mut builder);");
             self.write_str("        builder.finish(offset, None);");
             self.write_str("");
             self.write_str("        PyBytes::new_bound(py, builder.finished_data())");
         } else if self.bind_type == PythonBindType::Enum {
```

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/event.fbs` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/event.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc.exe` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc.exe`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/flatc_mac` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/flatc_mac`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/gamestate.fbs` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/gamestate.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/matchstart.fbs` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/matchstart.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/rendering.fbs` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/rendering.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/flatbuffers-schema/rlbot.fbs` & `rlbot_flatbuffers-0.3.2/flatbuffers-schema/rlbot.fbs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/src/lib.rs` & `rlbot_flatbuffers-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rlbot_flatbuffers-0.3.1/Cargo.lock` & `rlbot_flatbuffers-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlbot-flatbuffers-py"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "flatbuffers",
  "get-size",
  "pyo3",
  "serde",
 ]
```

### Comparing `rlbot_flatbuffers-0.3.1/PKG-INFO` & `rlbot_flatbuffers-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlbot_flatbuffers
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: A Python module implemented in Rust for serializing and deserializing RLBot's flatbuffers
 License: MIT
 Requires-Python: >=3.10
```

