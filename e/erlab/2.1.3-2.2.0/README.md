# Comparing `tmp/erlab-2.1.3.tar.gz` & `tmp/erlab-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.1.3.tar", last modified: Thu Apr 11 03:07:02 2024, max compression
+gzip compressed data, was "erlab-2.2.tar", last modified: Fri Apr 12 18:28:40 2024, max compression
```

## Comparing `erlab-2.1.3.tar` & `erlab-2.2.tar`

### file list

```diff
@@ -1,174 +1,175 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.820390 erlab-2.1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.776389 erlab-2.1.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 03:06:56.000000 erlab-2.1.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 03:06:56.000000 erlab-2.1.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-11 03:06:56.000000 erlab-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-11 03:06:56.000000 erlab-2.1.3/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   104848 2024-04-11 03:06:59.000000 erlab-2.1.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-11 03:06:56.000000 erlab-2.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 03:07:02.820390 erlab-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 03:06:56.000000 erlab-2.1.3/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-11 03:06:56.000000 erlab-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.784390 erlab-2.1.3/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.788390 erlab-2.1.3/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    16011 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.792389 erlab-2.1.3/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   321080 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   317804 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2342 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     5063 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    50053 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379705 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    16193 2024-04-11 03:06:56.000000 erlab-2.1.3/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-11 03:06:56.000000 erlab-2.1.3/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-11 03:06:56.000000 erlab-2.1.3/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4373 2024-04-11 03:06:56.000000 erlab-2.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-11 03:06:56.000000 erlab-2.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 03:07:02.820390 erlab-2.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.776389 erlab-2.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.796390 erlab-2.1.3/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-11 03:06:59.000000 erlab-2.1.3/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.800390 erlab-2.1.3/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.800390 erlab-2.1.3/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      839 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9632 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)     9881 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15448 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10629 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.804390 erlab-2.1.3/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20867 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19705 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54143 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31737 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.808390 erlab-2.1.3/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7594 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7804 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6777 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.812390 erlab-2.1.3/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.812390 erlab-2.1.3/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18284 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32437 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-11 03:06:56.000000 erlab-2.1.3/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4675 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 03:07:02.000000 erlab-2.1.3/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-11 03:06:56.000000 erlab-2.1.3/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.780390 erlab-2.1.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:07:02.816390 erlab-2.1.3/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 03:06:56.000000 erlab-2.1.3/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.165212 erlab-2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.125213 erlab-2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-12 18:28:33.000000 erlab-2.2/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-12 18:28:33.000000 erlab-2.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.125213 erlab-2.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-12 18:28:33.000000 erlab-2.2/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-12 18:28:33.000000 erlab-2.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-12 18:28:33.000000 erlab-2.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-12 18:28:33.000000 erlab-2.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-12 18:28:33.000000 erlab-2.2/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   106158 2024-04-12 18:28:36.000000 erlab-2.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-12 18:28:33.000000 erlab-2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-12 18:28:40.161213 erlab-2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-12 18:28:33.000000 erlab-2.2/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-12 18:28:33.000000 erlab-2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.129212 erlab-2.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-12 18:28:33.000000 erlab-2.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-12 18:28:33.000000 erlab-2.2/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-12 18:28:33.000000 erlab-2.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      451 2024-04-12 18:28:33.000000 erlab-2.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.129212 erlab-2.2/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16040 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.137213 erlab-2.2/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   321080 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   317804 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3285 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.137213 erlab-2.2/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.141213 erlab-2.2/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    21971 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50534 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379705 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16293 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-12 18:28:33.000000 erlab-2.2/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-12 18:28:33.000000 erlab-2.2/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-12 18:28:33.000000 erlab-2.2/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-12 18:28:33.000000 erlab-2.2/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4373 2024-04-12 18:28:33.000000 erlab-2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-12 18:28:33.000000 erlab-2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 18:28:40.165212 erlab-2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.141213 erlab-2.2/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-12 18:28:36.000000 erlab-2.2/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35543 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9760 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     7809 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    11340 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15393 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.149212 erlab-2.2/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21311 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22774 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9454 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.149212 erlab-2.2/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19705 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31737 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    37209 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47782 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4718 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-12 18:28:33.000000 erlab-2.2/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-12 18:28:33.000000 erlab-2.2/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-12 18:28:33.000000 erlab-2.2/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_utilities.py
```

### Comparing `erlab-2.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/.github/workflows/pr.yml` & `erlab-2.2/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/.github/workflows/release.yml` & `erlab-2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/.gitignore` & `erlab-2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/.pre-commit-config.yaml` & `erlab-2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/.readthedocs.yaml` & `erlab-2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/CHANGELOG.md` & `erlab-2.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,40 @@
 # CHANGELOG
 
 
 
+## v2.2.0 (2024-04-12)
+
+### Documentation
+
+* improve fitting documentation ([`9e0a106`](https://github.com/kmnhan/erlabpy/commit/9e0a10611a32ac75798e68f864cff55b5661330f))
+
+* add curve fitting guide ([`ff9743c`](https://github.com/kmnhan/erlabpy/commit/ff9743c2203eb773af6bdb8d88426907f4300924))
+
+* add docstrings to plotting.colors ([`1a15a70`](https://github.com/kmnhan/erlabpy/commit/1a15a706aa2fd591a18401ea53f950005391c88f))
+
+### Feature
+
+* enable component evaluation for MultiPeakModel ([`8875b74`](https://github.com/kmnhan/erlabpy/commit/8875b7443d26313156fcdcc43586d40af4ff4f00))
+
+* (**analysis.fit**) add BCS gap equation and Dynes formula ([`f862aa4`](https://github.com/kmnhan/erlabpy/commit/f862aa4af4d2ba470f1ea074fc90442d9b18b336))
+
+### Fix
+
+* curvefittingtool errors ([`9abb99c`](https://github.com/kmnhan/erlabpy/commit/9abb99c35633bc722469276d4837a2372c132042))
+
+### Refactor
+
+* cleanup fit namespace ([`906aa99`](https://github.com/kmnhan/erlabpy/commit/906aa99193f78577e705218b2d6c22378611f84b))
+
+* rename ExtendedAffineBroadenedFD to FermiEdgeModel ([`a98aa82`](https://github.com/kmnhan/erlabpy/commit/a98aa82bcbdf22ff8a156d800e336653f9afba07))
+
+* (**interactive**) exclude bad colormaps ([`877c915`](https://github.com/kmnhan/erlabpy/commit/877c915def6eb3dddb3862d6ac64c8c70f456ad3))
+
+
 ## v2.1.3 (2024-04-11)
 
 ### Fix
 
 * (**interactive**) update data load functions used in imagetool ([`c3abe35`](https://github.com/kmnhan/erlabpy/commit/c3abe3517046ed603a9221de38b22257322d3a51))
```

### Comparing `erlab-2.1.3/LICENSE` & `erlab-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/PKG-INFO` & `erlab-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.3/PythonInterface.ipf` & `erlab-2.2/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/README.md` & `erlab-2.2/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/Makefile` & `erlab-2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/environment.yml` & `erlab-2.2/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/make.bat` & `erlab-2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/conf.py` & `erlab-2.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     "lmfit": ("https://lmfit.github.io/lmfit-py/", None),
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
     "pandas": ("https://pandas.pydata.org/docs/", None),
     "pyqtgraph": ("https://pyqtgraph.readthedocs.io/en/latest/", None),
     "csaps": ("https://csaps.readthedocs.io/en/latest/", None),
     "iminuit": ("https://scikit-hep.org/iminuit/", None),
+    "cmasher": ("https://cmasher.readthedocs.io/", None),
 }
 
 
 # -- Plot configuration ------------------------------------------------------
 
 plot_formats = ["pdf"]
 plot_basedir = "pyplots"
@@ -417,15 +418,14 @@
 }
 
 # -- LaTeX options -----------------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#latex-options
 
 latex_engine = "lualatex"
 latex_show_pagerefs = True
-latex_show_urls = "footnote"
 latex_table_style = ["booktabs", "colorrows"]
 latex_elements = {
     "fontpkg": r"""\usepackage{fontspec,unicode-math}
 \setmainfont{DejaVu Serif}
 \setsansfont{DejaVu Sans}
 \setmonofont{DejaVu Sans Mono}
 """
```

### Comparing `erlab-2.1.3/docs/source/contributing.rst` & `erlab-2.2/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/getting-started.rst` & `erlab-2.2/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/flowchart_multiple.pdf` & `erlab-2.2/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/flowchart_single.pdf` & `erlab-2.2/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/imagetool_dark.png` & `erlab-2.2/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/imagetool_light.png` & `erlab-2.2/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/ktool_1_dark.png` & `erlab-2.2/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/ktool_1_light.png` & `erlab-2.2/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/ktool_2_dark.png` & `erlab-2.2/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/images/ktool_2_light.png` & `erlab-2.2/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/index.rst` & `erlab-2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/pyplots/norms.py` & `erlab-2.2/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/reference.rst` & `erlab-2.2/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/refs.bib` & `erlab-2.2/docs/source/refs.bib`

 * *Files 8% similar despite different names*

```diff
@@ -69,7 +69,19 @@
   journal   = {J. Open Res. Softw.},
   volume    = {5},
   number    = {1},
   year      = {2017},
   publisher = {Ubiquity Press},
   doi       = {10.5334/jors.148}
 }
+
+@article{dynes1978dynes,
+  author  = {Dynes, R. C. and Narayanamurti, V. and Garno, J. P.},
+  title   = {Direct Measurement of Quasiparticle-Lifetime Broadening in a Strong-Coupled Superconductor},
+  journal = {Phys. Rev. Lett.},
+  volume  = {41},
+  number  = {21},
+  pages   = {1509-1512},
+  doi     = {10.1103/PhysRevLett.41.1509},
+  year    = {1978},
+  type    = {Journal Article}
+}
```

### Comparing `erlab-2.1.3/docs/source/user-guide/index.rst` & `erlab-2.2/docs/source/user-guide/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
    :caption: Table of Contents
    :maxdepth: 2
 
    io
    indexing
    plotting
    kconv
+   curve-fitting
 
 Further reading
 ===============
 
 - `Lectures on scientific computing with Python
   <https://github.com/jrjohansson/scientific-python-lectures>`_
 - `The beginner's guide to numpy
```

### Comparing `erlab-2.1.3/docs/source/user-guide/indexing.ipynb` & `erlab-2.2/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/user-guide/io.ipynb` & `erlab-2.2/docs/source/user-guide/io.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990961113977754%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(16, '\\n'), (17, 'Reading data\\n'), (18, "*

 * *            "'------------\\n'), (19, '\\n'), (20, 'Python has a wide range of libraries to read "*

 * *            "and write data. Here, we will focus on\\n'), (21, 'working with Igor Pro and xarray "*

 * *            "objects.\\n'), (24, '~~~~~~~~~~~~~\\n')], delete: [18]}}, 1: {'source': {insert: [(1, "*

 * *            "'~~~~~~~~~~~~~~~~~~~~~~\\n')], delete: [1]}}, 2: {'source': {insert: [(18, 'To Igor "*

 * *            "Pro\\n'), (19, '~~ […]*

```diff
@@ -27,16 +27,22 @@
                 "\n",
                 "This guide will introduce you to reading and writing data from and to various file\n",
                 "formats, and how to implement a custom reader for a experimental setup.\n",
                 "\n",
                 "Skip to the `corresponding section <#Loading-ARPES-data>`_ for guides on loading ARPES\n",
                 "data.\n",
                 "\n",
+                "Reading data\n",
+                "------------\n",
+                "\n",
+                "Python has a wide range of libraries to read and write data. Here, we will focus on\n",
+                "working with Igor Pro and xarray objects.\n",
+                "\n",
                 "From Igor Pro\n",
-                "-------------\n",
+                "~~~~~~~~~~~~~\n",
                 "\n",
                 ".. warning::\n",
                 "\n",
                 "   Loading waves from complex ``.pxp`` files may fail or produce unexpected results. It\n",
                 "   is recommended to export the waves to a ``.ibw`` file to load them in ERLabPy. If you\n",
                 "   encounter any problems, please let us know by opening an issue.\n",
                 "\n",
@@ -77,15 +83,15 @@
                 "tags": [],
                 "vscode": {
                     "languageId": "raw"
                 }
             },
             "source": [
                 "From arbitrary formats\n",
-                "----------------------\n",
+                "~~~~~~~~~~~~~~~~~~~~~~\n",
                 "\n",
                 "Spreadsheet data can be read using :func:`pandas.read_csv` or :func:`pandas.read_excel`.\n",
                 "The resulting DataFrame can be converted to an xarray object using\n",
                 ":meth:`pandas.DataFrame.to_xarray` or :meth:`xarray.Dataset.from_dataframe`.\n",
                 "\n",
                 "For reading HDF5 files with arbitrary groups and metadata, explore each group using\n",
                 "`h5netcdf <https://h5netcdf.org/>`_. Loading into an xarray object can be done using\n",
@@ -124,23 +130,26 @@
                 "languages and are optimized for fast read and write operations.\n",
                 "\n",
                 "To save and load :mod:`xarray` objects, see the :mod:`xarray` documentation on `I/O\n",
                 "operations <https://docs.xarray.dev/en/stable/user-guide/io.html>`_. ERLabPy offers\n",
                 "convenience functions :func:`load_hdf5 <erlab.io.load_hdf5>` and :func:`save_as_hdf5\n",
                 "<erlab.io.save_as_hdf5>` for loading and saving xarray objects from and to HDF5 files.\n",
                 "\n",
-                ".. note::\n",
                 "\n",
-                "   As an experimental feature, :func:`save_as_hdf5 <erlab.io.save_as_hdf5>` can save\n",
-                "   certain :class:`xarray.DataArray`\\ s in a format that is compatible with the Igor Pro\n",
-                "   HDF5 loader. An `accompanying Igor procedure\n",
-                "   <https://github.com/kmnhan/erlabpy/blob/main/PythonInterface.ipf>`_ is available in\n",
-                "   the repository. If loading in Igor Pro fails, try saving again with all attributes\n",
-                "   removed.\n",
-                "\n"
+                "To Igor Pro\n",
+                "~~~~~~~~~~~\n",
+                "\n",
+                "As an experimental feature, :func:`save_as_hdf5 <erlab.io.save_as_hdf5>` can save\n",
+                "certain :class:`xarray.DataArray`\\ s in a format that is compatible with the Igor Pro\n",
+                "HDF5 loader. An `accompanying Igor procedure\n",
+                "<https://github.com/kmnhan/erlabpy/blob/main/PythonInterface.ipf>`_ is available in the\n",
+                "repository. If loading in Igor Pro fails, try saving again with all attributes removed.\n",
+                "\n",
+                "Alternatively, `igorwriter <https://github.com/t-onoz/igorwriter>`_ can be used to write\n",
+                "numpy arrays to ``.ibw`` and ``.itx`` files directly."
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "editable": true,
                 "raw_mimetype": "text/restructuredtext",
```

### Comparing `erlab-2.1.3/docs/source/user-guide/kconv.ipynb` & `erlab-2.2/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/docs/source/user-guide/plotting.ipynb` & `erlab-2.2/docs/source/user-guide/plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'cells'": "{3: {'source': ['First, let us generate some example data from a simple tight binding "*

 * *            "model of graphene.\\n', 'A rigid shift of 200 meV has been applied so that the Dirac "*

 * *            "cone is visible.']}, 4: {'source': {insert: [(2, 'dat = "*

 * *            "generate_data(bandshift=-0.2).T')], delete: [2]}}}"}*

```diff
@@ -63,15 +63,16 @@
                 "editable": true,
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "First, let us generate some example data from a simple tight binding model of graphene."
+                "First, let us generate some example data from a simple tight binding model of graphene.\n",
+                "A rigid shift of 200 meV has been applied so that the Dirac cone is visible."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "editable": true,
@@ -80,15 +81,15 @@
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from erlab.interactive.exampledata import generate_data\n",
                 "\n",
-                "dat = generate_data().T"
+                "dat = generate_data(bandshift=-0.2).T"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `erlab-2.1.3/environment.yml` & `erlab-2.2/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/environment_apple.yml` & `erlab-2.2/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/environment_nogit.yml` & `erlab-2.2/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/environment_nogit_mkl.yml` & `erlab-2.2/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/pyproject.toml` & `erlab-2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/accessors.py` & `erlab-2.2/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/__init__.py` & `erlab-2.2/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/correlation.py` & `erlab-2.2/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.2/src/erlab/analysis/fit/functions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 """
 
 __all__ = [
     "TINY",
     "FermiEdge2dFunction",
     "MultiPeakFunction",
     "PolynomialFunction",
+    "bcs_gap",
     "do_convolve",
     "do_convolve_y",
+    "dynes",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
     "gaussian_wh",
     "lorentzian_wh",
     "step_broad",
     "step_linbkg_broad",
@@ -32,16 +34,18 @@
 from erlab.analysis.fit.functions.dynamic import (
     FermiEdge2dFunction,
     MultiPeakFunction,
     PolynomialFunction,
 )
 from erlab.analysis.fit.functions.general import (
     TINY,
+    bcs_gap,
     do_convolve,
     do_convolve_y,
+    dynes,
     fermi_dirac,
     fermi_dirac_linbkg,
     fermi_dirac_linbkg_broad,
     gaussian_wh,
     lorentzian_wh,
     step_broad,
     step_linbkg_broad,
```

### Comparing `erlab-2.1.3/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.2/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,17 @@
         return kws
 
     def eval_peak(self, index: int, x: npt.NDArray[np.float64], **params: dict):
         return self.peak_funcs[index](
             x, **{k[3:]: v for k, v in params.items() if k.startswith(f"p{index}")}
         )
 
+    def eval_bkg(self, x: npt.NDArray[np.float64], **params: dict):
+        return params["lin_bkg"] * x + params["const_bkg"]
+
     def pre_call(
         self, x: npt.NDArray[np.float64], **params: dict
     ) -> npt.NDArray[np.float64]:
         x = np.asarray(x).copy()
         y = np.zeros_like(x)
 
         for i, func in enumerate(self.peak_funcs):
```

### Comparing `erlab-2.1.3/src/erlab/analysis/fit/minuit.py` & `erlab-2.2/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/fit/models.py` & `erlab-2.2/src/erlab/analysis/fit/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Models for fitting data."""
 
 __all__ = [
-    "ExtendedAffineBroadenedFD",
+    "BCSGapModel",
+    "DynesModel",
+    "FermiEdgeModel",
     "FermiEdge2dModel",
     "MultiPeakModel",
     "PolynomialModel",
     "StepEdgeModel",
 ]
 
 import lmfit
@@ -15,14 +17,16 @@
 import scipy.ndimage
 import xarray as xr
 
 from erlab.analysis.fit.functions import (
     FermiEdge2dFunction,
     MultiPeakFunction,
     PolynomialFunction,
+    bcs_gap,
+    dynes,
     fermi_dirac_linbkg_broad,
     step_linbkg_broad,
 )
 
 
 @numba.njit("f8[:,:](f8[:], i8)", cache=True)
 def _coeff_mat(x, deg):
@@ -96,15 +100,15 @@
         np.array(x[-len_fit:], dtype=np.float64),
         np.array(data[-len_fit:], dtype=np.float64),
         deg=1,
     )
     return n0, m0, n1, m1
 
 
-class ExtendedAffineBroadenedFD(lmfit.Model):
+class FermiEdgeModel(lmfit.Model):
     """
     Fermi-dirac function with linear background above and below the fermi level,
     convolved with a gaussian kernel.
     """
 
     @staticmethod
     def LinearBroadFermiDirac(
@@ -231,14 +235,21 @@
         super().__init__(
             MultiPeakFunction(
                 npeaks, peak_shapes=peak_shapes, fd=fd, convolve=convolve
             ),
             **kwargs,
         )
 
+        for i in range(self.func.npeaks):
+            self.set_param_hint(f"p{i}_width", min=0.0)
+            self.set_param_hint(f"p{i}_height", min=0.0)
+
+        if self.func.fd:
+            self.set_param_hint("temp", min=0.0)
+
         if self.func.convolve:
             self.set_param_hint("resolution", min=0.0)
 
     def guess(self, data, x=None, **kwargs):
         pars = self.make_params()
         # !TODO: better guesses
         if self.func.fd:
@@ -256,14 +267,37 @@
         for i in range(self.func.npeaks):  # Number of peaks
             pars[f"{self.prefix}p{i}_center"].set(value=0.0)
             pars[f"{self.prefix}p{i}_height"].set(value=data.mean())
             pars[f"{self.prefix}p{i}_width"].set(value=0.1 * xrange)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
 
+    def eval_components(self, params=None, **kwargs):
+        key = self._prefix
+        if len(key) < 1:
+            key = self._name
+
+        if params is not None:
+            kwargs = kwargs | params.valuesdict()
+
+        # Coerce into numpy arrays
+        for k in list(kwargs.keys()):
+            if np.iterable(kwargs[k]):
+                kwargs[k] = np.asarray(kwargs[k])
+
+        fargs = self.make_funcargs(params, kwargs)
+
+        out = {}
+        for i in range(self.func.npeaks):
+            out[f"{key}_p{i}"] = self.func.eval_peak(i, **fargs)
+
+        out[f"{key}_bkg"] = self.func.eval_bkg(**fargs)
+
+        return out
+
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
 
 
 class FermiEdge2dModel(lmfit.Model):
     r"""A 2D model for a polynomial Fermi edge with a linear density of states.
 
     The model function can be written as
@@ -312,7 +346,27 @@
         if isinstance(data, xr.DataArray):
             data = data.transpose("eV", "alpha").values
         # Ensure flat fit
         return super().fit(data.ravel(), *args, **kwargs)
 
     __init__.__doc__ = lmfit.models.COMMON_INIT_DOC.replace("['x']", "['eV', 'alpha']")
     guess.__doc__ = lmfit.models.COMMON_GUESS_DOC
+
+
+class BCSGapModel(lmfit.Model):
+    def __init__(self, **kwargs):
+        super().__init__(bcs_gap, **kwargs)
+        self.set_param_hint("a", min=0.0)
+        self.set_param_hint("tc", min=0.0)
+
+    __doc__ = bcs_gap.__doc__
+    __init__.doc = lmfit.models.COMMON_INIT_DOC
+
+
+class DynesModel(lmfit.Model):
+    def __init__(self, **kwargs):
+        super().__init__(dynes, **kwargs)
+        self.set_param_hint("gamma", min=0.0)
+        self.set_param_hint("delta", min=0.0)
+
+    __doc__ = dynes.__doc__
+    __init__.doc = lmfit.models.COMMON_INIT_DOC
```

### Comparing `erlab-2.1.3/src/erlab/analysis/fit/spline.py` & `erlab-2.2/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/gold.py` & `erlab-2.2/src/erlab/analysis/gold.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import numpy as np
 import numpy.typing as npt
 import scipy.interpolate
 import uncertainties
 import xarray as xr
 
 from erlab.analysis.fit.models import (
-    ExtendedAffineBroadenedFD,
+    FermiEdgeModel,
     PolynomialModel,
     StepEdgeModel,
 )
 from erlab.analysis.utilities import correct_with_edge
 from erlab.parallel import joblib_progress
 from erlab.plotting.general import autoscale_to, figwh
 
@@ -103,15 +103,15 @@
     if fast:
         params = lmfit.create_params()
         model_cls = StepEdgeModel
     else:
         if temp is None:
             temp = gold.attrs["temp_sample"]
         params = lmfit.create_params(temp={"value": temp, "vary": vary_temp})
-        model_cls = ExtendedAffineBroadenedFD
+        model_cls = FermiEdgeModel
 
     model = model_cls()
 
     if parallel_kw is None:
         parallel_kw = {}
 
     if fixed_center is not None:
@@ -435,17 +435,17 @@
     gold_roi = gold_corr.sel(alpha=slice(*angle_range))
     edc_avg = gold_roi.mean("alpha").sel(eV=slice(*eV_range_fit))
 
     params = lmfit.create_params(
         temp={"value": gold_roi.attrs["temp_sample"], "vary": False},
         resolution={"value": 0.1, "vary": True, "min": 0},
     )
-    model = ExtendedAffineBroadenedFD()
+    model = FermiEdgeModel()
     params = model.guess(edc_avg, x=edc_avg["eV"]).update(params)
-    fit = ExtendedAffineBroadenedFD().fit(
+    fit = FermiEdgeModel().fit(
         edc_avg, x=edc_avg["eV"], params=params, method=method, scale_covar=scale_covar
     )
     if plot:
         plt.show()
         ax = plt.gca()
         gold_corr.qplot(ax=ax, cmap="copper", gamma=0.5)
         rect = mpatches.Rectangle(
@@ -483,15 +483,15 @@
 ) -> lmfit.model.ModelResult:
     edc_avg = gold_roi.mean("alpha").sel(eV=slice(*eV_range))
 
     params = lmfit.create_params(
         temp={"value": gold_roi.attrs["temp_sample"], "vary": not fix_temperature},
         resolution={"value": 0.1, "vary": True, "min": 0},
     )
-    model = ExtendedAffineBroadenedFD()
+    model = FermiEdgeModel()
     params = model.guess(edc_avg, x=edc_avg["eV"]).update(params)
     fit = model.fit(
         edc_avg,
         x=edc_avg["eV"],
         params=params,
         method=method,
         scale_covar=scale_covar,  # weights=1 / edc_stderr
```

### Comparing `erlab-2.1.3/src/erlab/analysis/image.py` & `erlab-2.2/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/interpolate.py` & `erlab-2.2/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/kspace.py` & `erlab-2.2/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/mask/__init__.py` & `erlab-2.2/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/mask/polygon.py` & `erlab-2.2/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/transform.py` & `erlab-2.2/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/analysis/utilities.py` & `erlab-2.2/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/characterization/resistance.py` & `erlab-2.2/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/characterization/xrd.py` & `erlab-2.2/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/constants.py` & `erlab-2.2/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/__init__.py` & `erlab-2.2/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/bzplot.py` & `erlab-2.2/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/colors.py` & `erlab-2.2/src/erlab/interactive/colors.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,35 @@
 
 import matplotlib.colors as mcolors
 import numpy as np
 import numpy.typing as npt
 import pyqtgraph as pg
 from qtpy import QtCore, QtGui, QtWidgets
 
+EXCLUDED_CMAPS: tuple[str, ...] = (
+    "prism",
+    "tab10",
+    "tab20",
+    "tab20b",
+    "tab20c",
+    "flag",
+    "Set1",
+    "Set2",
+    "Set3",
+    "Pastel1",
+    "Pastel2",
+    "Pastel3",
+    "Paired",
+    "Dark2",
+)
+"""
+Colormaps to exclude from the list of available colormaps. They are not suitable for
+continuous data, and looks horrible.
+"""
+
 
 class ColorMapComboBox(QtWidgets.QComboBox):
     LOAD_ALL_TEXT = "Load all..."
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.setPlaceholderText("Select colormap...")
@@ -545,29 +566,33 @@
     """
     local = sorted(pg.colormap.listMaps())
     if source == "local":
         return local
     else:
         _mpl = sorted(pg.colormap.listMaps(source="matplotlib"))
         for cmap in _mpl:
-            if cmap.startswith("cet_"):
-                _mpl = list(filter((cmap).__ne__, _mpl))
-            elif cmap.endswith("_r"):
-                # _mpl_r.append(cmap)
+            if (
+                cmap.startswith("cet_")
+                or cmap.endswith(("_r", "_r_i"))
+                or cmap in EXCLUDED_CMAPS
+            ):
                 _mpl = list(filter((cmap).__ne__, _mpl))
         if source == "all":
             cet = sorted(pg.colormap.listMaps(source="colorcet"))
+            for cmap in cet:
+                if cmap.startswith("glasbey"):
+                    cet = list(filter((cmap).__ne__, cet))
+
             # if (_mpl != []) and (cet != []):
             # local = []
-            # _mpl_r = []
 
             if exclude_local:
                 all_cmaps = cet + _mpl
             else:
-                all_cmaps = local + cet + _mpl  # + _mpl_r
+                all_cmaps = local + cet + _mpl
         elif exclude_local:
             all_cmaps = _mpl
         else:
             all_cmaps = local + _mpl
     return list(dict.fromkeys(all_cmaps))
```

### Comparing `erlab-2.1.3/src/erlab/interactive/curvefittingtool.py` & `erlab-2.2/src/erlab/interactive/curvefittingtool.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 import lmfit
 import pyqtgraph as pg
 import xarray as xr
 from qtpy import QtCore, QtWidgets
 
-from erlab.analysis.fit import MultiPeakModel
+from erlab.analysis.fit.models import MultiPeakModel
 from erlab.interactive.utilities import FittingParameterWidget, ParameterGroup
 
 # EDCmultiFitting Igor procedure - 2D wave EDC fit along momentum range
 
 # Momentum range to fit
 # Number of bands
 # Initial parameters
@@ -112,14 +112,18 @@
         self.update()
 
     def setPen(self, *args, **kargs):
         super().setPen(*args, **kargs)
         self._pen_color = self.opts["pen"].color()
         self._pen_width = self.opts["pen"].width()
 
+    def viewRangeChanged(self):
+        super().viewRangeChanged()
+        self._mouseShape = None
+
     def setMouseHover(self, hover):
         # Inform the item that the mouse is (not) hovering over it
         # if self.mouseHovering == hover:
         # return
         # self.mouseHovering = hover
         if hover:
             self.setTempPen(self._pen_color, width=2 * self._pen_width)
@@ -133,14 +137,19 @@
     def __init__(
         self, param_widget: SinglePeakWidget, curve: PlotPeakItem, *args, **kargs
     ):
         self.param_widget = param_widget
         self.curve = curve
         super().__init__(*args, movable=True, **kargs)
 
+        self.addMarker("o", -0.5)
+
+    def boundingRect(self):
+        return super().boundingRect()
+
     def mouseDragEvent(self, ev):
         if not self.movable:
             ev.ignore()
             return
         if ev.button() == QtCore.Qt.MouseButton.LeftButton:
             if ev.isStart():
                 self.moving = True
@@ -158,15 +167,15 @@
             self.param_widget.widgets["center"].setValue(pos.x())
             self.param_widget.widgets["height"].setValue(
                 self._start_height + self.mapToParent(ev.pos() - ev.buttonDownPos()).y()
             )
 
         elif QtCore.Qt.MouseButton.RightButton in ev.buttons():
             if ev.isStart():
-                self._start_width = self.param_widgÏet.widgets["width"].value()
+                self._start_width = self.param_widget.widgets["width"].value()
             ev.accept()
 
             val = self.mapToParent(ev.buttonDownPos() - ev.pos()).y()
             y0, _, y1, _ = self.boundingRect().getCoords()
             amount = val / abs(y1 - y0)
             self.param_widget.widgets["width"].setValue(self._start_width + amount)
         if ev.isFinish():
@@ -246,15 +255,15 @@
                 "spin_kw": {"value": 30, "minimum": 0, "minimumWidth": 200},
             },
             efermi={
                 "qwtype": "fitparam",
                 "showlabel": "Fermi Level",
                 "name": "efermi",
                 "fixed": True,
-                "spin_kw": {"value": 0, "minimum": 0, "minimumWidth": 200},
+                "spin_kw": {"value": 0, "minimumWidth": 200},
             },
             Method={"qwtype": "combobox", "items": LMFIT_METHODS},
             go={
                 "qwtype": "pushbtn",
                 "showlabel": False,
                 "text": "Go",
                 "clicked": self.do_fit,
@@ -337,14 +346,16 @@
             self.n_bands,
             peak_shapes=[
                 self._params_peak.widget(i).peak_shape for i in range(self.n_bands)
             ],
         )
 
     def refresh_n_peaks(self):
+        if not hasattr(self, "_params_peak"):
+            return
         current = int(self._params_peak.count())
         if self.n_bands > current:
             while self.n_bands > self._params_peak.count():
                 self._params_peak.addTab(SinglePeakWidget(current), f"Peak {current}")
                 self._params_peak.widget(current).sigParameterChanged.connect(
                     self._refresh_plot_peaks
                 )
@@ -571,14 +582,16 @@
             peak_shapes=[
                 self._params_peak.widget(i).peak_shape for i in range(self.n_bands)
             ],
             fd=False,
         )
 
     def refresh_n_peaks(self):
+        if not hasattr(self, "_params_peak"):
+            return
         current = int(self._params_peak.count())
         if self.n_bands > current:
             while self.n_bands > self._params_peak.count():
                 self._params_peak.addTab(SinglePeakWidget(current), f"Peak {current}")
                 self._params_peak.widget(current).sigParameterChanged.connect(
                     self._refresh_plot_peaks
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `erlab-2.1.3/src/erlab/interactive/derivative.py` & `erlab-2.2/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/dtool.ui` & `erlab-2.2/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/exampledata.py` & `erlab-2.2/src/erlab/interactive/exampledata.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 def generate_data(
     shape: tuple[int, int, int] = (250, 250, 300),
     krange: float | tuple[float, float] | dict[str, tuple[float, float]] = 0.89,
     Erange: tuple[float, float] = (-0.45, 0.09),
     temp: float = 20.0,
     a: float = 6.97,
     t: float = 0.43,
-    bandshift: float = -0.2,
+    bandshift: float = 0.0,
     Sreal: float = 0.0,
     Simag: float = 0.03,
     kres: float = 0.01,
     Eres: float = 2.0e-3,
     noise: bool = True,
     count: int = 10000,
     ccd_sigma: float = 0.6,
@@ -73,15 +73,15 @@
         The temperature in Kelvins for the Fermi-Dirac cutoff. If 0, no cutoff is
         applied, by default 20.0
     a
         Tight binding parameter :math:`a`, by default 6.97
     t
         Tight binding parameter :math:`t`, by default 0.43
     bandshift
-        The rigid energy shift in eV, by default -0.2
+        The rigid energy shift in eV, by default 0.0
     Sreal
         The real part of the self energy, by default 0.0
     Simag
         The imaginary part of the self energy, by default 0.03
     kres
         Broadening in momentum in inverse angstroms, by default 0.01
     Eres
@@ -152,15 +152,15 @@
     hv: float = 50.0,
     configuration: (
         erlab.analysis.kspace.AxesConfiguration | int
     ) = erlab.analysis.kspace.AxesConfiguration.Type1,
     temp: float = 20.0,
     a: float = 6.97,
     t: float = 0.43,
-    bandshift: float = -0.2,
+    bandshift: float = 0.0,
     Sreal: float = 0.0,
     Simag: float = 0.03,
     angres: float = 0.1,
     Eres: float = 10.0e-3,
     noise: bool = True,
     count: int = 10000,
     ccd_sigma: float = 0.6,
@@ -187,15 +187,15 @@
         The temperature in Kelvins for the Fermi-Dirac cutoff. If 0, no cutoff is
         applied, by default 20.0
     a
         Tight binding parameter :math:`a`, by default 6.97
     t
         Tight binding parameter :math:`t`, by default 0.43
     bandshift
-        The rigid energy shift in eV, by default -0.2
+        The rigid energy shift in eV, by default 0.0
     Sreal
         The real part of the self energy, by default 0.0
     Simag
         The imaginary part of the self energy, by default 0.03
     angres
         Broadening in angle in degrees, by default 0.01
     Eres
```

### Comparing `erlab-2.1.3/src/erlab/interactive/fermiedge.py` & `erlab-2.2/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.2/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/controls.py` & `erlab-2.2/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/core.py` & `erlab-2.2/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.2/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.2/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/kspace.py` & `erlab-2.2/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/ktool.ui` & `erlab-2.2/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/masktool.py` & `erlab-2.2/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/interactive/utilities.py` & `erlab-2.2/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/__init__.py` & `erlab-2.2/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/dataloader.py` & `erlab-2.2/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/igor.py` & `erlab-2.2/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/plugins/__init__.py` & `erlab-2.2/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/plugins/da30.py` & `erlab-2.2/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/plugins/kriss.py` & `erlab-2.2/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/plugins/merlin.py` & `erlab-2.2/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/plugins/ssrl52.py` & `erlab-2.2/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/io/utilities.py` & `erlab-2.2/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/lattice.py` & `erlab-2.2/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/parallel.py` & `erlab-2.2/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.2/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/__init__.py` & `erlab-2.2/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/annotations.py` & `erlab-2.2/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/atoms.py` & `erlab-2.2/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/bz.py` & `erlab-2.2/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/colors.py` & `erlab-2.2/src/erlab/plotting/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "CenteredPowerNorm",
     "InversePowerNorm",
     "TwoSlopeInversePowerNorm",
     "TwoSlopePowerNorm",
     "axes_textcolor",
     "close_to_white",
     "color_distance",
+    "combined_cmap",
     "flatten_transparency",
     "gen_2d_colormap",
     "get_mappable",
     "image_is_light",
     "nice_colorbar",
     "prominent_color",
     "proportional_colorbar",
@@ -46,21 +47,25 @@
 
 from collections.abc import Iterable, Sequence
 from numbers import Number
 from typing import Literal
 
 import matplotlib
 import matplotlib.axes
-import matplotlib.colors as mcolors
+import matplotlib.cm
+import matplotlib.collections
+import matplotlib.colors
+import matplotlib.image
 import matplotlib.pyplot as plt
-import matplotlib.transforms as mtransforms
+import matplotlib.transforms
 import numpy as np
+import numpy.typing as npt
 
 
-class InversePowerNorm(mcolors.Normalize):
+class InversePowerNorm(matplotlib.colors.Normalize):
     r"""
     Linearly map a given value to the 0-1 range and then apply an inverse power-law
     normalization over that range.
 
     For values :math:`x`, `matplotlib.colors.PowerNorm` calculates
     :math:`x^\gamma`, whereas `InversePowerNorm` calculates :math:`1-x^{1/\gamma}`.
     This provides higher contrast for values closer to ``vmin``.
@@ -224,15 +229,15 @@
         return np.ma.asarray(val_)
     elif value < 0.5:
         return pow(2 * value, gamma) * (vcenter - vcenter) + vmin
     else:
         return pow(2 - 2 * value, gamma) * (vcenter - vmax) + vmax
 
 
-class TwoSlopePowerNorm(mcolors.TwoSlopeNorm):
+class TwoSlopePowerNorm(matplotlib.colors.TwoSlopeNorm):
     r"""Power-law normalization of data with a set center.
 
     Useful when mapping data with an unequal rates of change around a
     conceptual center, e.g., data that range from -2 to 4, with 0 as
     the midpoint.
 
     Parameters
@@ -288,15 +293,15 @@
         gamma = self.gamma
         (vmin,), _ = self.process_value(self.vmin)
         (vmax,), _ = self.process_value(self.vmax)
         (vcenter,), _ = self.process_value(self.vcenter)
         return self._func_i(value, gamma, vmin, vmax, vcenter)
 
 
-class CenteredPowerNorm(mcolors.CenteredNorm):
+class CenteredPowerNorm(matplotlib.colors.CenteredNorm):
     r"""Power-law normalization of symmetrical data around a center.
 
     Unlike `TwoSlopePowerNorm`, `CenteredPowerNorm` applies an equal rate of
     change around the center.
 
     Useful when mapping symmetrical data around a conceptual center e.g., data that
     range from -2 to 4, with 0 as the midpoint, and with equal rates of change
@@ -489,25 +494,45 @@
             "creation. First define a mappable such as "
             "an image (with imshow) or a contour set ("
             "with contourf)."
         )
     return mappable
 
 
-def unify_clim(axes, target=None, image_only: bool = False):
+def unify_clim(
+    axes: np.ndarray,
+    target: matplotlib.axes.Axes | None = None,
+    image_only: bool = False,
+) -> None:
+    """Unify the color limits for mappables in multiple axes.
+
+    Parameters
+    ----------
+    axes
+        Array of :class:`matplotlib.axes.Axes` to unify the color limits.
+    target
+        The target axis to unify the color limits. If provided, the target color limits
+        will be taken from this axes. Otherwise, the color limits will be set to include
+        all mappables in the ``axes``.
+    image_only
+        If `True`, only consider mappables that are images. Default is `False`.
+
+    """
     if target is None:
         vmn, vmx = [], []
         for ax in axes.flat:
             mappable = get_mappable(ax, image_only=image_only)
             vmn.append(mappable.norm.vmin)
             vmx.append(mappable.norm.vmax)
         vmn, vmx = min(vmn), max(vmx)
+
     else:
         mappable = get_mappable(target, image_only=image_only)
         vmn, vmx = mappable.norm.vmin, mappable.norm.vmax
+
     for ax in axes.flat:
         mappable = get_mappable(ax, image_only=image_only)
         mappable.norm.vmin, mappable.norm.vmax = vmn, vmx
 
 
 def proportional_colorbar(
     mappable: matplotlib.cm.ScalarMappable | None = None,
@@ -544,23 +569,23 @@
 
     Examples
     --------
     ::
 
         import numpy as np
         import matplotlib.pyplot as plt
-        import matplotlib.colors as colors
+        import matplotlib.colors
 
         # Create example data and plot
         X, Y = np.mgrid[0 : 3 : complex(0, 100), 0 : 2 : complex(0, 100)]
         pcm = plt.pcolormesh(
             X,
             Y,
             (1 + np.sin(Y * 10.0)) * X**2,
-            norm=mcolors.PowerNorm(gamma=0.5),
+            norm=matplotlib.colors.PowerNorm(gamma=0.5),
             cmap="Blues_r",
             shading="auto",
         )
 
         # Plot evenly spaced colorbar
         proportional_colorbar()
 
@@ -705,18 +730,20 @@
         self._transAxes = ax.transAxes
         self._width = width
         self._height = height
         self._loc = loc
         self.set_pad(pad)
 
     def __call__(self, ax, renderer):
-        return mtransforms.TransformedBbox(
-            mtransforms.Bbox.from_bounds(*self._size_to_bounds(ax)),
+        return matplotlib.transforms.TransformedBbox(
+            matplotlib.transforms.Bbox.from_bounds(*self._size_to_bounds(ax)),
             self._transAxes
-            + mtransforms.ScaledTranslation(*self.pads, ax.figure.dpi_scale_trans)
+            + matplotlib.transforms.ScaledTranslation(
+                *self.pads, ax.figure.dpi_scale_trans
+            )
             - ax.figure.transSubfigure,
         )
 
     def set_pad(self, pad):
         pad_num = False
         if isinstance(pad, Number):
             pad_num = True
@@ -844,15 +871,15 @@
             cax=_gen_cax(parent, width, aspect, pad, is_horizontal),
             orientation=orientation,
             **kwargs,
         )
 
     else:
         if np.iterable(ax):
-            bbox = mtransforms.Bbox.union(
+            bbox = matplotlib.transforms.Bbox.union(
                 [
                     x.get_window_extent().transformed(
                         x.figure.dpi_scale_trans.inverted()
                     )
                     for x in ax.flat
                 ]
             )
@@ -897,42 +924,80 @@
         cbar.ax.set_box_aspect(1 / aspect)
     else:
         cbar.ax.set_box_aspect(aspect)
 
     return cbar
 
 
-def flatten_transparency(rgba, background: Sequence[float] | None = None):
+def flatten_transparency(rgba: npt.NDArray, background: Sequence[float] | None = None):
+    """
+    Flatten the transparency of an RGBA image by blending it with a background color.
+
+    Parameters
+    ----------
+    rgba
+        The input RGBA image as a numpy array.
+    background
+        The background color to blend with. Defaults to white ``(1, 1, 1)``.
+
+    """
     if background is None:
         background = (1, 1, 1)
     original_shape = rgba.shape
     rgba = rgba.reshape(-1, 4)
     rgb = rgba[:, :-1]
     a = rgba[:, -1][:, np.newaxis]
     rgb *= a
     rgb += (1 - a) * background
     return rgb.reshape(original_shape[:-1] + (3,))
 
 
-def _is_segment_iterable(cmap: mcolors.Colormap) -> bool:
-    if not isinstance(cmap, mcolors.LinearSegmentedColormap):
+def _is_segment_iterable(cmap: matplotlib.colors.Colormap) -> bool:
+    if not isinstance(cmap, matplotlib.colors.LinearSegmentedColormap):
         return False
     if any(callable(cmap._segmentdata[c]) for c in ["red", "green", "blue"]):
         return False
     return True
 
 
 def combined_cmap(
-    cmap1: mcolors.Colormap | str,
-    cmap2: mcolors.Colormap | str,
+    cmap1: matplotlib.colors.Colormap | str,
+    cmap2: matplotlib.colors.Colormap | str,
     name: str,
     register: bool = False,
     N=256,
-):
-    """Stitch two existing colormaps to create a new colormap."""
+) -> matplotlib.colors.Colormap:
+    """Stitch two existing colormaps to create a new colormap.
+
+    This was implemented before :func:`cmasher.combine_cmaps` existed. Using that might
+    be better.
+
+    Parameters
+    ----------
+    cmap1
+        The first colormap to be combined. Can be either a
+        :class:`matplotlib.colors.Colormap` or a string representing the name of a
+        registered colormap.
+    cmap2
+        The second colormap to be combined. Can be either a
+        :class:`matplotlib.colors.Colormap` or a string representing the name of a
+        registered colormap.
+    name
+        The name of the combined colormap.
+    register
+        Whether to register the combined colormap. Defaults to `False`.
+    N
+        The number of colors in the resulting colormap. Defaults to 256.
+
+    Returns
+    -------
+    matplotlib.colors.Colormap
+        The combined colormap.
+
+    """
     if isinstance(cmap1, str):
         cmap1 = matplotlib.colormaps[cmap1]
     if isinstance(cmap2, str):
         cmap2 = matplotlib.colormaps[cmap2]
 
     if all(_is_segment_iterable(c) for c in (cmap1, cmap2)):
         segnew = {}
@@ -940,17 +1005,19 @@
             seg1_c, seg2_c = (
                 np.asarray(cmap1._segmentdata[c]),
                 np.asarray(cmap2._segmentdata[c]),
             )
             seg1_c[:, 0] = seg1_c[:, 0] * 0.5
             seg2_c[:, 0] = seg2_c[:, 0] * 0.5 + 0.5
             segnew[c] = np.r_[seg1_c, seg2_c]
-        cmap = mcolors.LinearSegmentedColormap(name=name, segmentdata=segnew, N=N)
+        cmap = matplotlib.colors.LinearSegmentedColormap(
+            name=name, segmentdata=segnew, N=N
+        )
     else:
-        cmap = mcolors.LinearSegmentedColormap.from_list(
+        cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
             name=name,
             colors=np.r_[
                 cmap1(np.linspace(0, 1, int(N / 2))),
                 cmap2(np.linspace(0, 1, int(N / 2))),
             ],
         )
     if register:
@@ -958,88 +1025,181 @@
         matplotlib.colormaps.register(cmap.reversed())
     return cmap
 
 
 def gen_2d_colormap(
     ldat,
     cdat,
-    cmap: mcolors.Colormap | str = None,
-    colorbar: bool = True,
+    cmap: matplotlib.colors.Colormap | str = None,
     *,
     lnorm: plt.Normalize | None = None,
     cnorm: plt.Normalize | None = None,
     background: Sequence[float] | None = None,
     N: int = 256,
 ):
+    """Generate a 2D colormap image from lightness and color data.
+
+    Parameters
+    ----------
+    ldat : array-like
+        The lightness data.
+    cdat : array-like
+        The color data. Must have the same shape as `ldat`.
+    cmap
+        The colormap to use for the color axis. If `None`, a predefined linear segmented
+        colormap is used.
+    lnorm
+        The normalization for the lightness axes.
+    cnorm
+        The normalization for the color axes.
+    background
+        The background color. If `None`, it is set to white.
+    N
+        The number of levels in the colormap. Default is 256. The resulting colormap
+        will have a shape of ``(N, N, 4)``, where the last dimension represents the RGBA
+        values.
+
+    Returns
+    -------
+    cmap_img : array-like
+        RGBA image of the colormap.
+    img : array-like
+        RGBA image with the 2D colormap applied.
+
+    """
     if cmap is None:
-        cmap = mcolors.LinearSegmentedColormap.from_list(
+        cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
             "", colors=[[0, 0, 1], [0, 0, 0], [1, 0, 0]], N=N
         )
+
     elif isinstance(cmap, str):
         cmap = plt.get_cmap(cmap)
+
     if lnorm is None:
         lnorm = plt.Normalize()
+
     if cnorm is None:
         cnorm = plt.Normalize()
+
     if background is None:
         background = (1, 1, 1)
 
     lnorm.autoscale_None(ldat)
     cnorm.autoscale_None(cdat)
 
     l_vals = lnorm(ldat)[:, :, np.newaxis]
     img = cmap(cnorm(cdat))[:, :, :-1]
     img *= l_vals
     img += (1 - l_vals) * background
+    l_vals = lnorm(np.linspace(lnorm.vmin, lnorm.vmax, N))[:, np.newaxis, np.newaxis]
+    cmap_img = np.repeat(
+        cmap(cnorm(np.linspace(cnorm.vmin, cnorm.vmax, N)))[np.newaxis, :], N, 0
+    )[:, :, :-1]
+    cmap_img *= l_vals
+    cmap_img += (1 - l_vals) * background
 
-    if colorbar:
-        l_vals = lnorm(np.linspace(lnorm.vmin, lnorm.vmax, N))[
-            :, np.newaxis, np.newaxis
-        ]
-        cmap_img = np.repeat(
-            cmap(cnorm(np.linspace(cnorm.vmin, cnorm.vmax, N)))[np.newaxis, :], N, 0
-        )[:, :, :-1]
-        cmap_img *= l_vals
-        cmap_img += (1 - l_vals) * background
-        return cmap_img, img
-    else:
-        return None, img
+    return cmap_img, img
+
+
+def color_distance(c1, c2) -> float:
+    """Calculate the color distance between two RGB colors.
+
+    Parameters
+    ----------
+    c1, c2
+        Color to calculate the distance between in any format that
+        :func:`matplotlib.colors.to_rgb` can handle.
 
+    Returns
+    -------
+    float
+        The color distance between the two colors.
 
-def color_distance(c1, c2):
-    # https://www.compuphase.com/cmetric.htm
-    R1, G1, B1 = (np.array(mcolors.to_rgb(c1)) * 255).astype(int)
-    R2, G2, B2 = (np.array(mcolors.to_rgb(c2)) * 255).astype(int)
+    Note
+    ----
+    The color distance is calculated using the Euclidean distance formula in the RGB
+    color space. The formula takes into account the perceptual differences between
+    colors.
+
+    See Also
+    --------
+    - https://www.compuphase.com/cmetric.htm
+
+    """
+    R1, G1, B1 = (np.array(matplotlib.colors.to_rgb(c1)) * 255).astype(int)
+    R2, G2, B2 = (np.array(matplotlib.colors.to_rgb(c2)) * 255).astype(int)
     dR2 = (R2 - R1) ** 2
     dG2 = (G2 - G1) ** 2
     dB2 = (B2 - B1) ** 2
     r = 0.5 * (R1 + R2) / 256
     return np.sqrt((2 + r) * dR2 + 4 * dG2 + (2 + 255 / 256 - r) * dB2)
 
 
-def close_to_white(c):
+def close_to_white(c) -> bool:
+    """Check if a given color is closer to white than black.
+
+    Parameters
+    ----------
+    c
+        Color in any format that :func:`matplotlib.colors.to_rgb` can handle.
+
+    Returns
+    -------
+    bool
+        `True` if the color is closer to white than black, `False` otherwise.
+    """
     c2k = color_distance(c, (0, 0, 0))
     c2w = color_distance(c, (1, 1, 1))
     return bool(c2k > c2w)
 
 
-def prominent_color(im):
+def prominent_color(im: matplotlib.image._ImageBase | matplotlib.collections.QuadMesh):
+    """Calculate the prominent color of an image.
+
+    This function calculates the prominent color of an image by finding the most
+    frequent color in the image's histogram in color space. If the image array is
+    `None`, returns white.
+
+    """
     im_array = im.get_array()
     if im_array is None:
-        return mcolors.to_rgba("w")
+        return matplotlib.colors.to_rgba("w")
     hist, edges = np.histogram(np.nan_to_num(im_array), "auto")
     mx = hist.argmax()
     return im.to_rgba(edges[mx : mx + 2].mean())
 
 
-def image_is_light(im):
+def image_is_light(
+    im: matplotlib.image._ImageBase | matplotlib.collections.QuadMesh,
+) -> bool:
+    """
+    Determines if an image is *light* or *dark* by checking whether the prominent color
+    is closer to white than black.
+
+    """
     return close_to_white(prominent_color(im))
 
 
-def axes_textcolor(ax, light="k", dark="w"):
+def axes_textcolor(ax: matplotlib.axes.Axes, light="k", dark="w"):
+    """Determine the text color based on the color of the mappable in an axes.
+
+    Parameters
+    ----------
+    ax
+        The axes object for which the text color needs to be determined.
+    light
+        The *light* color, returned when :func:`image_is_light
+        <erlab.plotting.colors.image_is_light>` returns `False`. Default is ``'w'``
+        (white).
+    dark
+        The *dark* color, returned when :func:`image_is_light
+        <erlab.plotting.colors.image_is_light>` returns `True`. Default is ``'k'``
+        (black).
+
+    """
     c = light
     mappable = get_mappable(ax, silent=True)
     if mappable is not None:
         if isinstance(
             mappable, matplotlib.image._ImageBase | matplotlib.collections.QuadMesh
         ):
             if not image_is_light(mappable):
```

### Comparing `erlab-2.1.3/src/erlab/plotting/erplot.py` & `erlab-2.2/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/general.py` & `erlab-2.2/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/plot3d.py` & `erlab-2.2/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.2/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/src/erlab.egg-info/PKG-INFO` & `erlab-2.2/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.1.3
+Version: 2.2.0
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-2.1.3/src/erlab.egg-info/SOURCES.txt` & `erlab-2.2/src/erlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 docs/source/images/imagetool_dark.png
 docs/source/images/imagetool_light.png
 docs/source/images/ktool_1_dark.png
 docs/source/images/ktool_1_light.png
 docs/source/images/ktool_2_dark.png
 docs/source/images/ktool_2_light.png
 docs/source/pyplots/norms.py
+docs/source/user-guide/curve-fitting.ipynb
 docs/source/user-guide/index.rst
 docs/source/user-guide/indexing.ipynb
 docs/source/user-guide/io.ipynb
 docs/source/user-guide/kconv.ipynb
 docs/source/user-guide/plotting.ipynb
 src/erlab/__init__.py
 src/erlab/accessors.py
```

### Comparing `erlab-2.1.3/src/erlab.egg-info/requires.txt` & `erlab-2.2/src/erlab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/templates/.macros.j2` & `erlab-2.2/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_fastbinning.py` & `erlab-2.2/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.2/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_fit_functions_general.py` & `erlab-2.2/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_image.py` & `erlab-2.2/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_interpolate.py` & `erlab-2.2/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_kspace.py` & `erlab-2.2/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.1.3/tests/analysis/test_utilities.py` & `erlab-2.2/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

