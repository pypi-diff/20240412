# Comparing `tmp/zope.interface-6.1a2.tar.gz` & `tmp/zope.interface-6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.interface-6.1a2.tar", last modified: Thu Apr 13 06:24:13 2023, max compression
+gzip compressed data, was "zope.interface-6.2.tar", last modified: Fri Feb 16 07:42:53 2024, max compression
```

## Comparing `zope.interface-6.1a2.tar` & `zope.interface-6.2.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.826079 zope.interface-6.1a2/
--rw-r--r--   0 mac        (513) staff       (20)      588 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.coveragerc
--rwxr-xr-x   0 mac        (513) staff       (20)     2183 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.manylinux-install.sh
--rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.manylinux.sh
--rw-r--r--   0 mac        (513) staff       (20)    38648 2023-04-13 06:24:12.000000 zope.interface-6.1a2/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      799 2023-04-13 06:24:12.000000 zope.interface-6.1a2/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-13 06:24:12.000000 zope.interface-6.1a2/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-13 06:24:12.000000 zope.interface-6.1a2/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      564 2023-04-13 06:24:12.000000 zope.interface-6.1a2/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    41194 2023-04-13 06:24:13.826254 zope.interface-6.1a2/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1353 2023-04-13 06:24:12.000000 zope.interface-6.1a2/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     1949 2023-04-13 06:24:12.000000 zope.interface-6.1a2/appveyor.yml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.794986 zope.interface-6.1a2/benchmarks/
--rw-r--r--   0 mac        (513) staff       (20)     8497 2023-04-13 06:24:12.000000 zope.interface-6.1a2/benchmarks/micro.py
--rw-r--r--   0 mac        (513) staff       (20)      838 2023-04-13 06:24:12.000000 zope.interface-6.1a2/build.cmd
--rw-r--r--   0 mac        (513) staff       (20)      215 2023-04-13 06:24:12.000000 zope.interface-6.1a2/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.800061 zope.interface-6.1a2/docs/
--rw-r--r--   0 mac        (513) staff       (20)     5592 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)    41051 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/README.rst
--rw-r--r--   0 mac        (513) staff       (20)    33998 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/README.ru.rst
--rw-r--r--   0 mac        (513) staff       (20)    18817 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/adapter.rst
--rw-r--r--   0 mac        (513) staff       (20)    21169 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/adapter.ru.rst
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.803496 zope.interface-6.1a2/docs/api/
--rw-r--r--   0 mac        (513) staff       (20)      691 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/adapters.rst
--rw-r--r--   0 mac        (513) staff       (20)     1283 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/common.rst
--rw-r--r--   0 mac        (513) staff       (20)     2465 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/components.rst
--rw-r--r--   0 mac        (513) staff       (20)    21746 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/declarations.rst
--rw-r--r--   0 mac        (513) staff       (20)      165 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      687 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/ro.rst
--rw-r--r--   0 mac        (513) staff       (20)     9948 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/specifications.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/changes.rst
--rw-r--r--   0 mac        (513) staff       (20)     9081 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     1742 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/foodforthought.rst
--rw-r--r--   0 mac        (513) staff       (20)     9509 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)     6537 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/human.rst
--rw-r--r--   0 mac        (513) staff       (20)    10681 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/human.ru.rst
--rw-r--r--   0 mac        (513) staff       (20)      639 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5110 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)    10222 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/verify.rst
--rw-r--r--   0 mac        (513) staff       (20)      286 2023-04-13 06:24:12.000000 zope.interface-6.1a2/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      604 2023-04-13 06:24:13.826903 zope.interface-6.1a2/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     4885 2023-04-13 06:24:12.000000 zope.interface-6.1a2/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.788312 zope.interface-6.1a2/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.803831 zope.interface-6.1a2/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.811390 zope.interface-6.1a2/src/zope/interface/
--rw-r--r--   0 mac        (513) staff       (20)     3463 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     4369 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)     1056 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_flatten.py
--rw-r--r--   0 mac        (513) staff       (20)    57678 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 mac        (513) staff       (20)    36218 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/adapter.py
--rw-r--r--   0 mac        (513) staff       (20)     3890 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/advice.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.814552 zope.interface-6.1a2/src/zope/interface/common/
--rw-r--r--   0 mac        (513) staff       (20)    10461 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3027 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/builtins.py
--rw-r--r--   0 mac        (513) staff       (20)     6792 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/collections.py
--rw-r--r--   0 mac        (513) staff       (20)    20858 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/idatetime.py
--rw-r--r--   0 mac        (513) staff       (20)     5367 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1241 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/io.py
--rw-r--r--   0 mac        (513) staff       (20)     4677 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/mapping.py
--rw-r--r--   0 mac        (513) staff       (20)     1682 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/numbers.py
--rw-r--r--   0 mac        (513) staff       (20)     5525 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.817204 zope.interface-6.1a2/src/zope/interface/common/tests/
--rw-r--r--   0 mac        (513) staff       (20)     5310 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3906 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 mac        (513) staff       (20)     1345 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 mac        (513) staff       (20)     5724 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 mac        (513) staff       (20)     1594 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1597 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 mac        (513) staff       (20)     1394 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 mac        (513) staff       (20)    42843 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/declarations.py
--rw-r--r--   0 mac        (513) staff       (20)     4067 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/document.py
--rw-r--r--   0 mac        (513) staff       (20)     8635 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/exceptions.py
--rw-r--r--   0 mac        (513) staff       (20)    38825 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/interface.py
--rw-r--r--   0 mac        (513) staff       (20)    50125 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)    25828 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/registry.py
--rw-r--r--   0 mac        (513) staff       (20)    24155 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/ro.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.825739 zope.interface-6.1a2/src/zope/interface/tests/
--rw-r--r--   0 mac        (513) staff       (20)     3961 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      897 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 mac        (513) staff       (20)      911 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/dummy.py
--rw-r--r--   0 mac        (513) staff       (20)      889 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/idummy.py
--rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/m1.py
--rw-r--r--   0 mac        (513) staff       (20)     3015 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/odd.py
--rw-r--r--   0 mac        (513) staff       (20)    79548 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 mac        (513) staff       (20)     5962 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 mac        (513) staff       (20)     1290 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 mac        (513) staff       (20)    82128 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 mac        (513) staff       (20)    16899 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_document.py
--rw-r--r--   0 mac        (513) staff       (20)     1118 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_element.py
--rw-r--r--   0 mac        (513) staff       (20)     6411 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 mac        (513) staff       (20)    91465 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 mac        (513) staff       (20)     4377 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     7565 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 mac        (513) staff       (20)   112819 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 mac        (513) staff       (20)    14121 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 mac        (513) staff       (20)     1933 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 mac        (513) staff       (20)    19190 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 mac        (513) staff       (20)     7154 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/verify.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.806270 zope.interface-6.1a2/src/zope.interface.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    41194 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2921 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      153 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1430 2023-04-13 06:24:13.000000 zope.interface-6.1a2/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.332718 zope.interface-6.2/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      588 2024-02-16 07:42:52.000000 zope.interface-6.2/.coveragerc
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)     2259 2024-02-16 07:42:52.000000 zope.interface-6.2/.manylinux-install.sh
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-02-16 07:42:52.000000 zope.interface-6.2/.manylinux.sh
+-rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-02-16 07:42:52.000000 zope.interface-6.2/.readthedocs.yaml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    38873 2024-02-16 07:42:52.000000 zope.interface-6.2/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-02-16 07:42:52.000000 zope.interface-6.2/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-02-16 07:42:52.000000 zope.interface-6.2/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-02-16 07:42:52.000000 zope.interface-6.2/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      579 2024-02-16 07:42:52.000000 zope.interface-6.2/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41923 2024-02-16 07:42:53.332606 zope.interface-6.2/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1353 2024-02-16 07:42:52.000000 zope.interface-6.2/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1971 2024-02-16 07:42:52.000000 zope.interface-6.2/appveyor.yml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.317380 zope.interface-6.2/benchmarks/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8497 2024-02-16 07:42:52.000000 zope.interface-6.2/benchmarks/micro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      838 2024-02-16 07:42:52.000000 zope.interface-6.2/build.cmd
+-rw-r--r--   0 m.howitz   (502) staff       (20)      215 2024-02-16 07:42:52.000000 zope.interface-6.2/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.320127 zope.interface-6.2/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5592 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41051 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    33998 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/README.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18817 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/adapter.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21169 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/adapter.ru.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.321381 zope.interface-6.2/docs/api/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      691 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/adapters.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1283 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/common.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2465 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/components.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    21746 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/declarations.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      165 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      687 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/ro.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9948 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/api/specifications.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/changes.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9130 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1742 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/foodforthought.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9509 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6537 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/human.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10681 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/human.ru.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      639 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5110 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/requirements.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10222 2024-02-16 07:42:52.000000 zope.interface-6.2/docs/verify.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      599 2024-02-16 07:42:53.332985 zope.interface-6.2/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5014 2024-02-16 07:42:52.000000 zope.interface-6.2/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.314466 zope.interface-6.2/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.321572 zope.interface-6.2/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.325064 zope.interface-6.2/src/zope/interface/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3460 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4369 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_compat.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1057 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_flatten.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    57205 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)    36218 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3892 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/advice.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.326789 zope.interface-6.2/src/zope/interface/common/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10462 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3027 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6792 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    20964 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5368 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1242 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4678 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/mapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1682 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5526 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.328035 zope.interface-6.2/src/zope/interface/common/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5309 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3907 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5718 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1923 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      813 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1597 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1394 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    43007 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4068 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8636 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    39099 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    50126 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    25829 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    24157 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/ro.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.331680 zope.interface-6.2/src/zope/interface/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3961 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      898 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      912 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      890 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/m1.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3015 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/odd.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    79479 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5962 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1290 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    82140 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17164 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1120 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6412 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    92312 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4377 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7566 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)   112910 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    14124 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1934 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19191 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7226 2024-02-16 07:42:52.000000 zope.interface-6.2/src/zope/interface/verify.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:42:53.331923 zope.interface-6.2/src/zope.interface.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    41923 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2953 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2024-02-16 07:42:53.000000 zope.interface-6.2/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2045 2024-02-16 07:42:52.000000 zope.interface-6.2/tox.ini
```

### Comparing `zope.interface-6.1a2/.coveragerc` & `zope.interface-6.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/.manylinux-install.sh` & `zope.interface-6.2/.manylinux-install.sh`

 * *Files 6% similar despite different names*

```diff
@@ -24,34 +24,36 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
-        *"cp312"*) echo 'py312';;
+        *"cp313"*) echo 'py313';;
         *"cp37"*) echo 'py37';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
+        *"cp312"*) echo 'py312';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
+       [[ "${PYBIN}" == *"cp313"* ]] || \
        [[ "${PYBIN}" == *"cp311"* ]] || \
+       [[ "${PYBIN}" == *"cp312"* ]] || \
        [[ "${PYBIN}" == *"cp37"* ]] || \
        [[ "${PYBIN}" == *"cp38"* ]] || \
        [[ "${PYBIN}" == *"cp39"* ]] || \
        [[ "${PYBIN}" == *"cp310"* ]] ; then
-        if [[ "${PYBIN}" == *"cp312"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313"* ]] ; then
             "${PYBIN}/pip" install --pre -e /io/
             "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
         else
             "${PYBIN}/pip" install -e /io/
             "${PYBIN}/pip" wheel /io/ -w wheelhouse/
         fi
         if [ `uname -m` == 'aarch64' ]; then
```

### Comparing `zope.interface-6.1a2/CHANGES.rst` & `zope.interface-6.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 =========
  Changes
 =========
 
-6.1a2 (2023-04-13)
-==================
+6.2 (2024-02-16)
+================
 
-- Fix building of the docs for non-final versions.
+- Add preliminary support for Python 3.13 as of 3.13a3.
 
+- Add support to use the pipe (``|``) syntax for ``typing.Union``.
+  (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
 
-6.1a1 (2023-04-06)
-==================
 
-- Add support for building ppc64le wheels.
+6.1 (2023-10-05)
+================
+
+- Build Linux binary wheels for Python 3.12.
+
+- Add support for Python 3.12.
+
+- Fix building of the docs for non-final versions.
 
 
 6.0 (2023-03-17)
 ================
 
 - Build Linux binary wheels for Python 3.11.
```

### Comparing `zope.interface-6.1a2/CONTRIBUTING.md` & `zope.interface-6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/LICENSE.txt` & `zope.interface-6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/MANIFEST.in` & `zope.interface-6.2/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 
 recursive-include src *.py
+include *.yaml
 include *.cmd
 include *.sh
 include *.yml
 include .coveragerc
 recursive-include benchmarks *.py
 recursive-include docs *.bat
 recursive-include docs *.py
```

### Comparing `zope.interface-6.1a2/PKG-INFO` & `zope.interface-6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.1a2
+Version: 6.2
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,23 +14,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+Requires-Dist: setuptools
 Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
+Requires-Dist: coverage>=5.0.3; extra == "test"
+Requires-Dist: zope.event; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
 Provides-Extra: testing
-License-File: LICENSE.txt
+Requires-Dist: coverage>=5.0.3; extra == "testing"
+Requires-Dist: zope.event; extra == "testing"
+Requires-Dist: zope.testing; extra == "testing"
 
 ====================
  ``zope.interface``
 ====================
 
 .. image:: https://img.shields.io/pypi/v/zope.interface.svg
     :target: https://pypi.python.org/pypi/zope.interface/
@@ -60,24 +71,31 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
-6.1a2 (2023-04-13)
-==================
+6.2 (2024-02-16)
+================
 
-- Fix building of the docs for non-final versions.
+- Add preliminary support for Python 3.13 as of 3.13a3.
 
+- Add support to use the pipe (``|``) syntax for ``typing.Union``.
+  (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
 
-6.1a1 (2023-04-06)
-==================
 
-- Add support for building ppc64le wheels.
+6.1 (2023-10-05)
+================
+
+- Build Linux binary wheels for Python 3.12.
+
+- Add support for Python 3.12.
+
+- Fix building of the docs for non-final versions.
 
 
 6.0 (2023-03-17)
 ================
 
 - Build Linux binary wheels for Python 3.11.
```

### Comparing `zope.interface-6.1a2/README.rst` & `zope.interface-6.2/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/appveyor.yml` & `zope.interface-6.2/appveyor.yml`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 
   matrix:
     - python: 37-x64
     - python: 38-x64
     - python: 39-x64
     - python: 310-x64
     - python: 311-x64
+    - python: 312-x64
     # `multibuild` cannot install non-final versions as they are not on
-    # ftp.python.org, so we skip Python 3.11 until its final release:
-    # - python: 312-x64
+    # ftp.python.org, so we skip Python 3.13 until its final release:
+    # - python: 313-x64
 
 install:
   - "SET PYTHONVERSION=%PYTHON%"
   - "SET PATH=C:\\Python%PYTHON%;c:\\Python%PYTHON%\\scripts;%PATH%"
   - ps: |
       $env:PYTHON = "C:\\Python${env:PYTHON}"
       if (-not (Test-Path $env:PYTHON)) {
```

### Comparing `zope.interface-6.1a2/benchmarks/micro.py` & `zope.interface-6.2/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/build.cmd` & `zope.interface-6.2/build.cmd`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/Makefile` & `zope.interface-6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/README.rst` & `zope.interface-6.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/README.ru.rst` & `zope.interface-6.2/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/adapter.rst` & `zope.interface-6.2/docs/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/adapter.ru.rst` & `zope.interface-6.2/docs/adapter.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/adapters.rst` & `zope.interface-6.2/docs/api/adapters.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/common.rst` & `zope.interface-6.2/docs/api/common.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/components.rst` & `zope.interface-6.2/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/declarations.rst` & `zope.interface-6.2/docs/api/declarations.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/ro.rst` & `zope.interface-6.2/docs/api/ro.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/api/specifications.rst` & `zope.interface-6.2/docs/api/specifications.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/conf.py` & `zope.interface-6.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -259,17 +259,17 @@
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'https://docs.python.org/': None,
-    'https://persistent.readthedocs.io/en/latest/': None,
-    'https://btrees.readthedocs.io/en/latest/': None,
+    'python': ('https://docs.python.org/', None),
+    'persistent': ('https://persistent.readthedocs.io/en/latest/', None),
+    'btrees': ('https://btrees.readthedocs.io/en/latest/', None),
 }
 
 # Sphinx 1.8+ prefers this to `autodoc_default_flags`. It's documented that
 # either True or None mean the same thing as just setting the flag, but
 # only None works in 1.8 (True works in 2.0)
 autodoc_default_options = {
     'members': None,
```

### Comparing `zope.interface-6.1a2/docs/foodforthought.rst` & `zope.interface-6.2/docs/foodforthought.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/hacking.rst` & `zope.interface-6.2/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/human.rst` & `zope.interface-6.2/docs/human.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/human.ru.rst` & `zope.interface-6.2/docs/human.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/index.rst` & `zope.interface-6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/make.bat` & `zope.interface-6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/docs/verify.rst` & `zope.interface-6.2/docs/verify.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/setup.cfg` & `zope.interface-6.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	docs/_build/html/_sources/*
 	docs/_build/html/_sources/api/*
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
-known_third_party = six, docutils, pkg_resources, pytz
+known_third_party = docutils, pkg_resources, pytz
 known_zope = 
 known_first_party = 
 default_section = ZOPE
 line_length = 79
 lines_after_imports = 2
 
 [egg_info]
```

### Comparing `zope.interface-6.1a2/setup.py` & `zope.interface-6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.interface package
 """
 
 import os
 import sys
-
 from distutils.errors import CCompilerError
 from distutils.errors import DistutilsExecError
 from distutils.errors import DistutilsPlatformError
 
-from setuptools import setup, Extension
-from setuptools.command.build_ext import build_ext
+from setuptools import Extension
 from setuptools import find_packages
+from setuptools import setup
+from setuptools.command.build_ext import build_ext
 
 
 class optional_build_ext(build_ext):
     """This class subclasses build_ext and allows
        the building of C extensions to fail.
     """
     def run(self):
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.1a2',
+      version='6.2',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
@@ -115,14 +115,15 @@
           "Programming Language :: Python",
           "Programming Language :: Python :: 3",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
+          "Programming Language :: Python :: 3.12",
           "Programming Language :: Python :: Implementation :: CPython",
           "Programming Language :: Python :: Implementation :: PyPy",
           "Framework :: Zope :: 3",
           "Topic :: Software Development :: Libraries :: Python Modules",
       ],
       packages=find_packages('src'),
       package_dir={'': 'src'},
@@ -133,14 +134,16 @@
       test_suite='zope.interface.tests',
       include_package_data=True,
       zip_safe=False,
       tests_require=tests_require,
       install_requires=['setuptools'],
       python_requires='>=3.7',
       extras_require={
-          'docs': ['Sphinx', 'repoze.sphinx.autointerface'],
+          'docs': ['Sphinx',
+                   'repoze.sphinx.autointerface',
+                   'sphinx_rtd_theme'],
           'test': tests_require,
           'testing': testing_extras,
       },
       ext_modules=ext_modules,
       keywords=['interface', 'components', 'plugins'],
 )
```

### Comparing `zope.interface-6.1a2/src/zope/interface/__init__.py` & `zope.interface-6.2/src/zope/interface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,45 +49,42 @@
 See the module doc strings for more information.
 """
 __docformat__ = 'restructuredtext'
 # pylint:disable=wrong-import-position,unused-import
 from zope.interface.interface import Interface
 from zope.interface.interface import _wire
 
+
 # Need to actually get the interface elements to implement the right interfaces
 _wire()
 del _wire
 
 from zope.interface.declarations import Declaration
+# The following are to make spec pickles cleaner
+from zope.interface.declarations import Provides
 from zope.interface.declarations import alsoProvides
 from zope.interface.declarations import classImplements
 from zope.interface.declarations import classImplementsFirst
 from zope.interface.declarations import classImplementsOnly
 from zope.interface.declarations import directlyProvidedBy
 from zope.interface.declarations import directlyProvides
 from zope.interface.declarations import implementedBy
 from zope.interface.declarations import implementer
 from zope.interface.declarations import implementer_only
 from zope.interface.declarations import moduleProvides
 from zope.interface.declarations import named
 from zope.interface.declarations import noLongerProvides
 from zope.interface.declarations import providedBy
 from zope.interface.declarations import provider
-
 from zope.interface.exceptions import Invalid
-
 from zope.interface.interface import Attribute
 from zope.interface.interface import interfacemethod
 from zope.interface.interface import invariant
 from zope.interface.interface import taggedValue
-
-# The following are to make spec pickles cleaner
-from zope.interface.declarations import Provides
-
-
 from zope.interface.interfaces import IInterfaceDeclaration
 
+
 moduleProvides(IInterfaceDeclaration)
 
 __all__ = ('Interface', 'Attribute') + tuple(IInterfaceDeclaration)
 
 assert all(k in globals() for k in __all__)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/_compat.py` & `zope.interface-6.2/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/_flatten.py` & `zope.interface-6.2/src/zope/interface/_flatten.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ##############################################################################
 """Adapter-style interface registry
 
 See Adapter class.
 """
 from zope.interface import Declaration
 
+
 def _flatten(implements, include_None=0):
 
     try:
         r = implements.flattened()
     except AttributeError:
         if implements is None:
             r=()
```

### Comparing `zope.interface-6.1a2/src/zope/interface/_zope_interface_coptimizations.c` & `zope.interface-6.2/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files 1% similar despite different names*

```diff
@@ -1973,42 +1973,35 @@
    "Get an object's interfaces (internal api)"},
   {"providedBy", (PyCFunction)providedBy, METH_O,
    "Get an object's interfaces"},
 
   {NULL,         (PyCFunction)NULL, 0, NULL}            /* sentinel */
 };
 
-#if  PY_MAJOR_VERSION >= 3
 static char module_doc[] = "C optimizations for zope.interface\n\n";
 
 static struct PyModuleDef _zic_module = {
         PyModuleDef_HEAD_INIT,
         "_zope_interface_coptimizations",
         module_doc,
         -1,
         m_methods,
         NULL,
         NULL,
         NULL,
         NULL
 };
-#endif
 
 static PyObject *
 init(void)
 {
   PyObject *m;
 
-#if  PY_MAJOR_VERSION < 3
-#define DEFINE_STRING(S) \
-  if(! (str ## S = PyString_FromString(# S))) return NULL
-#else
 #define DEFINE_STRING(S) \
   if(! (str ## S = PyUnicode_FromString(# S))) return NULL
-#endif
 
   DEFINE_STRING(__dict__);
   DEFINE_STRING(__implemented__);
   DEFINE_STRING(__provides__);
   DEFINE_STRING(__class__);
   DEFINE_STRING(__providedBy__);
   DEFINE_STRING(extends);
@@ -2050,21 +2043,15 @@
   if (PyType_Ready(&LookupBase) < 0)
     return NULL;
 
   VerifyingBase.tp_new = PyBaseObject_Type.tp_new;
   if (PyType_Ready(&VerifyingBase) < 0)
     return NULL;
 
-  #if PY_MAJOR_VERSION < 3
-  /* Create the module and add the functions */
-  m = Py_InitModule3("_zope_interface_coptimizations", m_methods,
-                     "C optimizations for zope.interface\n\n");
-  #else
   m = PyModule_Create(&_zic_module);
-  #endif
   if (m == NULL)
     return NULL;
 
   /* Add types: */
   if (PyModule_AddObject(m, "SpecificationBase", OBJECT(&SpecificationBaseType)) < 0)
     return NULL;
   if (PyModule_AddObject(m, "ObjectSpecificationDescriptor",
@@ -2080,22 +2067,15 @@
     return NULL;
   if (PyModule_AddObject(m, "adapter_hooks", adapter_hooks) < 0)
     return NULL;
   return m;
 }
 
 PyMODINIT_FUNC
-#if PY_MAJOR_VERSION < 3
-init_zope_interface_coptimizations(void)
-{
-  init();
-}
-#else
 PyInit__zope_interface_coptimizations(void)
 {
   return init();
 }
-#endif
 
 #ifdef __clang__
 #pragma clang diagnostic pop
 #endif
```

### Comparing `zope.interface-6.1a2/src/zope/interface/adapter.py` & `zope.interface-6.2/src/zope/interface/adapter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 #
 ##############################################################################
 """Adapter management
 """
 import itertools
 import weakref
 
+from zope.interface import Interface
 from zope.interface import implementer
 from zope.interface import providedBy
-from zope.interface import Interface
 from zope.interface import ro
-from zope.interface.interfaces import IAdapterRegistry
-
 from zope.interface._compat import _normalize_name
 from zope.interface._compat import _use_c_impl
+from zope.interface.interfaces import IAdapterRegistry
+
 
 __all__ = [
     'AdapterRegistry',
     'VerifyingAdapterRegistry',
 ]
 
 # In the CPython implementation,
```

### Comparing `zope.interface-6.1a2/src/zope/interface/advice.py` & `zope.interface-6.2/src/zope/interface/advice.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 not require) Zope 3 and Twisted.  It provides tools for manipulating UML
 models, object-relational persistence, aspect-oriented programming, and more.
 Visit the PEAK home page at http://peak.telecommunity.com for more information.
 """
 
 from types import FunctionType
 
+
 __all__ = [
     'determineMetaclass',
     'getFrameInfo',
     'isClassAdvisor',
     'minimalBases',
 ]
 
 import sys
 
+
 def getFrameInfo(frame):
     """Return (kind,module,locals,globals) for a frame
 
     'kind' is one of "exec", "module", "class", "function call", or "unknown".
     """
 
     f_locals = frame.f_locals
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/__init__.py` & `zope.interface-6.2/src/zope/interface/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 
 import itertools
 from types import FunctionType
 
-from zope.interface import classImplements
 from zope.interface import Interface
-from zope.interface.interface import fromFunction
+from zope.interface import classImplements
 from zope.interface.interface import InterfaceClass
 from zope.interface.interface import _decorator_non_return
+from zope.interface.interface import fromFunction
+
 
 __all__ = [
     # Nothing public here.
 ]
 
 
 # pylint:disable=inherit-non-class,
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/builtins.py` & `zope.interface-6.2/src/zope/interface/common/builtins.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 After this module is imported, the standard library types will declare
 that they implement the appropriate interface.
 
 .. versionadded:: 5.0.0
 """
 
 from zope.interface import classImplements
-
 from zope.interface.common import collections
-from zope.interface.common import numbers
 from zope.interface.common import io
+from zope.interface.common import numbers
+
 
 __all__ = [
     'IList',
     'ITuple',
     'ITextString',
     'IByteString',
     'INativeString',
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/collections.py` & `zope.interface-6.2/src/zope/interface/common/collections.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
     - `range.index` does not accept the ``start`` and ``stop`` arguments.
 
 .. versionadded:: 5.0.0
 """
 
 import sys
-
 from abc import ABCMeta
-from collections import abc
 from collections import OrderedDict
-from collections import UserList
 from collections import UserDict
+from collections import UserList
 from collections import UserString
+from collections import abc
 
 from zope.interface.common import ABCInterface
 from zope.interface.common import optional
 
+
 # pylint:disable=inherit-non-class,
 # pylint:disable=no-self-argument,no-method-argument
 # pylint:disable=unexpected-special-method-signature
 # pylint:disable=no-value-for-parameter
 
 
 def _new_in_ver(name, ver,
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/idatetime.py` & `zope.interface-6.2/src/zope/interface/common/idatetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 """Datetime interfaces.
 
 This module is called idatetime because if it were called datetime the import
 of the real datetime would fail.
 """
-from datetime import timedelta, date, datetime, time, tzinfo
+from datetime import date
+from datetime import datetime
+from datetime import time
+from datetime import timedelta
+from datetime import tzinfo
 
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
 from zope.interface import classImplements
 
 
 class ITimeDeltaClass(Interface):
     """This is the timedelta class interface.
 
     This is symbolic; this module does **not** make
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/interfaces.py` & `zope.interface-6.2/src/zope/interface/common/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 ##############################################################################
 """Interfaces for standard python exceptions
 """
 from zope.interface import Interface
 from zope.interface import classImplements
 
+
 class IException(Interface):
     "Interface for `Exception`"
 classImplements(Exception, IException)
 
 
 class IStandardError(IException):
     "Interface for `StandardError` (no longer existing.)"
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/io.py` & `zope.interface-6.2/src/zope/interface/common/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .. versionadded:: 5.0.0
 """
 
 import io as abc
 
 from zope.interface.common import ABCInterface
 
+
 # pylint:disable=inherit-non-class,
 # pylint:disable=no-member
 
 class IIOBase(ABCInterface):
     abc = abc.IOBase
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/mapping.py` & `zope.interface-6.2/src/zope/interface/common/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 The standard library :class:`dict` and :class:`collections.UserDict`
 implement ``IMutableMapping``, but *do not* implement any of the
 interfaces in this module.
 """
 from zope.interface import Interface
 from zope.interface.common import collections
 
+
 class IItemMapping(Interface):
     """Simplest readable mapping object
     """
 
     def __getitem__(key):
         """Get a value for a key
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/numbers.py` & `zope.interface-6.2/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/common/sequence.py` & `zope.interface-6.2/src/zope/interface/common/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 in this module.
 """
 
 __docformat__ = 'restructuredtext'
 from zope.interface import Interface
 from zope.interface.common import collections
 
+
 class IMinimalSequence(collections.IIterable):
     """Most basic sequence interface.
 
     All sequences are iterable.  This requires at least one of the
     following:
 
     - a `__getitem__()` method that takes a single argument; integer
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/__init__.py` & `zope.interface-6.2/src/zope/interface/common/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 
 import unittest
 
-from zope.interface.verify import verifyClass
-from zope.interface.verify import verifyObject
-
 from zope.interface.common import ABCInterface
 from zope.interface.common import ABCInterfaceClass
+from zope.interface.verify import verifyClass
+from zope.interface.verify import verifyObject
 
 
 def iter_abc_interfaces(predicate=lambda iface: True):
     # Iterate ``(iface, classes)``, where ``iface`` is a descendent of
     # the ABCInterfaceClass passing the *predicate* and ``classes`` is
     # an iterable of classes registered to conform to that interface.
     #
@@ -68,17 +67,17 @@
             )
             name = 'test_auto_' + suffix
             test.__name__ = name
             assert not hasattr(cls, name), (name, list(cls.__dict__))
             setattr(cls, name, test)
 
             def test_ro(self, stdlib_class=stdlib_class, iface=iface):
-                from zope.interface import ro
-                from zope.interface import implementedBy
                 from zope.interface import Interface
+                from zope.interface import implementedBy
+                from zope.interface import ro
                 self.assertEqual(
                     tuple(ro.ro(iface, strict=True)),
                     iface.__sro__)
                 implements = implementedBy(stdlib_class)
                 sro = implements.__sro__
                 self.assertIs(sro[-1], Interface)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/basemapping.py` & `zope.interface-6.2/src/zope/interface/common/tests/basemapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Base Mapping tests
 """
 from operator import __getitem__
 
+
 def testIReadMapping(self, inst, state, absent):
     for key in state:
         self.assertEqual(inst[key], state[key])
         self.assertEqual(inst.get(key, None), state[key])
         self.assertTrue(key in inst)
 
     for key in absent:
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_builtins.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_collections.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,34 +9,28 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 
 
 import array
 import unittest
+from collections import OrderedDict
 from collections import abc
 from collections import deque
-from collections import OrderedDict
-
-
 from types import MappingProxyType
 
 from zope.interface import Invalid
-
-
+from zope.interface._compat import PYPY
 # Note that importing z.i.c.collections does work on import.
 from zope.interface.common import collections
 
-
-from zope.interface._compat import PYPY
-
-
-from . import add_abc_interface_tests
 from . import VerifyClassMixin
 from . import VerifyObjectMixin
+from . import add_abc_interface_tests
+
 
 class TestVerifyClass(VerifyClassMixin, unittest.TestCase):
 
     # Here we test some known builtin classes that are defined to implement
     # various collection interfaces as a quick sanity test.
     def test_frozenset(self):
         self.assertIsInstance(frozenset(), abc.Set)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_idatetime.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_idatetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,32 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test for datetime interfaces
 """
 
 import unittest
+from datetime import date
+from datetime import datetime
+from datetime import time
+from datetime import timedelta
+from datetime import tzinfo
+
+from zope.interface.common.idatetime import IDate
+from zope.interface.common.idatetime import IDateClass
+from zope.interface.common.idatetime import IDateTime
+from zope.interface.common.idatetime import IDateTimeClass
+from zope.interface.common.idatetime import ITime
+from zope.interface.common.idatetime import ITimeClass
+from zope.interface.common.idatetime import ITimeDelta
+from zope.interface.common.idatetime import ITimeDeltaClass
+from zope.interface.common.idatetime import ITZInfo
+from zope.interface.verify import verifyClass
+from zope.interface.verify import verifyObject
 
-from zope.interface.verify import verifyObject, verifyClass
-from zope.interface.common.idatetime import ITimeDelta, ITimeDeltaClass
-from zope.interface.common.idatetime import IDate, IDateClass
-from zope.interface.common.idatetime import IDateTime, IDateTimeClass
-from zope.interface.common.idatetime import ITime, ITimeClass, ITZInfo
-from datetime import timedelta, date, datetime, time, tzinfo
 
 class TestDateTimeInterfaces(unittest.TestCase):
 
     def test_interfaces(self):
         verifyObject(ITimeDelta, timedelta(minutes=20))
         verifyObject(IDate, date(2000, 1, 2))
         verifyObject(IDateTime, datetime(2000, 1, 2, 10, 20))
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_import_interfaces.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
+
 class TestInterfaceImport(unittest.TestCase):
 
     def test_import(self):
         import zope.interface.common.interfaces as x
         self.assertIsNotNone(x)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_io.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_io.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 
 
-import unittest
 import io as abc
+import unittest
 
 # Note that importing z.i.c.io does work on import.
 from zope.interface.common import io
 
-from . import add_abc_interface_tests
 from . import VerifyClassMixin
 from . import VerifyObjectMixin
+from . import add_abc_interface_tests
 
 
 class TestVerifyClass(VerifyClassMixin,
                       unittest.TestCase):
     pass
 
 add_abc_interface_tests(TestVerifyClass, io.IIOBase.__module__)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/common/tests/test_numbers.py` & `zope.interface-6.2/src/zope/interface/common/tests/test_numbers.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 ##############################################################################
 
 
-import unittest
 import numbers as abc
+import unittest
 
 # Note that importing z.i.c.numbers does work on import.
 from zope.interface.common import numbers
 
-from . import add_abc_interface_tests
 from . import VerifyClassMixin
 from . import VerifyObjectMixin
+from . import add_abc_interface_tests
 
 
 class TestVerifyClass(VerifyClassMixin,
                       unittest.TestCase):
 
     def test_int(self):
         self.assertIsInstance(int(), abc.Integral)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/declarations.py` & `zope.interface-6.2/src/zope/interface/declarations.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,26 @@
   - ProvidesDeclarations are used to express interfaces directly
     provided by objects.
 
 """
 __docformat__ = 'restructuredtext'
 
 import sys
+import weakref
 from types import FunctionType
 from types import MethodType
 from types import ModuleType
-import weakref
 
+from zope.interface._compat import _use_c_impl
 from zope.interface.interface import Interface
 from zope.interface.interface import InterfaceClass
-from zope.interface.interface import SpecificationBase
-from zope.interface.interface import Specification
 from zope.interface.interface import NameAndModuleComparisonMixin
-from zope.interface._compat import _use_c_impl
+from zope.interface.interface import Specification
+from zope.interface.interface import SpecificationBase
+
 
 __all__ = [
     # None. The public APIs of this module are
     # re-exported from zope.interface directly.
 ]
 
 # pylint:disable=too-many-lines
@@ -785,15 +786,19 @@
 ProvidesClass = Provides
 
 # Registry of instance declarations
 # This is a memory optimization to allow objects to share specifications.
 InstanceDeclarations = weakref.WeakValueDictionary()
 
 def Provides(*interfaces): # pylint:disable=function-redefined
-    """Cache instance declarations
+    """Declaration for an instance of *cls*.
+
+       The correct signature is ``cls, *interfaces``.
+       The *cls* is necessary to avoid the
+       construction of inconsistent resolution orders.
 
       Instance declarations are shared among instances that have the same
       declaration. The declarations are cached in a weak value dictionary.
     """
     spec = InstanceDeclarations.get(interfaces)
     if spec is None:
         spec = ProvidesClass(*interfaces)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/document.py` & `zope.interface-6.2/src/zope/interface/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """ Pretty-Print an Interface object as structured text (Yum)
 
 This module provides a function, asStructuredText, for rendering an
 interface as structured text.
 """
 import zope.interface
 
+
 __all__ = [
     'asReStructuredText',
     'asStructuredText',
 ]
 
 def asStructuredText(I, munge=0, rst=False):
     """ Output structured text format.  Note, this will whack any existing
```

### Comparing `zope.interface-6.1a2/src/zope/interface/exceptions.py` & `zope.interface-6.2/src/zope/interface/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     def mess(self):
         return self.args[1] # pylint:disable=unsubscriptable-object
 
     @staticmethod
     def __implementation_str(impl):
         # It could be a callable or some arbitrary object, we don't
         # know yet.
-        import inspect # Inspect is a heavy-weight dependency, lots of imports
+        import inspect  # Inspect is a heavy-weight dependency, lots of imports
         try:
             sig = inspect.signature
             formatsig = str
         except AttributeError:
             sig = inspect.getargspec
             f = inspect.formatargspec
             formatsig = lambda sig: f(*sig) # pylint:disable=deprecated-method
```

### Comparing `zope.interface-6.1a2/src/zope/interface/interface.py` & `zope.interface-6.2/src/zope/interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Interface object implementation
 """
 # pylint:disable=protected-access
 import sys
-from types import MethodType
-from types import FunctionType
 import weakref
+from types import FunctionType
+from types import MethodType
+from typing import Union
 
+from zope.interface import ro
 from zope.interface._compat import _use_c_impl
 from zope.interface.exceptions import Invalid
 from zope.interface.ro import ro as calculate_ro
-from zope.interface import ro
+
 
 __all__ = [
     # Most of the public API from this module is directly exported
     # from zope.interface. The only remaining public API intended to
     # be imported from here should be those few things documented as
     # such.
     'InterfaceClass',
@@ -937,14 +939,22 @@
             # This clever trick is from Phillip Eby
 
         return None # pragma: no cover
 
     def __reduce__(self):
         return self.__name__
 
+    def __or__(self, other):
+        """Allow type hinting syntax: Interface | None."""
+        return Union[self, other]
+
+    def __ror__(self, other):
+        """Allow type hinting syntax: None | Interface."""
+        return Union[other, self]
+
 Interface = InterfaceClass("Interface", __module__='zope.interface')
 # Interface is the only member of its own SRO.
 Interface._calculate_sro = lambda: (Interface,)
 Interface.changed(Interface)
 assert Interface.__sro__ == (Interface,)
 Specification._ROOT = Interface
 ro._ROOT = Interface
@@ -1117,15 +1127,16 @@
     classImplements(InterfaceClass, IInterface)
 
 
 # We import this here to deal with module dependencies.
 # pylint:disable=wrong-import-position
 from zope.interface.declarations import implementedBy
 from zope.interface.declarations import providedBy
-from zope.interface.exceptions import InvalidInterface
 from zope.interface.exceptions import BrokenImplementation
+from zope.interface.exceptions import InvalidInterface
+
 
 # This ensures that ``Interface`` winds up in the flattened()
 # list of the immutable declaration. It correctly overrides changed()
 # as a no-op, so we bypass that.
 from zope.interface.declarations import _empty
 Specification.changed(_empty, _empty)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/interfaces.py` & `zope.interface-6.2/src/zope/interface/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Interface Package Interfaces
 """
 __docformat__ = 'restructuredtext'
 
+from zope.interface.declarations import implementer
 from zope.interface.interface import Attribute
 from zope.interface.interface import Interface
-from zope.interface.declarations import implementer
+
 
 __all__ = [
     'ComponentLookupError',
     'IAdapterRegistration',
     'IAdapterRegistry',
     'IAttribute',
     'IComponentLookup',
```

### Comparing `zope.interface-6.1a2/src/zope/interface/registry.py` & `zope.interface-6.2/src/zope/interface/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,35 +11,36 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Basic components support
 """
 from collections import defaultdict
 
+
 try:
     from zope.event import notify
 except ImportError: # pragma: no cover
     def notify(*arg, **kw): pass
 
-from zope.interface.interfaces import ISpecification
+from zope.interface.adapter import AdapterRegistry
+from zope.interface.declarations import implementedBy
+from zope.interface.declarations import implementer
+from zope.interface.declarations import implementer_only
+from zope.interface.declarations import providedBy
+from zope.interface.interface import Interface
 from zope.interface.interfaces import ComponentLookupError
 from zope.interface.interfaces import IAdapterRegistration
 from zope.interface.interfaces import IComponents
 from zope.interface.interfaces import IHandlerRegistration
+from zope.interface.interfaces import ISpecification
 from zope.interface.interfaces import ISubscriptionAdapterRegistration
 from zope.interface.interfaces import IUtilityRegistration
 from zope.interface.interfaces import Registered
 from zope.interface.interfaces import Unregistered
 
-from zope.interface.interface import Interface
-from zope.interface.declarations import implementedBy
-from zope.interface.declarations import implementer
-from zope.interface.declarations import implementer_only
-from zope.interface.declarations import providedBy
-from zope.interface.adapter import AdapterRegistry
 
 __all__ = [
     # Components is public API, but
     # the *Registration classes are just implementations
     # of public interfaces.
     'Components',
 ]
```

### Comparing `zope.interface-6.1a2/src/zope/interface/ro.py` & `zope.interface-6.2/src/zope/interface/ro.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,14 +450,15 @@
     __slots__ = ()
     def _guess_next_base(self, base_tree_remaining):
         import traceback
         bad_iros = C3.BAD_IROS
         if self.leaf not in bad_iros:
             if bad_iros == ():
                 import weakref
+
                 # This is a race condition, but it doesn't matter much.
                 bad_iros = C3.BAD_IROS = weakref.WeakKeyDictionary()
             bad_iros[self.leaf] = t = (
                 InconsistentResolutionOrderError(self, base_tree_remaining),
                 traceback.format_stack()
             )
             _logger().warning("Tracking inconsistent IRO: %s", t[0])
@@ -523,14 +524,15 @@
         for x in chunk:
             to_.append(operation(x))
             from_.append(self.Empty())
 
     def _generate_report(self):
         if self._c3_report is None:
             import difflib
+
             # The opcodes we get describe how to turn 'a' into 'b'. So
             # the old one (legacy) needs to be first ('a')
             matcher = difflib.SequenceMatcher(None, self.legacy_ro, self.c3_ro)
             # The reports are equal length sequences. We're going for a
             # side-by-side diff.
             self._c3_report = c3_report = []
             self._legacy_report = legacy_report = []
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/__init__.py` & `zope.interface-6.2/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/advisory_testing.py` & `zope.interface-6.2/src/zope/interface/tests/advisory_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import sys
 
 from zope.interface.advice import getFrameInfo
 
+
 my_globals = globals()
 
 ClassicClass = None
 
 class NewStyleClass:
     __metaclass__ = type
     classLevelFrameInfo = getFrameInfo(sys._getframe())
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/dummy.py` & `zope.interface-6.2/src/zope/interface/tests/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 #
 ##############################################################################
 """ Dummy Module
 """
 from zope.interface import moduleProvides
 from zope.interface.tests.idummy import IDummyModule
 
+
 moduleProvides(IDummyModule)
 
 def bar(baz):
     # Note:  no 'self', because the module provides the interface directly.
     raise NotImplementedError()
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/idummy.py` & `zope.interface-6.2/src/zope/interface/tests/idummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Interface describing API of zope.interface.tests.dummy test module
 """
 from zope.interface import Interface
 
+
 class IDummyModule(Interface):
     """ Dummy interface for unit tests.
     """
     def bar(baz):
         """ Just a note.
         """
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/m1.py` & `zope.interface-6.2/src/zope/interface/tests/m1.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test module that declares an interface
 """
-from zope.interface import Interface, moduleProvides
+from zope.interface import Interface
+from zope.interface import moduleProvides
+
 
 class I1(Interface): pass
 class I2(Interface): pass
 
 moduleProvides(I1, I2)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/odd.py` & `zope.interface-6.2/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_adapter.py` & `zope.interface-6.2/src/zope/interface/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ##############################################################################
 """Adapter registry tests
 """
 import unittest
 
 from zope.interface.tests import OptimizationTestMixin
 
+
 # pylint:disable=inherit-non-class,protected-access,too-many-lines
 # pylint:disable=attribute-defined-outside-init,blacklisted-name
 
 def _makeInterfaces():
     from zope.interface import Interface
 
     class IB0(Interface):
@@ -870,15 +871,15 @@
     def assertLeafIdentity(self, leaf1, leaf2):
         self.assertIs(leaf1, leaf2)
 
 
 class LookupBaseFallbackTests(unittest.TestCase):
 
     def _getFallbackClass(self):
-        from zope.interface.adapter import LookupBaseFallback # pylint:disable=no-name-in-module
+        from zope.interface.adapter import LookupBaseFallback
         return LookupBaseFallback
 
     _getTargetClass = _getFallbackClass
 
     def _makeOne(self, uc_lookup=None, uc_lookupAll=None,
                  uc_subscriptions=None):
         # pylint:disable=function-redefined
@@ -1207,15 +1208,15 @@
         from zope.interface.adapter import LookupBase
         return LookupBase
 
 
 class VerifyingBaseFallbackTests(unittest.TestCase):
 
     def _getFallbackClass(self):
-        from zope.interface.adapter import VerifyingBaseFallback # pylint:disable=no-name-in-module
+        from zope.interface.adapter import VerifyingBaseFallback
         return VerifyingBaseFallback
 
     _getTargetClass = _getFallbackClass
 
     def _makeOne(self, registry, uc_lookup=None, uc_lookupAll=None,
                  uc_subscriptions=None):
         # pylint:disable=function-redefined
@@ -1998,16 +1999,16 @@
         from zope.interface.adapter import VerifyingAdapterRegistry
         return VerifyingAdapterRegistry
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def test_verify_object_provides_IAdapterRegistry(self):
-        from zope.interface.verify import verifyObject
         from zope.interface.interfaces import IAdapterRegistry
+        from zope.interface.verify import verifyObject
         registry = self._makeOne()
         verifyObject(IAdapterRegistry, registry)
 
 
 class AdapterRegistryTests(VerifyingAdapterRegistryTests):
 
     def _getTargetClass(self):
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_advice.py` & `zope.interface-6.2/src/zope/interface/tests/test_advice.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 PEAK is a Python application framework that interoperates with (but does
 not require) Zope 3 and Twisted.  It provides tools for manipulating UML
 models, object-relational persistence, aspect-oriented programming, and more.
 Visit the PEAK home page at http://peak.telecommunity.com for more information.
 """
 
-import unittest
 import sys
+import unittest
 
 
 class FrameInfoTest(unittest.TestCase):
 
     def test_w_module(self):
         from zope.interface.tests import advisory_testing
         (kind, module,
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_compile_flags.py` & `zope.interface-6.2/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_declarations.py` & `zope.interface-6.2/src/zope/interface/tests/test_declarations.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test the new API for making and checking interface declarations
 """
 import unittest
 
-from zope.interface.tests import OptimizationTestMixin
 from zope.interface.tests import MissingSomeAttrs
-from zope.interface.tests.test_interface import NameAndModuleComparisonTestsMixin
+from zope.interface.tests import OptimizationTestMixin
+from zope.interface.tests.test_interface import \
+    NameAndModuleComparisonTestsMixin
+
 
 # pylint:disable=inherit-non-class,too-many-lines,protected-access
 # pylint:disable=blacklisted-name,attribute-defined-outside-init
 
 class _Py3ClassAdvice:
 
     def _run_generated_code(self, code, globs, locs,
@@ -286,17 +288,17 @@
     def test___add___overlapping_interface(self):
         # The derived interfaces end up with higher priority, and
         # don't produce a C3 resolution order violation. This
         # example produced a C3 error, and the resulting legacy order
         # used to be wrong ([IBase, IDerived] instead of
         # the other way).
         from zope.interface import Interface
+        from zope.interface import ro
         from zope.interface.interface import InterfaceClass
         from zope.interface.tests.test_ro import C3Setting
-        from zope.interface import ro
 
         IBase = InterfaceClass('IBase')
         IDerived = InterfaceClass('IDerived', (IBase,))
 
         with C3Setting(ro.C3.STRICT_IRO, True):
             base = self._makeOne(IBase)
             after = base + IDerived
@@ -309,16 +311,16 @@
         # Like test___add___overlapping_interface, but pulling
         # in a realistic example. This one previously produced a
         # C3 error, but the resulting legacy order was (somehow)
         # correct.
         from zope.interface import Interface
         from zope.interface import implementedBy
         from zope.interface import implementer
-        from zope.interface.tests.test_ro import C3Setting
         from zope.interface import ro
+        from zope.interface.tests.test_ro import C3Setting
 
         class IBase(Interface):
             pass
 
         class IDerived(IBase):
             pass
 
@@ -786,16 +788,16 @@
             pass
 
         self.assertEqual(list(self._callFUT(Derived)), [IDerived])
 
         sup = super(Derived, Derived)
         self.assertEqual(list(self._callFUT(sup)), [])
     def test_super_multi_level_multi_inheritance(self):
-        from zope.interface.declarations import implementer
         from zope.interface import Interface
+        from zope.interface.declarations import implementer
 
         class IBase(Interface):
             pass
 
         class IM1(Interface):
             pass
 
@@ -1052,16 +1054,16 @@
 class Test__implements_advice(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.interface.declarations import _implements_advice
         return _implements_advice(*args, **kw)
 
     def test_no_existing_implements(self):
-        from zope.interface.declarations import classImplements
         from zope.interface.declarations import Implements
+        from zope.interface.declarations import classImplements
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass('IFoo')
         class Foo:
             __implements_advice_data__ = ((IFoo,), classImplements)
         self._callFUT(Foo)
         self.assertNotIn('__implements_advice_data__', Foo.__dict__)
         self.assertIsInstance(Foo.__implemented__, Implements) # pylint:disable=no-member
@@ -1104,14 +1106,15 @@
     def test_does_not_leak_on_unique_classes(self):
         # Make sure nothing is hanging on to the class or Implements
         # object after they go out of scope. There was briefly a bug
         # in 5.x that caused SpecificationBase._bases (in C) to not be
         # traversed or cleared.
         # https://github.com/zopefoundation/zope.interface/issues/216
         import gc
+
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass('IFoo')
 
         begin_count = len(gc.get_objects())
 
         for _ in range(1900):
             class TestClass:
@@ -1180,15 +1183,15 @@
         IFoo = InterfaceClass("IFoo")
         class Foo:
             pass
         spec = self._makeOne(Foo, IFoo)
         self.assertEqual(list(spec), [IFoo])
 
     def test___reduce__(self):
-        from zope.interface.declarations import Provides # the function
+        from zope.interface.declarations import Provides  # the function
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
         class Foo:
             pass
         spec = self._makeOne(Foo, IFoo)
         klass, args = spec.__reduce__()
         self.assertIs(klass, Provides)
@@ -1225,16 +1228,16 @@
             def _do_calculate_ro(self, base_mros):
                 return ProvidesClass._do_calculate_ro(self, base_mros=base_mros, strict=True)
         return StrictProvides
 
     def test_overlapping_interfaces_corrected(self):
         # Giving Provides(cls, IFace), where IFace is already
         # provided by cls, doesn't produce invalid resolution orders.
-        from zope.interface import implementedBy
         from zope.interface import Interface
+        from zope.interface import implementedBy
         from zope.interface import implementer
 
         class IBase(Interface):
             pass
 
         @implementer(IBase)
         class Base:
@@ -1283,26 +1286,28 @@
             repr(provides),
             "directlyProvides(sys.modules['zope.interface.tests.dummy'], IDummyModule)"
         )
 
     def test__repr__module_after_pickle(self):
         # It doesn't matter, these objects can't be pickled.
         import pickle
+
         from zope.interface.tests import dummy
         provides = dummy.__provides__ # pylint:disable=no-member
         for proto in range(pickle.HIGHEST_PROTOCOL + 1):
             with self.assertRaises(pickle.PicklingError):
                 pickle.dumps(provides, proto)
 
     def test__repr__directlyProvides_module(self):
         import sys
-        from zope.interface.tests import dummy
-        from zope.interface.declarations import directlyProvides
+
         from zope.interface.declarations import alsoProvides
+        from zope.interface.declarations import directlyProvides
         from zope.interface.interface import InterfaceClass
+        from zope.interface.tests import dummy
 
         IFoo = InterfaceClass('IFoo')
         IBar = InterfaceClass('IBar')
 
         orig_provides = dummy.__provides__ # pylint:disable=no-member
         del dummy.__provides__ # pylint:disable=no-member
         self.addCleanup(setattr, dummy, '__provides__', orig_provides)
@@ -1335,16 +1340,16 @@
             repr(provides),
             "directlyProvides(('zope.interface.tests.dummy', "
             "'zope.interface.tests.test_declarations'), "
             "IFoo, IBar)"
         )
 
     def test__repr__module_provides_cached_shared(self):
-        from zope.interface.interface import InterfaceClass
         from zope.interface.declarations import ModuleType
+        from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
 
         inst = self._makeOne(ModuleType, IFoo)
         inst._v_module_names += ('some.module',)
         inst._v_module_names += ('another.module',)
         self.assertEqual(
             repr(inst),
@@ -1413,17 +1418,17 @@
         inst = providedBy(Foo())
         self.assertEqual(
             repr(inst),
             'classImplements(Foo, IFoo)'
         )
 
     def test__repr__providedBy_alsoProvides(self):
+        from zope.interface.declarations import alsoProvides
         from zope.interface.declarations import implementer
         from zope.interface.declarations import providedBy
-        from zope.interface.declarations import alsoProvides
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
         IBar = InterfaceClass("IBar")
 
         @implementer(IFoo)
         class Foo:
             pass
@@ -1530,16 +1535,16 @@
             pass
         obj = Foo()
         self._callFUT(obj, IFoo)
         self.assertIsInstance(obj.__provides__, ProvidesClass) # pylint:disable=no-member
         self.assertEqual(list(obj.__provides__), [IFoo]) # pylint:disable=no-member
 
     def test_w_existing_provides(self):
-        from zope.interface.declarations import directlyProvides
         from zope.interface.declarations import ProvidesClass
+        from zope.interface.declarations import directlyProvides
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
         IBar = InterfaceClass("IBar")
         class Foo:
             pass
         obj = Foo()
         directlyProvides(obj, IFoo)
@@ -1700,16 +1705,16 @@
             def _do_calculate_ro(self, base_mros):
                 return ClassProvides._do_calculate_ro(self, base_mros=base_mros, strict=True)
         return StrictClassProvides
 
     def test_overlapping_interfaces_corrected(self):
         # Giving ClassProvides(cls, metaclass, IFace), where IFace is already
         # provided by metacls, doesn't produce invalid resolution orders.
-        from zope.interface import implementedBy
         from zope.interface import Interface
+        from zope.interface import implementedBy
         from zope.interface import implementer
 
         class IBase(Interface):
             pass
 
         @implementer(IBase)
         class metaclass(type):
@@ -1768,16 +1773,16 @@
         inst = self._makeOne(type(self), type, IFoo, IBaz, IFoo2)
         self.assertEqual(
             repr(inst),
             "directlyProvides(TestClassProvidesRepr, IFoo, IBaz, mod2.IFoo)"
         )
 
     def test__repr__implementedBy(self):
-        from zope.interface.declarations import implementer
         from zope.interface.declarations import implementedBy
+        from zope.interface.declarations import implementer
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
 
         @implementer(IFoo)
         class Foo:
             pass
 
@@ -1785,14 +1790,15 @@
         self.assertEqual(
             repr(inst),
             'classImplements(Foo, IFoo)'
         )
 
     def test__repr__implementedBy_generic_callable(self):
         from zope.interface.declarations import implementedBy
+
         # We can't get a __name__ by default, so we get a
         # module name and a question mark
         class Callable:
             def __call__(self):
                 return self
 
         inst = implementedBy(Callable())
@@ -2200,16 +2206,16 @@
         sup = super(Derived, derived)
         fut = self._callFUT(sup)
         self.assertIsNone(fut._dependents)
         self.assertEqual(list(fut), [])
 
     def test_super_when_object_directly_provides(self):
         from zope.interface import Interface
-        from zope.interface.declarations import implementer
         from zope.interface.declarations import directlyProvides
+        from zope.interface.declarations import implementer
 
         class IBase(Interface):
             pass
 
         class IDerived(IBase):
             pass
 
@@ -2228,16 +2234,16 @@
 
         sup = super(Derived, derived)
         fut = self._callFUT(sup)
         self.assertIsNone(fut._dependents)
         self.assertEqual(list(fut), [IBase])
 
     def test_super_multi_level_multi_inheritance(self):
-        from zope.interface.declarations import implementer
         from zope.interface import Interface
+        from zope.interface.declarations import implementer
 
         class IBase(Interface):
             pass
 
         class IM1(Interface):
             pass
 
@@ -2302,16 +2308,16 @@
         return providedBy
 
 
 class ObjectSpecificationDescriptorFallbackTests(unittest.TestCase):
 
     def _getFallbackClass(self):
         # pylint:disable=no-name-in-module
-        from zope.interface.declarations \
-            import ObjectSpecificationDescriptorFallback
+        from zope.interface.declarations import \
+            ObjectSpecificationDescriptorFallback
         return ObjectSpecificationDescriptorFallback
 
     _getTargetClass = _getFallbackClass
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
@@ -2322,31 +2328,31 @@
         class Foo:
             pass
         Foo.__provides__ = Provides(Foo, IFoo)
         Foo.__providedBy__ = self._makeOne()
         self.assertEqual(list(Foo.__providedBy__), [IFoo])
 
     def test_accessed_via_inst_wo_provides(self):
-        from zope.interface.declarations import implementer
         from zope.interface.declarations import Provides
+        from zope.interface.declarations import implementer
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
         IBar = InterfaceClass("IBar")
         @implementer(IFoo)
         class Foo:
             pass
         Foo.__provides__ = Provides(Foo, IBar)
         Foo.__providedBy__ = self._makeOne()
         foo = Foo()
         self.assertEqual(list(foo.__providedBy__), [IFoo])
 
     def test_accessed_via_inst_w_provides(self):
+        from zope.interface.declarations import Provides
         from zope.interface.declarations import directlyProvides
         from zope.interface.declarations import implementer
-        from zope.interface.declarations import Provides
         from zope.interface.interface import InterfaceClass
         IFoo = InterfaceClass("IFoo")
         IBar = InterfaceClass("IBar")
         IBaz = InterfaceClass("IBaz")
         @implementer(IFoo)
         class Foo:
             pass
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_document.py` & `zope.interface-6.2/src/zope/interface/tests/test_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Documentation tests.
 """
+import sys
 import unittest
 
 
 class Test_asStructuredText(unittest.TestCase):
 
     def _callFUT(self, iface):
         from zope.interface.document import asStructuredText
@@ -46,22 +47,26 @@
         class IEmpty(Interface):
             """ This is an empty interface.
             """
         self.assertEqual(self._callFUT(IEmpty), EXPECTED)
 
     def test_asStructuredText_empty_with_multiline_docstring(self):
         from zope.interface import Interface
+
+        # In Python 3.13+, compiler strips indents from docstrings
+        indent = " " * 12 if sys.version_info < (3, 13) else ""
+
         EXPECTED = '\n'.join([
             "IEmpty",
             "",
             " This is an empty interface.",
             " ",
-            ("             It can be used to annotate any class or object, "
+            (f"{indent} It can be used to annotate any class or object, "
                              "because it promises"),
-            "             nothing.",
+            f"{indent} nothing.",
             "",
             " Attributes:",
             "",
             " Methods:",
             "",
             ""
         ])
@@ -270,22 +275,26 @@
         class IEmpty(Interface):
             """ This is an empty interface.
             """
         self.assertEqual(self._callFUT(IEmpty), EXPECTED)
 
     def test_asReStructuredText_empty_with_multiline_docstring(self):
         from zope.interface import Interface
+
+        # In Python 3.13+, compiler strips indents from docstrings
+        indent = " " * 12 if sys.version_info < (3, 13) else ""
+
         EXPECTED = '\n'.join([
             "``IEmpty``",
             "",
             " This is an empty interface.",
             " ",
-            ("             It can be used to annotate any class or object, "
+            (f"{indent} It can be used to annotate any class or object, "
                              "because it promises"),
-            "             nothing.",
+            f"{indent} nothing.",
             "",
             " Attributes:",
             "",
             " Methods:",
             "",
             ""
         ])
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_element.py` & `zope.interface-6.2/src/zope/interface/tests/test_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test Element meta-class.
 """
 
 import unittest
+
 from zope.interface.interface import Element
 
+
 class TestElement(unittest.TestCase):
 
     def test_taggedValues(self):
         """Test that we can update tagged values of more than one element
         """
 
         e1 = Element("foo")
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_exceptions.py` & `zope.interface-6.2/src/zope/interface/tests/test_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ zope.interface.exceptions unit tests
 """
 import unittest
 
+
 def _makeIface():
     from zope.interface import Interface
     class IDummy(Interface):
         pass
     return IDummy
 
 class DoesNotImplementTests(unittest.TestCase):
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_interface.py` & `zope.interface-6.2/src/zope/interface/tests/test_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,39 +19,40 @@
 # pylint:disable=redefined-builtin,signature-differs,arguments-differ
 # Things you get inheriting from Interface
 # pylint:disable=inherit-non-class,no-self-argument,no-method-argument
 # Things you get using methods of an Interface 'subclass'
 # pylint:disable=no-value-for-parameter
 import unittest
 
+from zope.interface.tests import CleanUp
 from zope.interface.tests import MissingSomeAttrs
 from zope.interface.tests import OptimizationTestMixin
-from zope.interface.tests import CleanUp
+
 
 _marker = object()
 
 
 class Test_invariant(unittest.TestCase):
 
     def test_w_single(self):
-        from zope.interface.interface import invariant
         from zope.interface.interface import TAGGED_DATA
+        from zope.interface.interface import invariant
 
         def _check(*args, **kw):
             raise NotImplementedError()
 
         class Foo:
             invariant(_check)
 
         self.assertEqual(getattr(Foo, TAGGED_DATA, None),
                          {'invariants': [_check]})
 
     def test_w_multiple(self):
-        from zope.interface.interface import invariant
         from zope.interface.interface import TAGGED_DATA
+        from zope.interface.interface import invariant
 
         def _check(*args, **kw):
             raise NotImplementedError()
 
         def _another_check(*args, **kw):
             raise NotImplementedError()
 
@@ -62,37 +63,37 @@
         self.assertEqual(getattr(Foo, TAGGED_DATA, None),
                          {'invariants': [_check, _another_check]})
 
 
 class Test_taggedValue(unittest.TestCase):
 
     def test_w_single(self):
-        from zope.interface.interface import taggedValue
         from zope.interface.interface import TAGGED_DATA
+        from zope.interface.interface import taggedValue
 
         class Foo:
             taggedValue('bar', ['baz'])
 
         self.assertEqual(getattr(Foo, TAGGED_DATA, None),
                          {'bar': ['baz']})
 
     def test_w_multiple(self):
-        from zope.interface.interface import taggedValue
         from zope.interface.interface import TAGGED_DATA
+        from zope.interface.interface import taggedValue
 
         class Foo:
             taggedValue('bar', ['baz'])
             taggedValue('qux', 'spam')
 
         self.assertEqual(getattr(Foo, TAGGED_DATA, None),
                          {'bar': ['baz'], 'qux': 'spam'})
 
     def test_w_multiple_overwriting(self):
-        from zope.interface.interface import taggedValue
         from zope.interface.interface import TAGGED_DATA
+        from zope.interface.interface import taggedValue
 
         class Foo:
             taggedValue('bar', ['baz'])
             taggedValue('qux', 'spam')
             taggedValue('bar', 'frob')
 
         self.assertEqual(getattr(Foo, TAGGED_DATA, None),
@@ -170,15 +171,15 @@
         element = self._makeOne()
         verifyObject(IElement, element)
 
 
 class GenericSpecificationBaseTests(unittest.TestCase):
     # Tests that work with both implementations
     def _getFallbackClass(self):
-        from zope.interface.interface import SpecificationBasePy # pylint:disable=no-name-in-module
+        from zope.interface.interface import SpecificationBasePy
         return SpecificationBasePy
 
     _getTargetClass = _getFallbackClass
 
     def _makeOne(self):
         return self._getTargetClass()()
 
@@ -562,17 +563,17 @@
 
     def test_multiple_inheritance_no_interfaces(self):
         # If we extend an object that implements interfaces,
         # plus one that doesn't, we do not interject `Interface`
         # early in the resolution order. It stays at the end,
         # like it should.
         # See https://github.com/zopefoundation/zope.interface/issues/8
-        from zope.interface.interface import Interface
-        from zope.interface.declarations import implementer
         from zope.interface.declarations import implementedBy
+        from zope.interface.declarations import implementer
+        from zope.interface.interface import Interface
 
         class IDefaultViewName(Interface):
             pass
 
         class Context:
             pass
 
@@ -1145,16 +1146,16 @@
         with self.assertRaises(AttributeError):
             inst.__module__ = 'different.module'
 
 
 class InterfaceTests(unittest.TestCase):
 
     def test_attributes_link_to_interface(self):
-        from zope.interface import Interface
         from zope.interface import Attribute
+        from zope.interface import Interface
 
         class I1(Interface):
             attr = Attribute("My attr")
 
         self.assertTrue(I1['attr'].interface is I1)
 
     def test_methods_link_to_interface(self):
@@ -1429,16 +1430,16 @@
         self.assertEqual(sorted(IDerived.names()),
                          ['attr2', 'method', 'method2'])
         self.assertEqual(sorted(IDerived.names(all=True)),
                          ['attr', 'attr2', 'method', 'method2'])
 
     def test_namesAndDescriptions_simple(self):
         from zope.interface import Attribute
-        from zope.interface.interface import Method
         from zope.interface import Interface
+        from zope.interface.interface import Method
 
 
         class ISimple(Interface):
             attr = Attribute('My attr')
 
             def method():
                 "My method"
@@ -1518,16 +1519,16 @@
         class IEmpty(Interface):
             pass
 
         self.assertRaises(KeyError, IEmpty.getDescriptionFor, 'nonesuch')
 
     def test_getDescriptionFor_simple(self):
         from zope.interface import Attribute
-        from zope.interface.interface import Method
         from zope.interface import Interface
+        from zope.interface.interface import Method
 
 
         class ISimple(Interface):
             attr = Attribute('My attr')
 
             def method():
                 "My method"
@@ -1540,16 +1541,16 @@
         m_desc = ISimple.getDescriptionFor('method')
         self.assertTrue(isinstance(m_desc, Method))
         self.assertEqual(m_desc.__name__, 'method')
         self.assertEqual(m_desc.__doc__, 'My method')
 
     def test_getDescriptionFor_derived(self):
         from zope.interface import Attribute
-        from zope.interface.interface import Method
         from zope.interface import Interface
+        from zope.interface.interface import Method
 
 
         class IBase(Interface):
             attr = Attribute('My attr')
 
             def method():
                 "My method"
@@ -1589,16 +1590,16 @@
         class IEmpty(Interface):
             pass
 
         self.assertRaises(KeyError, IEmpty.__getitem__, 'nonesuch')
 
     def test___getitem__simple(self):
         from zope.interface import Attribute
-        from zope.interface.interface import Method
         from zope.interface import Interface
+        from zope.interface.interface import Method
 
 
         class ISimple(Interface):
             attr = Attribute('My attr')
 
             def method():
                 "My method"
@@ -1611,16 +1612,16 @@
         m_desc = ISimple['method']
         self.assertTrue(isinstance(m_desc, Method))
         self.assertEqual(m_desc.__name__, 'method')
         self.assertEqual(m_desc.__doc__, 'My method')
 
     def test___getitem___derived(self):
         from zope.interface import Attribute
-        from zope.interface.interface import Method
         from zope.interface import Interface
+        from zope.interface.interface import Method
 
 
         class IBase(Interface):
             attr = Attribute('My attr')
 
             def method():
                 "My method"
@@ -1919,16 +1920,16 @@
         has_invariant.foo = 1
         has_invariant.bar = 2
         self.assertEqual(IInvariant.validateInvariants(has_invariant), None)
         # clean up
         IInvariant.setTaggedValue('invariants', old_invariants)
 
     def test___doc___element(self):
-        from zope.interface import Interface
         from zope.interface import Attribute
+        from zope.interface import Interface
         class IDocstring(Interface):
             "xxx"
 
         self.assertEqual(IDocstring.__doc__, "xxx")
         self.assertEqual(list(IDocstring), [])
 
         class IDocstringAndAttribute(Interface):
@@ -1936,16 +1937,16 @@
 
             __doc__ = Attribute('the doc')
 
         self.assertEqual(IDocstringAndAttribute.__doc__, "")
         self.assertEqual(list(IDocstringAndAttribute), ['__doc__'])
 
     def test_invariant_as_decorator(self):
-        from zope.interface import Interface
         from zope.interface import Attribute
+        from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import invariant
         from zope.interface.exceptions import Invalid
 
         class IRange(Interface):
             min = Attribute("Lower bound")
             max = Attribute("Upper bound")
@@ -1990,16 +1991,16 @@
         self.assertEqual(list(ITagged.getTaggedValueTags()), ['qux'])
 
         self.assertEqual(IDerived2.getTaggedValue('qux'), 'Spam Spam')
         self.assertEqual(IDerived2.getTaggedValue('foo'), 'bar')
         self.assertEqual(set(IDerived2.getTaggedValueTags()), {'qux', 'foo'})
 
     def _make_taggedValue_tree(self, base):
-        from zope.interface import taggedValue
         from zope.interface import Attribute
+        from zope.interface import taggedValue
         O = base
         class F(O):
             taggedValue('tag', 'F')
             tag = Attribute('F')
         class E(O):
             taggedValue('tag', 'E')
             tag = Attribute('E')
@@ -2059,16 +2060,16 @@
         self.assertEqual(C.getDirectTaggedValue('tag'), 'C')
         self.assertEqual(['tag'], list(C.getDirectTaggedValueTags()))
 
     def test_description_cache_management(self):
         # See https://bugs.launchpad.net/zope.interface/+bug/185974
         # There was a bug where the cache used by Specification.get() was not
         # cleared when the bases were changed.
-        from zope.interface import Interface
         from zope.interface import Attribute
+        from zope.interface import Interface
 
         class I1(Interface):
             a = Attribute('a')
 
         class I2(I1):
             pass
 
@@ -2155,16 +2156,16 @@
         try:
             self.assertTrue(I(c) is self)
         finally:
             adapter_hooks[:] = old_adapter_hooks
 
     def test___call___w_overridden_adapt(self):
         from zope.interface import Interface
-        from zope.interface import interfacemethod
         from zope.interface import implementer
+        from zope.interface import interfacemethod
 
         class I(Interface):
 
             @interfacemethod
             def __adapt__(self, obj):
                 return 42
 
@@ -2177,16 +2178,16 @@
         # the interface if it chooses.
         self.assertEqual(42, I(O()))
 
     def test___call___w_overridden_adapt_and_conform(self):
         # Conform is first, taking precedence over __adapt__,
         # *if* it returns non-None
         from zope.interface import Interface
-        from zope.interface import interfacemethod
         from zope.interface import implementer
+        from zope.interface import interfacemethod
 
         class IAdapt(Interface):
             @interfacemethod
             def __adapt__(self, obj):
                 return 42
 
         class ISimple(Interface):
@@ -2211,17 +2212,18 @@
             ISimple(ConformNone())
 
         self.assertEqual(42, IAdapt(ConformNone()))
 
 
     def test___call___w_overridden_adapt_call_super(self):
         import sys
+
         from zope.interface import Interface
-        from zope.interface import interfacemethod
         from zope.interface import implementer
+        from zope.interface import interfacemethod
 
         class I(Interface):
 
             @interfacemethod
             def __adapt__(self, obj):
                 if not self.providedBy(obj):
                     return 42
@@ -2632,7 +2634,45 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for key, value in self.to_restore.items():
             setattr(self.module, key, value)
+
+class TestTypeAnnotations(unittest.TestCase):
+    """Test using Interfaces in type annotations."""
+
+    def test___or__(self):
+        from typing import Optional
+        from typing import Union
+
+        from zope.interface import Interface
+        class I1(Interface):
+            pass
+        class I2(Interface):
+            pass
+
+        class B:
+            a: I1|None
+            b: I1|I2
+
+        self.assertEqual(
+            B.__annotations__, {'a': Optional[I1], 'b': Union[I1, I2]})
+
+    def test___ror__(self):
+        from typing import Optional
+        from typing import Union
+
+        from zope.interface import Interface
+        class I1(Interface):
+            pass
+
+        class A:
+            pass
+
+        class B:
+            a: None|I1
+            b: A|I1
+
+        self.assertEqual(
+            B.__annotations__, {'a': Optional[I1], 'b': Union[A, I1]})
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_interfaces.py` & `zope.interface-6.2/src/zope/interface/tests/test_interfaces.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -118,11 +118,11 @@
         verifyObject(self._getTargetInterface(), self._makeOne())
 
     def test_instance_consistent__iro__(self):
         from zope.interface import ro
         self.assertTrue(ro.is_consistent(self._getTargetInterface()))
 
     def test_class_consistent__iro__(self):
-        from zope.interface import ro
         from zope.interface import implementedBy
+        from zope.interface import ro
 
         self.assertTrue(ro.is_consistent(implementedBy(self._getTargetClass())))
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_odd_declarations.py` & `zope.interface-6.2/src/zope/interface/tests/test_odd_declarations.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 """Test interface declarations against ExtensionClass-like classes.
 
 These tests are to make sure we do something sane in the presence of
 classic ExtensionClass classes and instances.
 """
 import unittest
 
-from zope.interface.tests import odd
 from zope.interface import Interface
-from zope.interface import implementer
-from zope.interface import directlyProvides
-from zope.interface import providedBy
-from zope.interface import directlyProvidedBy
 from zope.interface import classImplements
 from zope.interface import classImplementsOnly
+from zope.interface import directlyProvidedBy
+from zope.interface import directlyProvides
 from zope.interface import implementedBy
+from zope.interface import implementer
+from zope.interface import providedBy
+from zope.interface.tests import odd
+
 
 class I1(Interface): pass
 class I2(Interface): pass
 class I3(Interface): pass
 class I31(I3): pass
 class I4(Interface): pass
 class I5(Interface): pass
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_registry.py` & `zope.interface-6.2/src/zope/interface/tests/test_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ##############################################################################
 """Component Registry Tests"""
 # pylint:disable=protected-access
 import unittest
 
 from zope.interface import Interface
 from zope.interface.adapter import VerifyingAdapterRegistry
-
 from zope.interface.registry import Components
 
+
 class ComponentsTests(unittest.TestCase):
 
     def _getTargetClass(self):
         return Components
 
     def _makeOne(self, name='test', *args, **kw):
         return self._getTargetClass()(name, *args, **kw)
@@ -72,15 +72,16 @@
         self.assertEqual(comp.__bases__, (base1, base2))
         self.assertEqual(comp.adapters.__bases__,
                          (base1.adapters, base2.adapters))
         self.assertEqual(comp.utilities.__bases__,
                          (base1.utilities, base2.utilities))
 
     def test_registerUtility_with_component_name(self):
-        from zope.interface.declarations import named, InterfaceClass
+        from zope.interface.declarations import InterfaceClass
+        from zope.interface.declarations import named
 
 
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
 
         @named('foo')
@@ -173,16 +174,16 @@
         _name = 'name'
         _to_reg = Foo()
         comp = self._makeOne()
         self.assertRaises(TypeError,
                           comp.registerUtility, _to_reg, None, _name, _info)
 
     def test_registerUtility_wo_provided(self):
-        from zope.interface.declarations import directlyProvides
         from zope.interface.declarations import InterfaceClass
+        from zope.interface.declarations import directlyProvides
         from zope.interface.interfaces import Registered
         from zope.interface.registry import UtilityRegistration
 
         class IFoo(InterfaceClass):
             pass
         class Foo:
             pass
@@ -267,16 +268,16 @@
         self.assertEqual(comp._utility_registrations[(ifoo, _name2)],
                          (_to_reg, _info, None))
         self.assertEqual(comp.utilities._subscribers[0][ifoo][''],
                          (_other_reg, _to_reg,))
 
     def test_registerUtility_replaces_existing_reg(self):
         from zope.interface.declarations import InterfaceClass
-        from zope.interface.interfaces import Unregistered
         from zope.interface.interfaces import Registered
+        from zope.interface.interfaces import Unregistered
         from zope.interface.registry import UtilityRegistration
 
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         _info = 'info'
         _name = 'name'
@@ -482,16 +483,16 @@
         self.assertTrue(event.object.registry is comp)
         self.assertTrue(event.object.provided is ifoo)
         self.assertTrue(event.object.name is _name)
         self.assertTrue(event.object.component is _to_reg)
         self.assertTrue(event.object.factory is _factory)
 
     def test_unregisterUtility_wo_explicit_provided(self):
-        from zope.interface.declarations import directlyProvides
         from zope.interface.declarations import InterfaceClass
+        from zope.interface.declarations import directlyProvides
         from zope.interface.interfaces import Unregistered
         from zope.interface.registry import UtilityRegistration
 
         class IFoo(InterfaceClass):
             pass
         class Foo:
             pass
@@ -516,16 +517,16 @@
         self.assertTrue(event.object.provided is ifoo)
         self.assertTrue(event.object.name is _name)
         self.assertTrue(event.object.component is _to_reg)
         self.assertTrue(event.object.info is _info)
         self.assertTrue(event.object.factory is None)
 
     def test_unregisterUtility_wo_component_or_factory(self):
-        from zope.interface.declarations import directlyProvides
         from zope.interface.declarations import InterfaceClass
+        from zope.interface.declarations import directlyProvides
         from zope.interface.interfaces import Unregistered
         from zope.interface.registry import UtilityRegistration
 
         class IFoo(InterfaceClass):
             pass
         class Foo:
             pass
@@ -683,15 +684,14 @@
 
     def test_registeredUtilities_empty(self):
         comp = self._makeOne()
         self.assertEqual(list(comp.registeredUtilities()), [])
 
     def test_registeredUtilities_notempty(self):
         from zope.interface.declarations import InterfaceClass
-
         from zope.interface.registry import UtilityRegistration
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         _info = 'info'
         _name1 = 'name1'
         _name2 = 'name2'
@@ -805,15 +805,16 @@
         comp = self._makeOne()
         comp.registerUtility(_to_reg, ifoo, name=_name1)
         comp.registerUtility(_to_reg, ifoo, name=_name2)
         self.assertEqual(list(comp.getAllUtilitiesRegisteredFor(ifoo)),
                          [_to_reg])
 
     def test_registerAdapter_with_component_name(self):
-        from zope.interface.declarations import named, InterfaceClass
+        from zope.interface.declarations import InterfaceClass
+        from zope.interface.declarations import named
 
 
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         ibar = IFoo('IBar')
 
@@ -984,16 +985,16 @@
         self.assertEqual(event.object.required, (Interface,))
         self.assertTrue(event.object.name is _name)
         self.assertTrue(event.object.info is _info)
         self.assertTrue(event.object.factory is _Factory)
 
     def test_registerAdapter_w_required_containing_class(self):
         from zope.interface.declarations import InterfaceClass
-        from zope.interface.declarations import implementer
         from zope.interface.declarations import implementedBy
+        from zope.interface.declarations import implementer
         from zope.interface.interfaces import Registered
         from zope.interface.registry import AdapterRegistration
 
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         ibar = IFoo('IBar')
@@ -1223,15 +1224,14 @@
 
     def test_registeredAdapters_empty(self):
         comp = self._makeOne()
         self.assertEqual(list(comp.registeredAdapters()), [])
 
     def test_registeredAdapters_notempty(self):
         from zope.interface.declarations import InterfaceClass
-
         from zope.interface.registry import AdapterRegistration
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         ibar = IFoo('IFoo')
         _info = 'info'
         _name1 = 'name1'
@@ -1830,15 +1830,14 @@
 
     def test_registeredSubscriptionAdapters_empty(self):
         comp = self._makeOne()
         self.assertEqual(list(comp.registeredSubscriptionAdapters()), [])
 
     def test_registeredSubscriptionAdapters_notempty(self):
         from zope.interface.declarations import InterfaceClass
-
         from zope.interface.registry import SubscriptionRegistration
         class IFoo(InterfaceClass):
             pass
         ifoo = IFoo('IFoo')
         ibar = IFoo('IFoo')
         _info = 'info'
         _blank = ''
@@ -2473,21 +2472,21 @@
         klass = self._getTargetClass()
         return (klass(registry, ifoo, name, component, doc, factory),
                 registry,
                 name,
                )
 
     def test_class_conforms_to_IUtilityRegistration(self):
-        from zope.interface.verify import verifyClass
         from zope.interface.interfaces import IUtilityRegistration
+        from zope.interface.verify import verifyClass
         verifyClass(IUtilityRegistration, self._getTargetClass())
 
     def test_instance_conforms_to_IUtilityRegistration(self):
-        from zope.interface.verify import verifyObject
         from zope.interface.interfaces import IUtilityRegistration
+        from zope.interface.verify import verifyObject
         ur, _, _ =  self._makeOne()
         verifyObject(IUtilityRegistration, ur)
 
     def test___repr__(self):
         class _Component:
             __name__ = 'TEST'
         _component = _Component()
@@ -2659,21 +2658,21 @@
         klass = self._getTargetClass()
         return (klass(registry, (ibar,), ifoo, name, component, doc),
                 registry,
                 name,
                )
 
     def test_class_conforms_to_IAdapterRegistration(self):
-        from zope.interface.verify import verifyClass
         from zope.interface.interfaces import IAdapterRegistration
+        from zope.interface.verify import verifyClass
         verifyClass(IAdapterRegistration, self._getTargetClass())
 
     def test_instance_conforms_to_IAdapterRegistration(self):
-        from zope.interface.verify import verifyObject
         from zope.interface.interfaces import IAdapterRegistration
+        from zope.interface.verify import verifyObject
         ar, _, _ =  self._makeOne()
         verifyObject(IAdapterRegistration, ar)
 
     def test___repr__(self):
         class _Component:
             __name__ = 'TEST'
         _component = _Component()
@@ -2868,21 +2867,21 @@
         klass = self._getTargetClass()
         return (klass(registry, (ibar,), ifoo, name, component, doc),
                 registry,
                 name,
                )
 
     def test_class_conforms_to_ISubscriptionAdapterRegistration(self):
-        from zope.interface.verify import verifyClass
         from zope.interface.interfaces import ISubscriptionAdapterRegistration
+        from zope.interface.verify import verifyClass
         verifyClass(ISubscriptionAdapterRegistration, self._getTargetClass())
 
     def test_instance_conforms_to_ISubscriptionAdapterRegistration(self):
-        from zope.interface.verify import verifyObject
         from zope.interface.interfaces import ISubscriptionAdapterRegistration
+        from zope.interface.verify import verifyObject
         sar, _, _ =  self._makeOne()
         verifyObject(ISubscriptionAdapterRegistration, sar)
 
 
 class HandlerRegistrationTests(unittest.TestCase):
 
     def _getTargetClass(self):
@@ -2904,21 +2903,21 @@
         klass = self._getTargetClass()
         return (klass(registry, (ifoo,), name, component, doc),
                 registry,
                 name,
                )
 
     def test_class_conforms_to_IHandlerRegistration(self):
-        from zope.interface.verify import verifyClass
         from zope.interface.interfaces import IHandlerRegistration
+        from zope.interface.verify import verifyClass
         verifyClass(IHandlerRegistration, self._getTargetClass())
 
     def test_instance_conforms_to_IHandlerRegistration(self):
-        from zope.interface.verify import verifyObject
         from zope.interface.interfaces import IHandlerRegistration
+        from zope.interface.verify import verifyObject
         hr, _, _ =  self._makeOne()
         verifyObject(IHandlerRegistration, hr)
 
     def test_properties(self):
         def _factory(context):
             raise NotImplementedError()
         hr, _, _ =  self._makeOne(_factory)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_ro.py` & `zope.interface-6.2/src/zope/interface/tests/test_ro.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Resolution ordering utility tests"""
 import unittest
 
+
 # pylint:disable=blacklisted-name,protected-access,attribute-defined-outside-init
 
 class Test__mergeOrderings(unittest.TestCase):
 
     def _callFUT(self, orderings):
         from zope.interface.ro import _legacy_mergeOrderings
         return _legacy_mergeOrderings(orderings)
@@ -140,18 +141,18 @@
 
         self.assertEqual(self._callFUT(IOErr), bases)
 
     def test_mixed_inheritance_and_implementation(self):
         # https://github.com/zopefoundation/zope.interface/issues/8
         # This test should fail, but doesn't, as described in that issue.
         # pylint:disable=inherit-non-class
-        from zope.interface import implementer
         from zope.interface import Interface
-        from zope.interface import providedBy
         from zope.interface import implementedBy
+        from zope.interface import implementer
+        from zope.interface import providedBy
 
         class IFoo(Interface):
             pass
 
         @implementer(IFoo)
         class ImplementsFoo:
             pass
@@ -272,14 +273,15 @@
                                     + zope.interface.tests.test_ro.E
     zope.interface.tests.test_ro.F    zope.interface.tests.test_ro.F
     zope.interface.Interface          zope.interface.Interface""")
 
     def test_ExtendedPathIndex_implement_thing_implementedby_super(self):
         # See https://github.com/zopefoundation/zope.interface/pull/182#issuecomment-598754056
         from zope.interface import ro
+
         # pylint:disable=inherit-non-class
         class _Based:
             __bases__ = ()
 
             def __init__(self, name, bases=(), attrs=None):
                 self.__name__ = name
                 self.__bases__ = bases
@@ -333,30 +335,31 @@
         record, = self.log_handler.records
         self.assertIn('used the legacy', record.getMessage())
 
         with self.assertRaises(ro.InconsistentResolutionOrderError):
             self._callFUT(ExtendedPathIndex, strict=True)
 
     def test_OSError_IOError(self):
-        from zope.interface.common import interfaces
         from zope.interface import providedBy
+        from zope.interface.common import interfaces
 
         self.assertEqual(
             list(providedBy(OSError()).flattened()),
             [
                 interfaces.IOSError,
                 interfaces.IIOError,
                 interfaces.IEnvironmentError,
                 interfaces.IStandardError,
                 interfaces.IException,
                 interfaces.Interface,
             ])
 
     def test_non_orderable(self):
         import warnings
+
         from zope.interface import ro
         try:
             # If we've already warned, we must reset that state.
             del ro.__warningregistry__
         except AttributeError:
             pass
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_sorting.py` & `zope.interface-6.2/src/zope/interface/tests/test_sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Test interface sorting
 """
 
 import unittest
 
 from zope.interface import Interface
 
+
 class I1(Interface): pass
 class I2(I1): pass
 class I3(I1): pass
 class I4(Interface): pass
 class I5(I4): pass
 class I6(I2): pass
```

### Comparing `zope.interface-6.1a2/src/zope/interface/tests/test_verify.py` & `zope.interface-6.2/src/zope/interface/tests/test_verify.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ zope.interface.verify unit tests
 """
 import unittest
 
+
 # pylint:disable=inherit-non-class,no-method-argument,no-self-argument
 
 class Test_verifyClass(unittest.TestCase):
 
     verifier = None
 
     def setUp(self):
@@ -482,17 +483,17 @@
         @implementer(ICurrent)
         class Current:
             pass
 
         self._callFUT(ICurrent, Current)
 
     def test_w_callable_non_func_method(self):
-        from zope.interface.interface import Method
         from zope.interface import Interface
         from zope.interface import implementer
+        from zope.interface.interface import Method
 
         class QuasiMethod(Method):
             def __call__(self, *args, **kw):
                 raise NotImplementedError()
 
         class QuasiCallable:
             def __call__(self, *args, **kw):
@@ -548,19 +549,19 @@
     def test_tuple_IReadSequence(self):
         # As for test_dict_IFullMapping
         from zope.interface.common.sequence import IReadSequence
         self._callFUT(IReadSequence, tuple, tentative=True)
 
 
     def test_multiple_invalid(self):
-        from zope.interface.exceptions import MultipleInvalid
-        from zope.interface.exceptions import DoesNotImplement
-        from zope.interface.exceptions import BrokenImplementation
         from zope.interface import Interface
         from zope.interface import classImplements
+        from zope.interface.exceptions import BrokenImplementation
+        from zope.interface.exceptions import DoesNotImplement
+        from zope.interface.exceptions import MultipleInvalid
 
         class ISeveralMethods(Interface):
             def meth1(arg1):
                 "Method 1"
             def meth2(arg1):
                 "Method 2"
 
@@ -610,23 +611,23 @@
         class Current:
             pass
 
         self.assertRaises(BrokenImplementation,
                           self._callFUT, ICurrent, Current)
 
     def test_module_hit(self):
-        from zope.interface.tests.idummy import IDummyModule
         from zope.interface.tests import dummy
+        from zope.interface.tests.idummy import IDummyModule
 
         self._callFUT(IDummyModule, dummy)
 
     def test_module_miss(self):
         from zope.interface import Interface
-        from zope.interface.tests import dummy
         from zope.interface.exceptions import DoesNotImplement
+        from zope.interface.tests import dummy
 
         # same name, different object
         class IDummyModule(Interface):
             pass
 
         self.assertRaises(DoesNotImplement,
                           self._callFUT, IDummyModule, dummy)
```

### Comparing `zope.interface-6.1a2/src/zope/interface/verify.py` & `zope.interface-6.2/src/zope/interface/verify.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,18 @@
 from types import MethodType
 
 from zope.interface.exceptions import BrokenImplementation
 from zope.interface.exceptions import BrokenMethodImplementation
 from zope.interface.exceptions import DoesNotImplement
 from zope.interface.exceptions import Invalid
 from zope.interface.exceptions import MultipleInvalid
+from zope.interface.interface import Method
+from zope.interface.interface import fromFunction
+from zope.interface.interface import fromMethod
 
-from zope.interface.interface import fromMethod, fromFunction, Method
 
 __all__ = [
     'verifyObject',
     'verifyClass',
 ]
 
 # This will be monkey-patched when running under Zope 2, so leave this
```

### Comparing `zope.interface-6.1a2/src/zope.interface.egg-info/PKG-INFO` & `zope.interface-6.2/src/zope.interface.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.1a2
+Version: 6.2
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,23 +14,34 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+Requires-Dist: setuptools
 Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
+Requires-Dist: coverage>=5.0.3; extra == "test"
+Requires-Dist: zope.event; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
 Provides-Extra: testing
-License-File: LICENSE.txt
+Requires-Dist: coverage>=5.0.3; extra == "testing"
+Requires-Dist: zope.event; extra == "testing"
+Requires-Dist: zope.testing; extra == "testing"
 
 ====================
  ``zope.interface``
 ====================
 
 .. image:: https://img.shields.io/pypi/v/zope.interface.svg
     :target: https://pypi.python.org/pypi/zope.interface/
@@ -60,24 +71,31 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
-6.1a2 (2023-04-13)
-==================
+6.2 (2024-02-16)
+================
 
-- Fix building of the docs for non-final versions.
+- Add preliminary support for Python 3.13 as of 3.13a3.
 
+- Add support to use the pipe (``|``) syntax for ``typing.Union``.
+  (`#280 <https://github.com/zopefoundation/zope.interface/issues/280>`_)
 
-6.1a1 (2023-04-06)
-==================
 
-- Add support for building ppc64le wheels.
+6.1 (2023-10-05)
+================
+
+- Build Linux binary wheels for Python 3.12.
+
+- Add support for Python 3.12.
+
+- Fix building of the docs for non-final versions.
 
 
 6.0 (2023-03-17)
 ================
 
 - Build Linux binary wheels for Python 3.11.
```

### Comparing `zope.interface-6.1a2/src/zope.interface.egg-info/SOURCES.txt` & `zope.interface-6.2/src/zope.interface.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .coveragerc
 .manylinux-install.sh
 .manylinux.sh
+.readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 appveyor.yml
 build.cmd
 buildout.cfg
-rtd.txt
 setup.cfg
 setup.py
 tox.ini
 benchmarks/micro.py
 docs/Makefile
 docs/README.rst
 docs/README.ru.rst
@@ -24,14 +24,15 @@
 docs/conf.py
 docs/foodforthought.rst
 docs/hacking.rst
 docs/human.rst
 docs/human.ru.rst
 docs/index.rst
 docs/make.bat
+docs/requirements.txt
 docs/verify.rst
 docs/api/adapters.rst
 docs/api/common.rst
 docs/api/components.rst
 docs/api/declarations.rst
 docs/api/index.rst
 docs/api/ro.rst
```

### Comparing `zope.interface-6.1a2/tox.ini` & `zope.interface-6.2/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -6,60 +6,87 @@
     lint
     py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
     py312,py312-pure
+    py313,py313-pure
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
-pip_pre = py312: true
+pip_pre = py313: true
 deps =
+    py37: urllib3 < 2
     Sphinx
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     ZOPE_INTERFACE_STRICT_IRO=1
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     coverage run -p -m unittest discover -s src {posargs}
     sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
+    py37: urllib3 < 2
 setenv =
     PURE_PYTHON=1
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage combine
     coverage html -i
     coverage report -i -m --fail-under=99
 depends = py37,py37-pure,py38,py38-pure,py39,py39-pure,py310,py310-pure,py311,py311-pure,pypy,pypy3,docs
 parallel_show_output = true
-
-[testenv:lint]
+[testenv:release-check]
+description = ensure that the distribution is ready to release
 basepython = python3
 skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
 commands =
     check-manifest
     check-python-versions
+    python -m build --sdist --no-isolation
+    twine check dist/*
+
+[testenv:lint]
+basepython = python3
+skip_install = true
 deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
+    isort
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
+commands =
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
```

