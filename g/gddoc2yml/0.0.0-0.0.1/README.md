# Comparing `tmp/gddoc2yml-0.0.0.tar.gz` & `tmp/gddoc2yml-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gddoc2yml-0.0.0.tar", last modified: Fri Apr 12 07:32:20 2024, max compression
+gzip compressed data, was "gddoc2yml-0.0.1.tar", last modified: Fri Apr 12 07:51:28 2024, max compression
```

## Comparing `gddoc2yml-0.0.0.tar` & `gddoc2yml-0.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.673263 gddoc2yml-0.0.0/
--rw-rw-rw-   0        0        0     1077 2024-04-07 18:34:59.000000 gddoc2yml-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-11 06:32:16.000000 gddoc2yml-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2709 2024-04-12 07:32:20.672762 gddoc2yml-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2024-04-12 06:33:07.000000 gddoc2yml-0.0.0/README.md
--rw-rw-rw-   0        0        0     1140 2024-04-12 07:24:06.000000 gddoc2yml-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 07:32:20.673762 gddoc2yml-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.654102 gddoc2yml-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.658610 gddoc2yml-0.0.0/src/gddoc2yml/
--rw-rw-rw-   0        0        0        0 2024-04-11 02:45:37.000000 gddoc2yml-0.0.0/src/gddoc2yml/__init__.py
--rw-rw-rw-   0        0        0     6093 2024-04-11 07:52:24.000000 gddoc2yml-0.0.0/src/gddoc2yml/gdxml2yml.py
--rw-rw-rw-   0        0        0   106910 2024-04-11 02:42:39.000000 gddoc2yml-0.0.0/src/gddoc2yml/make_rst.py
--rw-rw-rw-   0        0        0      166 2024-04-06 18:37:47.000000 gddoc2yml-0.0.0/src/gddoc2yml/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.672262 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/
--rw-rw-rw-   0        0        0     2709 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 07:32:20.000000 gddoc2yml-0.0.0/src/gddoc2yml.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.668145 gddoc2yml-0.0.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-12 07:32:20.671762 gddoc2yml-0.0.0/tests/classes/
--rw-rw-rw-   0        0        0    13286 2024-04-08 03:14:56.000000 gddoc2yml-0.0.0/tests/classes/CollisionObject3D.xml
--rw-rw-rw-   0        0        0    79398 2024-04-08 03:14:56.000000 gddoc2yml-0.0.0/tests/classes/Node.xml
--rw-rw-rw-   0        0        0    20604 2024-04-08 03:14:56.000000 gddoc2yml-0.0.0/tests/classes/Node3D.xml
--rw-rw-rw-   0        0        0    54560 2024-04-08 03:14:56.000000 gddoc2yml-0.0.0/tests/classes/Object.xml
--rw-rw-rw-   0        0        0     6182 2024-04-08 03:14:56.000000 gddoc2yml-0.0.0/tests/classes/PhysicsBody3D.xml
--rw-rw-rw-   0        0        0     2376 2024-04-08 03:14:32.000000 gddoc2yml-0.0.0/tests/classes/StaticBody3D.xml
--rw-rw-rw-   0        0        0      581 2024-04-11 07:52:27.000000 gddoc2yml-0.0.0/tests/test_console.py
--rw-rw-rw-   0        0        0     1007 2024-04-11 07:52:41.000000 gddoc2yml-0.0.0/tests/test_gdxml2yml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.339531 gddoc2yml-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.339531 gddoc2yml-0.0.1/src/gddoc2yml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/gdxml2yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106910 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/make_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/src/gddoc2yml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 07:51:28.000000 gddoc2yml-0.0.1/src/gddoc2yml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:51:28.343531 gddoc2yml-0.0.1/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/CollisionObject3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    79398 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Node.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Node3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    54560 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/Object.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/PhysicsBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/classes/StaticBody3D.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 07:51:16.000000 gddoc2yml-0.0.1/tests/test_gdxml2yml.py
```

### Comparing `gddoc2yml-0.0.0/LICENSE` & `gddoc2yml-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/PKG-INFO` & `gddoc2yml-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: gddoc2yml
-Version: 0.0.0
-Summary: Convert godot xml docs to docfx yml
-Author-email: Nick Maltbie <nick.dmalt@gmail.com>
-Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
-Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
-Keywords: godot,docfx,yml,xml,documentation
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pathvalidate
-Requires-Dist: PyYAML
-
-# Godot Doc 2 Yml
-
-Convert godot xml docs exported via the `godot --doctool` for gdscript
-to yml compatible with docfx.
-
-## References
-
-* [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
-* [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
-* [DocFx -- Github](https://github.com/dotnet/docfx)
-* [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
-
-## Setup
-
-Build package
-
-```bash
-# Install dependencies
-python3 -m pip install -r requirements.txt
-
-# Install build if required
-# python3 -m pip install build
-# Project will be created in dir dist
-python3 -m build
-```
-
-## Linting
-
-Lint using [flake8](https://github.com/pycqa/flake8/) tool.
-
-```bash
-# Run flake8 from .flake8 config file
-# Install via python3 -m pip install flake8
-flake8 .
-```
-
-## Tests
-
-Run tests for project via Python's unittest module -- [Unit testing framework](https://docs.python.org/3/library/unittest.html)
-
-```bash
-python3 -m unittest
-```
-
-### Code Coverage
-
-Compute code coverage using [coveragepy](https://github.com/nedbat/coveragepy)
-
-```bash
-# Get code coverage using coverage
-# Install via python -m pip install coverage
-coverage run -m unittest discover
-
-# Get results
-coverage report -m
-```
-
-## Example
-
-Build godot docs using latest gddoc2yml.
-
-```bash
-# Install from repo
-python3 -m pip install .
-
-# Generate docs using gdxml2yml
-gdxml2yml godot/doc/classes doc/api
-
-# Startup docfx website
-dotnet tool run docfx --serve doc/docfx.json
-```
+Metadata-Version: 2.1
+Name: gddoc2yml
+Version: 0.0.1
+Summary: Convert godot xml docs to docfx yml
+Author-email: Nick Maltbie <nick.dmalt@gmail.com>
+Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
+Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
+Keywords: godot,docfx,yml,xml,documentation
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pathvalidate
+Requires-Dist: PyYAML
+
+# Godot Doc 2 Yml
+
+Convert godot xml docs exported via the `godot --doctool` for gdscript
+to yml compatible with docfx.
+
+## References
+
+* [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
+* [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
+* [DocFx -- Github](https://github.com/dotnet/docfx)
+* [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
+
+## Setup
+
+Build package
+
+```bash
+# Install dependencies
+python3 -m pip install -r requirements.txt
+
+# Install build if required
+# python3 -m pip install build
+# Project will be created in dir dist
+python3 -m build
+```
+
+## Linting
+
+Lint using [flake8](https://github.com/pycqa/flake8/) tool.
+
+```bash
+# Run flake8 from .flake8 config file
+# Install via python3 -m pip install flake8
+flake8 .
+```
+
+## Tests
+
+Run tests for project via Python's unittest module -- [Unit testing framework](https://docs.python.org/3/library/unittest.html)
+
+```bash
+python3 -m unittest
+```
+
+### Code Coverage
+
+Compute code coverage using [coveragepy](https://github.com/nedbat/coveragepy)
+
+```bash
+# Get code coverage using coverage
+# Install via python -m pip install coverage
+coverage run -m unittest discover
+
+# Get results
+coverage report -m
+```
+
+## Example
+
+Build godot docs using latest gddoc2yml.
+
+```bash
+# Install from repo
+python3 -m pip install .
+
+# Generate docs using gdxml2yml
+gdxml2yml godot/doc/classes doc/api
+
+# Startup docfx website
+dotnet tool run docfx --serve doc/docfx.json
+```
```

### Comparing `gddoc2yml-0.0.0/README.md` & `gddoc2yml-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/pyproject.toml` & `gddoc2yml-0.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "pathvalidate>=3.2.0", "PyYAML>=6.0.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gddoc2yml"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Nick Maltbie", email="nick.dmalt@gmail.com" },
 ]
 description = "Convert godot xml docs to docfx yml"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `gddoc2yml-0.0.0/src/gddoc2yml/gdxml2yml.py` & `gddoc2yml-0.0.1/src/gddoc2yml/gdxml2yml.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/src/gddoc2yml/make_rst.py` & `gddoc2yml-0.0.1/src/gddoc2yml/make_rst.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/src/gddoc2yml.egg-info/PKG-INFO` & `gddoc2yml-0.0.1/src/gddoc2yml.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: gddoc2yml
-Version: 0.0.0
-Summary: Convert godot xml docs to docfx yml
-Author-email: Nick Maltbie <nick.dmalt@gmail.com>
-Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
-Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
-Keywords: godot,docfx,yml,xml,documentation
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pathvalidate
-Requires-Dist: PyYAML
-
-# Godot Doc 2 Yml
-
-Convert godot xml docs exported via the `godot --doctool` for gdscript
-to yml compatible with docfx.
-
-## References
-
-* [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
-* [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
-* [DocFx -- Github](https://github.com/dotnet/docfx)
-* [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
-
-## Setup
-
-Build package
-
-```bash
-# Install dependencies
-python3 -m pip install -r requirements.txt
-
-# Install build if required
-# python3 -m pip install build
-# Project will be created in dir dist
-python3 -m build
-```
-
-## Linting
-
-Lint using [flake8](https://github.com/pycqa/flake8/) tool.
-
-```bash
-# Run flake8 from .flake8 config file
-# Install via python3 -m pip install flake8
-flake8 .
-```
-
-## Tests
-
-Run tests for project via Python's unittest module -- [Unit testing framework](https://docs.python.org/3/library/unittest.html)
-
-```bash
-python3 -m unittest
-```
-
-### Code Coverage
-
-Compute code coverage using [coveragepy](https://github.com/nedbat/coveragepy)
-
-```bash
-# Get code coverage using coverage
-# Install via python -m pip install coverage
-coverage run -m unittest discover
-
-# Get results
-coverage report -m
-```
-
-## Example
-
-Build godot docs using latest gddoc2yml.
-
-```bash
-# Install from repo
-python3 -m pip install .
-
-# Generate docs using gdxml2yml
-gdxml2yml godot/doc/classes doc/api
-
-# Startup docfx website
-dotnet tool run docfx --serve doc/docfx.json
-```
+Metadata-Version: 2.1
+Name: gddoc2yml
+Version: 0.0.1
+Summary: Convert godot xml docs to docfx yml
+Author-email: Nick Maltbie <nick.dmalt@gmail.com>
+Project-URL: Homepage, https://github.com/nicholas-maltbie/gddoc2yml
+Project-URL: Issues, https://github.com/nicholas-maltbie/gddoc2yml/issues
+Keywords: godot,docfx,yml,xml,documentation
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pathvalidate
+Requires-Dist: PyYAML
+
+# Godot Doc 2 Yml
+
+Convert godot xml docs exported via the `godot --doctool` for gdscript
+to yml compatible with docfx.
+
+## References
+
+* [Godot -- CLI Reference](https://docs.godotengine.org/en/stable/tutorials/editor/command_line_tutorial.html#command-line-reference)
+* [Godot -- make_rst.py](https://github.com/godotengine/godot/blob/master/doc/tools/make_rst.py)
+* [DocFx -- Github](https://github.com/dotnet/docfx)
+* [DocFx -- Introduction to Multiple Languages Support](https://xxred.gitee.io/docfx/tutorial/universalreference/intro_multiple_langs_support.html)
+
+## Setup
+
+Build package
+
+```bash
+# Install dependencies
+python3 -m pip install -r requirements.txt
+
+# Install build if required
+# python3 -m pip install build
+# Project will be created in dir dist
+python3 -m build
+```
+
+## Linting
+
+Lint using [flake8](https://github.com/pycqa/flake8/) tool.
+
+```bash
+# Run flake8 from .flake8 config file
+# Install via python3 -m pip install flake8
+flake8 .
+```
+
+## Tests
+
+Run tests for project via Python's unittest module -- [Unit testing framework](https://docs.python.org/3/library/unittest.html)
+
+```bash
+python3 -m unittest
+```
+
+### Code Coverage
+
+Compute code coverage using [coveragepy](https://github.com/nedbat/coveragepy)
+
+```bash
+# Get code coverage using coverage
+# Install via python -m pip install coverage
+coverage run -m unittest discover
+
+# Get results
+coverage report -m
+```
+
+## Example
+
+Build godot docs using latest gddoc2yml.
+
+```bash
+# Install from repo
+python3 -m pip install .
+
+# Generate docs using gdxml2yml
+gdxml2yml godot/doc/classes doc/api
+
+# Startup docfx website
+dotnet tool run docfx --serve doc/docfx.json
+```
```

### Comparing `gddoc2yml-0.0.0/src/gddoc2yml.egg-info/SOURCES.txt` & `gddoc2yml-0.0.1/src/gddoc2yml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/CollisionObject3D.xml` & `gddoc2yml-0.0.1/tests/classes/CollisionObject3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/Node.xml` & `gddoc2yml-0.0.1/tests/classes/Node.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/Node3D.xml` & `gddoc2yml-0.0.1/tests/classes/Node3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/Object.xml` & `gddoc2yml-0.0.1/tests/classes/Object.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/PhysicsBody3D.xml` & `gddoc2yml-0.0.1/tests/classes/PhysicsBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/classes/StaticBody3D.xml` & `gddoc2yml-0.0.1/tests/classes/StaticBody3D.xml`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/test_console.py` & `gddoc2yml-0.0.1/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `gddoc2yml-0.0.0/tests/test_gdxml2yml.py` & `gddoc2yml-0.0.1/tests/test_gdxml2yml.py`

 * *Files identical despite different names*

