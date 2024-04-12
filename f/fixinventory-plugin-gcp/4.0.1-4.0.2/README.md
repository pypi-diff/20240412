# Comparing `tmp/fixinventory-plugin-gcp-4.0.1.tar.gz` & `tmp/fixinventory-plugin-gcp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-gcp-4.0.1.tar", last modified: Thu Mar 14 14:06:49 2024, max compression
+gzip compressed data, was "fixinventory-plugin-gcp-4.0.2.tar", last modified: Fri Apr 12 12:19:21 2024, max compression
```

## Comparing `fixinventory-plugin-gcp-4.0.1.tar` & `fixinventory-plugin-gcp-4.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:06:49.552687 fixinventory-plugin-gcp-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-14 14:06:49.552687 fixinventory-plugin-gcp-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:06:49.548687 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:06:49.548687 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)   364397 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    69260 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20501 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:06:49.552687 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:04.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-14 14:06:49.000000 fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-14 14:06:49.552687 fixinventory-plugin-gcp-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:06:49.552687 fixinventory-plugin-gcp-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-14 14:01:52.000000 fixinventory-plugin-gcp-4.0.1/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.080606 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.080606 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)   364421 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69260 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20501 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:33.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_storage.py
```

### Comparing `fixinventory-plugin-gcp-4.0.1/PKG-INFO` & `fixinventory-plugin-gcp-4.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-gcp
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix GCP Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/gcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
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
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 Requires-Dist: google-api-python-client
 Requires-Dist: oauth2client
 Requires-Dist: retrying
 Requires-Dist: tenacity
 
 # fix-plugin-gcp
 An GCP collector plugin for Fix.
```

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/__init__.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/collector.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/config.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/gcp_client.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/base.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/billing.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/compute.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -5479,23 +5479,23 @@
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "certificate": S("certificate"),
         "expire_time": S("expireTime"),
-        "managed": S("managed", default={}) >> Bend(GcpSslCertificateManagedSslCertificate.mapping),
+        "certificate_managed": S("managed", default={}) >> Bend(GcpSslCertificateManagedSslCertificate.mapping),
         "private_key": S("privateKey"),
         "self_managed": S("selfManaged", default={}) >> Bend(GcpSslCertificateSelfManagedSslCertificate.mapping),
         "subject_alternative_names": S("subjectAlternativeNames", default=[]),
         "type": S("type"),
     }
     certificate: Optional[str] = field(default=None)
     expire_time: Optional[datetime] = field(default=None)
-    managed: Optional[GcpSslCertificateManagedSslCertificate] = field(default=None)
+    certificate_managed: Optional[GcpSslCertificateManagedSslCertificate] = field(default=None)
     private_key: Optional[str] = field(default=None)
     self_managed: Optional[GcpSslCertificateSelfManagedSslCertificate] = field(default=None)
     subject_alternative_names: Optional[List[str]] = field(default=None)
     type: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
```

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/container.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/sqladmin.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/resources/storage.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fix_plugin_gcp/utils.py` & `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/PKG-INFO` & `fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-gcp
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix GCP Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/gcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
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
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 Requires-Dist: google-api-python-client
 Requires-Dist: oauth2client
 Requires-Dist: retrying
 Requires-Dist: tenacity
 
 # fix-plugin-gcp
 An GCP collector plugin for Fix.
```

### Comparing `fixinventory-plugin-gcp-4.0.1/fixinventory_plugin_gcp.egg-info/SOURCES.txt` & `fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/pyproject.toml` & `fixinventory-plugin-gcp-4.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-gcp"
 description = "Fix GCP Collector Plugin"
-version = "4.0.1"
+version = "4.0.2"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
     # Audience
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     # License information
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
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
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."fix.plugins"]
```

### Comparing `fixinventory-plugin-gcp-4.0.1/test/conftest.py` & `fixinventory-plugin-gcp-4.0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/random_client.py` & `fixinventory-plugin-gcp-4.0.2/test/random_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_base.py` & `fixinventory-plugin-gcp-4.0.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_billing.py` & `fixinventory-plugin-gcp-4.0.2/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_collector.py` & `fixinventory-plugin-gcp-4.0.2/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_compute.py` & `fixinventory-plugin-gcp-4.0.2/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_config.py` & `fixinventory-plugin-gcp-4.0.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_container.py` & `fixinventory-plugin-gcp-4.0.2/test/test_container.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.1/test/test_sqladmin.py` & `fixinventory-plugin-gcp-4.0.2/test/test_sqladmin.py`

 * *Files identical despite different names*

