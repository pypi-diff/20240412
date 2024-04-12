# Comparing `tmp/tad_mctc-0.1.1.tar.gz` & `tmp/tad_mctc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_mctc-0.1.1.tar", last modified: Fri Mar 29 21:34:21 2024, max compression
+gzip compressed data, was "tad_mctc-0.1.2.tar", last modified: Fri Apr 12 11:37:11 2024, max compression
```

## Comparing `tad_mctc-0.1.1.tar` & `tad_mctc-0.1.2.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.098591 tad_mctc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-03-29 21:34:21.098591 tad_mctc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-29 21:34:21.098591 tad_mctc-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.078591 tad_mctc-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.082591 tad_mctc-0.1.1/src/tad_mctc/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.082591 tad_mctc-0.1.1/src/tad_mctc/autograd/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/batched.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/autograd/internals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.086591 tad_mctc-0.1.1/src/tad_mctc/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/batch/agnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/batch/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/batch/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/batch/unpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.086591 tad_mctc-0.1.1/src/tad_mctc/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/convert/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/convert/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/convert/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/convert/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.086591 tad_mctc-0.1.1/src/tad_mctc/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/en.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    69463 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/radii.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/data/zeff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.086591 tad_mctc-0.1.1/src/tad_mctc/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/exceptions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/exceptions/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/exceptions/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.086591 tad_mctc-0.1.1/src/tad_mctc/io/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.090591 tad_mctc-0.1.1/src/tad_mctc/io/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/checks/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/checks/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.090591 tad_mctc-0.1.1/src/tad_mctc/io/read/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/dotfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/frompath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/orca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/tblite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/turbomole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/read/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.090591 tad_mctc-0.1.1/src/tad_mctc/io/write/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/write/turbomole.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/write/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/io/write/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.090591 tad_mctc-0.1.1/src/tad_mctc/math/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/math/einsum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.090591 tad_mctc-0.1.1/src/tad_mctc/molecule/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/molecule/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/molecule/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/molecule/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.094591 tad_mctc-0.1.1/src/tad_mctc/ncoord/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/d3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/d4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/ncoord/eeq.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.094591 tad_mctc-0.1.1/src/tad_mctc/storch/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/storch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/storch/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/storch/elemental.py
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/storch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/storch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.094591 tad_mctc-0.1.1/src/tad_mctc/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/typing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/typing/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/typing/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.094591 tad_mctc-0.1.1/src/tad_mctc/units/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/codata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-29 21:34:16.000000 tad_mctc-0.1.1/src/tad_mctc/units/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 21:34:21.094591 tad_mctc-0.1.1/src/tad_mctc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-03-29 21:34:21.000000 tad_mctc-0.1.1/src/tad_mctc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-29 21:34:21.000000 tad_mctc-0.1.1/src/tad_mctc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 21:34:21.000000 tad_mctc-0.1.1/src/tad_mctc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-29 21:34:21.000000 tad_mctc-0.1.1/src/tad_mctc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 21:34:21.000000 tad_mctc-0.1.1/src/tad_mctc.egg-info/top_level.txt
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/
+-rw-rw-r--   0 friede    (1000) friede    (1000)    11358 2024-03-28 13:09:56.000000 tad_mctc-0.1.2/LICENSE
+-rw-rw-r--   0 friede    (1000) friede    (1000)     9497 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)     8658 2024-03-28 13:09:56.000000 tad_mctc-0.1.2/README.md
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1648 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/pyproject.toml
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1250 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/setup.cfg
+-rw-rw-r--   0 friede    (1000) friede    (1000)      714 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/setup.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4302 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1590 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/_version.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc/autograd/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      921 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1455 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/batched.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4489 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/compat.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4188 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/gradcheck.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2691 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/hessian.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2058 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/internals.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2578 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/autograd/nonfunctorch.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/batch/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      817 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/batch/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1911 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/batch/agnostic.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3305 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/mask.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5722 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/pack.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5898 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/batch/unpack.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/convert/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      903 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3963 2024-04-05 08:07:49.000000 tad_mctc-0.1.2/src/tad_mctc/convert/numpy.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1692 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/pse.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3928 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/pytorch.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2733 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/convert/tensor.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/data/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1041 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1890 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/en.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3320 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/getters.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2421 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/mass.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    69463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/molecules.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4440 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/pse.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4312 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/radii.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3607 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/data/zeff.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/exceptions/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      803 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1143 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/io.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      994 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/molecule.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      944 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/exceptions/pytorch.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      750 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/__init__.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/checks/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      782 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     6220 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/molecule.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2251 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/checks/shape.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/read/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1144 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/dotfiles.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     6505 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/frompath.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2834 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/orca.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3169 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/qcschema.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5446 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/reader.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2370 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/tblite.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5433 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/turbomole.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5472 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/read/xyz.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/io/write/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      770 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2240 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/turbomole.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2704 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/writer.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2446 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/io/write/xyz.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/math/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      746 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/math/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2251 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/math/einsum.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.166719 tad_mctc-0.1.2/src/tad_mctc/molecule/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      793 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    13209 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/bond.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4014 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/geometry.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4546 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/molecule/property.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/ncoord/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2871 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5967 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/count.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     5623 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/d3.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3731 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/d4.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1593 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/defaults.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4019 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/ncoord/eeq.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)        0 2024-01-09 09:57:14.000000 tad_mctc-0.1.2/src/tad_mctc/py.typed
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/storch/
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1113 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4538 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/distance.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4289 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/storch/elemental.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)    30570 2024-04-05 12:07:52.000000 tad_mctc-0.1.2/src/tad_mctc/storch/linalg.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1343 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/storch/utils.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/typing/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      920 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1137 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/builtin.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     4777 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/typing/compat.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     8427 2024-04-12 11:36:53.000000 tad_mctc-0.1.2/src/tad_mctc/typing/pytorch.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.170719 tad_mctc-0.1.2/src/tad_mctc/units/
+-rw-rw-r--   0 friede    (1000) friede    (1000)      841 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/__init__.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2025 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/codata.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     3517 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/energy.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1463 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/length.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1682 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/mass.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)      873 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/math.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2490 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/spectroscopy.py
+-rw-rw-r--   0 friede    (1000) friede    (1000)     1047 2024-04-02 14:20:05.000000 tad_mctc-0.1.2/src/tad_mctc/units/time.py
+drwxrwxr-x   0 friede    (1000) friede    (1000)        0 2024-04-12 11:37:11.162719 tad_mctc-0.1.2/src/tad_mctc.egg-info/
+-rw-r--r--   0 friede    (1000) friede    (1000)     9497 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/PKG-INFO
+-rw-rw-r--   0 friede    (1000) friede    (1000)     2617 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/SOURCES.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)        1 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/dependency_links.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)      238 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/requires.txt
+-rw-rw-r--   0 friede    (1000) friede    (1000)        9 2024-04-12 11:37:11.000000 tad_mctc-0.1.2/src/tad_mctc.egg-info/top_level.txt
```

### Comparing `tad_mctc-0.1.1/LICENSE` & `tad_mctc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/PKG-INFO` & `tad_mctc-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_mctc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Torch Autodiff Utility
 Author: "Marvin Friede"
 License: Apache-2.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -14,39 +14,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: opt-einsum
-Requires-Dist: scipy
-Requires-Dist: torch>=1.11
-Requires-Dist: typing-extensions
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-random-order; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: tox; extra == "dev"
 Provides-Extra: tox
-Requires-Dist: covdefaults; extra == "tox"
-Requires-Dist: pytest; extra == "tox"
-Requires-Dist: pytest-cov; extra == "tox"
-Requires-Dist: pytest-random-order; extra == "tox"
-Requires-Dist: pytest-xdist; extra == "tox"
-Requires-Dist: scipy; extra == "tox"
+License-File: LICENSE
 
 # Torch Autodiff Utility
 
 <table>
   <tr>
     <td>Compatibility:</td>
     <td>
```

#### html2text {}

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.1 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.2 Summary: Torch Autodiff
 Utility Author: "Marvin Friede" License: Apache-2.0 Classifier: Framework ::
 Pytest Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: opt-
-einsum Requires-Dist: scipy Requires-Dist: torch>=1.11 Requires-Dist: typing-
-extensions Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-
-Dist: covdefaults; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-
-Dist: pre-commit; extra == "dev" Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-random-order; extra == "dev" Requires-Dist: pytest-xdist;
-extra == "dev" Requires-Dist: scipy; extra == "dev" Requires-Dist: tox; extra
-== "dev" Provides-Extra: tox Requires-Dist: covdefaults; extra == "tox"
-Requires-Dist: pytest; extra == "tox" Requires-Dist: pytest-cov; extra == "tox"
-Requires-Dist: pytest-random-order; extra == "tox" Requires-Dist: pytest-xdist;
-extra == "tox" Requires-Dist: scipy; extra == "tox" # Torch Autodiff Utility
+text/markdown Provides-Extra: dev Provides-Extra: tox License-File: LICENSE #
+Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
```

### Comparing `tad_mctc-0.1.1/README.md` & `tad_mctc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/pyproject.toml` & `tad_mctc-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/setup.cfg` & `tad_mctc-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/setup.py` & `tad_mctc-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/_version.py` & `tad_mctc-0.1.2/src/tad_mctc/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,9 +46,9 @@
             f"versioning scheme of MAJOR.MINOR.PATCH ({s})."
         )
 
     version_numbers = [int(part) for part in s[:3]]
     return tuple(version_numbers)
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __tversion__ = version_tuple(torch.__version__)
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/autograd/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/autograd/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 - Jacobians
 - Hessians
 """
 from .batched import *
 from .gradcheck import *
 from .hessian import *
 from .internals import *
+from .nonfunctorch import *
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/autograd/compat.py` & `tad_mctc-0.1.2/src/tad_mctc/autograd/compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 
 def jacrev_compat(
     f: Callable[..., Tensor], argnums: int = 0, **kwargs: Any
 ) -> Any:  # pragma: no cover
     """
     Wrapper for Jacobian calcluation.
 
+    .. warning::
+
+        The compatibility wrapper sets `create_graph=True` by default.
+
     Parameters
     ----------
     f : Callable[[Any], Tensor]
         The function whose result is differentiated.
     argnums : int, optional
         The variable w.r.t. which will be differentiated. Defaults to 0.
     """
@@ -48,15 +52,15 @@
         from torch.autograd.functional import jacobian  # type: ignore[import-error]
     except ImportError as e:
         raise ImportError(
             f"Failed to import required modules. {e}. {e.name} provides "
             "an API for Jacobian calculations for older PyTorch versions."
         ) from e
 
-    def wrap(*inps: Any) -> Any:
+    def jacrev_compat_wrap(*inps: Any) -> Any:
         """
         Wrapper to imitate the calling signature of functorch's `jacrev`
         with `torch.autograd.functional.jacobian`.
 
         Parameters
         ----------
         inps : tuple[Any, ...]
@@ -84,17 +88,20 @@
         after = inps[(argnums + 1) :]
 
         # `jacobian` only takes tensors, requiring another wrapper that
         # passes the non-tensor arguments to the function `f`
         def _f(arg: Tensor) -> Tensor:
             return f(*(*before, arg, *after))
 
-        return jacobian(_f, inputs=diffarg, **kwargs)  # type: ignore # pylint: disable=used-before-assignment
+        create_graph = kwargs.pop("create_graph", True)
+
+        # pylint: disable=used-before-assignment
+        return jacobian(_f, inputs=diffarg, create_graph=create_graph, **kwargs)
 
-    return wrap
+    return jacrev_compat_wrap
 
 
 def vmap_compat(
     func: Callable[..., Tensor],
     in_dims: int = 0,
     out_dims: int = 0,
 ) -> Callable[..., Tensor]:
@@ -111,24 +118,25 @@
         Index of output dimension to be vectorized over. Defaults to 0.
 
     Returns
     -------
     Callable[..., Tensor]
         Vectorized function.
     """
+    # pylint: disable=import-outside-toplevel
     from warnings import warn
 
     warn(
         "Using a simple manual vmap implementation. Consider upgrading PyTorch "
         "(functorch) for better performance and more features.",
         DeprecationWarning,
     )
 
     def manual_vmap(*args, **kwargs):
-        # some sanity checks
+        # some sanity checks, non-exhaustive
         assert isinstance(in_dims, int), "Input dimensions must be integer."
         assert isinstance(out_dims, int), "Output dimensions must be integer."
         assert len(args) > 0, "At least one argument is required."
         assert isinstance(args[0], Tensor), "First argument must be a tensor."
 
         outputs = []
         for i in range(args[0].size(in_dims)):
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/autograd/gradcheck.py` & `tad_mctc-0.1.2/src/tad_mctc/autograd/gradcheck.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/autograd/hessian.py` & `tad_mctc-0.1.2/src/tad_mctc/autograd/hessian.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/autograd/internals.py` & `tad_mctc-0.1.2/src/tad_mctc/autograd/internals.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,23 +20,38 @@
 
 This module imports PyTorch's own autograd functions, depending on the version.
 
 Important! Before PyTorch 2.0.0, `functorch` does not work together with custom
 autograd functions, which we definitely require. Additionally, `functorch`
 imposes the implementation of a `forward` **and** `setup_context` method, i.e.,
 the traditional way of using `forward` with the `ctx` argument does not work.
+
+Note
+----
+`functorch` is shipped with PyTorch 1.13.0 and later. Earlier versions require
+a separate installation.
 """
 from __future__ import annotations
 
-import torch
+from .._version import __tversion__
+
+__all__ = ["jacrev", "fjacrev", "vmap", "fvmap"]
 
-__all__ = ["jacrev", "vmap"]
 
+if __tversion__ < (2, 0, 0):
+    # We always use the compatiblity functions even if `functorch` is available,
+    # because `functorch` does not work with custom autograd functions.
+    from .compat import jacrev_compat as jacrev
+    from .compat import vmap_compat as vmap
 
-if torch.__version__ < (2, 0, 0):  # type: ignore[operator]
     try:
-        from functorch import jacrev, vmap  # type: ignore[import-error]
+        from functorch import jacrev as fjacrev  # type: ignore[import-error]
+        from functorch import vmap as fvmap  # type: ignore[import-error]
     except ModuleNotFoundError:
-        from .compat import jacrev_compat as jacrev
-        from .compat import vmap_compat as vmap
+        fjacrev = None
+        fvmap = None
 else:
-    from torch.func import jacrev, vmap  # type: ignore[import-error]
+    from torch.func import jacrev as jacrev  # type: ignore[import-error]
+    from torch.func import vmap  # type: ignore[import-error]
+
+    fjacrev = jacrev
+    fvmap = vmap
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/batch/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/batch/agnostic.py` & `tad_mctc-0.1.2/src/tad_mctc/batch/agnostic.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/batch/mask.py` & `tad_mctc-0.1.2/src/tad_mctc/batch/mask.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import torch
 
 from ..typing import Tensor
 
 __all__ = ["real_atoms", "real_pairs", "real_triples"]
 
 
+@torch.jit.script
 def real_atoms(numbers: Tensor) -> Tensor:
     """
     Create a mask for atoms, discerning padding and actual atoms.
     Padding value is zero.
 
     Parameters
     ----------
@@ -43,14 +44,15 @@
     -------
     Tensor
         Mask for atoms that discerns padding and real atoms.
     """
     return numbers != 0
 
 
+@torch.jit.script
 def real_pairs(numbers: Tensor, mask_diagonal: bool = True) -> Tensor:
     """
     Create a mask for pairs of atoms from atomic numbers, discerning padding
     and actual atoms. Padding value is zero.
 
     Parameters
     ----------
@@ -69,14 +71,15 @@
     mask = real.unsqueeze(-2) * real.unsqueeze(-1)
 
     if mask_diagonal is True:
         mask *= ~torch.diag_embed(torch.ones_like(real))
     return mask
 
 
+@torch.jit.script
 def real_triples(
     numbers: Tensor, mask_diagonal: bool = True, mask_self: bool = True
 ) -> Tensor:
     """
     Create a mask for triples from atomic numbers. Padding value is zero.
 
     Parameters
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/batch/pack.py` & `tad_mctc-0.1.2/src/tad_mctc/batch/pack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# This file is part of tad-mctc.
+# This file is part of dxtb, modified from tbmalt/tbmalt.
 #
 # SPDX-Identifier: Apache-2.0
 # Copyright (C) 2024 Grimme Group
 #
+# Original file licensed under the LGPL-3.0 License by tbmalt/tbmalt.
+# Modifications made by Grimme Group.
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/batch/unpack.py` & `tad_mctc-0.1.2/src/tad_mctc/batch/unpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-# This file is part of tad-mctc.
+# This file is part of dxtb, modified from tbmalt/tbmalt.
 #
 # SPDX-Identifier: Apache-2.0
 # Copyright (C) 2024 Grimme Group
 #
+# Original file licensed under the LGPL-3.0 License by tbmalt/tbmalt.
+# Modifications made by Grimme Group.
+#
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/convert/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/convert/numpy.py` & `tad_mctc-0.1.2/src/tad_mctc/convert/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         dtype = torch_to_numpy_dtype_dict.get(x.dtype, np.dtype(np.float64))
 
     xdtype = torch_to_numpy_dtype_dict.get(x.dtype)
     x = x.detach().cpu()
 
     # pylint: disable=protected-access
     # see: https://github.com/pytorch/pytorch/issues/91810
-    if __tversion__ >= (2, 0, 0):
+    if __tversion__ >= (1, 13, 0):
         if torch._C._functorch.is_gradtrackingtensor(x):
             while torch._C._functorch.is_functorch_wrapped_tensor(x) is True:
                 x = torch._C._functorch.get_unwrapped(x)
 
             if __tversion__ < (2, 0, 0):  # type: ignore[operator] # pragma: no cover
                 interpreted = np.array(x.storage().tolist(), dtype=dtype)
             else:
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/convert/pse.py` & `tad_mctc-0.1.2/src/tad_mctc/convert/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/convert/pytorch.py` & `tad_mctc-0.1.2/src/tad_mctc/convert/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/convert/tensor.py` & `tad_mctc-0.1.2/src/tad_mctc/convert/tensor.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/en.py` & `tad_mctc-0.1.2/src/tad_mctc/data/en.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/getters.py` & `tad_mctc-0.1.2/src/tad_mctc/data/getters.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/mass.py` & `tad_mctc-0.1.2/src/tad_mctc/data/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/molecules.py` & `tad_mctc-0.1.2/src/tad_mctc/data/molecules.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/pse.py` & `tad_mctc-0.1.2/src/tad_mctc/data/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/radii.py` & `tad_mctc-0.1.2/src/tad_mctc/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/data/zeff.py` & `tad_mctc-0.1.2/src/tad_mctc/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/exceptions/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/exceptions/io.py` & `tad_mctc-0.1.2/src/tad_mctc/exceptions/io.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/exceptions/molecule.py` & `tad_mctc-0.1.2/src/tad_mctc/exceptions/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/exceptions/pytorch.py` & `tad_mctc-0.1.2/src/tad_mctc/exceptions/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/checks/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/io/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/checks/molecule.py` & `tad_mctc-0.1.2/src/tad_mctc/io/checks/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/checks/shape.py` & `tad_mctc-0.1.2/src/tad_mctc/io/checks/shape.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/dotfiles.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/dotfiles.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/frompath.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/frompath.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/orca.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/orca.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/qcschema.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/qcschema.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/reader.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/reader.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/tblite.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/tblite.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/turbomole.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/read/xyz.py` & `tad_mctc-0.1.2/src/tad_mctc/io/read/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/write/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/io/write/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/write/turbomole.py` & `tad_mctc-0.1.2/src/tad_mctc/io/write/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/write/writer.py` & `tad_mctc-0.1.2/src/tad_mctc/io/write/writer.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/io/write/xyz.py` & `tad_mctc-0.1.2/src/tad_mctc/io/write/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/math/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/math/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/math/einsum.py` & `tad_mctc-0.1.2/src/tad_mctc/math/einsum.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/molecule/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/molecule/bond.py` & `tad_mctc-0.1.2/src/tad_mctc/molecule/bond.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/molecule/geometry.py` & `tad_mctc-0.1.2/src/tad_mctc/molecule/geometry.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/molecule/property.py` & `tad_mctc-0.1.2/src/tad_mctc/molecule/property.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/count.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/count.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/d3.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/d3.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/d4.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/d4.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/defaults.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/ncoord/eeq.py` & `tad_mctc-0.1.2/src/tad_mctc/ncoord/eeq.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/storch/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/storch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/storch/distance.py` & `tad_mctc-0.1.2/src/tad_mctc/storch/distance.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/storch/elemental.py` & `tad_mctc-0.1.2/src/tad_mctc/storch/elemental.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 def divide(
     x: Tensor, y: Tensor, *, eps: Tensor | float | int | None = None, **kwargs: Any
 ) -> Tensor:
     """
     Safe divide operation.
+    Only adds a small value to the denominator where it is zero.
 
     Parameters
     ----------
     x : Tensor
         Input tensor (nominator).
     y : Tensor
         Input tensor (denominator).
@@ -64,15 +65,16 @@
         eps = eps.to(device=x.device, dtype=x.dtype)
     else:
         raise TypeError(
             "Value for clamping must be None (default), Tensor, float, or int, "
             f"but {type(eps)} was given."
         )
 
-    return torch.divide(x, (y + eps), **kwargs)
+    y_safe = torch.where(y == 0, torch.full_like(y, eps), y)
+    return torch.divide(x, y_safe, **kwargs)
 
 
 def reciprocal(
     x: Tensor, *, eps: Tensor | float | int | None = None, **kwargs: Any
 ) -> Tensor:
     """
     Safe reciprocal operation.
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/storch/linalg.py` & `tad_mctc-0.1.2/src/tad_mctc/storch/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,15 +712,14 @@
         # For Cholesky decomposition scheme
         if scheme == "chol":
             # Perform Cholesky factorization (A = LL^{T}) of B to attain L
             l = torch.linalg.cholesky(b)
 
             # Compute the inverse of L:
             if kwargs.get("direct_inv", False):
-                print("Direct inversion")
                 # Via the direct method if specifically requested
                 l_inv = torch.inverse(l)
             else:
                 # Otherwise compute via an indirect method (default)
                 identity = torch.zeros_like(l)
                 identity.diagonal(dim1=-2, dim2=-1)[:] = 1
                 l_inv = torch.linalg.solve(l, identity)
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/storch/utils.py` & `tad_mctc-0.1.2/src/tad_mctc/storch/utils.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/typing/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/typing/builtin.py` & `tad_mctc-0.1.2/src/tad_mctc/typing/builtin.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/typing/compat.py` & `tad_mctc-0.1.2/src/tad_mctc/typing/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/typing/pytorch.py` & `tad_mctc-0.1.2/src/tad_mctc/typing/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 __all__ = [
     "DD",
     "MockTensor",
     "Molecule",
     "get_default_device",
     "get_default_dtype",
+    "Tensor",
     "TensorLike",
 ]
 
 
 class DD(TypedDict):
     """Collection of torch.device and torch.dtype."""
 
@@ -119,22 +120,21 @@
 
     __dtype: torch.dtype
     """Floating point dtype used by class object."""
 
     __dd: DD
     """Shortcut for device and dtype."""
 
-    __slots__ = ["__device", "__dtype", "__dd"]
+    __slots__ = ["__device", "__dtype"]
 
     def __init__(
         self, device: torch.device | None = None, dtype: torch.dtype | None = None
     ):
         self.__device = device if device is not None else get_default_device()
         self.__dtype = dtype if dtype is not None else get_default_dtype()
-        self.__dd = {"device": self.device, "dtype": self.dtype}
 
     @property
     def device(self) -> torch.device:
         """The device on which the class object resides."""
         return self.__device
 
     @device.setter
@@ -175,15 +175,15 @@
             Setter is called.
         """
         raise AttributeError("Change object to dtype using the `.type` method")
 
     @property
     def dd(self) -> DD:
         """Shortcut for device and dtype."""
-        return self.__dd
+        return {"device": self.device, "dtype": self.dtype}
 
     @dd.setter
     def dd(self, *_: Any) -> NoReturn:
         """
         Instruct users to use the `.type` and `.to` methods to change.
 
         Returns
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/__init__.py` & `tad_mctc-0.1.2/src/tad_mctc/units/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/codata.py` & `tad_mctc-0.1.2/src/tad_mctc/units/codata.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/energy.py` & `tad_mctc-0.1.2/src/tad_mctc/units/energy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/length.py` & `tad_mctc-0.1.2/src/tad_mctc/units/length.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/mass.py` & `tad_mctc-0.1.2/src/tad_mctc/units/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/math.py` & `tad_mctc-0.1.2/src/tad_mctc/units/math.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/spectroscopy.py` & `tad_mctc-0.1.2/src/tad_mctc/units/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc/units/time.py` & `tad_mctc-0.1.2/src/tad_mctc/units/time.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.1/src/tad_mctc.egg-info/PKG-INFO` & `tad_mctc-0.1.2/src/tad_mctc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tad_mctc
-Version: 0.1.1
+Name: tad-mctc
+Version: 0.1.2
 Summary: Torch Autodiff Utility
 Author: "Marvin Friede"
 License: Apache-2.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -14,39 +14,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: opt-einsum
-Requires-Dist: scipy
-Requires-Dist: torch>=1.11
-Requires-Dist: typing-extensions
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-random-order; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: tox; extra == "dev"
 Provides-Extra: tox
-Requires-Dist: covdefaults; extra == "tox"
-Requires-Dist: pytest; extra == "tox"
-Requires-Dist: pytest-cov; extra == "tox"
-Requires-Dist: pytest-random-order; extra == "tox"
-Requires-Dist: pytest-xdist; extra == "tox"
-Requires-Dist: scipy; extra == "tox"
+License-File: LICENSE
 
 # Torch Autodiff Utility
 
 <table>
   <tr>
     <td>Compatibility:</td>
     <td>
```

#### html2text {}

```diff
@@ -1,29 +1,19 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.1 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad-mctc Version: 0.1.2 Summary: Torch Autodiff
 Utility Author: "Marvin Friede" License: Apache-2.0 Classifier: Framework ::
 Pytest Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: opt-
-einsum Requires-Dist: scipy Requires-Dist: torch>=1.11 Requires-Dist: typing-
-extensions Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-
-Dist: covdefaults; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-
-Dist: pre-commit; extra == "dev" Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: pytest-random-order; extra == "dev" Requires-Dist: pytest-xdist;
-extra == "dev" Requires-Dist: scipy; extra == "dev" Requires-Dist: tox; extra
-== "dev" Provides-Extra: tox Requires-Dist: covdefaults; extra == "tox"
-Requires-Dist: pytest; extra == "tox" Requires-Dist: pytest-cov; extra == "tox"
-Requires-Dist: pytest-random-order; extra == "tox" Requires-Dist: pytest-xdist;
-extra == "tox" Requires-Dist: scipy; extra == "tox" # Torch Autodiff Utility
+text/markdown Provides-Extra: dev Provides-Extra: tox License-File: LICENSE #
+Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
```

### Comparing `tad_mctc-0.1.1/src/tad_mctc.egg-info/SOURCES.txt` & `tad_mctc-0.1.2/src/tad_mctc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/tad_mctc.egg-info/top_level.txt
 src/tad_mctc/autograd/__init__.py
 src/tad_mctc/autograd/batched.py
 src/tad_mctc/autograd/compat.py
 src/tad_mctc/autograd/gradcheck.py
 src/tad_mctc/autograd/hessian.py
 src/tad_mctc/autograd/internals.py
+src/tad_mctc/autograd/nonfunctorch.py
 src/tad_mctc/batch/__init__.py
 src/tad_mctc/batch/agnostic.py
 src/tad_mctc/batch/mask.py
 src/tad_mctc/batch/pack.py
 src/tad_mctc/batch/unpack.py
 src/tad_mctc/convert/__init__.py
 src/tad_mctc/convert/numpy.py
```

