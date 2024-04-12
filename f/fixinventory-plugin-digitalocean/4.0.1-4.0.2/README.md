# Comparing `tmp/fixinventory-plugin-digitalocean-4.0.1.tar.gz` & `tmp/fixinventory-plugin-digitalocean-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-digitalocean-4.0.1.tar", last modified: Thu Mar 14 14:05:54 2024, max compression
+gzip compressed data, was "fixinventory-plugin-digitalocean-4.0.2.tar", last modified: Fri Apr 12 12:19:04 2024, max compression
```

## Comparing `fixinventory-plugin-digitalocean-4.0.1.tar` & `fixinventory-plugin-digitalocean-4.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:54.352815 fixinventory-plugin-digitalocean-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-14 14:05:54.352815 fixinventory-plugin-digitalocean-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:54.344815 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48601 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:54.352815 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:09.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 14:05:54.000000 fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:05:54.352815 fixinventory-plugin-digitalocean-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:54.348815 fixinventory-plugin-digitalocean-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:54.352815 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/cpu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/memory_available.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/neighbor_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25838 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-14 14:01:56.000000 fixinventory-plugin-digitalocean-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:04.188727 fixinventory-plugin-digitalocean-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-12 12:19:04.188727 fixinventory-plugin-digitalocean-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:04.180726 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48601 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:04.188727 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:18.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 12:19:04.000000 fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:19:04.188727 fixinventory-plugin-digitalocean-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:04.184726 fixinventory-plugin-digitalocean-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:04.188727 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/cpu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/memory_available.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/neighbor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25838 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 12:15:04.000000 fixinventory-plugin-digitalocean-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-digitalocean-4.0.1/PKG-INFO` & `fixinventory-plugin-digitalocean-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-digitalocean
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/digitalocean
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
 Requires-Dist: boto3
 Requires-Dist: requests
 Requires-Dist: botocore
 Requires-Dist: retrying
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: tzlocal; extra == "test"
```

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/__init__.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/client.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/collector.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/config.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/resources.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fix_plugin_digitalocean/utils.py` & `fixinventory-plugin-digitalocean-4.0.2/fix_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/PKG-INFO` & `fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-digitalocean
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/digitalocean
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
 Requires-Dist: boto3
 Requires-Dist: requests
 Requires-Dist: botocore
 Requires-Dist: retrying
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: tzlocal; extra == "test"
```

### Comparing `fixinventory-plugin-digitalocean-4.0.1/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt` & `fixinventory-plugin-digitalocean-4.0.2/fixinventory_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/pyproject.toml` & `fixinventory-plugin-digitalocean-4.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-digitalocean"
 description = "Fix DigitalOcean Collector Plugin"
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
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
```

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/__init__.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/apps.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/cpu_metrics.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/databases.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/domain_records.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/droplets.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/firewalls.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/floatingip.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/k8s.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/loadbalancers.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/memory_available.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/memory_available.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/projectresources.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/projects.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/regions.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/registry_repositories.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/tags.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/fixtures/volumes.py` & `fixinventory-plugin-digitalocean-4.0.2/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-digitalocean-4.0.1/test/test_collector.py` & `fixinventory-plugin-digitalocean-4.0.2/test/test_collector.py`

 * *Files identical despite different names*

