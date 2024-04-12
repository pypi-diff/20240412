# Comparing `tmp/apmtools-0.0.1.tar.gz` & `tmp/apmtools-0.0.2.tar.gz`

## Comparing `apmtools-0.0.1.tar` & `apmtools-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.1/src/apmtools/__init__.py
--rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 apmtools-0.0.1/src/apmtools/classes.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 apmtools-0.0.1/src/apmtools/functions.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.1/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 apmtools-0.0.1/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 apmtools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/__init__.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.2/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.2/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 apmtools-0.0.2/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 apmtools-0.0.2/PKG-INFO
```

### Comparing `apmtools-0.0.1/src/apmtools/classes.py` & `apmtools-0.0.2/src/apmtools/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         if type(filter_dict) != type(dict()):
             print("subset function error: type filter_dict should be dict")
             return
         return_dict = self
         for i, j in filter_dict.items():
             a = {}
             for key, value in return_dict.items():
-                if hasattr(value, 'metadata') & (type(value.metadata) == type({})) & (i in value.metadata.keys()):
+                if hasattr(value, 'meta') & (type(value.metadata) == type({})) & (i in value.metadata.keys()):
                     try:
-                        if value.__getattr__('metadata')[i] in j:
+                        if value.__getattr__('meta')[i] in j:
                             a[key] = value
                     except:
                         pass
                 else:
                     try:
                         if value.__getattr__(i) in j:
                             a[key] = value
@@ -51,17 +51,17 @@
 
     def set_attrib(self, attribute):
         """
         returns the set of attribute values for dictionary
         """
         return_set = set()
         for i in self.values():
-            if hasattr(i, 'metadata') & (type(i.metadata) == type({})) & (attribute in i.metadata.keys()):
+            if hasattr(i, 'meta') & (type(i.metadata) == type({})) & (attribute in i.metadata.keys()):
                 try:
-                    return_set.add(i.__getattr__('metadata')[attribute])
+                    return_set.add(i.__getattr__('meta')[attribute])
                 except:
                     pass
             else:
                 try:
                     return_set.add(i.__getattr__(attribute))
                 except:
                     pass
```

### Comparing `apmtools-0.0.1/src/apmtools/functions.py` & `apmtools-0.0.2/src/apmtools/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os as os
+import uuid as uuid
+
 def show(dictionary, number=0):
     """
     return an element of a dictionary
     If number is not specified, returns the values associated with the first key
     """
     try:
         return(dictionary[list(dictionary.keys())[number]])
@@ -54,8 +57,20 @@
                 pass
         else:
             try:
                 return_set.add(i.__getattr__(attribute))
             except:
                 pass
     
-    return return_set 
+    return return_set
+
+
+def scan(directory, function, extension, target_dictionary):
+    for j in os.listdir(directory):
+        if j.split('.')[-1] == extension:
+            processed = function(directory, j)
+            target_dictionary[str(uuid.uuid4())] = processed
+        elif (len(j.split('.'))) == 1:
+            d = directory+j+'/'
+            scan(d, function, extension, target_dictionary)
+        else:
+            pass
```

### Comparing `apmtools-0.0.1/LICENSE` & `apmtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.1/pyproject.toml` & `apmtools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.1/PKG-INFO` & `apmtools-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

