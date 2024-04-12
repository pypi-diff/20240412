# Comparing `tmp/zeroset-0.0.3.tar.gz` & `tmp/zeroset-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroset-0.0.3.tar", last modified: Fri Apr 12 07:55:17 2024, max compression
+gzip compressed data, was "zeroset-0.0.4.tar", last modified: Fri Apr 12 07:59:34 2024, max compression
```

## Comparing `zeroset-0.0.3.tar` & `zeroset-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.322929 zeroset-0.0.3/
--rw-rw-rw-   0        0        0      821 2024-04-12 07:55:17.322929 zeroset-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-12-14 09:12:56.000000 zeroset-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 07:55:17.322929 zeroset-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-04-10 12:55:35.000000 zeroset-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.284467 zeroset-0.0.3/test/
--rw-rw-rw-   0        0        0      204 2024-04-10 13:06:04.000000 zeroset-0.0.3/test/test_cv0.py
--rw-rw-rw-   0        0        0      231 2023-07-23 05:21:32.000000 zeroset-0.0.3/test/test_glob.py
--rw-rw-rw-   0        0        0     1070 2023-12-17 10:16:05.000000 zeroset-0.0.3/test/test_script.py
--rw-rw-rw-   0        0        0     3666 2023-12-14 11:18:25.000000 zeroset-0.0.3/test/test_tabulate.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.309511 zeroset-0.0.3/zeroset/
--rw-rw-rw-   0        0        0      373 2024-04-03 06:30:00.000000 zeroset-0.0.3/zeroset/__init__.py
--rw-rw-rw-   0        0        0     8935 2024-04-10 12:58:17.000000 zeroset-0.0.3/zeroset/cv0.py
--rw-rw-rw-   0        0        0      844 2023-08-31 14:08:59.000000 zeroset-0.0.3/zeroset/fmt0.py
--rw-rw-rw-   0        0        0     5888 2024-04-10 08:02:20.000000 zeroset-0.0.3/zeroset/l0.py
--rw-rw-rw-   0        0        0     2160 2023-12-14 11:32:37.000000 zeroset-0.0.3/zeroset/py0.py
--rw-rw-rw-   0        0        0     3760 2024-02-15 14:22:09.000000 zeroset-0.0.3/zeroset/s0.py
--rw-rw-rw-   0        0        0    40729 2024-04-12 07:53:45.000000 zeroset-0.0.3/zeroset/v0.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:55:17.321929 zeroset-0.0.3/zeroset.egg-info/
--rw-rw-rw-   0        0        0      821 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 07:55:17.000000 zeroset-0.0.3/zeroset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:34.810363 zeroset-0.0.4/
+-rw-rw-rw-   0        0        0      821 2024-04-12 07:59:34.809362 zeroset-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-12-14 09:12:56.000000 zeroset-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:59:34.810363 zeroset-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-04-12 07:59:14.000000 zeroset-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:34.797851 zeroset-0.0.4/test/
+-rw-rw-rw-   0        0        0      204 2024-04-10 13:06:04.000000 zeroset-0.0.4/test/test_cv0.py
+-rw-rw-rw-   0        0        0      231 2023-07-23 05:21:32.000000 zeroset-0.0.4/test/test_glob.py
+-rw-rw-rw-   0        0        0     1070 2023-12-17 10:16:05.000000 zeroset-0.0.4/test/test_script.py
+-rw-rw-rw-   0        0        0     3666 2023-12-14 11:18:25.000000 zeroset-0.0.4/test/test_tabulate.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:34.803363 zeroset-0.0.4/zeroset/
+-rw-rw-rw-   0        0        0      373 2024-04-03 06:30:00.000000 zeroset-0.0.4/zeroset/__init__.py
+-rw-rw-rw-   0        0        0     8935 2024-04-10 12:58:17.000000 zeroset-0.0.4/zeroset/cv0.py
+-rw-rw-rw-   0        0        0      844 2023-08-31 14:08:59.000000 zeroset-0.0.4/zeroset/fmt0.py
+-rw-rw-rw-   0        0        0     5888 2024-04-10 08:02:20.000000 zeroset-0.0.4/zeroset/l0.py
+-rw-rw-rw-   0        0        0     2160 2023-12-14 11:32:37.000000 zeroset-0.0.4/zeroset/py0.py
+-rw-rw-rw-   0        0        0     3760 2024-02-15 14:22:09.000000 zeroset-0.0.4/zeroset/s0.py
+-rw-rw-rw-   0        0        0    40733 2024-04-12 07:58:36.000000 zeroset-0.0.4/zeroset/v0.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:34.808363 zeroset-0.0.4/zeroset.egg-info/
+-rw-rw-rw-   0        0        0      821 2024-04-12 07:59:34.000000 zeroset-0.0.4/zeroset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-12 07:59:34.000000 zeroset-0.0.4/zeroset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:59:34.000000 zeroset-0.0.4/zeroset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-12 07:59:34.000000 zeroset-0.0.4/zeroset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 07:59:34.000000 zeroset-0.0.4/zeroset.egg-info/top_level.txt
```

### Comparing `zeroset-0.0.3/PKG-INFO` & `zeroset-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Useful collection of features.
 Home-page: https://github.com/springkim/zeroset
 Author: Bomm Kim
 Author-email: springnode@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zeroset-0.0.3/setup.py` & `zeroset-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="zeroset",
-        version="0.0.3",
+        version="0.0.4",
         author="Bomm Kim",
         author_email="springnode@gmail.com",
         description="Useful collection of features.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/springkim/zeroset",
         packages=setuptools.find_packages(),
```

### Comparing `zeroset-0.0.3/test/test_script.py` & `zeroset-0.0.4/test/test_script.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/test/test_tabulate.py` & `zeroset-0.0.4/test/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/cv0.py` & `zeroset-0.0.4/zeroset/cv0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/fmt0.py` & `zeroset-0.0.4/zeroset/fmt0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/l0.py` & `zeroset-0.0.4/zeroset/l0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/py0.py` & `zeroset-0.0.4/zeroset/py0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/s0.py` & `zeroset-0.0.4/zeroset/s0.py`

 * *Files identical despite different names*

### Comparing `zeroset-0.0.3/zeroset/v0.py` & `zeroset-0.0.4/zeroset/v0.py`

 * *Files 0% similar despite different names*

```diff
@@ -959,15 +959,15 @@
         cv2.drawContours(image_combined, [contour], -1, color_bgr, thickness)
         if name != "":
             M = cv2.moments(contour)
             cX = int(M["m10"] / M["m00"])
             cY = int(M["m01"] / M["m00"])
             (fw, fh), baseline = cv2.getTextSize(name, fontface, fontscale, font_thickness)
             org = (0 + cX, fh + baseline // 2 + cY)
-            cv2.rectangle(image_combined, (cX - padding, cY - padding), (fw + cX + padding, fh + baseline + cY + padding), color, cv2.FILLED)
+            cv2.rectangle(image_combined, (cX - padding, cY - padding), (fw + cX + padding, fh + baseline + cY + padding), color_bgr, cv2.FILLED)
             # cv2.putText(image_combined, name, (org[0] + padding, org[1] + padding), fontface, fontscale, (64, 64, 64), font_thickness)
             cv2.putText(image_combined, name, org, fontface, fontscale, (255, 255, 255), font_thickness)
 
     return image_combined
 
 
 if __name__ == '__main__':
```

### Comparing `zeroset-0.0.3/zeroset.egg-info/PKG-INFO` & `zeroset-0.0.4/zeroset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Useful collection of features.
 Home-page: https://github.com/springkim/zeroset
 Author: Bomm Kim
 Author-email: springnode@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

