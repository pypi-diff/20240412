# Comparing `tmp/zeroset-0.0.2.tar.gz` & `tmp/zeroset-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroset-0.0.2.tar", last modified: Wed Apr 10 08:46:43 2024, max compression
+gzip compressed data, was "zeroset-0.0.3.tar", last modified: Fri Apr 12 07:55:17 2024, max compression
```

## Comparing `zeroset-0.0.2.tar` & `zeroset-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.747323 zeroset-0.0.2/
--rw-rw-rw-   0        0        0      821 2024-04-10 08:46:43.747323 zeroset-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-12-14 09:12:56.000000 zeroset-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 08:46:43.747323 zeroset-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-04-10 08:06:37.000000 zeroset-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.708570 zeroset-0.0.2/test/
--rw-rw-rw-   0        0        0      170 2024-04-10 07:45:29.000000 zeroset-0.0.2/test/test_cv0.py
--rw-rw-rw-   0        0        0      231 2023-07-23 05:21:32.000000 zeroset-0.0.2/test/test_glob.py
--rw-rw-rw-   0        0        0     1070 2023-12-17 10:16:05.000000 zeroset-0.0.2/test/test_script.py
--rw-rw-rw-   0        0        0     3666 2023-12-14 11:18:25.000000 zeroset-0.0.2/test/test_tabulate.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.732263 zeroset-0.0.2/zeroset/
--rw-rw-rw-   0        0        0      373 2024-04-03 06:30:00.000000 zeroset-0.0.2/zeroset/__init__.py
--rw-rw-rw-   0        0        0     8067 2024-04-10 07:48:24.000000 zeroset-0.0.2/zeroset/cv0.py
--rw-rw-rw-   0        0        0      844 2023-08-31 14:08:59.000000 zeroset-0.0.2/zeroset/fmt0.py
--rw-rw-rw-   0        0        0     5888 2024-04-10 08:02:20.000000 zeroset-0.0.2/zeroset/l0.py
--rw-rw-rw-   0        0        0     2160 2023-12-14 11:32:37.000000 zeroset-0.0.2/zeroset/py0.py
--rw-rw-rw-   0        0        0     3760 2024-02-15 14:22:09.000000 zeroset-0.0.2/zeroset/s0.py
-drwxrwxrwx   0        0        0        0 2024-04-10 08:46:43.746216 zeroset-0.0.2/zeroset.egg-info/
--rw-rw-rw-   0        0        0      821 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 08:46:43.000000 zeroset-0.0.2/zeroset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.322929 zeroset-0.0.3/
+-rw-rw-rw-   0        0        0      821 2024-04-12 07:55:17.322929 zeroset-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-12-14 09:12:56.000000 zeroset-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:55:17.322929 zeroset-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-04-10 12:55:35.000000 zeroset-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.284467 zeroset-0.0.3/test/
+-rw-rw-rw-   0        0        0      204 2024-04-10 13:06:04.000000 zeroset-0.0.3/test/test_cv0.py
+-rw-rw-rw-   0        0        0      231 2023-07-23 05:21:32.000000 zeroset-0.0.3/test/test_glob.py
+-rw-rw-rw-   0        0        0     1070 2023-12-17 10:16:05.000000 zeroset-0.0.3/test/test_script.py
+-rw-rw-rw-   0        0        0     3666 2023-12-14 11:18:25.000000 zeroset-0.0.3/test/test_tabulate.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.309511 zeroset-0.0.3/zeroset/
+-rw-rw-rw-   0        0        0      373 2024-04-03 06:30:00.000000 zeroset-0.0.3/zeroset/__init__.py
+-rw-rw-rw-   0        0        0     8935 2024-04-10 12:58:17.000000 zeroset-0.0.3/zeroset/cv0.py
+-rw-rw-rw-   0        0        0      844 2023-08-31 14:08:59.000000 zeroset-0.0.3/zeroset/fmt0.py
+-rw-rw-rw-   0        0        0     5888 2024-04-10 08:02:20.000000 zeroset-0.0.3/zeroset/l0.py
+-rw-rw-rw-   0        0        0     2160 2023-12-14 11:32:37.000000 zeroset-0.0.3/zeroset/py0.py
+-rw-rw-rw-   0        0        0     3760 2024-02-15 14:22:09.000000 zeroset-0.0.3/zeroset/s0.py
+-rw-rw-rw-   0        0        0    40729 2024-04-12 07:53:45.000000 zeroset-0.0.3/zeroset/v0.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.321929 zeroset-0.0.3/zeroset.egg-info/
+-rw-rw-rw-   0        0        0      821 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/top_level.txt
```

### Comparing `zeroset-0.0.2/PKG-INFO` & `zeroset-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroset
-Version: 0.0.2
+Version: 0.0.3
 Summary: Useful collection of features.
 Home-page: https://github.com/springkim/zeroset
 Author: Bomm Kim
 Author-email: springnode@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zeroset-0.0.2/setup.py` & `zeroset-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="zeroset",
-        version="0.0.2",
+        version="0.0.3",
         author="Bomm Kim",
         author_email="springnode@gmail.com",
         description="Useful collection of features.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/springkim/zeroset",
         packages=setuptools.find_packages(),
```

### Comparing `zeroset-0.0.2/test/test_script.py` & `zeroset-0.0.3/test/test_script.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/test/test_tabulate.py` & `zeroset-0.0.3/test/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/zeroset/cv0.py` & `zeroset-0.0.3/zeroset/cv0.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,20 @@
     return base64.b64encode(cv2.imencode(ext, img, params)[1]).decode("utf-8")
 
 
 def to_bytes(img: np.ndarray, ext: str = ".png"):
     return cv2.imencode(ext, img)[1].tobytes()
 
 
+def to_color(img: np.ndarray):
+    if len(img.shape) == 2 or img.shape[2] == 1:
+        img = cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
+    return img
+
+
 def imread(filename: str, flags=cv2.IMREAD_COLOR):
     return cv2.imdecode(np.fromfile(filename, np.uint8), flags)
 
 
 def imwrite(filename: str, img: np.ndarray, params=None):
     r, eimg = cv2.imencode(os.path.splitext(filename)[1], img, params)
     if r:
@@ -230,18 +236,40 @@
             imgs.append(arg)
         else:
             pass
     return imgs
 
 
 def hconcat(*args):
+    """
+    Return the input images horizontally.
+    :param args: opencv image list OR comma seperated images
+    :return: opencv image
+    """
     imgs = _to_image_list(args)
     max_height = max(img.shape[0] for img in imgs)
-    rimgs = [resize(img, height=max_height) for img in imgs]
+    rimgs = [to_color(resize(img, height=max_height)) for img in imgs]
     return cv2.hconcat(rimgs)
 
 
 def vconcat(*args):
+    """
+    Return the input images vertically.
+    :param args: opencv image list OR comma seperated images
+    :return: opencv image
+    """
     imgs = _to_image_list(args)
     max_width = max(img.shape[1] for img in imgs)
-    rimgs = [resize(img, width=max_width) for img in imgs]
+    rimgs = [to_color(resize(img, width=max_width)) for img in imgs]
     return cv2.vconcat(rimgs)
+
+
+def canny(img: np.ndarray):
+    if len(img.shape) == 3:
+        if img.shape[2] == 3:
+            img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+        elif img.shape[2] == 4:
+            img = cv2.cvtColor(img, cv2.COLOR_BGRA2GRAY)
+
+    high_th, _ = cv2.threshold(img, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+    low_th = high_th / 2
+    return cv2.Canny(img, low_th, high_th)
```

### Comparing `zeroset-0.0.2/zeroset/fmt0.py` & `zeroset-0.0.3/zeroset/fmt0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/zeroset/l0.py` & `zeroset-0.0.3/zeroset/l0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/zeroset/py0.py` & `zeroset-0.0.3/zeroset/py0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/zeroset/s0.py` & `zeroset-0.0.3/zeroset/s0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.2/zeroset.egg-info/PKG-INFO` & `zeroset-0.0.3/zeroset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroset
-Version: 0.0.2
+Version: 0.0.3
 Summary: Useful collection of features.
 Home-page: https://github.com/springkim/zeroset
 Author: Bomm Kim
 Author-email: springnode@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

