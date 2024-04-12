# Comparing `tmp/vnav-0.3.1-py2.py3-none-any.whl.zip` & `tmp/vnav-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5427 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx     9600 b- defN 23-Apr-17 14:29 vnav-0.3.1.data/scripts/parse_vNav_Motion.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      286 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      471 b- defN 23-Apr-17 14:29 vnav-0.3.1.dist-info/RECORD
-6 files, 11525 bytes uncompressed, 4573 bytes compressed:  60.3%
+Zip file size: 5622 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx    10170 b- defN 24-Apr-12 21:42 vnav-0.4.0.data/scripts/parse_vNav_Motion.py
+-rw-r--r--  2.0 unx     1057 b- defN 24-Apr-12 21:42 vnav-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      286 b- defN 24-Apr-12 21:42 vnav-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-12 21:42 vnav-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-12 21:42 vnav-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      472 b- defN 24-Apr-12 21:42 vnav-0.4.0.dist-info/RECORD
+6 files, 12096 bytes uncompressed, 4768 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: vnav-0.3.1.data/scripts/parse_vNav_Motion.py
+Filename: vnav-0.4.0.data/scripts/parse_vNav_Motion.py
 Comment: 
 
-Filename: vnav-0.3.1.dist-info/LICENSE
+Filename: vnav-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: vnav-0.3.1.dist-info/METADATA
+Filename: vnav-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: vnav-0.3.1.dist-info/WHEEL
+Filename: vnav-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: vnav-0.3.1.dist-info/top_level.txt
+Filename: vnav-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vnav-0.3.1.dist-info/RECORD
+Filename: vnav-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vnav-0.3.1.data/scripts/parse_vNav_Motion.py` & `vnav-0.4.0.data/scripts/parse_vNav_Motion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #!python
 
+import logging
 import pydicom as dicom
 import os
 import numpy as np
 import itertools
 import glob
 import argparse
 import json
 import re
 import matplotlib.pyplot as plt
 
+logger = logging.getLogger()
+logging.basicConfig(level=logging.INFO)
+
 def normalize(x):
   return x / np.sqrt(np.dot(x,x))
 
 def readRotAndTransFromDicom(paths):
+  failure = re.compile('^.*\? F:')
+  pattern = re.compile('.*R:\s+(.*?)\s+(.*?)\s+(.*?)\s+(.*?)\s+T:\s+(.*?)\s+(.*?)\s+(.*?)\s+F:.*')
+
   files = itertools.chain.from_iterable([glob.glob(path) for path in paths])
 
   # Sort DICOMs by AcquisitionNumber (important!)
   ds = sorted([dicom.read_file(x) for x in files], key=lambda dcm: dcm.AcquisitionNumber)
 
   failed = None
 
@@ -29,21 +36,29 @@
   for x in ds[1:]:
     instance = x.InstanceNumber
     acquisition = x.AcquisitionNumber
     '''
     vNav failures do not appear to be encoded consistently. The following regular
     expression was crafted based on a small number of examples.
     '''
-    if re.match('^.*\? F:', x.ImageComments):
-        print(f'failure detected instance={instance}, acquisition={acquisition}')
+    if failure.match(x.ImageComments):
+        logger.error(f'failure detected instance={instance}, acquisition={acquisition}')
         failed = (instance, acquisition)
         break
-    y = str.split(x.ImageComments)
-    rotation = np.array(list(map(float, y[1:5])))
-    translation = np.array(list(map(float, y[6:9])))
+    match = pattern.match(x.ImageComments)
+    if not match:
+        logger.critical(f'instance {instance} ImageComments failed pattern match')
+        logger.critical(x.ImageComments)
+        sys.exit(1)
+    R = match.groups(0)[0:4]
+    T = match.groups(0)[4:]
+    logger.debug(x.ImageComments)
+    logger.debug(f'R={R} and T={T}')
+    rotation = np.array(list(map(float, R)))
+    translation = np.array(list(map(float, T)))
     quaternions.append((rotation, translation))
 
   return quaternions,failed
 
 def readRotAndTransFromJson(js):
   '''
   vNav failures do not appear to be encoded consistently. The following regular
@@ -228,14 +243,17 @@
 parser.add_argument('--radius', type=float, default=100, help='radius (mm) of assumed sphere (default: %(default)s)')
 parser.add_argument('--plot', help='output plot of chosen measure across frames', action='store_true')
 parser.add_argument('-v','--verbose', help='increase output verbosity', action='store_true')
 parser.add_argument('--output-dir', default='.', help='output directory')
 
 args = parser.parse_args()
 
+if args.verbose:
+    logger.setLevel(logging.DEBUG)
+
 if args.rms is False and args.max is False:
   parser.error('At least one of --rms or --max is required.')
 
 if not os.path.exists(args.output_dir):
   os.makedirs(args.output_dir)
 
 summary = dict()
@@ -246,15 +264,15 @@
   for f in os.listdir(args.input_dir):
     f = os.path.join(args.input_dir, f)
     # only add valid dicom files from input directory
     try:
       with open(f, 'rb') as fo:
         dicom.filereader.read_preamble(fo, force=False)
     except dicom.errors.InvalidDicomError:
-      print(f'ignoring invalid dicom {f}')
+      logger.warning(f'ignoring invalid dicom {f}')
       continue
     args.input.append(f)
 
 if args.input_json:
   args.input_json = os.path.expanduser(args.input_json)
   with open(args.input_json, 'r') as fo:
     args.input_json = json.load(fo)
```

## Comparing `vnav-0.3.1.dist-info/LICENSE` & `vnav-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

