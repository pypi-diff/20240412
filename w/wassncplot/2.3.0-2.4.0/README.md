# Comparing `tmp/wassncplot-2.3.0.tar.gz` & `tmp/wassncplot-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-f86snpwr/wassncplot-2.3.0.tar", last modified: Mon Apr  8 09:43:21 2024, max compression
+gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-e0ircvrj/wassncplot-2.4.tar", last modified: Fri Apr 12 19:59:10 2024, max compression
```

## Comparing `wassncplot-2.3.0.tar` & `wassncplot-2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-08 09:43:21.719773 wassncplot-2.3.0/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.3.0/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.3.0/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-08 09:43:21.719773 wassncplot-2.3.0/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.715773 wassncplot-2.3.0/src/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.715773 wassncplot-2.3.0/src/wassncplot/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/waveview2.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/__init.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.3.0/src/wassncplot/wassncplot.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    10965 2024-04-08 09:42:58.000000 wassncplot-2.3.0/src/wassncplot/wassncplot2.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-08 09:43:21.719773 wassncplot-2.3.0/src/wassncplot.egg-info/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-08 09:43:21.000000 wassncplot-2.3.0/src/wassncplot.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:59:10.406988 wassncplot-2.4/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-12 19:59:10.406988 wassncplot-2.4/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.4/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.4/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-12 19:59:10.406988 wassncplot-2.4/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:59:10.402989 wassncplot-2.4/src/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:59:10.402989 wassncplot-2.4/src/wassncplot/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:59:10.402989 wassncplot-2.4/src/wassncplot/WaveFieldVisualize/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.4/src/wassncplot/WaveFieldVisualize/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.4/src/wassncplot/WaveFieldVisualize/waveview2.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.4/src/wassncplot/__init.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.4/src/wassncplot/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.4/src/wassncplot/wassncplot.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    11691 2024-04-12 19:41:19.000000 wassncplot-2.4/src/wassncplot/wassncplot2.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:59:10.406988 wassncplot-2.4/src/wassncplot.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-12 19:59:10.000000 wassncplot-2.4/src/wassncplot.egg-info/top_level.txt
```

### Comparing `wassncplot-2.3.0/PKG-INFO` & `wassncplot-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.3.0
+Version: 2.4.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wassncplot-2.3.0/README.md` & `wassncplot-2.4/README.md`

 * *Files identical despite different names*

### Comparing `wassncplot-2.3.0/pyproject.toml` & `wassncplot-2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassncplot-2.3.0/src/wassncplot/WaveFieldVisualize/waveview2.py` & `wassncplot-2.4/src/wassncplot/WaveFieldVisualize/waveview2.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.3.0/src/wassncplot/wassncplot.py` & `wassncplot-2.4/src/wassncplot/wassncplot.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.3.0/src/wassncplot/wassncplot2.py` & `wassncplot-2.4/src/wassncplot/wassncplot2.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from .WaveFieldVisualize.waveview2 import WaveView
 from tqdm import tqdm
 import sys
 import os
 import argparse
 import glob
 import scipy.io
-from scipy.interpolate import LinearNDInterpolator
+from scipy.interpolate import LinearNDInterpolator, CloughTocher2DInterpolator
 
 
-VERSION="2.3.0"
+VERSION="2.4.0"
 
 
 
 def wassncplot_main():
 
     print(" wassncplot v.", VERSION )
     print("=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\nCopyright (C) Filippo Bergamasco 2023 \n")
@@ -37,19 +37,19 @@
     parser.add_argument("--pxscale", default=1, type=int, help="A scale factor to apply between logical and physical pixels in addition to the actual scale factor determined by the backend. (default 1)")
     parser.add_argument("--text_prefix", default="", help="Bottom overlay text prefix")
     parser.add_argument("--zeromean", dest="zeromean", action="store_true", help="subtract the mean value of every grid point before rendering")
     parser.add_argument("--wireframe", dest="wireframe", action="store_true", help="Render surface in wireframe (default)")
     parser.add_argument("--upscale2x", dest="upscale2x", action="store_true", help="Upscale the input image before rendering")
     parser.add_argument("--applymask", dest="applymask", action="store_true", help="Apply user-defined mask if available")
     parser.add_argument("--no-wireframe", dest="wireframe", action="store_false", help="Render shaded surface")
-    parser.add_argument("--no-textoverlay", dest="textoverlay", action="store_false", help="Add text overlay at the bottom of the frame")
-    parser.add_argument("--savexyz", dest="savexyz", action="store_true", help="Save mapping between image pixels and 3D coordinates as a Matlab mat file")
-    parser.add_argument("--create-texture", dest="createtx", action="store_true", help="Compute sea surface radiance for each grid point and store it into the input NetCDF file.")
-    parser.add_argument("--save-texture", dest="savetx", action="store_true", help="Save each sea surface radiance texture to a png image (data is also stored in the NetCDF)")
-    parser.add_argument("--saveimg", dest="saveimg", action="store_true", help="Save the undistorted image (without the superimposed grid)")
+    parser.add_argument("--no-textoverlay", dest="textoverlay", action="store_false", help="Disable text overlay at the bottom of the frame")
+    parser.add_argument("--savexyz", dest="savexyz", action="store_true", help="Save mapping between image pixels and 3D coordinates as Matlab mat files")
+    parser.add_argument("--save-texture-in-netcdf", dest="createtx", action="store_true", help="Compute sea surface radiance for each grid point and store it into the input NetCDF file.")
+    parser.add_argument("--save-texture-in-img", dest="savetx", action="store_true", help="Compute sea surface radiance for each grid point and store it into a png image.")
+    parser.add_argument("--save-img", dest="saveimg", action="store_true", help="Save the undistorted image (without the superimposed grid)")
     parser.add_argument("--ffmpeg", dest="ffmpeg", action="store_true", help="Call ffmpeg to create a sequence video file")
     parser.add_argument("--gif", dest="gif", action="store_true", help="Create an animated GIF sequence")
     parser.add_argument("--ffmpeg-delete-frames", dest="ffmpegdelete", action="store_true", help="Delete the produced frames after running ffmpeg")
     parser.add_argument("--ffmpeg-fps", dest="ffmpeg_fps", default=10.0, type=float, help="Sequence framerate")
     parser.set_defaults(wireframe=True)
     args = parser.parse_args()
 
@@ -71,15 +71,30 @@
         print("Loading baseline from netcdf")
         stereo_baseline = rootgrp["scale"][0]
 
     print("Stereo baseline: ",stereo_baseline, " (use -b option to change)")
     XX = np.array( rootgrp["X_grid"] )/1000.0
     YY = np.array( rootgrp["Y_grid"] )/1000.0
     ZZ = rootgrp["Z"]
-    P0plane = np.array( rootgrp["meta"]["P0plane"] )
+
+
+    P0plane = None
+    P1plane = None
+    stereo_image_index = 0
+
+    if "P0plane" in rootgrp["meta"].variables:
+        P0plane = np.array( rootgrp["meta"]["P0plane"] )
+    if "P1plane" in rootgrp["meta"].variables:
+        P1plane = np.array( rootgrp["meta"]["P1plane"] )
+
+    if "stereo_image_index" in rootgrp["meta"].ncattrs():
+        stereo_image_index = rootgrp["meta"].stereo_image_index
+
+    print("Rendering frames from camera %d"%stereo_image_index )
+
     nframes = ZZ.shape[0]
 
     Iw, Ih = rootgrp["meta"].image_width, rootgrp["meta"].image_height
 
     if args.zmin is None:
         try:
             args.zmin = rootgrp["meta"].zmin
@@ -176,50 +191,54 @@
         #mask = (ZZ_data == 0.0)
         #ZZ_dil = cv.dilate( ZZ_data, np.ones((3,3)))
         #ZZ_data[mask]=ZZ_dil
 
         img, img_xyz = waveview.render( I0, ZZ_data )
 
         #%%
-        if args.createtx:
-            if not "radiance" in rootgrp.variables:
-                radiance = rootgrp.createVariable("radiance","u8",( rootgrp.dimensions["count"], 
-                                                                    rootgrp.dimensions["X"], 
-                                                                    rootgrp.dimensions["Y"]),
-                                                                    fill_value=0 )
-                radiance.long_name = "Sea surface radiance for each grid point"
-
-
+        if args.createtx or args.savetx:
             interp = LinearNDInterpolator( np.reshape( img_xyz[:,:,0:2], [-1,2]), I0.flatten(), 0 )
+            #interp = CloughTocher2DInterpolator( np.reshape( img_xyz[:,:,0:2], [-1,2]), I0.flatten(), 0 )
             tx = interp( XX, YY ).astype( np.uint8 )
 
-            # Add texture to NetCDF
-            (rootgrp["radiance"])[image_idx,:,:] = np.expand_dims( tx, axis=0 )
+            if args.createtx:
+                if not "radiance" in rootgrp.variables:
+                    radiance = rootgrp.createVariable("radiance","u8",( rootgrp.dimensions["count"], 
+                                                                        rootgrp.dimensions["X"], 
+                                                                        rootgrp.dimensions["Y"]),
+                                                                        fill_value=0 )
+                    radiance.long_name = "Sea surface radiance for each grid point"
+
+
+                (rootgrp["radiance"])[image_idx,:,:] = np.expand_dims( tx, axis=0 )
+
 
             # Optional: save to a png image
             if args.savetx:
                 cv.imwrite( "%s/radiance_%08d.png"%(outdir,image_idx), tx )
 
 
-        
-
 
         #%% 
 
         if args.savexyz:
-            scipy.io.savemat( '%s/%08d.mat'%(outdir,image_idx), {"px_2_3D": img_xyz} )
+            scipy.io.savemat( '%s/%08d.mat'%(outdir,image_idx), {"px_2_3D": img_xyz}, do_compression=True )
 
         img = (img*255).astype( np.uint8 )
         img = (I0mask>0)*img + ((I0mask==0)*np.expand_dims(I0, axis=-1))
         img = cv.cvtColor( img, cv.COLOR_RGB2BGR )
 
         if args.textoverlay:
-            img[(img.shape[0]-20):,:,:] //= 3
-            img[(img.shape[0]-20):,:,:] *= 2
-            cv.putText( img, "%s frame %d"%(args.text_prefix,image_idx), (5,img.shape[0]-5), cv.FONT_HERSHEY_DUPLEX, 0.5, color=(255,255,255))
+            dark_area_h = int(45.0/2048.0*img.shape[0])
+
+            img[(img.shape[0]-dark_area_h):,:,:] //= 3
+            img[(img.shape[0]-dark_area_h):,:,:] *= 2
+
+            texth = 1.5/2048*img.shape[0]
+            cv.putText( img, "%s Frame %d"%(args.text_prefix,image_idx), (5,img.shape[0]-5), cv.FONT_HERSHEY_DUPLEX, texth, color=(255,255,255))
 
         cv.imwrite('%s/%08d_grid.png'%(outdir,image_idx), img )
 
         if output_image_size is None:
             output_image_size = (img.shape[1],img.shape[0])
 
         if args.saveimg:
```

### Comparing `wassncplot-2.3.0/src/wassncplot.egg-info/PKG-INFO` & `wassncplot-2.4/src/wassncplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.3.0
+Version: 2.4.0
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

