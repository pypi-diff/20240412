# Comparing `tmp/gixpy-1.3.tar.gz` & `tmp/gixpy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gixpy-1.3.tar", last modified: Thu Apr 11 03:20:01 2024, max compression
+gzip compressed data, was "gixpy-1.4.tar", last modified: Thu Apr 11 15:01:50 2024, max compression
```

## Comparing `gixpy-1.3.tar` & `gixpy-1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:01.971228 gixpy-1.3/
--rw-rw-rw-   0        0        0      433 2024-04-11 03:20:01.969230 gixpy-1.3/PKG-INFO
--rw-rw-rw-   0        0        0    21235 2024-04-11 03:19:30.000000 gixpy-1.3/gixpy.c
-drwxrwxrwx   0        0        0        0 2024-04-11 03:20:01.965226 gixpy-1.3/gixpy.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 03:20:01.000000 gixpy-1.3/gixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2024-04-11 03:19:20.000000 gixpy-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 03:20:01.972227 gixpy-1.3/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-04-11 03:19:24.000000 gixpy-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:01:50.761292 gixpy-1.4/
+-rw-rw-rw-   0        0        0      433 2024-04-11 15:01:50.756793 gixpy-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21502 2024-04-11 14:33:37.000000 gixpy-1.4/gixpy.c
+drwxrwxrwx   0        0        0        0 2024-04-11 15:01:50.746159 gixpy-1.4/gixpy.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-11 15:01:50.000000 gixpy-1.4/gixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-04-11 15:01:50.000000 gixpy-1.4/gixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 15:01:50.000000 gixpy-1.4/gixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 15:01:50.000000 gixpy-1.4/gixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2024-04-11 14:01:21.000000 gixpy-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 15:01:50.762294 gixpy-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-04-11 14:01:21.000000 gixpy-1.4/setup.py
```

### Comparing `gixpy-1.3/gixpy.c` & `gixpy-1.4/gixpy.c`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     to_pixel = 1. / pixel_size;
     
     struct Geometry geometry = {
         .beam_center_x = beam_center_x * to_pixel,
         .beam_center_y = (double)rows - beam_center_y * to_pixel,
         .det_dist = det_dist * to_pixel,
         .incident_angle = incident_angle * DEG2RAD,
-        .tilt_angle = incident_angle * DEG2RAD,
+        .tilt_angle = tilt_angle * DEG2RAD,
         .rows = rows,
         .columns = columns
     };
 
     struct Point2D* r_arr = (struct Point2D*)malloc((im_size) * sizeof(struct Point2D));
     if (r_arr == NULL) {
         PyErr_SetString(PyExc_ValueError, "Failed to allocate memory for distances for transform.");
@@ -374,15 +374,17 @@
     new_beam_center->y = DBL_MIN;
     double min_x = DBL_MAX;
     double min_y = DBL_MAX;
     double det_dist_sq = geo->det_dist * geo->det_dist;
     //int64_t last_index;
     //int64_t index = 0;
 
-    if (geo->tilt_angle != 0.0) {
+    printf("%.10f\n", geo->tilt_angle);
+    printf("%d, %d\n", geo->tilt_angle > 1e-6, geo->tilt_angle < -1e-6);
+    if (geo->tilt_angle > 1e-6 || geo->tilt_angle < -1e-6) {
         tilt_cos = cos(geo->tilt_angle);
         tilt_sin = sin(geo->tilt_angle);
         for (size_t rr = 0; rr < geo->rows; ++rr) {
             for (size_t cc = 0; cc < geo->columns; ++cc) {
                 x_pos = x[cc] * tilt_cos - y[rr] * tilt_sin;
                 y_pos = y[rr] * tilt_cos + x[cc] * tilt_sin;
                 hori_travel_sq = det_dist_sq + x_pos * x_pos;
@@ -402,15 +404,17 @@
                 if (r_z > new_beam_center->y) { new_beam_center->y = r_z; }
                 if (r_xy < min_x) { min_x = r_xy; }
                 if (r_z < min_y) { min_y = r_z; }
                 r_ii->x = r_xy;
                 r_ii++->y = r_z;
             }
         }
-    } else {
+    }
+    else {
+        size_t image_size = geo->rows * geo->columns;
         for (size_t cc = 0; cc < geo->columns; ++cc) {
             x_pos = x[cc];
             hori_travel_sq = det_dist_sq + x_pos * x_pos;
             sin_phi = x_pos / sqrt(hori_travel_sq);
             cos_phi = sqrt(1 - sin_phi * sin_phi);
             for (size_t rr = 0; rr < geo->rows; ++rr) {
                 y_pos = y[rr];
@@ -426,17 +430,17 @@
                 r_z = q_z * q_scaler;
                 if (r_xy > new_beam_center->x) { new_beam_center->x = r_xy; }
                 if (r_z > new_beam_center->y) { new_beam_center->y = r_z; }
                 if (r_xy < min_x) { min_x = r_xy; }
                 if (r_z < min_y) { min_y = r_z; }
                 r_ii->x = r_xy;
                 r_ii->y = r_z;
-                r_ii += geo->columns;
+                r_ii += geo->columns;   // move down one in current column
             }
-            r_ii += 1 - geo->columns;
+            r_ii += 1 - image_size;     // move to top of next column
         }
     }
     new_image_shape->cols = ceil(new_beam_center->x - min_x) + 1;
     new_image_shape->rows = ceil(new_beam_center->y - min_y) + 1;
     free(x);
     free(y);
     return 1;
```

### Comparing `gixpy-1.3/pyproject.toml` & `gixpy-1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gixpy"
-version = "1.3"
+version = "1.4"
 authors = [
   { name="Teddy Tortorici", email="edward.tortorici@colorado.edu" },
 ]
 description = "Transform GIWAXS images"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `gixpy-1.3/setup.py` & `gixpy-1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         'C:\\Users\\Teddy\\AppData\\Roaming\\Python\\Python39\\site-packages\\numpy\\core\\include'],
     library_dirs=["\\root\\project"],
     language="c",
 )
 
 setup(
     name='gixpy',
-    version="1.3",
+    version="1.4",
     description="Python package to quickly transform GIWAXS images using C",
     long_description="Visit github.com/etortorici/gixpy for details",
     author_email='edward.tortorici@colorado.edu',
     license='GPL',
     ext_modules=[gp_module],
     install_requires=["numpy"],
 )
```

