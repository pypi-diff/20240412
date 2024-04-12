# Comparing `tmp/fastcs-0.2.tar.gz` & `tmp/fastcs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcs-0.2.tar", last modified: Thu Jan 25 15:03:51 2024, max compression
+gzip compressed data, was "fastcs-0.3.0.tar", last modified: Fri Apr 12 15:21:56 2024, max compression
```

## Comparing `fastcs-0.2.tar` & `fastcs-0.3.0.tar`

### file list

```diff
@@ -1,103 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.454254 fastcs-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-01-25 15:03:42.000000 fastcs-0.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-25 15:03:42.000000 fastcs-0.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.438254 fastcs-0.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-25 15:03:42.000000 fastcs-0.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-25 15:03:42.000000 fastcs-0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-25 15:03:42.000000 fastcs-0.2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3043 2024-01-25 15:03:42.000000 fastcs-0.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-01-25 15:03:42.000000 fastcs-0.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-25 15:03:42.000000 fastcs-0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-25 15:03:42.000000 fastcs-0.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-25 15:03:42.000000 fastcs-0.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-25 15:03:42.000000 fastcs-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-25 15:03:42.000000 fastcs-0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.442254 fastcs-0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-25 15:03:42.000000 fastcs-0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-25 15:03:42.000000 fastcs-0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-25 15:03:42.000000 fastcs-0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-25 15:03:42.000000 fastcs-0.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-25 15:03:42.000000 fastcs-0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-25 15:03:42.000000 fastcs-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-01-25 15:03:51.454254 fastcs-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-25 15:03:42.000000 fastcs-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-25 15:03:42.000000 fastcs-0.2/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-25 15:03:42.000000 fastcs-0.2/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-01-25 15:03:42.000000 fastcs-0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-25 15:03:42.000000 fastcs-0.2/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-25 15:03:42.000000 fastcs-0.2/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-01-25 15:03:42.000000 fastcs-0.2/docs/images/fastcs.svg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-25 15:03:42.000000 fastcs-0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-25 15:03:42.000000 fastcs-0.2/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-25 15:03:42.000000 fastcs-0.2/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-25 15:03:42.000000 fastcs-0.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-25 15:03:42.000000 fastcs-0.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.446254 fastcs-0.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-25 15:03:42.000000 fastcs-0.2/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-01-25 15:03:42.000000 fastcs-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 15:03:51.454254 fastcs-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.438254 fastcs-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.450254 fastcs-0.2/src/fastcs/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.450254 fastcs-0.2/src/fastcs/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/asyncio_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.454254 fastcs-0.2/src/fastcs/backends/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/epics/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/epics/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/epics/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/backends/epics/ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1637 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/cs_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-25 15:03:42.000000 fastcs-0.2/src/fastcs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.454254 fastcs-0.2/src/fastcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-25 15:03:51.000000 fastcs-0.2/src/fastcs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 15:03:51.454254 fastcs-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-25 15:03:42.000000 fastcs-0.2/tests/test_boilerplate_removed.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-25 15:03:42.000000 fastcs-0.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.916255 fastcs-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 15:21:49.000000 fastcs-0.3.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 15:21:49.000000 fastcs-0.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.900255 fastcs-0.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.904255 fastcs-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 15:21:49.000000 fastcs-0.3.0/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-12 15:21:49.000000 fastcs-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 15:21:49.000000 fastcs-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 15:21:49.000000 fastcs-0.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 15:21:49.000000 fastcs-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 15:21:49.000000 fastcs-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 15:21:56.916255 fastcs-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-12 15:21:49.000000 fastcs-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 15:21:49.000000 fastcs-0.3.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/images/fastcs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.908255 fastcs-0.3.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 15:21:49.000000 fastcs-0.3.0/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-12 15:21:49.000000 fastcs-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:21:56.916255 fastcs-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.900255 fastcs-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/asyncio_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/backends/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/backends/epics/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/connections/ip_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1645 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/cs_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-12 15:21:49.000000 fastcs-0.3.0/src/fastcs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/src/fastcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 15:21:56.000000 fastcs-0.3.0/src/fastcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:21:56.912255 fastcs-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/test_boilerplate_removed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 15:21:49.000000 fastcs-0.3.0/tests/test_cli.py
```

### Comparing `fastcs-0.2/.github/pages/make_switcher.py` & `fastcs-0.3.0/.github/pages/make_switcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,94 @@
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
-from typing import List, Optional
 
 
-def report_output(stdout: bytes, label: str) -> List[str]:
+def report_output(stdout: bytes, label: str) -> list[str]:
     ret = stdout.decode().strip().split("\n")
     print(f"{label}: {ret}")
     return ret
 
 
-def get_branch_contents(ref: str) -> List[str]:
+def get_branch_contents(ref: str) -> list[str]:
     """Get the list of directories in a branch."""
     stdout = check_output(["git", "ls-tree", "-d", "--name-only", ref])
     return report_output(stdout, "Branch contents")
 
 
-def get_sorted_tags_list() -> List[str]:
+def get_sorted_tags_list() -> list[str]:
     """Get a list of sorted tags in descending order from the repository."""
     stdout = check_output(["git", "tag", "-l", "--sort=-v:refname"])
     return report_output(stdout, "Tags list")
 
 
-def get_versions(ref: str, add: Optional[str], remove: Optional[str]) -> List[str]:
+def get_versions(ref: str, add: str | None) -> list[str]:
     """Generate the file containing the list of all GitHub Pages builds."""
     # Get the directories (i.e. builds) from the GitHub Pages branch
     try:
         builds = set(get_branch_contents(ref))
     except CalledProcessError:
         builds = set()
         logging.warning(f"Cannot get {ref} contents")
 
     # Add and remove from the list of builds
     if add:
         builds.add(add)
-    if remove:
-        assert remove in builds, f"Build '{remove}' not in {sorted(builds)}"
-        builds.remove(remove)
 
     # Get a sorted list of tags
     tags = get_sorted_tags_list()
 
     # Make the sorted versions list from main branches and tags
-    versions: List[str] = []
+    versions: list[str] = []
     for version in ["master", "main"] + tags:
         if version in builds:
             versions.append(version)
             builds.remove(version)
 
     # Add in anything that is left to the bottom
     versions += sorted(builds)
     print(f"Sorted versions: {versions}")
     return versions
 
 
 def write_json(path: Path, repository: str, versions: str):
     org, repo_name = repository.split("/")
+    pages_url = f"https://{org}.github.io"
+    if repo_name != f"{org}.github.io":
+        # Only add the repo name if it isn't the source for the org pages site
+        pages_url += f"/{repo_name}"
     struct = [
-        {"version": version, "url": f"https://{org}.github.io/{repo_name}/{version}/"}
-        for version in versions
+        {"version": version, "url": f"{pages_url}/{version}/"} for version in versions
     ]
     text = json.dumps(struct, indent=2)
     print(f"JSON switcher:\n{text}")
     path.write_text(text, encoding="utf-8")
 
 
 def main(args=None):
     parser = ArgumentParser(
-        description="Make a versions.txt file from gh-pages directories"
+        description="Make a versions.json file from gh-pages directories"
     )
     parser.add_argument(
         "--add",
         help="Add this directory to the list of existing directories",
     )
     parser.add_argument(
-        "--remove",
-        help="Remove this directory from the list of existing directories",
-    )
-    parser.add_argument(
         "repository",
         help="The GitHub org and repository name: ORG/REPO",
     )
     parser.add_argument(
         "output",
         type=Path,
         help="Path of write switcher.json to",
     )
     args = parser.parse_args(args)
 
     # Write the versions file
-    versions = get_versions("origin/gh-pages", args.add, args.remove)
+    versions = get_versions("origin/gh-pages", args.add)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fastcs-0.2/.gitignore` & `fastcs-0.3.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
-.venv
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
@@ -52,15 +51,14 @@
 *.pot
 
 # Django stuff:
 *.log
 
 # Sphinx documentation
 docs/_build/
-docs/**/_autosummary
 
 # PyBuilder
 target/
 
 # likely venv names
 .venv*
 venv*
```

### Comparing `fastcs-0.2/.vscode/launch.json` & `fastcs-0.3.0/.vscode/launch.json`

 * *Files 25% similar despite different names*

```diff
@@ -2,24 +2,22 @@
     // Use IntelliSense to learn about possible attributes.
     // Hover to view descriptions of existing attributes.
     // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
     "version": "0.2.0",
     "configurations": [
         {
             "name": "Debug Unit Test",
-            "type": "python",
+            "type": "debugpy",
             "request": "launch",
             "justMyCode": false,
             "program": "${file}",
             "purpose": [
                 "debug-test"
             ],
             "console": "integratedTerminal",
             "env": {
-                // The default config in pyproject.toml's "[tool.pytest.ini_options]" adds coverage.
-                // Cannot have coverage and debugging at the same time.
-                // https://github.com/microsoft/vscode-python/issues/693
-                "PYTEST_ADDOPTS": "--no-cov"
+                // Enable break on exception when debugging tests (see: tests/conftest.py)
+                "PYTEST_RAISE": "1",
             },
         }
     ]
 }
```

### Comparing `fastcs-0.2/LICENSE` & `fastcs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/PKG-INFO` & `fastcs-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcs
-Version: 0.2
+Version: 0.3.0
 Summary: Control system agnostic framework for building Device support in Python that will work for both EPICS and Tango
 Author-email: Martin Gaughran <martin.gaughran@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,80 +204,52 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/DiamondLightSource/FastCS
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pydantic
-Requires-Dist: pvi~=0.7.1
+Requires-Dist: pvi~=0.8.1
 Requires-Dist: softioc
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: copier; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 
-FastCS
-===========================
+<img alt="FastCS Logo" align="right" width="100" height="100" src="https://raw.githubusercontent.com/DiamondLightSource/FastCS/main/docs/images/fastcs.svg" target=https://github.com/DiamondLightSource/FastCS>
 
-|code_ci| |docs_ci| |coverage| |pypi_version| |license|
+[![CI](https://github.com/DiamondLightSource/FastCS/actions/workflows/ci.yml/badge.svg)](https://github.com/DiamondLightSource/FastCS/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/DiamondLightSource/FastCS/branch/main/graph/badge.svg)](https://codecov.io/gh/DiamondLightSource/FastCS)
+[![PyPI](https://img.shields.io/pypi/v/fastcs.svg)](https://pypi.org/project/fastcs)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-.. image:: https://raw.githubusercontent.com/DiamondLightSource/FastCS/main/docs/images/fastcs.svg
-    :width: 150px
-    :height: 150px
-    :align: left
-    :name: logo
-    :target: https://DiamondLightSource.github.io/FastCS
+# FastCS
 
-:PyPI:           ``pip install FastCS``
-:Source code:    https://github.com/DiamondLightSource/FastCS
-:Documentation:  https://DiamondLightSource.github.io/FastCS
-:Releases:       https://github.com/DiamondLightSource/FastCS/releases
+Source          | <https://github.com/DiamondLightSource/FastCS>
+:---:           | :---:
+PyPI            | `pip install fastcs`
+Documentation   | <https://diamondlightsource.github.io/FastCS>
+Releases        | <https://github.com/DiamondLightSource/FastCS/releases>
 
-FastCS is a control system agnostic framework for building Device support in
-Python that will work for both EPICS and Tango without depending on either.
+FastCS is a control system agnostic framework for building Device support in Python that
+will work for both EPICS and Tango without depending on either.
 
-.. note::
+<!-- README only content. Anything below this line won't be included in index.md -->
 
-    This repository is in an early stage of development, and doesn't currently do the above!
-
-.. |code_ci| image:: https://github.com/DiamondLightSource/FastCS/actions/workflows/code.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/FastCS/actions/workflows/code.yml
-    :alt: Code CI
-
-.. |docs_ci| image:: https://github.com/DiamondLightSource/FastCS/actions/workflows/docs.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/FastCS/actions/workflows/docs.yml
-    :alt: Docs CI
-
-.. |coverage| image:: https://codecov.io/gh/DiamondLightSource/FastCS/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/DiamondLightSource/FastCS
-    :alt: Test Coverage
-
-.. |pypi_version| image:: https://img.shields.io/pypi/v/FastCS.svg
-    :target: https://pypi.org/project/FastCS
-    :alt: Latest PyPI version
-
-.. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: Apache License
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
-
-See https://DiamondLightSource.github.io/FastCS for more detailed documentation.
+See https://diamondlightsource.github.io/FastCS for more detailed documentation.
```

### Comparing `fastcs-0.2/docs/conf.py` & `fastcs-0.3.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 import sys
 from pathlib import Path
 from subprocess import check_output
 
-import requests  # type:ignore
+import requests
 
 import fastcs
 
 # -- General configuration ------------------------------------------------
 
 # General information about the project.
 project = "FastCS"
@@ -28,32 +28,36 @@
     version = git_branch.decode().strip()
 else:
     version = release
 
 extensions = [
     # Use this for generating API docs
     "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
     # This can parse google style docstrings
     "sphinx.ext.napoleon",
     # For linking to external sphinx documentation
     "sphinx.ext.intersphinx",
     # Add links to source code in API docs
     "sphinx.ext.viewcode",
     # Adds the inheritance-diagram generation directive
     "sphinx.ext.inheritance_diagram",
     # Add a copy button to each code block
     "sphinx_copybutton",
     # For the card element
     "sphinx_design",
+    # So we can write markdown files
+    "myst_parser",
 ]
 
+# So we can use the ::: syntax
+myst_enable_extensions = ["colon_fence"]
+
 # If true, Sphinx will warn about all references where the target cannot
 # be found.
-nitpicky = False
+nitpicky = True
 
 # A list of (type, target) tuples (by default empty) that should be ignored when
 # generating warnings in "nitpicky mode". Note that type should include the
 # domain name if present. Example entries would be ('py:func', 'int') or
 # ('envvar', 'LD_LIBRARY_PATH').
 nitpick_ignore = [
     ("py:class", "NoneType"),
@@ -61,86 +65,68 @@
     ("py:class", "'float'"),
     ("py:class", "'int'"),
     ("py:class", "'bool'"),
     ("py:class", "'object'"),
     ("py:class", "'id'"),
     ("py:class", "typing_extensions.Literal"),
 ]
+nitpick_ignore_regex = [
+    ("py:class", "fastcs.*.T"),
+]
 
 # Both the class’ and the __init__ method’s docstring are concatenated and
 # inserted into the main body of the autoclass directive
 autoclass_content = "both"
 
 # Order the members by the order they appear in the source code
 autodoc_member_order = "bysource"
 
 # Don't inherit docstrings from baseclasses
 autodoc_inherit_docstrings = False
 
-# Generate autosummary sections
-autosummary_generate = True
-
-templates_path = ["_templates"]
-exclude_patterns = ["_build", "_templates"]
-
 # Output graphviz directive produced images in a scalable format
 graphviz_output_format = "svg"
 
 # The name of a reST role (builtin or Sphinx extension) to use as the default
 # role, that is, for text marked up `like this`
 default_role = "any"
 
-# The suffix of source filenames.
-source_suffix = ".rst"
-
 # The master toctree document.
 master_doc = "index"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # These patterns also affect html_static_path and html_extra_path
 exclude_patterns = ["_build"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # This means you can link things like `str` and `asyncio` to the relevant
 # docs in the python documentation.
-intersphinx_mapping = {
-    "python": ("https://docs.python.org/3/", None),
-    "numpy": ("https://numpy.org/doc/stable/", None),
-}
+intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
 
 # A dictionary of graphviz graph attributes for inheritance diagrams.
 inheritance_graph_attrs = {"rankdir": "TB"}
 
-# Common links that should be available on every page
-rst_epilog = """
-.. _Diamond Light Source: http://www.diamond.ac.uk
-.. _black: https://github.com/psf/black
-.. _ruff: https://beta.ruff.rs/docs/
-.. _mypy: http://mypy-lang.org/
-.. _pre-commit: https://pre-commit.com/
-"""
-
 # Ignore localhost links for periodic check that links in docs are valid
 linkcheck_ignore = [r"http://localhost:\d+/"]
 
 # Set copy-button to ignore python and bash prompts
 # https://sphinx-copybutton.readthedocs.io/en/latest/use.html#using-regexp-prompt-identifiers
 copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
 copybutton_prompt_is_regexp = True
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
-github_repo = project
+github_repo = "FastCS"
 github_user = "DiamondLightSource"
 switcher_json = f"https://{github_user}.github.io/{github_repo}/switcher.json"
 switcher_exists = requests.get(switcher_json).ok
 if not switcher_exists:
     print(
         "*** Can't read version switcher, is GitHub pages enabled? \n"
         "    Once Docs CI job has successfully run once, set the "
@@ -148,18 +134,18 @@
         f"    https://github.com/{github_user}/{github_repo}/settings/pages",
         file=sys.stderr,
     )
 
 # Theme options for pydata_sphinx_theme
 # We don't check switcher because there are 3 possible states for a repo:
 # 1. New project, docs are not published so there is no switcher
-# 2. Existing project with latest skeleton, switcher exists and works
-# 3. Existing project with old skeleton that makes broken switcher,
+# 2. Existing project with latest copier template, switcher exists and works
+# 3. Existing project with old copier template that makes broken switcher,
 #    switcher exists but is broken
-# Point 3 makes checking switcher difficult, because the updated skeleton
+# Point 3 makes checking switcher difficult, because the updated copier template
 # will fix the switcher at the end of the docs workflow, but never gets a chance
 # to complete as the docs build warns and fails.
 html_theme_options = {
     "logo": {
         "text": project,
     },
     "use_edit_page_button": True,
@@ -173,27 +159,21 @@
     ],
     "switcher": {
         "json_url": switcher_json,
         "version_match": version,
     },
     "check_switcher": False,
     "navbar_end": ["theme-switcher", "icon-links", "version-switcher"],
-    "external_links": [
-        {
-            "name": "Release Notes",
-            "url": f"https://github.com/{github_user}/{github_repo}/releases",
-        }
-    ],
     "navigation_with_keys": False,
 }
 
 # A dictionary of values to pass into the template engine’s context for all pages
 html_context = {
     "github_user": github_user,
-    "github_repo": project,
+    "github_repo": github_repo,
     "github_version": version,
     "doc_path": "docs",
 }
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = False
```

### Comparing `fastcs-0.2/docs/images/fastcs.svg` & `fastcs-0.3.0/docs/images/fastcs.svg`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/docs/user/tutorials/installation.rst` & `fastcs-0.3.0/docs/tutorials/installation.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-Installation
-============
+# Installation
 
-Check your version of python
-----------------------------
+## Check your version of python
 
-You will need python 3.8 or later. You can check your version of python by
-typing into a terminal::
+You will need python 3.11 or later. You can check your version of python by
+typing into a terminal:
 
-    $ python3 --version
+```
+$ python3 --version
+```
 
-
-Create a virtual environment
-----------------------------
+## Create a virtual environment
 
 It is recommended that you install into a “virtual environment” so this
-installation will not interfere with any existing Python software::
-
-    $ python3 -m venv /path/to/venv
-    $ source /path/to/venv/bin/activate
+installation will not interfere with any existing Python software:
 
+```
+$ python3 -m venv /path/to/venv
+$ source /path/to/venv/bin/activate
+```
 
-Installing the library
-----------------------
+## Installing the library
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use `pip` to install the library and its dependencies:
 
-    $ python3 -m pip install FastCS
+```
+$ python3 -m pip install fastcs
+```
 
 If you require a feature that is not currently released you can also install
-from github::
+from github:
 
-    $ python3 -m pip install git+https://github.com/DiamondLightSource/FastCS.git
+```
+$ python3 -m pip install git+https://github.com/DiamondLightSource/FastCS.git
+```
 
 The library should now be installed and the commandline interface on your path.
-You can check the version that has been installed by typing::
+You can check the version that has been installed by typing:
 
-    $ FastCS --version
+```
+$ FastCS --version
+```
```

### Comparing `fastcs-0.2/pyproject.toml` & `fastcs-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
+requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastcs"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Control system agnostic framework for building Device support in Python that will work for both EPICS and Tango"
 dependencies = [
     "numpy",
     "pydantic",
-    "pvi~=0.7.1",
+    "pvi~=0.8.1",
     "softioc",
-] # Add project dependencies here, e.g. ["click", "numpy"]
+]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.10"
+readme = "README.md"
+requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
-    "black",
+    "copier",
     "mypy",
+    "myst-parser",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pytest",
     "pytest-cov",
     "ruff",
     "sphinx-autobuild",
@@ -76,35 +76,36 @@
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist=True
 
-[testenv:{pre-commit,mypy,pytest,docs}]
+[testenv:{pre-commit,type-checking,tests,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
 allowlist_externals =
     pytest
     pre-commit
     mypy
     sphinx-build
     sphinx-autobuild
 commands =
-    pytest: pytest --cov=fastcs --cov-report term --cov-report xml:cov.xml {posargs}
-    mypy: mypy src tests {posargs}
-    pre-commit: pre-commit run --all-files {posargs}
+    pre-commit: pre-commit run --all-files --show-diff-on-failure {posargs}
+    type-checking: mypy src tests {posargs}
+    tests: pytest --cov=fastcs --cov-report term --cov-report xml:cov.xml {posargs}
     docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html
 """
 
-
 [tool.ruff]
 src = ["src", "tests"]
 line-length = 88
-select = [
-    "C4",   # flake8-comprehensions - https://beta.ruff.rs/docs/rules/#flake8-comprehensions-c4
-    "E",    # pycodestyle errors - https://beta.ruff.rs/docs/rules/#error-e
-    "F",    # pyflakes rules - https://beta.ruff.rs/docs/rules/#pyflakes-f
-    "W",    # pycodestyle warnings - https://beta.ruff.rs/docs/rules/#warning-w
-    "I001", # isort
+lint.select = [
+    "B",  # flake8-bugbear - https://docs.astral.sh/ruff/rules/#flake8-bugbear-b
+    "C4", # flake8-comprehensions - https://docs.astral.sh/ruff/rules/#flake8-comprehensions-c4
+    "E",  # pycodestyle errors - https://docs.astral.sh/ruff/rules/#error-e
+    "F",  # pyflakes rules - https://docs.astral.sh/ruff/rules/#pyflakes-f
+    "W",  # pycodestyle warnings - https://docs.astral.sh/ruff/rules/#warning-w
+    "I",  # isort - https://docs.astral.sh/ruff/rules/#isort-i
+    "UP", # pyupgrade - https://docs.astral.sh/ruff/rules/#pyupgrade-up
 ]
```

### Comparing `fastcs-0.2/src/fastcs/attributes.py` & `fastcs-0.3.0/src/fastcs/attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,50 +3,50 @@
 from enum import Enum
 from typing import Any, Generic, Protocol, runtime_checkable
 
 from .datatypes import ATTRIBUTE_TYPES, AttrCallback, DataType, T
 
 
 class AttrMode(Enum):
-    """Access mode of an `Attribute`."""
+    """Access mode of an ``Attribute``."""
 
     READ = 1
     WRITE = 2
     READ_WRITE = 3
 
 
 @runtime_checkable
 class Sender(Protocol):
-    """Protocol for setting the value of an `Attribute`."""
+    """Protocol for setting the value of an ``Attribute``."""
 
     async def put(self, controller: Any, attr: AttrW, value: Any) -> None:
         pass
 
 
 @runtime_checkable
 class Updater(Protocol):
-    """Protocol for updating the cached readback value of an `Attribute`."""
+    """Protocol for updating the cached readback value of an ``Attribute``."""
 
     update_period: float
 
     async def update(self, controller: Any, attr: AttrR) -> None:
         pass
 
 
 @runtime_checkable
 class Handler(Sender, Updater, Protocol):
-    """Protocol encapsulating both `Sender` and `Updater`."""
+    """Protocol encapsulating both ``Sender`` and ``Updater``."""
 
     pass
 
 
 class Attribute(Generic[T]):
     """Base FastCS attribute.
 
-    Instances of this class added to a `Controller` will be used by the backend.
+    Instances of this class added to a ``Controller`` will be used by the backend.
     """
 
     def __init__(
         self,
         datatype: DataType[T],
         access_mode: AttrMode,
         group: str | None = None,
@@ -73,15 +73,15 @@
 
     @property
     def group(self) -> str | None:
         return self._group
 
 
 class AttrR(Attribute[T]):
-    """A read-only `Attribute`."""
+    """A read-only ``Attribute``."""
 
     def __init__(
         self,
         datatype: DataType[T],
         access_mode=AttrMode.READ,
         group: str | None = None,
         handler: Updater | None = None,
@@ -105,15 +105,15 @@
 
     @property
     def updater(self) -> Updater | None:
         return self._updater
 
 
 class AttrW(Attribute[T]):
-    """A write-only `Attribute`."""
+    """A write-only ``Attribute``."""
 
     def __init__(
         self,
         datatype: DataType[T],
         access_mode=AttrMode.WRITE,
         group: str | None = None,
         handler: Sender | None = None,
@@ -144,15 +144,15 @@
 
     @property
     def sender(self) -> Sender | None:
         return self._sender
 
 
 class AttrRW(AttrW[T], AttrR[T]):
-    """A read-write `Attribute`."""
+    """A read-write ``Attribute``."""
 
     def __init__(
         self,
         datatype: DataType[T],
         access_mode=AttrMode.READ_WRITE,
         group: str | None = None,
         handler: Handler | None = None,
```

### Comparing `fastcs-0.2/src/fastcs/backend.py` & `fastcs-0.3.0/src/fastcs/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from collections import defaultdict
+from collections.abc import Callable
 from types import MethodType
-from typing import Callable
 
 from .attributes import AttrR, AttrW, Sender, Updater
 from .exceptions import FastCSException
 from .mapping import Mapping, SingleMapping
 
 
 def _get_initial_tasks(mapping: Mapping) -> list[Callable]:
```

### Comparing `fastcs-0.2/src/fastcs/backends/asyncio_backend.py` & `fastcs-0.3.0/src/fastcs/backends/asyncio_backend.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/src/fastcs/backends/epics/backend.py` & `fastcs-0.3.0/src/fastcs/backends/epics/backend.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from .docs import EpicsDocs, EpicsDocsOptions
 from .gui import EpicsGUI, EpicsGUIOptions
 from .ioc import EpicsIOC
 
 
 class EpicsBackend:
-    def __init__(self, mapping: Mapping):
+    def __init__(self, mapping: Mapping, pv_prefix: str = "MY-DEVICE-PREFIX"):
         self._mapping = mapping
+        self._pv_prefix = pv_prefix
 
     def create_docs(self, options: EpicsDocsOptions | None = None) -> None:
         docs = EpicsDocs(self._mapping)
         docs.create_docs(options)
 
     def create_gui(self, options: EpicsGUIOptions | None = None) -> None:
-        gui = EpicsGUI(self._mapping)
+        gui = EpicsGUI(self._mapping, self._pv_prefix)
         gui.create_gui(options)
 
     def get_ioc(self) -> EpicsIOC:
-        return EpicsIOC(self._mapping)
+        return EpicsIOC(self._mapping, self._pv_prefix)
```

### Comparing `fastcs-0.2/src/fastcs/backends/epics/gui.py` & `fastcs-0.3.0/src/fastcs/backends/epics/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 
 from pvi._format.dls import DLSFormatter
 from pvi.device import (
     LED,
-    CheckBox,
+    ButtonPanel,
     Component,
     Device,
     Grid,
     Group,
     ReadWidget,
     SignalR,
     SignalRW,
     SignalW,
     SignalX,
     SubScreen,
     TextFormat,
     TextRead,
     TextWrite,
+    ToggleButton,
     Tree,
     WriteWidget,
 )
 
 from fastcs.attributes import Attribute, AttrR, AttrRW, AttrW
 from fastcs.cs_methods import Command
 from fastcs.datatypes import Bool, DataType, Float, Int, String
@@ -38,26 +39,24 @@
 @dataclass
 class EpicsGUIOptions:
     output_path: Path = Path.cwd() / "output.bob"
     file_format: EpicsGUIFormat = EpicsGUIFormat.bob
 
 
 class EpicsGUI:
-    def __init__(self, mapping: Mapping) -> None:
+    def __init__(self, mapping: Mapping, pv_prefix: str) -> None:
         self._mapping = mapping
+        self._pv_prefix = pv_prefix
 
-    @staticmethod
-    def _get_pv(attr_path: str, name: str):
+    def _get_pv(self, attr_path: str, name: str):
         if attr_path:
             attr_path = ":" + attr_path
         attr_path += ":"
 
-        pv = attr_path.upper() + name.title().replace("_", "")
-
-        return pv
+        return f"{self._pv_prefix}{attr_path.upper()}{name.title().replace('_', '')}"
 
     @staticmethod
     def _get_read_widget(datatype: DataType) -> ReadWidget:
         match datatype:
             case Bool():
                 return LED()
             case Int() | Float():
@@ -67,51 +66,54 @@
             case _:
                 raise FastCSException(f"Unsupported type {type(datatype)}: {datatype}")
 
     @staticmethod
     def _get_write_widget(datatype: DataType) -> WriteWidget:
         match datatype:
             case Bool():
-                return CheckBox()
+                return ToggleButton()
             case Int() | Float():
                 return TextWrite()
             case String():
                 return TextWrite(format=TextFormat.string)
             case _:
                 raise FastCSException(f"Unsupported type {type(datatype)}: {datatype}")
 
-    @classmethod
-    def _get_attribute_component(cls, attr_path: str, name: str, attribute: Attribute):
-        pv = cls._get_pv(attr_path, name)
+    def _get_attribute_component(self, attr_path: str, name: str, attribute: Attribute):
+        pv = self._get_pv(attr_path, name)
         name = name.title().replace("_", "")
 
         match attribute:
             case AttrRW():
-                read_widget = cls._get_read_widget(attribute.datatype)
-                write_widget = cls._get_write_widget(attribute.datatype)
+                read_widget = self._get_read_widget(attribute.datatype)
+                write_widget = self._get_write_widget(attribute.datatype)
                 return SignalRW(
                     name=name,
-                    pv=pv,
-                    widget=write_widget,
+                    write_pv=pv,
+                    write_widget=write_widget,
                     read_pv=pv + "_RBV",
                     read_widget=read_widget,
                 )
             case AttrR():
-                read_widget = cls._get_read_widget(attribute.datatype)
-                return SignalR(name=name, pv=pv, widget=read_widget)
+                read_widget = self._get_read_widget(attribute.datatype)
+                return SignalR(name=name, read_pv=pv, read_widget=read_widget)
             case AttrW():
-                write_widget = cls._get_write_widget(attribute.datatype)
-                return SignalW(name=name, pv=pv, widget=TextWrite())
+                write_widget = self._get_write_widget(attribute.datatype)
+                return SignalW(name=name, write_pv=pv, write_widget=TextWrite())
 
-    @classmethod
-    def _get_command_component(cls, attr_path: str, name: str):
-        pv = cls._get_pv(attr_path, name)
+    def _get_command_component(self, attr_path: str, name: str):
+        pv = self._get_pv(attr_path, name)
         name = name.title().replace("_", "")
 
-        return SignalX(name=name, pv=pv, value="1")
+        return SignalX(
+            name=name,
+            write_pv=pv,
+            value="1",
+            write_widget=ButtonPanel(actions={name: "1"}),
+        )
 
     def create_gui(self, options: EpicsGUIOptions | None = None) -> None:
         if options is None:
             options = EpicsGUIOptions()
 
         if options.file_format is EpicsGUIFormat.edl:
             raise FastCSException("FastCS does not support .edl screens.")
@@ -132,15 +134,15 @@
                     layout=SubScreen(),
                     children=self.extract_mapping_components(sub_controller_mapping),
                 )
             )
 
         device = Device(label="Simple Device", children=components)
 
-        formatter.format(device, "MY-DEVICE-PREFIX", options.output_path)
+        formatter.format(device, options.output_path)
 
     def extract_mapping_components(self, mapping: SingleMapping) -> list[Component]:
         components: Tree[Component] = []
         attr_path = mapping.controller.path
 
         groups: dict[str, list[Component]] = {}
         for attr_name, attribute in mapping.attributes.items():
```

### Comparing `fastcs-0.2/src/fastcs/backends/epics/ioc.py` & `fastcs-0.3.0/src/fastcs/backends/epics/ioc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from collections.abc import Callable
 from dataclasses import dataclass
 from types import MethodType
-from typing import Any, Callable
+from typing import Any
 
 from softioc import asyncio_dispatcher, builder, softioc
 from softioc.pythonSoftIoc import RecordWrapper
 
 from fastcs.attributes import AttrR, AttrRW, AttrW
 from fastcs.backend import Backend
 from fastcs.datatypes import Bool, DataType, Float, Int, String
@@ -66,24 +67,24 @@
 
 def _create_and_link_write_pv(pv_name: str, attribute: AttrW) -> None:
     record = _get_output_record(
         pv_name, attribute.datatype, on_update=attribute.process_without_display_update
     )
 
     async def async_wrapper(v):
-        record.set(v)
+        record.set(v, process=False)
 
     attribute.set_write_display_callback(async_wrapper)
 
 
 def _create_and_link_command_pv(pv_name: str, method: Callable) -> None:
     async def wrapped_method(_: Any):
         await method()
 
-    builder.aOut(pv_name, always_update=True, on_update=wrapped_method)
+    builder.aOut(pv_name, initial_value=0, always_update=True, on_update=wrapped_method)
 
 
 def _create_and_link_attribute_pvs(mapping: Mapping) -> None:
     for single_mapping in mapping.get_controller_mappings():
         path = single_mapping.controller.path
         for attr_name, attribute in single_mapping.attributes.items():
             attr_name = attr_name.title().replace("_", "")
@@ -108,27 +109,28 @@
 
             _create_and_link_command_pv(
                 pv_name, MethodType(method.fn, single_mapping.controller)
             )
 
 
 class EpicsIOC:
-    def __init__(self, mapping: Mapping):
+    def __init__(self, mapping: Mapping, pv_prefix: str):
         self._mapping = mapping
+        self._pv_prefix = pv_prefix
 
     def run(self, options: EpicsIOCOptions | None = None) -> None:
         if options is None:
             options = EpicsIOCOptions()
 
         # Create an asyncio dispatcher; the event loop is now running
         dispatcher = asyncio_dispatcher.AsyncioDispatcher()
         backend = Backend(self._mapping, dispatcher.loop)
 
         # Set the record prefix
-        builder.SetDeviceName("MY-DEVICE-PREFIX")
+        builder.SetDeviceName(self._pv_prefix)
 
         _create_and_link_attribute_pvs(self._mapping)
 
         _create_and_link_command_pvs(self._mapping)
 
         # Boilerplate to get the IOC started
         builder.LoadDatabase()
```

### Comparing `fastcs-0.2/src/fastcs/connections.py` & `fastcs-0.3.0/src/fastcs/connections/ip_connection.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/src/fastcs/controller.py` & `fastcs-0.3.0/src/fastcs/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
                 setattr(self, attr_name, new_attribute)
 
 
 class Controller(BaseController):
     """Top-level controller for a device.
 
     This is the primary class for implementing device support in FastCS. Instances of
-    this class can be loaded into a backend to access its `Attribute`s. The backend can
-    then perform a specific function with the set of `Attributes`, such as generating a
-    UI or creating parameters for a control system.
+    this class can be loaded into a backend to access its ``Attribute``s. The backend
+    can then perform a specific function with the set of ``Attributes``, such as
+    generating a UI or creating parameters for a control system.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.__sub_controllers: list[SubController] = []
 
     async def connect(self) -> None:
@@ -42,15 +42,15 @@
         self.__sub_controllers.append(controller)
 
     def get_sub_controllers(self) -> list[SubController]:
         return self.__sub_controllers
 
 
 class SubController(BaseController):
-    """A subordinate to a `Controller` for managing a subset of a device.
+    """A subordinate to a ``Controller`` for managing a subset of a device.
 
-    An instance of this class can be registered with a parent `Controller` to include it
-    as part of a larger device.
+    An instance of this class can be registered with a parent ``Controller`` to include
+    it as part of a larger device.
     """
 
     def __init__(self, path: str) -> None:
         super().__init__(path)
```

### Comparing `fastcs-0.2/src/fastcs/cs_methods.py` & `fastcs-0.3.0/src/fastcs/cs_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from asyncio import iscoroutinefunction
+from collections.abc import Awaitable, Callable
 from inspect import Signature, getdoc, signature
-from typing import Awaitable, Callable
 
 from .exceptions import FastCSException
 
 ScanCallback = Callable[..., Awaitable[None]]
 
 
 class Method:
```

### Comparing `fastcs-0.2/src/fastcs/datatypes.py` & `fastcs-0.3.0/src/fastcs/datatypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod
+from collections.abc import Awaitable, Callable
 from dataclasses import dataclass
-from typing import Awaitable, Callable, Generic, TypeVar
+from typing import Generic, TypeVar
 
 T = TypeVar("T", int, float, bool, str)
 ATTRIBUTE_TYPES: tuple[type] = T.__constraints__  # type: ignore
 
 
 AttrCallback = Callable[[T], Awaitable[None]]
 
@@ -18,44 +19,44 @@
     @abstractmethod
     def dtype(self) -> type[T]:  # Using property due to lack of Generic ClassVars
         pass
 
 
 @dataclass(frozen=True)
 class Int(DataType[int]):
-    """`DataType` mapping to builtin `int`."""
+    """`DataType` mapping to builtin ``int``."""
 
     @property
     def dtype(self) -> type[int]:
         return int
 
 
 @dataclass(frozen=True)
 class Float(DataType[float]):
-    """`DataType` mapping to builtin `float`."""
+    """`DataType` mapping to builtin ``float``."""
 
     prec: int = 2
 
     @property
     def dtype(self) -> type[float]:
         return float
 
 
 @dataclass(frozen=True)
 class Bool(DataType[bool]):
-    """`DataType` mapping to builtin `bool`."""
+    """`DataType` mapping to builtin ``bool``."""
 
     znam: str = "OFF"
     onam: str = "ON"
 
     @property
     def dtype(self) -> type[bool]:
         return bool
 
 
 @dataclass(frozen=True)
 class String(DataType[str]):
-    """`DataType` mapping to builtin `str`."""
+    """`DataType` mapping to builtin ``str``."""
 
     @property
     def dtype(self) -> type[str]:
         return str
```

### Comparing `fastcs-0.2/src/fastcs/mapping.py` & `fastcs-0.3.0/src/fastcs/mapping.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/src/fastcs/wrappers.py` & `fastcs-0.3.0/src/fastcs/wrappers.py`

 * *Files identical despite different names*

### Comparing `fastcs-0.2/src/fastcs.egg-info/PKG-INFO` & `fastcs-0.3.0/src/fastcs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcs
-Version: 0.2
+Version: 0.3.0
 Summary: Control system agnostic framework for building Device support in Python that will work for both EPICS and Tango
 Author-email: Martin Gaughran <martin.gaughran@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,80 +204,52 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/DiamondLightSource/FastCS
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pydantic
-Requires-Dist: pvi~=0.7.1
+Requires-Dist: pvi~=0.8.1
 Requires-Dist: softioc
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
+Requires-Dist: copier; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
+Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 
-FastCS
-===========================
+<img alt="FastCS Logo" align="right" width="100" height="100" src="https://raw.githubusercontent.com/DiamondLightSource/FastCS/main/docs/images/fastcs.svg" target=https://github.com/DiamondLightSource/FastCS>
 
-|code_ci| |docs_ci| |coverage| |pypi_version| |license|
+[![CI](https://github.com/DiamondLightSource/FastCS/actions/workflows/ci.yml/badge.svg)](https://github.com/DiamondLightSource/FastCS/actions/workflows/ci.yml)
+[![Coverage](https://codecov.io/gh/DiamondLightSource/FastCS/branch/main/graph/badge.svg)](https://codecov.io/gh/DiamondLightSource/FastCS)
+[![PyPI](https://img.shields.io/pypi/v/fastcs.svg)](https://pypi.org/project/fastcs)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-.. image:: https://raw.githubusercontent.com/DiamondLightSource/FastCS/main/docs/images/fastcs.svg
-    :width: 150px
-    :height: 150px
-    :align: left
-    :name: logo
-    :target: https://DiamondLightSource.github.io/FastCS
+# FastCS
 
-:PyPI:           ``pip install FastCS``
-:Source code:    https://github.com/DiamondLightSource/FastCS
-:Documentation:  https://DiamondLightSource.github.io/FastCS
-:Releases:       https://github.com/DiamondLightSource/FastCS/releases
+Source          | <https://github.com/DiamondLightSource/FastCS>
+:---:           | :---:
+PyPI            | `pip install fastcs`
+Documentation   | <https://diamondlightsource.github.io/FastCS>
+Releases        | <https://github.com/DiamondLightSource/FastCS/releases>
 
-FastCS is a control system agnostic framework for building Device support in
-Python that will work for both EPICS and Tango without depending on either.
+FastCS is a control system agnostic framework for building Device support in Python that
+will work for both EPICS and Tango without depending on either.
 
-.. note::
+<!-- README only content. Anything below this line won't be included in index.md -->
 
-    This repository is in an early stage of development, and doesn't currently do the above!
-
-.. |code_ci| image:: https://github.com/DiamondLightSource/FastCS/actions/workflows/code.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/FastCS/actions/workflows/code.yml
-    :alt: Code CI
-
-.. |docs_ci| image:: https://github.com/DiamondLightSource/FastCS/actions/workflows/docs.yml/badge.svg?branch=main
-    :target: https://github.com/DiamondLightSource/FastCS/actions/workflows/docs.yml
-    :alt: Docs CI
-
-.. |coverage| image:: https://codecov.io/gh/DiamondLightSource/FastCS/branch/main/graph/badge.svg
-    :target: https://codecov.io/gh/DiamondLightSource/FastCS
-    :alt: Test Coverage
-
-.. |pypi_version| image:: https://img.shields.io/pypi/v/FastCS.svg
-    :target: https://pypi.org/project/FastCS
-    :alt: Latest PyPI version
-
-.. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
-    :target: https://opensource.org/licenses/Apache-2.0
-    :alt: Apache License
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
-
-See https://DiamondLightSource.github.io/FastCS for more detailed documentation.
+See https://diamondlightsource.github.io/FastCS for more detailed documentation.
```

### Comparing `fastcs-0.2/src/fastcs.egg-info/SOURCES.txt` & `fastcs-0.3.0/src/fastcs.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,54 @@
+.copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
-README.rst
+README.md
+catalog-info.yaml
 pyproject.toml
 .devcontainer/devcontainer.json
-.github/CONTRIBUTING.rst
+.github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
-.github/workflows/code.yml
-.github/workflows/docs.yml
-.github/workflows/docs_clean.yml
-.github/workflows/linkcheck.yml
+.github/workflows/_check.yml
+.github/workflows/_dist.yml
+.github/workflows/_docs.yml
+.github/workflows/_pypi.yml
+.github/workflows/_release.yml
+.github/workflows/_test.yml
+.github/workflows/_tox.yml
+.github/workflows/ci.yml
+.github/workflows/periodic.yml
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
-docs/genindex.rst
-docs/index.rst
-docs/_templates/custom-class-template.rst
-docs/_templates/custom-module-template.rst
-docs/developer/index.rst
-docs/developer/explanations/decisions.rst
-docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
-docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
-docs/developer/how-to/build-docs.rst
-docs/developer/how-to/contribute.rst
-docs/developer/how-to/lint.rst
-docs/developer/how-to/make-release.rst
-docs/developer/how-to/pin-requirements.rst
-docs/developer/how-to/run-tests.rst
-docs/developer/how-to/static-analysis.rst
-docs/developer/how-to/test-container.rst
-docs/developer/how-to/update-tools.rst
-docs/developer/reference/standards.rst
-docs/developer/tutorials/dev-install.rst
+docs/explanations.md
+docs/genindex.md
+docs/how-to.md
+docs/index.md
+docs/reference.md
+docs/tutorials.md
+docs/explanations/decisions.md
+docs/explanations/decisions/0001-record-architecture-decisions.md
+docs/explanations/decisions/0002-switched-to-python-copier-template.md
+docs/explanations/decisions/COPYME
+docs/how-to/contribute.md
 docs/images/fastcs.svg
-docs/user/index.rst
-docs/user/explanations/docs-structure.rst
-docs/user/how-to/run-container.rst
-docs/user/reference/api.rst
-docs/user/tutorials/installation.rst
+docs/reference/api.md
+docs/tutorials/installation.md
 src/fastcs/__init__.py
 src/fastcs/__main__.py
 src/fastcs/_version.py
 src/fastcs/attributes.py
 src/fastcs/backend.py
-src/fastcs/connections.py
 src/fastcs/controller.py
 src/fastcs/cs_methods.py
 src/fastcs/datatypes.py
 src/fastcs/exceptions.py
 src/fastcs/mapping.py
 src/fastcs/wrappers.py
 src/fastcs.egg-info/PKG-INFO
@@ -65,9 +60,12 @@
 src/fastcs/backends/__init__.py
 src/fastcs/backends/asyncio_backend.py
 src/fastcs/backends/epics/__init__.py
 src/fastcs/backends/epics/backend.py
 src/fastcs/backends/epics/docs.py
 src/fastcs/backends/epics/gui.py
 src/fastcs/backends/epics/ioc.py
+src/fastcs/connections/__init__.py
+src/fastcs/connections/ip_connection.py
+tests/conftest.py
 tests/test_boilerplate_removed.py
 tests/test_cli.py
```

### Comparing `fastcs-0.2/tests/test_boilerplate_removed.py` & `fastcs-0.3.0/tests/test_boilerplate_removed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This file checks that all the example boilerplate text has been removed.
 It can be deleted when all the contained tests pass
 """
+
 from pathlib import Path
 
 ROOT = Path(__file__).parent.parent
 
 
 def skeleton_check(check: bool, text: str):
     if ROOT.name == "python3-pip-skeleton" or str(ROOT) == "/project":
```

