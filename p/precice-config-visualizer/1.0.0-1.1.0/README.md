# Comparing `tmp/precice-config-visualizer-1.0.0.tar.gz` & `tmp/precice-config-visualizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice-config-visualizer-1.0.0.tar", last modified: Thu Apr 11 13:27:21 2024, max compression
+gzip compressed data, was "precice-config-visualizer-1.1.0.tar", last modified: Thu Apr 11 14:54:24 2024, max compression
```

## Comparing `precice-config-visualizer-1.0.0.tar` & `precice-config-visualizer-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.983594 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:27:21.000000 precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:21.983594 precice-config-visualizer-1.0.0/preciceconfigvisualizer/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2473 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/preciceconfigvisualizer/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/preciceconfigvisualizer/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:27:21.987594 precice-config-visualizer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:27:13.000000 precice-config-visualizer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:54:24.442190 precice-config-visualizer-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-11 14:54:24.442190 precice-config-visualizer-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:54:24.442190 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 14:54:24.000000 precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:54:24.442190 precice-config-visualizer-1.1.0/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2473 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/preciceconfigvisualizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:54:24.442190 precice-config-visualizer-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:54:08.000000 precice-config-visualizer-1.1.0/setup.py
```

### Comparing `precice-config-visualizer-1.0.0/LICENSE` & `precice-config-visualizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.0.0/PKG-INFO` & `precice-config-visualizer-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
@@ -18,27 +18,35 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
 Requires-Dist: typing_extensions
+Provides-Extra: gui
+Requires-Dist: precice-config-visualizer-gui; extra == "gui"
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
 
 Install directly from PyPi using [pipx](https://pipx.pypa.io/stable/) or via pip:
 
 ```
 pipx install precice-config-visualizer
 ```
 
+To also install [the GUI](https://pypi.org/project/precice-config-visualizer-gui/), run:
+
+```
+pipx install 'precice-config-visualizer[gui]'
+```
+
 ## Usage
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
```

### Comparing `precice-config-visualizer-1.0.0/README.md` & `precice-config-visualizer-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 Install directly from PyPi using [pipx](https://pipx.pypa.io/stable/) or via pip:
 
 ```
 pipx install precice-config-visualizer
 ```
 
+To also install [the GUI](https://pypi.org/project/precice-config-visualizer-gui/), run:
+
+```
+pipx install 'precice-config-visualizer[gui]'
+```
+
 ## Usage
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
```

### Comparing `precice-config-visualizer-1.0.0/precice_config_visualizer.egg-info/PKG-INFO` & `precice-config-visualizer-1.1.0/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.0.0
+Version: 1.1.0
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
@@ -18,27 +18,35 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: pydot
 Requires-Dist: typing_extensions
+Provides-Extra: gui
+Requires-Dist: precice-config-visualizer-gui; extra == "gui"
 
 # preCICE Config-Visualizer
 
 The `config-visualizer` is a tool meant to help visualize and debug precice configuration xml files. This tool produces a dot file as output, which visualizes the various participants, communicators and meshes defined in the configuration file and the movement of data between them.
 
 ## Installation options
 
 Install directly from PyPi using [pipx](https://pipx.pypa.io/stable/) or via pip:
 
 ```
 pipx install precice-config-visualizer
 ```
 
+To also install [the GUI](https://pypi.org/project/precice-config-visualizer-gui/), run:
+
+```
+pipx install 'precice-config-visualizer[gui]'
+```
+
 ## Usage
 
 ```
 precice-config-visualizer --help
 precice-config-visualizer [OPTIONS] [-o OUTFILE] [<CONFIG-FILE>]
 ```
```

### Comparing `precice-config-visualizer-1.0.0/preciceconfigvisualizer/cli.py` & `precice-config-visualizer-1.1.0/preciceconfigvisualizer/cli.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.0.0/preciceconfigvisualizer/common.py` & `precice-config-visualizer-1.1.0/preciceconfigvisualizer/common.py`

 * *Files identical despite different names*

### Comparing `precice-config-visualizer-1.0.0/pyproject.toml` & `precice-config-visualizer-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 Documentation = "https://precice.org/tooling-config-visualization.html"
 Repository = "https://github.com/precice/config-visualizer.git"
 "Bug Tracker" = "https://github.com/precice/config-visualizer/issues"
 
 [project.scripts]
 precice-config-visualizer = "preciceconfigvisualizer.cli:main"
 
+[project.optional-dependencies]
+gui = [ "precice-config-visualizer-gui" ]
+
 [tool.setuptools]
 packages=["preciceconfigvisualizer"]
 
 [tool.setuptools-git-versioning]
 enabled = true
 
 [tool.mypy]
```

