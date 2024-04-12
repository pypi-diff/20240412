# Comparing `tmp/modopt-1.7.1.tar.gz` & `tmp/modopt-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modopt-1.7.1.tar", last modified: Fri Jan 19 12:05:19 2024, max compression
+gzip compressed data, was "modopt-1.7.2.tar", last modified: Fri Apr 12 10:21:49 2024, max compression
```

## Comparing `modopt-1.7.1.tar` & `modopt-1.7.2.tar`

### file list

```diff
@@ -1,69 +1,118 @@
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1071 2024-01-08 11:37:51.000000 modopt-1.7.1/LICENCE.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      114 2024-01-16 09:05:29.000000 modopt-1.7.1/MANIFEST.in
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6124 2024-01-19 12:05:19.994281 modopt-1.7.1/PKG-INFO
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4118 2024-01-16 09:05:43.000000 modopt-1.7.1/README.md
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      195 2024-01-16 09:06:10.000000 modopt-1.7.1/develop.txt
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/docs/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      180 2024-01-16 09:05:43.000000 modopt-1.7.1/docs/requirements.txt
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/modopt/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      470 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/__init__.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/modopt/base/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      311 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/base/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5602 2024-01-19 12:04:45.000000 modopt-1.7.1/modopt/base/backend.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5785 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/base/np_adjust.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7482 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/base/observable.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7571 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/base/transform.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4435 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/base/types.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      969 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/base/wrappers.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/modopt/examples/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      212 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/examples/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1220 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/examples/conftest.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4089 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/examples/example_lasso_forward_backward.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/modopt/interface/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      212 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/interface/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     3357 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/interface/errors.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1704 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/interface/log.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.990281 modopt-1.7.1/modopt/math/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      222 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/math/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4394 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/math/convolve.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9245 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/math/matrix.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5552 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/math/metrics.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6858 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/math/stats.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt/opt/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      261 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/opt/__init__.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt/opt/algorithms/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1871 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/algorithms/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9865 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/algorithms/admm.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9328 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/algorithms/base.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    32236 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/algorithms/forward_backward.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    12249 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/opt/algorithms/gradient_descent.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8690 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/algorithms/primal_dual.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8613 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/cost.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7102 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/opt/gradient.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt/opt/linear/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      448 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/linear/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7243 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/linear/base.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6294 2024-01-19 12:04:45.000000 modopt-1.7.1/modopt/opt/linear/wavelet.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    38964 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/opt/proximity.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2404 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/opt/reweight.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt/plot/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      186 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/plot/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1196 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/plot/cost_plot.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt/signal/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      243 2024-01-08 11:37:51.000000 modopt-1.7.1/modopt/signal/__init__.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2512 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/signal/filter.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4985 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/signal/noise.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2408 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/signal/positivity.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8422 2024-01-16 09:05:43.000000 modopt-1.7.1/modopt/signal/svd.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1940 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/signal/validation.py
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9936 2024-01-16 09:05:29.000000 modopt-1.7.1/modopt/signal/wavelet.py
-drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-19 12:05:19.994281 modopt-1.7.1/modopt.egg-info/
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6124 2024-01-19 12:05:19.000000 modopt-1.7.1/modopt.egg-info/PKG-INFO
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1375 2024-01-19 12:05:19.000000 modopt-1.7.1/modopt.egg-info/SOURCES.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)        1 2024-01-19 12:05:19.000000 modopt-1.7.1/modopt.egg-info/dependency_links.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      450 2024-01-19 12:05:19.000000 modopt-1.7.1/modopt.egg-info/requires.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)        7 2024-01-19 12:05:19.000000 modopt-1.7.1/modopt.egg-info/top_level.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)       66 2024-01-16 09:05:43.000000 modopt-1.7.1/requirements.txt
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2359 2024-01-19 12:05:19.994281 modopt-1.7.1/setup.cfg
--rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2123 2024-01-19 12:04:45.000000 modopt-1.7.1/setup.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      100 2024-01-08 11:37:51.000000 modopt-1.7.2/.coveragerc
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.812115 modopt-1.7.2/.github/
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.816115 modopt-1.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      977 2024-01-08 11:37:51.000000 modopt-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      778 2024-01-08 11:37:51.000000 modopt-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      219 2024-01-08 11:37:51.000000 modopt-1.7.2/.github/ISSUE_TEMPLATE/help-.md
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      732 2024-01-08 11:37:51.000000 modopt-1.7.2/.github/ISSUE_TEMPLATE/installation-issue.md
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.816115 modopt-1.7.2/.github/workflows/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1688 2024-04-12 10:21:14.000000 modopt-1.7.2/.github/workflows/cd-build.yml
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1591 2024-04-12 10:21:14.000000 modopt-1.7.2/.github/workflows/ci-build.yml
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      816 2024-04-12 10:21:14.000000 modopt-1.7.2/.github/workflows/style.yml
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2138 2024-04-12 10:21:14.000000 modopt-1.7.2/.gitignore
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     3219 2024-01-08 11:37:51.000000 modopt-1.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8158 2024-01-08 11:37:51.000000 modopt-1.7.2/CONTRIBUTING.md
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1071 2024-01-08 11:37:51.000000 modopt-1.7.2/LICENCE.txt
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6620 2024-04-12 10:21:49.820115 modopt-1.7.2/PKG-INFO
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4118 2024-04-12 10:21:14.000000 modopt-1.7.2/README.md
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.816115 modopt-1.7.2/docs/
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.816115 modopt-1.7.2/docs/_templates/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      174 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/_templates/module.rst_t
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1060 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/_templates/package.rst_t
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      128 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/_templates/toc.rst_t
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      180 2024-04-12 10:21:14.000000 modopt-1.7.2/docs/requirements.txt
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/docs/source/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1583 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/about.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      186 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/citing.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8163 2024-04-12 10:21:14.000000 modopt-1.7.2/docs/source/conf.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      569 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/contributing.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)   116127 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/cosmostat_logo.jpg
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2243 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/dependencies.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      744 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/index.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1182 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/installation.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)   622687 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/modopt_logo.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      921 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/my_ref.bib
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    97699 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/neurospin_logo.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)       87 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/notebooks.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    17262 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/output_17_0.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    17262 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/output_21_0.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8346 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/output_5_0.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    11844 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/output_9_0.png
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6265 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/plugin_example.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      157 2024-01-08 11:37:51.000000 modopt-1.7.2/docs/source/quickstart.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7567 2024-04-12 10:21:14.000000 modopt-1.7.2/docs/source/refs.bib
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      450 2024-04-12 10:21:14.000000 modopt-1.7.2/docs/source/toc.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)       50 2024-01-16 09:05:29.000000 modopt-1.7.2/docs/source/z_ref.rst
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/examples/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      100 2024-04-12 10:21:14.000000 modopt-1.7.2/examples/README.rst
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      212 2024-04-12 10:21:14.000000 modopt-1.7.2/examples/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1223 2024-04-12 10:21:14.000000 modopt-1.7.2/examples/conftest.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4106 2024-04-12 10:21:14.000000 modopt-1.7.2/examples/example_lasso_forward_backward.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/notebooks/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)        0 2024-01-08 11:37:51.000000 modopt-1.7.2/notebooks/.gitkeep
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1494 2024-04-12 10:21:14.000000 modopt-1.7.2/pyproject.toml
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)       38 2024-04-12 10:21:49.820115 modopt-1.7.2/setup.cfg
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.812115 modopt-1.7.2/src/
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      566 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/__init__.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/base/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      274 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5579 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/backend.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5744 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/np_adjust.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7407 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/observable.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7619 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/transform.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     3968 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/base/types.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/interface/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      187 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/interface/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     3280 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/interface/errors.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1670 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/interface/log.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/math/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      197 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/math/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     4395 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/math/convolve.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9307 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/math/matrix.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5501 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/math/metrics.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6789 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/math/stats.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/opt/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      236 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/__init__.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/opt/algorithms/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1624 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9869 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/admm.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9291 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/base.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    32095 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/forward_backward.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    12207 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/gradient_descent.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8621 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/algorithms/primal_dual.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8567 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/cost.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7041 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/gradient.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/opt/linear/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      448 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/linear/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     7195 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/linear/base.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    14993 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/linear/wavelet.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    39335 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/proximity.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2361 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/opt/reweight.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/plot/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      161 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/plot/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     1162 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/plot/cost_plot.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt/signal/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      218 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2485 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/filter.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     5116 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/noise.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2383 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/positivity.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8319 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/svd.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2158 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/validation.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9870 2024-04-12 10:21:14.000000 modopt-1.7.2/src/modopt/signal/wavelet.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/src/modopt.egg-info/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6620 2024-04-12 10:21:49.000000 modopt-1.7.2/src/modopt.egg-info/PKG-INFO
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     2590 2024-04-12 10:21:49.000000 modopt-1.7.2/src/modopt.egg-info/SOURCES.txt
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)        1 2024-04-12 10:21:49.000000 modopt-1.7.2/src/modopt.egg-info/dependency_links.txt
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      250 2024-04-12 10:21:49.000000 modopt-1.7.2/src/modopt.egg-info/requires.txt
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)        7 2024-04-12 10:21:49.000000 modopt-1.7.2/src/modopt.egg-info/top_level.txt
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/tests/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     8525 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_algorithms.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     6467 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_base.py
+drwxr-xr-x   0 cg260486 (1342872018) domain users (150600513)        0 2024-04-12 10:21:49.820115 modopt-1.7.2/tests/test_helpers/
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      122 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_helpers/__init__.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)      748 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_helpers/utils.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)     9744 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_math.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    16214 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_opt.py
+-rw-r--r--   0 cg260486 (1342872018) domain users (150600513)    10127 2024-04-12 10:21:14.000000 modopt-1.7.2/tests/test_signal.py
```

### Comparing `modopt-1.7.1/LICENCE.txt` & `modopt-1.7.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `modopt-1.7.1/PKG-INFO` & `modopt-1.7.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 Metadata-Version: 2.1
 Name: modopt
-Version: 1.7.1
+Version: 1.7.2
 Summary: Modular Optimisation tools for soliving inverse problems.
-Home-page: https://github.com/cea-cosmic/modopt
-Author: Samuel Farrens
-Author-email: samuel.farrens@cea.fr
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Author-email: Samuel Farrens <samuel.farrens@cea.fr>, Chaithya GR <chaithyagr@gmail.com>, Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>, Philippe Ciuciu <philippe.ciuciu@cea.fr>
+License: MIT License
+        
+        Copyright (c) 2017 Samuel Farrens
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: importlib_metadata>=3.7.0
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: scipy>=1.5.4
-Requires-Dist: tqdm>=4.64.0
-Provides-Extra: develop
-Requires-Dist: coverage>=5.5; extra == "develop"
-Requires-Dist: pytest>=6.2.2; extra == "develop"
-Requires-Dist: pytest-raises>=0.10; extra == "develop"
-Requires-Dist: pytest-cases>=3.6; extra == "develop"
-Requires-Dist: pytest-xdist>=3.0.1; extra == "develop"
-Requires-Dist: pytest-cov>=2.11.1; extra == "develop"
-Requires-Dist: pytest-emoji>=0.2.0; extra == "develop"
-Requires-Dist: pydocstyle==6.1.1; extra == "develop"
-Requires-Dist: pytest-pydocstyle>=2.2.0; extra == "develop"
-Requires-Dist: black; extra == "develop"
-Requires-Dist: isort; extra == "develop"
-Requires-Dist: pytest-black; extra == "develop"
-Requires-Dist: jupyter==1.0.0; extra == "develop"
-Requires-Dist: myst-parser==0.16.1; extra == "develop"
-Requires-Dist: nbsphinx==0.8.7; extra == "develop"
-Requires-Dist: nbsphinx-link==1.3.0; extra == "develop"
-Requires-Dist: numpydoc==1.1.0; extra == "develop"
-Requires-Dist: sphinx==4.3.1; extra == "develop"
-Requires-Dist: sphinxcontrib-bibtex==2.4.1; extra == "develop"
-Requires-Dist: sphinxawesome-theme==3.2.1; extra == "develop"
-Requires-Dist: sphinx-gallery==0.11.1; extra == "develop"
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: importlib_metadata
+Provides-Extra: gpu
+Requires-Dist: torch; extra == "gpu"
+Requires-Dist: ptwt; extra == "gpu"
+Provides-Extra: doc
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: nbsphinx-link; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: sphinxawesome-theme; extra == "doc"
+Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest<8.0.0; extra == "test"
+Requires-Dist: pytest-cases; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
 
 # ModOpt
 
 <img width=400 src="https://raw.githubusercontent.com/CEA-COSMIC/ModOpt/master/docs/source/modopt_logo.png">
 
 | Usage | Development | Release |
 | ----- | ----------- | ------- |
```

### Comparing `modopt-1.7.1/README.md` & `modopt-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `modopt-1.7.1/modopt/base/backend.py` & `modopt-1.7.2/src/modopt/base/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """BACKEND MODULE.
 
 This module contains methods for GPU Compatiblity.
 
 :Author: Chaithya G R <chaithyagr@gmail.com>
 
 """
@@ -22,30 +20,32 @@
 except ImportError:  # pragma: no cover
     import_torch = False
 else:
     import_torch = True
 
 # Handle the compatibility with variable
 LIBRARIES = {
-    'cupy': None,
-    'tensorflow': None,
-    'numpy': np,
+    "cupy": None,
+    "tensorflow": None,
+    "numpy": np,
 }
 
-if util.find_spec('cupy') is not None:
+if util.find_spec("cupy") is not None:
     try:
         import cupy as cp
-        LIBRARIES['cupy'] = cp
+
+        LIBRARIES["cupy"] = cp
     except ImportError:
         pass
 
-if util.find_spec('tensorflow') is not None:
+if util.find_spec("tensorflow") is not None:
     try:
         from tensorflow.experimental import numpy as tnp
-        LIBRARIES['tensorflow'] = tnp
+
+        LIBRARIES["tensorflow"] = tnp
     except ImportError:
         pass
 
 
 def get_backend(backend):
     """Get backend.
 
@@ -62,20 +62,20 @@
     tuple
         Returns the module for carrying out calculations and the actual backend
         that was reverted towards. If the right libraries are not installed,
         the function warns and reverts to the ``'numpy'`` backend.
     """
     if backend not in LIBRARIES.keys() or LIBRARIES[backend] is None:
         msg = (
-            '{0} backend not possible, please ensure that '
-            + 'the optional libraries are installed.\n'
-            + 'Reverting to numpy.'
+            "{0} backend not possible, please ensure that "
+            + "the optional libraries are installed.\n"
+            + "Reverting to numpy."
         )
         warn(msg.format(backend))
-        backend = 'numpy'
+        backend = "numpy"
     return LIBRARIES[backend], backend
 
 
 def get_array_module(input_data):
     """Get Array Module.
 
     This method returns the array module, which tells if the data is residing
@@ -88,24 +88,24 @@
 
     Returns
     -------
     module
         The numpy or cupy module
 
     """
-    if LIBRARIES['tensorflow'] is not None:
-        if isinstance(input_data, LIBRARIES['tensorflow'].ndarray):
-            return LIBRARIES['tensorflow']
-    if LIBRARIES['cupy'] is not None:
-        if isinstance(input_data, LIBRARIES['cupy'].ndarray):
-            return LIBRARIES['cupy']
+    if LIBRARIES["tensorflow"] is not None:
+        if isinstance(input_data, LIBRARIES["tensorflow"].ndarray):
+            return LIBRARIES["tensorflow"]
+    if LIBRARIES["cupy"] is not None:
+        if isinstance(input_data, LIBRARIES["cupy"].ndarray):
+            return LIBRARIES["cupy"]
     return np
 
 
-def change_backend(input_data, backend='cupy'):
+def change_backend(input_data, backend="cupy"):
     """Move data to device.
 
     This method changes the backend of an array. This can be used to copy data
     to GPU or to CPU.
 
     Parameters
     ----------
@@ -147,21 +147,21 @@
     Raises
     ------
     ValueError
         if the input does not correspond to any array
     """
     xp = get_array_module(input_data)
 
-    if xp == LIBRARIES['numpy']:
+    if xp == LIBRARIES["numpy"]:
         return input_data
-    elif xp == LIBRARIES['cupy']:
+    elif xp == LIBRARIES["cupy"]:
         return input_data.get()
-    elif xp == LIBRARIES['tensorflow']:
+    elif xp == LIBRARIES["tensorflow"]:
         return input_data.data.numpy()
-    raise ValueError('Cannot identify the array type.')
+    raise ValueError("Cannot identify the array type.")
 
 
 def convert_to_tensor(input_data):
     """Convert data to a tensor.
 
     This method converts input data to a torch tensor. Particularly, this
     method is helpful to convert CuPy array to Tensor.
@@ -180,17 +180,17 @@
     ------
     ImportError
         If Torch package not found
 
     """
     if not import_torch:
         raise ImportError(
-            'Required version of Torch package not found'
-            + 'see documentation for details: https://cea-cosmic.'
-            + 'github.io/ModOpt/#optional-packages',
+            "Required version of Torch package not found"
+            + "see documentation for details: https://cea-cosmic."
+            + "github.io/ModOpt/#optional-packages",
         )
 
     xp = get_array_module(input_data)
 
     if xp == np:
         return torch.Tensor(input_data)
 
@@ -216,16 +216,16 @@
     ------
     ImportError
         If Torch package not found
 
     """
     if not import_torch:
         raise ImportError(
-            'Required version of Torch package not found'
-            + 'see documentation for details: https://cea-cosmic.'
-            + 'github.io/ModOpt/#optional-packages',
+            "Required version of Torch package not found"
+            + "see documentation for details: https://cea-cosmic."
+            + "github.io/ModOpt/#optional-packages",
         )
 
     if input_data.is_cuda:
         return cp.fromDlpack(torch_to_dlpack(input_data))
 
     return input_data.detach().numpy()
```

### Comparing `modopt-1.7.1/modopt/base/np_adjust.py` & `modopt-1.7.2/src/modopt/base/np_adjust.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """NUMPY ADJUSTMENT ROUTINES.
 
 This module contains methods for adjusting the default output for certain
 Numpy functions.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
@@ -150,25 +148,24 @@
 
     if isinstance(padding, int):
         padding = np.array([padding])
     elif isinstance(padding, (tuple, list)):
         padding = np.array(padding)
     elif not isinstance(padding, np.ndarray):
         raise ValueError(
-            'Padding must be an integer or a tuple (or list, np.ndarray) '
-            + 'of itegers',
+            "Padding must be an integer or a tuple (or list, np.ndarray) of integers",
         )
 
     if padding.size == 1:
         padding = np.repeat(padding, 2)
 
     pad_x = (padding[0], padding[0])
     pad_y = (padding[1], padding[1])
 
-    return np.pad(input_data, (pad_x, pad_y), 'constant')
+    return np.pad(input_data, (pad_x, pad_y), "constant")
 
 
 def ftr(input_data):
     """Fancy transpose right.
 
     Apply ``fancy_transpose`` to data with ``roll=1``.
```

### Comparing `modopt-1.7.1/modopt/base/observable.py` & `modopt-1.7.2/src/modopt/base/observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-# -*- coding: utf-8 -*-
-
 """Observable.
 
 This module contains observable classes
 
 :Author: Benoir Sarthou
 
 """
 
 import time
 
 import numpy as np
 
 
-class SignalObject(object):
+class SignalObject:
     """Dummy class for signals."""
 
     pass
 
 
-class Observable(object):
+class Observable:
     """Base class for observable classes.
 
     This class defines a simple interface to add or remove observers
     on an object.
 
     Parameters
     ----------
     signals : list
         The allowed signals
 
     """
 
     def __init__(self, signals):
-
         # Define class parameters
         self._allowed_signals = []
         self._observers = {}
 
         # Set allowed signals
         for signal in signals:
             self._allowed_signals.append(signal)
@@ -173,15 +170,15 @@
             An obervation function to be removed
 
         """
         if observer in self._observers[signal]:
             self._observers[signal].remove(observer)
 
 
-class MetricObserver(object):
+class MetricObserver:
     """Metric observer.
 
     Wrapper of the metric to the observer object notify by the Observable
     class.
 
     Parameters
     ----------
@@ -211,15 +208,14 @@
         metric,
         mapping,
         cst_kwargs,
         early_stopping=False,
         wind=6,
         eps=1.0e-3,
     ):
-
         self.name = name
         self.metric = metric
         self.mapping = mapping
         self.cst_kwargs = cst_kwargs
         self.list_cv_values = []
         self.list_iters = []
         self.list_dates = []
@@ -260,17 +256,15 @@
         """
         if len(self.list_cv_values) < self.wind:
             return
         start_idx = -self.wind
         mid_idx = -(self.wind // 2)
         old_mean = np.array(self.list_cv_values[start_idx:mid_idx]).mean()
         current_mean = np.array(self.list_cv_values[mid_idx:]).mean()
-        normalize_residual_metrics = (
-            np.abs(old_mean - current_mean) / np.abs(old_mean)
-        )
+        normalize_residual_metrics = np.abs(old_mean - current_mean) / np.abs(old_mean)
         self.converge_flag = normalize_residual_metrics < self.eps
 
     def retrieve_metrics(self):
         """Retrieve metrics.
 
         Return the convergence metrics saved with the corresponding
         iterations.
@@ -283,11 +277,11 @@
         """
         time_val = np.array(self.list_dates)
 
         if time_val.size >= 1:
             time_val -= time_val[0]
 
         return {
-            'time': time_val,
-            'index': self.list_iters,
-            'values': self.list_cv_values,
+            "time": time_val,
+            "index": self.list_iters,
+            "values": self.list_cv_values,
         }
```

### Comparing `modopt-1.7.1/modopt/base/transform.py` & `modopt-1.7.2/src/modopt/base/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """DATA TRANSFORM ROUTINES.
 
 This module contains methods for transforming data.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -49,26 +47,25 @@
 
     See Also
     --------
     map2cube : complimentary function
 
     """
     if data_cube.ndim != 3:
-        raise ValueError('The input data must have 3 dimensions.')
+        raise ValueError("The input data must have 3 dimensions.")
 
     if data_cube.shape[0] != np.prod(layout):
         raise ValueError(
-            'The desired layout must match the number of input '
-            + 'data layers.',
+            "The desired layout must match the number of input " + "data layers.",
         )
 
-    res = ([
+    res = [
         np.hstack(data_cube[slice(layout[1] * elem, layout[1] * (elem + 1))])
         for elem in range(layout[0])
-    ])
+    ]
 
     return np.vstack(res)
 
 
 def map2cube(data_map, layout):
     """Map to cube.
 
@@ -114,28 +111,32 @@
     See Also
     --------
     cube2map : complimentary function
 
     """
     if np.all(np.array(data_map.shape) % np.array(layout)):
         raise ValueError(
-            'The desired layout must be a multiple of the number '
-            + 'pixels in the data map.',
+            "The desired layout must be a multiple of the number "
+            + "pixels in the data map.",
         )
 
     d_shape = np.array(data_map.shape) // np.array(layout)
 
-    return np.array([
-        data_map[(
-            slice(i_elem * d_shape[0], (i_elem + 1) * d_shape[0]),
-            slice(j_elem * d_shape[1], (j_elem + 1) * d_shape[1]),
-        )]
-        for i_elem in range(layout[0])
-        for j_elem in range(layout[1])
-    ])
+    return np.array(
+        [
+            data_map[
+                (
+                    slice(i_elem * d_shape[0], (i_elem + 1) * d_shape[0]),
+                    slice(j_elem * d_shape[1], (j_elem + 1) * d_shape[1]),
+                )
+            ]
+            for i_elem in range(layout[0])
+            for j_elem in range(layout[1])
+        ]
+    )
 
 
 def map2matrix(data_map, layout):
     """Map to Matrix.
 
     This method transforms a 2D map to a 2D matrix.
 
@@ -182,17 +183,17 @@
             image_shape * (i_elem % layout[1]),
         )
         upper = (
             image_shape * (i_elem // layout[1] + 1),
             image_shape * (i_elem % layout[1] + 1),
         )
         data_matrix.append(
-            (
-                data_map[lower[0]:upper[0], lower[1]:upper[1]]
-            ).reshape(image_shape ** 2),
+            (data_map[lower[0] : upper[0], lower[1] : upper[1]]).reshape(
+                image_shape**2
+            ),
         )
 
     return np.array(data_matrix).T
 
 
 def matrix2map(data_matrix, map_shape):
     """Matrix to Map.
@@ -228,15 +229,15 @@
     map2matrix : complimentary function
 
     """
     map_shape = np.array(map_shape)
 
     # Get the shape and layout of the images
     image_shape = np.sqrt(data_matrix.shape[0]).astype(int)
-    layout = np.array(map_shape // np.repeat(image_shape, 2), dtype='int')
+    layout = np.array(map_shape // np.repeat(image_shape, 2), dtype="int")
 
     # Map objects from matrix
     data_map = np.zeros(map_shape)
 
     temp = data_matrix.reshape(image_shape, image_shape, data_matrix.shape[1])
 
     for i_elem in range(data_matrix.shape[1]):
@@ -244,15 +245,15 @@
             image_shape * (i_elem // layout[1]),
             image_shape * (i_elem % layout[1]),
         )
         upper = (
             image_shape * (i_elem // layout[1] + 1),
             image_shape * (i_elem % layout[1] + 1),
         )
-        data_map[lower[0]:upper[0], lower[1]:upper[1]] = temp[:, :, i_elem]
+        data_map[lower[0] : upper[0], lower[1] : upper[1]] = temp[:, :, i_elem]
 
     return data_map.astype(int)
 
 
 def cube2matrix(data_cube):
     """Cube to Matrix.
 
@@ -281,15 +282,15 @@
 
     See Also
     --------
     matrix2cube : complimentary function
 
     """
     return data_cube.reshape(
-        [data_cube.shape[0]] + [np.prod(data_cube.shape[1:])],
+        [data_cube.shape[0], np.prod(data_cube.shape[1:])],
     ).T
 
 
 def matrix2cube(data_matrix, im_shape):
     """Matrix to Cube.
 
     This method transforms a 2D matrix to a 3D cube.
@@ -326,8 +327,8 @@
             [14, 15]]])
 
     See Also
     --------
     cube2matrix : complimentary function
 
     """
-    return data_matrix.T.reshape([data_matrix.shape[1]] + list(im_shape))
+    return data_matrix.T.reshape([data_matrix.shape[1], *list(im_shape)])
```

### Comparing `modopt-1.7.1/modopt/base/types.py` & `modopt-1.7.2/src/modopt/base/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,38 @@
-# -*- coding: utf-8 -*-
-
 """TYPE HANDLING ROUTINES.
 
 This module contains methods for handing object types.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
 
 import numpy as np
-
-from modopt.base.wrappers import add_args_kwargs
 from modopt.interface.errors import warn
 
 
-def check_callable(input_obj, add_agrs=True):
+def check_callable(input_obj):
     """Check input object is callable.
 
     This method checks if the input operator is a callable funciton and
     optionally adds support for arguments and keyword arguments if not already
     provided.
 
     Parameters
     ----------
     input_obj : callable
         Callable function
-    add_agrs : bool, optional
-        Option to add support for agrs and kwargs (default is ``True``)
-
-    Returns
-    -------
-    function
-        Function wrapped by ``add_args_kwargs``
 
     Raises
     ------
     TypeError
         For invalid input type
-
-    See Also
-    --------
-    modopt.base.wrappers.add_args_kwargs : wrapper used
-
     """
     if not callable(input_obj):
-        raise TypeError('The input object must be a callable function.')
-
-    if add_agrs:
-        input_obj = add_args_kwargs(input_obj)
-
+        raise TypeError("The input object must be a callable function.")
     return input_obj
 
 
 def check_float(input_obj):
     """Check Float.
 
     Check if input object is a float or a numpy.ndarray of floats, if not
@@ -85,22 +65,21 @@
 
     See Also
     --------
     check_int : related function
 
     """
     if not isinstance(input_obj, (int, float, list, tuple, np.ndarray)):
-        raise TypeError('Invalid input type.')
+        raise TypeError("Invalid input type.")
     if isinstance(input_obj, int):
         input_obj = float(input_obj)
     elif isinstance(input_obj, (list, tuple)):
         input_obj = np.array(input_obj, dtype=float)
-    elif (
-        isinstance(input_obj, np.ndarray)
-        and (not np.issubdtype(input_obj.dtype, np.floating))
+    elif isinstance(input_obj, np.ndarray) and (
+        not np.issubdtype(input_obj.dtype, np.floating)
     ):
         input_obj = input_obj.astype(float)
 
     return input_obj
 
 
 def check_int(input_obj):
@@ -135,22 +114,21 @@
 
     See Also
     --------
     check_float : related function
 
     """
     if not isinstance(input_obj, (int, float, list, tuple, np.ndarray)):
-        raise TypeError('Invalid input type.')
+        raise TypeError("Invalid input type.")
     if isinstance(input_obj, float):
         input_obj = int(input_obj)
     elif isinstance(input_obj, (list, tuple)):
         input_obj = np.array(input_obj, dtype=int)
-    elif (
-        isinstance(input_obj, np.ndarray)
-        and (not np.issubdtype(input_obj.dtype, np.integer))
+    elif isinstance(input_obj, np.ndarray) and (
+        not np.issubdtype(input_obj.dtype, np.integer)
     ):
         input_obj = input_obj.astype(int)
 
     return input_obj
 
 
 def check_npndarray(input_obj, dtype=None, writeable=True, verbose=True):
@@ -174,23 +152,22 @@
     TypeError
         For invalid input type
     TypeError
         For invalid numpy.ndarray dtype
 
     """
     if not isinstance(input_obj, np.ndarray):
-        raise TypeError('Input is not a numpy array.')
+        raise TypeError("Input is not a numpy array.")
 
-    if (
-        (not isinstance(dtype, type(None)))
-        and (not np.issubdtype(input_obj.dtype, dtype))
+    if (not isinstance(dtype, type(None))) and (
+        not np.issubdtype(input_obj.dtype, dtype)
     ):
         raise (
             TypeError(
-                'The numpy array elements are not of type: {0}'.format(dtype),
+                f"The numpy array elements are not of type: {dtype}",
             ),
         )
 
     if not writeable and verbose and input_obj.flags.writeable:
-        warn('Making input data immutable.')
+        warn("Making input data immutable.")
 
     input_obj.flags.writeable = writeable
```

### Comparing `modopt-1.7.1/modopt/examples/conftest.py` & `modopt-1.7.2/examples/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 
 Notes
 -----
 Based on:
 https://stackoverflow.com/questions/56807698/how-to-run-script-as-pytest-test
 
 """
+
 from pathlib import Path
 import runpy
 import pytest
 
+
 def pytest_collect_file(path, parent):
     """Pytest hook.
 
     Create a collector for the given path, or None if not relevant.
     The new node needs to have the specified parent as parent.
     """
     p = Path(path)
-    if p.suffix == '.py' and 'example' in p.name:
+    if p.suffix == ".py" and "example" in p.name:
         return Script.from_parent(parent, path=p, name=p.name)
 
 
 class Script(pytest.File):
     """Script files collected by pytest."""
 
     def collect(self):
         """Collect the script as its own item."""
         yield ScriptItem.from_parent(self, name=self.name)
 
+
 class ScriptItem(pytest.Item):
     """Item script collected by pytest."""
 
     def runtest(self):
         """Run the script as a test."""
         runpy.run_path(str(self.path))
```

### Comparing `modopt-1.7.1/modopt/examples/example_lasso_forward_backward.py` & `modopt-1.7.2/examples/example_lasso_forward_backward.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# noqa: D205
 """
 Solving the LASSO Problem with the Forward Backward Algorithm.
 ==============================================================
 
 This an example to show how to solve an example LASSO Problem
 using the Forward-Backward Algorithm.
 
@@ -72,15 +71,15 @@
 fb_fista = ForwardBackward(
     np.zeros(8),
     beta_param=1 / lip,
     grad=grad_op,
     prox=prox_op,
     cost=cost_op_fista,
     metric_call_period=1,
-    auto_iterate=False, # Just to give us the pleasure of doing things by ourself.
+    auto_iterate=False,  # Just to give us the pleasure of doing things by ourself.
 )
 
 fb_fista.iterate()
 
 # %%
 # After the run we can have a look at the results
 
@@ -111,15 +110,15 @@
     np.zeros(8),
     np.zeros(8),
     beta_param=1 / lip,
     grad=grad_op,
     prox=prox_op,
     cost=cost_op_pogm,
     metric_call_period=1,
-    auto_iterate=False, # Just to give us the pleasure of doing things by ourself.
+    auto_iterate=False,  # Just to give us the pleasure of doing things by ourself.
 )
 
 fb_pogm.iterate()
 
 # %%
 # After the run we can have a look at the results
 
@@ -129,14 +128,15 @@
 plt.stem(fb_pogm.x_final, label="estimation", linefmt="C0-")
 plt.stem(BETA_TRUE, label="reference", linefmt="C1-")
 plt.legend()
 plt.title(f"FISTA Estimation MSE={mse_pogm:.4f}")
 #
 # sphinx_gallery_start_ignore
 assert mse(fb_pogm.x_final, BETA_TRUE) < 1
+# sphinx_gallery_end_ignore
 
 # %%
 # Comparing the Two algorithms
 # ----------------------------
 
 plt.figure()
 plt.semilogy(cost_op_fista._cost_list, label="FISTA convergence")
```

### Comparing `modopt-1.7.1/modopt/interface/errors.py` & `modopt-1.7.2/src/modopt/interface/errors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ERROR HANDLING ROUTINES.
 
 This module contains methods for handing warnings and errors.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -30,24 +28,24 @@
     warn_string : str
         Warning message string
     log : logging.Logger, optional
         Logging structure instance (default is ``None``)
 
     """
     if import_fail:
-        warn_txt = 'WARNING'
+        warn_txt = "WARNING"
     else:
-        warn_txt = colored('WARNING', 'yellow')
+        warn_txt = colored("WARNING", "yellow")
 
     # Print warning to stdout.
-    sys.stderr.write('{0}: {1}\n'.format(warn_txt, warn_string))
+    sys.stderr.write(f"{warn_txt}: {warn_string}\n")
 
     # Check if a logging structure is provided.
     if not isinstance(log, type(None)):
-        warnings.warn(warn_string)
+        warnings.warn(warn_string, stacklevel=2)
 
 
 def catch_error(exception, log=None):
     """Catch error.
 
     This method catches errors and prints them to the terminal. It also saves
     the errors to a log if provided.
@@ -57,25 +55,25 @@
     exception : str
         Exception message string
     log : logging.Logger, optional
         Logging structure instance (default is ``None``)
 
     """
     if import_fail:
-        err_txt = 'ERROR'
+        err_txt = "ERROR"
     else:
-        err_txt = colored('ERROR', 'red')
+        err_txt = colored("ERROR", "red")
 
     # Print exception to stdout.
-    stream_txt = '{0}: {1}\n'.format(err_txt, exception)
+    stream_txt = f"{err_txt}: {exception}\n"
     sys.stderr.write(stream_txt)
 
     # Check if a logging structure is provided.
     if not isinstance(log, type(None)):
-        log_txt = 'ERROR: {0}\n'.format(exception)
+        log_txt = f"ERROR: {exception}\n"
         log.exception(log_txt)
 
 
 def file_name_error(file_name):
     """File name error.
 
     This method checks if the input file name is valid.
@@ -87,19 +85,19 @@
 
     Raises
     ------
     IOError
         If file name not specified or file not found
 
     """
-    if file_name == '' or file_name[0][0] == '-':
-        raise IOError('Input file name not specified.')
+    if file_name == "" or file_name[0][0] == "-":
+        raise OSError("Input file name not specified.")
 
     elif not os.path.isfile(file_name):
-        raise IOError('Input file name {0} not found!'.format(file_name))
+        raise OSError(f"Input file name {file_name} not found!")
 
 
 def is_exe(fpath):
     """Is Executable.
 
     Check if the input file path corresponds to an executable on the system.
 
@@ -132,25 +130,23 @@
     TypeError
         For invalid input type
     IOError
         For invalid system executable
 
     """
     if not isinstance(exe_name, str):
-        raise TypeError('Executable name must be a string.')
+        raise TypeError("Executable name must be a string.")
 
     fpath, fname = os.path.split(exe_name)
 
     if fpath:
         res = is_exe(exe_name)
 
     else:
         res = any(
             is_exe(os.path.join(path, exe_name))
-            for path in os.environ['PATH'].split(os.pathsep)
+            for path in os.environ["PATH"].split(os.pathsep)
         )
 
     if not res:
-        message = (
-            '{0} does not appear to be a valid executable on this system.'
-        )
-        raise IOError(message.format(exe_name))
+        message = "{0} does not appear to be a valid executable on this system."
+        raise OSError(message.format(exe_name))
```

### Comparing `modopt-1.7.1/modopt/interface/log.py` & `modopt-1.7.2/src/modopt/interface/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """LOGGING ROUTINES.
 
 This module contains methods for handing logging.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -26,40 +24,40 @@
     Returns
     -------
     logging.Logger
         Logging instance
 
     """
     # Add file extension.
-    filename = '{0}.log'.format(filename)
+    filename = f"{filename}.log"
 
     if verbose:
-        print('Preparing log file:', filename)
+        print("Preparing log file:", filename)
 
     # Capture warnings.
     logging.captureWarnings(True)
 
     # Set output format.
     formatter = logging.Formatter(
-        fmt='%(asctime)s %(message)s',
-        datefmt='%d/%m/%Y %H:%M:%S',
+        fmt="%(asctime)s %(message)s",
+        datefmt="%d/%m/%Y %H:%M:%S",
     )
 
     # Create file handler.
-    fh = logging.FileHandler(filename=filename, mode='w')
+    fh = logging.FileHandler(filename=filename, mode="w")
     fh.setLevel(logging.DEBUG)
     fh.setFormatter(formatter)
 
     # Create log.
     log = logging.getLogger(filename)
     log.setLevel(logging.DEBUG)
     log.addHandler(fh)
 
     # Send opening message.
-    log.info('The log file has been set-up.')
+    log.info("The log file has been set-up.")
 
     return log
 
 
 def close_log(log, verbose=True):
     """Close log.
 
@@ -70,15 +68,15 @@
     log : logging.Logger
         Logging instance
     verbose : bool
         Option for verbose output (default is ``True``)
 
     """
     if verbose:
-        print('Closing log file:', log.name)
+        print("Closing log file:", log.name)
 
     # Send closing message.
-    log.info('The log file has been closed.')
+    log.info("The log file has been closed.")
 
     # Remove all handlers from log.
     for log_handler in log.handlers:
         log.removeHandler(log_handler)
```

### Comparing `modopt-1.7.1/modopt/math/convolve.py` & `modopt-1.7.2/src/modopt/math/convolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """CONVOLUTION ROUTINES.
 
 This module contains methods for convolution.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -14,27 +12,27 @@
 from modopt.base.np_adjust import rotate_stack
 from modopt.interface.errors import warn
 
 try:
     from astropy.convolution import convolve_fft
 except ImportError:  # pragma: no cover
     import_astropy = False
-    warn('astropy not found, will default to scipy for convolution')
+    warn("astropy not found, will default to scipy for convolution")
 else:
     import_astropy = True
 try:
     import pyfftw
 except ImportError:  # pragma: no cover
     pass
 else:  # pragma: no cover
     scipy.fftpack = pyfftw.interfaces.scipy_fftpack
     warn('Using pyFFTW "monkey patch" for scipy.fftpack')
 
 
-def convolve(input_data, kernel, method='scipy'):
+def convolve(input_data, kernel, method="scipy"):
     """Convolve data with kernel.
 
     This method convolves the input data with a given kernel using FFT and
     is the default convolution used for all routines.
 
     Parameters
     ----------
@@ -76,37 +74,37 @@
     See Also
     --------
     scipy.signal.fftconvolve : scipy FFT convolution
     astropy.convolution.convolve_fft : astropy FFT convolution
 
     """
     if input_data.ndim != kernel.ndim:
-        raise ValueError('Data and kernel must have the same dimensions.')
+        raise ValueError("Data and kernel must have the same dimensions.")
 
-    if method not in {'astropy', 'scipy'}:
+    if method not in {"astropy", "scipy"}:
         raise ValueError('Invalid method. Options are "astropy" or "scipy".')
 
     if not import_astropy:  # pragma: no cover
-        method = 'scipy'
+        method = "scipy"
 
-    if method == 'astropy':
+    if method == "astropy":
         return convolve_fft(
             input_data,
             kernel,
-            boundary='wrap',
+            boundary="wrap",
             crop=False,
-            nan_treatment='fill',
+            nan_treatment="fill",
             normalize_kernel=False,
         )
 
-    elif method == 'scipy':
-        return scipy.signal.fftconvolve(input_data, kernel, mode='same')
+    elif method == "scipy":
+        return scipy.signal.fftconvolve(input_data, kernel, mode="same")
 
 
-def convolve_stack(input_data, kernel, rot_kernel=False, method='scipy'):
+def convolve_stack(input_data, kernel, rot_kernel=False, method="scipy"):
     """Convolve stack of data with stack of kernels.
 
     This method convolves the input data with a given kernel using FFT and
     is the default convolution used for all routines.
 
     Parameters
     ----------
@@ -152,11 +150,13 @@
     --------
     convolve : The convolution function called by convolve_stack
 
     """
     if rot_kernel:
         kernel = rotate_stack(kernel)
 
-    return np.array([
-        convolve(data_i, kernel_i, method=method)
-        for data_i, kernel_i in zip(input_data, kernel)
-    ])
+    return np.array(
+        [
+            convolve(data_i, kernel_i, method=method)
+            for data_i, kernel_i in zip(input_data, kernel)
+        ]
+    )
```

### Comparing `modopt-1.7.1/modopt/math/matrix.py` & `modopt-1.7.2/src/modopt/math/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """MATRIX ROUTINES.
 
 This module contains methods for matrix operations.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -11,15 +9,15 @@
 from itertools import product
 
 import numpy as np
 
 from modopt.base.backend import get_array_module, get_backend
 
 
-def gram_schmidt(matrix, return_opt='orthonormal'):
+def gram_schmidt(matrix, return_opt="orthonormal"):
     r"""Gram-Schmit.
 
     This method orthonormalizes the row vectors of the input matrix.
 
     Parameters
     ----------
     matrix : numpy.ndarray
@@ -51,41 +49,40 @@
 
     Notes
     -----
     Implementation from:
     https://en.wikipedia.org/wiki/Gram%E2%80%93Schmidt_process
 
     """
-    if return_opt not in {'orthonormal', 'orthogonal', 'both'}:
+    if return_opt not in {"orthonormal", "orthogonal", "both"}:
         raise ValueError(
             'Invalid return_opt, options are: "orthonormal", "orthogonal" or '
             + '"both"',
         )
 
     u_vec = []
     e_vec = []
 
     for vector in matrix:
-
         if u_vec:
             u_now = vector - sum(project(u_i, vector) for u_i in u_vec)
         else:
             u_now = vector
 
         u_vec.append(u_now)
         e_vec.append(u_now / np.linalg.norm(u_now, 2))
 
     u_vec = np.array(u_vec)
     e_vec = np.array(e_vec)
 
-    if return_opt == 'orthonormal':
+    if return_opt == "orthonormal":
         return e_vec
-    elif return_opt == 'orthogonal':
+    elif return_opt == "orthogonal":
         return u_vec
-    elif return_opt == 'both':
+    elif return_opt == "both":
         return u_vec, e_vec
 
 
 def nuclear_norm(input_data):
     r"""Nuclear norm.
 
     This method computes the nuclear (or trace) norm of the input data.
@@ -197,15 +194,15 @@
             \sin(\theta) & \cos(\theta)
         \end{bmatrix}
 
     """
     return np.around(
         np.array(
             [[np.cos(angle), -np.sin(angle)], [np.sin(angle), np.cos(angle)]],
-            dtype='float',
+            dtype="float",
         ),
         10,
     )
 
 
 def rotate(matrix, angle):
     """Rotate.
@@ -239,30 +236,29 @@
            [1, 4, 7],
            [0, 3, 6]])
 
     """
     shape = np.array(matrix.shape)
 
     if shape[0] != shape[1]:
-        raise ValueError('Input matrix must be square.')
+        raise ValueError("Input matrix must be square.")
 
     shift = (shape - 1) // 2
 
     index = (
-        np.array(list(product(*np.array([np.arange(sval) for sval in shape]))))
-        - shift
+        np.array(list(product(*np.array([np.arange(sval) for sval in shape])))) - shift
     )
 
-    new_index = np.array(np.dot(index, rot_matrix(angle)), dtype='int') + shift
+    new_index = np.array(np.dot(index, rot_matrix(angle)), dtype="int") + shift
     new_index[new_index >= shape[0]] -= shape[0]
 
     return matrix[tuple(zip(new_index.T))].reshape(shape.T)
 
 
-class PowerMethod(object):
+class PowerMethod:
     """Power method class.
 
     This method performs implements power method to calculate the spectral
     radius of the input data.
 
     Parameters
     ----------
@@ -273,14 +269,16 @@
     data_type : {``float``, ``complex``}, optional
         Random data type (default is ``float``)
     auto_run : bool, optional
         Option to automatically calcualte the spectral radius upon
         initialisation (default is ``True``)
     verbose : bool, optional
         Optional verbosity (default is ``False``)
+    rng: int, xp.random.Generator or None (default is ``None``)
+        Random number generator or seed.
 
     Examples
     --------
     >>> import numpy as np
     >>> from modopt.math.matrix import PowerMethod
     >>> np.random.seed(1)
     >>> pm = PowerMethod(lambda x: x.dot(x.T), (3, 3))
@@ -297,24 +295,25 @@
 
     def __init__(
         self,
         operator,
         data_shape,
         data_type=float,
         auto_run=True,
-        compute_backend='numpy',
+        compute_backend="numpy",
         verbose=False,
+        rng=None,
     ):
-
         self._operator = operator
         self._data_shape = data_shape
         self._data_type = data_type
         self._verbose = verbose
         xp, compute_backend = get_backend(compute_backend)
         self.xp = xp
+        self.rng = None
         self.compute_backend = compute_backend
         if auto_run:
             self.get_spec_rad()
 
     def _set_initial_x(self):
         """Set initial value of :math:`x`.
 
@@ -323,15 +322,16 @@
 
         Returns
         -------
         numpy.ndarray
             Random values of the same shape as the input data
 
         """
-        return self.xp.random.random(self._data_shape).astype(self._data_type)
+        rng = self.xp.random.default_rng(self.rng)
+        return rng.random(self._data_shape).astype(self._data_type)
 
     def get_spec_rad(self, tolerance=1e-6, max_iter=20, extra_factor=1.0):
         """Get spectral radius.
 
         This method calculates the spectral radius
 
         Parameters
@@ -359,26 +359,22 @@
 
             x_new = self._operator(x_old)
 
             x_new_norm = xp.linalg.norm(x_new)
 
             x_new /= x_new_norm
 
-            if (xp.abs(x_new_norm - x_old_norm) < tolerance):
-                message = (
-                    ' - Power Method converged after {0} iterations!'
-                )
+            if xp.abs(x_new_norm - x_old_norm) < tolerance:
+                message = " - Power Method converged after {0} iterations!"
                 if self._verbose:
                     print(message.format(i_elem + 1))
                 break
 
             elif i_elem == max_iter - 1 and self._verbose:
-                message = (
-                    ' - Power Method did not converge after {0} iterations!'
-                )
+                message = " - Power Method did not converge after {0} iterations!"
                 print(message.format(max_iter))
 
             xp.copyto(x_old, x_new)
             x_old_norm = x_new_norm
 
         self.spec_rad = x_new_norm * extra_factor
         self.inv_spec_rad = 1.0 / self.spec_rad
```

### Comparing `modopt-1.7.1/modopt/math/metrics.py` & `modopt-1.7.2/src/modopt/math/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """METRICS.
 
 This module contains classes of different metric functions for optimization.
 
 :Author: Benoir Sarthou
 
 """
@@ -67,23 +65,21 @@
 
     Returns
     -------
     float
         The SNR
 
     """
-    test = np.abs(np.copy(test)).astype('float64')
-    ref = np.abs(np.copy(ref)).astype('float64')
+    test = np.abs(np.copy(test)).astype("float64")
+    ref = np.abs(np.copy(ref)).astype("float64")
     test = min_max_normalize(test)
     ref = min_max_normalize(ref)
 
     if (not isinstance(mask, np.ndarray)) and (mask is not None):
-        message = (
-            'Mask should be None, or a numpy.ndarray, got "{0}" instead.'
-        )
+        message = 'Mask should be None, or a numpy.ndarray, got "{0}" instead.'
         raise ValueError(message.format(mask))
 
     if mask is None:
         return test, ref, None
 
     return test, ref, mask
 
@@ -115,17 +111,17 @@
     -------
     float
         The SNR
 
     """
     if not import_skimage:  # pragma: no cover
         raise ImportError(
-            'Required version of Scikit-Image package not found'
-            + 'see documentation for details: https://cea-cosmic.'
-            + 'github.io/ModOpt/#optional-packages',
+            "Required version of Scikit-Image package not found"
+            + "see documentation for details: https://cea-cosmic."
+            + "github.io/ModOpt/#optional-packages",
         )
 
     test, ref, mask = _preprocess_input(test, ref, mask)
     test = move_to_cpu(test)
     assim, ssim_value = compare_ssim(test, ref, full=True, data_range=1.0)
 
     if mask is None:
@@ -266,10 +262,10 @@
     test, ref, mask = _preprocess_input(test, ref, mask)
 
     if mask is not None:
         test = mask * test
         ref = mask * ref
 
     num = np.sqrt(mse(test, ref))
-    deno = np.sqrt(np.mean((np.square(test))))
+    deno = np.sqrt(np.mean(np.square(test)))
 
     return num / deno
```

### Comparing `modopt-1.7.1/modopt/math/stats.py` & `modopt-1.7.2/src/modopt/math/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """STATISTICS ROUTINES.
 
 This module contains methods for basic statistics.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -27,16 +25,16 @@
 
     Parameters
     ----------
     data_shape : tuple
         Desiered shape of the kernel
     sigma : float
         Standard deviation of the kernel
-    norm : {'max', 'sum'}, optional
-        Normalisation of the kerenl (options are ``'max'`` or ``'sum'``, default is ``'max'``)
+    norm : {'max', 'sum'}, optional, default='max'
+        Normalisation of the kernel
 
     Returns
     -------
     numpy.ndarray
         Kernel
 
     Raises
```

### Comparing `modopt-1.7.1/modopt/opt/algorithms/admm.py` & `modopt-1.7.2/src/modopt/opt/algorithms/admm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ADMM Algorithms."""
+
 import numpy as np
 
 from modopt.base.backend import get_array_module
 from modopt.opt.algorithms.base import SetUp
 from modopt.opt.cost import CostParent
 
 
@@ -63,15 +64,16 @@
         cost += self.tau * xp.linalg.norm(self.A.op(u) + self.B.op(v) - self.b)
         return cost
 
 
 class ADMM(SetUp):
     r"""Fast ADMM Optimisation Algorihm.
 
-    This class implement the ADMM algorithm described in :cite:`Goldstein2014` (Algorithm 1).
+    This class implement the ADMM algorithm described in :cite:`Goldstein2014`
+    (Algorithm 1).
 
     Parameters
     ----------
     u: numpy.ndarray
         Initial value for first primal variable of ADMM
     v: numpy.ndarray
         Initial value for second primal variable of ADMM
@@ -81,15 +83,15 @@
         Linear operator for u
     B:  modopt.opt.linear.LinearOperator
         Linear operator for v
     b : numpy.ndarray
         Constraint vector
     optimizers: tuple
         2-tuple of callable, that are the optimizers for the u and v.
-        Each callable should access an init and obs argument and returns an estimate for:
+        Each callable should access init and obs argument and returns an estimate for:
         .. math:: u_{k+1} = \argmin H(u) + \frac{\tau}{2}\|A u - y\|^2
         .. math:: v_{k+1} = \argmin G(v) + \frac{\tau}{2}\|Bv - y \|^2
     cost_funcs: tuple
         2-tuple of callable, that compute values of H and G.
     tau: float, default=1
         Coupling parameter for ADMM.
 
@@ -184,42 +186,42 @@
         """
         self._run_alg(max_iter)
 
         # retrieve metrics results
         self.retrieve_outputs()
         # rename outputs as attributes
         self.u_final = self._u_new
-        self.x_final = self.u_final # for backward compatibility
+        self.x_final = self.u_final  # for backward compatibility
         self.v_final = self._v_new
 
     def get_notify_observers_kwargs(self):
         """Notify observers.
 
         Return the mapping between the metrics call and the iterated
         variables.
 
         Returns
         -------
         dict
            The mapping between the iterated variables
         """
         return {
-            'x_new': self._u_new,
-            'v_new': self._v_new,
-            'idx': self.idx,
+            "x_new": self._u_new,
+            "v_new": self._v_new,
+            "idx": self.idx,
         }
 
     def retrieve_outputs(self):
         """Retrieve outputs.
 
         Declare the outputs of the algorithms as attributes: x_final,
         y_final, metrics.
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
 
 
 class FastADMM(ADMM):
     r"""Fast ADMM Optimisation Algorihm.
 
@@ -238,29 +240,30 @@
         Linear operator for u
     B:  modopt.opt.linear.LinearOperator
         Linear operator for v
     b : numpy.ndarray
         Constraint vector
     optimizers: tuple
         2-tuple of callable, that are the optimizers for the u and v.
-        Each callable should access an init and obs argument and returns an estimate for:
+        Each callable should access init and obs argument and returns an estimate for:
         .. math:: u_{k+1} = \argmin H(u) + \frac{\tau}{2}\|A u - y\|^2
         .. math:: v_{k+1} = \argmin G(v) + \frac{\tau}{2}\|Bv - y \|^2
     cost_funcs: tuple
         2-tuple of callable, that compute values of H and G.
     tau: float, default=1
         Coupling parameter for ADMM.
     eta: float, default=0.999
         Convergence parameter for ADMM.
     alpha: float, default=1.
         Initial value for the FISTA-like acceleration parameter.
 
     Notes
     -----
-    This is an accelerated version of the ADMM algorithm. The convergence hypothesis are stronger than for the ADMM algorithm.
+    This is an accelerated version of the ADMM algorithm. The convergence hypothesis are
+    stronger than for the ADMM algorithm.
 
     See Also
     --------
     ADMM: parent class
     """
 
     def __init__(
```

### Comparing `modopt-1.7.1/modopt/opt/algorithms/base.py` & `modopt-1.7.2/src/modopt/opt/algorithms/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Base SetUp for optimisation algorithms."""
 
 from inspect import getmro
 
 import numpy as np
 from tqdm.auto import tqdm
 
@@ -65,80 +64,77 @@
     def __init__(
         self,
         metric_call_period=5,
         metrics=None,
         verbose=False,
         progress=True,
         step_size=None,
-        compute_backend='numpy',
+        compute_backend="numpy",
         **dummy_kwargs,
     ):
         self.idx = 0
         self.converge = False
         self.verbose = verbose
         self.progress = progress
         self.metrics = metrics
         self.step_size = step_size
         self._op_parents = (
-            'GradParent',
-            'ProximityParent',
-            'LinearParent',
-            'costObj',
+            "GradParent",
+            "ProximityParent",
+            "LinearParent",
+            "costObj",
         )
 
         self.metric_call_period = metric_call_period
 
         # Declaration of observers for metrics
-        super().__init__(['cv_metrics'])
+        super().__init__(["cv_metrics"])
 
         for name, dic in self.metrics.items():
             observer = MetricObserver(
                 name,
-                dic['metric'],
-                dic['mapping'],
-                dic['cst_kwargs'],
-                dic['early_stopping'],
+                dic["metric"],
+                dic["mapping"],
+                dic["cst_kwargs"],
+                dic["early_stopping"],
             )
-            self.add_observer('cv_metrics', observer)
+            self.add_observer("cv_metrics", observer)
 
         xp, compute_backend = backend.get_backend(compute_backend)
         self.xp = xp
         self.compute_backend = compute_backend
 
     @property
     def metrics(self):
         """Set metrics dictionary."""
         return self._metrics
 
     @metrics.setter
     def metrics(self, metrics):
-
         if isinstance(metrics, type(None)):
             self._metrics = {}
         elif isinstance(metrics, dict):
             self._metrics = metrics
         else:
             raise TypeError(
-                'Metrics must be a dictionary, not {0}.'.format(type(metrics)),
+                f"Metrics must be a dictionary, not {type(metrics)}.",
             )
 
     def any_convergence_flag(self):
         """Check convergence flag.
 
         Retur True if any matrix values matched the convergence criteria.
 
         Returns
         -------
         bool
             True if any convergence criteria met
 
         """
-        return any(
-            obs.converge_flag for obs in self._observers['cv_metrics']
-        )
+        return any(obs.converge_flag for obs in self._observers["cv_metrics"])
 
     def copy_data(self, input_data):
         """Copy Data.
 
         Set directive for copying data.
 
         Parameters
@@ -148,18 +144,20 @@
 
         Returns
         -------
         numpy.ndarray
             Copy of input data
 
         """
-        return self.xp.copy(backend.change_backend(
-            input_data,
-            self.compute_backend,
-        ))
+        return self.xp.copy(
+            backend.change_backend(
+                input_data,
+                self.compute_backend,
+            )
+        )
 
     def _check_input_data(self, input_data):
         """Check input data type.
 
         This method checks if the input data is a numpy array
 
         Parameters
@@ -171,15 +169,15 @@
         ------
         TypeError
             For invalid input type
 
         """
         if not (isinstance(input_data, (self.xp.ndarray, np.ndarray))):
             raise TypeError(
-                'Input data must be a numpy array or backend array',
+                "Input data must be a numpy array or backend array",
             )
 
     def _check_param(self, param_val):
         """Check algorithm parameters.
 
         This method checks if the specified algorithm parameters are floats
 
@@ -191,15 +189,15 @@
         Raises
         ------
         TypeError
             For invalid input type
 
         """
         if not isinstance(param_val, float):
-            raise TypeError('Algorithm parameter must be a float value.')
+            raise TypeError("Algorithm parameter must be a float value.")
 
     def _check_param_update(self, param_update):
         """Check algorithm parameter update methods.
 
         This method checks if the specified algorithm parameters are floats
 
         Parameters
@@ -209,22 +207,21 @@
 
         Raises
         ------
         TypeError
             For invalid input type
 
         """
-        param_conditions = (
-            not isinstance(param_update, type(None))
-            and not callable(param_update)
+        param_conditions = not isinstance(param_update, type(None)) and not callable(
+            param_update
         )
 
         if param_conditions:
             raise TypeError(
-                'Algorithm parameter update must be a callabale function.',
+                "Algorithm parameter update must be a callabale function.",
             )
 
     def _check_operator(self, operator):
         """Check set-Up.
 
         This method checks algorithm operator against the expected parent
         classes
@@ -235,26 +232,26 @@
             Algorithm operator to check
 
         """
         if not isinstance(operator, type(None)):
             tree = [op_obj.__name__ for op_obj in getmro(operator.__class__)]
 
             if not any(parent in tree for parent in self._op_parents):
-                message = '{0} does not inherit an operator parent.'
+                message = "{0} does not inherit an operator parent."
                 warn(message.format(str(operator.__class__)))
 
     def _compute_metrics(self):
         """Compute metrics during iteration.
 
         This method create the args necessary for metrics computation, then
         call the observers to compute metrics
 
         """
         kwargs = self.get_notify_observers_kwargs()
-        self.notify_observers('cv_metrics', **kwargs)
+        self.notify_observers("cv_metrics", **kwargs)
 
     def _iterations(self, max_iter, progbar=None):
         """Iterate method.
 
         Iterate the update step of the given algorithm.
 
         Parameters
@@ -269,27 +266,26 @@
             self._update()
 
             # Calling metrics every metric_call_period cycle
             # Also calculate at the end (max_iter or at convergence)
             # We do not call metrics if metrics is empty or metric call
             # period is None
             if self.metrics and self.metric_call_period is not None:
-
                 metric_conditions = (
                     self.idx % self.metric_call_period == 0
                     or self.idx == (max_iter - 1)
                     or self.converge,
                 )
 
                 if metric_conditions:
                     self._compute_metrics()
 
             if self.converge:
                 if self.verbose:
-                    print(' - Converged!')
+                    print(" - Converged!")
                 break
 
             if progbar:
                 progbar.update()
 
     def _run_alg(self, max_iter, progbar=None):
         """Run algorithm.
```

### Comparing `modopt-1.7.1/modopt/opt/algorithms/forward_backward.py` & `modopt-1.7.2/src/modopt/opt/algorithms/forward_backward.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
 """Forward-Backward Algorithms."""
 
 import numpy as np
 
 from modopt.base import backend
 from modopt.opt.algorithms.base import SetUp
 from modopt.opt.cost import costObj
 from modopt.opt.linear import Identity
 
 
-class FISTA(object):
+class FISTA:
     r"""FISTA.
 
     This class is inherited by optimisation classes to speed up convergence
     The parameters for the modified FISTA are as described in :cite:`liang2018`
     :math:`(p, q, r)`-lazy or in :cite:`chambolle2015` (a_cd).
     The restarting strategies are those described in :cite:`liang2018`,
     algorithms 4-5.
@@ -48,20 +47,20 @@
     r_lazy: float
         Parameter for the update of lambda in Fista-Mod, it must satisfy
         :math:`r \in ]0, 4]`
 
     """
 
     _restarting_strategies = (
-        'adaptive',  # option 1 in alg 4
-        'adaptive-i',
-        'adaptive-1',
-        'adaptive-ii',  # option 2 in alg 4
-        'adaptive-2',
-        'greedy',  # alg 5
+        "adaptive",  # option 1 in alg 4
+        "adaptive-i",
+        "adaptive-1",
+        "adaptive-ii",  # option 2 in alg 4
+        "adaptive-2",
+        "greedy",  # alg 5
         None,  # no restarting
     )
 
     def __init__(
         self,
         restart_strategy=None,
         min_beta=None,
@@ -69,45 +68,47 @@
         xi_restart=None,
         a_cd=None,
         p_lazy=1,
         q_lazy=1,
         r_lazy=4,
         **kwargs,
     ):
-
         if isinstance(a_cd, type(None)):
-            self.mode = 'regular'
+            self.mode = "regular"
             self.p_lazy = p_lazy
             self.q_lazy = q_lazy
             self.r_lazy = r_lazy
 
         elif a_cd > 2:
-            self.mode = 'CD'
+            self.mode = "CD"
             self.a_cd = a_cd
             self._n = 0
 
         else:
             raise ValueError(
-                'a_cd must either be None (for regular mode) or a number > 2',
+                "a_cd must either be None (for regular mode) or a number > 2",
             )
 
         if restart_strategy in self._restarting_strategies:
             self._check_restart_params(
-                restart_strategy, min_beta, s_greedy, xi_restart,
+                restart_strategy,
+                min_beta,
+                s_greedy,
+                xi_restart,
             )
             self.restart_strategy = restart_strategy
             self.min_beta = min_beta
             self.s_greedy = s_greedy
             self.xi_restart = xi_restart
 
         else:
-            message = 'Restarting strategy must be one of {0}.'
+            message = "Restarting strategy must be one of {0}."
             raise ValueError(
                 message.format(
-                    ', '.join(self._restarting_strategies),
+                    ", ".join(self._restarting_strategies),
                 ),
             )
         self._t_now = 1.0
         self._t_prev = 1.0
         self._delta0 = None
         self._safeguard = False
 
@@ -151,30 +152,28 @@
             When a parameter that should be set isn't or doesn't verify the
             correct assumptions.
 
         """
         if restart_strategy is None:
             return True
 
-        if self.mode != 'regular':
+        if self.mode != "regular":
             raise ValueError(
-                'Restarting strategies can only be used with regular mode.',
+                "Restarting strategies can only be used with regular mode.",
             )
 
-        greedy_params_check = (
-            min_beta is None or s_greedy is None or s_greedy <= 1
-        )
+        greedy_params_check = min_beta is None or s_greedy is None or s_greedy <= 1
 
-        if restart_strategy == 'greedy' and greedy_params_check:
+        if restart_strategy == "greedy" and greedy_params_check:
             raise ValueError(
-                'You need a min_beta and an s_greedy > 1 for greedy restart.',
+                "You need a min_beta and an s_greedy > 1 for greedy restart.",
             )
 
         if xi_restart is None or xi_restart >= 1:
-            raise ValueError('You need a xi_restart < 1 for restart.')
+            raise ValueError("You need a xi_restart < 1 for restart.")
 
         return True
 
     def is_restart(self, z_old, x_new, x_old):
         r"""Check whether the algorithm needs to restart.
 
         This method implements the checks necessary to tell whether the
@@ -206,20 +205,20 @@
 
         if self.restart_strategy is None:
             return False
 
         criterion = xp.vdot(z_old - x_new, x_new - x_old) >= 0
 
         if criterion:
-            if 'adaptive' in self.restart_strategy:
+            if "adaptive" in self.restart_strategy:
                 self.r_lazy *= self.xi_restart
-            if self.restart_strategy in {'adaptive-ii', 'adaptive-2'}:
+            if self.restart_strategy in {"adaptive-ii", "adaptive-2"}:
                 self._t_now = 1
 
-        if self.restart_strategy == 'greedy':
+        if self.restart_strategy == "greedy":
             cur_delta = xp.linalg.norm(x_new - x_old)
             if self._delta0 is None:
                 self._delta0 = self.s_greedy * cur_delta
             else:
                 self._safeguard = cur_delta >= self._delta0
 
         return criterion
@@ -265,25 +264,25 @@
             Current :math:`\lambda` value
 
         Notes
         -----
         Implements steps 3 and 4 from algoritm 10.7 in :cite:`bauschke2009`.
 
         """
-        if self.restart_strategy == 'greedy':
+        if self.restart_strategy == "greedy":
             return 2
 
         # Steps 3 and 4 from alg.10.7.
         self._t_prev = self._t_now
 
-        if self.mode == 'regular':
-            sqrt_part = self.r_lazy * self._t_prev ** 2 + self.q_lazy
+        if self.mode == "regular":
+            sqrt_part = self.r_lazy * self._t_prev**2 + self.q_lazy
             self._t_now = self.p_lazy + np.sqrt(sqrt_part) * 0.5
 
-        elif self.mode == 'CD':
+        elif self.mode == "CD":
             self._t_now = (self._n + self.a_cd - 1) / self.a_cd
             self._n += 1
 
         return 1 + (self._t_prev - 1) / self._t_now
 
 
 class ForwardBackward(SetUp):
@@ -340,26 +339,25 @@
     """
 
     def __init__(
         self,
         x,
         grad,
         prox,
-        cost='auto',
+        cost="auto",
         beta_param=1.0,
         lambda_param=1.0,
         beta_update=None,
-        lambda_update='fista',
+        lambda_update="fista",
         auto_iterate=True,
         metric_call_period=5,
         metrics=None,
         linear=None,
         **kwargs,
     ):
-
         # Set default algorithm properties
         super().__init__(
             metric_call_period=metric_call_period,
             metrics=metrics,
             **kwargs,
         )
 
@@ -372,23 +370,23 @@
         for operator in (grad, prox, cost):
             self._check_operator(operator)
 
         self._grad = grad
         self._prox = prox
         self._linear = linear
 
-        if cost == 'auto':
+        if cost == "auto":
             self._cost_func = costObj([self._grad, self._prox])
         else:
             self._cost_func = cost
 
         # Check if there is a linear op, needed for metrics in the FB algoritm
         if metrics and self._linear is None:
             raise ValueError(
-                'When using metrics, you must pass a linear operator',
+                "When using metrics, you must pass a linear operator",
             )
 
         if self._linear is None:
             self._linear = Identity()
 
         # Set the algorithm parameters
         for param_val in (beta_param, lambda_param):
@@ -396,15 +394,15 @@
 
         self._beta = self.step_size or beta_param
         self._lambda = lambda_param
 
         # Set the algorithm parameter update methods
         self._check_param_update(beta_update)
         self._beta_update = beta_update
-        if isinstance(lambda_update, str) and lambda_update == 'fista':
+        if isinstance(lambda_update, str) and lambda_update == "fista":
             fista = FISTA(**kwargs)
             self._lambda_update = fista.update_lambda
             self._is_restart = fista.is_restart
             self._beta_update = fista.update_beta
         else:
             self._check_param_update(lambda_update)
             self._lambda_update = lambda_update
@@ -458,17 +456,16 @@
         self._z_old = self.xp.copy(self._z_new)
 
         # Update parameter values for next iteration.
         self._update_param()
 
         # Test cost function for convergence.
         if self._cost_func:
-            self.converge = (
-                self.any_convergence_flag()
-                or self._cost_func.get_cost(self._x_new)
+            self.converge = self.any_convergence_flag() or self._cost_func.get_cost(
+                self._x_new
             )
 
     def iterate(self, max_iter=150, progbar=None):
         """Iterate.
 
         This method calls update until either the convergence criteria is met
         or the maximum number of iterations is reached.
@@ -496,28 +493,28 @@
         Returns
         -------
         dict
            The mapping between the iterated variables
 
         """
         return {
-            'x_new': self._linear.adj_op(self._x_new),
-            'z_new': self._z_new,
-            'idx': self.idx,
+            "x_new": self._linear.adj_op(self._x_new),
+            "z_new": self._z_new,
+            "idx": self.idx,
         }
 
     def retrieve_outputs(self):
         """Retireve outputs.
 
         Declare the outputs of the algorithms as attributes: ``x_final``,
         ``y_final``, ``metrics``.
 
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
 
 
 class GenForwardBackward(SetUp):
     r"""Generalized Forward-Backward Algorithm.
 
@@ -573,55 +570,54 @@
     """
 
     def __init__(
         self,
         x,
         grad,
         prox_list,
-        cost='auto',
+        cost="auto",
         gamma_param=1.0,
         lambda_param=1.0,
         gamma_update=None,
         lambda_update=None,
         weights=None,
         auto_iterate=True,
         metric_call_period=5,
         metrics=None,
         linear=None,
         **kwargs,
     ):
-
         # Set default algorithm properties
         super().__init__(
             metric_call_period=metric_call_period,
             metrics=metrics,
             **kwargs,
         )
 
         # Set the initial variable values
         self._check_input_data(x)
         self._x_old = self.xp.copy(x)
 
         # Set the algorithm operators
-        for operator in [grad, cost] + prox_list:
+        for operator in [grad, cost, *prox_list]:
             self._check_operator(operator)
 
         self._grad = grad
         self._prox_list = self.xp.array(prox_list)
         self._linear = linear
 
-        if cost == 'auto':
-            self._cost_func = costObj([self._grad] + prox_list)
+        if cost == "auto":
+            self._cost_func = costObj([self._grad, *prox_list])
         else:
             self._cost_func = cost
 
         # Check if there is a linear op, needed for metrics in the FB algoritm
         if metrics and self._linear is None:
             raise ValueError(
-                'When using metrics, you must pass a linear operator',
+                "When using metrics, you must pass a linear operator",
             )
 
         if self._linear is None:
             self._linear = Identity()
 
         # Set the algorithm parameters
         for param_val in (gamma_param, lambda_param):
@@ -637,17 +633,15 @@
         self._gamma_update = gamma_update
         self._lambda_update = lambda_update
 
         # Set the proximity weights
         self._set_weights(weights)
 
         # Set initial z
-        self._z = self.xp.array([
-            self._x_old for i in range(self._prox_list.size)
-        ])
+        self._z = self.xp.array([self._x_old for i in range(self._prox_list.size)])
 
         # Automatically run the algorithm
         if auto_iterate:
             self.iterate()
 
     def _set_weights(self, weights):
         """Set weights.
@@ -669,33 +663,33 @@
         """
         if isinstance(weights, type(None)):
             weights = self.xp.repeat(
                 1.0 / self._prox_list.size,
                 self._prox_list.size,
             )
         elif not isinstance(weights, (list, tuple, np.ndarray)):
-            raise TypeError('Weights must be provided as a list.')
+            raise TypeError("Weights must be provided as a list.")
 
         weights = self.xp.array(weights)
 
         if not np.issubdtype(weights.dtype, np.floating):
-            raise ValueError('Weights must be list of float values.')
+            raise ValueError("Weights must be list of float values.")
 
         if weights.size != self._prox_list.size:
             raise ValueError(
-                'The number of weights must match the number of proximity '
-                + 'operators.',
+                "The number of weights must match the number of proximity "
+                + "operators.",
             )
 
         expected_weight_sum = 1.0
 
         if self.xp.sum(weights) != expected_weight_sum:
             raise ValueError(
-                'Proximity operator weights must sum to 1.0. Current sum of '
-                + 'weights = {0}'.format(self.xp.sum(weights)),
+                "Proximity operator weights must sum to 1.0. Current sum of "
+                + f"weights = {self.xp.sum(weights)}",
             )
 
         self._weights = weights
 
     def _update_param(self):
         """Update parameters.
 
@@ -722,17 +716,15 @@
 
         """
         # Calculate gradient for current iteration.
         self._grad.get_grad(self._x_old)
 
         # Update z values.
         for i in range(self._prox_list.size):
-            z_temp = (
-                2 * self._x_old - self._z[i] - self._gamma * self._grad.grad
-            )
+            z_temp = 2 * self._x_old - self._z[i] - self._gamma * self._grad.grad
             z_prox = self._prox_list[i].op(
                 z_temp,
                 extra_factor=self._gamma / self._weights[i],
             )
             self._z[i] += self._lambda_param * (z_prox - self._x_old)
 
         # Update current reconstruction.
@@ -780,28 +772,28 @@
         Returns
         -------
         dict
            The mapping between the iterated variables
 
         """
         return {
-            'x_new': self._linear.adj_op(self._x_new),
-            'z_new': self._z,
-            'idx': self.idx,
+            "x_new": self._linear.adj_op(self._x_new),
+            "z_new": self._z,
+            "idx": self.idx,
         }
 
     def retrieve_outputs(self):
         """Retrieve outputs.
 
         Declare the outputs of the algorithms as attributes: ``x_final``,
         ``y_final``, ``metrics``.
 
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
 
 
 class POGM(SetUp):
     r"""Proximal Optimised Gradient Method.
 
@@ -867,24 +859,23 @@
         self,
         u,
         x,
         y,
         z,
         grad,
         prox,
-        cost='auto',
+        cost="auto",
         linear=None,
         beta_param=1.0,
         sigma_bar=1.0,
         auto_iterate=True,
         metric_call_period=5,
         metrics=None,
         **kwargs,
     ):
-
         # Set default algorithm properties
         super().__init__(
             metric_call_period=metric_call_period,
             metrics=metrics,
             linear=linear,
             **kwargs,
         )
@@ -901,28 +892,28 @@
         # Set the algorithm operators
         for operator in (grad, prox, cost):
             self._check_operator(operator)
 
         self._grad = grad
         self._prox = prox
         self._linear = linear
-        if cost == 'auto':
+        if cost == "auto":
             self._cost_func = costObj([self._grad, self._prox])
         else:
             self._cost_func = cost
 
         # If linear is None, make it Identity for call of metrics
         if self._linear is None:
             self._linear = Identity()
 
         # Set the algorithm parameters
         for param_val in (beta_param, sigma_bar):
             self._check_param(param_val)
         if sigma_bar < 0 or sigma_bar > 1:
-            raise ValueError('The sigma bar parameter needs to be in [0, 1]')
+            raise ValueError("The sigma bar parameter needs to be in [0, 1]")
 
         self._beta = self.step_size or beta_param
         self._sigma_bar = sigma_bar
         self._xi = 1.0
         self._sigma = 1.0
         self._t_old = 1.0
         self._grad.get_grad(self._x_old)
@@ -940,52 +931,50 @@
         Notes
         -----
         Implements algorithm 3 from :cite:`kim2017`.
 
         """
         # Step 4 from alg. 3
         self._grad.get_grad(self._x_old)
-        #self._u_new = self._x_old - self._beta * self._grad.grad
-        self._u_new =  -self._beta * self._grad.grad
+        # self._u_new = self._x_old - self._beta * self._grad.grad
+        self._u_new = -self._beta * self._grad.grad
         self._u_new += self._x_old
 
         # Step 5 from alg. 3
-        self._t_new = 0.5 * (1 + self.xp.sqrt(1 + 4 * self._t_old ** 2))
+        self._t_new = 0.5 * (1 + self.xp.sqrt(1 + 4 * self._t_old**2))
 
         # Step 6 from alg. 3
         t_shifted_ratio = (self._t_old - 1) / self._t_new
         sigma_t_ratio = self._sigma * self._t_old / self._t_new
         beta_xi_t_shifted_ratio = t_shifted_ratio * self._beta / self._xi
-        self._z = - beta_xi_t_shifted_ratio * (self._x_old - self._z)
+        self._z = -beta_xi_t_shifted_ratio * (self._x_old - self._z)
         self._z += self._u_new
         self._z += t_shifted_ratio * (self._u_new - self._u_old)
         self._z += sigma_t_ratio * (self._u_new - self._x_old)
 
         # Step 7 from alg. 3
         self._xi = self._beta * (1 + t_shifted_ratio + sigma_t_ratio)
 
         # Step 8 from alg. 3
         self._x_new = self._prox.op(self._z, extra_factor=self._xi)
 
         # Restarting and gamma-Decreasing
         # Step 9 from alg. 3
-        #self._g_new = self._grad.grad - (self._x_new - self._z) / self._xi
-        self._g_new = (self._z - self._x_new)
+        # self._g_new = self._grad.grad - (self._x_new - self._z) / self._xi
+        self._g_new = self._z - self._x_new
         self._g_new /= self._xi
         self._g_new += self._grad.grad
 
         # Step 10 from alg 3.
-        #self._y_new = self._x_old - self._beta * self._g_new
-        self._y_new = - self._beta * self._g_new
+        # self._y_new = self._x_old - self._beta * self._g_new
+        self._y_new = -self._beta * self._g_new
         self._y_new += self._x_old
 
         # Step 11 from alg. 3
-        restart_crit = (
-            self.xp.vdot(-self._g_new, self._y_new - self._y_old) < 0
-        )
+        restart_crit = self.xp.vdot(-self._g_new, self._y_new - self._y_old) < 0
         if restart_crit:
             self._t_new = 1
             self._sigma = 1
 
         # Step 13 from alg. 3
         elif self.xp.vdot(self._g_new, self._g_old) < 0:
             self._sigma *= self._sigma_bar
@@ -995,17 +984,16 @@
         self.xp.copyto(self._u_old, self._u_new)
         self.xp.copyto(self._x_old, self._x_new)
         self.xp.copyto(self._g_old, self._g_new)
         self.xp.copyto(self._y_old, self._y_new)
 
         # Test cost function for convergence.
         if self._cost_func:
-            self.converge = (
-                self.any_convergence_flag()
-                or self._cost_func.get_cost(self._x_new)
+            self.converge = self.any_convergence_flag() or self._cost_func.get_cost(
+                self._x_new
             )
 
     def iterate(self, max_iter=150, progbar=None):
         """Iterate.
 
         This method calls update until either convergence criteria is met or
         the maximum number of iterations is reached.
@@ -1033,28 +1021,28 @@
         Returns
         -------
         dict
            The mapping between the iterated variables
 
         """
         return {
-            'u_new': self._u_new,
-            'x_new': self._linear.adj_op(self._x_new),
-            'y_new': self._y_new,
-            'z_new': self._z,
-            'xi': self._xi,
-            'sigma': self._sigma,
-            't': self._t_new,
-            'idx': self.idx,
+            "u_new": self._u_new,
+            "x_new": self._linear.adj_op(self._x_new),
+            "y_new": self._y_new,
+            "z_new": self._z,
+            "xi": self._xi,
+            "sigma": self._sigma,
+            "t": self._t_new,
+            "idx": self.idx,
         }
 
     def retrieve_outputs(self):
         """Retrieve outputs.
 
         Declare the outputs of the algorithms as attributes: ``x_final``,
         ``y_final``, ``metrics``.
 
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
```

### Comparing `modopt-1.7.1/modopt/opt/algorithms/gradient_descent.py` & `modopt-1.7.2/src/modopt/opt/algorithms/gradient_descent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Gradient Descent Algorithms."""
 
 import numpy as np
 
 from modopt.opt.algorithms.base import SetUp
 from modopt.opt.cost import costObj
 
@@ -99,15 +98,15 @@
         self._speed_grad = np.zeros(x.shape, dtype=float)
         self._dir_grad = np.zeros_like(x)
         # Set the algorithm operators
         for operator in (grad, prox, cost):
             self._check_operator(operator)
         self._grad = grad
         self._prox = prox
-        if cost == 'auto':
+        if cost == "auto":
             self._cost_func = costObj([self._grad, self._prox])
         else:
             self._cost_func = cost
         # Set the algorithm parameters
         for param_val in (eta, epsilon):
             self._check_param(param_val)
         self._eta = eta
@@ -153,17 +152,16 @@
             self.reset()
             self._update_reg(step)
         self._x_old = self._x_new.copy()
         if self._eta_update is not None:
             self._eta = self._eta_update(self._eta, self.idx)
         # Test cost function for convergence.
         if self._cost_func:
-            self.converge = (
-                self.any_convergence_flag()
-                or self._cost_func.get_cost(self._x_new)
+            self.converge = self.any_convergence_flag() or self._cost_func.get_cost(
+                self._x_new
             )
 
     def _update_grad_dir(self, grad):
         """Update the gradient descent direction.
 
         Parameters
         ----------
@@ -204,29 +202,29 @@
         Returns
         -------
         dict
            The mapping between the iterated variables
 
         """
         return {
-            'x_new': self._x_new,
-            'dir_grad': self._dir_grad,
-            'speed_grad': self._speed_grad,
-            'idx': self.idx,
+            "x_new": self._x_new,
+            "dir_grad": self._dir_grad,
+            "speed_grad": self._speed_grad,
+            "idx": self.idx,
         }
 
     def retrieve_outputs(self):
         """Retrieve outputs.
 
         Declare the outputs of the algorithms as attributes: x_final,
         y_final, metrics.
 
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
 
     def reset(self):
         """Reset internal state of the algorithm."""
         pass
 
@@ -304,15 +302,15 @@
     GenericGradOpt : parent class
 
     """
 
     def __init__(self, *args, gamma=0.5, **kwargs):
         super().__init__(*args, **kwargs)
         if gamma < 0 or gamma > 1:
-            raise ValueError('gamma is outside of range [0,1]')
+            raise ValueError("gamma is outside of range [0,1]")
         self._check_param(gamma)
         self._gamma = gamma
 
     def _update_grad_speed(self, grad):
         """Rmsprop update speed.
 
         Parameters
@@ -401,17 +399,17 @@
     """
 
     def __init__(self, *args, gamma=0.9, beta=0.9, **kwargs):
         super().__init__(*args, **kwargs)
         self._check_param(gamma)
         self._check_param(beta)
         if gamma < 0 or gamma >= 1:
-            raise ValueError('gamma is outside of range [0,1]')
+            raise ValueError("gamma is outside of range [0,1]")
         if beta < 0 or beta >= 1:
-            raise ValueError('beta is outside of range [0,1]')
+            raise ValueError("beta is outside of range [0,1]")
         self._gamma = gamma
         self._beta = beta
         self._beta_pow = 1
         self._gamma_pow = 1
 
     def _update_grad_dir(self, grad):
         """ADAM Update of gradient direction."""
```

### Comparing `modopt-1.7.1/modopt/opt/algorithms/primal_dual.py` & `modopt-1.7.2/src/modopt/opt/algorithms/primal_dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Primal-Dual Algorithms."""
 
 from modopt.opt.algorithms.base import SetUp
 from modopt.opt.cost import costObj
 from modopt.opt.linear import Identity
 
 
@@ -77,30 +76,29 @@
         self,
         x,
         y,
         grad,
         prox,
         prox_dual,
         linear=None,
-        cost='auto',
+        cost="auto",
         reweight=None,
         rho=0.5,
         sigma=1.0,
         tau=1.0,
         rho_update=None,
         sigma_update=None,
         tau_update=None,
         auto_iterate=True,
         max_iter=150,
         n_rewightings=1,
         metric_call_period=5,
         metrics=None,
         **kwargs,
     ):
-
         # Set default algorithm properties
         super().__init__(
             metric_call_period=metric_call_period,
             metrics=metrics,
             **kwargs,
         )
 
@@ -119,20 +117,22 @@
         self._prox = prox
         self._prox_dual = prox_dual
         self._reweight = reweight
         if isinstance(linear, type(None)):
             self._linear = Identity()
         else:
             self._linear = linear
-        if cost == 'auto':
-            self._cost_func = costObj([
-                self._grad,
-                self._prox,
-                self._prox_dual,
-            ])
+        if cost == "auto":
+            self._cost_func = costObj(
+                [
+                    self._grad,
+                    self._prox,
+                    self._prox_dual,
+                ]
+            )
         else:
             self._cost_func = cost
 
         # Set the algorithm parameters
         for param_val in (rho, sigma, tau):
             self._check_param(param_val)
 
@@ -183,30 +183,25 @@
         - Primal proximity operator set up for positivity constraint.
 
         """
         # Step 1 from eq.9.
         self._grad.get_grad(self._x_old)
 
         x_prox = self._prox.op(
-            self._x_old - self._tau * self._grad.grad - self._tau
-            * self._linear.adj_op(self._y_old),
+            self._x_old
+            - self._tau * self._grad.grad
+            - self._tau * self._linear.adj_op(self._y_old),
         )
 
         # Step 2 from eq.9.
-        y_temp = (
-            self._y_old + self._sigma
-            * self._linear.op(2 * x_prox - self._x_old)
-        )
+        y_temp = self._y_old + self._sigma * self._linear.op(2 * x_prox - self._x_old)
 
-        y_prox = (
-            y_temp - self._sigma
-            * self._prox_dual.op(
-                y_temp / self._sigma,
-                extra_factor=(1.0 / self._sigma),
-            )
+        y_prox = y_temp - self._sigma * self._prox_dual.op(
+            y_temp / self._sigma,
+            extra_factor=(1.0 / self._sigma),
         )
 
         # Step 3 from eq.9.
         self._x_new = self._rho * x_prox + (1 - self._rho) * self._x_old
         self._y_new = self._rho * y_prox + (1 - self._rho) * self._y_old
 
         del x_prox, y_prox, y_temp
@@ -216,17 +211,16 @@
         self.xp.copyto(self._y_old, self._y_new)
 
         # Update parameter values for next iteration.
         self._update_param()
 
         # Test cost function for convergence.
         if self._cost_func:
-            self.converge = (
-                self.any_convergence_flag()
-                or self._cost_func.get_cost(self._x_new, self._y_new)
+            self.converge = self.any_convergence_flag() or self._cost_func.get_cost(
+                self._x_new, self._y_new
             )
 
     def iterate(self, max_iter=150, n_rewightings=1, progbar=None):
         """Iterate.
 
         This method calls update until either convergence criteria is met or
         the maximum number of iterations is reached.
@@ -263,20 +257,20 @@
 
         Returns
         -------
         notify_observers_kwargs : dict,
            The mapping between the iterated variables
 
         """
-        return {'x_new': self._x_new, 'y_new': self._y_new, 'idx': self.idx}
+        return {"x_new": self._x_new, "y_new": self._y_new, "idx": self.idx}
 
     def retrieve_outputs(self):
         """Retrieve outputs.
 
         Declare the outputs of the algorithms as attributes: ``x_final``,
         ``y_final``, ``metrics``.
 
         """
         metrics = {}
-        for obs in self._observers['cv_metrics']:
+        for obs in self._observers["cv_metrics"]:
             metrics[obs.name] = obs.retrieve_metrics()
         self.metrics = metrics
```

### Comparing `modopt-1.7.1/modopt/opt/cost.py` & `modopt-1.7.2/src/modopt/opt/cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         initial_cost=1e6,
         tolerance=1e-4,
         cost_interval=1,
         test_range=4,
         verbose=True,
         plot_output=None,
     ):
-
         self.cost = initial_cost
         self._cost_list = []
         self._cost_interval = cost_interval
         self._iteration = 1
         self._test_list = []
         self._test_range = test_range
         self._tolerance = tolerance
@@ -108,38 +107,37 @@
         # Add current cost value to the test list
         self._test_list.append(self.cost)
 
         xp = get_array_module(self.cost)
 
         # Check if enough cost values have been collected
         if len(self._test_list) == self._test_range:
-
             # The mean of the first half of the test list
             t1 = xp.mean(
-                xp.array(self._test_list[len(self._test_list) // 2:]),
+                xp.array(self._test_list[len(self._test_list) // 2 :]),
                 axis=0,
             )
             # The mean of the second half of the test list
             t2 = xp.mean(
-                xp.array(self._test_list[:len(self._test_list) // 2]),
+                xp.array(self._test_list[: len(self._test_list) // 2]),
                 axis=0,
             )
             # Calculate the change across the test list
             if xp.around(t1, decimals=16):
-                cost_diff = (xp.linalg.norm(t1 - t2) / xp.linalg.norm(t1))
+                cost_diff = xp.linalg.norm(t1 - t2) / xp.linalg.norm(t1)
             else:
                 cost_diff = 0
 
             # Reset the test list
             self._test_list = []
 
             if self._verbose:
-                print(' - CONVERGENCE TEST - ')
-                print(' - CHANGE IN COST:', cost_diff)
-                print('')
+                print(" - CONVERGENCE TEST - ")
+                print(" - CHANGE IN COST:", cost_diff)
+                print("")
 
             # Check for convergence
             return cost_diff <= self._tolerance
 
         return False
 
     @abc.abstractmethod
@@ -172,32 +170,31 @@
         -------
         bool
             Result of the convergence test
 
         """
         # Check if the cost should be calculated
         test_conditions = (
-            self._cost_interval is None
-            or self._iteration % self._cost_interval
+            self._cost_interval is None or self._iteration % self._cost_interval
         )
 
         if test_conditions:
             test_result = False
 
         else:
             if self._verbose:
-                print(' - ITERATION:', self._iteration)
+                print(" - ITERATION:", self._iteration)
 
             # Calculate the current cost
-            self.cost = self._calc_cost(verbose=self._verbose, *args, **kwargs)
+            self.cost = self._calc_cost(*args, verbose=self._verbose, **kwargs)
             self._cost_list.append(self.cost)
 
             if self._verbose:
-                print(' - COST:', self.cost)
-                print('')
+                print(" - COST:", self.cost)
+                print("")
 
             # Test for convergence
             test_result = self._check_cost()
 
         # Update the current iteration number
         self._iteration += 1
 
@@ -284,21 +281,19 @@
         TypeError
             For invalid operators type
         ValueError
             For operators without ``cost`` method
 
         """
         if not isinstance(self._operators, (list, tuple, np.ndarray)):
-            message = (
-                'Input operators must be provided as a list, not {0}'
-            )
+            message = "Input operators must be provided as a list, not {0}"
             raise TypeError(message.format(type(self._operators)))
 
         for op in self._operators:
-            if not hasattr(op, 'cost'):
+            if not hasattr(op, "cost"):
                 raise ValueError('Operators must contain "cost" method.')
             op.cost = check_callable(op.cost)
 
     def _calc_cost(self, *args, **kwargs):
         """Calculate the cost.
 
         This method calculates the cost from each of the input operators.
```

### Comparing `modopt-1.7.1/modopt/opt/gradient.py` & `modopt-1.7.2/src/modopt/opt/gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# -*- coding: utf-8 -*-
-
 """GRADIENT CLASSES.
 
 This module contains classses for defining algorithm gradients.
 Based on work by Yinghao Ge and Fred Ngole.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
 
 import numpy as np
 
 from modopt.base.types import check_callable, check_float, check_npndarray
 
 
-class GradParent(object):
+class GradParent:
     """Gradient Parent Class.
 
     This class defines the basic methods that will be inherited by specific
     gradient classes.
 
     Parameters
     ----------
@@ -67,15 +65,14 @@
         trans_op,
         get_grad=None,
         cost=None,
         data_type=None,
         input_data_writeable=False,
         verbose=True,
     ):
-
         self.verbose = verbose
         self._input_data_writeable = input_data_writeable
         self._grad_data_type = data_type
         self.obs_data = input_data
         self.op = op
         self.trans_op = trans_op
 
@@ -96,15 +93,14 @@
             The observed data
 
         """
         return self._obs_data
 
     @obs_data.setter
     def obs_data(self, input_data):
-
         if self._grad_data_type in {float, np.floating}:
             input_data = check_float(input_data)
         check_npndarray(
             input_data,
             dtype=self._grad_data_type,
             writeable=self._input_data_writeable,
             verbose=self.verbose,
@@ -124,15 +120,14 @@
             The operator function
 
         """
         return self._op
 
     @op.setter
     def op(self, operator):
-
         self._op = check_callable(operator)
 
     @property
     def trans_op(self):
         r"""Transpose operator.
 
         The transpose operator :math:`\mathbf{H}^T`.
@@ -143,47 +138,43 @@
             The transpose operator function
 
         """
         return self._trans_op
 
     @trans_op.setter
     def trans_op(self, operator):
-
         self._trans_op = check_callable(operator)
 
     @property
     def get_grad(self):
         """Get gradient value."""
         return self._get_grad
 
     @get_grad.setter
     def get_grad(self, method):
-
         self._get_grad = check_callable(method)
 
     @property
     def grad(self):
         """Gradient value."""
         return self._grad
 
     @grad.setter
     def grad(self, input_value):
-
         if self._grad_data_type in {float, np.floating}:
             input_value = check_float(input_value)
         self._grad = input_value
 
     @property
     def cost(self):
         """Cost contribution."""
         return self._cost
 
     @cost.setter
     def cost(self, method):
-
         self._cost = check_callable(method)
 
     def trans_op_op(self, input_data):
         r"""Transpose Operation of the Operator.
 
         This method calculates the action of the transpose operator on
         the action of the operator on the data.
@@ -239,15 +230,14 @@
     See Also
     --------
     GradParent : parent class
 
     """
 
     def __init__(self, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
         self.get_grad = self._get_grad_method
         self.cost = self._cost_method
 
     def _get_grad_method(self, input_data):
         r"""Get the gradient.
 
@@ -285,11 +275,11 @@
         -------
         float
             Gradient cost component
 
         """
         cost_val = 0.5 * np.linalg.norm(self.obs_data - self.op(args[0])) ** 2
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - DATA FIDELITY (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - DATA FIDELITY (X):", cost_val)
 
         return cost_val
```

### Comparing `modopt-1.7.1/modopt/opt/linear/base.py` & `modopt-1.7.2/src/modopt/opt/linear/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Base classes for linear operators."""
 
 import numpy as np
 
 from modopt.base.types import check_callable
 from modopt.base.backend import get_array_module
 
-class LinearParent(object):
+
+class LinearParent:
     """Linear Operator Parent Class.
 
     This class sets the structure for defining linear operator instances.
 
     Parameters
     ----------
     op : callable
@@ -25,36 +26,33 @@
     4
     >>> a.adj_op(2)
     8
 
     """
 
     def __init__(self, op, adj_op):
-
         self.op = op
         self.adj_op = adj_op
 
     @property
     def op(self):
         """Linear Operator."""
         return self._op
 
     @op.setter
     def op(self, operator):
-
         self._op = check_callable(operator)
 
     @property
     def adj_op(self):
         """Linear Adjoint Operator."""
         return self._adj_op
 
     @adj_op.setter
     def adj_op(self, operator):
-
         self._adj_op = check_callable(operator)
 
 
 class Identity(LinearParent):
     """Identity Operator Class.
 
     This is a dummy class that can be used in the optimisation classes.
@@ -62,18 +60,17 @@
     See Also
     --------
     LinearParent : parent class
 
     """
 
     def __init__(self):
-
         self.op = lambda input_data: input_data
         self.adj_op = self.op
-        self.cost= lambda *args, **kwargs: 0
+        self.cost = lambda *args, **kwargs: 0
 
 
 class MatrixOperator(LinearParent):
     """
     Matrix Operator class.
 
     This class transforms an array into a suitable linear operator.
@@ -122,15 +119,14 @@
 
     See Also
     --------
     LinearParent : parent class
     """
 
     def __init__(self, operators, weights=None):
-
         operators, weights = self._check_inputs(operators, weights)
         self.operators = operators
         self.weights = weights
         self.op = self._op_method
         self.adj_op = self._adj_op_method
 
     def _check_type(self, input_val):
@@ -155,22 +151,21 @@
             For invalid input type
         ValueError
             If input list is empty
 
         """
         if not isinstance(input_val, (list, tuple, np.ndarray)):
             raise TypeError(
-                'Invalid input type, input must be a list, tuple or numpy '
-                + 'array.',
+                "Invalid input type, input must be a list, tuple or numpy " + "array.",
             )
 
         input_val = np.array(input_val)
 
         if not input_val.size:
-            raise ValueError('Input list is empty.')
+            raise ValueError("Input list is empty.")
 
         return input_val
 
     def _check_inputs(self, operators, weights):
         """Check inputs.
 
         This method cheks that the input operators and weights are correctly
@@ -195,35 +190,33 @@
         TypeError
             If the individual weight values are not floats
 
         """
         operators = self._check_type(operators)
 
         for operator in operators:
-
-            if not hasattr(operator, 'op'):
+            if not hasattr(operator, "op"):
                 raise ValueError('Operators must contain "op" method.')
 
-            if not hasattr(operator, 'adj_op'):
+            if not hasattr(operator, "adj_op"):
                 raise ValueError('Operators must contain "adj_op" method.')
 
             operator.op = check_callable(operator.op)
             operator.adj_op = check_callable(operator.adj_op)
 
         if not isinstance(weights, type(None)):
             weights = self._check_type(weights)
 
             if weights.size != operators.size:
                 raise ValueError(
-                    'The number of weights must match the number of '
-                    + 'operators.',
+                    "The number of weights must match the number of " + "operators.",
                 )
 
             if not np.issubdtype(weights.dtype, np.floating):
-                raise TypeError('The weights must be a list of float values.')
+                raise TypeError("The weights must be a list of float values.")
 
         return operators, weights
 
     def _op_method(self, input_data):
         """Operator.
 
         This method returns the input data operated on by all of the operators.
```

### Comparing `modopt-1.7.1/modopt/opt/proximity.py` & `modopt-1.7.2/src/modopt/opt/proximity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """PROXIMITY OPERATORS.
 
 This module contains classes of proximity operators for optimisation.
 
 :Authors:
 
 * Samuel Farrens <samuel.farrens@cea.fr>,
@@ -18,24 +16,25 @@
 try:
     from sklearn.isotonic import isotonic_regression
 except ImportError:
     import_sklearn = False
 else:
     import_sklearn = True
 
+from modopt.base.backend import get_array_module
 from modopt.base.transform import cube2matrix, matrix2cube
 from modopt.base.types import check_callable
 from modopt.interface.errors import warn
 from modopt.math.matrix import nuclear_norm
 from modopt.signal.noise import thresh
 from modopt.signal.positivity import positive
 from modopt.signal.svd import svd_thresh, svd_thresh_coef, svd_thresh_coef_fast
 
 
-class ProximityParent(object):
+class ProximityParent:
     """Proximity Operator Parent Class.
 
     This class sets the structure for defining proximity operator instances.
 
     Parameters
     ----------
     op : callable
@@ -43,26 +42,24 @@
     cost : callable
         Callable function that implements the proximity contribution to the
         cost
 
     """
 
     def __init__(self, op, cost):
-
         self.op = op
         self.cost = cost
 
     @property
     def op(self):
         """Linear operator."""
         return self._op
 
     @op.setter
     def op(self, operator):
-
         self._op = check_callable(operator)
 
     @property
     def cost(self):
         """Cost contribution.
 
         This method defines the proximity operator's contribution to the total
@@ -74,15 +71,14 @@
             Cost contribution value
 
         """
         return self._cost
 
     @cost.setter
     def cost(self, method):
-
         self._cost = check_callable(method)
 
 
 class IdentityProx(ProximityParent):
     """Identity Proxmity Operator.
 
     This is a dummy class that can be used as a proximity operator.
@@ -94,17 +90,16 @@
     See Also
     --------
     ProximityParent : parent class
 
     """
 
     def __init__(self):
-
-        self.op = lambda x_val: x_val
-        self.cost = lambda x_val: 0
+        self.op = lambda x_val, *args, **kwargs: x_val
+        self.cost = lambda x_val, *args, **kwargs: 0
 
 
 class Positivity(ProximityParent):
     """Positivity Proximity Operator.
 
     This class defines the positivity proximity operator.
 
@@ -112,18 +107,33 @@
     --------
     ProximityParent : parent class
     modopt.signal.positivity.positive : positivity operator
 
     """
 
     def __init__(self):
-
-        self.op = lambda input_data: positive(input_data)
         self.cost = self._cost_method
 
+    def op(self, input_data, *args, **kwargs):
+        """
+        Make the data positive.
+
+        Parameters
+        ----------
+        input_data: np.ndarray
+            Input array
+        *args, **kwargs: dummy.
+
+        Returns
+        -------
+        np.ndarray
+            Positive data.
+        """
+        return positive(input_data)
+
     def _cost_method(self, *args, **kwargs):
         """Calculate positivity component of the cost.
 
         This method returns ``0`` as the posivituty does not contribute to the
         cost.
 
         Parameters
@@ -135,16 +145,16 @@
 
         Returns
         -------
         float
             ``0.0``
 
         """
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - Min (X):', np.min(args[0]))
+        if kwargs.get("verbose"):
+            print(" - Min (X):", np.min(args[0]))
 
         return 0
 
 
 class SparseThreshold(ProximityParent):
     """Sparse Threshold Proximity Operator.
 
@@ -162,16 +172,15 @@
     See Also
     --------
     ProximityParent : parent class
     modopt.signal.noise.thresh : thresholding function
 
     """
 
-    def __init__(self, linear, weights, thresh_type='soft'):
-
+    def __init__(self, linear, weights, thresh_type="soft"):
         self._linear = linear
         self.weights = weights
         self._thresh_type = thresh_type
         self.op = self._op_method
         self.cost = self._cost_method
 
     def _op_method(self, input_data, extra_factor=1.0):
@@ -211,18 +220,21 @@
 
         Returns
         -------
         float
             Sparsity cost component
 
         """
-        cost_val = np.sum(np.abs(self.weights * self._linear.op(args[0])))
+        xp = get_array_module(args[0])
+        cost_val = xp.sum(xp.abs(self.weights * self._linear.op(args[0])))
+        if isinstance(cost_val, xp.ndarray):
+            cost_val = cost_val.item()
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - L1 NORM (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - L1 NORM (X):", cost_val)
 
         return cost_val
 
 
 class LowRankMatrix(ProximityParent):
     """Low-rank Proximity Operator.
 
@@ -265,20 +277,19 @@
     modopt.math.matrix.nuclear_norm : nuclear norm implementation
 
     """
 
     def __init__(
         self,
         threshold,
-        thresh_type='soft',
-        lowr_type='standard',
+        thresh_type="soft",
+        lowr_type="standard",
         initial_rank=None,
         operator=None,
     ):
-
         self.thresh = threshold
         self.thresh_type = thresh_type
         self.lowr_type = lowr_type
         self.operator = operator
         self.op = self._op_method
         self.cost = self._cost_method
         self.rank = initial_rank
@@ -307,39 +318,39 @@
         Raises
         ------
         ValueError
             if lowr_type is not in ``{'standard', 'ngole'}``
         """
         # Update threshold with extra factor.
         threshold = self.thresh * extra_factor
-        if self.lowr_type == 'standard' and self.rank is None and rank is None:
+        if self.lowr_type == "standard" and self.rank is None and rank is None:
             data_matrix = svd_thresh(
                 cube2matrix(input_data),
                 threshold,
                 thresh_type=self.thresh_type,
             )
-        elif self.lowr_type == 'standard':
+        elif self.lowr_type == "standard":
             data_matrix, update_rank = svd_thresh_coef_fast(
                 cube2matrix(input_data),
                 threshold,
                 n_vals=rank or self.rank,
                 extra_vals=5,
                 thresh_type=self.thresh_type,
             )
             self.rank = update_rank  # save for future use
 
-        elif self.lowr_type == 'ngole':
+        elif self.lowr_type == "ngole":
             data_matrix = svd_thresh_coef(
                 cube2matrix(input_data),
                 self.operator,
                 threshold,
                 thresh_type=self.thresh_type,
             )
         else:
-            raise ValueError('lowr_type should be standard or ngole')
+            raise ValueError("lowr_type should be standard or ngole")
 
         # Return updated data.
         return matrix2cube(data_matrix, input_data.shape[1:])
 
     def _cost_method(self, *args, **kwargs):
         """Calculate low-rank component of the cost.
 
@@ -357,16 +368,16 @@
         -------
         float
             Low-rank cost component
 
         """
         cost_val = self.thresh * nuclear_norm(cube2matrix(args[0]))
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - NUCLEAR NORM (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - NUCLEAR NORM (X):", cost_val)
 
         return cost_val
 
 
 class LinearCompositionProx(ProximityParent):
     """Proximity Operator of a Linear Composition.
 
@@ -462,15 +473,14 @@
     See Also
     --------
     ProximityParent : parent class
 
     """
 
     def __init__(self, operators):
-
         operators = self._check_operators(operators)
         self.operators = operators
         self.op = self._op_method
         self.cost = self._cost_method
 
     def _check_operators(self, operators):
         """Check operators.
@@ -498,27 +508,27 @@
             For missing op method
         ValueError
             For missing cost method
 
         """
         if not isinstance(operators, (list, tuple, np.ndarray)):
             raise TypeError(
-                'Invalid input type, operators must be a list, tuple or '
-                + 'numpy array.',
+                "Invalid input type, operators must be a list, tuple or "
+                + "numpy array.",
             )
 
         operators = np.array(operators)
 
         if not operators.size:
-            raise ValueError('Operator list is empty.')
+            raise ValueError("Operator list is empty.")
 
         for operator in operators:
-            if not hasattr(operator, 'op'):
+            if not hasattr(operator, "op"):
                 raise ValueError('Operators must contain "op" method.')
-            if not hasattr(operator, 'cost'):
+            if not hasattr(operator, "cost"):
                 raise ValueError('Operators must contain "cost" method.')
             operator.op = check_callable(operator.op)
             operator.cost = check_callable(operator.cost)
 
         return operators
 
     def _op_method(self, input_data, extra_factor=1.0):
@@ -565,18 +575,20 @@
 
         Returns
         -------
         float
             Combinded cost components
 
         """
-        return np.sum([
-            operator.cost(input_data)
-            for operator, input_data in zip(self.operators, args[0])
-        ])
+        return np.sum(
+            [
+                operator.cost(input_data)
+                for operator, input_data in zip(self.operators, args[0])
+            ]
+        )
 
 
 class OrderedWeightedL1Norm(ProximityParent):
     """Ordered Weighted L1 norm proximity operator.
 
     This class defines the OWL proximity operator described in
     :cite:`figueiredo2014`.
@@ -609,24 +621,24 @@
     sklearn.isotonic.isotonic_regression : isotonic regression implementation
 
     """
 
     def __init__(self, weights):
         if not import_sklearn:  # pragma: no cover
             raise ImportError(
-                'Required version of Scikit-Learn package not found see '
-                + 'documentation for details: '
-                + 'https://cea-cosmic.github.io/ModOpt/#optional-packages',
+                "Required version of Scikit-Learn package not found see "
+                + "documentation for details: "
+                + "https://cea-cosmic.github.io/ModOpt/#optional-packages",
             )
         if np.max(np.diff(weights)) > 0:
-            raise ValueError('Weights must be non increasing')
+            raise ValueError("Weights must be non increasing")
         self.weights = weights.flatten()
         if (self.weights < 0).any():
             raise ValueError(
-                'The weight values must be provided in descending order',
+                "The weight values must be provided in descending order",
             )
         self.op = self._op_method
         self.cost = self._cost_method
 
     def _op_method(self, input_data, extra_factor=1.0):
         """Operator.
 
@@ -656,23 +668,25 @@
         data_abs = np.abs(data_squeezed)
         data_abs_sort_idx = np.argsort(data_abs)[::-1]
         data_abs = data_abs[data_abs_sort_idx]
 
         # Projection onto the monotone non-negative cone using
         # isotonic_regression
         data_abs = isotonic_regression(
-            data_abs - threshold, y_min=0, increasing=False,
+            data_abs - threshold,
+            y_min=0,
+            increasing=False,
         )
 
         # Unsorting the data
         data_abs_unsorted = np.empty_like(data_abs)
         data_abs_unsorted[data_abs_sort_idx] = data_abs
 
         # Putting the sign back
-        with np.errstate(invalid='ignore'):
+        with np.errstate(invalid="ignore"):
             sign_data = data_squeezed / np.abs(data_squeezed)
 
         # Removing NAN caused by the sign
         sign_data[np.isnan(sign_data)] = 0
 
         return np.reshape(sign_data * data_abs_unsorted, input_data.shape)
 
@@ -694,16 +708,16 @@
             OWL cost component
 
         """
         cost_val = np.sum(
             self.weights * np.sort(np.squeeze(np.abs(args[0]))[::-1]),
         )
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - OWL NORM (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - OWL NORM (X):", cost_val)
 
         return cost_val
 
 
 class Ridge(ProximityParent):
     r"""L2-norm Proximity Operator (`i.e.` Shrinkage).
 
@@ -726,16 +740,15 @@
 
     See Also
     --------
     ProximityParent : parent class
 
     """
 
-    def __init__(self, linear, weights, thresh_type='soft'):
-
+    def __init__(self, linear, weights, thresh_type="soft"):
         self._linear = linear
         self.weights = weights
         self.op = self._op_method
         self.cost = self._cost_method
 
     def _op_method(self, input_data, extra_factor=1.0):
         """Operator Method.
@@ -778,16 +791,16 @@
             Sparsity cost component
 
         """
         cost_val = np.sum(
             np.abs(self.weights * self._linear.op(args[0]) ** 2),
         )
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - L2 NORM (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - L2 NORM (X):", cost_val)
 
         return cost_val
 
 
 class ElasticNet(ProximityParent):
     r"""Elastic Net.
 
@@ -814,15 +827,14 @@
     --------
     ProximityParent : parent class
     modopt.signal.noise.thresh : thresholding function
 
     """
 
     def __init__(self, linear, alpha, beta):
-
         self._linear = linear
         self.alpha = alpha
         self.beta = beta
         self.op = self._op_method
         self.cost = self._cost_method
 
     def _op_method(self, input_data, extra_factor=1.0):
@@ -840,16 +852,16 @@
         Returns
         -------
         numpy.ndarray
             Thresholded data
 
         """
         soft_threshold = self.beta * extra_factor
-        normalization = (self.alpha * 2 * extra_factor + 1)
-        return thresh(input_data, soft_threshold, 'soft') / normalization
+        normalization = self.alpha * 2 * extra_factor + 1
+        return thresh(input_data, soft_threshold, "soft") / normalization
 
     def _cost_method(self, *args, **kwargs):
         """Calculate Ridge component of the cost.
 
         This method returns the l2 norm error of the weighted wavelet
         coefficients.
 
@@ -867,16 +879,16 @@
 
         """
         cost_val = np.sum(
             np.abs(self.alpha * self._linear.op(args[0]) ** 2)
             + np.abs(self.beta * self._linear.op(args[0])),
         )
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - ELASTIC NET (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - ELASTIC NET (X):", cost_val)
 
         return cost_val
 
 
 class KSupportNorm(ProximityParent):
     """K-support Norm Proximity Operator.
 
@@ -934,15 +946,15 @@
         """Get the :math:`k` value."""
         return self._k_value
 
     @k_value.setter
     def k_value(self, k_val):
         if k_val < 1:
             raise ValueError(
-                'The k parameter should be greater or equal than 1',
+                "The k parameter should be greater or equal than 1",
             )
         self._k_value = k_val
 
     def _compute_theta(self, input_data, alpha, extra_factor=1.0):
         r"""Compute theta.
 
         This method computes theta from Corollary 16:
@@ -979,15 +991,15 @@
             np.expand_dims(alpha, -1),
             np.expand_dims(np.abs(input_data), -1).T,
         )
         theta = np.zeros(alpha_input.shape)
         alpha_beta = alpha_input - self.beta * extra_factor
         theta = alpha_beta * ((alpha_beta <= 1) & (alpha_beta >= 0))
         theta = np.nan_to_num(theta)
-        theta += (alpha_input > (self.beta * extra_factor + 1))
+        theta += alpha_input > (self.beta * extra_factor + 1)
         return theta
 
     def _interpolate(self, alpha0, alpha1, sum0, sum1):
         r"""Linear interpolation of alpha (:math:`\alpha`).
 
         This method estimats :math:`\alpha^*` such that
         :math:`\sum\theta(\alpha^*)=k` via a linear interpolation.
@@ -1070,37 +1082,35 @@
             found = True
 
         if sum0 >= self._k_value:
             found = True
             midpoint = 0
 
         while (first_idx <= last_idx) and not found and (cnt < alpha.shape[0]):
-
             midpoint = (first_idx + last_idx) // 2
             cnt += 1
 
             if prev_midpoint == midpoint:
-
                 # Particular case
                 sum0 = self._compute_theta(
                     data_abs,
                     alpha[first_idx],
                     extra_factor,
                 ).sum()
                 sum1 = self._compute_theta(
                     data_abs,
                     alpha[last_idx],
                     extra_factor,
                 ).sum()
 
-                if (np.abs(sum0 - self._k_value) <= tolerance):
+                if np.abs(sum0 - self._k_value) <= tolerance:
                     found = True
                     midpoint = first_idx
 
-                if (np.abs(sum1 - self._k_value) <= tolerance):
+                if np.abs(sum1 - self._k_value) <= tolerance:
                     found = True
                     midpoint = last_idx - 1
                     # -1 because output is index such that
                     # `sum(theta(alpha[index])) <= k`
 
                 if (first_idx - last_idx) in {1, 2}:
                     sum0 = self._compute_theta(
@@ -1137,21 +1147,25 @@
             elif sum0 > self._k_value:
                 last_idx = midpoint
 
             prev_midpoint = midpoint
 
         if found:
             return (
-                midpoint, alpha[midpoint], alpha[midpoint + 1], sum0, sum1,
+                midpoint,
+                alpha[midpoint],
+                alpha[midpoint + 1],
+                sum0,
+                sum1,
             )
 
         raise ValueError(
-            'Cannot find the coordinate of alpha (i) such '
-            + 'that sum(theta(alpha[i])) =< k and '
-            + 'sum(theta(alpha[i+1])) >= k ',
+            "Cannot find the coordinate of alpha (i) such "
+            + "that sum(theta(alpha[i])) =< k and "
+            + "sum(theta(alpha[i+1])) >= k ",
         )
 
     def _find_alpha(self, input_data, extra_factor=1.0):
         """Find alpha value to compute theta.
 
         This method aim at finding alpha such that sum(theta(alpha)) = k.
 
@@ -1167,23 +1181,21 @@
         float
             An interpolation of alpha such that sum(theta(alpha)) = k
 
         """
         data_size = input_data.shape[0]
 
         # Computes the alpha^i points line 1 in Algorithm 1.
-        alpha = np.zeros((data_size * 2))
+        alpha = np.zeros(data_size * 2)
         data_abs = np.abs(input_data)
-        alpha[:data_size] = (
-            (self.beta * extra_factor)
-            / (data_abs + sys.float_info.epsilon)
+        alpha[:data_size] = (self.beta * extra_factor) / (
+            data_abs + sys.float_info.epsilon
         )
-        alpha[data_size:] = (
-            (self.beta * extra_factor + 1)
-            / (data_abs + sys.float_info.epsilon)
+        alpha[data_size:] = (self.beta * extra_factor + 1) / (
+            data_abs + sys.float_info.epsilon
         )
         alpha = np.sort(np.unique(alpha))
 
         # Identify points alpha^i and alpha^{i+1} line 2. Algorithm 1
         _, *alpha_sum = self._binary_search(
             input_data,
             alpha,
@@ -1212,29 +1224,28 @@
             Proximal map
 
         """
         data_shape = input_data.shape
         k_max = np.prod(data_shape)
         if self._k_value > k_max:
             warn(
-                'K value of the K-support norm is greater than the input '
-                + 'dimension, its value will be set to {0}'.format(k_max),
+                "K value of the K-support norm is greater than the input "
+                + f"dimension, its value will be set to {k_max}",
             )
             self._k_value = k_max
 
         # Computes line 1., 2. and 3. in Algorithm 1
         alpha = self._find_alpha(np.abs(input_data.flatten()), extra_factor)
 
         # Computes line 4. in Algorithm 1
         theta = self._compute_theta(np.abs(input_data.flatten()), alpha)
 
         # Computes line 5. in Algorithm 1.
         rslt = np.nan_to_num(
-            (input_data.flatten() * theta)
-            / (theta + self.beta * extra_factor),
+            (input_data.flatten() * theta) / (theta + self.beta * extra_factor),
         )
         return rslt.reshape(data_shape)
 
     def _find_q(self, sorted_data):
         r"""Find :math:`q`.
 
         Find the :math:`q` index value.
@@ -1267,33 +1278,28 @@
         cnt = 0
 
         # Particular case
         if (sorted_data.sum() / (self._k_value)) >= sorted_data[0]:
             found = True
             q_val = 0
 
-        elif (
-            (sorted_data[self._k_value - 1:].sum())
-            <= sorted_data[self._k_value - 1]
-        ):
+        elif (sorted_data[self._k_value - 1 :].sum()) <= sorted_data[self._k_value - 1]:
             found = True
             q_val = self._k_value - 1
 
         while (
-            not found and not cnt == self._k_value
+            not found
+            and not cnt == self._k_value
             and (first_idx <= last_idx < self._k_value)
         ):
-
             q_val = (first_idx + last_idx) // 2
             cnt += 1
             l1_part = sorted_data[q_val:].sum() / (self._k_value - q_val)
 
-            if (
-                sorted_data[q_val + 1] <= l1_part <= sorted_data[q_val]
-            ):
+            if sorted_data[q_val + 1] <= l1_part <= sorted_data[q_val]:
                 found = True
 
             else:
                 if sorted_data[q_val] <= l1_part:
                     last_idx = q_val
                 if l1_part <= sorted_data[q_val + 1]:
                     first_idx = q_val
@@ -1320,23 +1326,20 @@
 
         """
         data_abs = np.abs(args[0].flatten())
         ix = np.argsort(data_abs)[::-1]
         data_abs = data_abs[ix]  # Sorted absolute value of the data
         q_val = self._find_q(data_abs)
         cost_val = (
-            (
-                np.sum(data_abs[:q_val] ** 2) * 0.5
-                + np.sum(data_abs[q_val:]) ** 2
-                / (self._k_value - q_val)
-            ) * self.beta
-        )
+            np.sum(data_abs[:q_val] ** 2) * 0.5
+            + np.sum(data_abs[q_val:]) ** 2 / (self._k_value - q_val)
+        ) * self.beta
 
-        if 'verbose' in kwargs and kwargs['verbose']:
-            print(' - K-SUPPORT NORM (X):', cost_val)
+        if kwargs.get("verbose"):
+            print(" - K-SUPPORT NORM (X):", cost_val)
 
         return cost_val
 
 
 class GroupLASSO(ProximityParent):
     """Group LASSO norm proximity.
 
@@ -1373,25 +1376,26 @@
     """
 
     def __init__(self, weights):
         self.weights = weights
         self.op = self._op_method
         self.cost = self._cost_method
 
-    def _op_method(self, input_data, extra_factor=1.0):
+    def _op_method(self, input_data, *args, extra_factor=1.0, **kwargs):
         """Operator.
 
         This method returns the input data thresholded by the weights.
 
         Parameters
         ----------
         input_data : numpy.ndarray
             Input data array
         extra_factor : float
             Additional multiplication factor (default is ``1.0``)
+        *args, **kwargs: no effects
 
         Returns
         -------
         numpy.ndarray
             With proximal of GroupLASSO regularization
 
         """
@@ -1399,24 +1403,26 @@
         denominator = np.maximum(norm2, np.finfo(np.float32).eps)
 
         return input_data * np.maximum(
             0,
             (1.0 - self.weights * extra_factor / denominator),
         )
 
-    def _cost_method(self, input_data):
+    def _cost_method(self, input_data, *args, **kwargs):
         """Calculate the group LASSO component of the cost.
 
         This method calculate the cost function of the proximable part.
 
         Parameters
         ----------
         input_data : numpy.ndarray
             Input array of the sparse code
 
+        *args, **kwargs: no effects.
+
         Returns
         -------
         float
             The cost of GroupLASSO regularizer
 
         """
         return np.sum(self.weights * np.linalg.norm(input_data, axis=0))
```

### Comparing `modopt-1.7.1/modopt/opt/reweight.py` & `modopt-1.7.2/src/modopt/opt/reweight.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# -*- coding: utf-8 -*-
-
 """REWEIGHTING CLASSES.
 
 This module contains classes for reweighting optimisation implementations.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
 
 import numpy as np
 
 from modopt.base.types import check_float
 
 
-class cwbReweight(object):
+class cwbReweight:
     """Candes, Wakin and Boyd reweighting class.
 
     This class implements the reweighting scheme described in
     :cite:`candes2007`.
 
     Parameters
     ----------
@@ -41,15 +39,14 @@
     array([[0.5, 1. , 1.5],
            [2. , 2.5, 3. ],
            [3.5, 4. , 4.5]])
 
     """
 
     def __init__(self, weights, thresh_factor=1.0, verbose=False):
-
         self.weights = check_float(weights)
         self.original_weights = np.copy(self.weights)
         self.thresh_factor = check_float(thresh_factor)
         self._rw_num = 1
         self.verbose = verbose
 
     def reweight(self, input_data):
@@ -77,23 +74,23 @@
             w = w \left( \frac{1}{1 + \frac{|x^w|}{n \sigma}} \right)
 
         where :math:`w` are the weights, :math:`x` is the ``input_data`` and
         :math:`n` is the ``thresh_factor``.
 
         """
         if self.verbose:
-            print(' - Reweighting: {0}'.format(self._rw_num))
+            print(f" - Reweighting: {self._rw_num}")
 
         self._rw_num += 1
 
         input_data = check_float(input_data)
 
         if input_data.shape != self.weights.shape:
             raise ValueError(
-                'Input data must have the same shape as the initial weights.',
+                "Input data must have the same shape as the initial weights.",
             )
 
         thresh_weights = self.thresh_factor * self.original_weights
 
         self.weights *= np.array(
             1.0 / (1.0 + np.abs(input_data) / (thresh_weights)),
         )
```

### Comparing `modopt-1.7.1/modopt/plot/cost_plot.py` & `modopt-1.7.2/src/modopt/plot/cost_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """PLOTTING ROUTINES.
 
 This module contains methods for making plots.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -33,24 +31,24 @@
     Raises
     ------
     ImportError
         If Matplotlib package not found
 
     """
     if import_fail:
-        raise ImportError('Matplotlib package not found')
+        raise ImportError("Matplotlib package not found")
 
     else:
         if isinstance(output, type(None)):
-            file_name = 'cost_function.png'
+            file_name = "cost_function.png"
         else:
-            file_name = '{0}_cost_function.png'.format(output)
+            file_name = f"{output}_cost_function.png"
 
         plt.figure()
-        plt.plot(np.log10(cost_list), 'r-')
-        plt.title('Cost Function')
-        plt.xlabel('Iteration')
-        plt.ylabel(r'$\log_{10}$ Cost')
+        plt.plot(np.log10(cost_list), "r-")
+        plt.title("Cost Function")
+        plt.xlabel("Iteration")
+        plt.ylabel(r"$\log_{10}$ Cost")
         plt.savefig(file_name)
         plt.close()
 
-        print(' - Saving cost function data to:', file_name)
+        print(" - Saving cost function data to:", file_name)
```

### Comparing `modopt-1.7.1/modopt/signal/filter.py` & `modopt-1.7.2/src/modopt/signal/filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """FILTER ROUTINES.
 
 This module contains methods for distance measurements in cosmology.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -77,15 +75,15 @@
     -0.352139052257134
 
     """
     data_point = check_float(data_point)
     sigma = check_float(sigma)
 
     xs = (data_point / sigma) ** 2
-    factor = 2 * (3 * sigma) ** -0.5 * np.pi ** -0.25
+    factor = 2 * (3 * sigma) ** -0.5 * np.pi**-0.25
 
     return factor * (1 - xs) * np.exp(-0.5 * xs)
 
 
 def mex_hat_dir(data_gauss, data_mex, sigma):
     """Directional Mexican hat.
```

### Comparing `modopt-1.7.1/modopt/signal/noise.py` & `modopt-1.7.2/src/modopt/signal/noise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-# -*- coding: utf-8 -*-
-
 """NOISE ROUTINES.
 
 This module contains methods for adding and removing noise from data.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
 
-from builtins import zip
-
 import numpy as np
 
 from modopt.base.backend import get_array_module
 
 
-def add_noise(input_data, sigma=1.0, noise_type='gauss'):
+def add_noise(input_data, sigma=1.0, noise_type="gauss", rng=None):
     """Add noise to data.
 
     This method adds Gaussian or Poisson noise to the input data.
 
     Parameters
     ----------
     input_data : numpy.ndarray, list or tuple
         Input data array
     sigma : float or list, optional
         Standard deviation of the noise to be added (``'gauss'`` only,
         default is ``1.0``)
     noise_type : {'gauss', 'poisson'}
         Type of noise to be added (default is ``'gauss'``)
+    rng: np.random.Generator or int
+        A Random number generator or a seed to initialize one.
+
 
     Returns
     -------
     numpy.ndarray
         Input data with added noise
 
     Raises
@@ -64,43 +63,45 @@
     >>> x
     array([0., 0., 0., 0., 0.])
     >>> np.random.seed(1)
     >>> add_noise(x, sigma=2.0)
     array([ 3.24869073, -1.22351283, -1.0563435 , -2.14593724,  1.73081526])
 
     """
+    if not isinstance(rng, np.random.Generator):
+        rng = np.random.default_rng(rng)
+
     input_data = np.array(input_data)
 
-    if noise_type not in {'gauss', 'poisson'}:
+    if noise_type not in {"gauss", "poisson"}:
         raise ValueError(
             'Invalid noise type. Options are "gauss" or "poisson"',
         )
 
     if isinstance(sigma, (list, tuple, np.ndarray)):
         if len(sigma) != input_data.shape[0]:
             raise ValueError(
-                'Number of sigma values must match first dimension of input '
-                + 'data',
+                "Number of sigma values must match first dimension of input " + "data",
             )
 
-    if noise_type == 'gauss':
-        random = np.random.randn(*input_data.shape)
+    if noise_type == "gauss":
+        random = rng.standard_normal(input_data.shape)
 
-    elif noise_type == 'poisson':
-        random = np.random.poisson(np.abs(input_data))
+    elif noise_type == "poisson":
+        random = rng.poisson(np.abs(input_data))
 
     if isinstance(sigma, (int, float)):
         return input_data + sigma * random
 
     noise = np.array([sig * rand for sig, rand in zip(sigma, random)])
 
     return input_data + noise
 
 
-def thresh(input_data, threshold, threshold_type='hard'):
+def thresh(input_data, threshold, threshold_type="hard"):
     r"""Threshold data.
 
     This method perfoms hard or soft thresholding on the input data.
 
     Parameters
     ----------
     input_data : numpy.ndarray, list or tuple
@@ -165,19 +166,19 @@
            [0.        , 0.14556073, 0.19676747]])
 
     """
     xp = get_array_module(input_data)
 
     input_data = xp.array(input_data)
 
-    if threshold_type not in {'hard', 'soft'}:
+    if threshold_type not in {"hard", "soft"}:
         raise ValueError(
             'Invalid threshold type. Options are "hard" or "soft"',
         )
 
-    if threshold_type == 'soft':
+    if threshold_type == "soft":
         denominator = xp.maximum(xp.finfo(np.float64).eps, xp.abs(input_data))
         max_value = xp.maximum((1.0 - threshold / denominator), 0)
 
         return xp.around(max_value * input_data, decimals=15)
 
     return input_data * (xp.abs(input_data) >= threshold)
```

### Comparing `modopt-1.7.1/modopt/signal/positivity.py` & `modopt-1.7.2/src/modopt/signal/positivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """POSITIVITY.
 
 This module contains a function that retains only positive coefficients in
 an array.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
@@ -43,15 +41,15 @@
 
     Returns
     -------
     numpy.ndarray
         Positive coefficients
 
     """
-    if input_data.dtype == 'O':
+    if input_data.dtype == "O":
         res = np.array([pos_recursive(elem) for elem in input_data], dtype="object")
 
     else:
         res = pos_thresh(input_data)
 
     return res
 
@@ -93,21 +91,21 @@
     array([[0, 0, 0],
            [0, 0, 0],
            [1, 2, 3]])
 
     """
     if not isinstance(input_data, (int, float, list, tuple, np.ndarray)):
         raise TypeError(
-            'Invalid data type, input must be `int`, `float`, `list`, '
-            + '`tuple` or `np.ndarray`.',
+            "Invalid data type, input must be `int`, `float`, `list`, "
+            + "`tuple` or `np.ndarray`.",
         )
 
     if isinstance(input_data, (int, float)):
         return pos_thresh(input_data)
 
     if ragged:
-        input_data = np.array(input_data, dtype='object')
+        input_data = np.array(input_data, dtype="object")
 
     else:
         input_data = np.array(input_data)
 
     return pos_recursive(input_data)
```

### Comparing `modopt-1.7.1/modopt/signal/svd.py` & `modopt-1.7.2/src/modopt/signal/svd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """SVD ROUTINES.
 
 This module contains methods for thresholding singular values.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
 """
@@ -48,16 +46,16 @@
     >>> x = np.arange(18).reshape(9, 2).astype(float)
     >>> find_n_pc(svd(x)[0])
     1
 
     """
     if np.sqrt(u_vec.shape[0]) % 1:
         raise ValueError(
-            'Invalid left singular vector. The size of the first '
-            + 'dimenion of ``u_vec`` must be perfect square.',
+            "Invalid left singular vector. The size of the first "
+            + "dimenion of ``u_vec`` must be perfect square.",
         )
 
     # Get the shape of the array
     array_shape = np.repeat(int(np.sqrt(u_vec.shape[0])), 2)
 
     # Find the auto correlation of the left singular vector.
     u_auto = [
@@ -65,21 +63,20 @@
             elem.reshape(array_shape),
             np.rot90(elem.reshape(array_shape), 2),
         )
         for elem in u_vec.T
     ]
 
     # Return the required number of principal components.
-    return np.sum([
-        (
-            u_val[tuple(zip(array_shape // 2))] ** 2 <= factor
-            * np.sum(u_val ** 2),
-        )
-        for u_val in u_auto
-    ])
+    return np.sum(
+        [
+            (u_val[tuple(zip(array_shape // 2))] ** 2 <= factor * np.sum(u_val**2),)
+            for u_val in u_auto
+        ]
+    )
 
 
 def calculate_svd(input_data):
     """Calculate Singular Value Decomposition.
 
     This method calculates the Singular Value Decomposition (SVD) of the input
     data using SciPy.
@@ -97,25 +94,25 @@
     Raises
     ------
     TypeError
         For invalid data type
 
     """
     if (not isinstance(input_data, np.ndarray)) or (input_data.ndim != 2):
-        raise TypeError('Input data must be a 2D np.ndarray.')
+        raise TypeError("Input data must be a 2D np.ndarray.")
 
     return svd(
         input_data,
         check_finite=False,
-        lapack_driver='gesvd',
+        lapack_driver="gesvd",
         full_matrices=False,
     )
 
 
-def svd_thresh(input_data, threshold=None, n_pc=None, thresh_type='hard'):
+def svd_thresh(input_data, threshold=None, n_pc=None, thresh_type="hard"):
     """Threshold the singular values.
 
     This method thresholds the input data using singular value decomposition.
 
     Parameters
     ----------
     input_data : numpy.ndarray
@@ -152,65 +149,59 @@
            [10.05054985, 10.95361772],
            [11.96102884, 13.03575819],
            [13.87150784, 15.11789866],
            [15.78198684, 17.20003913]])
 
     """
     less_than_zero = isinstance(n_pc, int) and n_pc <= 0
-    str_not_all = isinstance(n_pc, str) and n_pc != 'all'
+    str_not_all = isinstance(n_pc, str) and n_pc != "all"
 
-    if (
-        (not isinstance(n_pc, (int, str, type(None))))
-        or less_than_zero
-        or str_not_all
-    ):
+    if (not isinstance(n_pc, (int, str, type(None)))) or less_than_zero or str_not_all:
         raise ValueError(
-            'Invalid value for "n_pc", specify a positive integer value or '
-            + '"all"',
+            'Invalid value for "n_pc", specify a positive integer value or ' + '"all"',
         )
 
     # Get SVD of input data.
     u_vec, s_values, v_vec = calculate_svd(input_data)
 
     # Find the threshold if not provided.
     if isinstance(threshold, type(None)):
         # Find the required number of principal components if not specified.
         if isinstance(n_pc, type(None)):
             n_pc = find_n_pc(u_vec, factor=0.1)
-            print('xxxx', n_pc, u_vec)
+            print("xxxx", n_pc, u_vec)
 
         # If the number of PCs is too large use all of the singular values.
-        if (
-            (isinstance(n_pc, int) and n_pc >= s_values.size)
-            or (isinstance(n_pc, str) and n_pc == 'all')
+        if (isinstance(n_pc, int) and n_pc >= s_values.size) or (
+            isinstance(n_pc, str) and n_pc == "all"
         ):
             n_pc = s_values.size
-            warn('Using all singular values.')
+            warn("Using all singular values.")
 
         threshold = s_values[n_pc - 1]
 
     # Threshold the singular values.
     s_new = thresh(s_values, threshold, thresh_type)
 
     if np.all(s_new == s_values):
-        warn('No change to singular values.')
+        warn("No change to singular values.")
 
     # Diagonalize the svd
     s_new = np.diag(s_new)
 
     # Return the thresholded data.
     return np.dot(u_vec, np.dot(s_new, v_vec))
 
 
 def svd_thresh_coef_fast(
     input_data,
     threshold,
     n_vals=-1,
     extra_vals=5,
-    thresh_type='hard',
+    thresh_type="hard",
 ):
     """Threshold the singular values coefficients.
 
     This method thresholds the input data by using singular value
     decomposition, but only computing the the greastest ``n_vals``
     values.
 
@@ -237,15 +228,15 @@
         thresholding (int)
     """
     if n_vals == -1:
         n_vals = min(input_data.shape) - 1
     ok = False
     while not ok:
         (u_vec, s_values, v_vec) = svds(input_data, k=n_vals)
-        ok = (s_values[0] <= threshold or n_vals == min(input_data.shape) - 1)
+        ok = s_values[0] <= threshold or n_vals == min(input_data.shape) - 1
         n_vals = min(n_vals + extra_vals, *input_data.shape)
 
     s_values = thresh(
         s_values,
         threshold,
         threshold_type=thresh_type,
     )
@@ -255,15 +246,15 @@
             u_vec[:, -rank:] * s_values[-rank:],
             v_vec[-rank:, :],
         ),
         rank,
     )
 
 
-def svd_thresh_coef(input_data, operator, threshold, thresh_type='hard'):
+def svd_thresh_coef(input_data, operator, threshold, thresh_type="hard"):
     """Threshold the singular values coefficients.
 
     This method thresholds the input data using singular value decomposition.
 
     Parameters
     ----------
     input_data : numpy.ndarray
@@ -283,33 +274,32 @@
     Raises
     ------
     TypeError
         If operator not callable
 
     """
     if not callable(operator):
-        raise TypeError('Operator must be a callable function.')
+        raise TypeError("Operator must be a callable function.")
 
     # Get SVD of data matrix
     u_vec, s_values, v_vec = calculate_svd(input_data)
 
     # Diagnalise s
     s_values = np.diag(s_values)
 
     # Compute coefficients
     a_matrix = np.dot(s_values, v_vec)
 
     # Get the shape of the array
     array_shape = np.repeat(int(np.sqrt(u_vec.shape[0])), 2)
 
     # Compute threshold matrix.
-    ti = np.array([
-        np.linalg.norm(elem)
-        for elem in operator(matrix2cube(u_vec, array_shape))
-    ])
+    ti = np.array(
+        [np.linalg.norm(elem) for elem in operator(matrix2cube(u_vec, array_shape))]
+    )
     threshold *= np.repeat(ti, a_matrix.shape[1]).reshape(a_matrix.shape)
 
     # Threshold coefficients.
     a_new = thresh(a_matrix, threshold, thresh_type)
 
     # Return the thresholded image.
     return np.dot(u_vec, a_new)
```

### Comparing `modopt-1.7.1/modopt/signal/validation.py` & `modopt-1.7.2/src/modopt/signal/validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 def transpose_test(
     operator,
     operator_t,
     x_shape,
     x_args=None,
     y_shape=None,
     y_args=None,
+    rng=None,
 ):
     """Transpose test.
 
     This method tests two operators to see if they are the transpose of each
     other.
 
     Parameters
@@ -32,14 +33,16 @@
         Shape of operator input data
     x_args : tuple
         Arguments to be passed to operator (default is ``None``)
     y_shape : tuple, optional
         Shape of transpose operator input data (default is ``None``)
     y_args : tuple, optional
         Arguments to be passed to transpose operator (default is ``None``)
+    rng: numpy.random.Generator or int or None (default is ``None``)
+        Initialized random number generator or seed.
 
     Raises
     ------
     TypeError
         If input operators not callable
 
     Examples
@@ -50,27 +53,29 @@
     >>> a = np.random.ranf((3, 3))
     >>> transpose_test(lambda x, y: x.dot(y), lambda x, y: x.dot(y.T),
     ... a.shape, x_args=a)
      - |<MX, Y> - <X, M.TY>| = 0.0
 
     """
     if not callable(operator) or not callable(operator_t):
-        raise TypeError('The input operators must be callable functions.')
+        raise TypeError("The input operators must be callable functions.")
 
     if isinstance(y_shape, type(None)):
         y_shape = x_shape
 
     if isinstance(y_args, type(None)):
         y_args = x_args
 
+    if not isinstance(rng, np.random.Generator):
+        rng = np.random.default_rng(rng)
     # Generate random arrays.
-    x_val = np.random.ranf(x_shape)
-    y_val = np.random.ranf(y_shape)
+    x_val = rng.random(x_shape)
+    y_val = rng.random(y_shape)
 
     # Calculate <MX, Y>
     mx_y = np.sum(np.multiply(operator(x_val, x_args), y_val))
 
     # Calculate <X, M.TY>
     x_mty = np.sum(np.multiply(x_val, operator_t(y_val, y_args)))
 
     # Test the difference between the two.
-    print(' - |<MX, Y> - <X, M.TY>| =', np.abs(mx_y - x_mty))
+    print(" - |<MX, Y> - <X, M.TY>| =", np.abs(mx_y - x_mty))
```

### Comparing `modopt-1.7.1/modopt/signal/wavelet.py` & `modopt-1.7.2/src/modopt/signal/wavelet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """WAVELET MODULE.
 
 This module contains methods for performing wavelet transformations using
 Spars2D.
 
 :Author: Samuel Farrens <samuel.farrens@cea.fr>
 
@@ -54,28 +52,28 @@
     Raises
     ------
     TypeError
         For invalid input type
 
     """
     if not isinstance(command_line, str):
-        raise TypeError('Command line must be a string.')
+        raise TypeError("Command line must be a string.")
 
     command = command_line.split()
 
     process = sp.Popen(command, stdout=sp.PIPE, stderr=sp.PIPE)
     stdout, stderr = process.communicate()
 
-    return stdout.decode('utf-8'), stderr.decode('utf-8')
+    return stdout.decode("utf-8"), stderr.decode("utf-8")
 
 
 def call_mr_transform(
     input_data,
-    opt='',
-    path='./',
+    opt="",
+    path="./",
     remove_files=True,
 ):  # pragma: no cover
     """Call ``mr_transform``.
 
     This method calls the Sparse2D module ``mr_transform``.
 
     Parameters
@@ -123,51 +121,48 @@
     <BLANKLINE>
            [[ 3.6484375 ,  3.73632812,  3.82421875],
             [ 3.91210938,  4.        ,  4.08789062],
             [ 4.17578125,  4.26367188,  4.3515625 ]]])
 
     """
     if not import_astropy:
-        raise ImportError('Astropy package not found.')
+        raise ImportError("Astropy package not found.")
 
     if (not isinstance(input_data, np.ndarray)) or (input_data.ndim != 2):
-        raise ValueError('Input data must be a 2D numpy array.')
+        raise ValueError("Input data must be a 2D numpy array.")
 
-    executable = 'mr_transform'
+    executable = "mr_transform"
 
     # Make sure mr_transform is installed.
     is_executable(executable)
 
     # Create a unique string using the current date and time.
-    unique_string = (
-        datetime.now().strftime('%Y.%m.%d_%H.%M.%S')
-        + str(getrandbits(128))
-    )
+    unique_string = datetime.now().strftime("%Y.%m.%d_%H.%M.%S") + str(getrandbits(128))
 
     # Set the ouput file names.
-    file_name = '{0}mr_temp_{1}'.format(path, unique_string)
-    file_fits = '{0}.fits'.format(file_name)
-    file_mr = '{0}.mr'.format(file_name)
+    file_name = f"{path}mr_temp_{unique_string}"
+    file_fits = f"{file_name}.fits"
+    file_mr = f"{file_name}.mr"
 
     # Write the input data to a fits file.
     fits.writeto(file_fits, input_data)
 
     if isinstance(opt, str):
         opt = opt.split()
 
     # Prepare command and execute it
-    command_line = ' '.join([executable] + opt + [file_fits, file_mr])
+    command_line = " ".join([executable, *opt, file_fits, file_mr])
     stdout, _ = execute(command_line)
 
     # Check for errors
-    if any(word in stdout for word in ('bad', 'Error', 'Sorry')):
+    if any(word in stdout for word in ("bad", "Error", "Sorry")):
         remove(file_fits)
         message = '{0} raised following exception: "{1}"'
         raise RuntimeError(
-            message.format(executable, stdout.rstrip('\n')),
+            message.format(executable, stdout.rstrip("\n")),
         )
 
     # Retrieve wavelet transformed data.
     data_trans = fits.getdata(file_mr).astype(input_data.dtype)
 
     # Remove the temporary files.
     if remove_files:
@@ -194,20 +189,20 @@
         Trimmed filter
 
     """
     non_zero_indices = np.array(np.where(filter_array != 0))
     min_idx = np.min(non_zero_indices, axis=-1)
     max_idx = np.max(non_zero_indices, axis=-1)
 
-    return filter_array[min_idx[0]:max_idx[0] + 1, min_idx[1]:max_idx[1] + 1]
+    return filter_array[min_idx[0] : max_idx[0] + 1, min_idx[1] : max_idx[1] + 1]
 
 
 def get_mr_filters(
     data_shape,
-    opt='',
+    opt="",
     coarse=False,
     trim=False,
 ):  # pragma: no cover
     """Get ``mr_transform`` filters.
 
     This method obtains wavelet filters by calling mr_transform.
 
@@ -252,15 +247,15 @@
     # Return filters
     if coarse:
         return mr_filters
 
     return mr_filters[:-1]
 
 
-def filter_convolve(input_data, filters, filter_rot=False, method='scipy'):
+def filter_convolve(input_data, filters, filter_rot=False, method="scipy"):
     """Filter convolve.
 
     This method convolves the input image with the wavelet filters.
 
     Parameters
     ----------
     input_data : numpy.ndarray
@@ -311,24 +306,22 @@
             [
                 convolve(coef, filt, method=method)
                 for coef, filt in zip(input_data, rotate_stack(filters))
             ],
             axis=0,
         )
 
-    return np.array([
-        convolve(input_data, filt, method=method) for filt in filters
-    ])
+    return np.array([convolve(input_data, filt, method=method) for filt in filters])
 
 
 def filter_convolve_stack(
     input_data,
     filters,
     filter_rot=False,
-    method='scipy',
+    method="scipy",
 ):
     """Filter convolve.
 
     This method convolves the a stack of input images with the wavelet filters.
 
     Parameters
     ----------
@@ -362,11 +355,13 @@
     <BLANKLINE>
            [[ 22.,  19.,  22.],
             [ 85.,  82.,  85.],
             [148., 145., 148.]]])
 
     """
     # Return the convolved data cube.
-    return np.array([
-        filter_convolve(elem, filters, filter_rot=filter_rot, method=method)
-        for elem in input_data
-    ])
+    return np.array(
+        [
+            filter_convolve(elem, filters, filter_rot=filter_rot, method=method)
+            for elem in input_data
+        ]
+    )
```

### Comparing `modopt-1.7.1/modopt.egg-info/PKG-INFO` & `modopt-1.7.2/src/modopt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 Metadata-Version: 2.1
 Name: modopt
-Version: 1.7.1
+Version: 1.7.2
 Summary: Modular Optimisation tools for soliving inverse problems.
-Home-page: https://github.com/cea-cosmic/modopt
-Author: Samuel Farrens
-Author-email: samuel.farrens@cea.fr
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
+Author-email: Samuel Farrens <samuel.farrens@cea.fr>, Chaithya GR <chaithyagr@gmail.com>, Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>, Philippe Ciuciu <philippe.ciuciu@cea.fr>
+License: MIT License
+        
+        Copyright (c) 2017 Samuel Farrens
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: importlib_metadata>=3.7.0
-Requires-Dist: numpy>=1.19.5
-Requires-Dist: scipy>=1.5.4
-Requires-Dist: tqdm>=4.64.0
-Provides-Extra: develop
-Requires-Dist: coverage>=5.5; extra == "develop"
-Requires-Dist: pytest>=6.2.2; extra == "develop"
-Requires-Dist: pytest-raises>=0.10; extra == "develop"
-Requires-Dist: pytest-cases>=3.6; extra == "develop"
-Requires-Dist: pytest-xdist>=3.0.1; extra == "develop"
-Requires-Dist: pytest-cov>=2.11.1; extra == "develop"
-Requires-Dist: pytest-emoji>=0.2.0; extra == "develop"
-Requires-Dist: pydocstyle==6.1.1; extra == "develop"
-Requires-Dist: pytest-pydocstyle>=2.2.0; extra == "develop"
-Requires-Dist: black; extra == "develop"
-Requires-Dist: isort; extra == "develop"
-Requires-Dist: pytest-black; extra == "develop"
-Requires-Dist: jupyter==1.0.0; extra == "develop"
-Requires-Dist: myst-parser==0.16.1; extra == "develop"
-Requires-Dist: nbsphinx==0.8.7; extra == "develop"
-Requires-Dist: nbsphinx-link==1.3.0; extra == "develop"
-Requires-Dist: numpydoc==1.1.0; extra == "develop"
-Requires-Dist: sphinx==4.3.1; extra == "develop"
-Requires-Dist: sphinxcontrib-bibtex==2.4.1; extra == "develop"
-Requires-Dist: sphinxawesome-theme==3.2.1; extra == "develop"
-Requires-Dist: sphinx-gallery==0.11.1; extra == "develop"
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: importlib_metadata
+Provides-Extra: gpu
+Requires-Dist: torch; extra == "gpu"
+Requires-Dist: ptwt; extra == "gpu"
+Provides-Extra: doc
+Requires-Dist: myst-parser; extra == "doc"
+Requires-Dist: nbsphinx; extra == "doc"
+Requires-Dist: nbsphinx-link; extra == "doc"
+Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: sphinxawesome-theme; extra == "doc"
+Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest<8.0.0; extra == "test"
+Requires-Dist: pytest-cases; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
 
 # ModOpt
 
 <img width=400 src="https://raw.githubusercontent.com/CEA-COSMIC/ModOpt/master/docs/source/modopt_logo.png">
 
 | Usage | Development | Release |
 | ----- | ----------- | ------- |
```

