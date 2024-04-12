# Comparing `tmp/servicing-0.0.1.tar.gz` & `tmp/servicing-0.0.2.tar.gz`

## Comparing `servicing-0.0.1.tar` & `servicing-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.1/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-04-10 20:43:32.000000 servicing-0.0.1/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-04-10 20:43:32.000000 servicing-0.0.1/.gitignore
--rw-r--r--   0     1001      127      165 2024-04-10 20:43:32.000000 servicing-0.0.1/.vimspector.json
--rw-r--r--   0     1001      127      755 2024-04-10 20:43:32.000000 servicing-0.0.1/README.md
--rw-r--r--   0     1001      127      271 2024-04-10 20:43:32.000000 servicing-0.0.1/build.rs
--rw-r--r--   0     1001      127    10988 2024-04-10 20:43:32.000000 servicing-0.0.1/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-04-10 20:43:32.000000 servicing-0.0.1/src/error/mod.rs
--rw-r--r--   0     1001      127     5533 2024-04-10 20:43:32.000000 servicing-0.0.1/src/helper/mod.rs
--rw-r--r--   0     1001      127      355 2024-04-10 20:43:32.000000 servicing-0.0.1/src/lib.rs
--rw-r--r--   0     1001      127     2382 2024-04-10 20:43:32.000000 servicing-0.0.1/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-04-10 20:43:32.000000 servicing-0.0.1/template/service.yaml
--rw-r--r--   0     1001      127    41593 2024-04-10 20:43:32.000000 servicing-0.0.1/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-10 20:43:32.000000 servicing-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 servicing-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-04-12 02:37:11.000000 servicing-0.0.2/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-04-12 02:37:11.000000 servicing-0.0.2/.gitignore
+-rw-r--r--   0     1001      127      165 2024-04-12 02:37:11.000000 servicing-0.0.2/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-04-12 02:37:11.000000 servicing-0.0.2/README.md
+-rw-r--r--   0     1001      127      271 2024-04-12 02:37:11.000000 servicing-0.0.2/build.rs
+-rw-r--r--   0     1001      127     2448 2024-04-12 02:37:11.000000 servicing-0.0.2/servicing.pyi
+-rw-r--r--   0     1001      127    12103 2024-04-12 02:37:11.000000 servicing-0.0.2/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-04-12 02:37:11.000000 servicing-0.0.2/src/error/mod.rs
+-rw-r--r--   0     1001      127     5533 2024-04-12 02:37:11.000000 servicing-0.0.2/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-04-12 02:37:11.000000 servicing-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      127     2596 2024-04-12 02:37:11.000000 servicing-0.0.2/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-04-12 02:37:11.000000 servicing-0.0.2/template/service.yaml
+-rw-r--r--   0     1001      127    41593 2024-04-12 02:37:11.000000 servicing-0.0.2/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-04-12 02:37:11.000000 servicing-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.2/PKG-INFO
```

### Comparing `servicing-0.0.1/Cargo.toml` & `servicing-0.0.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.1"
+version = "0.0.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
```

### Comparing `servicing-0.0.1/.github/workflows/cicd.yml` & `servicing-0.0.2/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.1/.gitignore` & `servicing-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.1/README.md` & `servicing-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-<img src="https://github.com/acceleratedscience/stressor/assets/14236737/3b48d7f4-4605-406d-95b3-062e9e694b2c" width="100"></br>
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
 
-###### How to run this locally...
+###### How to run this locally from source
  1. Clone this repository:
 
  ```bash
  git clone git@github.com:acceleratedscience/servicing.git
  ```
  2. Install Rust toolchain:
  ```bash
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  ```
  3. Download Maturin (Python bindings for Rust)
  ```bash
  cargo install maturin
  ```
- 4. Build the project:
+ 4. Create Python virtual environment:
  ```bash
- maturin develop
+ virtualenv .venv
  ```
- 5. Create Python virtual environment:
+ 5. Build the project:
  ```bash
- virtualenv .venv
+ maturin develop
  ```
  6. Activate the virtual environment:
  ```bash
  source .venv/bin/activate
  ```
+ 7. Use Servicing
+ ```bash
+ python
+ import servicing
+ ```
```

### Comparing `servicing-0.0.1/src/dispatcher/mod.rs` & `servicing-0.0.2/src/dispatcher/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -327,10 +327,45 @@
         }
         Err(ServicingError::ServiceNotFound(name))
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use crate::models::UserProvidedConfig;
+
     #[test]
-    fn test_fetch() {}
+    fn test_dispatcher() {
+        let mut dis = super::Dispatcher::new().unwrap();
+
+        dis.add_service(
+            "testing".to_string(),
+            Some(UserProvidedConfig {
+                port: 1234,
+                replicas: 5,
+                cloud: "aws".to_string(),
+            }),
+        )
+        .unwrap();
+
+        dis.save().unwrap();
+
+        // check what has been added
+        {
+            let services = dis.service.lock().unwrap();
+            let service = services.get("testing").unwrap();
+            assert_eq!(service.template.resources.ports, 1234);
+            assert_eq!(service.template.service.replicas, 5);
+            assert_eq!(service.template.resources.cloud, "aws");
+        }
+
+        dis.remove_service("testing".to_string()).unwrap();
+        assert!(dis.service.lock().unwrap().get("testing").is_none());
+
+        dis.load(None).unwrap();
+        {
+            let services = dis.service.lock().unwrap();
+            let service = services.get("testing").unwrap();
+            assert_eq!(service.template.resources.ports, 1234);
+        }
+    }
 }
```

### Comparing `servicing-0.0.1/src/error/mod.rs` & `servicing-0.0.2/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.1/src/helper/mod.rs` & `servicing-0.0.2/src/helper/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.1/src/models/mod.rs` & `servicing-0.0.2/src/models/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-use pyo3::pyclass;
+use pyo3::{pyclass, pymethods};
 use serde::{Deserialize, Serialize};
 
 #[pyclass]
 #[derive(Clone, Serialize, Deserialize, Debug)]
 pub struct UserProvidedConfig {
-    pub name: String,
     pub port: u16,
     pub replicas: u16,
     pub cloud: String,
 }
 
+#[pymethods]
+impl UserProvidedConfig {
+    #[new]
+    pub fn new(port: u16, replicas: u16, cloud: String) -> Self {
+        UserProvidedConfig {
+            port,
+            replicas,
+            cloud,
+        }
+    }
+}
+
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Configuration {
     pub service: Service,
     pub resources: Resources,
     pub workdir: String,
     pub setup: String,
     pub run: String,
```

### Comparing `servicing-0.0.1/Cargo.lock` & `servicing-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "base64 0.22.0",
  "bincode",
  "dirs",
  "env_logger",
  "log",
  "pyo3",
```

### Comparing `servicing-0.0.1/PKG-INFO` & `servicing-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-<img src="https://github.com/acceleratedscience/stressor/assets/14236737/3b48d7f4-4605-406d-95b3-062e9e694b2c" width="100"></br>
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
 
-###### How to run this locally...
+###### How to run this locally from source
  1. Clone this repository:
 
  ```bash
  git clone git@github.com:acceleratedscience/servicing.git
  ```
  2. Install Rust toolchain:
  ```bash
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  ```
  3. Download Maturin (Python bindings for Rust)
  ```bash
  cargo install maturin
  ```
- 4. Build the project:
+ 4. Create Python virtual environment:
  ```bash
- maturin develop
+ virtualenv .venv
  ```
- 5. Create Python virtual environment:
+ 5. Build the project:
  ```bash
- virtualenv .venv
+ maturin develop
  ```
  6. Activate the virtual environment:
  ```bash
  source .venv/bin/activate
  ```
+ 7. Use Servicing
+ ```bash
+ python
+ import servicing
+ ```
```

