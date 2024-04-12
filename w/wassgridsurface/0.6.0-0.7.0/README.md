# Comparing `tmp/wassgridsurface-0.6.0.tar.gz` & `tmp/wassgridsurface-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-5v42hc9l/wassgridsurface-0.6.0.tar", last modified: Fri Apr 21 17:47:16 2023, max compression
+gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-36y3l1ge/wassgridsurface-0.7.tar", last modified: Fri Apr 12 19:57:42 2024, max compression
```

## Comparing `wassgridsurface-0.6.0.tar` & `wassgridsurface-0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.6.0/.gitignore
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/BUILD.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.6.0/environment.yml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-01-12 09:58:42.000000 wassgridsurface-0.6.0/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/wassgridsurface/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4947 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/DCTInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.6.0/wassgridsurface/IDWInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.6.0/wassgridsurface/TFVariationalRefinement.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.6.0/wassgridsurface/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.6.0/wassgridsurface/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6083 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/netcdfoutput.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.6.0/wassgridsurface/wass_utils.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    25343 2023-04-21 17:45:17.000000 wassgridsurface-0.6.0/wassgridsurface/wassgridsurface.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2023-04-21 17:47:16.101683 wassgridsurface-0.6.0/wassgridsurface.egg-info/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1651 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2023-04-21 17:47:16.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2023-04-21 17:47:15.000000 wassgridsurface-0.6.0/wassgridsurface.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.856318 wassgridsurface-0.7/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.7/.gitignore
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-05-09 15:56:57.000000 wassgridsurface-0.7/BUILD.md
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-12 19:57:42.856318 wassgridsurface-0.7/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-05-09 15:56:57.000000 wassgridsurface-0.7/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.7/environment.yml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-05-09 15:56:57.000000 wassgridsurface-0.7/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-12 19:57:42.856318 wassgridsurface-0.7/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.852318 wassgridsurface-0.7/wassgridsurface/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4947 2023-05-09 15:56:57.000000 wassgridsurface-0.7/wassgridsurface/DCTInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.7/wassgridsurface/IDWInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.7/wassgridsurface/TFVariationalRefinement.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.7/wassgridsurface/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.7/wassgridsurface/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6200 2024-04-12 15:10:55.000000 wassgridsurface-0.7/wassgridsurface/netcdfoutput.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.7/wassgridsurface/wass_utils.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    26002 2024-04-12 19:33:14.000000 wassgridsurface-0.7/wassgridsurface/wassgridsurface.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.856318 wassgridsurface-0.7/wassgridsurface.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/top_level.txt
```

### Comparing `wassgridsurface-0.6.0/PKG-INFO` & `wassgridsurface-0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.6.0
+Version: 0.7.0
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: torch
+Requires-Dist: matplotlib
+Requires-Dist: colorama
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: opencv-python>=2.4.6
+Requires-Dist: netcdf4
 
 # wassgridsurface
 ---
 
 wassgridsurface is a tool to interpolate into a uniform grid the scattered
 point clouds produced by [WASS](https://sites.google.com/unive.it/wass).
```

### Comparing `wassgridsurface-0.6.0/README.md` & `wassgridsurface-0.7/README.md`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/pyproject.toml` & `wassgridsurface-0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/DCTInterpolator.py` & `wassgridsurface-0.7/wassgridsurface/DCTInterpolator.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/IDWInterpolator.py` & `wassgridsurface-0.7/wassgridsurface/IDWInterpolator.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/TFVariationalRefinement.py` & `wassgridsurface-0.7/wassgridsurface/TFVariationalRefinement.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/__init__.py` & `wassgridsurface-0.7/wassgridsurface/__init__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/__main__.py` & `wassgridsurface-0.7/wassgridsurface/__main__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/netcdfoutput.py` & `wassgridsurface-0.7/wassgridsurface/netcdfoutput.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,27 +109,29 @@
     def set_mask( self, maskZ ):
         if self.rootgrp == None:
             return
 
         self.maskZ[:] = maskZ
 
 
-    def set_instrinsics( self, K0, K1, kc0, kc1, P0plane ):
+    def set_instrinsics( self, K0, K1, kc0, kc1, P0plane, P1plane ):
         if self.rootgrp == None:
             return
 
         self.metagrp.createDimension( "V3", 3 )
         self.metagrp.createDimension( "V4", 4 )
         self.metagrp.createDimension( "DistV", 5 )
         K0v = self.metagrp.createVariable("intr0", "f8", ("V3","V3") )
         K0v[:] = K0
         K1v = self.metagrp.createVariable("intr1", "f8", ("V3","V3") )
         K1v[:] = K1
         _P0plane = self.metagrp.createVariable("P0plane", "f8", ("V4","V4") )
         _P0plane[:] = P0plane
+        _P1plane = self.metagrp.createVariable("P1plane", "f8", ("V4","V4") )
+        _P1plane[:] = P1plane
         kc0v = self.metagrp.createVariable("dist0", "f8", ("DistV") )
         kc0v[:] = kc0
         kc1v = self.metagrp.createVariable("dist1", "f8", ("DistV") )
         kc1v[:] = kc1
 
     # def push_Z( self, Zdata, time ):
     #     if self.rootgrp != None:
```

### Comparing `wassgridsurface-0.6.0/wassgridsurface/wass_utils.py` & `wassgridsurface-0.7/wassgridsurface/wass_utils.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.6.0/wassgridsurface/wassgridsurface.py` & `wassgridsurface-0.7/wassgridsurface/wassgridsurface.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
-VERSION = "0.6.0"
+VERSION = "0.7.0"
 
 
 import argparse
 import configparser
 import scipy.io as sio
 import scipy.interpolate
 import os
@@ -81,14 +81,15 @@
     toNorm = np.array( [[ 2.0/Iw, 0     , -1, 0],
                         [ 0     , 2.0/Ih, -1, 0],
                         [ 0,      0,       1, 0],
                         [ 0,      0,       0, 1]], dtype=float )
 
     SCALEi = 1.0/baseline
     P0plane = toNorm @ P0Cam @ RTplane @ np.diag((SCALEi,SCALEi,-SCALEi, 1))
+    P1plane = toNorm @ P1Cam @ RTplane @ np.diag((SCALEi,SCALEi,-SCALEi, 1))
 
     area_size_m_x = np.floor( area_size_x / 2)
     area_size_m_y = np.floor( area_size_y / 2)
     xmin = area_center[0]-area_size_m_x
     xmax = area_center[0]+area_size_m_x
     ymin = area_center[1]-area_size_m_y
     ymax = area_center[1]+area_size_m_y
@@ -150,14 +151,15 @@
         "Ny":Ny,
         "N":np.amax([Nx,Ny]),
         "R":R,
         "T":T,
         "Rpl":Rpl,
         "Tpl":Tpl,
         "P0plane":P0plane,
+        "P1plane":P1plane,
         "CAM_BASELINE":baseline,
         "scale":baseline,
         "XX":XX,
         "YY":YY,
         "KX_ab":KX_ab,
         "KY_ab":KY_ab,
         "spec_scale":spec_scale,
@@ -165,16 +167,15 @@
         "y_spacing":y_spacing,
         "fps":fps,
         "timestring":timestring
     } )
 
 
 
-def grid( wass_frames, matfile, outdir, subsample_percent=100, mf=0, algorithm="DCT", user_mask_filename=None, alg_options=None, NUM_PARALLEL_PROCESSES=1 ):
-    step=150
+def grid( wass_frames, matfile, outdir, subsample_percent=100, mf=0, algorithm="DCT", user_mask_filename=None, alg_options=None, NUM_PARALLEL_PROCESSES=1, image_id_to_save=0 ):
     gridsetup = sio.loadmat( matfile )
     XX = gridsetup["XX"]
     YY = gridsetup["YY"]
 
     Rpl = gridsetup["Rpl"]
     Tpl = gridsetup["Tpl"]
     Rp2c = Rpl.T
@@ -183,29 +184,32 @@
     P0cam = gridsetup["P0cam"]
     P1cam = gridsetup["P1cam"]
 
     outdata = NetCDFOutput( filename=path.join(outdir,"gridded.nc" ), M=XX.shape[0], N=XX.shape[1] )
     baseline = gridsetup["CAM_BASELINE"].item(0)
 
     fps = gridsetup["fps"].item(0)
+    stereo_image_index = image_id_to_save
 
     outdata.scale[:] = baseline
     outdata.add_meta_attribute("info", "Generated with WASS gridder v.%s"%VERSION )
     outdata.add_meta_attribute("generator", "WASS" )
     outdata.add_meta_attribute("baseline", baseline )
     outdata.add_meta_attribute("fps", fps)
+    outdata.add_meta_attribute("stereo_image_index", stereo_image_index)
     outdata.add_meta_attribute("timestring", gridsetup["timestring"] )
     outdata.set_grids( XX*1000.0, YY*1000.0 )
     outdata.set_kxky( gridsetup["KX_ab"], gridsetup["KY_ab"] )
 
     outdata.set_instrinsics( np.zeros( (3,3), dtype=np.float32),
                              np.zeros( (3,3), dtype=np.float32),
                              np.zeros( (5,1), dtype=np.float32),
                              np.zeros( (5,1), dtype=np.float32),
-                             gridsetup["P0plane"])
+                             gridsetup["P0plane"],
+                             gridsetup["P1plane"])
 
 
     wass_frames_with_indices = [ x for x in enumerate(wass_frames) ]
     N_frames = len( wass_frames_with_indices )
 
 
     user_mask = np.ones( XX.shape, dtype=np.float32 )
@@ -414,20 +418,20 @@
         # Zi now contains the interpolated surface
 
         Zmeans.append( np.nanmean(Zi) )
         Zmins.append( np.nanmin(Zi) )
         Zmaxs.append( np.nanmax(Zi) )
 
 
-        I0 = cv.imread( path.join(wdir,"00000000_s.png"))
+        I0 = cv.imread( path.join(wdir,"%08d_s.png"%image_id_to_save))
         outdata.add_meta_attribute("image_width", I0.shape[1] )
         outdata.add_meta_attribute("image_height", I0.shape[0] )
         ret, imgjpeg = cv.imencode(".jpg", I0 )
 
-        mask_filename = path.join( wdir, "undistorted", "mask0.png" ) 
+        mask_filename = path.join( wdir, "undistorted", "mask%d.png"%image_id_to_save ) 
         imagemask = None
         if path.exists( mask_filename ): 
             with open( mask_filename, "rb" ) as f:
                 imagemask = np.fromfile(f, np.uint8 );
 
         outdata.push_Z( Zi*1000, float(idx)/float(fps) if fps>0 else 0.0, FRAME_IDX, imgjpeg, imagemask, idx=idx )
 
@@ -504,14 +508,15 @@
     parser.add_argument("-Ih", "--image_height", type=float, help="Camera frame height" )
     parser.add_argument("--ss", "--subsample_percent", type=float, default=100, help="Point subsampling 0..100%%" )
     parser.add_argument("--mf", "--medianfilter", type=int, default=0, help="Median filter window size (0,3,5,7)" )
     parser.add_argument("-n", "--num_frames", type=int, default=-1, help="Number of frames to process. -1 to process all frames." )
     parser.add_argument("-p", "--parallel", type=int, default=1, help="Number of parallel tasks to execute" )
     parser.add_argument("--ia", "--interpolation_algorithm", type=str, default="DCT", help='Interpolation algorithm to use. Alternatives are: "DCT", "IDW", "LinearND" ' )
     parser.add_argument("--mask", type=str, default=None, help='User supplied grid mask filename. Must be a grayscale (bw) image with the same size of the grid' )
+    parser.add_argument("--stereo_image_idx", type=int, default=0, help='Which stereo frame to store in the NetCDF, 0 or 1' )
     parser.add_argument("--dct_nfreqs", type=int, default=None, help="DCT interpolator number of frequencies" )
     parser.add_argument("--dct_regalpha", type=float, default=None, help="DCT interpolator regularizer alpha" )
     parser.add_argument("--dct_maxtol", type=float, default=None, help="DCT interpolator max function tolerance change" )
     parser.add_argument("--dct_lr", type=float, default=None, help="DCT interpolator learning rate" )
     parser.add_argument("--dct_maxiters", type=int, default=None, help="DCT interpolator max number of iterations" )
     args = parser.parse_args()
 
@@ -600,14 +605,19 @@
                fps=args.fps,
                timestring=args.timestring )
 
     elif args.action == "grid":
 
         if args.gridsetup is None:
             print("Grid setup file not specified. See --gridsetup option")
+            sys.exit(-1)
+
+        if args.stereo_image_idx > 1 or args.stereo_image_idx < 0:
+            print("--stereo_image_idx must be 0 or 1")
+            sys.exit(-1)
 
         grid( wass_frames,
               matfile=args.gridsetup,
               outdir=args.outdir,
               mf=args.mf,
               subsample_percent=args.ss,
               algorithm=args.ia,
@@ -615,16 +625,17 @@
               alg_options = {
                   "Nfreqs": args.dct_nfreqs,
                   "REGULARIZER_ALPHA": args.dct_regalpha,
                   "MAX_ITERS": args.dct_maxiters,
                   "TOLERANCE_CHANGE": args.dct_maxtol,
                   "LEARNING_RATE": args.dct_lr,
                   },
-              NUM_PARALLEL_PROCESSES=args.parallel )
+              NUM_PARALLEL_PROCESSES=args.parallel,
+              image_id_to_save=args.stereo_image_idx)
 
         print("Gridding completed.")
 
     else:
-        print("Invalid actions specified.")
+        print("Invalid action specified.")
         sys.exit(-2)
```

### Comparing `wassgridsurface-0.6.0/wassgridsurface.egg-info/PKG-INFO` & `wassgridsurface-0.7/wassgridsurface.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.6.0
+Version: 0.7.0
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: torch
+Requires-Dist: matplotlib
+Requires-Dist: colorama
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: opencv-python>=2.4.6
+Requires-Dist: netcdf4
 
 # wassgridsurface
 ---
 
 wassgridsurface is a tool to interpolate into a uniform grid the scattered
 point clouds produced by [WASS](https://sites.google.com/unive.it/wass).
```

### Comparing `wassgridsurface-0.6.0/wassgridsurface.egg-info/SOURCES.txt` & `wassgridsurface-0.7/wassgridsurface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

