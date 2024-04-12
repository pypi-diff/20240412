# Comparing `tmp/preprocess-docs-0.0.3.tar.gz` & `tmp/preprocess-docs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocess-docs-0.0.3.tar", last modified: Fri Apr 12 03:52:27 2024, max compression
+gzip compressed data, was "preprocess-docs-0.0.4.tar", last modified: Fri Apr 12 04:38:47 2024, max compression
```

## Comparing `preprocess-docs-0.0.3.tar` & `preprocess-docs-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.697692 preprocess-docs-0.0.3/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 03:51:18.000000 preprocess-docs-0.0.3/LICENSE
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 03:52:27.697524 preprocess-docs-0.0.3/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-12 03:51:17.000000 preprocess-docs-0.0.3/README.md
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.696032 preprocess-docs-0.0.3/preprocess/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       78 2024-04-12 03:51:25.000000 preprocess-docs-0.0.3/preprocess/__init__.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      685 2024-04-12 03:51:24.000000 preprocess-docs-0.0.3/preprocess/element.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1011 2024-04-12 03:51:27.000000 preprocess-docs-0.0.3/preprocess/html.py
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.696952 preprocess-docs-0.0.3/preprocess_docs.egg-info/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      284 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/SOURCES.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/dependency_links.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       15 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/requires.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/top_level.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-12 03:52:27.697762 preprocess-docs-0.0.3/setup.cfg
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      696 2024-04-12 03:52:07.000000 preprocess-docs-0.0.3/setup.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.281505 preprocess-docs-0.0.4/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 03:51:18.000000 preprocess-docs-0.0.4/LICENSE
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 04:38:47.281336 preprocess-docs-0.0.4/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-12 03:51:17.000000 preprocess-docs-0.0.4/README.md
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.280217 preprocess-docs-0.0.4/preprocess/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       78 2024-04-12 03:51:25.000000 preprocess-docs-0.0.4/preprocess/__init__.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      685 2024-04-12 04:35:52.000000 preprocess-docs-0.0.4/preprocess/element.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 04:35:47.000000 preprocess-docs-0.0.4/preprocess/html.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.281091 preprocess-docs-0.0.4/preprocess_docs.egg-info/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      284 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       15 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/requires.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/top_level.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-12 04:38:47.281571 preprocess-docs-0.0.4/setup.cfg
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      696 2024-04-12 04:38:35.000000 preprocess-docs-0.0.4/setup.py
```

### Comparing `preprocess-docs-0.0.3/LICENSE` & `preprocess-docs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.3/PKG-INFO` & `preprocess-docs-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.3
+Version: 0.0.4
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.3/preprocess/element.py` & `preprocess-docs-0.0.4/preprocess/element.py`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.3/preprocess/html.py` & `preprocess-docs-0.0.4/preprocess/html.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,23 @@
   queue = deque([(html_tag, document)])
   while queue:
     cur, parent = queue.popleft()
     if cur in visited:
       continue
     visited.add(cur)
     if isinstance(cur, bs4.element.NavigableString):
-      stripped_text = cur.string.strip()
-      if stripped_text:
-        child_elem = TextElement(text=cur.string.strip())
-        parent.children.append(child_elem)
+      if cur.string is None or cur.string.strip() == "":
+        continue
+      child_elem = TextElement(text=cur.string.strip())
+      parent.children.append(child_elem)
     elif isinstance(cur, bs4.element.Tag):
       if cur.name == 'a':
-        child_elem = LinkElement(text=cur.string.strip(), url=cur.get('href'))
+        text = None if cur.string is None else cur.string.strip()
+        child_elem = LinkElement(text=text, url=cur.get('href'))
         parent.children.append(child_elem)
       else:
         child_elem = Element(cur.name)
         parent.children.append(child_elem)
-        for child in cur.children:
-          queue.append((child, child_elem))
+
+      for child in cur.children:
+        queue.append((child, child_elem))
   return document
```

### Comparing `preprocess-docs-0.0.3/preprocess_docs.egg-info/PKG-INFO` & `preprocess-docs-0.0.4/preprocess_docs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.3
+Version: 0.0.4
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.3/setup.py` & `preprocess-docs-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="preprocess-docs",
-    version="0.0.3",
+    version="0.0.4",
     author="Eddy Jin",
     description="An open source document preprocessor for AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eddyjin1/preprocess",
     packages=setuptools.find_packages(),
     install_requires = [
```

