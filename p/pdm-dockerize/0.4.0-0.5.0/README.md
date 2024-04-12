# Comparing `tmp/pdm_dockerize-0.4.0.tar.gz` & `tmp/pdm_dockerize-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_dockerize-0.4.0.tar", last modified: Thu Apr  4 17:57:42 2024, max compression
+gzip compressed data, was "pdm_dockerize-0.5.0.tar", last modified: Fri Apr 12 15:03:46 2024, max compression
```

## Comparing `pdm_dockerize-0.4.0.tar` & `pdm_dockerize-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1070 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/LICENSE
--rw-r--r--   0        0        0     4591 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/README.md
--rw-r--r--   0        0        0     4026 2024-04-04 17:57:42.411753 pdm_dockerize-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-04 17:57:42.407753 pdm_dockerize-0.4.0/src/pdm_dockerize/VERSION
--rw-r--r--   0        0        0      321 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/commands.py
--rw-r--r--   0        0        0      638 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/config.py
--rw-r--r--   0        0        0     9236 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/entrypoint.py
--rw-r--r--   0        0        0      596 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/filters.py
--rw-r--r--   0        0        0     3534 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/installer.py
--rw-r--r--   0        0        0        0 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/src/pdm_dockerize/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-all].sh
--rw-r--r--   0        0        0      575 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh
--rw-r--r--   0        0        0      486 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all-but-prefix].sh
--rw-r--r--   0        0        0      717 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh
--rw-r--r--   0        0        0      458 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-list].sh
--rw-r--r--   0        0        0      470 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-prefix-except].sh
--rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[no-filter].sh
--rw-r--r--   0        0        0      440 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_global_env.sh
--rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_global_env_file.sh
--rw-r--r--   0        0        0      329 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_pythonpath_explicit_src_layout.sh
--rw-r--r--   0        0        0      329 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_pythonpath_implicit_src_layout.sh
--rw-r--r--   0        0        0      821 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh
--rw-r--r--   0        0        0      694 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh
--rw-r--r--   0        0        0      456 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[call-with-arguments].sh
--rw-r--r--   0        0        0      418 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[call].sh
--rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-dict].sh
--rw-r--r--   0        0        0      413 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-list].sh
--rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-str].sh
--rw-r--r--   0        0        0      419 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[composite-inline].sh
--rw-r--r--   0        0        0      410 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[composite].sh
--rw-r--r--   0        0        0      470 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env].sh
--rw-r--r--   0        0        0      593 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override-precedance].sh
--rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override].sh
--rw-r--r--   0        0        0      593 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-precedance].sh
--rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file].sh
--rw-r--r--   0        0        0      316 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[no_script].sh
--rw-r--r--   0        0        0      554 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[pre-post].sh
--rw-r--r--   0        0        0      474 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env].sh
--rw-r--r--   0        0        0      547 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env_file].sh
--rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shell].sh
--rw-r--r--   0        0        0      624 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh
--rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist.sh
--rw-r--r--   0        0        0      381 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist_to_target.sh
--rw-r--r--   0        0        0     1662 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     6305 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_entrypoint.py
--rw-r--r--   0        0        0      953 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_filters.py
--rw-r--r--   0        0        0     4011 2024-04-04 17:57:20.983804 pdm_dockerize-0.4.0/tests/test_pdm_dockerize.py
--rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 pdm_dockerize-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5105 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/README.md
+-rw-r--r--   0        0        0     4021 2024-04-12 15:03:46.955520 pdm_dockerize-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-12 15:03:46.951520 pdm_dockerize-0.5.0/src/pdm_dockerize/VERSION
+-rw-r--r--   0        0        0      321 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/commands.py
+-rw-r--r--   0        0        0      638 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/config.py
+-rw-r--r--   0        0        0     9236 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/entrypoint.py
+-rw-r--r--   0        0        0      596 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/filters.py
+-rw-r--r--   0        0        0     3519 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/installer.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/src/pdm_dockerize/py.typed
+-rw-r--r--   0        0        0        0 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      316 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-all].sh
+-rw-r--r--   0        0        0      575 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh
+-rw-r--r--   0        0        0      486 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all-but-prefix].sh
+-rw-r--r--   0        0        0      717 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh
+-rw-r--r--   0        0        0      458 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[include-list].sh
+-rw-r--r--   0        0        0      470 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[include-prefix-except].sh
+-rw-r--r--   0        0        0      316 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[no-filter].sh
+-rw-r--r--   0        0        0      440 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_global_env.sh
+-rw-r--r--   0        0        0      547 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_global_env_file.sh
+-rw-r--r--   0        0        0      329 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_pythonpath_explicit_src_layout.sh
+-rw-r--r--   0        0        0      329 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_pythonpath_implicit_src_layout.sh
+-rw-r--r--   0        0        0      821 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh
+-rw-r--r--   0        0        0      694 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh
+-rw-r--r--   0        0        0      456 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[call-with-arguments].sh
+-rw-r--r--   0        0        0      418 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[call].sh
+-rw-r--r--   0        0        0      381 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-dict].sh
+-rw-r--r--   0        0        0      413 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-list].sh
+-rw-r--r--   0        0        0      381 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[cmd-as-str].sh
+-rw-r--r--   0        0        0      419 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[composite-inline].sh
+-rw-r--r--   0        0        0      410 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[composite].sh
+-rw-r--r--   0        0        0      470 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env].sh
+-rw-r--r--   0        0        0      593 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override-precedance].sh
+-rw-r--r--   0        0        0      547 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override].sh
+-rw-r--r--   0        0        0      593 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-precedance].sh
+-rw-r--r--   0        0        0      547 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file].sh
+-rw-r--r--   0        0        0      316 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[no_script].sh
+-rw-r--r--   0        0        0      554 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[pre-post].sh
+-rw-r--r--   0        0        0      474 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env].sh
+-rw-r--r--   0        0        0      547 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env_file].sh
+-rw-r--r--   0        0        0      381 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[shell].sh
+-rw-r--r--   0        0        0      624 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh
+-rw-r--r--   0        0        0      381 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist.sh
+-rw-r--r--   0        0        0      381 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/__snapshots__/test_pdm_dockerize/test_generate_docker_dist_to_target.sh
+-rw-r--r--   0        0        0     1662 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     6305 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/test_entrypoint.py
+-rw-r--r--   0        0        0      953 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/test_filters.py
+-rw-r--r--   0        0        0     4011 2024-04-12 15:03:22.571335 pdm_dockerize-0.5.0/tests/test_pdm_dockerize.py
+-rw-r--r--   0        0        0     6376 1970-01-01 00:00:00.000000 pdm_dockerize-0.5.0/PKG-INFO
```

### Comparing `pdm_dockerize-0.4.0/LICENSE` & `pdm_dockerize-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/README.md` & `pdm_dockerize-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pdm-dockerize
 
 [![CI](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml/badge.svg)](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/noirbizarre/pdm-dockerize/main.svg)](https://results.pre-commit.ci/latest/github/noirbizarre/pdm-dockerize/main)
 [![PyPI](https://img.shields.io/pypi/v/pdm-dockerize)](https://pypi.org/project/pdm-dockerize/)
 [![PyPI - License](https://img.shields.io/pypi/l/pdm-dockerize)](https://pypi.org/project/pdm-dockerize/)
 
-Help generating docker image from PDM projects
+Help generating docker image from PDM projects.
 
 ## Installation
 
 Install `pdm-dockerize`:
 
 ### With `pipx`
 
@@ -182,10 +182,19 @@
 This file will only be loaded in the docker entrypoint.
 
 ```toml
 [tool.pdm.dockerize]
 env_file = "docker.env"
 ```
 
+## Internals
+
+This plugin works by providing by subclassing some `pdm.installers` classes to reuse the installation process:
+- `DockerizeInstallManager`, a `pdm` `InstallManager` filtering binaries
+- `DockerizeSynchronizer`, a `pdm` `Synchronizer` using a `DockerizeInstallManager` as `InstallManager`
+- `FilteringDestination`, a `pdm` `InstallDestination` filtering binaries
+
+This way, the dockerization is using the same installation process just tuned for docker and augmented with `pdm-dockerize` specifics.
+
 ## Contributing
 
 Read the [dedicated contributing guidelines](./CONTRIBUTING.md).
```

### Comparing `pdm_dockerize-0.4.0/pyproject.toml` & `pdm_dockerize-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Code Generators",
     "Typing :: Typed",
 ]
 dependencies = [
-    "pdm>=2.13",
+    "pdm>=2.14",
 ]
-version = "0.4.0"
+version = "0.5.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/noirbizarre/pdm-dockerize"
 Documentation = "https://github.com/noirbizarre/pdm-dockerize#readme"
@@ -63,18 +63,17 @@
     "pytest>=7.1.2",
     "pytest-sugar>=0.9.5",
     "pytest-cov>=3.0.0",
     "syrupy>=3.0.6",
     "shellcheck-py>=0.9.0.6",
 ]
 lint = [
-    "black>=23.7.0",
     "codespell>=2.2.6",
     "mypy>=1.5.1",
-    "ruff>=0.1.7",
+    "ruff>=0.3.0",
     "tomli; python_version<'3.11'",
 ]
 tox = [
     "tox",
     "tox-pdm>=0.5",
 ]
 release = [
@@ -93,16 +92,16 @@
 help = "Lint all tracked files using pre-commit"
 cmd = "pre-commit run --all-files"
 
 [tool.pdm.scripts.format]
 help = "Format the code according to known rules"
 composite = [
     "codespell --write-changes --interactive 2",
-    "ruff --fix-only --show-fixes src tests",
-    "black src tests",
+    "ruff check --select I --fix-only --show-fixes src tests",
+    "ruff format src tests",
 ]
 
 [tool.pdm.scripts.typing]
 help = "Full typing linting (includes imported packages and uncommmited files)"
 cmd = "mypy src tests --warn-unused-ignores"
 
 [tool.pdm.scripts.cover]
@@ -133,15 +132,15 @@
 name = "emotional"
 github = "noirbizarre/pdm-dockerize"
 order_by_scope = true
 version_provider = "scm"
 major_version_zero = true
 
 [tool.pytest.ini_options]
-addopts = "-ra"
+addopts = "-rfEX"
 norecursedirs = ".git build dist"
 testpaths = [
     "src/",
     "tests/",
 ]
 
 [tool.coverage.run]
@@ -156,34 +155,33 @@
 [tool.coverage.report]
 exclude_also = [
     "def __repr__",
     "if TYPE_CHECKING:",
 ]
 ignore_errors = true
 
-[tool.black]
-line-length = 100
-
 [tool.ruff]
 line-length = 100
 respect-gitignore = true
+src = [
+    "src",
+    "tests",
+]
+
+[tool.ruff.lint]
 select = [
     "F",
     "E",
     "W",
     "C",
     "UP",
     "I001",
 ]
-src = [
-    "src",
-    "tests",
-]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = [
     "pdm_dockerize",
 ]
 known-third-party = [
     "pytest",
     "syrupy",
 ]
```

### Comparing `pdm_dockerize-0.4.0/src/pdm_dockerize/commands.py` & `pdm_dockerize-0.5.0/src/pdm_dockerize/commands.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/src/pdm_dockerize/config.py` & `pdm_dockerize-0.5.0/src/pdm_dockerize/config.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/src/pdm_dockerize/entrypoint.py` & `pdm_dockerize-0.5.0/src/pdm_dockerize/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/src/pdm_dockerize/filters.py` & `pdm_dockerize-0.5.0/src/pdm_dockerize/filters.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/src/pdm_dockerize/installer.py` & `pdm_dockerize-0.5.0/src/pdm_dockerize/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable
 
 from installer.destinations import Scheme
 from installer.records import RecordEntry
 from pdm.compat import Distribution
 from pdm.installers import Synchronizer
-from pdm.installers.installers import InstallDestination, PackageWheelSource, install
+from pdm.installers.installers import InstallDestination, WheelFile, install
 from pdm.installers.manager import InstallManager
 
 from . import filters
 
 if TYPE_CHECKING:
     from installer.scripts import ScriptSection
     from pdm.environments import BaseEnvironment
@@ -43,16 +43,16 @@
             scheme_dict=self.environment.get_paths(),
             interpreter=str(self.environment.interpreter.executable),
             script_kind=self.environment.script_kind,
             include=self.include,
             exclude=self.exclude,
         )
 
-        source = PackageWheelSource(prepared.get_cached_package())
-        dist_info = install(source, destination, additional_metadata)
+        with WheelFile.open(prepared.build()) as source:
+            dist_info = install(source, destination, additional_metadata)
         return Distribution.at(dist_info)
 
 
 class DockerizeSynchronizer(Synchronizer):
     """A `Synchronizer` using the `DockerizeInstallManager`"""
 
     def get_manager(self) -> InstallManager:
```

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[exclude-list].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_filtering[include-all].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_global_env_file.sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_global_env_file.sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder-with-defaults].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[args-placeholder].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override-precedance].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override-precedance].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-override].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-precedance].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file-precedance].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[env_file].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[pre-post].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[pre-post].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env_file].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[shared-env_file].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh` & `pdm_dockerize-0.5.0/tests/__snapshots__/test_entrypoint/test_serialization[whitespaces].sh`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/conftest.py` & `pdm_dockerize-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/test_entrypoint.py` & `pdm_dockerize-0.5.0/tests/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/test_filters.py` & `pdm_dockerize-0.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/tests/test_pdm_dockerize.py` & `pdm_dockerize-0.5.0/tests/test_pdm_dockerize.py`

 * *Files identical despite different names*

### Comparing `pdm_dockerize-0.4.0/PKG-INFO` & `pdm_dockerize-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-dockerize
-Version: 0.4.0
+Version: 0.5.0
 Summary: Help generating docker images from PDM projects
 Author-Email: Axel Haustant <noirbizarre@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -20,25 +20,25 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/noirbizarre/pdm-dockerize
 Project-URL: Documentation, https://github.com/noirbizarre/pdm-dockerize#readme
 Project-URL: Repository, https://github.com/noirbizarre/pdm-dockerize
 Project-URL: Issues, https://github.com/noirbizarre/pdm-dockerize/issues
 Requires-Python: >=3.8.1
-Requires-Dist: pdm>=2.13
+Requires-Dist: pdm>=2.14
 Description-Content-Type: text/markdown
 
 # pdm-dockerize
 
 [![CI](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml/badge.svg)](https://github.com/noirbizarre/pdm-dockerize/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/noirbizarre/pdm-dockerize/main.svg)](https://results.pre-commit.ci/latest/github/noirbizarre/pdm-dockerize/main)
 [![PyPI](https://img.shields.io/pypi/v/pdm-dockerize)](https://pypi.org/project/pdm-dockerize/)
 [![PyPI - License](https://img.shields.io/pypi/l/pdm-dockerize)](https://pypi.org/project/pdm-dockerize/)
 
-Help generating docker image from PDM projects
+Help generating docker image from PDM projects.
 
 ## Installation
 
 Install `pdm-dockerize`:
 
 ### With `pipx`
 
@@ -211,10 +211,19 @@
 This file will only be loaded in the docker entrypoint.
 
 ```toml
 [tool.pdm.dockerize]
 env_file = "docker.env"
 ```
 
+## Internals
+
+This plugin works by providing by subclassing some `pdm.installers` classes to reuse the installation process:
+- `DockerizeInstallManager`, a `pdm` `InstallManager` filtering binaries
+- `DockerizeSynchronizer`, a `pdm` `Synchronizer` using a `DockerizeInstallManager` as `InstallManager`
+- `FilteringDestination`, a `pdm` `InstallDestination` filtering binaries
+
+This way, the dockerization is using the same installation process just tuned for docker and augmented with `pdm-dockerize` specifics.
+
 ## Contributing
 
 Read the [dedicated contributing guidelines](./CONTRIBUTING.md).
```

