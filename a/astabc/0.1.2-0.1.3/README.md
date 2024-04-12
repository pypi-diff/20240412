# Comparing `tmp/astabc-0.1.2.tar.gz` & `tmp/astabc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astabc-0.1.2.tar", last modified: Fri Apr 12 08:05:51 2024, max compression
+gzip compressed data, was "astabc-0.1.3.tar", last modified: Fri Apr 12 08:07:15 2024, max compression
```

## Comparing `astabc-0.1.2.tar` & `astabc-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:05:51.105134 astabc-0.1.2/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.2/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:05:51.105134 astabc-0.1.2/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.2/README.md
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:05:51.101134 astabc-0.1.2/astabc/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.2/astabc/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2338 2024-04-12 08:02:03.000000 astabc-0.1.2/astabc/astabc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:05:51.101134 astabc-0.1.2/astabc.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       46 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-12 08:05:51.000000 astabc-0.1.2/astabc.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-12 08:05:51.105134 astabc-0.1.2/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      729 2024-04-12 08:05:48.000000 astabc-0.1.2/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:05:51.101134 astabc-0.1.2/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.2/tests/test_astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:07:15.736661 astabc-0.1.3/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-04-12 07:46:41.000000 astabc-0.1.3/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:07:15.736661 astabc-0.1.3/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      701 2024-04-12 07:32:42.000000 astabc-0.1.3/README.md
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:07:15.736661 astabc-0.1.3/astabc/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       58 2024-04-12 07:32:31.000000 astabc-0.1.3/astabc/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2274 2024-04-12 08:06:59.000000 astabc-0.1.3/astabc/astabc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:07:15.736661 astabc-0.1.3/astabc.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1149 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      265 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       46 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        7 2024-04-12 08:07:15.000000 astabc-0.1.3/astabc.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-04-12 08:07:15.736661 astabc-0.1.3/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      729 2024-04-12 08:07:13.000000 astabc-0.1.3/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-12 08:07:15.736661 astabc-0.1.3/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1313 2024-04-12 07:32:38.000000 astabc-0.1.3/tests/test_astabc.py
```

### Comparing `astabc-0.1.2/LICENSE` & `astabc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astabc-0.1.2/PKG-INFO` & `astabc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.2/README.md` & `astabc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astabc-0.1.2/astabc/astabc.py` & `astabc-0.1.3/astabc/astabc.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     new_filename = output_filename if output_filename else filename.replace("." + file_extension, "_abc" + abc_fn_suffix + "." + file_extension)
     cv2.imwrite(new_filename, img)
     print("Brightness and contrast corrected image saved as", new_filename)
     
     return img, alpha, beta
 
 def main():
-    parser = argparse.ArgumentParser(description='Image Brightness and Contrast Correction')
-    parser.description('Image Brightness and Contrast Correction by Guillaume D. Isabelle, 2024')
+    parser = argparse.ArgumentParser(description='Image Brightness and Contrast Correction\nby Guillaume D. Isabelle, 2024\n')
     parser.add_argument('filename', type=str, help='input image filename')
     parser.add_argument('-a','--abc', type=int, default=15, help='automatic brightness and contrast percentage (default: 25)')
     parser.add_argument('-o','--output', type=str, help='output image filename')
     
     args = parser.parse_args()
     
     correct(args.filename, args.abc, args.output)
```

### Comparing `astabc-0.1.2/astabc.egg-info/PKG-INFO` & `astabc-0.1.3/astabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astabc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module for automatic brightness and contrast optimization
 Home-page: https://github.com/jgwill/gia-abc
 Author: Guillaume Descoteaux-Isabelle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `astabc-0.1.2/setup.py` & `astabc-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="astabc",
-    version="0.1.2",
+    version="0.1.3",
     author="Guillaume Descoteaux-Isabelle",
     description="A Python module for automatic brightness and contrast optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jgwill/gia-abc",
     packages=["astabc"],
     entry_points={
```

### Comparing `astabc-0.1.2/tests/test_astabc.py` & `astabc-0.1.3/tests/test_astabc.py`

 * *Files identical despite different names*

