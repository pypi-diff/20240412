# Comparing `tmp/libredr-0.0.17.tar.gz` & `tmp/libredr-0.0.18.tar.gz`

## Comparing `libredr-0.0.17.tar` & `libredr-0.0.18.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-------   0     1000     1000      919 2023-11-03 06:29:07.000000 libredr-0.0.17/common/Cargo.toml
--rw-------   0     1000     1000       60 2023-10-09 07:46:23.000000 libredr-0.0.17/common/src/build.rs
--rw-------   0     1000     1000     5379 2024-02-13 08:38:31.000000 libredr-0.0.17/common/src/connection.rs
--rw-------   0     1000     1000    13359 2023-10-09 07:46:23.000000 libredr-0.0.17/common/src/geometry.rs
--rw-------   0     1000     1000     2203 2023-10-09 07:46:23.000000 libredr-0.0.17/common/src/lib.rs
--rw-------   0     1000     1000    17891 2023-10-19 07:18:42.000000 libredr-0.0.17/common/src/message.rs
--rw-------   0     1000     1000     1695 2023-10-09 07:46:23.000000 libredr-0.0.17/common/src/render.rs
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 libredr-0.0.17/client/Cargo.toml
--rw-------   0     1000     1000    34523 2023-05-20 05:47:22.000000 libredr-0.0.17/client/LICENSE
--rw-------   0     1000     1000     2096 2023-11-03 12:08:52.000000 libredr-0.0.17/client/README.md
--rw-------   0     1000     1000      781 2023-12-13 12:15:03.000000 libredr-0.0.17/client/python/libredr/__init__.py
--rw-------   0     1000     1000      292 2023-10-09 07:46:23.000000 libredr-0.0.17/client/python/libredr/camera/__init__.py
--rw-------   0     1000     1000     1904 2023-10-09 07:46:23.000000 libredr-0.0.17/client/python/libredr/camera/cube.py
--rw-------   0     1000     1000     2063 2023-10-09 07:46:23.000000 libredr-0.0.17/client/python/libredr/camera/equirectangular.py
--rw-------   0     1000     1000     1650 2023-10-09 07:46:23.000000 libredr-0.0.17/client/python/libredr/camera/perspective.py
--rw-------   0     1000     1000      294 2023-12-13 12:32:46.000000 libredr-0.0.17/client/python/libredr/torch/__init__.py
--rw-------   0     1000     1000     2017 2023-12-31 17:18:59.000000 libredr-0.0.17/client/python/libredr/torch/light_source/__init__.py
--rw-------   0     1000     1000     2852 2023-12-13 12:20:45.000000 libredr-0.0.17/client/python/libredr/torch/nn/functional.py
--rw-------   0     1000     1000     5749 2024-02-18 07:05:04.000000 libredr-0.0.17/client/python/libredr/torch/ray_tracing.py
--rw-------   0     1000     1000     3137 2023-10-09 07:46:23.000000 libredr-0.0.17/client/src/camera/orthogonal.rs
--rw-------   0     1000     1000     3592 2023-10-09 07:46:23.000000 libredr-0.0.17/client/src/camera.rs
--rw-------   0     1000     1000    11463 2023-10-09 07:46:23.000000 libredr-0.0.17/client/src/client.rs
--rw-------   0     1000     1000    17191 2023-11-03 12:08:54.000000 libredr-0.0.17/client/src/lib.rs
--rw-------   0     1000     1000     2049 2024-02-13 07:41:12.000000 libredr-0.0.17/client/src/light_source/directional.rs
--rw-------   0     1000     1000     1810 2024-02-18 12:19:38.000000 libredr-0.0.17/client/src/light_source/functional.rs
--rw-------   0     1000     1000      568 2024-02-13 06:23:12.000000 libredr-0.0.17/client/src/light_source.rs
--rw-------   0     1000     1000     2096 2023-11-03 12:08:52.000000 libredr-0.0.17/README.md
--rw-------   0     1000     1000    53284 2024-02-18 09:55:42.000000 libredr-0.0.17/Cargo.lock
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 libredr-0.0.17/Cargo.toml
--rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 libredr-0.0.17/pyproject.toml
--rw-------   0     1000     1000      294 2023-12-13 12:32:46.000000 libredr-0.0.17/python/libredr/torch/__init__.py
--rw-------   0     1000     1000     2852 2023-12-13 12:20:45.000000 libredr-0.0.17/python/libredr/torch/nn/functional.py
--rw-------   0     1000     1000     2017 2023-12-31 17:18:59.000000 libredr-0.0.17/python/libredr/torch/light_source/__init__.py
--rw-------   0     1000     1000     5749 2024-02-18 07:05:04.000000 libredr-0.0.17/python/libredr/torch/ray_tracing.py
--rw-------   0     1000     1000      781 2023-12-13 12:15:03.000000 libredr-0.0.17/python/libredr/__init__.py
--rw-------   0     1000     1000     1904 2023-10-09 07:46:23.000000 libredr-0.0.17/python/libredr/camera/cube.py
--rw-------   0     1000     1000     1650 2023-10-09 07:46:23.000000 libredr-0.0.17/python/libredr/camera/perspective.py
--rw-------   0     1000     1000      292 2023-10-09 07:46:23.000000 libredr-0.0.17/python/libredr/camera/__init__.py
--rw-------   0     1000     1000     2063 2023-10-09 07:46:23.000000 libredr-0.0.17/python/libredr/camera/equirectangular.py
--rw-------   0     1000     1000    34523 2023-05-20 05:47:22.000000 libredr-0.0.17/LICENSE
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 libredr-0.0.17/PKG-INFO
+-rw-------   0     1000     1000      919 2023-11-03 06:29:07.000000 libredr-0.0.18/common/Cargo.toml
+-rw-------   0     1000     1000       60 2023-10-09 07:46:23.000000 libredr-0.0.18/common/src/build.rs
+-rw-------   0     1000     1000     5379 2024-02-13 08:38:31.000000 libredr-0.0.18/common/src/connection.rs
+-rw-------   0     1000     1000    13359 2023-10-09 07:46:23.000000 libredr-0.0.18/common/src/geometry.rs
+-rw-------   0     1000     1000     2203 2023-10-09 07:46:23.000000 libredr-0.0.18/common/src/lib.rs
+-rw-------   0     1000     1000    17891 2023-10-19 07:18:42.000000 libredr-0.0.18/common/src/message.rs
+-rw-------   0     1000     1000     1695 2023-10-09 07:46:23.000000 libredr-0.0.18/common/src/render.rs
+-rw-------   0     1000     1000     2096 2023-11-03 12:08:52.000000 libredr-0.0.18/README.md
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 libredr-0.0.18/client/Cargo.toml
+-rw-------   0     1000     1000    34523 2023-05-20 05:47:22.000000 libredr-0.0.18/client/LICENSE
+-rw-------   0     1000     1000     2096 2023-11-03 12:08:52.000000 libredr-0.0.18/client/README.md
+-rw-------   0     1000     1000      781 2023-12-13 12:15:03.000000 libredr-0.0.18/client/python/libredr/__init__.py
+-rw-------   0     1000     1000      292 2023-10-09 07:46:23.000000 libredr-0.0.18/client/python/libredr/camera/__init__.py
+-rw-------   0     1000     1000     1904 2023-10-09 07:46:23.000000 libredr-0.0.18/client/python/libredr/camera/cube.py
+-rw-------   0     1000     1000     2063 2023-10-09 07:46:23.000000 libredr-0.0.18/client/python/libredr/camera/equirectangular.py
+-rw-------   0     1000     1000     1650 2023-10-09 07:46:23.000000 libredr-0.0.18/client/python/libredr/camera/perspective.py
+-rw-------   0     1000     1000      294 2023-12-13 12:32:46.000000 libredr-0.0.18/client/python/libredr/torch/__init__.py
+-rw-------   0     1000     1000     2017 2023-12-31 17:18:59.000000 libredr-0.0.18/client/python/libredr/torch/light_source/__init__.py
+-rw-------   0     1000     1000     2852 2023-12-13 12:20:45.000000 libredr-0.0.18/client/python/libredr/torch/nn/functional.py
+-rw-------   0     1000     1000     5749 2024-02-18 07:05:04.000000 libredr-0.0.18/client/python/libredr/torch/ray_tracing.py
+-rw-------   0     1000     1000     3177 2024-04-12 06:41:13.000000 libredr-0.0.18/client/src/camera/orthogonal.rs
+-rw-------   0     1000     1000     3651 2024-04-12 07:48:08.000000 libredr-0.0.18/client/src/camera.rs
+-rw-------   0     1000     1000    11463 2024-03-23 12:01:24.000000 libredr-0.0.18/client/src/client.rs
+-rw-------   0     1000     1000    17278 2024-04-12 07:44:57.000000 libredr-0.0.18/client/src/lib.rs
+-rw-------   0     1000     1000     2089 2024-04-12 07:22:58.000000 libredr-0.0.18/client/src/light_source/directional.rs
+-rw-------   0     1000     1000     1810 2024-02-18 12:19:38.000000 libredr-0.0.18/client/src/light_source/functional.rs
+-rw-------   0     1000     1000      594 2024-04-12 07:48:26.000000 libredr-0.0.18/client/src/light_source.rs
+-rw-------   0     1000     1000    53727 2024-04-12 05:46:23.000000 libredr-0.0.18/Cargo.lock
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 libredr-0.0.18/Cargo.toml
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 libredr-0.0.18/pyproject.toml
+-rw-------   0     1000     1000      294 2023-12-13 12:32:46.000000 libredr-0.0.18/python/libredr/torch/__init__.py
+-rw-------   0     1000     1000     2852 2023-12-13 12:20:45.000000 libredr-0.0.18/python/libredr/torch/nn/functional.py
+-rw-------   0     1000     1000     2017 2023-12-31 17:18:59.000000 libredr-0.0.18/python/libredr/torch/light_source/__init__.py
+-rw-------   0     1000     1000     5749 2024-02-18 07:05:04.000000 libredr-0.0.18/python/libredr/torch/ray_tracing.py
+-rw-------   0     1000     1000      781 2023-12-13 12:15:03.000000 libredr-0.0.18/python/libredr/__init__.py
+-rw-------   0     1000     1000     1904 2023-10-09 07:46:23.000000 libredr-0.0.18/python/libredr/camera/cube.py
+-rw-------   0     1000     1000     1650 2023-10-09 07:46:23.000000 libredr-0.0.18/python/libredr/camera/perspective.py
+-rw-------   0     1000     1000      292 2023-10-09 07:46:23.000000 libredr-0.0.18/python/libredr/camera/__init__.py
+-rw-------   0     1000     1000     2063 2023-10-09 07:46:23.000000 libredr-0.0.18/python/libredr/camera/equirectangular.py
+-rw-------   0     1000     1000    34523 2023-05-20 05:47:22.000000 libredr-0.0.18/LICENSE
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 libredr-0.0.18/PKG-INFO
```

### Comparing `libredr-0.0.17/common/Cargo.toml` & `libredr-0.0.18/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/common/src/connection.rs` & `libredr-0.0.18/common/src/connection.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/common/src/geometry.rs` & `libredr-0.0.18/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/common/src/lib.rs` & `libredr-0.0.18/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/common/src/message.rs` & `libredr-0.0.18/common/src/message.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/common/src/render.rs` & `libredr-0.0.18/common/src/render.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/Cargo.toml` & `libredr-0.0.18/client/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/LICENSE` & `libredr-0.0.18/client/LICENSE`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/README.md` & `libredr-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/__init__.py` & `libredr-0.0.18/client/python/libredr/__init__.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/camera/cube.py` & `libredr-0.0.18/client/python/libredr/camera/cube.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/camera/equirectangular.py` & `libredr-0.0.18/client/python/libredr/camera/equirectangular.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/camera/perspective.py` & `libredr-0.0.18/client/python/libredr/camera/perspective.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/torch/light_source/__init__.py` & `libredr-0.0.18/client/python/libredr/torch/light_source/__init__.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/torch/nn/functional.py` & `libredr-0.0.18/client/python/libredr/torch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/python/libredr/torch/ray_tracing.py` & `libredr-0.0.18/client/python/libredr/torch/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/src/camera/orthogonal.rs` & `libredr-0.0.18/client/src/camera/orthogonal.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::cmp::max;
 use nalgebra as na;
 use pyo3::prelude::*;
 use ndarray::{Axis, Array1, Array3};
 use anyhow::{Result, anyhow, ensure};
-use numpy::{PyReadonlyArray2, PyArray3, ToPyArray};
+use numpy::{PyReadonlyArray2, PyArray3, IntoPyArray, PyUntypedArrayMethods};
 use super::from_ray_corner;
 
 /// Construct input ray for orthogonal camera model
 /// # Arguments
 /// * `resolution`: tuple of 2 usize [`width`, `height`]
 /// * `intrinsic`: 3 * 3 matrix
 /// * `extrinsic`: 4 * 4 matrix
@@ -43,21 +43,21 @@
   from_ray_corner(ray_corner)
 }
 
 /// Python version [`orthogonal_ray`]
 /// `intrinsic` and `extrinsic` need to be F-contiguous (column first order)
 #[pyfunction]
 #[pyo3(name = "orthogonal_ray")]
-pub fn py_orthogonal_ray(
-    py: Python,
+pub fn py_orthogonal_ray<'py>(
+    py: Python<'py>,
     resolution: [usize; 2],
     intrinsic: PyReadonlyArray2<f32>,
-    extrinsic: PyReadonlyArray2<f32>) -> Result<Py<PyArray3<f32>>> {
+    extrinsic: PyReadonlyArray2<f32>) -> Result<Bound<'py, PyArray3<f32>>> {
   ensure!(intrinsic.shape() == [3, 3],
     "camera::orthogonal_ray: `intrinsic` expected shape {:?}, found {:?}", [3, 3], intrinsic.shape());
   let intrinsic = intrinsic.try_as_matrix().ok_or(anyhow!("camera::orthogonal_ray: `intrinsic` is not F-contiguous"))?;
   ensure!(extrinsic.shape() == [4, 4],
     "camera::orthogonal_ray: `extrinsic` expected shape {:?}, found {:?}", [4, 4], extrinsic.shape());
   let extrinsic = extrinsic.try_as_matrix().ok_or(anyhow!("camera::orthogonal_ray: `extrinsic` is not F-contiguous"))?;
   let ray = orthogonal_ray(&resolution, intrinsic, extrinsic)?;
-  Ok(ray.to_pyarray(py).to_owned())
+  Ok(ray.into_pyarray_bound(py))
 }
```

### Comparing `libredr-0.0.17/client/src/camera.rs` & `libredr-0.0.18/client/src/camera.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use nalgebra as na;
 use pyo3::prelude::*;
 use ndarray::{Axis, Array3};
 use anyhow::{Result, anyhow, ensure};
-use numpy::{PyReadonlyArray1, PyArray2, ToPyArray};
+use numpy::{PyReadonlyArray1, PyArray2, ToPyArray, PyUntypedArrayMethods};
 
 mod orthogonal;
 
 const EPS: f32 = 1e-6;
 
 /// Orthogonal camera model (Rust and Python)
 pub use self::orthogonal::{orthogonal_ray, py_orthogonal_ray};
@@ -51,30 +51,30 @@
   Ok(rotation * translation)
 }
 
 /// Python version [`look_at_extrinsic`]
 /// Return matrix is F-contiguous (column first order)
 #[pyfunction]
 #[pyo3(name = "look_at_extrinsic")]
-pub fn py_look_at_extrinsic(
-    py: Python<'_>,
+pub fn py_look_at_extrinsic<'py>(
+    py: Python<'py>,
     position: PyReadonlyArray1<f32>,
     look_at: PyReadonlyArray1<f32>,
-    up: PyReadonlyArray1<f32>) -> PyResult<Py<PyArray2<f32>>> {
+    up: PyReadonlyArray1<f32>) -> PyResult<Bound<'py, PyArray2<f32>>> {
   let position = position.try_as_matrix().ok_or(
     anyhow!("camera::look_at_extrinsic: `position` expected shape {:?}, found {:?}", [3], position.shape()))?;
   let look_at = look_at.try_as_matrix().ok_or(
     anyhow!("camera::look_at_extrinsic: `look_at` expected shape {:?}, found {:?}", [3], look_at.shape()))?;
   let up = up.try_as_matrix().ok_or(
     anyhow!("camera::look_at_extrinsic: `up` expected shape {:?}, found {:?}", [3], up.shape()))?;
   let extrinsic = look_at_extrinsic(position, look_at, up)?;
-  Ok(extrinsic.to_pyarray(py).to_owned())
+  Ok(extrinsic.to_pyarray_bound(py))
 }
 
 /// All camera models (Python)
-pub fn py_camera(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
-  let module = PyModule::new(py, "camera")?;
-  module.add_function(wrap_pyfunction!(py_look_at_extrinsic, module)?)?;
-  module.add_function(wrap_pyfunction!(py_orthogonal_ray, module)?)?;
-  parent_module.add_submodule(module)?;
+pub fn py_camera<'py>(py: Python<'py>, parent_module: &Bound<'py, PyModule>) -> PyResult<()> {
+  let module = PyModule::new_bound(py, "camera")?;
+  module.add_function(wrap_pyfunction!(py_look_at_extrinsic, &module)?)?;
+  module.add_function(wrap_pyfunction!(py_orthogonal_ray, &module)?)?;
+  parent_module.add_submodule(&module)?;
   Ok(())
 }
```

### Comparing `libredr-0.0.17/client/src/client.rs` & `libredr-0.0.18/client/src/client.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
   ///     * including ray position 9 * `image_shape`
   ///     * including ray direction 9 * `image_shape`
   ///   * if `camera_space` is `true`, add another (1 + 14) channels
   ///     * including ray depth 1 * `image_shape` (if depth <= 0, treat as hit miss)
   ///     * including ray material 14 * `image_shape`
   /// * `texture` - (3 + 3 + 3 + 1 + 3 + 1) * `texture_resolution` * `texture_resolution` (must be square image)
   ///   * including normal + diffuse + specular + roughness + intensity + window
-  /// * `envmap` - 3 * 8 * `envmap_resolution` * `envmap_resolution`
+  /// * `envmap` - 3 * 6 * `envmap_resolution` * `envmap_resolution`
   ///   * (must be box unwrapped 6 square images)
   /// * `sample_per_pixel` - `sample_per_pixel_forward`, `sample_per_pixel_backward`
   /// * `max_bounce` - `max_bounce_forward`, `max_bounce_backward`, `max_bounce_low_discrepancy`, `skip_bounce`
   /// * `switches` - tuple of 4 switches to determine hit miss and reflection behavior
   ///   * render::MISS_* - determine how to deal with ray hit miss
   ///     * [`common::render::MISS_NONE`]
   ///     * [`common::render::MISS_ENVMAP`]
@@ -187,15 +187,15 @@
   ///
   /// # Return
   /// Return shape will be,
   /// * if `camera_space` is `false` for [`RequestRayTracingForward`] task
   ///   * 1st return value (3 + 3 + 3 + 1 + 3 + 1) * `texture_resolution` * `texture_resolution`
   ///     * (same `texture_resolution` as [`RequestRayTracingForward`])
   ///     * including d_normal + d_diffuse + d_specular + d_roughness + d_intensity + d_window
-  ///   * 2nd return value 3 * 8 * `envmap_resolution` * `envmap_resolution`
+  ///   * 2nd return value 3 * 6 * `envmap_resolution` * `envmap_resolution`
   ///     * (same `envmap_resolution` as [`RequestRayTracingForward`])
   ///     * including d_envmap
   /// * if `camera_space` is `true` for [`RequestRayTracingForward`] task, add another
   ///   * 3rd return value 14 * `image_shape` (same shape as [`RequestRayTracingForward`])
   ///     * including d_ray_texture
   #[allow(clippy::too_many_arguments)]
   pub async fn ray_tracing_backward(&mut self, d_ray: ArrayD<f32>) ->
```

### Comparing `libredr-0.0.17/client/src/lib.rs` & `libredr-0.0.18/client/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 use pyo3::prelude::*;
 use anyhow::{Result, bail};
 use tokio::runtime::Runtime;
 use tracing::{error, debug};
 use once_cell::sync::OnceCell;
 use tracing_subscriber::{fmt, EnvFilter, prelude::*};
 use numpy::{PyReadonlyArray2, PyReadonlyArray3, PyReadonlyArray4, PyReadonlyArrayDyn, PyArray3, PyArray4, PyArrayDyn,
-  ToPyArray};
+  IntoPyArray, PyArrayMethods};
 use common::render;
 use common::message::*;
 pub use common::geometry::Geometry;
 pub use self::client::LibreDR;
 use self::camera::py_camera;
 use self::light_source::py_light_source;
 
@@ -177,15 +177,15 @@
   ///     * including ray position 9 * `image_shape`
   ///     * including ray direction 9 * `image_shape`
   ///   * if `camera_space` is `true`, add another (1 + 14) channels
   ///     * including ray depth 1 * `image_shape` (if depth <= 0, treat as hit miss)
   ///     * including ray material 14 * `image_shape`
   /// * `texture` - (3 + 3 + 3 + 1 + 3 + 1) * `texture_resolution` * `texture_resolution` (must be square image)
   ///   * including normal + diffuse + specular + roughness + intensity + window
-  /// * `envmap` - 3 * 8 * `envmap_resolution` * `envmap_resolution`
+  /// * `envmap` - 3 * 6 * `envmap_resolution` * `envmap_resolution`
   ///   * (must be box unwrapped 6 square images)
   /// * `sample_per_pixel` - `sample_per_pixel_forward`, (`sample_per_pixel_backward`)
   ///   * `sample_per_pixel` can be a single integer,
   ///     * (same value for forward and backward)
   ///   * or tuple of 2 integers.
   ///     * (only `sample_per_pixel_backward` number of rays are stored for backward)
   ///     * (must ensure `sample_per_pixel_forward` >= `sample_per_pixel_backward`)
@@ -231,29 +231,29 @@
   ///     * render image 3 * `image_shape`
   ///   * if `camera_space` is `false`, add another
   ///     * ray texture coordinate 2 * `image_shape`
   ///     * ray depth (Euclidean distance) 1 * `image_shape`
   ///     * ray normal 3 * `image_shape`
   #[pyo3(name = "ray_tracing_forward")]
   #[allow(clippy::too_many_arguments)]
-  pub fn py_ray_tracing_forward(
+  pub fn py_ray_tracing_forward<'py>(
       &mut self,
-      py: Python,
+      py: Python<'py>,
       geometry: &PyGeometry,
       ray: PyReadonlyArrayDyn<f32>,
       texture: PyReadonlyArray3<f32>,
       envmap: PyReadonlyArray4<f32>,
       sample_per_pixel: Py<PyAny>,
       max_bounce: Py<PyAny>,
       switches: (u8, u8, u8, u8),
       clip_near: Py<PyAny>,
       camera_space: bool,
       requires_grad: bool,
       srand: i32,
-      low_discrepancy: Option<u32>) -> Result<Py<PyArrayDyn<f32>>> {
+      low_discrepancy: Option<u32>) -> Result<Bound<'py, PyArrayDyn<f32>>> {
     debug!("py_ray_tracing_forward: enter");
     let ray = ray.to_owned_array();
     let texture = texture.to_owned_array();
     let envmap = envmap.to_owned_array();
     let sample_per_pixel:(usize, usize) = if let Ok(sample_per_pixel_forward) = sample_per_pixel.extract(py) {
       (sample_per_pixel_forward, sample_per_pixel_forward)
     } else if let Ok(sample_per_pixel) = sample_per_pixel.extract(py) {
@@ -294,15 +294,15 @@
         clip_near,
         camera_space,
         requires_grad,
         srand,
         low_discrepancy
       ))
     })?;
-    Ok(response.to_pyarray(py).to_owned())
+    Ok(response.into_pyarray_bound(py))
   }
 
   /// Create a [`RequestRayTracingBackward`] task and wait for response.
   ///
   /// Must be called consecutive to a [`RequestRayTracingForward`] task with `requires_grad` set to `true`. \
   /// To create multiple [`RequestRayTracingForward`] tasks and backward together, multiple client connections are
   /// required.
@@ -312,35 +312,36 @@
   ///
   /// # Return
   /// Return shape will be,
   /// * if `camera_space` is `false` for [`RequestRayTracingForward`] task
   ///   * 1st return value (3 + 3 + 3 + 1 + 3 + 1) * `texture_resolution` * `texture_resolution`
   ///     * (same `texture_resolution` as [`RequestRayTracingForward`])
   ///     * including d_normal + d_diffuse + d_specular + d_roughness + d_intensity + d_window
-  ///   * 2nd return value 3 * 8 * `envmap_resolution` * `envmap_resolution`
+  ///   * 2nd return value 3 * 6 * `envmap_resolution` * `envmap_resolution`
   ///     * (same `envmap_resolution` as [`RequestRayTracingForward`])
   ///     * including d_envmap
   /// * if `camera_space` is `true` for [`RequestRayTracingForward`] task, add another
   ///   * 3rd return value 14 * `image_shape` (same shape as [`RequestRayTracingForward`])
   ///     * including d_ray_texture
   #[pyo3(name = "ray_tracing_backward")]
   #[allow(clippy::type_complexity)]
-  pub fn py_ray_tracing_backward(
-    &mut self,
-    py: Python,
-    d_ray: PyReadonlyArrayDyn<f32>) -> Result<(Py<PyArray3<f32>>, Py<PyArray4<f32>>, Option<Py<PyArrayDyn<f32>>>)> {
+  pub fn py_ray_tracing_backward<'py>(
+      &mut self,
+      py: Python<'py>,
+      d_ray: PyReadonlyArrayDyn<f32>
+    ) -> Result<(Bound<'py, PyArray3<f32>>, Bound<'py, PyArray4<f32>>, Option<Bound<'py, PyArrayDyn<f32>>>)> {
     debug!("py_ray_tracing_backward: enter");
     let d_ray = d_ray.to_owned_array();
     let response = py.allow_threads(|| {
       let rt = RUNTIME.get().expect("Initialized in pymodule");
       rt.block_on(self.0.ray_tracing_backward(d_ray))
     })?;
-    let d_texture = response.0.to_pyarray(py).to_owned();
-    let d_envmap = response.1.to_pyarray(py).to_owned();
-    let d_ray_texture = response.2.map(|d_ray_texture| d_ray_texture.to_pyarray(py).to_owned());
+    let d_texture = response.0.into_pyarray_bound(py);
+    let d_envmap = response.1.into_pyarray_bound(py);
+    let d_ray_texture = response.2.map(|d_ray_texture| d_ray_texture.into_pyarray_bound(py));
     Ok((d_texture, d_envmap, d_ray_texture))
   }
 }
 
 impl Drop for PyLibreDR {
   fn drop(&mut self) {
     let rt = RUNTIME.get().expect("Initialized in pymodule");
@@ -371,15 +372,15 @@
 /// Accept `LIBREDR_LOG_LEVEL` environment variable to set `log_level`.
 /// * (default: info, feasible: debug, info, warn, error)
 ///
 /// Accept `LIBREDR_WORKER_THREADS` environment variable to set `worker_threads`
 /// * (default: 1)
 #[pymodule]
 #[pyo3(name = "libredr")]
-pub fn py_libredr(py: Python<'_>, module: &PyModule) -> PyResult<()> {
+pub fn py_libredr<'py>(py: Python<'py>, module: &Bound<'py, PyModule>) -> PyResult<()> {
   init_static()?;
   module.add("__author__", "Bohan Yu <ybh1998@protonmail.com>")?;
   module.add("__version__", format!("LibreDR {}", common::CLAP_LONG_VERSION))?;
   module.add_class::<PyLibreDR>()?;
   module.add_class::<PyGeometry>()?;
   py_camera(py, module)?;
   py_light_source(py, module)?;
```

### Comparing `libredr-0.0.17/client/src/light_source/directional.rs` & `libredr-0.0.18/client/src/light_source/directional.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use nalgebra as na;
 use pyo3::prelude::*;
 use ndarray::{s, Array4};
 use anyhow::{Result, anyhow, ensure};
-use numpy::{PyReadonlyArray1, PyArray4, ToPyArray};
+use numpy::{PyReadonlyArray1, PyArray4, IntoPyArray, PyUntypedArrayMethods};
 
 const EPS: f32 = 1e-6;
 
 /// Construct one-hot envmap with given direction and intensity
 /// # Arguments
 /// * `resolution`: a single integer
 /// * `direction`: f32 vector of 3
@@ -35,17 +35,17 @@
   envmap.slice_mut(s![.., face_id, envmap_row, envmap_col]).fill(intensity);
   Ok(envmap)
 }
 
 /// Python version [`directional_envmap`]
 #[pyfunction]
 #[pyo3(name = "directional_envmap")]
-pub fn py_directional_envmap(
-    py: Python,
+pub fn py_directional_envmap<'py>(
+    py: Python<'py>,
     resolution: usize,
     direction: PyReadonlyArray1<f32>,
-    intensity: f32) -> Result<Py<PyArray4<f32>>> {
+    intensity: f32) -> Result<Bound<'py, PyArray4<f32>>> {
   let direction = direction.try_as_matrix().ok_or(
     anyhow!("light_source::directional_envmap: `direction` expected shape {:?}, found {:?}", [3], direction.shape()))?;
   let envmap = directional_envmap(resolution, direction, intensity)?;
-  Ok(envmap.to_pyarray(py).to_owned())
+  Ok(envmap.into_pyarray_bound(py))
 }
```

### Comparing `libredr-0.0.17/client/src/light_source/functional.rs` & `libredr-0.0.18/client/src/light_source/functional.rs`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/client/src/light_source.rs` & `libredr-0.0.18/client/src/light_source.rs`

 * *Files 17% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 /// Functional light source models (Rust)
 pub use self::functional::functional_envmap;
 
 /// Directional light source models (Rust and Python)
 pub use self::directional::{directional_envmap, py_directional_envmap};
 
 /// All light source models (Python)
-pub fn py_light_source(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
-  let module = PyModule::new(py, "light_source")?;
-  module.add_function(wrap_pyfunction!(py_directional_envmap, module)?)?;
-  parent_module.add_submodule(module)?;
+pub fn py_light_source<'py>(py: Python<'py>, parent_module: &Bound<'py, PyModule>) -> PyResult<()> {
+  let module = PyModule::new_bound(py, "light_source")?;
+  module.add_function(wrap_pyfunction!(py_directional_envmap, &module)?)?;
+  parent_module.add_submodule(&module)?;
   Ok(())
 }
```

### Comparing `libredr-0.0.17/README.md` & `libredr-0.0.18/client/README.md`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/Cargo.lock` & `libredr-0.0.18/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42cd52102d3df161c77a887b608d7a4897d7cc112886a9537b738a887a03aaff"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
 version = "0.2.16"
@@ -58,17 +58,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.12"
+version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b09b5178381e0874812a9b157f7fe84982617e48f71f4e3235482775e5b540"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "utf8parse",
@@ -106,17 +106,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "approx"
 version = "0.5.1"
@@ -158,23 +158,23 @@
 checksum = "8cf2bce30dfe09ef0bfaef228b9d414faaf7e563035494d7fe092dba54b300f4"
 dependencies = [
  "critical-section",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -185,126 +185,126 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blake3"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0231f06152bf547e9c2b5194f247cd97aacf6dcd8b15d8e5ec0663f64580da87"
+checksum = "30cca6d3674597c30ddf2c587bf8d9d65c9a84d2326d941cc79c9842dfe0ef52"
 dependencies = [
  "arrayref",
  "arrayvec",
  "cc",
  "cfg-if",
  "constant_time_eq",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a994c2b3ca201d9b263612a374263f05e7adde37c4707f693dcd375076d1f"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.34"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits 0.2.18",
  "wasm-bindgen",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "cl-sys"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4febd824a957638c066180fbf72b2bed5bcee33740773f3dc59fe91f0a3e6595"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck",
+ "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -391,17 +391,17 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.11"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -464,28 +464,28 @@
 checksum = "be4551092f4d519593039259a9ed8daedf0da12e5109c5280338073eaeb81180"
 dependencies = [
  "num-traits 0.1.43",
 ]
 
 [[package]]
 name = "event-listener"
-version = "5.1.0"
+version = "5.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7ad6fd685ce13acd6d9541a30f6db6567a7a24c9ffd4ba2955d29e3f22c8b27"
+checksum = "6d9944b8ca13534cdfb2800775f8dd4902ff3fc75a50101466decadfdf322a24"
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener-strategy"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "feedafcaa9b749175d5ac357452a9d41ea2911da598fde46ce1fe02c37751291"
+checksum = "332f51cb23d20b0de8458b86580878211da09bcd4503cb579c225b3d124cabb3"
 dependencies = [
  "event-listener",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "form_urlencoded"
@@ -506,36 +506,36 @@
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
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
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "git2"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b3ba52851e73b46a4c3df1d89343741112003f0f6f13beb0dfac9e457c3fdcd"
+checksum = "232e6a7bfe35766bf715e55a88b39a700596c0ccfd88cd3680b4cdb40d66ef70"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
@@ -575,18 +575,24 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
@@ -615,44 +621,44 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "is_debug"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06d198e9919d9822d5f7083ba8530e04de87841eaf21ead9af8f2304efd57c89"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
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
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -675,15 +681,15 @@
  "libc",
  "libz-sys",
  "pkg-config",
 ]
 
 [[package]]
 name = "libredr-client"
-version = "0.0.17"
+version = "0.0.18"
 dependencies = [
  "anyhow",
  "hashbrown",
  "libredr-common",
  "nalgebra",
  "ndarray",
  "numpy",
@@ -692,15 +698,15 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "libredr-common"
-version = "0.0.17"
+version = "0.0.18"
 dependencies = [
  "anyhow",
  "blake3",
  "chrono",
  "configparser",
  "const_format",
  "hashbrown",
@@ -714,15 +720,15 @@
  "tokio",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "libredr-server"
-version = "0.0.17"
+version = "0.0.18"
 dependencies = [
  "anyhow",
  "async-channel",
  "chrono",
  "clap",
  "const_format",
  "hashbrown",
@@ -731,15 +737,15 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "libredr-worker"
-version = "0.0.17"
+version = "0.0.18"
 dependencies = [
  "aho-corasick",
  "anyhow",
  "blake3",
  "chrono",
  "clap",
  "const_format",
@@ -753,17 +759,17 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.15"
+version = "1.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "037731f5d3aaa87a5675e895b63ddff1a87624bc29f77004ea829809654e48f6"
+checksum = "5e143b5e666b2695d28f6bca6497720813f699c9602dd7f5cac91008b8ada7f9"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -775,17 +781,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
@@ -800,23 +806,23 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
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
 name = "miniz_oxide"
 version = "0.7.2"
@@ -824,28 +830,28 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nalgebra"
-version = "0.32.3"
+version = "0.32.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307ed9b18cc2423f29e83f84fd23a8e73628727990181f18641a8b5dc2ab1caa"
+checksum = "3ea4908d4f23254adda3daa60ffef0f1ac7b8c3e9a864cf3cc154b251908a2ef"
 dependencies = [
  "approx",
  "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits 0.2.18",
@@ -964,17 +970,17 @@
 checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "nalgebra",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits 0.2.18",
@@ -989,17 +995,17 @@
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "ocl"
-version = "0.19.6"
+version = "0.19.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1c3ce118fd2f00eeb3c01f8073db1ee127cac0b2f79848192c7889b2bd7fe40"
+checksum = "4297afb442d411793e4e24ee5a2977d15b6c95c743418f1c0ce0a2397d7ec8a3"
 dependencies = [
  "futures",
  "nodrop",
  "num-traits 0.2.18",
  "ocl-core",
  "qutex",
  "thiserror",
@@ -1081,25 +1087,31 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "postcard"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a55c51ee6c0db07e68448e336cf8ea4131a620edefebf9893e759b2d793420f8"
 dependencies = [
  "cobs",
  "embedded-io",
@@ -1117,97 +1129,99 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "anyhow",
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
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.49",
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
 name = "qutex"
-version = "0.2.4"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda4a51ba3d773c196f9450a6b239077ad8dda608b15263b4c9f29e58909883f"
+checksum = "11778238e7d8b0e3ca62033fdc69e01ef5cdb08809cdc2398b2ce5ec873a1757"
 dependencies = [
  "crossbeam",
  "futures",
 ]
 
 [[package]]
 name = "rand"
@@ -1243,17 +1257,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1272,55 +1286,55 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.4.5",
- "regex-syntax 0.8.2",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.8.2",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
@@ -1352,43 +1366,43 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.21"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "shadow-rs"
-version = "0.26.1"
+version = "0.27.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e5c5c8276991763b44ede03efaf966eaa0412fafbf299e6380704678ca3b997"
+checksum = "7960cbd6ba74691bb15e7ebf97f7136bd02d1115f5695a58c1f31d5645750128"
 dependencies = [
  "const_format",
  "git2",
  "is_debug",
  "time",
  "tzdb",
 ]
@@ -1422,26 +1436,26 @@
  "num-traits 0.2.18",
  "paste",
  "wide",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -1453,71 +1467,71 @@
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
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
-version = "2.0.49"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "915aea9e586f80826ee59f8453c1101f9d1c4b3964cd2460185ee8e299ada496"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tikv-jemalloc-sys"
@@ -1537,17 +1551,17 @@
 dependencies = [
  "libc",
  "tikv-jemalloc-sys",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "libc",
  "num-conv",
  "num_threads",
  "powerfmt",
@@ -1560,17 +1574,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
@@ -1585,26 +1599,26 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tobj"
-version = "4.0.1"
+version = "4.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f7ca3ec0405b0f2f95e0dbcced28882190dc79b0dac63ff82533d256d770223"
+checksum = "c3bd4ba05f29e4c65b6c0c11a58b6465ffa820bac890d76ad407b4e81d8372e8"
 dependencies = [
  "ahash",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -1619,15 +1633,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
@@ -1641,15 +1655,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1732,17 +1746,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
@@ -1770,33 +1784,33 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
  "rand",
  "serde",
  "uuid-macro-internal",
 ]
 
 [[package]]
 name = "uuid-macro-internal"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7abb14ae1a50dad63eaa768a458ef43d298cd1bd44951677bd10b732a9ba2a2d"
+checksum = "9881bea7cbe687e36c9ab3b778c36cd0487402e270304e8b1296d5085303c1a2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
@@ -1817,65 +1831,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wide"
 version = "0.7.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
 dependencies = [
@@ -1907,15 +1921,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -1925,15 +1939,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1945,110 +1959,110 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "zerocopy"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
@@ -2059,9 +2073,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.58",
 ]
```

### Comparing `libredr-0.0.17/Cargo.toml` & `libredr-0.0.18/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["common", "client"]
 resolver = "2"
 
 [workspace.package]
-version = "0.0.17"
+version = "0.0.18"
 edition = "2021"
 authors = ["Bohan Yu"]
 description = "LibreDR is an open-source ray-tracing differentiable renderer"
 documentation = "https://ybh1998.codeberg.page/LibreDR/"
 homepage = "https://codeberg.org/ybh1998/LibreDR/"
 readme = "README.md"
 license = "AGPL-3.0-or-later"
@@ -24,23 +24,23 @@
 ocl = "0.19"
 chrono = "0.4"
 once_cell = "1"
 tracing = "0.1"
 nalgebra = "0.32"
 aho-corasick = "1"
 configparser = "3"
-shadow-rs = "0.26"
+shadow-rs = "0.27"
 async-channel = "2"
 const_format = "0.2"
 tokio = { version = "1", features = ["full"] }
 clap = { version = "4", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
 anyhow = { version = "1", features = ["backtrace"] }
 ndarray = { version = "0.15", features = ["serde"] }
 postcard = { version = "1", features = ["use-std"] }
-numpy = { version = "0.20", features = ["nalgebra"] }
+numpy = { version = "0.21", features = ["nalgebra"] }
 hashbrown = { version = "0.14", features = ["serde"] }
-pyo3 = { version = "0.20", features = ["abi3-py37", "anyhow"] }
+pyo3 = { version = "0.21", features = ["abi3-py37", "anyhow"] }
 tracing-subscriber = { version = "0.3", features = ["env-filter"] }
 uuid = { version = "1", features = ["v4", "fast-rng", "macro-diagnostics", "serde"] }
 tikv-jemallocator = { version = "0.5", features = ["background_threads", "disable_initial_exec_tls"] }
-common = { package = "libredr-common", path = "common", version = "0.0.17" }
+common = { package = "libredr-common", path = "common", version = "0.0.18" }
```

### Comparing `libredr-0.0.17/pyproject.toml` & `libredr-0.0.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/torch/nn/functional.py` & `libredr-0.0.18/python/libredr/torch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/torch/light_source/__init__.py` & `libredr-0.0.18/python/libredr/torch/light_source/__init__.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/torch/ray_tracing.py` & `libredr-0.0.18/python/libredr/torch/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/__init__.py` & `libredr-0.0.18/python/libredr/__init__.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/camera/cube.py` & `libredr-0.0.18/python/libredr/camera/cube.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/camera/perspective.py` & `libredr-0.0.18/python/libredr/camera/perspective.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/python/libredr/camera/equirectangular.py` & `libredr-0.0.18/python/libredr/camera/equirectangular.py`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/LICENSE` & `libredr-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `libredr-0.0.17/PKG-INFO` & `libredr-0.0.18/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: libredr
-Version: 0.0.17
+Version: 0.0.18
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Dist: numpy
 Requires-Dist: torch ; extra == 'torch'
 Provides-Extra: torch
```

