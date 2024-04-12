# Comparing `tmp/xinterp-0.1.1.tar.gz` & `tmp/xinterp-0.1.2.tar.gz`

## Comparing `xinterp-0.1.1.tar` & `xinterp-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 xinterp-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     2832 2024-03-17 17:46:29.000000 xinterp-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      705 2024-03-17 17:46:29.000000 xinterp-0.1.1/.gitignore
--rw-r--r--   0     1001      127    35149 2024-03-17 17:46:29.000000 xinterp-0.1.1/LICENSE
--rw-r--r--   0     1001      127      881 2024-03-17 17:46:29.000000 xinterp-0.1.1/README.md
--rw-r--r--   0     1001      127     5511 2024-03-17 17:46:29.000000 xinterp-0.1.1/src/divop.rs
--rw-r--r--   0     1001      127     6563 2024-03-17 17:46:29.000000 xinterp-0.1.1/src/extended.rs
--rw-r--r--   0     1001      127     5460 2024-03-17 17:46:29.000000 xinterp-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127    19774 2024-03-17 17:46:29.000000 xinterp-0.1.1/src/piecewise.rs
--rw-r--r--   0     1001      127     4200 2024-03-17 17:46:29.000000 xinterp-0.1.1/src/schemes.rs
--rw-r--r--   0     1001      127    13133 2024-03-17 17:46:29.000000 xinterp-0.1.1/tests/test_core.py
--rw-r--r--   0     1001      127       35 2024-03-17 17:46:29.000000 xinterp-0.1.1/xinterp/__init__.py
--rw-r--r--   0     1001      127     5085 2024-03-17 17:46:29.000000 xinterp-0.1.1/xinterp/core.py
--rw-r--r--   0     1001      127    13324 2024-03-17 17:46:35.000000 xinterp-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127      455 2024-03-17 17:46:29.000000 xinterp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 xinterp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 xinterp-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     2832 2024-04-12 13:04:17.000000 xinterp-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      705 2024-04-12 13:04:17.000000 xinterp-0.1.2/.gitignore
+-rw-r--r--   0     1001      127    35149 2024-04-12 13:04:17.000000 xinterp-0.1.2/LICENSE
+-rw-r--r--   0     1001      127      881 2024-04-12 13:04:17.000000 xinterp-0.1.2/README.md
+-rw-r--r--   0     1001      127     5511 2024-04-12 13:04:17.000000 xinterp-0.1.2/src/divop.rs
+-rw-r--r--   0     1001      127     6252 2024-04-12 13:04:17.000000 xinterp-0.1.2/src/extended.rs
+-rw-r--r--   0     1001      127     5460 2024-04-12 13:04:17.000000 xinterp-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127    19774 2024-04-12 13:04:17.000000 xinterp-0.1.2/src/piecewise.rs
+-rw-r--r--   0     1001      127     4200 2024-04-12 13:04:17.000000 xinterp-0.1.2/src/schemes.rs
+-rw-r--r--   0     1001      127    14300 2024-04-12 13:04:17.000000 xinterp-0.1.2/tests/test_core.py
+-rw-r--r--   0     1001      127       35 2024-04-12 13:04:17.000000 xinterp-0.1.2/xinterp/__init__.py
+-rw-r--r--   0     1001      127     5085 2024-04-12 13:04:17.000000 xinterp-0.1.2/xinterp/core.py
+-rw-r--r--   0     1001      127    13324 2024-04-12 13:04:21.000000 xinterp-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127      455 2024-04-12 13:04:17.000000 xinterp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 xinterp-0.1.2/PKG-INFO
```

### Comparing `xinterp-0.1.1/.github/workflows/CI.yml` & `xinterp-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/.gitignore` & `xinterp-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/LICENSE` & `xinterp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/README.md` & `xinterp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/src/divop.rs` & `xinterp-0.1.2/src/divop.rs`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/src/extended.rs` & `xinterp-0.1.2/src/extended.rs`

 * *Files 2% similar despite different names*

```diff
@@ -141,24 +141,16 @@
     pub fn rem(&self, rhs: &F80) -> F80 {
         F80 {
             value: self.value.rem(&rhs.value),
         }
     }
     /// Rounds a F80  to its nearest integer using the round ties to even rule.
     pub fn round(&self) -> F80 {
-        let floor = self.floor();
-        let ceil = self.ceil();
-        let mid = floor.add(&ceil).div(&F80::from(2));
-        match self.cmp(&mid) {
-            Ordering::Less => floor,
-            Ordering::Equal => match floor.rem(&F80::from(2)).eq(&F80::from(0)) {
-                true => floor,
-                false => ceil,
-            },
-            Ordering::Greater => ceil,
+        F80 {
+            value: self.value.round(0, RoundingMode::ToEven),
         }
     }
     /// Floors a F80.
     pub fn floor(&self) -> F80 {
         F80 {
             value: self.value.floor(),
         }
```

### Comparing `xinterp-0.1.1/src/lib.rs` & `xinterp-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/src/piecewise.rs` & `xinterp-0.1.2/src/piecewise.rs`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/src/schemes.rs` & `xinterp-0.1.2/src/schemes.rs`

 * *Files identical despite different names*

### Comparing `xinterp-0.1.1/tests/test_core.py` & `xinterp-0.1.2/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,19 @@
         with pytest.raises(ValueError, match="xp and fp must be 1D"):
             forward([1], [0, 2], [[3, 5]])
 
     def test_raises_shape_mismatch(self):
         with pytest.raises(ValueError, match="xp and fp must have the same length"):
             forward([1], [0, 2, 5], [3, 5])
 
-    def test_raises_only_one_element(self):
+    def test_raises_at_no_element(self):
         with pytest.raises(
-            ValueError, match="xp and fp must have at least two elements"
+            ValueError, match="xp and fp must have at least one elements"
         ):
-            forward([1], [0], [3])
+            forward([1], [], [])
 
     def test_raises_xp_not_integer(self):
         with pytest.raises(ValueError, match="xp must have integer dtype"):
             forward([1], [0.0, 2.0], [3, 5])
 
     def test_raises_not_positive(self):
         with pytest.raises(ValueError, match="xp values must be positive"):
@@ -74,14 +74,24 @@
         assert forward([1], [0, 2], [3, 5]).ndim == 1
         assert forward(1, [0, 2], [3, 5]).ndim == 0
         assert forward([1], [0, 2], np.array([3, 5], "M8[s]")).ndim == 1
         assert forward(1, [0, 2], np.array([3, 5], "M8[s]")).ndim == 0
         assert forward([1], [0, 2], np.array([3, 5], "f4")).ndim == 1
         assert forward(1, [0, 2], np.array([3, 5], "f4")).ndim == 0
 
+    def test_empty_handling(self):
+        assert forward([], [0, 2], [3, 5]).shape == (0,)
+        assert forward([], [0, 2], np.array([3, 5], "M8[s]")).shape == (0,)
+        assert forward([], [0, 2], np.array([3, 5], "f4")).shape == (0,)
+
+    def test_singleton_handling(self):
+        assert forward(0, [0], [3]) == 3
+        assert forward(0, [0], [3.0]) == 3.0
+        assert forward(0, [0], np.array([3], "M8[s]")) == np.array([3], "M8[s]")
+
     def test_interpolation_accuracy_int(self):
         rng = np.random.default_rng(42)
         n = 1_000
         m = 10_000
         integers = np.arange(0, 65_535)
         xp = np.sort(rng.choice(integers, n, replace=False))
         fp = rng.integers(np.min(integers), np.max(integers), n)
@@ -116,19 +126,19 @@
         with pytest.raises(ValueError, match="xp and fp must be 1D"):
             inverse([4], [0, 2], [[3, 5]])
 
     def test_raises_shape_mismatch(self):
         with pytest.raises(ValueError, match="xp and fp must have the same length"):
             inverse([4], [0, 2, 5], [3, 5])
 
-    def test_raises_only_one_element(self):
+    def test_raises_no_element(self):
         with pytest.raises(
-            ValueError, match="xp and fp must have at least two elements"
+            ValueError, match="xp and fp must have at least one elements"
         ):
-            inverse([4], [0], [3])
+            inverse([4], [], [])
 
     def test_raises_xp_not_integer(self):
         with pytest.raises(ValueError, match="xp must have integer dtype"):
             inverse([4], [0.0, 2.0], [3, 5])
 
     def test_raises_not_positive(self):
         with pytest.raises(ValueError, match="xp values must be positive"):
@@ -204,14 +214,32 @@
         assert (
             inverse(np.array([4], "M8[s]"), [0, 2], np.array([3, 5], "M8[s]")).ndim == 1
         )
         assert (
             inverse(np.array(4, "M8[s]"), [0, 2], np.array([3, 5], "M8[s]")).ndim == 0
         )
 
+    def test_empty_handling(self):
+        assert inverse([], [0, 2], [3, 5]).shape == (0,)
+        assert inverse([], [0, 2], [3.0, 5.0]).shape == (0,)
+        assert inverse(
+            np.array([], "M8[s]"), [0, 2], np.array([3, 5], "M8[s]")
+        ).shape == (0,)
+
+    def test_singleton_handling(self):
+        assert inverse(3, [0], [3]) == 0
+        assert inverse(3.0, [0], [3.0]) == 0
+        assert inverse(np.array(3, "M8[s]"), [0], np.array([3], "M8[s]")) == 0
+        assert inverse(4, [0], [3], method="nearest") == 0
+        assert inverse(4.0, [0], [3.0], method="nearest") == 0
+        assert (
+            inverse(np.array(4, "M8[s]"), [0], np.array([3], "M8[s]"), method="nearest")
+            == 0
+        )
+
     def test_interpolation_accuracy_int(self):
         rng = np.random.default_rng(42)
         n = 1_000
         m = 10_000
         integers = np.arange(0, 65_535)
         xp = rng.integers(np.min(integers), np.max(integers), n)
         fp = np.sort(rng.choice(integers, n, replace=False))
```

### Comparing `xinterp-0.1.1/xinterp/core.py` & `xinterp-0.1.2/xinterp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 def check(xp, fp, x=None, f=None):
     xp = np.asarray(xp)
     fp = np.asarray(fp)
     if not (xp.ndim == 1 and fp.ndim == 1):
         raise ValueError("xp and fp must be 1D")
     if not (len(xp) == len(fp)):
         raise ValueError("xp and fp must have the same length")
-    if not (len(xp) > 1 and len(fp) > 1):
-        raise ValueError("xp and fp must have at least two elements")
+    if not (len(xp) > 0 and len(fp) > 0):
+        raise ValueError("xp and fp must have at least one elements")
     if not np.issubdtype(xp.dtype, np.integer):
         raise ValueError("xp must have integer dtype")
     if not np.all(xp >= 0):
         raise ValueError("xp values must be positive")
     if not np.all(np.isfinite(fp)):
         raise ValueError("fp values must be finite")
     if (x is None) == (f is None):
```

### Comparing `xinterp-0.1.1/Cargo.lock` & `xinterp-0.1.2/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "astro-float"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a278f34b7b731081d83aabe76931cb51b28230882ff565a50df393827fead49a"
+checksum = "3ffbd469c925b479358981be1e1f1207ab20fecd8ed72734edcbcfc8e9374312"
 dependencies = [
  "astro-float-macro",
  "astro-float-num",
 ]
 
 [[package]]
 name = "astro-float-macro"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fdfbb78b0e0657be5dc948bb6e4b09763f404f183017b513979ee026f875713c"
+checksum = "eac843ce8123b98c0da2667e1db6db6531d4dee133101a486afc6d8b1db34279"
 dependencies = [
  "astro-float-num",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "astro-float-num"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aea86464fc5b8b8ad30bc68d3b1b1fd75595189585dc6468a418a4f653a3c8c7"
+checksum = "3bf9647991ed5c8432085c326d70badf4d2480778434e657fb32a4fd353e441f"
 dependencies = [
  "itertools",
  "lazy_static",
  "rand",
  "serde",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -58,34 +58,34 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
@@ -122,17 +122,17 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
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
 name = "ndarray"
 version = "0.15.6"
@@ -281,35 +281,35 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -380,39 +380,39 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.53",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.53"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7383cd0e49fff4b6b90ca5670bfd3e9d6a733b3f90c686605aa7eec8c4996032"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -494,13 +494,13 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "xinterp"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "astro-float",
  "numpy",
  "pyo3",
 ]
```

### Comparing `xinterp-0.1.1/PKG-INFO` & `xinterp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xinterp
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: numpy
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Provides-Extra: dev
```

