# Comparing `tmp/bblib-1.1.3.tar.gz` & `tmp/bblib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-1.1.3.tar", max compression
+gzip compressed data, was "bblib-1.2.0.tar", max compression
```

## Comparing `bblib-1.1.3.tar` & `bblib-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-02-28 22:07:39.600299 bblib-1.1.3/LICENSE
--rw-r--r--   0        0        0     3753 2024-02-28 22:07:39.600299 bblib-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-02-28 22:07:39.600299 bblib-1.1.3/bblib/__init__.py
--rwxr-xr-x   0        0        0    34456 2024-02-28 22:07:39.600299 bblib-1.1.3/bblib/methods.py
--rwxr-xr-x   0        0        0     8691 2024-02-28 22:07:39.600299 bblib-1.1.3/bblib/models.py
--rwxr-xr-x   0        0        0    19287 2024-02-28 22:07:39.600299 bblib-1.1.3/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-02-28 22:07:54.088188 bblib-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-04-12 16:41:40.239125 bblib-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3753 2024-04-12 16:41:40.239125 bblib-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/__init__.py
+-rwxr-xr-x   0        0        0    35521 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/methods.py
+-rwxr-xr-x   0        0        0     9185 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/models.py
+-rwxr-xr-x   0        0        0    19615 2024-04-12 16:41:40.239125 bblib-1.2.0/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-04-12 16:41:49.919210 bblib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-1.2.0/PKG-INFO
```

### Comparing `bblib-1.1.3/LICENSE` & `bblib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-1.1.3/README.md` & `bblib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bblib-1.1.3/bblib/methods.py` & `bblib-1.2.0/bblib/methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from skimage.transform import hough_circle, hough_circle_peaks
 from skimage.feature import canny
 import multiprocessing
 import pathlib
 from scipy.optimize import curve_fit
-
+from matplotlib.colors import LogNorm
 
 class CenteringMethod(ABC):
     @abstractmethod
     def __init__(self, **kwargs) -> None: ...
 
     @abstractmethod
     def _prep_for_centering(self, **kwargs) -> None: ...
@@ -50,14 +50,21 @@
         self.PF8Config = PF8Config
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
+        if not config["plots_flag"] and not plots_info:
+            plots_info =  {
+	        "file_name": "",
+	        "folder_name": "",
+	        "root_path": ""
+            }
+
     def _prep_for_centering(self, data: np.ndarray) -> None:
         self.initial_detector_center = self.PF8Config.get_detector_center()
         pf8 = PF8(self.PF8Config)
         peak_list = pf8.get_peaks_pf8(data=data)
         peak_list_x_in_frame, peak_list_y_in_frame = pf8.peak_list_in_slab(peak_list)
         row_indexes = np.zeros(peak_list["num_peaks"], dtype=int)
         col_indexes = np.zeros(peak_list["num_peaks"], dtype=int)
@@ -109,15 +116,15 @@
             center[0] += self.config["offset"]["x"]
             center[1] += self.config["offset"]["y"]
 
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             ax1.imshow(
                 self.visual_data * self.mask_for_center_of_mass,
-                vmax=10,
+                norm=LogNorm(),
                 cmap="YlGn",
                 origin="lower",
             )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -149,14 +156,21 @@
         self.PF8Config = PF8Config
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
+        if not config["plots_flag"] and not plots_info:
+            plots_info =  {
+	        "file_name": "",
+	        "folder_name": "",
+	        "root_path": ""
+            }
+
     def _prep_for_centering(self, data: np.ndarray) -> None:
         self.initial_detector_center = self.PF8Config.get_detector_center()
         ## Find peaks
         pf8 = PF8(self.PF8Config)
         peak_list = pf8.get_peaks_pf8(data=data)
         peak_list_x_in_frame, peak_list_y_in_frame = pf8.peak_list_in_slab(peak_list)
         row_indexes = np.zeros(peak_list["num_peaks"], dtype=int)
@@ -241,15 +255,15 @@
             yc = -1
 
         center = [xc, yc]
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             ax1.imshow(
                 self.visual_data * self.mask_for_circle_detection,
-                vmax=10,
+                norm=LogNorm(),
                 origin="lower",
                 cmap="YlGn",
             )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -282,14 +296,22 @@
         self.plots_info = plots_info
         self.plot_fwhm_flag = False
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
+        if not config["plots_flag"] and not plots_info:
+            plots_info =  {
+	        "file_name": "",
+	        "folder_name": "",
+	        "root_path": ""
+            }
+
+
     def _calculate_fwhm(self, coordinate: tuple) -> dict:
         center_to_radial_average = coordinate
         try:
             x_all, y_all = azimuthal_average(
                 self.visual_data,
                 center=center_to_radial_average,
                 mask=self.mask_for_fwhm_min,
@@ -371,24 +393,24 @@
             "fwhm": fwhm,
             "r_squared": r_squared,
         }
 
     def _prep_for_centering(self, data: np.ndarray, initial_guess: tuple) -> None:
         self.initial_guess = initial_guess
         self.initial_detector_center = self.PF8Config.get_detector_center()
+        non_shifted_pixel_maps_for_visualization = self.PF8Config.pixel_maps.copy()
         ## Find peaks
         self.PF8Config.update_pixel_maps(
             initial_guess[0] - self.initial_detector_center[0],
             initial_guess[1] - self.initial_detector_center[1],
         )
         pf8 = PF8(self.PF8Config)
-
         # Assemble data and mask
-        data_visualize = geometry.DataVisualizer(pixel_maps=self.PF8Config.pixel_maps)
-
+        data_visualize = geometry.DataVisualizer(pixel_maps=non_shifted_pixel_maps_for_visualization)
+        
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
         if self.config["polarization"]["skip"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
                 self.PF8Config.pf8_detector_info["nasics_x"]
@@ -510,15 +532,15 @@
             self._calculate_fwhm(center)
             self.plot_fwhm_flag = False
 
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             ax1.imshow(
                 self.visual_data * self.mask_for_fwhm_min,
-                vmax=10,
+                norm=LogNorm(),
                 origin="lower",
                 cmap="YlGn",
             )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -557,15 +579,21 @@
         self.config = config
         self.PF8Config = PF8Config
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
-
+        
+        if not config["plots_flag"] and not plots_info:
+            plots_info =  {
+	        "file_name": "",
+	        "folder_name": "",
+	        "root_path": ""
+            }
     def _remove_repeated_pairs(self, pairs_list: list) -> list:
         x_vector = []
         y_vector = []
         unique_pairs = []
 
         for pair in pairs_list:
             peak_0, peak_1 = pair
@@ -646,24 +674,26 @@
         else:
             return cut_peaks_list[0][0]
 
     def _prep_for_centering(self, data: np.ndarray, initial_guess: tuple) -> None:
 
         self.initial_guess = initial_guess
         self.initial_detector_center = self.PF8Config.get_detector_center()
+        non_shifted_pixel_maps_for_visualization = self.PF8Config.pixel_maps.copy()
+
         ## Find peaks
         self.PF8Config.update_pixel_maps(
             initial_guess[0] - self.initial_detector_center[0],
             initial_guess[1] - self.initial_detector_center[1],
         )
 
         pf8 = PF8(self.PF8Config)
 
         # Assemble data and mask
-        data_visualize = geometry.DataVisualizer(pixel_maps=self.PF8Config.pixel_maps)
+        data_visualize = geometry.DataVisualizer(pixel_maps=non_shifted_pixel_maps_for_visualization)
 
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
         if self.config["polarization"]["skip"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
@@ -716,17 +746,19 @@
                 visual_mask = visualize_single_panel(
                     mask,
                     self.PF8Config.transformation_matrix,
                     self.PF8Config.ss_in_rows,
                 )
 
         peak_list_in_slab = pf8.peak_list_in_slab(peak_list)
+        #print(peak_list_in_slab)
         self.peak_list_x_in_frame, self.peak_list_y_in_frame = peak_list_in_slab
 
     def _run_centering(self, **kwargs) -> tuple:
+       
         peak_list_x_in_frame = self.peak_list_x_in_frame.copy()
         peak_list_y_in_frame = self.peak_list_y_in_frame.copy()
 
         peaks = list(zip(peak_list_x_in_frame, peak_list_y_in_frame))
         inverted_peaks_x = [-1 * k for k in peak_list_x_in_frame]
         inverted_peaks_y = [-1 * k for k in peak_list_y_in_frame]
         inverted_peaks = list(zip(inverted_peaks_x, inverted_peaks_y))
@@ -769,21 +801,22 @@
             distance_summary,
             f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}',
             f'{self.plots_info["file_name"]}',
             self.pixel_step,
             self.config["plots_flag"],
         )
 
+
         if self.config["plots_flag"] and self.centering_converged(center):
             shift_x = 2 * (center[0] - self.initial_guess[0])
             shift_y = 2 * (center[1] - self.initial_guess[1])
 
-            fig, ax = plt.subplots(1, 1, figsize=(8, 8))
+            fig, ax = plt.subplots(1, 1, figsize=(10, 10))
             pos = ax.imshow(
-                self.visual_data, vmin=0, vmax=100, cmap="YlGn", origin="lower"
+                self.visual_data, norm=LogNorm(), cmap="YlGn", origin="lower"
             )
             ax.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="b",
                 marker="o",
                 s=25,
@@ -803,27 +836,27 @@
                 center[1],
                 color="r",
                 marker="o",
                 s=25,
                 label=f"Refined detector center:({np.round(center[0],1)}, {np.round(center[1],1)})",
             )
             ax.set_xlim(200, 900)
-            ax.set_ylim(900, 200)
+            ax.set_ylim(200, 900)
             plt.title("Center refinement: autocorrelation of Friedel pairs")
             fig.colorbar(pos, shrink=0.6)
             ax.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/{self.plots_info["file_name"]}.png'
             )
             plt.close("all")
-
+            
             original_peaks_x = [
                 np.round(k + self.initial_guess[0]) for k in peak_list_x_in_frame
             ]
             original_peaks_y = [
                 np.round(k + self.initial_guess[1]) for k in peak_list_y_in_frame
             ]
 
@@ -837,28 +870,29 @@
                 np.round(k + self.initial_guess[0] + shift_x) for k in inverted_peaks_x
             ]
             inverted_shifted_peaks_y = [
                 np.round(k + self.initial_guess[1] + shift_y) for k in inverted_peaks_y
             ]
 
             ## Check pairs alignement
-            fig, ax = plt.subplots(1, 1, figsize=(8, 8))
+            fig, ax = plt.subplots(1, 1, figsize=(10, 10))
             pos = ax.imshow(
-                self.visual_data, vmin=0, vmax=100, cmap="YlGn", origin="lower"
+                self.visual_data, norm=LogNorm(), cmap="YlGn", origin="lower"
             )
             ax.scatter(
                 original_peaks_x,
                 original_peaks_y,
                 facecolor="none",
                 s=80,
                 marker="s",
                 edgecolor="red",
                 linewidth=1.5,
                 label="original peaks",
             )
+            
             ax.scatter(
                 inverted_non_shifted_peaks_x,
                 inverted_non_shifted_peaks_y,
                 s=80,
                 facecolor="none",
                 marker="s",
                 edgecolor="tab:orange",
@@ -873,16 +907,17 @@
                 s=120,
                 marker="D",
                 linewidth=1.8,
                 alpha=0.8,
                 edgecolor="blue",
                 label="shift of inverted peaks",
             )
+            
             ax.set_xlim(200, 900)
-            ax.set_ylim(900, 200)
+            ax.set_ylim(200, 900)
             plt.title("Bragg peaks alignement")
             fig.colorbar(pos, shrink=0.6)
             ax.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/peaks/'
             )
             path.mkdir(parents=True, exist_ok=True)
```

### Comparing `bblib-1.1.3/bblib/models.py` & `bblib-1.2.0/bblib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     max_res: np.int16
     pf8_detector_info: TypeDetectorLayoutInformation = None
     bad_pixel_map_filename: str = None
     bad_pixel_map_hdf5_path: str = None
     pixel_maps: TypePixelMaps = None
     pixel_resolution: float = None
     _shifted_pixel_maps: bool = False
+    geometry_txt: list = None
 
     def update_pixel_maps(self, detector_shift_x: int, detector_shift_y: int):
         if not self._shifted_pixel_maps:
             self._detector_shift_x = detector_shift_x
             self._detector_shift_y = detector_shift_y
             self._shifted_pixel_maps = True
             self.pixel_maps["x"] = (
@@ -37,47 +38,53 @@
             ).reshape(self._data_shape)
             self.pixel_maps["y"] = (
                 self.pixel_maps["y"].flatten() - detector_shift_y
             ).reshape(self._data_shape)
             self.pixel_maps["radius"] = np.sqrt(
                 np.square(self.pixel_maps["x"]) + np.square(self.pixel_maps["y"])
             ).reshape(self._data_shape)
+            self.pixel_maps["phi"] = np.arctan2(self.pixel_maps["y"], self.pixel_maps["x"])
         else:
             raise ValueError(
                 f"Pixel maps have been moved once before, to avoid errors reset the geometry before moving it again."
             )
 
-    def set_geometry_from_file(self, geometry_filename: str):
-        geometry_txt = open(geometry_filename, "r").readlines()
+    def set_geometry_from_file(self, geometry_filename: str = None):
+        if geometry_filename:
+            self.geometry_txt = open(geometry_filename, "r").readlines()
+        else:
+            if not self.geometry_txt:
+                raise ValueError("Please, specify the detector geometry in CrystFEL format.")
+
         self.bad_pixel_map_filename = [
             x.split(" = ")[-1][:-1]
-            for x in geometry_txt
+            for x in self.geometry_txt
             if x.split(" = ")[0] == "mask_file"
         ][0]
         self.bad_pixel_map_hdf5_path = [
-            x.split(" = ")[-1][:-1] for x in geometry_txt if x.split(" = ")[0] == "mask"
+            x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask"
         ][0]
 
         geom = GeometryInformation(
-            geometry_description=geometry_txt, geometry_format="crystfel"
+            geometry_description=self.geometry_txt, geometry_format="crystfel"
         )
         self.pixel_resolution = 1 / geom.get_pixel_size()
         self.pixel_maps = geom.get_pixel_maps()
         self._data_shape = self.pixel_maps["x"].shape
         self._flattened_data_shape = self.pixel_maps["x"].flatten().shape[0]
         self.pf8_detector_info = geom.get_layout_info()
         self._shifted_pixel_maps = False
         self.detector_center_from_geom = self.get_detector_center()
 
         if (
             self.pf8_detector_info["nasics_x"] * self.pf8_detector_info["nasics_y"]
         ) == 1:
             ## Get single panel transformation matrix from the geometry file
             ### Warning! Check carefully if the visualized data after reorientation of the panel makes sense, e.g. if it is equal to the real experimental data geometry.
-            detector, _, _ = _read_crystfel_geometry_from_text(text_lines=geometry_txt)
+            detector, _, _ = _read_crystfel_geometry_from_text(text_lines=self.geometry_txt)
             detector_panels = dict(detector["panels"])
             panel_name = list(detector_panels.keys())[0]
             frame_dim_structure = [
                 x
                 for x in detector_panels[panel_name]["dim_structure"]
                 if x == "ss" or x == "fs"
             ]
@@ -128,14 +135,15 @@
         elif parameter == "bad_pixel_map_filename":
             return self.bad_pixel_map_filename
         elif parameter == "bad_pixel_map_hdf5_path":
             return self.bad_pixel_map_hdf5_path
 
     def get_detector_center(self) -> list:
         if not self._shifted_pixel_maps:
+            
             if (
                 self.pf8_detector_info["nasics_x"] * self.pf8_detector_info["nasics_y"]
                 > 1
             ):
                 # Multiple panels
                 # Get minimum array shape
                 y_minimum = (
@@ -163,14 +171,15 @@
                 _img_center_x = int(visual_img_shape[1] / 2)
                 _img_center_y = int(visual_img_shape[0] / 2)
             else:
                 # Single panel
                 _img_center_x = int(abs(np.min(self.pixel_maps["x"])))
                 _img_center_y = int(abs(np.min(self.pixel_maps["y"])))
         else:
+            print("Warning! The detector center was moved by a previous operation, the detector center is not the same as in the geometry file.")
             _img_center_x = self.detector_center_from_geom[0] + self._detector_shift_x
             _img_center_y = self.detector_center_from_geom[1] + self._detector_shift_y
         return [_img_center_x, _img_center_y]
 
 
 class PF8:
     def __init__(self, info):
```

### Comparing `bblib-1.1.3/bblib/utils.py` & `bblib-1.2.0/bblib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,20 @@
          coordinates of the diffraction center in x and y, such as the image center corresponds to data[yc, xc].
     """
 
     if mask is None:
         mask = np.ones_like(data)
     data = data * mask
     indexes = np.where(data > 0)
-    xc = np.sum(data[indexes] * indexes[1]) / np.sum(data[indexes])
-    yc = np.sum(data[indexes] * indexes[0]) / np.sum(data[indexes])
+    if np.sum(data[indexes])>1e-7:
+        xc = np.sum(data[indexes] * indexes[1]) / np.sum(data[indexes])
+        yc = np.sum(data[indexes] * indexes[0]) / np.sum(data[indexes])
+    else:
+        xc = -1
+        yc = -1
 
     if np.isnan(xc) or np.isnan(yc):
         xc = -1
         yc = -1
 
     return [np.round(xc, 1), np.round(yc, 1)]
 
@@ -405,38 +409,47 @@
     ax1.set_ylabel("yc [px]")
     ax1.set_xlabel("xc [px]")
     ax1.set_title("Distance [px]")
 
     proj_x = np.sum(z, axis=0)
     # print('proj',len(proj_x))
     x = np.arange(x[0], x[-1] + pixel_step, pixel_step)
+    
     # print('x',len(x))
-    index_x = np.unravel_index(np.argmin(proj_x, axis=None), proj_x.shape)
-    # print(index_x)
-    xc = x[index_x]
-    ax2.scatter(x, proj_x + pixel_step, color="b")
-    ax2.scatter(xc, proj_x[index_x], color="r", label=f"xc: {np.round(xc,1)}")
-    ax2.set_ylabel("Average distance [px]")
-    ax2.set_xlabel("xc [px]")
-    ax2.set_title("Distance projection in x")
-    ax2.legend()
+    if len(proj_x)==len(x):
+        index_x = np.unravel_index(np.argmin(proj_x, axis=None), proj_x.shape)
+        xc = x[index_x]
+        ax2.scatter(x, proj_x + pixel_step, color="b")
+        ax2.scatter(xc, proj_x[index_x], color="r", label=f"xc: {np.round(xc,1)}")
+        ax2.set_ylabel("Average distance [px]")
+        ax2.set_xlabel("xc [px]")
+        ax2.set_title("Distance projection in x")
+        ax2.legend()
+    else:
+        converged = 0
+        xc = -1
+        yc = -1
 
     proj_y = np.sum(z, axis=1)
     x = np.arange(y[0], y[-1] + pixel_step, pixel_step)
-    index_y = np.unravel_index(np.argmin(proj_y, axis=None), proj_y.shape)
-    yc = x[index_y]
-    ax3.scatter(x, proj_y, color="b")
-    ax3.scatter(yc, proj_y[index_y], color="r", label=f"yc: {np.round(yc,1)}")
-    ax3.set_ylabel("Average Distance [px]")
-    ax3.set_xlabel("yc [px]")
-    ax3.set_title("Distance projection in y")
-    ax3.legend()
-
-    fig.colorbar(pos1, ax=ax1, shrink=0.6)
-
+    if len(proj_y)==len(x):
+        index_y = np.unravel_index(np.argmin(proj_y, axis=None), proj_y.shape)
+        yc = x[index_y]
+        ax3.scatter(x, proj_y, color="b")
+        ax3.scatter(yc, proj_y[index_y], color="r", label=f"yc: {np.round(yc,1)}")
+        ax3.set_ylabel("Average Distance [px]")
+        ax3.set_xlabel("yc [px]")
+        ax3.set_title("Distance projection in y")
+        ax3.legend()
+        fig.colorbar(pos1, ax=ax1, shrink=0.6)
+    else:
+        converged = 0
+        xc = -1
+        yc = -1
+        
     if int(np.sum(proj_y)) == 0 or int(np.sum(proj_x)) == 0:
         converged = 0
         xc = -1
         yc = -1
     else:
         converged = 1
         if plots_flag:
```

### Comparing `bblib-1.1.3/pyproject.toml` & `bblib-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "1.1.3"
+version = "1.2.0"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-1.1.3/PKG-INFO` & `bblib-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 1.1.3
+Version: 1.2.0
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

