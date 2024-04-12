# Comparing `tmp/pixi-kernel-0.1.2.tar.gz` & `tmp/pixi_kernel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixi-kernel-0.1.2.tar", last modified: Mon Apr  8 02:39:27 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pixi-kernel-0.1.2.tar` & `pixi_kernel-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.624547 pixi-kernel-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/assets/kernel.json
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/assets/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:39:27.624547 pixi-kernel-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/pixi_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 02:39:23.000000 pixi-kernel-0.1.2/src/pixi_kernel/pixi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:39:27.620547 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 02:39:27.000000 pixi-kernel-0.1.2/src/pixi_kernel.egg-info/top_level.txt
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/codecov.yml
+-rw-r--r--   0        0        0   494805 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pixi.lock
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pixi.toml
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0   169085 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/assets/launch-dark.png
+-rw-r--r--   0        0        0   176986 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/assets/launch-light.png
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-bash/kernel.json
+-rw-r--r--   0        0        0   801365 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-bash/logo-svg.svg
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/kernel.js
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/kernel.json
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-64x64.png
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-ir/logo-svg.svg
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/kernel.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-32x32.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-64x64.png
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-python3/logo-svg.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp11/logo-svg.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp14/logo-svg.svg
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/kernels/pixi-kernel-xcpp17/logo-svg.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/__init__.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/errors.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/pixi.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/src/pixi_kernel/provisioner.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/kernel.py
+-rw-r--r--   0        0        0   123358 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/pixi.lock
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/bash_kernel/pixi.toml
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/kernel.py
+-rw-r--r--   0        0        0   119641 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/pixi.lock
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/ipykernel/pixi.toml
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/kernel.py
+-rw-r--r--   0        0        0   329338 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/pixi.lock
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/r-irkernel/pixi.toml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/kernel.py
+-rw-r--r--   0        0        0    77254 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/pixi.lock
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/integration/xeus-cling/pixi.toml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/test_pixi.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/missing_ipykernel/pixi.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/pixi_project/pixi.toml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/tests/unit/data/pyproject_project/pyproject.toml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/README.md
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 pixi_kernel-0.2.0/PKG-INFO
```

### Comparing `pixi-kernel-0.1.2/LICENSE` & `pixi_kernel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixi-kernel-0.1.2/pyproject.toml` & `pixi_kernel-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixi-kernel"
-version = "0.1.2"
+version = "0.2.0"
 description = "Python Jupyter kernel using Pixi for reproducible notebooks"
 license = { text = "MIT" }
 authors = [
     { name = "Renan Rodrigues dos Santos", email = "renan.engmec@gmail.com" },
 ]
 
 readme = "README.md"
@@ -26,26 +26,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 requires-python = ">=3.8,<4.0"
-dependencies = ["ipykernel>=6,<7", "msgspec>=0.18,<1"]
+dependencies = ["jupyter-client>=7", "msgspec>=0.18"]
 
 [project.urls]
 Documentation = "https://github.com/renan-r-santos/pixi-kernel"
 Homepage = "https://github.com/renan-r-santos/pixi-kernel"
 Repository = "https://github.com/renan-r-santos/pixi-kernel"
 
-[tool.setuptools.data-files]
-"share/jupyter/kernels/pixi_kernel" = [
-    "assets/kernel.json",
-    "assets/logo-64x64.png",
-]
+[project.entry-points."jupyter_client.kernel_provisioners"]
+pixi-provisioner = "pixi_kernel.provisioner:PixiProvisioner"
 
 [tool.ruff]
 src = ["src"]
 line-length = 99
 
 [tool.ruff.lint]
 extend-select = [
@@ -72,12 +69,15 @@
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
 source = ["src/", ".pixi/envs/**/lib/python*/site-packages/"]
 
 [tool.coverage.report]
-fail_under = 60
+fail_under = 65
+
+[tool.hatch.build.targets.wheel.shared-data]
+"kernels" = "share/jupyter/kernels"
 
 [build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

