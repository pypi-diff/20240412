# Comparing `tmp/prometheus-pve-exporter-3.2.2.tar.gz` & `tmp/prometheus-pve-exporter-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-pve-exporter-3.2.2.tar", last modified: Tue Feb  6 09:09:40 2024, max compression
+gzip compressed data, was "prometheus-pve-exporter-3.2.4.tar", last modified: Fri Apr 12 07:45:30 2024, max compression
```

## Comparing `prometheus-pve-exporter-3.2.2.tar` & `prometheus-pve-exporter-3.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.560674 prometheus-pve-exporter-3.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.560674 prometheus-pve-exporter-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.github/workflows/container-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.github/workflows/container-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/pve.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/pylintrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.560674 prometheus-pve-exporter-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-06 09:09:40.000000 prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 09:09:40.564674 prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-02-06 09:09:30.000000 prometheus-pve-exporter-3.2.2/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/container-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pylintrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:45:30.150176 prometheus-pve-exporter-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.142176 prometheus-pve-exporter-3.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 07:45:30.000000 prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3845 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:45:30.146176 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-12 07:45:20.000000 prometheus-pve-exporter-3.2.4/src/pve_exporter/http.py
```

### Comparing `prometheus-pve-exporter-3.2.2/.github/workflows/ci.yml` & `prometheus-pve-exporter-3.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/.github/workflows/container-image.yml` & `prometheus-pve-exporter-3.2.4/.github/workflows/container-image.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/.github/workflows/container-test.yml` & `prometheus-pve-exporter-3.2.4/.github/workflows/container-test.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/.github/workflows/pypi.yml` & `prometheus-pve-exporter-3.2.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/CHANGELOG.rst` & `prometheus-pve-exporter-3.2.4/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,34 @@
 
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
+
+`3.2.4`_ - 2024-04-12
+---------------------
+
+Changed
+~~~~~~~
+
+- Bump idna from 3.6 to 3.7 (#239)
+- Bump werkzeug from 3.0.1 to 3.0.2 (#237)
+
+
+`3.2.3`_ - 2024-02-25
+---------------------
+
+Changed
+~~~~~~~
+
+- Bump cryptography from 42.0.2 to 42.0.4 (#232)
+
+
 `3.2.2`_ - 2024-02-06
 ---------------------
 
 Changed
 ~~~~~~~
 
 - Bump cryptography from 41.0.7 to 42.0.0 (#226)
@@ -356,15 +376,18 @@
 ~~~~~
 
 -  IPv6 support
 
 
 .. _Keep a Changelog: http://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: http://semver.org/spec/v2.0.0.html
-.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...HEAD
+.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...HEAD
+.. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.3
+.. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.2
+.. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.1
 .. _3.2.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.0
 .. _3.2.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.0...v3.1.0
 .. _3.1.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.1.0...v3.0.2
 .. _3.0.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.2...v3.0.1
 .. _3.0.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.1...v3.0.0
 .. _3.0.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.0.0b1...v3.0.0
 .. _3.0.0b1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v2.3.1...v3.0.0b1
```

### Comparing `prometheus-pve-exporter-3.2.2/Dockerfile` & `prometheus-pve-exporter-3.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/LICENSE` & `prometheus-pve-exporter-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/PKG-INFO` & `prometheus-pve-exporter-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.2
+Version: 3.2.4
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus-pve-exporter-3.2.2/README.rst` & `prometheus-pve-exporter-3.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/pylintrc.toml` & `prometheus-pve-exporter-3.2.4/pylintrc.toml`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/pyproject.toml` & `prometheus-pve-exporter-3.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus-pve-exporter"
-version = "3.2.2"
+version = "3.2.4"
 authors = [{ name = "Lorenz Schori", email = "lo@znerol.ch" }]
 description = "Proxmox VE exporter for the Prometheus monitoring system."
 requires-python = ">=3.9"
 keywords = ["prometheus", "exporter", "network", "monitoring", "proxmox"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `prometheus-pve-exporter-3.2.2/requirements.txt` & `prometheus-pve-exporter-3.2.4/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -181,55 +181,55 @@
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
-cryptography==42.0.0 \
-    --hash=sha256:0a68bfcf57a6887818307600c3c0ebc3f62fbb6ccad2240aa21887cda1f8df1b \
-    --hash=sha256:146e971e92a6dd042214b537a726c9750496128453146ab0ee8971a0299dc9bd \
-    --hash=sha256:14e4b909373bc5bf1095311fa0f7fcabf2d1a160ca13f1e9e467be1ac4cbdf94 \
-    --hash=sha256:206aaf42e031b93f86ad60f9f5d9da1b09164f25488238ac1dc488334eb5e221 \
-    --hash=sha256:3005166a39b70c8b94455fdbe78d87a444da31ff70de3331cdec2c568cf25b7e \
-    --hash=sha256:324721d93b998cb7367f1e6897370644751e5580ff9b370c0a50dc60a2003513 \
-    --hash=sha256:33588310b5c886dfb87dba5f013b8d27df7ffd31dc753775342a1e5ab139e59d \
-    --hash=sha256:35cf6ed4c38f054478a9df14f03c1169bb14bd98f0b1705751079b25e1cb58bc \
-    --hash=sha256:3ca482ea80626048975360c8e62be3ceb0f11803180b73163acd24bf014133a0 \
-    --hash=sha256:56ce0c106d5c3fec1038c3cca3d55ac320a5be1b44bf15116732d0bc716979a2 \
-    --hash=sha256:5a217bca51f3b91971400890905a9323ad805838ca3fa1e202a01844f485ee87 \
-    --hash=sha256:678cfa0d1e72ef41d48993a7be75a76b0725d29b820ff3cfd606a5b2b33fda01 \
-    --hash=sha256:69fd009a325cad6fbfd5b04c711a4da563c6c4854fc4c9544bff3088387c77c0 \
-    --hash=sha256:6cf9b76d6e93c62114bd19485e5cb003115c134cf9ce91f8ac924c44f8c8c3f4 \
-    --hash=sha256:74f18a4c8ca04134d2052a140322002fef535c99cdbc2a6afc18a8024d5c9d5b \
-    --hash=sha256:85f759ed59ffd1d0baad296e72780aa62ff8a71f94dc1ab340386a1207d0ea81 \
-    --hash=sha256:87086eae86a700307b544625e3ba11cc600c3c0ef8ab97b0fda0705d6db3d4e3 \
-    --hash=sha256:8814722cffcfd1fbd91edd9f3451b88a8f26a5fd41b28c1c9193949d1c689dc4 \
-    --hash=sha256:8fedec73d590fd30c4e3f0d0f4bc961aeca8390c72f3eaa1a0874d180e868ddf \
-    --hash=sha256:9515ea7f596c8092fdc9902627e51b23a75daa2c7815ed5aa8cf4f07469212ec \
-    --hash=sha256:988b738f56c665366b1e4bfd9045c3efae89ee366ca3839cd5af53eaa1401bce \
-    --hash=sha256:a2a8d873667e4fd2f34aedab02ba500b824692c6542e017075a2efc38f60a4c0 \
-    --hash=sha256:bd7cf7a8d9f34cc67220f1195884151426ce616fdc8285df9054bfa10135925f \
-    --hash=sha256:bdce70e562c69bb089523e75ef1d9625b7417c6297a76ac27b1b8b1eb51b7d0f \
-    --hash=sha256:be14b31eb3a293fc6e6aa2807c8a3224c71426f7c4e3639ccf1a2f3ffd6df8c3 \
-    --hash=sha256:be41b0c7366e5549265adf2145135dca107718fa44b6e418dc7499cfff6b4689 \
-    --hash=sha256:c310767268d88803b653fffe6d6f2f17bb9d49ffceb8d70aed50ad45ea49ab08 \
-    --hash=sha256:c58115384bdcfe9c7f644c72f10f6f42bed7cf59f7b52fe1bf7ae0a622b3a139 \
-    --hash=sha256:c640b0ef54138fde761ec99a6c7dc4ce05e80420262c20fa239e694ca371d434 \
-    --hash=sha256:ca20550bb590db16223eb9ccc5852335b48b8f597e2f6f0878bbfd9e7314eb17 \
-    --hash=sha256:d97aae66b7de41cdf5b12087b5509e4e9805ed6f562406dfcf60e8481a9a28f8 \
-    --hash=sha256:e9326ca78111e4c645f7e49cbce4ed2f3f85e17b61a563328c85a5208cf34440
+cryptography==42.0.4 \
+    --hash=sha256:01911714117642a3f1792c7f376db572aadadbafcd8d75bb527166009c9f1d1b \
+    --hash=sha256:0e89f7b84f421c56e7ff69f11c441ebda73b8a8e6488d322ef71746224c20fce \
+    --hash=sha256:12d341bd42cdb7d4937b0cabbdf2a94f949413ac4504904d0cdbdce4a22cbf88 \
+    --hash=sha256:15a1fb843c48b4a604663fa30af60818cd28f895572386e5f9b8a665874c26e7 \
+    --hash=sha256:1cdcdbd117681c88d717437ada72bdd5be9de117f96e3f4d50dab3f59fd9ab20 \
+    --hash=sha256:1df6fcbf60560d2113b5ed90f072dc0b108d64750d4cbd46a21ec882c7aefce9 \
+    --hash=sha256:3c6048f217533d89f2f8f4f0fe3044bf0b2090453b7b73d0b77db47b80af8dff \
+    --hash=sha256:3e970a2119507d0b104f0a8e281521ad28fc26f2820687b3436b8c9a5fcf20d1 \
+    --hash=sha256:44a64043f743485925d3bcac548d05df0f9bb445c5fcca6681889c7c3ab12764 \
+    --hash=sha256:4e36685cb634af55e0677d435d425043967ac2f3790ec652b2b88ad03b85c27b \
+    --hash=sha256:5f8907fcf57392cd917892ae83708761c6ff3c37a8e835d7246ff0ad251d9298 \
+    --hash=sha256:69b22ab6506a3fe483d67d1ed878e1602bdd5912a134e6202c1ec672233241c1 \
+    --hash=sha256:6bfadd884e7280df24d26f2186e4e07556a05d37393b0f220a840b083dc6a824 \
+    --hash=sha256:6d0fbe73728c44ca3a241eff9aefe6496ab2656d6e7a4ea2459865f2e8613257 \
+    --hash=sha256:6ffb03d419edcab93b4b19c22ee80c007fb2d708429cecebf1dd3258956a563a \
+    --hash=sha256:810bcf151caefc03e51a3d61e53335cd5c7316c0a105cc695f0959f2c638b129 \
+    --hash=sha256:831a4b37accef30cccd34fcb916a5d7b5be3cbbe27268a02832c3e450aea39cb \
+    --hash=sha256:887623fe0d70f48ab3f5e4dbf234986b1329a64c066d719432d0698522749929 \
+    --hash=sha256:a0298bdc6e98ca21382afe914c642620370ce0470a01e1bef6dd9b5354c36854 \
+    --hash=sha256:a1327f280c824ff7885bdeef8578f74690e9079267c1c8bd7dc5cc5aa065ae52 \
+    --hash=sha256:c1f25b252d2c87088abc8bbc4f1ecbf7c919e05508a7e8628e6875c40bc70923 \
+    --hash=sha256:c3a5cbc620e1e17009f30dd34cb0d85c987afd21c41a74352d1719be33380885 \
+    --hash=sha256:ce8613beaffc7c14f091497346ef117c1798c202b01153a8cc7b8e2ebaaf41c0 \
+    --hash=sha256:d2a27aca5597c8a71abbe10209184e1a8e91c1fd470b5070a2ea60cafec35bcd \
+    --hash=sha256:dad9c385ba8ee025bb0d856714f71d7840020fe176ae0229de618f14dae7a6e2 \
+    --hash=sha256:db4b65b02f59035037fde0998974d84244a64c3265bdef32a827ab9b63d61b18 \
+    --hash=sha256:e09469a2cec88fb7b078e16d4adec594414397e8879a4341c6ace96013463d5b \
+    --hash=sha256:e53dc41cda40b248ebc40b83b31516487f7db95ab8ceac1f042626bc43a2f992 \
+    --hash=sha256:f1e85a178384bf19e36779d91ff35c7617c885da487d689b05c1366f9933ad74 \
+    --hash=sha256:f47be41843200f7faec0683ad751e5ef11b9a56a220d57f300376cd8aba81660 \
+    --hash=sha256:fb0cef872d8193e487fc6bdb08559c3aa41b659a7d9be48b2e10747f47863925 \
+    --hash=sha256:ffc73996c4fca3d2b6c1c8c12bfd3ad00def8621da24f547626bf06441400449
     # via paramiko
 gunicorn==21.2.0 \
     --hash=sha256:3213aa5e8c24949e792bcacfc176fef362e7aac80b76c56f6b5122bf350722f0 \
     --hash=sha256:88ec8bff1d634f98e61b9f65bc4bf3cd918a90806c6f5c48bc5603849ec81033
     # via -r requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 markupsafe==2.1.3 \
     --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
     --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
     --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
     --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
     --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
@@ -293,17 +293,17 @@
     --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
     --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
     # via gunicorn
 paramiko==3.4.0 \
     --hash=sha256:43f0b51115a896f9c00f59618023484cb3a14b98bbceab43394a39c6739b7ee7 \
     --hash=sha256:aac08f26a31dc4dffd92821527d1682d99d52f9ef6851968114a8728f3c274d3
     # via -r requirements.in
-prometheus-client==0.19.0 \
-    --hash=sha256:4585b0d1223148c27a225b10dbec5ae9bc4c81a99a3fa80774fa6209935324e1 \
-    --hash=sha256:c88b1e6ecf6b41cd8fb5731c7ae919bf66df6ec6fafa555cd6c0e16ca169ae92
+prometheus-client==0.20.0 \
+    --hash=sha256:287629d00b147a32dcb2be0b9df905da599b2d82f80377083ec8463309a4bb89 \
+    --hash=sha256:cde524a85bce83ca359cc837f28b8c0db5cac7aa653a588fd7e84ba061c329e7
     # via -r requirements.in
 proxmoxer==2.0.1 \
     --hash=sha256:088923f1a81ee27631e88314c609bfe22b33d8a41271b5f02e86f996f837fe31 \
     --hash=sha256:badb3095507e486b76dfda75177545dd85da608a3aef8590d362901253f10576
     # via -r requirements.in
 pycparser==2.21 \
     --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
@@ -377,11 +377,11 @@
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via -r requirements.in
 urllib3==2.1.0 \
     --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
     --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
     # via requests
-werkzeug==3.0.1 \
-    --hash=sha256:507e811ecea72b18a404947aded4b3390e1db8f826b494d76550ef45bb3b1dcc \
-    --hash=sha256:90a285dc0e42ad56b34e696398b8122ee4c681833fb35b8334a095d82c56da10
+werkzeug==3.0.2 \
+    --hash=sha256:3aac3f5da756f93030740bc235d3e09449efcf65f2f55e3602e1d851b8f48795 \
+    --hash=sha256:e39b645a6ac92822588e7b39a692e7828724ceae0b0d702ef96701f90e70128d
     # via -r requirements.in
```

### Comparing `prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.2.2
+Version: 3.2.4
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus-pve-exporter-3.2.2/src/prometheus_pve_exporter.egg-info/SOURCES.txt` & `prometheus-pve-exporter-3.2.4/src/prometheus_pve_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/cli.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/__init__.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/cluster.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/cluster.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/collector/node.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/collector/node.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/config.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-exporter-3.2.2/src/pve_exporter/http.py` & `prometheus-pve-exporter-3.2.4/src/pve_exporter/http.py`

 * *Files identical despite different names*

