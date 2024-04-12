# Comparing `tmp/redfish_service_validator-2.4.2.tar.gz` & `tmp/redfish_service_validator-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_service_validator-2.4.2.tar", last modified: Fri Mar 22 19:25:25 2024, max compression
+gzip compressed data, was "redfish_service_validator-2.4.3.tar", last modified: Fri Apr 12 19:43:46 2024, max compression
```

## Comparing `redfish_service_validator-2.4.2.tar` & `redfish_service_validator-2.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:25:25.863163 redfish_service_validator-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-03-22 19:25:25.863163 redfish_service_validator-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:25:25.859163 redfish_service_validator-2.4.2/redfish_service_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/RedfishLogo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-03-22 19:25:16.000000 redfish_service_validator-2.4.2/redfish_service_validator/RedfishServiceValidator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/RedfishServiceValidatorGui.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/schema_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30081 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/validateRedfish.py
--rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/redfish_service_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:25:25.863163 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 19:25:25.000000 redfish_service_validator-2.4.2/redfish_service_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 19:25:25.863163 redfish_service_validator-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-22 19:25:16.000000 redfish_service_validator-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:25:25.863163 redfish_service_validator-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-03-22 19:25:15.000000 redfish_service_validator-2.4.2/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.766147 redfish_service_validator-2.4.3/redfish_service_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishLogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidatorGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/schema_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30236 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/validateRedfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/redfish_service_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:43:46.000000 redfish_service_validator-2.4.3/redfish_service_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:43:46.770147 redfish_service_validator-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-12 19:43:36.000000 redfish_service_validator-2.4.3/tests/test_catalog.py
```

### Comparing `redfish_service_validator-2.4.2/LICENSE.md` & `redfish_service_validator-2.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/PKG-INFO` & `redfish_service_validator-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.2
+Version: 2.4.3
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.2/README.md` & `redfish_service_validator-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/RedfishLogo.py` & `redfish_service_validator-2.4.3/redfish_service_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/RedfishServiceValidator.py` & `redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from redfish_service_validator.metadata import getSchemaDetails
 from redfish_service_validator.config import convert_config_to_args, convert_args_to_config
 from redfish_service_validator.validateResource import validateSingleURI, validateURITree
 from redfish_service_validator import tohtml, schema_pack, traverse
 from urllib.parse import urlparse
 from collections import Counter
 
-tool_version = '2.4.2'
+tool_version = '2.4.3'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO-1
 VERBOSE2 = logging.INFO-2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/RedfishServiceValidatorGui.py` & `redfish_service_validator-2.4.3/redfish_service_validator/RedfishServiceValidatorGui.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/catalog.py` & `redfish_service_validator-2.4.3/redfish_service_validator/catalog.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/config.py` & `redfish_service_validator-2.4.3/redfish_service_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/helper.py` & `redfish_service_validator-2.4.3/redfish_service_validator/helper.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/metadata.py` & `redfish_service_validator-2.4.3/redfish_service_validator/metadata.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/schema_pack.py` & `redfish_service_validator-2.4.3/redfish_service_validator/schema_pack.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/tohtml.py` & `redfish_service_validator-2.4.3/redfish_service_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/traverse.py` & `redfish_service_validator-2.4.3/redfish_service_validator/traverse.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/validateRedfish.py` & `redfish_service_validator-2.4.3/redfish_service_validator/validateRedfish.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,16 +256,20 @@
         #     new_act_name = '#{}.{}'.format(base_type, new_act)
         #     if new_act_name not in my_actions:
         #         my_actions.append((new_act_name, REDFISH_ABSENT))
 
         for act_name, actionDecoded in my_actions:
             if '@' in act_name:
                 continue
-            act_schema = sub_obj.Type.catalog.getSchemaDocByClass(getNamespace(act_name))
-            act_class = act_schema.classes.get(getNamespace(act_name))
+            try:
+                act_schema = sub_obj.Type.catalog.getSchemaDocByClass(getNamespace(act_name))
+                act_class = act_schema.classes.get(getNamespace(act_name))
+            except:
+                my_logger.warning('Schema not found for action {}'.format(act_name))
+                continue
 
             a, c = validateAction(act_name, actionDecoded, act_class.actions)
 
             actionMessages.update(a)
             actionCounts.update(c)
         subMsgs.update(actionMessages)
         subCounts.update(actionCounts)
```

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator/validateResource.py` & `redfish_service_validator-2.4.3/redfish_service_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator.egg-info/PKG-INFO` & `redfish_service_validator-2.4.3/redfish_service_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.2
+Version: 2.4.3
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.2/redfish_service_validator.egg-info/SOURCES.txt` & `redfish_service_validator-2.4.3/redfish_service_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.2/setup.py` & `redfish_service_validator-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_service_validator",
-    version="2.4.2",
+    version="2.4.3",
     description="Redfish Service Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `redfish_service_validator-2.4.2/tests/test_catalog.py` & `redfish_service_validator-2.4.3/tests/test_catalog.py`

 * *Files identical despite different names*

