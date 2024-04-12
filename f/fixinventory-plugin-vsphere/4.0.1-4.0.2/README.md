# Comparing `tmp/fixinventory-plugin-vsphere-4.0.1.tar.gz` & `tmp/fixinventory-plugin-vsphere-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-vsphere-4.0.1.tar", last modified: Thu Mar 14 14:04:45 2024, max compression
+gzip compressed data, was "fixinventory-plugin-vsphere-4.0.2.tar", last modified: Fri Apr 12 12:17:14 2024, max compression
```

## Comparing `fixinventory-plugin-vsphere-4.0.1.tar` & `fixinventory-plugin-vsphere-4.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:02:59.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 14:04:45.000000 fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:45.287542 fixinventory-plugin-vsphere-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-14 14:01:51.000000 fixinventory-plugin-vsphere-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:27.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-vsphere-4.0.1/LICENSE` & `fixinventory-plugin-vsphere-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/PKG-INFO` & `fixinventory-plugin-vsphere-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -207,25 +207,25 @@
         limitations under the License.
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/vsphere
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/__init__.py` & `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/config.py` & `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/resources.py` & `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/fix_plugin_vsphere/vsphere_client.py` & `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/PKG-INFO` & `fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -207,25 +207,25 @@
         limitations under the License.
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/vsphere
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-vsphere-4.0.1/fixinventory_plugin_vsphere.egg-info/SOURCES.txt` & `fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.1/pyproject.toml` & `fixinventory-plugin-vsphere-4.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-vsphere"
 description = "Fix VSphere Collector Plugin"
-version = "4.0.1"
+version = "4.0.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     # License information
     "License :: OSI Approved :: Apache Software License",
     # Supported python versions
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.11",
     # Supported OS's
     "Operating System :: POSIX :: Linux",
     "Operating System :: Unix",
     # Extra metadata
     "Environment :: Console",
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.1",
+    "fixinventorylib==4.0.2",
     "pyvmomi",
 ]
 
 [project.entry-points."fix.plugins"]
 vsphere = "fix_plugin_vsphere:VSphereCollectorPlugin"
 
 [project.urls]
```

