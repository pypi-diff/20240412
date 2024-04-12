# Comparing `tmp/sosviz-0.2.0.tar.gz` & `tmp/sosviz-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosviz-0.2.0.tar", last modified: Fri Apr 12 15:10:59 2024, max compression
+gzip compressed data, was "sosviz-0.2.2.tar", last modified: Fri Apr 12 15:30:16 2024, max compression
```

## Comparing `sosviz-0.2.0.tar` & `sosviz-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 rjarry    (1000) rjarry    (1000)        0 2024-04-12 15:10:59.074659 sosviz-0.2.0/
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1225 2024-04-12 15:10:59.072659 sosviz-0.2.0/PKG-INFO
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      993 2024-04-12 15:02:58.000000 sosviz-0.2.0/README.md
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     2096 2024-04-12 15:04:52.000000 sosviz-0.2.0/pyproject.toml
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)       38 2024-04-12 15:10:59.074659 sosviz-0.2.0/setup.cfg
-drwxr-xr-x   0 rjarry    (1000) rjarry    (1000)        0 2024-04-12 15:10:59.069659 sosviz-0.2.0/sosviz/
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)       71 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/__init__.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1612 2024-04-12 14:54:27.000000 sosviz-0.2.0/sosviz/__main__.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     2039 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/bits.py
-drwxr-xr-x   0 rjarry    (1000) rjarry    (1000)        0 2024-04-12 15:10:59.071659 sosviz-0.2.0/sosviz/collect/
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      725 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/collect/__init__.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     2165 2024-03-08 08:54:14.000000 sosviz-0.2.0/sosviz/collect/ip.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1537 2024-03-04 12:50:25.000000 sosviz-0.2.0/sosviz/collect/irq.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     4358 2024-02-22 16:11:04.000000 sosviz-0.2.0/sosviz/collect/libvirt.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     5392 2024-03-11 09:07:30.000000 sosviz-0.2.0/sosviz/collect/ovs.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     2680 2024-02-26 22:48:13.000000 sosviz-0.2.0/sosviz/collect/pci.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1750 2024-03-04 12:50:25.000000 sosviz-0.2.0/sosviz/collect/platform.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1500 2024-03-07 23:48:11.000000 sosviz-0.2.0/sosviz/collect/software.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     2180 2024-04-12 12:42:36.000000 sosviz-0.2.0/sosviz/collect/topo.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1488 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/collect/tuning.py
-drwxr-xr-x   0 rjarry    (1000) rjarry    (1000)        0 2024-04-12 15:10:59.071659 sosviz-0.2.0/sosviz/output/
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      370 2024-04-12 14:56:52.000000 sosviz-0.2.0/sosviz/output/__init__.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)    24102 2024-04-12 13:31:59.000000 sosviz-0.2.0/sosviz/output/dot.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      254 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/output/json.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      258 2024-04-12 14:51:35.000000 sosviz-0.2.0/sosviz/output/svg.py
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      270 2024-02-22 10:50:35.000000 sosviz-0.2.0/sosviz/output/text.py
-drwxr-xr-x   0 rjarry    (1000) rjarry    (1000)        0 2024-04-12 15:10:59.071659 sosviz-0.2.0/sosviz.egg-info/
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)     1225 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/PKG-INFO
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)      613 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/SOURCES.txt
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)        1 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/dependency_links.txt
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)       48 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/entry_points.txt
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)        9 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/requires.txt
--rw-r--r--   0 rjarry    (1000) rjarry    (1000)        7 2024-04-12 15:10:59.000000 sosviz-0.2.0/sosviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 15:30:08.000000 sosviz-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 15:30:16.864430 sosviz-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 15:30:08.000000 sosviz-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-12 15:30:08.000000 sosviz-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:30:16.864430 sosviz-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.860430 sosviz-0.2.2/sosviz/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/bits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz/collect/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/irq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/collect/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 15:30:08.000000 sosviz-0.2.2/sosviz/output/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:30:16.864430 sosviz-0.2.2/sosviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 15:30:16.000000 sosviz-0.2.2/sosviz.egg-info/top_level.txt
```

### Comparing `sosviz-0.2.0/PKG-INFO` & `sosviz-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: sosviz
-Version: 0.2.0
-Summary: Information extractor from sos reports
-Author-email: Robin Jarry <rjarry@redhat.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: graphviz
-
 # sosviz
 
 Extract information from [`sos`](https://github.com/sosreport/sos) reports and
 export it in other formats.
 
 ## Installation
```

### Comparing `sosviz-0.2.0/pyproject.toml` & `sosviz-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [build-system]
 requires = ["setuptools>=40.6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosviz"
-version = "0.2.0"
+version = "0.2.2"
 description = "Information extractor from sos reports"
+license = {file = "LICENSE"}
 dependencies = [
 	"graphviz",
 ]
 requires-python = ">= 3.8"
 readme = "README.md"
 authors = [
 	{name = "Robin Jarry", email = "rjarry@redhat.com"},
 ]
 
+[project.urls]
+Repository = "https://github.com/rjarry/sosviz"
+
 [project.scripts]
 sosviz = "sosviz.__main__:main"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
```

### Comparing `sosviz-0.2.0/sosviz/__main__.py` & `sosviz-0.2.2/sosviz/__main__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/bits.py` & `sosviz-0.2.2/sosviz/bits.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/__init__.py` & `sosviz-0.2.2/sosviz/collect/__init__.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/ip.py` & `sosviz-0.2.2/sosviz/collect/ip.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/irq.py` & `sosviz-0.2.2/sosviz/collect/irq.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/libvirt.py` & `sosviz-0.2.2/sosviz/collect/libvirt.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/ovs.py` & `sosviz-0.2.2/sosviz/collect/ovs.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/pci.py` & `sosviz-0.2.2/sosviz/collect/pci.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/platform.py` & `sosviz-0.2.2/sosviz/collect/platform.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/software.py` & `sosviz-0.2.2/sosviz/collect/software.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/topo.py` & `sosviz-0.2.2/sosviz/collect/topo.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/collect/tuning.py` & `sosviz-0.2.2/sosviz/collect/tuning.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz/output/dot.py` & `sosviz-0.2.2/sosviz/output/dot.py`

 * *Files identical despite different names*

### Comparing `sosviz-0.2.0/sosviz.egg-info/SOURCES.txt` & `sosviz-0.2.2/sosviz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 sosviz/__init__.py
 sosviz/__main__.py
 sosviz/bits.py
 sosviz.egg-info/PKG-INFO
 sosviz.egg-info/SOURCES.txt
```

