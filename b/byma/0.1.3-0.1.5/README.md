# Comparing `tmp/byma-0.1.3.tar.gz` & `tmp/byma-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.3.tar", last modified: Wed Apr 10 17:49:01 2024, max compression
+gzip compressed data, was "byma-0.1.5.tar", last modified: Fri Apr 12 08:12:59 2024, max compression
```

## Comparing `byma-0.1.3.tar` & `byma-0.1.5.tar`

### file list

```diff
@@ -1,108 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.985394 byma-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-10 17:48:47.000000 byma-0.1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-10 17:48:47.000000 byma-0.1.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-10 17:48:47.000000 byma-0.1.3/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-10 17:48:47.000000 byma-0.1.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-10 17:48:47.000000 byma-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-10 17:49:01.985394 byma-0.1.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-10 17:48:47.000000 byma-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.970394 byma-0.1.3/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-10 17:48:47.000000 byma-0.1.3/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-10 17:49:01.000000 byma-0.1.3/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.972394 byma-0.1.3/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-10 17:48:47.000000 byma-0.1.3/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.972394 byma-0.1.3/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/Iteral.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-10 17:48:47.000000 byma-0.1.3/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.973394 byma-0.1.3/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-10 17:48:47.000000 byma-0.1.3/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.974394 byma-0.1.3/byma/numy/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/Numy.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/_numy.py
--rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-10 17:48:47.000000 byma-0.1.3/byma/numy/integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.975394 byma-0.1.3/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-10 17:48:47.000000 byma-0.1.3/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-10 17:48:47.000000 byma-0.1.3/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 17:49:01.000000 byma-0.1.3/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.975394 byma-0.1.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-10 17:48:47.000000 byma-0.1.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-10 17:48:47.000000 byma-0.1.3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-10 17:48:47.000000 byma-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.976394 byma-0.1.3/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3791 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.977394 byma-0.1.3/docs/source/autoapi/byma/iteral/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/Iteral/
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/Iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.978394 byma-0.1.3/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2112 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.979394 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/nonstationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/Stationary/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/iteral/stationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.980394 byma-0.1.3/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.981394 byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/Numy/
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/Numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/_numy/
--rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/_numy/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.982394 byma-0.1.3/docs/source/autoapi/byma/numy/integration/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/numy/integration/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.983394 byma-0.1.3/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.983394 byma-0.1.3/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-10 17:48:47.000000 byma-0.1.3/docs/source/user/whatisbyma.rst
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-10 17:48:47.000000 byma-0.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-10 17:48:47.000000 byma-0.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 17:49:01.985394 byma-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-10 17:48:47.000000 byma-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:49:01.984394 byma-0.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 17:48:47.000000 byma-0.1.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.714717 byma-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-12 08:12:48.000000 byma-0.1.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-12 08:12:48.000000 byma-0.1.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-12 08:12:48.000000 byma-0.1.5/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-12 08:12:48.000000 byma-0.1.5/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-12 08:12:48.000000 byma-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-12 08:12:59.713717 byma-0.1.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-12 08:12:48.000000 byma-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.702717 byma-0.1.5/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-12 08:12:48.000000 byma-0.1.5/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-12 08:12:59.000000 byma-0.1.5/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.704717 byma-0.1.5/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-12 08:12:48.000000 byma-0.1.5/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.705717 byma-0.1.5/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/Iteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-04-12 08:12:48.000000 byma-0.1.5/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.706717 byma-0.1.5/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7951 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-12 08:12:48.000000 byma-0.1.5/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.706717 byma-0.1.5/byma/numy/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/Numy.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/_numy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-04-12 08:12:48.000000 byma-0.1.5/byma/numy/integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.707717 byma-0.1.5/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-12 08:12:48.000000 byma-0.1.5/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2024-04-12 08:12:48.000000 byma-0.1.5/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 08:12:59.000000 byma-0.1.5/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.707717 byma-0.1.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-12 08:12:48.000000 byma-0.1.5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-12 08:12:48.000000 byma-0.1.5/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-12 08:12:48.000000 byma-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.708717 byma-0.1.5/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/interface/Time/
+-rw-rw-rw-   0 root         (0) root         (0)     6246 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/Time/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3809 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.709717 byma-0.1.5/docs/source/autoapi/byma/iteral/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/Iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/Iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1912 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2112 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.710717 byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/Numy/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/Numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/_numy/
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/_numy/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.711717 byma-0.1.5/docs/source/autoapi/byma/numy/integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/numy/integration/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.712717 byma-0.1.5/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.712717 byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-12 08:12:48.000000 byma-0.1.5/docs/source/user/whatisbyma.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-12 08:12:48.000000 byma-0.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-12 08:12:48.000000 byma-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 08:12:59.714717 byma-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-12 08:12:48.000000 byma-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:12:59.713717 byma-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 08:12:48.000000 byma-0.1.5/tests/__init__.py
```

### Comparing `byma-0.1.3/.gitlab-ci.yml` & `byma-0.1.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/LICENSE.md` & `byma-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/PKG-INFO` & `byma-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.3/README.md` & `byma-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/__init__.py` & `byma-0.1.5/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/interface/BaseInterface.py` & `byma-0.1.5/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/interface/NonlinearHeat.py` & `byma-0.1.5/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/iteral/Newton.py` & `byma-0.1.5/byma/iteral/Newton.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/iteral/OrthogonalSubspace.py` & `byma-0.1.5/byma/iteral/OrthogonalSubspace.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/nuby/Continuation.py` & `byma-0.1.5/byma/nuby/Continuation.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/numy/integration.py` & `byma-0.1.5/byma/numy/integration.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/byma/pyplot/plots.py` & `byma-0.1.5/byma/pyplot/plots.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,138 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
     
 
-def plot_scale(x, y, label, scale, style=None):
+def plot_scale(x, y, label, scale, style={}):
     """
     Plot data with specified scale and style.
 
     Parameters
-    ----------
+    ================
     x : array-like
         Data points for the x-axis.
     y : array-like
         Data points for the y-axis.
     label : str
         Label for the data.
     scale : str
         Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
     style : dict or None, optional
         Dictionary specifying line style. If None, default style is used.
 
     Returns
     -------
     None
+    
+    Examples
+    ================
+    Plotting with different scales:
+
+    >>> import numpy as np
+    >>> import matplotlib.pyplot as plt
+    >>> import byma.pyplot as byplt
+
+    >>> x = np.linspace(0.1, 10, 100)
+    >>> y = np.sin(x)
+
+    # Normal scale
+    >>> plt.figure()
+    >>> byplt.plot_scale(x, y, label='sin(x)', scale='normal')
+    >>> plt.legend()
+    >>> plt.show()
+
+    # Log-log scale
+    >>> plt.figure()
+    >>> byplt.plot_scale(x, y, label='sin(x)', scale='loglog')
+    >>> plt.legend()
+    >>> plt.show()
+
+    # Semi-log x scale
+    >>> plt.figure()
+    >>> byplt.plot_scale(x, y, label='sin(x)', scale='xlog')
+    >>> plt.legend()
+    >>> plt.show()
+
+    # Semi-log y scale
+    >>> plt.figure()
+    >>> byplt.plot_scale(x, y, label='sin(x)', scale='ylog')
+    >>> plt.legend()
+    >>> plt.show()
     """
     if scale == 'loglog':
-        plt.loglog(x, y, label=label)
+        plt.loglog(x, y, label=label, **style)
     elif scale == 'xlog':
-        plt.semilogx(x, y, label=label)
+        plt.semilogx(x, y, label=label, **style)
     elif scale == 'ylog':
-        plt.semilogy(x, y, label=label)
+        plt.semilogy(x, y, label=label, **style)
+    elif scale == 'scatter':
+        plt.scatter(x, y, label=label, **style)
     else:
-        plt.plot(x, y, label=label)
+        plt.plot(x, y, label=label, **style)
 
-def plot(x, y, **kwargs):
+def plot(x=None, y=None, **kwargs):
     """
-    Function that create plots of different kinds. With this function it is possible to plots n numbers of 
+    Function that creates plots of different kinds. With this function, it is possible to plot n numbers of 
     function in the same figure quickly and with high personalization.
 
     Parameters
-    ----------
+    ==============
     x : array-like
         Array of x values.
     y : array-like
         Array of y values.
     **kwargs : dict, optional
         settings (dict): Overall plot settings.
             title (str): Title of the plot.
             xlabel (str): Label for the x-axis.
             ylabel (str): Label for the y-axis.
             label (str):  Label for the 1st function.
-            label{i} (str): Label for the ith function from i=2.
-            x{i} (array-like): Array of x values for the ith function from i=2.
-            y{i} (array-like): Array of y values for the ith function from i=2.
+            label{i} (str): Label for the ith function from i=1.
+            x{i} (array-like): Array of x values for the ith function from i=1.
+            y{i} (array-like): Array of y values for the ith function from i=1.
             save_title (str): File name to save the plot.
             save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
             scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-        style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
+            style{i} (dic, string): Dictionary, string having customization from the matplotlib functions, like style
 
     Returns
-    -------
-    None
+    ===========
+    A plot
     """
     settings = kwargs.pop('settings', {})
     settings.update(kwargs)  # Incorporate any additional kwargs into settings
 
-    scale = settings.get('scale', 'normal')
-    style = settings.get('style', None)
+    scale = settings.pop('scale', 'normal')
 
     plt.figure()
     plt.title(settings.get('title', 'Plot'))
     plt.xlabel(settings.get('xlabel', 'x'))
     plt.ylabel(settings.get('ylabel', 'y'))
+    
+    
+    x = settings.get('x') if (x is None) else x
+    y = settings.get('y') if (y is None) else y
+    style = settings.get('style', {'linestyle': '--'})
 
     plot_scale(x, y, label=settings.get('label', 'y'), scale=scale, style=style)
 
-    for i in range(2, 10):
+    i = 1
+    while f'y{i}' in settings:
         y_i = settings.get(f'y{i}', None)
+        x_i = settings.get(f'x{i}', None)
         if y_i is not None:
             label_i = settings.get(f'label{i}', f'y{i}')
-            style_i = style[i-2] if isinstance(style, list) else style
-            plot_scale(x, y_i, label=label_i, scale=scale, style=style_i)
-        else:
-            break
+            style_i = settings.get(f'style{i}', {'linestyle': '--'})
+            if x_i is None:
+                plot_scale(x, y_i, label=label_i, scale=scale, style=style_i)
+            else:
+                plot_scale(x_i, y_i, label=label_i, scale=scale, style=style_i)
+            i += 1
+
 
     plt.legend()
     plt.show()
 
     save_title = settings.get('save_title', settings.get('title', 'Plot'))
     save_path = settings.get('save_path', None)
```

### Comparing `byma-0.1.3/byma.egg-info/PKG-INFO` & `byma-0.1.5/byma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.3
+Version: 0.1.5
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.3/byma.egg-info/SOURCES.txt` & `byma-0.1.5/byma.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 byma/_version.py
 byma.egg-info/PKG-INFO
 byma.egg-info/SOURCES.txt
 byma.egg-info/dependency_links.txt
 byma.egg-info/top_level.txt
 byma/interface/BaseInterface.py
 byma/interface/NonlinearHeat.py
+byma/interface/Time.py
 byma/interface/__init__.py
 byma/iteral/Iteral.py
 byma/iteral/Newton.py
 byma/iteral/OrthogonalSubspace.py
 byma/iteral/__init__.py
 byma/nuby/Bifurcation.py
 byma/nuby/Continuation.py
@@ -37,24 +38,19 @@
 docs/source/index.rst
 docs/source/autoapi/index.rst
 docs/source/autoapi/byma/index.rst
 docs/source/autoapi/byma/_version/index.rst
 docs/source/autoapi/byma/interface/index.rst
 docs/source/autoapi/byma/interface/BaseInterface/index.rst
 docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+docs/source/autoapi/byma/interface/Time/index.rst
 docs/source/autoapi/byma/iteral/index.rst
 docs/source/autoapi/byma/iteral/Iteral/index.rst
 docs/source/autoapi/byma/iteral/Newton/index.rst
 docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst
-docs/source/autoapi/byma/iteral/nonstationary/index.rst
-docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
-docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
-docs/source/autoapi/byma/iteral/stationary/index.rst
-docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
-docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
 docs/source/autoapi/byma/nuby/index.rst
 docs/source/autoapi/byma/nuby/Bifurcation/index.rst
 docs/source/autoapi/byma/nuby/Continuation/index.rst
 docs/source/autoapi/byma/nuby/_nuby/index.rst
 docs/source/autoapi/byma/numy/index.rst
 docs/source/autoapi/byma/numy/Numy/index.rst
 docs/source/autoapi/byma/numy/_numy/index.rst
```

### Comparing `byma-0.1.3/docs/Makefile` & `byma-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/make.bat` & `byma-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/interface/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ----------
 .. toctree::
    :titlesonly:
    :maxdepth: 1
 
    BaseInterface/index.rst
    NonlinearHeat/index.rst
+   Time/index.rst
 
 
 Package Contents
 ----------------
 
 Classes
 ~~~~~~~
```

### Comparing `byma-0.1.3/docs/source/autoapi/byma/iteral/Newton/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/iteral/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/iteral/OrthogonalSubspace/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/numy/_numy/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/numy/_numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/numy/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/numy/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/numy/integration/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/numy/integration/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.5/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-:py:mod:`byma.pyplot`
-=====================
+:py:mod:`byma.pyplot.plots`
+===========================
 
-.. py:module:: byma.pyplot
+.. py:module:: byma.pyplot.plots
 
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
-
-   plots/index.rst
-
-
-Package Contents
-----------------
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.pyplot.plot_scale
-   byma.pyplot.plot
-   byma.pyplot.plot_numerical_error
+   byma.pyplot.plots.plot_scale
+   byma.pyplot.plots.plot
+   byma.pyplot.plots.plot_numerical_error
 
 
 
-.. py:function:: plot_scale(x, y, label, scale, style=None)
+.. py:function:: plot_scale(x, y, label, scale, style={})
 
    Plot data with specified scale and style.
 
    Parameters
-   ----------
+   ================
    x : array-like
        Data points for the x-axis.
    y : array-like
        Data points for the y-axis.
    label : str
        Label for the data.
    scale : str
@@ -45,43 +36,78 @@
    style : dict or None, optional
        Dictionary specifying line style. If None, default style is used.
 
    Returns
    -------
    None
 
+   Examples
+   ================
+   Plotting with different scales:
+
+   >>> import numpy as np
+   >>> import matplotlib.pyplot as plt
+   >>> import byma.pyplot as byplt
+
+   >>> x = np.linspace(0.1, 10, 100)
+   >>> y = np.sin(x)
+
+   # Normal scale
+   >>> plt.figure()
+   >>> byplt.plot_scale(x, y, label='sin(x)', scale='normal')
+   >>> plt.legend()
+   >>> plt.show()
+
+   # Log-log scale
+   >>> plt.figure()
+   >>> byplt.plot_scale(x, y, label='sin(x)', scale='loglog')
+   >>> plt.legend()
+   >>> plt.show()
+
+   # Semi-log x scale
+   >>> plt.figure()
+   >>> byplt.plot_scale(x, y, label='sin(x)', scale='xlog')
+   >>> plt.legend()
+   >>> plt.show()
+
+   # Semi-log y scale
+   >>> plt.figure()
+   >>> byplt.plot_scale(x, y, label='sin(x)', scale='ylog')
+   >>> plt.legend()
+   >>> plt.show()
 
-.. py:function:: plot(x, y, **kwargs)
 
-   Function that create plots of different kinds. With this function it is possible to plots n numbers of 
+.. py:function:: plot(x=None, y=None, **kwargs)
+
+   Function that creates plots of different kinds. With this function, it is possible to plot n numbers of 
    function in the same figure quickly and with high personalization.
 
    Parameters
-   ----------
+   ==============
    x : array-like
        Array of x values.
    y : array-like
        Array of y values.
    **kwargs : dict, optional
        settings (dict): Overall plot settings.
            title (str): Title of the plot.
            xlabel (str): Label for the x-axis.
            ylabel (str): Label for the y-axis.
            label (str):  Label for the 1st function.
-           label{i} (str): Label for the ith function from i=2.
-           x{i} (array-like): Array of x values for the ith function from i=2.
-           y{i} (array-like): Array of y values for the ith function from i=2.
+           label{i} (str): Label for the ith function from i=1.
+           x{i} (array-like): Array of x values for the ith function from i=1.
+           y{i} (array-like): Array of y values for the ith function from i=1.
            save_title (str): File name to save the plot.
            save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
            scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-       style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
+           style{i} (dic, string): Dictionary, string having customization from the matplotlib functions, like style
 
    Returns
-   -------
-   None
+   ===========
+   A plot
 
 
 .. py:function:: plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs)
 
    Plot the numerical error between the exact and numerical solutions and print the maximum error.
 
    Parameters
```

### Comparing `byma-0.1.3/docs/source/conf.py` & `byma-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/docs/source/index.rst` & `byma-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/pyproject.toml` & `byma-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.3/setup.py` & `byma-0.1.5/setup.py`

 * *Files identical despite different names*

