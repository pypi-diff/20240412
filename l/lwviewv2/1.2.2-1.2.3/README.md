# Comparing `tmp/lwviewv2-1.2.2-py3-none-any.whl.zip` & `tmp/lwviewv2-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27463 bytes, number of entries: 12
+Zip file size: 27567 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 13:02 lwviewv2/__init__.py
--rw-r--r--  2.0 unx     8039 b- defN 24-Mar-19 17:18 lwviewv2/landmark.py
+-rw-r--r--  2.0 unx     8629 b- defN 24-Apr-12 15:12 lwviewv2/landmark.py
 -rw-r--r--  2.0 unx     1091 b- defN 24-Mar-19 17:18 lwviewv2/lw_babel.py
 -rw-r--r--  2.0 unx     6985 b- defN 22-Oct-25 20:11 lwviewv2/lw_image.py
 -rw-r--r--  2.0 unx     1797 b- defN 24-Mar-19 17:18 lwviewv2/lw_nrrd.py
 -rw-r--r--  2.0 unx    43131 b- defN 24-Mar-15 20:11 lwviewv2/lw_view copy.py
--rw-r--r--  2.0 unx    58660 b- defN 24-Apr-10 13:35 lwviewv2/lw_view.py
+-rw-r--r--  2.0 unx    58671 b- defN 24-Apr-11 14:11 lwviewv2/lw_view.py
 -rw-r--r--  2.0 unx      285 b- defN 24-Mar-14 21:01 lwviewv2/util.py
--rw-r--r--  2.0 unx      618 b- defN 24-Apr-10 13:38 lwviewv2-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 13:38 lwviewv2-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-10 13:38 lwviewv2-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      912 b- defN 24-Apr-10 13:38 lwviewv2-1.2.2.dist-info/RECORD
-12 files, 121619 bytes uncompressed, 25949 bytes compressed:  78.7%
+-rw-r--r--  2.0 unx      618 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      912 b- defN 24-Apr-12 15:12 lwviewv2-1.2.3.dist-info/RECORD
+12 files, 122220 bytes uncompressed, 26053 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: lwviewv2/lw_view.py
 Comment: 
 
 Filename: lwviewv2/util.py
 Comment: 
 
-Filename: lwviewv2-1.2.2.dist-info/METADATA
+Filename: lwviewv2-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: lwviewv2-1.2.2.dist-info/WHEEL
+Filename: lwviewv2-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: lwviewv2-1.2.2.dist-info/top_level.txt
+Filename: lwviewv2-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lwviewv2-1.2.2.dist-info/RECORD
+Filename: lwviewv2-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lwviewv2/landmark.py

```diff
@@ -119,28 +119,30 @@
         # also 'correct' the landmark list correspondingly
         elif cmd == 'DC':
             p0 = od.MLwVw.lw_view_wgts[0].get_focus_xyz()
             p1 = od.MLwVw.lw_view_wgts[1].get_focus_xyz()
             disp = p1 - p0
             displace_img(od.MLwVw.lw_view_wgts[0].input_img, disp)
             print('displacing image: {}'.format(disp))
+            od.MLwVw.lw_view_wgts[0].image_slicer.focus_previous = np.array([-1,-1,-1])
             od.MLwVw.lw_view_wgts[0].update_images()
             od.MLwVw.lw_view_wgts[0].update_canvases()
             correction_offset += disp
             pnts_0 = list(map(lambda pnt: add(pnt, correction_offset), pnts_0))
         # Displacement Correct (hacks image 1 (the 'left' image) affine)
         # displaces by average displacement of landmarks
         # also 'correct' the landmark list correspondingly
         elif cmd == 'DCA':
             if n == 0:
                 print('no landmarks in list')
             else:
                 avg_disp = (sum(pnts_1) - sum(pnts_0)) / n
                 displace_img(od.MLwVw.lw_view_wgts[0].input_img, avg_disp)
                 print('displacing image: {}'.format(avg_disp))
+                od.MLwVw.lw_view_wgts[0].image_slicer.focus_previous = np.array([-1,-1,-1])
                 od.MLwVw.lw_view_wgts[0].update_images()
                 od.MLwVw.lw_view_wgts[0].update_canvases()
                 correction_offset += avg_disp
                 pnts_0 = list(map(lambda pnt: add(pnt, correction_offset), pnts_0))
         # show reticles
         elif cmd == 'R':
             od.MLwVw.lw_view_wgts[0].reticles_on()
@@ -148,14 +150,21 @@
         elif cmd == 'r':
             od.MLwVw.lw_view_wgts[0].reticles_off()
             od.MLwVw.lw_view_wgts[1].reticles_off()
 
         # Help
         elif cmd == 'h':
             print_help()
+            
+        # update the current landmark pair to be the current cursors
+        elif cmd == 'U':   
+            p0 = od.MLwVw.lw_view_wgts[0].get_focus_xyz()
+            p1 = od.MLwVw.lw_view_wgts[1].get_focus_xyz()
+            pnts_0[i] = p0
+            pnts_1[i] = p1
         # write left image out
         elif cmd[0] == 'w':
             fn = cmd.split()[1]
             print('saving image file {}...'.format(fn))
             img = od.MLwVw.lw_view_wgts[0].input_img
             nb.save(img, fn)
             print('done')
@@ -182,25 +191,28 @@
         return(None)
 
 # destructively translate an image by hacking it's affine
 def displace_img(img, displacement): # displacement is rowvec
     img.affine[0,3] += displacement[0]
     img.affine[1,3] += displacement[1]
     img.affine[2,3] += displacement[2]
+    
+    img.inv_affine = npl.inv(img.affine)
 
     
 def print_help():
     print('<an integer> : goto that item in landmark list')
     print('n: next item')
     print('p: previous item')
     print('a: append current foci to landmark list')
     # print('i: insert current foci into landmark list')
     print('d: delete current item in landmark list')
     print('l: lock the foci')
     print('u: unlock the foci')
+    print('U: update the current landmark pair to the current cursors')
     print('D: print current focus displacement')
     print('DA: print average displacement over landmark list')
     print('DC: displacement correct the left image by current difference between foci')
     print('DCA: displacement correct the left image by current average displacement of landmark list')
     print('R: show reticles')
     print("r: don't show reticles")
     print('q: quit')
```

## lwviewv2/lw_view.py

```diff
@@ -17,14 +17,15 @@
 import platform
 import scipy.ndimage as spndi
 import tkinter as tk
 from PIL import Image
 from PIL import ImageTk
 import lwviewv2.lw_image as lwi
 import sys
+import copy
 
 # creates a viewer object
 
 class LwView:
     def __init__(self, *args, **kwargs):
         if len(args) == 0:
             print('nothing to display?')
@@ -245,15 +246,15 @@
 # parent is the parent 'widget'
 class LwViewW:
     def __init__(self, input_img, parent, root, mm_per_pixel, reticles, interpolation_order):
        self.focus_hook = False
        self.show_green_dot = True
        self.show_reticles = reticles
        self.interpolation_order=interpolation_order
-       self.input_img = input_img  
+       self.input_img = input_img
        self.root = root
        # make a virtual image that has scaled identity affine
        # slices are taken from the virtual image by interpolating from
        # input_img
        self.rect_v_img = lwi.make_rectified_container(self.input_img, mm_per_pixel)
        self.image_slicer = VirtualImageSlicer(self.rect_v_img, self.input_img, self.interpolation_order)       
        #
```

## Comparing `lwviewv2-1.2.2.dist-info/METADATA` & `lwviewv2-1.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lwviewv2
-Version: 1.2.2
+Version: 1.2.3
 Summary: Viewer of images in python.
 Home-page: https://github.com/ReubenDo/lightweight-viewer
 Author: Sandy Wells
 Author-email: sw@bwh.harvard.edu
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

## Comparing `lwviewv2-1.2.2.dist-info/RECORD` & `lwviewv2-1.2.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lwviewv2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lwviewv2/landmark.py,sha256=PfqnFYSka8pPF4zAM9M9L57YKZtDh4hcdgB_YZVH_yc,8039
+lwviewv2/landmark.py,sha256=i-WZxHsCm0CpWhh7Opcfm0-eH6BhZZIx_Yz-Es9fIQA,8629
 lwviewv2/lw_babel.py,sha256=H84MF8uh4ADDiWK9e56iedtPdM3qGvbpTVDCpb_lLhQ,1091
 lwviewv2/lw_image.py,sha256=LH6hCzmyvssVseI0dM2gNkoN8XunDLBd84TTXtLFMiA,6985
 lwviewv2/lw_nrrd.py,sha256=2LxfO86sbjAbLyDKY41uPtrN7x6j6QUVhBv30_RsThM,1797
 lwviewv2/lw_view copy.py,sha256=A_4gWXB0SzufNiS-67erhvuF8y2qYYk0PSp0nvXnoRE,43131
-lwviewv2/lw_view.py,sha256=JQ75_Xw9ULLJecV1V4iOPjN-Cp19NW3Pgsgmcg5RVV0,58660
+lwviewv2/lw_view.py,sha256=2yJD1OR4eFis5wzmSq22oxsivTiUDBae-csuBCu650k,58671
 lwviewv2/util.py,sha256=pTAX578rsDylPGfFEHew73-3578bp4GSVbnnNKTA-U0,285
-lwviewv2-1.2.2.dist-info/METADATA,sha256=5b81oQtSt6_mO5yk93AOARc1_6iBVoSYnzFMJTs010s,618
-lwviewv2-1.2.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-lwviewv2-1.2.2.dist-info/top_level.txt,sha256=UBxEML6xSOAmiPwcH66C4QPfPW3Bid1w25rLoIdLKLM,9
-lwviewv2-1.2.2.dist-info/RECORD,,
+lwviewv2-1.2.3.dist-info/METADATA,sha256=GlwFJEe1Vaw1wP9cxysACJx2OQNTtj4_jtP7VYzf6OA,618
+lwviewv2-1.2.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+lwviewv2-1.2.3.dist-info/top_level.txt,sha256=UBxEML6xSOAmiPwcH66C4QPfPW3Bid1w25rLoIdLKLM,9
+lwviewv2-1.2.3.dist-info/RECORD,,
```

