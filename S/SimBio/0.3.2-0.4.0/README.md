# Comparing `tmp/SimBio-0.3.2.tar.gz` & `tmp/simbio-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimBio-0.3.2.tar", last modified: Wed Mar  6 19:09:11 2024, max compression
+gzip compressed data, was "simbio-0.4.tar", last modified: Fri Apr 12 19:06:53 2024, max compression
```

## Comparing `SimBio-0.3.2.tar` & `simbio-0.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.971867 SimBio-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-06 19:09:07.000000 SimBio-0.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.955867 SimBio-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.959867 SimBio-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-06 19:09:07.000000 SimBio-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-06 19:09:07.000000 SimBio-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-06 19:09:07.000000 SimBio-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-06 19:09:07.000000 SimBio-0.3.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-03-06 19:09:11.971867 SimBio-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-06 19:09:07.000000 SimBio-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-06 19:09:07.000000 SimBio-0.3.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.963867 SimBio-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.963867 SimBio-0.3.2/docs/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/compilers/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.963867 SimBio-0.3.2/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/design/dsl.md
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/design/features.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/design/multilevel_dsl.md
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/design/references.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.963867 SimBio-0.3.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/examples/basic.md
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/examples/chained-reactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/examples/compartments.md
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/examples/enzymatic.md
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/jupytext.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.963867 SimBio-0.3.2/docs/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/model/dynamic.md
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/model/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/model/reactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/model/static.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:07.000000 SimBio-0.3.2/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-06 19:09:07.000000 SimBio-0.3.2/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-06 19:09:07.000000 SimBio-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-06 19:09:07.000000 SimBio-0.3.2/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-06 19:09:07.000000 SimBio-0.3.2/requirements.io.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-06 19:09:07.000000 SimBio-0.3.2/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-06 19:09:07.000000 SimBio-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 19:09:11.971867 SimBio-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.959867 SimBio-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/SimBio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-03-06 19:09:11.000000 SimBio-0.3.2/src/SimBio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-06 19:09:11.000000 SimBio-0.3.2/src/SimBio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 19:09:11.000000 SimBio-0.3.2/src/SimBio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-06 19:09:11.000000 SimBio-0.3.2/src/SimBio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 19:09:11.000000 SimBio-0.3.2/src/SimBio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/io/
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/biomodels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/io/mathML/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/test_mathML.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/mathML/to_symbolite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/io/sbml/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/from_libsbml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/test_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/io/sbml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/tests/atol_factor.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/tests/test_sbml_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/io/sbml/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:09:11.967867 SimBio-0.3.2/src/simbio/reactions/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/reactions/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/reactions/enzymatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/reactions/single.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/reactions/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-06 19:09:07.000000 SimBio-0.3.2/src/simbio/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 19:06:49.000000 simbio-0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.554026 simbio-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.558026 simbio-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 19:06:49.000000 simbio-0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-12 19:06:49.000000 simbio-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-12 19:06:49.000000 simbio-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 19:06:49.000000 simbio-0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-12 19:06:53.566026 simbio-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-12 19:06:49.000000 simbio-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 19:06:49.000000 simbio-0.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.558026 simbio-0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 19:06:49.000000 simbio-0.4/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 19:06:49.000000 simbio-0.4/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.558026 simbio-0.4/docs/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 19:06:49.000000 simbio-0.4/docs/compilers/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.562026 simbio-0.4/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-12 19:06:49.000000 simbio-0.4/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-12 19:06:49.000000 simbio-0.4/docs/design/dsl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-12 19:06:49.000000 simbio-0.4/docs/design/features.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 19:06:49.000000 simbio-0.4/docs/design/multilevel_dsl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-12 19:06:49.000000 simbio-0.4/docs/design/references.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.562026 simbio-0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-12 19:06:49.000000 simbio-0.4/docs/examples/basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 19:06:49.000000 simbio-0.4/docs/examples/chained-reactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-12 19:06:49.000000 simbio-0.4/docs/examples/compartments.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-12 19:06:49.000000 simbio-0.4/docs/examples/enzymatic.md
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 19:06:49.000000 simbio-0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 19:06:49.000000 simbio-0.4/docs/jupytext.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.562026 simbio-0.4/docs/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-12 19:06:49.000000 simbio-0.4/docs/model/dynamic.md
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-12 19:06:49.000000 simbio-0.4/docs/model/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-12 19:06:49.000000 simbio-0.4/docs/model/reactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-12 19:06:49.000000 simbio-0.4/docs/model/static.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:49.000000 simbio-0.4/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 19:06:49.000000 simbio-0.4/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-12 19:06:49.000000 simbio-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 19:06:49.000000 simbio-0.4/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 19:06:49.000000 simbio-0.4/requirements.io.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 19:06:49.000000 simbio-0.4/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 19:06:49.000000 simbio-0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:06:53.566026 simbio-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.554026 simbio-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/src/SimBio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-12 19:06:53.000000 simbio-0.4/src/SimBio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-12 19:06:53.000000 simbio-0.4/src/SimBio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:06:53.000000 simbio-0.4/src/SimBio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 19:06:53.000000 simbio-0.4/src/SimBio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 19:06:53.000000 simbio-0.4/src/SimBio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.562026 simbio-0.4/src/simbio/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.562026 simbio-0.4/src/simbio/io/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      379 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/biomodels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/src/simbio/io/mathML/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/test_mathML.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/mathML/to_symbolite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/src/simbio/io/sbml/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/from_libsbml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/src/simbio/io/sbml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/tests/atol_factor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/tests/test_sbml_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/io/sbml/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:53.566026 simbio-0.4/src/simbio/reactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/reactions/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/reactions/enzymatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/reactions/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/reactions/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-12 19:06:49.000000 simbio-0.4/src/simbio/test_core.py
```

### Comparing `SimBio-0.3.2/.github/workflows/ci.yml` & `simbio-0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/.pre-commit-config.yaml` & `simbio-0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/PKG-INFO` & `simbio-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimBio
-Version: 0.3.2
+Version: 0.4.0
 Summary: Simulation of Biological Systems
 Author-email: "Hernán E. Grecco" <hernan.grecco@gmail.com>, Mauro Silberberg <maurosilber@gmail.com>
 Project-URL: Homepage, https://github.com/hgrecco/simbio
 Project-URL: Bug Tracker, https://github.com/hgrecco/simbio/issues
 Keywords: mass action,michaelis menten,ode,compartment,reaction,SBML,poincare
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: poincare>=0.3.1
 Provides-Extra: io
 Requires-Dist: biomodels; extra == "io"
 Requires-Dist: python-libsbml; extra == "io"
 Provides-Extra: test
 Requires-Dist: pooch; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest<8.1; extra == "test"
 Requires-Dist: simbio[io]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: numba; extra == "docs"
 Requires-Dist: simbio-corbat2018; extra == "docs"
 Requires-Dist: simbio[test]; extra == "docs"
@@ -137,15 +137,15 @@
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
 ```
 
 or download them from the [BioModels](https://www.ebi.ac.uk/biomodels/) repository:
 
 ```python
 >>> from simbio.io import biomodels
->>> biomodels.load_model("BIOMD12")
+>>> biomodels.load("BIOMD12")
 Elowitz2000 - Repressilator
 -----------------------------------------------------------------------------------
 type          total  names
 ----------  -------  --------------------------------------------------------------
 variables         6  PX, PY, PZ, X, Y, Z
 parameters       17  cell, beta, alpha0, alpha, eff, n, KM, tau_mRNA, tau_prot, ...
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
```

### Comparing `SimBio-0.3.2/README.md` & `simbio-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
 ```
 
 or download them from the [BioModels](https://www.ebi.ac.uk/biomodels/) repository:
 
 ```python
 >>> from simbio.io import biomodels
->>> biomodels.load_model("BIOMD12")
+>>> biomodels.load("BIOMD12")
 Elowitz2000 - Repressilator
 -----------------------------------------------------------------------------------
 type          total  names
 ----------  -------  --------------------------------------------------------------
 variables         6  PX, PY, PZ, X, Y, Z
 parameters       17  cell, beta, alpha0, alpha, eff, n, KM, tau_mRNA, tau_prot, ...
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
```

### Comparing `SimBio-0.3.2/conftest.py` & `simbio-0.4/conftest.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/_config.yml` & `simbio-0.4/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/_toc.yml` & `simbio-0.4/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/compilers/index.md` & `simbio-0.4/docs/compilers/index.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/design/design.md` & `simbio-0.4/docs/design/design.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/design/dsl.md` & `simbio-0.4/docs/design/dsl.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/design/features.md` & `simbio-0.4/docs/design/features.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/design/multilevel_dsl.md` & `simbio-0.4/docs/design/multilevel_dsl.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/design/references.md` & `simbio-0.4/docs/design/references.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/examples/basic.md` & `simbio-0.4/docs/examples/basic.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/examples/chained-reactions.md` & `simbio-0.4/docs/examples/chained-reactions.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/examples/compartments.md` & `simbio-0.4/docs/examples/compartments.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/examples/enzymatic.md` & `simbio-0.4/docs/examples/enzymatic.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/model/dynamic.md` & `simbio-0.4/docs/model/dynamic.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/model/reactions.md` & `simbio-0.4/docs/model/reactions.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/docs/model/static.md` & `simbio-0.4/docs/model/static.md`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/pyproject.toml` & `simbio-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/SimBio.egg-info/PKG-INFO` & `simbio-0.4/src/SimBio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimBio
-Version: 0.3.2
+Version: 0.4.0
 Summary: Simulation of Biological Systems
 Author-email: "Hernán E. Grecco" <hernan.grecco@gmail.com>, Mauro Silberberg <maurosilber@gmail.com>
 Project-URL: Homepage, https://github.com/hgrecco/simbio
 Project-URL: Bug Tracker, https://github.com/hgrecco/simbio/issues
 Keywords: mass action,michaelis menten,ode,compartment,reaction,SBML,poincare
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: poincare>=0.3.1
 Provides-Extra: io
 Requires-Dist: biomodels; extra == "io"
 Requires-Dist: python-libsbml; extra == "io"
 Provides-Extra: test
 Requires-Dist: pooch; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest<8.1; extra == "test"
 Requires-Dist: simbio[io]; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: numba; extra == "docs"
 Requires-Dist: simbio-corbat2018; extra == "docs"
 Requires-Dist: simbio[test]; extra == "docs"
@@ -137,15 +137,15 @@
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
 ```
 
 or download them from the [BioModels](https://www.ebi.ac.uk/biomodels/) repository:
 
 ```python
 >>> from simbio.io import biomodels
->>> biomodels.load_model("BIOMD12")
+>>> biomodels.load("BIOMD12")
 Elowitz2000 - Repressilator
 -----------------------------------------------------------------------------------
 type          total  names
 ----------  -------  --------------------------------------------------------------
 variables         6  PX, PY, PZ, X, Y, Z
 parameters       17  cell, beta, alpha0, alpha, eff, n, KM, tau_mRNA, tau_prot, ...
 equations        12  Reaction1, Reaction2, Reaction3, Reaction4, Reaction5, ...
```

### Comparing `SimBio-0.3.2/src/SimBio.egg-info/SOURCES.txt` & `simbio-0.4/src/SimBio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/core.py` & `simbio-0.4/src/simbio/core.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/mathML/exporter.py` & `simbio-0.4/src/simbio/io/mathML/exporter.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/mathML/importer.py` & `simbio-0.4/src/simbio/io/mathML/importer.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/mathML/test_mathML.py` & `simbio-0.4/src/simbio/io/mathML/test_mathML.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/mathML/to_symbolite.py` & `simbio-0.4/src/simbio/io/mathML/to_symbolite.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/from_libsbml.py` & `simbio-0.4/src/simbio/io/sbml/from_libsbml.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/importer.py` & `simbio-0.4/src/simbio/io/sbml/importer.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/test_importer.py` & `simbio-0.4/src/simbio/io/sbml/test_importer.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/tests/atol_factor.csv` & `simbio-0.4/src/simbio/io/sbml/tests/atol_factor.csv`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/tests/test_sbml_test_suite.py` & `simbio-0.4/src/simbio/io/sbml/tests/test_sbml_test_suite.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/io/sbml/types.py` & `simbio-0.4/src/simbio/io/sbml/types.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/reactions/__init__.py` & `simbio-0.4/src/simbio/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/reactions/compound.py` & `simbio-0.4/src/simbio/reactions/compound.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/reactions/enzymatic.py` & `simbio-0.4/src/simbio/reactions/enzymatic.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/reactions/single.py` & `simbio-0.4/src/simbio/reactions/single.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/reactions/test_reactions.py` & `simbio-0.4/src/simbio/reactions/test_reactions.py`

 * *Files identical despite different names*

### Comparing `SimBio-0.3.2/src/simbio/test_core.py` & `simbio-0.4/src/simbio/test_core.py`

 * *Files identical despite different names*

