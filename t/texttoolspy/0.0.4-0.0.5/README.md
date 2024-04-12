# Comparing `tmp/texttoolspy-0.0.4-py3-none-any.whl.zip` & `tmp/texttoolspy-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3539 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     2129 b- defN 24-Apr-09 18:37 texttoolspy/__init__.py
+Zip file size: 3678 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     2141 b- defN 24-Apr-12 20:39 texttoolspy/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 20:02 texttoolspy/main.py
--rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-10 17:56 texttoolspy-0.0.4.dist-info/Licence.txt
--rw-rw-rw-  2.0 fat     1264 b- defN 24-Apr-10 17:56 texttoolspy-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 17:56 texttoolspy-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-10 17:56 texttoolspy-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      563 b- defN 24-Apr-10 17:56 texttoolspy-0.0.4.dist-info/RECORD
-7 files, 5143 bytes uncompressed, 2535 bytes compressed:  50.7%
+-rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-12 20:41 texttoolspy-0.0.5.dist-info/Licence.txt
+-rw-rw-rw-  2.0 fat     1624 b- defN 24-Apr-12 20:41 texttoolspy-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 20:41 texttoolspy-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-12 20:41 texttoolspy-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      563 b- defN 24-Apr-12 20:41 texttoolspy-0.0.5.dist-info/RECORD
+7 files, 5515 bytes uncompressed, 2674 bytes compressed:  51.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: texttoolspy/__init__.py
 Comment: 
 
 Filename: texttoolspy/main.py
 Comment: 
 
-Filename: texttoolspy-0.0.4.dist-info/Licence.txt
+Filename: texttoolspy-0.0.5.dist-info/Licence.txt
 Comment: 
 
-Filename: texttoolspy-0.0.4.dist-info/METADATA
+Filename: texttoolspy-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: texttoolspy-0.0.4.dist-info/WHEEL
+Filename: texttoolspy-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: texttoolspy-0.0.4.dist-info/top_level.txt
+Filename: texttoolspy-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: texttoolspy-0.0.4.dist-info/RECORD
+Filename: texttoolspy-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## texttoolspy/__init__.py

```diff
@@ -11,25 +11,25 @@
 
 def write(letter, speed):
   stdout.write(letter)
   stdout.flush()
   if letter != " ":
     sleep(0.01 * speed)
   
-def type(string=None, speed=5, LineBreak=True):
+def typewriter(string=None, speed=5, LineBreak=True):
   cursor.hide()
   if string == None:
     print("TypeError: missing 'string'")
   else:
     for x in range(0,len(string)):
       write(string[x], speed)
     if LineBreak == True:
       print("  ")
     cursor.show()
-def typeColored(string=None, speed=5, color="white", LineBreak = True):
+def typewriterColored(string=None, color="white", speed=5, LineBreak = True):
   cursor.hide()
   if string == None:
     print("TypeError: missing 'string'")
   try:
     for x in range(0, len(string)):
       write(colored(string[x], color.lower()), speed)
     if LineBreak == True:
```

## Comparing `texttoolspy-0.0.4.dist-info/Licence.txt` & `texttoolspy-0.0.5.dist-info/Licence.txt`

 * *Files identical despite different names*

## Comparing `texttoolspy-0.0.4.dist-info/METADATA` & `texttoolspy-0.0.5.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: texttoolspy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool that allows you to create responsive tools in text
 Author: MilesWK
 Author-email: your_name@example.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 Requires-Dist: termcolor
 Requires-Dist: colorama
 Requires-Dist: readchar
 Requires-Dist: cursor
 
 # texttoolspy 0.0.4
+
+[![PyPI version](https://badge.fury.io/py/texttoolspy.svg)](https://badge.fury.io/py/texttoolspy)
+[![PyPI - Status](https://img.shields.io/pypi/status/texttoolspy.svg)](https://pypi.org/project/texttoolspy/)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
 Tools to make responsive and simple items in text.
 
 **How to install:**
 ```bash
 pip install texttoolspy
 ```
```

