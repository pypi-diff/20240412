# Comparing `tmp/pepeline-0.2.6.tar.gz` & `tmp/pepeline-0.2.7.tar.gz`

## Comparing `pepeline-0.2.6.tar` & `pepeline-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 pepeline-0.2.6/Cargo.toml
--rw-r--r--   0     1001      127     2162 2024-04-11 09:17:26.000000 pepeline-0.2.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     2844 2024-04-11 09:17:26.000000 pepeline-0.2.6/.github/workflows/pipl.yml
--rw-r--r--   0     1001      127      686 2024-04-11 09:17:26.000000 pepeline-0.2.6/.gitignore
--rw-r--r--   0     1001      127     1065 2024-04-11 09:17:26.000000 pepeline-0.2.6/LICENSE
--rw-r--r--   0     1001      127      781 2024-04-11 09:17:26.000000 pepeline-0.2.6/README.md
--rw-r--r--   0     1001      127     1825 2024-04-11 09:17:26.000000 pepeline-0.2.6/pepeline.pyi
--rw-r--r--   0     1001      127      629 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/lib.rs
--rw-r--r--   0     1001      127      977 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/core/color_levels.rs
--rw-r--r--   0     1001      127     2195 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/core/convert.rs
--rw-r--r--   0     1001      127     1274 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/core/noise.rs
--rw-r--r--   0     1001      127     3295 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/functions/core_funcion.rs
--rw-r--r--   0     1001      127     2463 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/functions/img_function.rs
--rw-r--r--   0     1001      127      878 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/functions/screentone_function.rs
--rw-r--r--   0     1001      127    10382 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/image/decode.rs
--rw-r--r--   0     1001      127     1254 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/image/save.rs
--rw-r--r--   0     1001      127      341 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/mod.rs
--rw-r--r--   0     1001      127     1353 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/screentone/dot.rs
--rw-r--r--   0     1001      127      986 2024-04-11 09:17:26.000000 pepeline-0.2.6/src/utils/screentone/screentone_add.rs
--rw-r--r--   0     1001      127    33999 2024-04-11 09:17:31.000000 pepeline-0.2.6/Cargo.lock
--rw-r--r--   0     1001      127      428 2024-04-11 09:17:26.000000 pepeline-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 pepeline-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 pepeline-0.2.7/Cargo.toml
+-rw-r--r--   0     1001      127     2162 2024-04-12 07:51:08.000000 pepeline-0.2.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     2844 2024-04-12 07:51:08.000000 pepeline-0.2.7/.github/workflows/pipl.yml
+-rw-r--r--   0     1001      127      686 2024-04-12 07:51:08.000000 pepeline-0.2.7/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-04-12 07:51:08.000000 pepeline-0.2.7/LICENSE
+-rw-r--r--   0     1001      127      781 2024-04-12 07:51:08.000000 pepeline-0.2.7/README.md
+-rw-r--r--   0     1001      127     1825 2024-04-12 07:51:08.000000 pepeline-0.2.7/pepeline.pyi
+-rw-r--r--   0     1001      127      629 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/lib.rs
+-rw-r--r--   0     1001      127      977 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/core/color_levels.rs
+-rw-r--r--   0     1001      127     2195 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/core/convert.rs
+-rw-r--r--   0     1001      127     1274 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/core/noise.rs
+-rw-r--r--   0     1001      127     3295 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/functions/core_funcion.rs
+-rw-r--r--   0     1001      127     2463 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/functions/img_function.rs
+-rw-r--r--   0     1001      127      878 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/functions/screentone_function.rs
+-rw-r--r--   0     1001      127    10344 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/image/decode.rs
+-rw-r--r--   0     1001      127     1254 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/image/save.rs
+-rw-r--r--   0     1001      127      341 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1353 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/screentone/dot.rs
+-rw-r--r--   0     1001      127      986 2024-04-12 07:51:08.000000 pepeline-0.2.7/src/utils/screentone/screentone_add.rs
+-rw-r--r--   0     1001      127    33999 2024-04-12 07:51:12.000000 pepeline-0.2.7/Cargo.lock
+-rw-r--r--   0     1001      127      428 2024-04-12 07:51:08.000000 pepeline-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 pepeline-0.2.7/PKG-INFO
```

### Comparing `pepeline-0.2.6/Cargo.toml` & `pepeline-0.2.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pepeline"
-version = "0.2.6"
+version = "0.2.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pepeline"
 crate-type = ["cdylib"]
```

### Comparing `pepeline-0.2.6/.github/workflows/CI.yml` & `pepeline-0.2.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/.github/workflows/pipl.yml` & `pepeline-0.2.7/.github/workflows/pipl.yml`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/.gitignore` & `pepeline-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/LICENSE` & `pepeline-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/README.md` & `pepeline-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/pepeline.pyi` & `pepeline-0.2.7/pepeline.pyi`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/lib.rs` & `pepeline-0.2.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/core/color_levels.rs` & `pepeline-0.2.7/src/utils/core/color_levels.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/core/convert.rs` & `pepeline-0.2.7/src/utils/core/convert.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/core/noise.rs` & `pepeline-0.2.7/src/utils/core/noise.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/functions/core_funcion.rs` & `pepeline-0.2.7/src/utils/functions/core_funcion.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/functions/img_function.rs` & `pepeline-0.2.7/src/utils/functions/img_function.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/functions/screentone_function.rs` & `pepeline-0.2.7/src/utils/functions/screentone_function.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/image/decode.rs` & `pepeline-0.2.7/src/utils/image/decode.rs`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,14 @@
         Ok(Array3::from_shape_vec((height as usize, width as usize, channels), px)?.into_dyn())
     }
 }
 
 pub fn all_read_u8(path: &Path, mode: u8) -> Result<ArrayD<u8>, Box<dyn Error>> {
     let img = FileBuffer::open(path).map_err(|err| Box::new(err) as Box<dyn Error>)?;
     let img_magic_byte = &img[..4];
-    println!("{:?}", img_magic_byte);
     match img_magic_byte {
         [255, 216, 255, 224] | [255, 216, 255, 225] => match &img[6..8] {
             [74, 70] | [69, 120] => match mode {
                 0 => Ok(gray_img_open(&img)?.into_dyn()),
                 _ => Ok(rgb_img_open(&img)?.into_dyn()),
             },
             _ => match mode {
```

### Comparing `pepeline-0.2.6/src/utils/image/save.rs` & `pepeline-0.2.7/src/utils/image/save.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/screentone/dot.rs` & `pepeline-0.2.7/src/utils/screentone/dot.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/src/utils/screentone/screentone_add.rs` & `pepeline-0.2.7/src/utils/screentone/screentone_add.rs`

 * *Files identical despite different names*

### Comparing `pepeline-0.2.6/Cargo.lock` & `pepeline-0.2.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -374,17 +374,17 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "f08474e32172238f2827bd160c67871cdb2801430f65c3979184dc362e3ca118"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.1"
@@ -645,15 +645,15 @@
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pepeline"
-version = "0.2.6"
+version = "0.2.7"
 dependencies = [
  "filebuffer",
  "image",
  "ndarray",
  "noise",
  "numpy",
  "pyo3",
@@ -1279,17 +1279,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "zune-core"
 version = "0.4.12"
```

### Comparing `pepeline-0.2.6/PKG-INFO` & `pepeline-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pepeline
-Version: 0.2.6
+Version: 0.2.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

