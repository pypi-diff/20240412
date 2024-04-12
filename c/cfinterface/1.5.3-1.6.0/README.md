# Comparing `tmp/cfinterface-1.5.3.tar.gz` & `tmp/cfinterface-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.5.3.tar", last modified: Mon Aug  7 14:17:21 2023, max compression
+gzip compressed data, was "cfinterface-1.6.tar", last modified: Fri Apr 12 20:29:53 2024, max compression
```

## Comparing `cfinterface-1.5.3.tar` & `cfinterface-1.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 14:16:06.000000 cfinterface-1.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-07 14:17:21.401047 cfinterface-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-07 14:16:06.000000 cfinterface-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:17:21.401047 cfinterface-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-07 14:16:06.000000 cfinterface-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 20:28:51.000000 cfinterface-1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-12 20:29:53.058245 cfinterface-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-12 20:28:51.000000 cfinterface-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.042245 cfinterface-1.6/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.046245 cfinterface-1.6/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-12 20:28:51.000000 cfinterface-1.6/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-12 20:29:53.000000 cfinterface-1.6/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 20:29:52.000000 cfinterface-1.6/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:29:53.058245 cfinterface-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 20:28:51.000000 cfinterface-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.050245 cfinterface-1.6/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.054245 cfinterface-1.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:29:53.058245 cfinterface-1.6/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-12 20:28:51.000000 cfinterface-1.6/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.5.3/LICENSE.md` & `cfinterface-1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/PKG-INFO` & `cfinterface-1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.3
+Version: 1.6.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 # cfinterface
 
 ![tests](https://github.com/rjmalves/cfi/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/rjmalves/cfi/branch/main/graph/badge.svg?token=86ZXJGB854)](https://codecov.io/gh/rjmalves/cfi)
 
 Python package that contains a framework for dealing with custom file formats, modulating reading, data formatting and writing in a scalable and modular way.
```

### Comparing `cfinterface-1.5.3/README.md` & `cfinterface-1.6/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.6/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/cfinterface/adapters/components/repository.py` & `cfinterface-1.6/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/cfinterface/adapters/reading/repository.py` & `cfinterface-1.6/cfinterface/adapters/reading/repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import IO, BinaryIO, TextIO, Union, Type, Dict
 from abc import ABC, abstractmethod
 from io import BytesIO, StringIO
 
 
 class Repository(ABC):
+
+    __slots__ = ["_content", "_wrap_io"]
+
     def __init__(
         self, content: Union[str, bytes], wrap_io: bool = False, *args
     ) -> None:
         self._content = content
         self._wrap_io = wrap_io
 
     def __enter__(self) -> "Repository":
@@ -32,14 +35,17 @@
     @property
     @abstractmethod
     def file(self) -> IO:
         raise NotImplementedError
 
 
 class BinaryRepository(Repository):
+
+    __slots__ = ["_filepointer"]
+
     def __init__(
         self, content: Union[str, bytes], wrap_io: bool = False, *args
     ) -> None:
         super().__init__(content, wrap_io)
         self._filepointer: BinaryIO = None  # type: ignore
 
     def __enter__(self):
@@ -68,14 +74,17 @@
 
     @property
     def file(self) -> BinaryIO:
         return self._filepointer
 
 
 class TextualRepository(Repository):
+
+    __slots__ = ["_filepointer", "_encoding"]
+
     def __init__(
         self,
         content: str,
         wrap_io: bool = False,
         encoding: str = "utf-8",
         *args
     ) -> None:
```

### Comparing `cfinterface-1.5.3/cfinterface/adapters/writing/repository.py` & `cfinterface-1.6/cfinterface/adapters/writing/repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import IO, BinaryIO, TextIO, Union, Dict, Type
 from abc import ABC, abstractmethod
 
 
 class Repository(ABC):
+
+    __slots__ = ["_to", "_wrap_io"]
+
     def __init__(self, to: Union[str, IO], *args) -> None:
         self._to = to
         self._wrap_io = isinstance(to, str)
 
     def __enter__(self) -> "Repository":
         return self
 
@@ -26,14 +29,17 @@
     @property
     @abstractmethod
     def file(self) -> IO:
         raise NotImplementedError
 
 
 class BinaryRepository(Repository):
+
+    __slots__ = ["_filepointer"]
+
     def __init__(self, path: str, *args) -> None:
         super().__init__(path)
         self._filepointer: BinaryIO = None  # type: ignore
 
     def __enter__(self):
         self._filepointer = open(self._to, "wb") if self._wrap_io else self._to
         return super().__enter__()
@@ -55,14 +61,17 @@
 
     @property
     def file(self) -> BinaryIO:
         return self._filepointer
 
 
 class TextualRepository(Repository):
+
+    __slots__ = ["_filepointer", "_encoding"]
+
     def __init__(self, path: str, encoding: str) -> None:
         super().__init__(path)
         self._filepointer: TextIO = None  # type: ignore
         self._encoding = encoding
 
     def __enter__(self):
         self._filepointer = (
```

### Comparing `cfinterface-1.5.3/cfinterface/components/block.py` & `cfinterface-1.6/cfinterface/components/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class Block:
     """
     Class for a generic block in a textfile, with given markers
     for beginning and end and reading states.
     """
 
+    __slots__ = ["__previous", "__next", "__data"]
+
     BEGIN_PATTERN: Union[str, bytes] = ""
     END_PATTERN: Union[str, bytes] = ""
     MAX_LINES = 10000
 
     def __init__(
         self,
         previous=None,
```

### Comparing `cfinterface-1.5.3/cfinterface/components/datetimefield.py` & `cfinterface-1.6/cfinterface/components/datetimefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 class DatetimeField(Field):
     """
     Class for representing an datetime field for being read from and
     written to a file. The format to read and write the value is given
     by an optional argument.
     """
 
+    __slots__ = ["__format"]
+
     def __init__(
         self,
         size: int = 16,
         starting_position: int = 0,
         format: str = "%Y/%m/%d",
         value: Optional[datetime] = None,
     ) -> None:
```

### Comparing `cfinterface-1.5.3/cfinterface/components/defaultblock.py` & `cfinterface-1.6/cfinterface/components/defaultblock.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class DefaultBlock(Block):
     """
     A class for representing a default block, which contains exactly
     the data from the read line. Mainly used for comments.
     """
 
+    __slots__ = []
+
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, DefaultBlock):
             return False
         return self.data == o.data
 
     def read(self, file: IO, *args, **kwargs) -> bool:
         self.data = file.readline()
```

### Comparing `cfinterface-1.5.3/cfinterface/components/defaultregister.py` & `cfinterface-1.6/cfinterface/components/defaultregister.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class DefaultRegister(Register):
     """
     A class for representing a default register, which contains exactly
     the data from the read line. Mainly used for comments.
     """
 
+    __slots__ = []
+
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, DefaultRegister):
             return False
         return self.data == o.data
```

### Comparing `cfinterface-1.5.3/cfinterface/components/defaultsection.py` & `cfinterface-1.6/cfinterface/components/defaultsection.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class DefaultSection(Section):
     """
     A class for representing a default section, which contains no data
     and is used for representing empty data.
     """
 
+    __slots__ = []
+
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, DefaultSection):
             return False
         return self.data == o.data
 
     def read(self, file: IO, *args, **kwargs) -> bool:
         self.data = file.readline()
```

### Comparing `cfinterface-1.5.3/cfinterface/components/field.py` & `cfinterface-1.6/cfinterface/components/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 class Field:
     """
     Class for representing an field for being read from and written
     in a file.
     """
 
+    __slots__ = ["_size", "_starting_position", "_ending_position", "_value"]
+
     T = TypeVar("T", str, bytes)
 
     def __init__(
         self,
         size: int,
         starting_position: int,
         value: Optional[Any] = None,
```

### Comparing `cfinterface-1.5.3/cfinterface/components/floatfield.py` & `cfinterface-1.6/cfinterface/components/floatfield.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 class FloatField(Field):
     """
     Class for representing an float field for being read from and
     written to a file. The format to read and write the value is given
     by 'F' for fixed point notation and 'E' for scientific notation.
     """
 
+    __slots__ = ["__decimal_digits", "__format", "__sep", "__type"]
+
     TYPES = {
         2: np.float16,
         4: np.float32,
         8: np.float64,
     }
 
     def __init__(
```

### Comparing `cfinterface-1.5.3/cfinterface/components/integerfield.py` & `cfinterface-1.6/cfinterface/components/integerfield.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 class IntegerField(Field):
     """
     Class for representing an integer field for being read from and
     written to a file.
     """
 
+    __slots__ = ["__type"]
+
     TYPES = {
         2: np.int16,
         4: np.int32,
         8: np.int64,
     }
 
     def __init__(
```

### Comparing `cfinterface-1.5.3/cfinterface/components/line.py` & `cfinterface-1.6/cfinterface/components/line.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 class Line:
     """
     Class for representing a generic line that is composed
     of fields and can be read from or written to a file.
     """
 
+    __slots__ = [
+        "_delimiter",
+        "_fields",
+        "_values",
+        "_storage",
+        "_repository",
+        "_size",
+    ]
+
     def __init__(
         self,
         fields: List[Field],
         values: Optional[List[Any]] = None,
         delimiter: Optional[Union[str, bytes]] = None,
         storage: str = "",
     ):
```

### Comparing `cfinterface-1.5.3/cfinterface/components/literalfield.py` & `cfinterface-1.6/cfinterface/components/literalfield.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class LiteralField(Field):
     """
     Class for representing an literal field for being read from and
     written to a file.
     """
 
+    __slots__ = []
+
     def __init__(
         self,
         size: int = 80,
         starting_position: int = 0,
         value: Optional[str] = None,
     ) -> None:
         super().__init__(size, starting_position, value)
```

### Comparing `cfinterface-1.5.3/cfinterface/components/register.py` & `cfinterface-1.6/cfinterface/components/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 class Register:
     """
     Class for a generic register in a textfile, with a given identifier
     which is located at the beginning of the line.
     """
 
+    __slots__ = ["__previous", "__next", "__data", "__identifier_field"]
+
     IDENTIFIER: Union[str, bytes] = ""
     IDENTIFIER_DIGITS = 0
     LINE = Line([])
     _REGISTER_PROPERTIES = [
         "data",
         "empty",
         "is_first",
```

### Comparing `cfinterface-1.5.3/cfinterface/components/section.py` & `cfinterface-1.6/cfinterface/components/section.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class Section:
     """
     Class for a generic section in a textfile, which begins and ends in
     a given order
     """
 
+    __slots__ = ["__previous", "__next", "__data"]
+
     STORAGE: str = "TEXT"
 
     def __init__(
         self,
         previous=None,
         next=None,
         data=None,
```

### Comparing `cfinterface-1.5.3/cfinterface/data/blockdata.py` & `cfinterface-1.6/cfinterface/data/blockdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 class BlockData:
     """
     Class for a storing, managing and accessing data for a block file.
     """
 
+    __slots__ = ["__root", "__head"]
+
     T = TypeVar("T")
 
     def __init__(self, root: Block) -> None:
         self.__root = root
         self.__head = root
 
     def __iter__(self):
```

### Comparing `cfinterface-1.5.3/cfinterface/data/registerdata.py` & `cfinterface-1.6/cfinterface/data/registerdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 class RegisterData:
     """
     Class for a storing, managing and accessing data for a register file.
     """
 
+    __slots__ = ["__root", "__head"]
+
     T = TypeVar("T")
 
     def __init__(self, root: Register) -> None:
         self.__root = root
         self.__head = root
 
     def __iter__(self):
```

### Comparing `cfinterface-1.5.3/cfinterface/data/sectiondata.py` & `cfinterface-1.6/cfinterface/data/sectiondata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 class SectionData:
     """
     Class for a storing, managing and accessing data for a section file.
     """
 
+    __slots__ = ["__root", "__head"]
+
     T = TypeVar("T")
 
     def __init__(self, root: Section) -> None:
         self.__root = root
         self.__head = root
 
     def __iter__(self):
```

### Comparing `cfinterface-1.5.3/cfinterface/files/blockfile.py` & `cfinterface-1.6/cfinterface/files/blockfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class BlockFile:
     """
     Class that models a file divided by blocks, where the reading
     and writing are given by a series of blocks.
     """
 
+    __slots__ = ["__data", "__storage", "__encoding"]
+
     VERSIONS: Dict[str, List[Type[Block]]] = {}
     BLOCKS: List[Type[Block]] = []
     ENCODING = "utf-8"
     STORAGE = "TEXT"
     __VERSION = "latest"
 
     def __init__(
```

### Comparing `cfinterface-1.5.3/cfinterface/files/registerfile.py` & `cfinterface-1.6/cfinterface/files/registerfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class RegisterFile:
     """
     Class that models a file divided by registers, where the reading
     and writing are given by a series of registers.
     """
 
+    __slots__ = ["__data", "__storage", "__encoding"]
+
     VERSIONS: Dict[str, List[Type[Register]]] = {}
     REGISTERS: List[Type[Register]] = []
     ENCODING = "utf-8"
     STORAGE = "TEXT"
     __VERSION = "latest"
 
     def __init__(
```

### Comparing `cfinterface-1.5.3/cfinterface/files/sectionfile.py` & `cfinterface-1.6/cfinterface/files/sectionfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class SectionFile:
     """
     Class that models a file divided by registers, where the reading
     and writing are given by a series of registers.
     """
 
+    __slots__ = ["__data", "__storage", "__encoding"]
+
     VERSIONS: Dict[str, List[Type[Section]]] = {}
     SECTIONS: List[Type[Section]] = []
     ENCODING = "utf-8"
     STORAGE = "TEXT"
     __VERSION = "latest"
 
     def __init__(
```

### Comparing `cfinterface-1.5.3/cfinterface/reading/blockreading.py` & `cfinterface-1.6/cfinterface/reading/blockreading.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 
 class BlockReading:
     """
     Class for reading custom files based on a BlockData structure.
     """
 
+    __slots__ = [
+        "__allowed_blocks",
+        "__data",
+        "__last_position_filepointer",
+        "__storage",
+        "__linesize",
+        "__repository",
+    ]
+
     def __init__(
         self,
         allowed_blocks: List[Type[Block]],
         storage: str = "",
         linesize: int = 1,
     ) -> None:
         self.__allowed_blocks = allowed_blocks
```

### Comparing `cfinterface-1.5.3/cfinterface/reading/registerreading.py` & `cfinterface-1.6/cfinterface/reading/registerreading.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 
 class RegisterReading:
     """
     Class for reading custom files based on a RegisterData structure.
     """
 
+    __slots__ = [
+        "__allowed_registers",
+        "__data",
+        "__last_position_filepointer",
+        "__storage",
+        "__linesize",
+        "__repository",
+    ]
+
     def __init__(
         self,
         allowed_registers: List[Type[Register]],
         storage: str = "",
         linesize: int = 1,
     ) -> None:
         self.__allowed_registers = allowed_registers
```

### Comparing `cfinterface-1.5.3/cfinterface/reading/sectionreading.py` & `cfinterface-1.6/cfinterface/reading/sectionreading.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
 
 class SectionReading:
     """
     Class for reading custom files based on a SectionData structure.
     """
 
+    __slots__ = [
+        "__sections",
+        "__data",
+        "__last_position_filepointer",
+        "__storage",
+        "__linesize",
+        "__repository",
+    ]
+
     def __init__(
         self,
         sections: List[Type[Section]],
         storage: str = "",
         linesize: int = 1,
     ) -> None:
         self.__sections = sections
```

### Comparing `cfinterface-1.5.3/cfinterface/writing/blockwriting.py` & `cfinterface-1.6/cfinterface/writing/blockwriting.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 
 
 class BlockWriting:
     """
     Class for writing custom files based on a BlockData structure.
     """
 
+    __slots__ = [
+        "__data",
+        "__storage",
+        "__repository",
+    ]
+
     def __init__(self, data: BlockData, storage: str = "") -> None:
         self.__data = data
         self.__storage = storage
         self.__repository: Repository = None  # type: ignore
 
     def __write_file(self, *args, **kwargs):
         """
```

### Comparing `cfinterface-1.5.3/cfinterface/writing/registerwriting.py` & `cfinterface-1.6/cfinterface/writing/registerwriting.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
 
 class RegisterWriting:
     """
     Class for writing custom files based on a RegisterData structure.
     """
 
+    __slots__ = [
+        "__data",
+        "__storage",
+        "__repository",
+    ]
+
     def __init__(self, data: RegisterData, storage: str = "") -> None:
         self.__data = data
         self.__storage = storage
         self.__repository: Repository = None  # type: ignore
 
     def __write_file(self, *args, **kwargs):
         """
```

### Comparing `cfinterface-1.5.3/cfinterface/writing/sectionwriting.py` & `cfinterface-1.6/cfinterface/writing/sectionwriting.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
 
 class SectionWriting:
     """
     Class for writing custom files based on a SectionData structure.
     """
 
+    __slots__ = [
+        "__data",
+        "__storage",
+        "__repository",
+    ]
+
     def __init__(self, data: SectionData, storage: str = "") -> None:
         self.__data = data
         self.__storage = storage
         self.__repository: Repository = None  # type: ignore
 
     def __write_file(self, *args, **kwargs):
         """
```

### Comparing `cfinterface-1.5.3/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.6/cfinterface.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.3
+Version: 1.6.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 # cfinterface
 
 ![tests](https://github.com/rjmalves/cfi/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/rjmalves/cfi/branch/main/graph/badge.svg?token=86ZXJGB854)](https://codecov.io/gh/rjmalves/cfi)
 
 Python package that contains a framework for dealing with custom file formats, modulating reading, data formatting and writing in a scalable and modular way.
```

### Comparing `cfinterface-1.5.3/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.6/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/setup.py` & `cfinterface-1.6/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/adapters/components/test_linerepository.py` & `cfinterface-1.6/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_block.py` & `cfinterface-1.6/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_datetimefield.py` & `cfinterface-1.6/tests/components/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_defaultblock.py` & `cfinterface-1.6/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_defaultregister.py` & `cfinterface-1.6/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_defaultsection.py` & `cfinterface-1.6/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_floatfield.py` & `cfinterface-1.6/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_integerfield.py` & `cfinterface-1.6/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_line.py` & `cfinterface-1.6/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_literalfield.py` & `cfinterface-1.6/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_register.py` & `cfinterface-1.6/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/components/test_section.py` & `cfinterface-1.6/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/data/test_blockdata.py` & `cfinterface-1.6/tests/data/test_blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/data/test_registerdata.py` & `cfinterface-1.6/tests/data/test_registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/data/test_sectiondata.py` & `cfinterface-1.6/tests/data/test_sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/files/test_blockfile.py` & `cfinterface-1.6/tests/files/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/files/test_registerfile.py` & `cfinterface-1.6/tests/files/test_registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/files/test_sectionfile.py` & `cfinterface-1.6/tests/files/test_sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/mocks/mock_open.py` & `cfinterface-1.6/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/reading/test_blockreading.py` & `cfinterface-1.6/tests/reading/test_blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/reading/test_registerreading.py` & `cfinterface-1.6/tests/reading/test_registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/reading/test_sectionreading.py` & `cfinterface-1.6/tests/reading/test_sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/writing/test_blockwriting.py` & `cfinterface-1.6/tests/writing/test_blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/writing/test_registerwriting.py` & `cfinterface-1.6/tests/writing/test_registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.3/tests/writing/test_sectionwriting.py` & `cfinterface-1.6/tests/writing/test_sectionwriting.py`

 * *Files identical despite different names*

