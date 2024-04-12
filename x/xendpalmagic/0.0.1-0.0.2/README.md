# Comparing `tmp/xendpalmagic-0.0.1.tar.gz` & `tmp/xendpalmagic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xendpalmagic-0.0.1.tar", last modified: Tue Mar 26 20:28:44 2024, max compression
+gzip compressed data, was "xendpalmagic-0.0.2.tar", last modified: Fri Apr 12 17:51:10 2024, max compression
```

## Comparing `xendpalmagic-0.0.1.tar` & `xendpalmagic-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-03-26 20:28:44.066573 xendpalmagic-0.0.1/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-03-23 10:10:08.000000 xendpalmagic-0.0.1/LICENSE
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)      161 2024-03-26 20:23:38.000000 xendpalmagic-0.0.1/MANIFEST.in
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3229 2024-03-26 20:28:44.066573 xendpalmagic-0.0.1/PKG-INFO
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     2245 2024-03-26 20:14:41.000000 xendpalmagic-0.0.1/README.md
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-03-23 10:09:39.000000 xendpalmagic-0.0.1/requirements.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)       38 2024-03-26 20:28:44.066573 xendpalmagic-0.0.1/setup.cfg
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3271 2024-03-26 20:27:20.000000 xendpalmagic-0.0.1/setup.py
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-03-26 20:28:44.063240 xendpalmagic-0.0.1/xendpalmagic/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-03-23 10:08:00.000000 xendpalmagic-0.0.1/xendpalmagic/__init__.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3624 2024-03-26 13:21:40.000000 xendpalmagic-0.0.1/xendpalmagic/core.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     1281 2024-03-26 12:20:50.000000 xendpalmagic-0.0.1/xendpalmagic/exceptions.py
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)    12673 2024-03-26 12:11:49.000000 xendpalmagic-0.0.1/xendpalmagic/signatures.py
-drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-03-26 20:28:44.063240 xendpalmagic-0.0.1/xendpalmagic.egg-info/
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3229 2024-03-26 20:28:44.000000 xendpalmagic-0.0.1/xendpalmagic.egg-info/PKG-INFO
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)      299 2024-03-26 20:28:44.000000 xendpalmagic-0.0.1/xendpalmagic.egg-info/SOURCES.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)        1 2024-03-26 20:28:44.000000 xendpalmagic-0.0.1/xendpalmagic.egg-info/dependency_links.txt
--rw-r--r--   0 joelogin  (1000) joelogin  (1004)       13 2024-03-26 20:28:44.000000 xendpalmagic-0.0.1/xendpalmagic.egg-info/top_level.txt
+drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/LICENSE
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)      161 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/MANIFEST.in
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3227 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/PKG-INFO
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     2243 2024-04-12 17:49:31.000000 xendpalmagic-0.0.2/README.md
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)        0 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/requirements.txt
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)       38 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/setup.cfg
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3271 2024-04-12 17:49:51.000000 xendpalmagic-0.0.2/setup.py
+drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.807257 xendpalmagic-0.0.2/xendpalmagic/
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)       94 2024-04-12 17:32:22.000000 xendpalmagic-0.0.2/xendpalmagic/__init__.py
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3624 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/core.py
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     1281 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/exceptions.py
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)    12673 2024-04-11 16:29:54.000000 xendpalmagic-0.0.2/xendpalmagic/signatures.py
+drwxr-xr-x   0 joelogin  (1000) joelogin  (1004)        0 2024-04-12 17:51:10.810590 xendpalmagic-0.0.2/xendpalmagic.egg-info/
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)     3227 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/PKG-INFO
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)      299 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)        1 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 joelogin  (1000) joelogin  (1004)       13 2024-04-12 17:51:10.000000 xendpalmagic-0.0.2/xendpalmagic.egg-info/top_level.txt
```

### Comparing `xendpalmagic-0.0.1/PKG-INFO` & `xendpalmagic-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xendpalmagic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Xendpal-magic: Advanced File Type Detection Library
 Author: joeygoesgrey
 Author-email: <mail@godfreydjoseph@gmail.com>
 License: MIT
 Keywords: file type detection,file signatures,MIME type,content analysis,python,file handling,file identification,magic numbers,file metadata
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -37,37 +37,37 @@
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
 
 ## Installation
 
 Install Xendpal-magic using pip:
 
 ```bash
-pip install xendpal-magic
+pip install xendpalmagic
 ```
 
 ## Quick Start
 
 ```python
-from xendpal_magic import FileSignatureMatcher
+from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('example.pdf')
+file_type = matcher.determine_file_type('path to file')
 print(file_type)  # Outputs: 'application/pdf'
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('example.docx')
+file_description = matcher.determine_file_type('path to file')
 print(file_description)  # Outputs: 'Microsoft Word document'
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
@@ -84,12 +84,12 @@
 
 ## License
 
 Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
 
 ---
```

### Comparing `xendpalmagic-0.0.1/README.md` & `xendpalmagic-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,37 +13,37 @@
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
 
 ## Installation
 
 Install Xendpal-magic using pip:
 
 ```bash
-pip install xendpal-magic
+pip install xendpalmagic
 ```
 
 ## Quick Start
 
 ```python
-from xendpal_magic import FileSignatureMatcher
+from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('example.pdf')
+file_type = matcher.determine_file_type('path to file')
 print(file_type)  # Outputs: 'application/pdf'
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('example.docx')
+file_description = matcher.determine_file_type('path to file')
 print(file_description)  # Outputs: 'Microsoft Word document'
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
@@ -60,12 +60,12 @@
 
 ## License
 
 Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
 
 ---
```

### Comparing `xendpalmagic-0.0.1/setup.py` & `xendpalmagic-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Xendpal-magic: Advanced File Type Detection Library'
 LONG_DESCRIPTION = """Xendpal-magic is a cutting-edge Python library designed to elevate file type detection to new heights. Unlike traditional methods that rely solely on file extensions or basic signatures, Xendpal-magic introduces a multifaceted approach incorporating file extensions, magic numbers, content analysis, and header parsing to deliver unparalleled accuracy and reliability. This library stands out by offering customizable detection strategies, allowing users to tailor the detection process to their specific needs—whether prioritizing speed, accuracy, or a balance of both.
 
 At the heart of Xendpal-magic lies a comprehensive database of file signatures and MIME types, covering a vast spectrum of file formats. From common image and document formats to more obscure or custom file types, Xendpal-magic ensures your application can identify and handle a wide array of files confidently. Furthermore, the library's extensible design means users can effortlessly add new signatures and MIME types, making it an ever-evolving tool that adapts to new file formats and industry standards.
 
 Designed with both ease of use and flexibility in mind, Xendpal-magic caters to developers looking for a simple solution to file type detection while also offering advanced features for those needing more control over the detection process. Whether you're building a content management system, a digital asset manager, or any application that requires robust file handling capabilities, Xendpal-magic is equipped to meet the challenge.
```

### Comparing `xendpalmagic-0.0.1/xendpalmagic/core.py` & `xendpalmagic-0.0.2/xendpalmagic/core.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.1/xendpalmagic/exceptions.py` & `xendpalmagic-0.0.2/xendpalmagic/exceptions.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.1/xendpalmagic/signatures.py` & `xendpalmagic-0.0.2/xendpalmagic/signatures.py`

 * *Files identical despite different names*

### Comparing `xendpalmagic-0.0.1/xendpalmagic.egg-info/PKG-INFO` & `xendpalmagic-0.0.2/xendpalmagic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xendpalmagic
-Version: 0.0.1
+Version: 0.0.2
 Summary: Xendpal-magic: Advanced File Type Detection Library
 Author: joeygoesgrey
 Author-email: <mail@godfreydjoseph@gmail.com>
 License: MIT
 Keywords: file type detection,file signatures,MIME type,content analysis,python,file handling,file identification,magic numbers,file metadata
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -37,37 +37,37 @@
 - **Developer-friendly**: Easy to integrate and use in any Python project requiring file handling capabilities.
 
 ## Installation
 
 Install Xendpal-magic using pip:
 
 ```bash
-pip install xendpal-magic
+pip install xendpalmagic
 ```
 
 ## Quick Start
 
 ```python
-from xendpal_magic import FileSignatureMatcher
+from xendpalmagic import FileSignatureMatcher
 
 # Initialize the matcher
 matcher = FileSignatureMatcher()
 
 # Determine the file type of 'example.pdf'
-file_type = matcher.determine_file_type('example.pdf')
+file_type = matcher.determine_file_type('path to file')
 print(file_type)  # Outputs: 'application/pdf'
 ```
 
 ## Advanced Usage
 
 ### Custom Detection Strategy
 
 ```python
 matcher = FileSignatureMatcher(detection_method='signature', return_type='description')
-file_description = matcher.determine_file_type('example.docx')
+file_description = matcher.determine_file_type('path to file')
 print(file_description)  # Outputs: 'Microsoft Word document'
 ```
 
 ### Adding Custom File Signatures
 
 ```python
 matcher.add_custom_signature(
@@ -84,12 +84,12 @@
 
 ## License
 
 Xendpal-magic is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
-- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpal-magic into what it is today.
+- Special thanks to all [contributors](https://github.com/yourusername/xendpal-magic/contributors) who have helped shape Xendpalmagic into what it is today.
 
 ---
```

