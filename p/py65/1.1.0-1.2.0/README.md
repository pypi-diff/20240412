# Comparing `tmp/py65-1.1.0.tar.gz` & `tmp/py65-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py65-1.1.0.tar", last modified: Sun Jul  1 21:16:32 2018, max compression
+gzip compressed data, was "py65-1.2.tar", last modified: Fri Apr 12 20:01:50 2024, max compression
```

## Comparing `py65-1.1.0.tar` & `py65-1.2.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/
--rw-r--r--   0 mnaberez   (501) staff       (20)     1468 2018-07-01 21:16:32.000000 py65-1.1.0/PKG-INFO
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/
--rw-r--r--   0 mnaberez   (501) staff       (20)    29923 2018-06-26 22:52:00.000000 py65-1.1.0/py65/monitor.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     2382 2017-02-17 16:47:18.000000 py65-1.1.0/py65/memory.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     4742 2018-06-26 00:02:53.000000 py65-1.1.0/py65/disassembler.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/tests/
--rw-r--r--   0 mnaberez   (501) staff       (20)    40535 2018-06-26 22:52:00.000000 py65-1.1.0/py65/tests/test_monitor.py
--rw-r--r--   0 mnaberez   (501) staff       (20)       20 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/__init__.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/tests/utils/
--rw-r--r--   0 mnaberez   (501) staff       (20)     1087 2017-09-19 16:07:36.000000 py65-1.1.0/py65/tests/utils/test_conversions.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     6581 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/utils/test_addressing.py
--rw-r--r--   0 mnaberez   (501) staff       (20)      234 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/utils/test_console.py
--rw-r--r--   0 mnaberez   (501) staff       (20)       20 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/utils/__init__.py
--rw-r--r--   0 mnaberez   (501) staff       (20)       22 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/utils/test_devices.py
--rw-r--r--   0 mnaberez   (501) staff       (20)    45745 2018-06-25 16:59:33.000000 py65-1.1.0/py65/tests/test_disassembler.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     4576 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/test_memory.py
--rw-r--r--   0 mnaberez   (501) staff       (20)    34604 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/test_assembler.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/tests/devices/
--rw-r--r--   0 mnaberez   (501) staff       (20)       20 2017-02-17 16:47:18.000000 py65-1.1.0/py65/tests/devices/__init__.py
--rw-r--r--   0 mnaberez   (501) staff       (20)    48721 2017-12-16 03:00:40.000000 py65-1.1.0/py65/tests/devices/test_mpu65c02.py
--rw-r--r--   0 mnaberez   (501) staff       (20)   203687 2017-12-16 02:54:37.000000 py65-1.1.0/py65/tests/devices/test_mpu6502.py
--rw-r--r--   0 mnaberez   (501) staff       (20)      244 2017-02-17 16:47:18.000000 py65-1.1.0/py65/__init__.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/utils/
--rw-r--r--   0 mnaberez   (501) staff       (20)     3200 2017-02-17 16:47:18.000000 py65-1.1.0/py65/utils/console.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     2375 2017-09-19 22:29:01.000000 py65-1.1.0/py65/utils/conversions.py
--rw-r--r--   0 mnaberez   (501) staff       (20)       20 2017-02-17 16:47:18.000000 py65-1.1.0/py65/utils/__init__.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     3366 2017-02-17 16:47:18.000000 py65-1.1.0/py65/utils/addressing.py
--rw-r--r--   0 mnaberez   (501) staff       (20)      469 2017-02-17 16:47:18.000000 py65-1.1.0/py65/utils/devices.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     4691 2017-02-17 16:47:18.000000 py65-1.1.0/py65/assembler.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65/devices/
--rw-r--r--   0 mnaberez   (501) staff       (20)     1451 2017-02-17 16:47:18.000000 py65-1.1.0/py65/devices/mpu65org16.py
--rw-r--r--   0 mnaberez   (501) staff       (20)       20 2017-02-17 16:47:18.000000 py65-1.1.0/py65/devices/__init__.py
--rw-r--r--   0 mnaberez   (501) staff       (20)    34980 2018-06-26 18:36:13.000000 py65-1.1.0/py65/devices/mpu6502.py
--rw-r--r--   0 mnaberez   (501) staff       (20)     8503 2017-12-16 03:10:29.000000 py65-1.1.0/py65/devices/mpu65c02.py
--rw-r--r--   0 mnaberez   (501) staff       (20)      179 2017-02-17 16:47:18.000000 py65-1.1.0/MANIFEST.in
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/docs/
--rw-r--r--   0 mnaberez   (501) staff       (20)    13885 2017-02-17 16:47:17.000000 py65-1.1.0/docs/index.rst
--rw-r--r--   0 mnaberez   (501) staff       (20)     2339 2017-02-17 16:47:17.000000 py65-1.1.0/docs/Makefile
--rw-r--r--   0 mnaberez   (501) staff       (20)     5978 2018-07-01 21:10:03.000000 py65-1.1.0/docs/conf.py
--rw-r--r--   0 mnaberez   (501) staff       (20)    11159 2018-07-01 21:10:52.000000 py65-1.1.0/CHANGES.txt
--rw-r--r--   0 mnaberez   (501) staff       (20)     2139 2018-07-01 21:09:46.000000 py65-1.1.0/setup.py
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/
--rw-r--r--   0 mnaberez   (501) staff       (20)     1468 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/PKG-INFO
--rw-r--r--   0 mnaberez   (501) staff       (20)        1 2017-02-17 16:47:18.000000 py65-1.1.0/py65.egg-info/not-zip-safe
--rw-r--r--   0 mnaberez   (501) staff       (20)     1127 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/SOURCES.txt
--rw-r--r--   0 mnaberez   (501) staff       (20)       47 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/entry_points.txt
--rw-r--r--   0 mnaberez   (501) staff       (20)        5 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/top_level.txt
--rw-r--r--   0 mnaberez   (501) staff       (20)        1 2018-07-01 21:16:32.000000 py65-1.1.0/py65.egg-info/dependency_links.txt
-drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2018-07-01 21:16:32.000000 py65-1.1.0/examples/
--rw-r--r--   0 mnaberez   (501) staff       (20)      744 2017-02-17 16:47:18.000000 py65-1.1.0/examples/swapcase.asm
--rw-r--r--   0 mnaberez   (501) staff       (20)     8627 2017-02-17 16:47:18.000000 py65-1.1.0/examples/65Org16.boot.asm
--rw-r--r--   0 mnaberez   (501) staff       (20)       79 2017-02-17 16:47:18.000000 py65-1.1.0/examples/swapcase.hex
--rw-r--r--   0 mnaberez   (501) staff       (20)     1024 2017-02-17 16:47:18.000000 py65-1.1.0/examples/65Org16.boot.rom
--rw-r--r--   0 mnaberez   (501) staff       (20)      232 2017-02-17 16:47:18.000000 py65-1.1.0/examples/README.txt
--rwxr-xr-x   0 mnaberez   (501) staff       (20)    65536 2017-02-17 16:47:18.000000 py65-1.1.0/examples/ehbasic.bin
--rw-r--r--   0 mnaberez   (501) staff       (20)       67 2018-07-01 21:16:32.000000 py65-1.1.0/setup.cfg
--rw-r--r--   0 mnaberez   (501) staff       (20)     3257 2017-02-17 16:47:18.000000 py65-1.1.0/README.rst
--rw-r--r--   0 mnaberez   (501) staff       (20)     1538 2017-02-17 16:47:18.000000 py65-1.1.0/LICENSE.txt
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.959410 py65-1.2/
+-rw-r--r--   0 mnaberez   (501) staff       (20)    11805 2024-04-12 19:59:45.000000 py65-1.2/CHANGES.rst
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1538 2024-04-12 18:10:51.000000 py65-1.2/LICENSE.txt
+-rw-r--r--   0 mnaberez   (501) staff       (20)      179 2022-11-01 01:54:48.000000 py65-1.2/MANIFEST.in
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1647 2024-04-12 20:01:50.959358 py65-1.2/PKG-INFO
+-rw-r--r--   0 mnaberez   (501) staff       (20)     3053 2023-11-19 00:43:13.000000 py65-1.2/README.rst
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.954092 py65-1.2/docs/
+-rw-r--r--   0 mnaberez   (501) staff       (20)     2339 2022-11-01 01:54:48.000000 py65-1.2/docs/Makefile
+-rw-r--r--   0 mnaberez   (501) staff       (20)     5978 2024-04-12 19:59:57.000000 py65-1.2/docs/conf.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    13896 2022-11-01 01:54:48.000000 py65-1.2/docs/index.rst
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.954833 py65-1.2/examples/
+-rw-r--r--   0 mnaberez   (501) staff       (20)     8627 2022-11-01 01:54:48.000000 py65-1.2/examples/65Org16.boot.asm
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1024 2022-11-01 01:54:48.000000 py65-1.2/examples/65Org16.boot.rom
+-rw-r--r--   0 mnaberez   (501) staff       (20)      232 2022-11-01 01:54:48.000000 py65-1.2/examples/README.txt
+-rwxr-xr-x   0 mnaberez   (501) staff       (20)    65536 2022-11-01 01:54:48.000000 py65-1.2/examples/ehbasic.bin
+-rw-r--r--   0 mnaberez   (501) staff       (20)      744 2022-11-01 01:54:48.000000 py65-1.2/examples/swapcase.asm
+-rw-r--r--   0 mnaberez   (501) staff       (20)       79 2022-11-01 01:54:48.000000 py65-1.2/examples/swapcase.hex
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.955521 py65-1.2/py65/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2023-06-24 15:35:53.000000 py65-1.2/py65/__init__.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     4688 2024-04-12 19:24:05.000000 py65-1.2/py65/assembler.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)      393 2024-04-12 19:24:05.000000 py65-1.2/py65/compat.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.956674 py65-1.2/py65/devices/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2022-11-01 01:54:48.000000 py65-1.2/py65/devices/__init__.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    35791 2022-11-01 01:54:48.000000 py65-1.2/py65/devices/mpu6502.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     8503 2023-09-12 20:12:57.000000 py65-1.2/py65/devices/mpu65c02.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1451 2022-11-01 01:54:48.000000 py65-1.2/py65/devices/mpu65org16.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     4737 2023-09-12 20:12:57.000000 py65-1.2/py65/disassembler.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     2382 2022-11-01 01:54:48.000000 py65-1.2/py65/memory.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    31765 2024-04-12 19:23:15.000000 py65-1.2/py65/monitor.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.957394 py65-1.2/py65/tests/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/__init__.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.957862 py65-1.2/py65/tests/devices/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/devices/__init__.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)   210737 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/devices/test_mpu6502.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    48721 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/devices/test_mpu65c02.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     2486 2024-04-12 19:24:05.000000 py65-1.2/py65/tests/end_to_end.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    34614 2023-09-12 20:12:57.000000 py65-1.2/py65/tests/test_assembler.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    45962 2023-09-12 20:14:48.000000 py65-1.2/py65/tests/test_disassembler.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     4576 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/test_memory.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)    41470 2023-11-19 00:42:31.000000 py65-1.2/py65/tests/test_monitor.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.958465 py65-1.2/py65/tests/utils/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/utils/__init__.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     6581 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/utils/test_addressing.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)      234 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/utils/test_console.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1087 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/utils/test_conversions.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)       22 2022-11-01 01:54:48.000000 py65-1.2/py65/tests/utils/test_devices.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.959026 py65-1.2/py65/utils/
+-rw-r--r--   0 mnaberez   (501) staff       (20)       20 2022-11-01 01:54:48.000000 py65-1.2/py65/utils/__init__.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     3368 2024-04-12 19:23:15.000000 py65-1.2/py65/utils/addressing.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     7839 2024-04-12 19:24:05.000000 py65-1.2/py65/utils/console.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)     2375 2022-11-01 01:54:48.000000 py65-1.2/py65/utils/conversions.py
+-rw-r--r--   0 mnaberez   (501) staff       (20)      469 2022-11-01 01:54:48.000000 py65-1.2/py65/utils/devices.py
+drwxr-xr-x   0 mnaberez   (501) staff       (20)        0 2024-04-12 20:01:50.959182 py65-1.2/py65.egg-info/
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1647 2024-04-12 20:01:50.000000 py65-1.2/py65.egg-info/PKG-INFO
+-rw-r--r--   0 mnaberez   (501) staff       (20)     1167 2024-04-12 20:01:50.000000 py65-1.2/py65.egg-info/SOURCES.txt
+-rw-r--r--   0 mnaberez   (501) staff       (20)        1 2024-04-12 20:01:50.000000 py65-1.2/py65.egg-info/dependency_links.txt
+-rw-r--r--   0 mnaberez   (501) staff       (20)       46 2024-04-12 20:01:50.000000 py65-1.2/py65.egg-info/entry_points.txt
+-rw-r--r--   0 mnaberez   (501) staff       (20)        1 2022-11-01 01:54:48.000000 py65-1.2/py65.egg-info/not-zip-safe
+-rw-r--r--   0 mnaberez   (501) staff       (20)        5 2024-04-12 20:01:50.000000 py65-1.2/py65.egg-info/top_level.txt
+-rw-r--r--   0 mnaberez   (501) staff       (20)       67 2024-04-12 20:01:50.959597 py65-1.2/setup.cfg
+-rw-r--r--   0 mnaberez   (501) staff       (20)     2277 2024-04-12 20:00:10.000000 py65-1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py65-1.1.0/PKG-INFO` & `py65-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: py65
-Version: 1.1.0
+Version: 1.2.0
 Summary: 6502 microprocessor simulation package
 Home-page: https://github.com/mnaberez/py65
 Author: Mike Naberezny
 Author-email: mike@naberezny.com
+Maintainer: Mike Naberezny
+Maintainer-email: mike@naberezny.com
 License: License :: OSI Approved :: BSD License
-Description-Content-Type: UNKNOWN
-Description: Simulate 6502-based microcomputer systems in Python.
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Assembly
 Classifier: Topic :: Software Development :: Assemblers
 Classifier: Topic :: Software Development :: Disassemblers
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Hardware
+License-File: LICENSE.txt
+
+Simulate 6502-based microcomputer systems in Python.
```

### Comparing `py65-1.1.0/py65/monitor.py` & `py65-1.2/py65/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import cmd
 import getopt
 import os
 import re
 import shlex
 import sys
+import traceback
 
-from asyncore import compact_traceback
 from py65.devices.mpu6502 import MPU as NMOS6502
 from py65.devices.mpu65c02 import MPU as CMOS65C02
 from py65.devices.mpu65org16 import MPU as V65Org16
 from py65.disassembler import Disassembler
 from py65.assembler import Assembler
 from py65.utils.addressing import AddressParser
 from py65.utils import console
@@ -49,36 +49,68 @@
         self.memory = memory
         self.putc_addr = putc_addr
         self.getc_addr = getc_addr
         self._breakpoints = []
         self._width = 78
         self.prompt = "."
         self._add_shortcuts()
-        cmd.Cmd.__init__(self, stdin=stdin, stdout=stdout)
 
-        if argv is None:
-            argv = sys.argv
-        load, rom, goto = self._parse_args(argv)
-
-        self._reset(self.mpu_type, self.getc_addr, self.putc_addr)
-
-        if load is not None:
-            self.do_load(load)
-
-        if goto is not None:
-            self.do_goto(goto)
-
-        if rom is not None:
-            # load a ROM and run from the reset vector
-            self.do_load("%r top" % rom)
-            physMask = self._mpu.memory.physMask
-            reset = self._mpu.RESET & physMask
-            dest = self._mpu.memory[reset] + \
-                (self._mpu.memory[reset + 1] << self.byteWidth)
-            self.do_goto("$%x" % dest)
+        # Save the current system input mode so it can be restored after
+        # after processing commands and before exiting.
+        console.save_mode(sys.stdin)
+
+        # Attempt to get a copy of stdin that is unbuffered on systems
+        # that support it.  This allows for immediate response to
+        # typed input as well as pasted input.  If unable to get an
+        # unbuffered version of stdin, the original version is returned.
+        self.unbuffered_stdin = console.get_unbuffered_stdin(stdin)
+
+        cmd.Cmd.__init__(self, stdin=self.unbuffered_stdin, stdout=stdout)
+
+        # Check for any exceptions thrown during __init__ while
+        # processing the arguments.
+        try:
+
+            if argv is None:
+                argv = sys.argv
+            load, rom, goto = self._parse_args(argv)
+
+            self._reset(self.mpu_type, self.getc_addr, self.putc_addr)
+
+            if load is not None:
+                self.do_load("%r" % load)
+
+            if goto is not None:
+                self.do_goto(goto)
+
+            if rom is not None:
+                # load a ROM and run from the reset vector
+                self.do_load("%r top" % rom)
+                physMask = self._mpu.memory.physMask
+                reset = self._mpu.RESET & physMask
+                dest = self._mpu.memory[reset] + \
+                    (self._mpu.memory[reset + 1] << self.byteWidth)
+                self.do_goto("$%x" % dest)
+        except:
+            # Restore input mode on any exception and then rethrow the
+            # exception.
+            console.restore_mode()
+            raise
+
+    def __del__(self):
+        try:
+            # Restore the input mode.
+            console.restore_mode()
+            # Close the unbuffered input file handle, if it exists.
+            if self.unbuffered_stdin != None:
+                if self.unbuffered_stdin != sys.stdin:
+                    self.unbuffered_stdin.close()
+        except:
+            pass
+
 
     def _parse_args(self, argv):
         try:
             shortopts = 'hi:o:m:l:r:g:'
             longopts = ['help', 'mpu=', 'input=', 'output=', 'load=', 'rom=', 'goto=']
             options, args = getopt.getopt(argv[1:], shortopts, longopts)
         except getopt.GetoptError as exc:
@@ -128,21 +160,23 @@
 
         result = None
         try:
             result = cmd.Cmd.onecmd(self, line)
         except KeyboardInterrupt:
             self._output("Interrupt")
         except Exception:
-            (file, fun, line), t, v, tbinfo = compact_traceback()
-            error = 'Error: %s, %s: file: %s line: %s' % (t, v, file, line)
+            error = ''.join(traceback.format_exception(*sys.exc_info()))
             self._output(error)
 
         if not line.startswith("quit"):
             self._output_mpu_status()
 
+        # Switch back to the previous input mode.
+        console.restore_mode()
+
         return result
 
     def _reset(self, mpu_type, getc_addr=0xF004, putc_addr=0xF001):
         self._mpu = mpu_type(memory=self.memory)
         self.addrWidth = self._mpu.ADDR_WIDTH
         self.byteWidth = self._mpu.BYTE_WIDTH
         self.addrFmt = self._mpu.ADDR_FORMAT
@@ -201,15 +235,15 @@
 
         # command shortcuts
         for shortcut, command in self._shortcuts.items():
             if line == shortcut:
                 line = command
                 break
 
-            pattern = '^%s\s+' % re.escape(shortcut)
+            pattern = r'^%s\s+' % re.escape(shortcut)
             matches = re.match(pattern, line)
             if matches:
                 start, end = matches.span()
                 line = "%s %s" % (command, line[end:])
                 break
 
         return line
@@ -463,14 +497,18 @@
 
     def _run(self, stopcodes):
         stopcodes = set(stopcodes)
         breakpoints = set(self._breakpoints)
         mpu = self._mpu
         mem = self._mpu.memory
 
+        # Switch to immediate (noncanonical) no-echo input mode on POSIX
+        # operating systems.  This has no effect on Windows.
+        console.noncanonical_mode(self.stdin)
+
         if not breakpoints:
             while True:
                 mpu.step()
                 if mem[mpu.pc] in stopcodes:
                     break
         else:
             while True:
@@ -479,14 +517,17 @@
                 if mem[pc] in stopcodes:
                     break
                 if pc in breakpoints:
                     msg = "Breakpoint %d reached."
                     self._output(msg % self._breakpoints.index(pc))
                     break
 
+        # Switch back to the previous input mode.
+        console.restore_mode()
+
     def help_radix(self):
         self._output("radix [H|D|O|B]")
         self._output("Set default radix to hex, decimal, octal, or binary.")
         self._output("With no argument, the current radix is printed.")
 
     def help_cycles(self):
         self._output("Display the total number of cycles executed.")
@@ -535,15 +576,15 @@
         self._output("Assign respective registers.  With no parameters,")
         self._output("display register values.")
 
     def do_registers(self, args):
         if args == '':
             return
 
-        pairs = re.findall('([^=,\s]*)=([^=,\s]*)', args)
+        pairs = re.findall(r'([^=,\s]*)=([^=,\s]*)', args)
         if pairs == []:
             return self._output("Syntax error: %s" % args)
 
         for register, value in pairs:
             if register not in ('pc', 'sp', 'a', 'x', 'y', 'p'):
                 self._output("Invalid register: %s" % register)
             else:
@@ -688,17 +729,26 @@
     def do_fill(self, args):
         split = shlex.split(args)
         if len(split) < 2:
             return self.help_fill()
 
         try:
             start, end = self._address_parser.range(split[0])
-            filler = list(map(self._address_parser.number, split[1:]))
+            filler = []
+            for piece in split[1:]:
+                value = self._address_parser.number(piece)
+                if value > self.byteMask:
+                    raise OverflowError(value)
+                filler.append(value)
         except KeyError as exc:
-            self._output(exc.args[0])  # "Label not found: foo"
+            # "Label not found: foo"
+            self._output(exc.args[0])
+        except OverflowError as exc:
+            # "Overflow: $10000"
+            self._output("Overflow: $%x" % exc.args[0])
         else:
             self._fill(start, end, filler)
 
     def _fill(self, start, end, filler):
         address = start
         length, index = len(filler), 0
 
@@ -873,10 +923,11 @@
         pass
 
     try:
         c.onecmd('version')
         c.cmdloop()
     except KeyboardInterrupt:
         c._output('')
+        console.restore_mode()
 
 if __name__ == "__main__":
     main()
```

### Comparing `py65-1.1.0/py65/memory.py` & `py65-1.2/py65/memory.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/disassembler.py` & `py65-1.2/py65/disassembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,16 @@
                 targ, '$' + self.addrFmt % targ)
             disasm += ' ' + address_or_label
             length = 2
 
         elif addressing == 'zpi':
             zp_address = self._mpu.ByteAt(pc + 1)
             address_or_label = self._address_parser.label_for(
-                zp_address, '($' + self.byteFmt % zp_address + ')')
-            disasm += ' %s' % address_or_label
+                zp_address, '$' + self.byteFmt % zp_address)
+            disasm += ' (%s)' % address_or_label
             length = 2
 
         elif addressing == 'zpg':
             zp_address = self._mpu.ByteAt(pc + 1)
             address_or_label = self._address_parser.label_for(
                 zp_address, '$' + self.byteFmt % zp_address)
             disasm += ' %s' % address_or_label
```

### Comparing `py65-1.1.0/py65/tests/test_monitor.py` & `py65-1.2/py65/tests/test_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         out = stdout.getvalue()
         self.assertEqual("$c000  a9 ab     LDA #$ab\n", out)
 
     def test_do_assemble_parses_start_address_label(self):
         stdout = StringIO()
         mon = Monitor(stdout=stdout)
         mon.do_add_label('c000 base')
-        mon.do_assemble('c000 rts')
+        mon.do_assemble('base rts')
 
         mpu = mon._mpu
         self.assertEqual(0x60, mpu.memory[0xC000])
 
     def test_do_assemble_shows_bad_label_error(self):
         stdout = StringIO()
         mon = Monitor(stdout=stdout)
@@ -470,14 +470,38 @@
         stdout = StringIO()
         mon = Monitor(stdout=stdout)
         mon.do_fill('0 nonexistent')
 
         out = stdout.getvalue()
         self.assertTrue(out.startswith("Label not found: nonexistent"))
 
+    def test_do_fill_bad_start_address(self):
+        stdout = StringIO()
+        mon = Monitor(stdout=stdout)
+        mon.do_fill('10000 00')
+
+        out = stdout.getvalue()
+        self.assertTrue(out.startswith("Overflow: $10000"))
+
+    def test_do_fill_bad_end_address(self):
+        stdout = StringIO()
+        mon = Monitor(stdout=stdout)
+        mon.do_fill('ffff:10000 00 00')
+
+        out = stdout.getvalue()
+        self.assertTrue(out.startswith("Overflow: $10000"))
+
+    def test_do_fill_bad_data(self):
+        stdout = StringIO()
+        mon = Monitor(stdout=stdout)
+        mon.do_fill('0 100')
+
+        out = stdout.getvalue()
+        self.assertTrue(out.startswith("Overflow: $100"))
+
     # goto
 
     def test_shortcut_for_goto(self):
         stdout = StringIO()
         mon = Monitor(stdout=stdout)
         mon.do_help('g')
 
@@ -1180,40 +1204,44 @@
         memory[0xc000] = 0xea # c000 nop
         memory[0xc001] = 0xea # c001 nop
         memory[0xc002] = 0x00 # c002 brk
         mon = Monitor(argv=argv, stdout=stdout, memory=memory)
         self.assertEqual(0xc002, mon._mpu.pc)
 
     def test_argv_load(self):
-        with tempfile.NamedTemporaryFile('wb+') as f:
-            data = bytearray([0xab, 0xcd])
-            f.write(data)
-            f.flush()
+        try:
+            with tempfile.NamedTemporaryFile('wb+', delete=False) as f:
+                data = bytearray([0xab, 0xcd])
+                f.write(data)
 
             argv = ['py65mon', '--load', f.name]
             stdout = StringIO()
             mon = Monitor(argv=argv, stdout=stdout)
             self.assertEqual(list(data), mon._mpu.memory[:len(data)])
+        finally:
+            os.unlink(f.name)
 
     def test_argv_rom(self):
-        with tempfile.NamedTemporaryFile('wb+') as f:
-            rom = bytearray(4096)
-            rom[0]  = 0xea          # f000 nop
-            rom[1]  = 0xea          # f001 nop
-            rom[2]  = 0x00          # f002 brk
-            rom[-2] = 0xf000 & 0xff # fffc reset vector low
-            rom[-3] = 0xf000 >> 8   # fffd reset vector high
-            f.write(rom)
-            f.flush()
+        try:
+            with tempfile.NamedTemporaryFile('wb+', delete=False) as f:
+                rom = bytearray(4096)
+                rom[0]  = 0xea          # f000 nop
+                rom[1]  = 0xea          # f001 nop
+                rom[2]  = 0x00          # f002 brk
+                rom[-2] = 0xf000 & 0xff # fffc reset vector low
+                rom[-3] = 0xf000 >> 8   # fffd reset vector high
+                f.write(rom)
 
             argv = ['py65mon', '--rom', f.name]
             stdout = StringIO()
             mon = Monitor(argv=argv, stdout=stdout)
             self.assertEqual(list(rom), mon._mpu.memory[-len(rom):])
             self.assertEqual(0xf002, mon._mpu.pc)
+        finally:
+            os.unlink(f.name)
 
     def test_argv_input(self):
         argv = ['py65mon', '--input', 'abcd']
         stdout = StringIO()
         mon = Monitor(argv=argv, stdout=stdout)
         read_subscribers = mon._mpu.memory._read_subscribers
         self.assertEqual(1, len(read_subscribers))
@@ -1224,29 +1252,31 @@
         stdout = StringIO()
         mon = Monitor(argv=argv, stdout=stdout)
         write_subscribers = mon._mpu.memory._write_subscribers
         self.assertEqual(1, len(write_subscribers))
         self.assertTrue('putc' in repr(write_subscribers[0xdcba]))
 
     def test_argv_combination_rom_mpu(self):
-        with tempfile.NamedTemporaryFile('wb+') as f:
-            rom = bytearray(4096)
-            rom[0]  = 0xea          # f000 nop
-            rom[1]  = 0xea          # f001 nop
-            rom[2]  = 0x00          # f002 brk
-            rom[-2] = 0xf000 & 0xff # fffc reset vector low
-            rom[-3] = 0xf000 >> 8   # fffd reset vector high
-            f.write(rom)
-            f.flush()
+        try:
+            with tempfile.NamedTemporaryFile('wb+', delete=False) as f:
+                rom = bytearray(4096)
+                rom[0]  = 0xea          # f000 nop
+                rom[1]  = 0xea          # f001 nop
+                rom[2]  = 0x00          # f002 brk
+                rom[-2] = 0xf000 & 0xff # fffc reset vector low
+                rom[-3] = 0xf000 >> 8   # fffd reset vector high
+                f.write(rom)
 
             argv = ['py65mon', '--rom', f.name, '--mpu', '65c02',]
             stdout = StringIO()
             mon = Monitor(argv=argv, stdout=stdout)
             self.assertEqual('65C02', mon._mpu.name)
             self.assertEqual(list(rom), mon._mpu.memory[-len(rom):])
             self.assertEqual(0xf002, mon._mpu.pc)
+        finally:
+            os.unlink(f.name)
 
 def test_suite():
     return unittest.findTestCases(sys.modules[__name__])
 
 if __name__ == '__main__':
     unittest.main(defaultTest='test_suite')
```

### Comparing `py65-1.1.0/py65/tests/utils/test_conversions.py` & `py65-1.2/py65/tests/utils/test_conversions.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/tests/utils/test_addressing.py` & `py65-1.2/py65/tests/utils/test_addressing.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/tests/test_disassembler.py` & `py65-1.2/py65/tests/test_disassembler.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,14 +532,20 @@
         self.assertEqual('???', disasm)
 
     def test_disassembles_64(self):
         length, disasm = self.disassemble([0x64])
         self.assertEqual(1, length)
         self.assertEqual('???', disasm)
 
+    def test_disassembles_64_65c02(self):
+        mpu = MPU65C02()
+        length, disasm = self.disassemble([0x64, 0x12], 0x0000, mpu)
+        self.assertEqual(2, length)
+        self.assertEqual('STZ $12', disasm)
+
     def test_disassembles_65(self):
         length, disasm = self.disassemble([0x65, 0x44])
         self.assertEqual(2, length)
         self.assertEqual('ADC $44', disasm)
 
     def test_disassembles_66(self):
         length, disasm = self.disassemble([0x66, 0x44])
```

### Comparing `py65-1.1.0/py65/tests/test_memory.py` & `py65-1.2/py65/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/tests/test_assembler.py` & `py65-1.2/py65/tests/test_assembler.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,16 +497,16 @@
         pass
 
     def dont_test_assembles_64(self):
         pass
 
     def test_assembles_64_65c02(self):
         mpu = MPU65C02()
-        self.assertEqual([0x64],
-                         self.assemble('STZ', 0x0000, mpu))
+        self.assertEqual([0x64, 0x12],
+                         self.assemble('STZ $12', 0x0000, mpu))
 
     def test_assembles_65(self):
         self.assertEqual([0x65, 0x44],
                          self.assemble('ADC $44'))
 
     def test_assembles_66(self):
         self.assertEqual([0x66, 0x44],
```

### Comparing `py65-1.1.0/py65/tests/devices/test_mpu65c02.py` & `py65-1.2/py65/tests/devices/test_mpu65c02.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/tests/devices/test_mpu6502.py` & `py65-1.2/py65/tests/devices/test_mpu6502.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,32 @@
         mpu.reset()
         self.assertEqual(0xFF, mpu.sp)
         self.assertEqual(0, mpu.a)
         self.assertEqual(0, mpu.x)
         self.assertEqual(0, mpu.y)
         self.assertEqual(mpu.BREAK | mpu.UNUSED, mpu.p)
 
+    def test_reset_sets_pc_to_0_by_default(self):
+        mpu = self._make_mpu()
+        mpu.reset()
+        self.assertEqual(mpu.pc, 0)
+
+    def test_reset_sets_pc_to_start_pc_if_not_None(self):
+        mpu = self._make_mpu(pc=0x1234)
+        mpu.reset()
+        self.assertEqual(mpu.pc, 0x1234)
+
+    def test_reset_reads_reset_vector_if_start_pc_is_None(self):
+        mpu = self._make_mpu(pc=None)
+        target = 0xABCD
+        mpu.memory[mpu.RESET+0] = target & 0xff
+        mpu.memory[mpu.RESET+1] = target >> 8
+        mpu.reset()
+        self.assertEqual(mpu.pc, 0xABCD)
+
     # ADC Absolute
 
     def test_adc_bcd_off_absolute_carry_clear_in_accumulator_zeroes(self):
         mpu = self._make_mpu()
         mpu.a = 0
         # $0000 ADC $C000
         self._write(mpu.memory, 0x0000, (0x6D, 0x00, 0xC0))
@@ -1558,19 +1576,19 @@
         mpu.step()
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bcc_carry_clear_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.CARRY)
         mpu.pc = 0x0050
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         # $0000 BCC -6
         self._write(mpu.memory, 0x0050, (0x90, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bcc_carry_set_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.CARRY
         # $0000 BCC +6
         self._write(mpu.memory, 0x0000, (0x90, 0x06))
         mpu.step()
@@ -1586,19 +1604,19 @@
         mpu.step()
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bcs_carry_set_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.CARRY
         mpu.pc = 0x0050
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         # $0000 BCS -6
         self._write(mpu.memory, 0x0050, (0xB0, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bcs_carry_clear_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.CARRY)
         # $0000 BCS +6
         self._write(mpu.memory, 0x0000, (0xB0, 0x06))
         mpu.step()
@@ -1614,19 +1632,19 @@
         mpu.step()
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_beq_zero_set_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.ZERO
         mpu.pc = 0x0050
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         # $0000 BEQ -6
         self._write(mpu.memory, 0x0050, (0xF0, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_beq_zero_clear_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.ZERO)
         # $0000 BEQ +6
         self._write(mpu.memory, 0x0000, (0xF0, 0x06))
         mpu.step()
@@ -1813,18 +1831,18 @@
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bmi_negative_set_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.NEGATIVE
         mpu.pc = 0x0050
         # $0000 BMI -6
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         self._write(mpu.memory, 0x0050, (0x30, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bmi_negative_clear_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.NEGATIVE)
         # $0000 BEQ +6
         self._write(mpu.memory, 0x0000, (0x30, 0x06))
         mpu.step()
@@ -1841,18 +1859,18 @@
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bne_zero_clear_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.ZERO)
         mpu.pc = 0x0050
         # $0050 BNE -6
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         self._write(mpu.memory, 0x0050, (0xD0, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bne_zero_set_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.ZERO
         # $0000 BNE +6
         self._write(mpu.memory, 0x0000, (0xD0, 0x06))
         mpu.step()
@@ -1869,18 +1887,18 @@
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bpl_negative_clear_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.NEGATIVE)
         mpu.pc = 0x0050
         # $0050 BPL -6
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         self._write(mpu.memory, 0x0050, (0x10, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bpl_negative_set_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.NEGATIVE
         # $0000 BPL +6
         self._write(mpu.memory, 0x0000, (0x10, 0x06))
         mpu.step()
@@ -1901,33 +1919,65 @@
         self.assertEqual(0xC0, mpu.memory[0x1FF])  # PCH
         self.assertEqual(0x02, mpu.memory[0x1FE])  # PCL
         self.assertEqual(mpu.BREAK | mpu.UNUSED, mpu.memory[0x1FD])  # Status
         self.assertEqual(0xFC, mpu.sp)
 
         self.assertEqual(mpu.BREAK | mpu.UNUSED | mpu.INTERRUPT, mpu.p)
 
+    # IRQ and NMI handling (very similar to BRK)
+
+    def test_irq_pushes_pc_and_correct_status_then_sets_pc_to_irq_vector(self):
+        mpu = self._make_mpu()
+        mpu.p = mpu.UNUSED
+        self._write(mpu.memory, 0xFFFA, (0x88, 0x77))
+        self._write(mpu.memory, 0xFFFE, (0xCD, 0xAB))
+        mpu.pc = 0xC123
+        mpu.irq()
+        self.assertEqual(0xABCD, mpu.pc)
+        self.assertEqual(0xC1, mpu.memory[0x1FF])  # PCH
+        self.assertEqual(0x23, mpu.memory[0x1FE])  # PCL
+        self.assertEqual(mpu.UNUSED, mpu.memory[0x1FD])  # Status
+        self.assertEqual(0xFC, mpu.sp)
+        self.assertEqual(mpu.UNUSED | mpu.INTERRUPT, mpu.p)
+        self.assertEqual(7, mpu.processorCycles)
+
+    def test_nmi_pushes_pc_and_correct_status_then_sets_pc_to_nmi_vector(self):
+        mpu = self._make_mpu()
+        mpu.p = mpu.UNUSED
+        self._write(mpu.memory, 0xFFFA, (0x88, 0x77))
+        self._write(mpu.memory, 0xFFFE, (0xCD, 0xAB))
+        mpu.pc = 0xC123
+        mpu.nmi()
+        self.assertEqual(0x7788, mpu.pc)
+        self.assertEqual(0xC1, mpu.memory[0x1FF])  # PCH
+        self.assertEqual(0x23, mpu.memory[0x1FE])  # PCL
+        self.assertEqual(mpu.UNUSED, mpu.memory[0x1FD])  # Status
+        self.assertEqual(0xFC, mpu.sp)
+        self.assertEqual(mpu.UNUSED | mpu.INTERRUPT, mpu.p)
+        self.assertEqual(7, mpu.processorCycles)
+
     # BVC
 
     def test_bvc_overflow_clear_branches_relative_forward(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.OVERFLOW)
         # $0000 BVC +6
         self._write(mpu.memory, 0x0000, (0x50, 0x06))
         mpu.step()
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bvc_overflow_clear_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.OVERFLOW)
         mpu.pc = 0x0050
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         # $0050 BVC -6
         self._write(mpu.memory, 0x0050, (0x50, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bvc_overflow_set_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.OVERFLOW
         # $0000 BVC +6
         self._write(mpu.memory, 0x0000, (0x50, 0x06))
         mpu.step()
@@ -1943,19 +1993,19 @@
         mpu.step()
         self.assertEqual(0x0002 + 0x06, mpu.pc)
 
     def test_bvs_overflow_set_branches_relative_backward(self):
         mpu = self._make_mpu()
         mpu.p |= mpu.OVERFLOW
         mpu.pc = 0x0050
-        rel = (0x06 ^ 0xFF + 1)  # two's complement of 6
+        rel = (0x06 ^ 0xFF) + 1  # two's complement of 6
         # $0050 BVS -6
         self._write(mpu.memory, 0x0050, (0x70, rel))
         mpu.step()
-        self.assertEqual(0x0052 + rel, mpu.pc)
+        self.assertEqual(0x0052 - 0x06, mpu.pc)
 
     def test_bvs_overflow_clear_does_not_branch(self):
         mpu = self._make_mpu()
         mpu.p &= ~(mpu.OVERFLOW)
         # $0000 BVS +6
         self._write(mpu.memory, 0x0000, (0x70, 0x06))
         mpu.step()
@@ -2001,14 +2051,145 @@
         mpu.p |= mpu.OVERFLOW
         # $0000 CLV
         mpu.memory[0x0000] = 0xB8
         mpu.step()
         self.assertEqual(0x0001, mpu.pc)
         self.assertEqual(0, mpu.p & mpu.OVERFLOW)
 
+    # Compare instructions
+
+    # See http://6502.org/tutorials/compare_instructions.html
+    # and http://www.6502.org/tutorials/compare_beyond.html
+    # Cheat sheet:
+    #
+    #    - Comparison is actually subtraction "register - memory"
+    #    - Z contains equality result (1 equal, 0 not equal)
+    #    - C contains result of unsigned comparison (0 if A<m, 1 if A>=m)
+    #    - N holds MSB of subtraction result (*NOT* of signed subtraction)
+    #    - V is not affected by comparison
+    #    - D has no effect on comparison
+
+    # CMP Immediate
+
+    def test_cmp_imm_sets_zero_carry_clears_neg_flags_if_equal(self):
+        """Comparison: A == m"""
+        mpu = self._make_mpu()
+        # $0000 CMP #10 , A will be 10
+        self._write(mpu.memory, 0x0000, (0xC9, 10))
+        mpu.a = 10
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE)
+        self.assertEqual(mpu.ZERO, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY)
+
+    def test_cmp_imm_clears_zero_carry_takes_neg_if_less_unsigned(self):
+        """Comparison: A < m (unsigned)"""
+        mpu = self._make_mpu()
+        # $0000 CMP #10 , A will be 1
+        self._write(mpu.memory, 0x0000, (0xC9, 10))
+        mpu.a = 1
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(mpu.NEGATIVE, mpu.p & mpu.NEGATIVE) # 0x01-0x0A=0xF7
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(0, mpu.p & mpu.CARRY)
+
+    def test_cmp_imm_clears_zero_sets_carry_takes_neg_if_less_signed(self):
+        """Comparison: A < #nn (signed), A negative"""
+        mpu = self._make_mpu()
+        # $0000 CMP #1, A will be -1 (0xFF)
+        self._write(mpu.memory, 0x0000, (0xC9, 1))
+        mpu.a = 0xFF
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(mpu.NEGATIVE, mpu.p & mpu.NEGATIVE) # 0xFF-0x01=0xFE
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY) # A>m unsigned
+
+    def test_cmp_imm_clears_zero_carry_takes_neg_if_less_signed_nega(self):
+        """Comparison: A < m (signed), A and m both negative"""
+        mpu = self._make_mpu()
+        # $0000 CMP #0xFF (-1), A will be -2 (0xFE)
+        self._write(mpu.memory, 0x0000, (0xC9, 0xFF))
+        mpu.a = 0xFE
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(mpu.NEGATIVE, mpu.p & mpu.NEGATIVE) # 0xFE-0xFF=0xFF
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(0, mpu.p & mpu.CARRY) # A<m unsigned
+
+    def test_cmp_imm_clears_zero_sets_carry_takes_neg_if_more_unsigned(self):
+        """Comparison: A > m (unsigned)"""
+        mpu = self._make_mpu()
+        # $0000 CMP #1 , A will be 10
+        self._write(mpu.memory, 0x0000, (0xC9, 1))
+        mpu.a = 10
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE) # 0x0A-0x01 = 0x09
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY) # A>m unsigned
+
+    def test_cmp_imm_clears_zero_carry_takes_neg_if_more_signed(self):
+        """Comparison: A > m (signed), memory negative"""
+        mpu = self._make_mpu()
+        # $0000 CMP #$FF (-1), A will be 2
+        self._write(mpu.memory, 0x0000, (0xC9, 0xFF))
+        mpu.a = 2
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE) # 0x02-0xFF=0x01
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(0, mpu.p & mpu.CARRY) # A<m unsigned
+
+    def test_cmp_imm_clears_zero_carry_takes_neg_if_more_signed_nega(self):
+        """Comparison: A > m (signed), A and m both negative"""
+        mpu = self._make_mpu()
+        # $0000 CMP #$FE (-2), A will be -1 (0xFF)
+        self._write(mpu.memory, 0x0000, (0xC9, 0xFE))
+        mpu.a = 0xFF
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE) # 0xFF-0xFE=0x01
+        self.assertEqual(0, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY) # A>m unsigned
+
+
+    # CPX Immediate
+
+    def test_cpx_imm_sets_zero_carry_clears_neg_flags_if_equal(self):
+        """Comparison: X == m"""
+        mpu = self._make_mpu()
+        # $0000 CPX #$20
+        self._write(mpu.memory, 0x0000, (0xE0, 0x20))
+        mpu.x = 0x20
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(mpu.ZERO, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE)
+
+
+    # CPY Immediate
+
+    def test_cpy_imm_sets_zero_carry_clears_neg_flags_if_equal(self):
+        """Comparison: Y == m"""
+        mpu = self._make_mpu()
+        # $0000 CPY #$30
+        self._write(mpu.memory, 0x0000, (0xC0, 0x30))
+        mpu.y = 0x30
+        mpu.step()
+        self.assertEqual(0x0002, mpu.pc)
+        self.assertEqual(mpu.ZERO, mpu.p & mpu.ZERO)
+        self.assertEqual(mpu.CARRY, mpu.p & mpu.CARRY)
+        self.assertEqual(0, mpu.p & mpu.NEGATIVE)
+
+
+
     # DEC Absolute
 
     def test_dec_abs_decrements_memory(self):
         mpu = self._make_mpu()
         # $0000 DEC 0xABCD
         self._write(mpu.memory, 0x0000, (0xCE, 0xCD, 0xAB))
         mpu.memory[0xABCD] = 0x10
```

### Comparing `py65-1.1.0/py65/utils/conversions.py` & `py65-1.2/py65/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/utils/addressing.py` & `py65-1.2/py65/utils/addressing.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 return self._constrain(int(num[1:], 2))
 
             elif num in self.labels:
                 # label name
                 return self.labels[num]
 
             else:
-                matches = re.match('^([^\s+-]+)\s*([+\-])\s*([$+%]?\d+)$', num)
+                matches = re.match(r'^([^\s+-]+)\s*([+\-])\s*([$+%]?\d+)$', num)
                 if matches:
                     label, sign, offset = matches.groups()
 
                     if label not in self.labels:
                         raise KeyError("Label not found: %s" % label)
 
                     base = self.labels[label]
@@ -84,15 +84,15 @@
         except ValueError:
             raise KeyError("Label not found: %s" % num)
 
     def range(self, addresses):
         """Parse a string containing an address or a range of addresses
         into a tuple of (start address, end address)
         """
-        matches = re.match('^([^:,]+)\s*[:,]+\s*([^:,]+)$', addresses)
+        matches = re.match(r'^([^:,]+)\s*[:,]+\s*([^:,]+)$', addresses)
         if matches:
             start, end = map(self.number, matches.groups(0))
         else:
             start = end = self.number(addresses)
 
         if start > end:
             start, end = end, start
```

### Comparing `py65-1.1.0/py65/assembler.py` & `py65-1.2/py65/assembler.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     def normalize_and_split(self, statement):
         """ Given an assembly language statement like "lda $c12,x", normalize
             the statement by uppercasing it, removing unnecessary whitespace,
             and parsing the address part using AddressParser.  The result of
             the normalization is a tuple of two strings (opcode, operand).
         """
-        statement = ' '.join(str.split(statement))
+        statement = ' '.join(statement.split())
 
         # normalize target in operand
         match = self.Statement.match(statement)
         if match:
             before, target, after = match.groups()
 
             # target is an immediate value
```

### Comparing `py65-1.1.0/py65/devices/mpu65org16.py` & `py65-1.2/py65/devices/mpu65org16.py`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/py65/devices/mpu6502.py` & `py65-1.2/py65/devices/mpu6502.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.excycles = 0
         self.addcycles = False
         self.processorCycles = 0
 
         if memory is None:
             memory = 0x10000 * [0x00]
         self.memory = memory
-        self.start_pc = pc
+        self.start_pc = pc # if None, reset vector is used
 
         # init
         self.reset()
 
     def reprformat(self):
         return ("%s PC  AC XR YR SP NV-BDIZC\n"
                 "%s: %04x %02x %02x %02x %02x %s")
@@ -63,21 +63,45 @@
         self.instruct[instructCode](self)
         self.pc &= self.addrMask
         self.processorCycles += self.cycletime[instructCode] + self.excycles
         return self
 
     def reset(self):
         self.pc = self.start_pc
+        if self.pc is None:
+            self.pc = self.WordAt(self.RESET)
         self.sp = self.byteMask
         self.a = 0
         self.x = 0
         self.y = 0
         self.p = self.BREAK | self.UNUSED
         self.processorCycles = 0
 
+    def irq(self):
+        # triggers a normal IRQ
+        # this is very similar to the BRK instruction
+        if self.p & self.INTERRUPT:
+            return
+        self.stPushWord(self.pc)
+        self.p &= ~self.BREAK
+        self.stPush(self.p | self.UNUSED)
+        self.p |= self.INTERRUPT
+        self.pc = self.WordAt(self.IRQ)
+        self.processorCycles += 7
+
+    def nmi(self):
+        # triggers a NMI IRQ in the processor
+        # this is very similar to the BRK instruction
+        self.stPushWord(self.pc)
+        self.p &= ~self.BREAK
+        self.stPush(self.p | self.UNUSED)
+        self.p |= self.INTERRUPT
+        self.pc = self.WordAt(self.NMI)
+        self.processorCycles += 7
+
     # Helpers for addressing modes
 
     def ByteAt(self, addr):
         return self.memory[addr]
 
     def WordAt(self, addr):
         return self.ByteAt(addr) + (self.ByteAt(addr + 1) << self.BYTE_WIDTH)
```

### Comparing `py65-1.1.0/py65/devices/mpu65c02.py` & `py65-1.2/py65/devices/mpu65c02.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         self.opRMB(self.ZeroPageAddr, 0xDF)
         self.pc += 1
 
     @instruction(name="PHY", mode="imp", cycles=3)
     def inst_0x5a(self):
         self.stPush(self.y)
 
-    @instruction(name="STZ", mode="imp", cycles=3)
+    @instruction(name="STZ", mode="zpg", cycles=3)
     def inst_0x64(self):
         self.opSTZ(self.ZeroPageAddr)
         self.pc += 1
 
     @instruction(name="RMB6", mode="zpg", cycles=5)
     def inst_0x67(self):
         self.opRMB(self.ZeroPageAddr, 0xBF)
```

### Comparing `py65-1.1.0/docs/index.rst` & `py65-1.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,18 @@
          PC  AC XR YR SP NV-BDIZC
   6502: 0000 00 00 00 ff 00110000
   .
 
 Once the monitor has started, it will display a register dump and the
 dot prompt.  You can then enter commands for the monitor at this prompt.
 
-Py65Mon uses commands that are very similar to those used by the monitor
-included with the `VICE emulator <http://viceteam.org>`_ for Commodore
-computers.  You can get a list of available commands with ``help`` or
-help on a specific command with ``help command``.
+Py65Mon uses commands that are very similar to those used by the
+`VICE emulator's monitor <http://vice-emu.sourceforge.net/vice_12.html>`_
+for Commodore computers.  You can get a list of available commands
+with ``help`` or help on a specific command with ``help command``.
 
 Number Systems
 --------------
 
 When working with Py65Mon, you will frequently need to enter numbers, addresses,
 and ranges of addresses.  Almost all Py65 command support entering numbers in
 binary, decimal, and hexadecimal.
@@ -128,15 +128,15 @@
 by ``add_breakpoint``::
 
   .add_breakpoint $ff84
   Breakpoint 0 added at $FF84
   .delete_breakpoint 0
   Breakpoint 0 removed
 
-Breakpoint can be listed using the ``list_breakpoint`` command::
+Breakpoints can be listed using the ``show_breakpoints`` command::
 
   .add_breakpoint $1234
   Breakpoint 0 added at $1234
   .add_breakpoint $5678
   Breakpoint 1 added at $5678
   .add_breakpoint $9ABC
   Breakpoint 2 added at $9ABC
```

### Comparing `py65-1.1.0/docs/Makefile` & `py65-1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/docs/conf.py` & `py65-1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 copyright = u'2008-%d, Mike Naberezny and contributors' % year
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.1.0'
+version = '1.2.0'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `py65-1.1.0/CHANGES.txt` & `py65-1.2/CHANGES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,334 +1,361 @@
+1.2.0 (2024-04-12)
+------------------
+
+- Fixed a bug with character input that would cause characters to be
+  dropped when pasting in larger amounts of text.  This makes it possible
+  to paste programs into EhBASIC and Taliforth.  Patch by SamCoVT.
+
+- Fixed interactive assembly on Python 3.
+
+- Fixed regular expression warnings on Python 3.12.
+
+- The ``fill`` command in the monitor now shows an error message if an
+  address or value is out of range.
+
+- Added ``irq()`` and ``nmi()`` methods to the ``MPU`` class, so that
+  interrupts can be simulated. Patch by Irmen de Jong.
+
+- The ``MPU`` class constructor now accepts ``None`` for the initial PC, which
+  will cause it to read the address from the reset vector on ``reset()``.
+
+- The ``py65`` package is no longer a namespace package.
+
+- Fixed assembly and disassembly of 65C02 instruction $64 (``STZ $12``).
+  Patch by Patrick Surry.
+
+- Removed use of the ``asyncore`` module deprecated in Python 3.10.
+
 1.1.0 (2018-07-01)
 ------------------
 
- - The ``Monitor`` class now allows the default memory to be supplied in
-   the constructor.  Patch by Irmen de Jong.
+- The ``Monitor`` class now allows the default memory to be supplied in
+  the constructor.  Patch by Irmen de Jong.
 
- - Fixed a bug where setting the MPU via ``py65mon`` command line arguments
-   would have no effect.  Reported by Michael A. Morris, patch by Ed Spittles.
+- Fixed a bug where setting the MPU via ``py65mon`` command line arguments
+  would have no effect.  Reported by Michael A. Morris, patch by Ed Spittles.
 
- - The ``itoa()`` function in ``conversions.py`` now raises an error when an
-   unsupported base is given.  Patch by Scot W. Stevenson.
+- The ``itoa()`` function in ``conversions.py`` now raises an error when an
+  unsupported base is given.  Patch by Scot W. Stevenson.
 
- - The unused hexdump loader utility has been removed.
+- The unused hexdump loader utility has been removed.
 
 1.0.0 (2017-05-11)
 ------------------
 
- - Fixed a bug where the ordering of ``py65mon`` command line arguments
-   produced different results.  Arguments can now be specified in any
-   order.  Patch by Mario Keller.
-
- - Added new ``--input`` and ``--output`` arguments to ``py65mon`` that
-   allow the addresses of the ``getc`` and ``putc`` handlers to be
-   changed.  Patch by Mario Keller.
+- Fixed a bug where the ordering of ``py65mon`` command line arguments
+  produced different results.  Arguments can now be specified in any
+  order.  Patch by Mario Keller.
+
+- Added new ``--input`` and ``--output`` arguments to ``py65mon`` that
+  allow the addresses of the ``getc`` and ``putc`` handlers to be
+  changed.  Patch by Mario Keller.
 
- - Fixed a 65C02 bug where the TSB and TRB instructions did not set
-   the Z flag correctly.  Thanks to Kris Kennaway for reporting it.
+- Fixed a 65C02 bug where the TSB and TRB instructions did not set
+  the Z flag correctly.  Thanks to Kris Kennaway for reporting it.
 
 0.24 (2015-03-31)
 -----------------
 
- - Released as a universal wheel.
+- Released as a universal wheel.
 
 0.23 (2015-02-10)
 -----------------
 
- - Added a workaround to $F001 output to catch encoding errors and
-   display a "?" instead of crashing.  This condition can occur if
-   the 6502 program sends bytes to $F001 that aren't compatible with
-   the terminal's character encoding.
+- Added a workaround to $F001 output to catch encoding errors and
+  display a "?" instead of crashing.  This condition can occur if
+  the 6502 program sends bytes to $F001 that aren't compatible with
+  the terminal's character encoding.
 
 0.22 (2015-02-09)
 -----------------
 
- - Fixed a bug where ``py65mon --rom`` would raise an exception
-   on Python 3.
+- Fixed a bug where ``py65mon --rom`` would raise an exception
+  on Python 3.
 
 0.21 (2015-02-09)
 -----------------
 
- - Added support for breakpoints in the monitor.  Contributed by
-   Alessandro Gatti.
+- Added support for breakpoints in the monitor.  Contributed by
+  Alessandro Gatti.
 
- - ASCII literals are now supported by the assembler.  The statement
-   "LDA #'A'" is equivalent to "LDA #$41".
+- ASCII literals are now supported by the assembler.  The statement
+  "LDA #'A'" is equivalent to "LDA #$41".
 
- - Fixed console input when run under Python 3 on Windows.  Closes #27.
+- Fixed console input when run under Python 3 on Windows.  Closes #27.
 
 0.20 (2014-05-08)
 -----------------
 
-  - Page wrapping for indexed indirect (X) operations on 65C02 has been
-    restored.  This reverts the change introduced in 0.18.  We now believe
-    that this mode works the same on the 65C02 as it does on the 6502.
+- Page wrapping for indexed indirect (X) operations on 65C02 has been
+  restored.  This reverts the change introduced in 0.18.  We now believe
+  that this mode works the same on the 65C02 as it does on the 6502.
 
 0.19 (2014-03-12)
 -----------------
 
-  - Fixed 65C02 opcode $D2: CMP Zero Page, Indirect.
+- Fixed 65C02 opcode $D2: CMP Zero Page, Indirect.
 
-  - Blocking character input at $F005 has been removed.  The I/O area
-    was designed to be compatible with Michal Kowalski's simulator,
-    and it uses this address for another purpose.  Examples that depended
-    on $F005 have been changed to use $F004.
+- Blocking character input at $F005 has been removed.  The I/O area
+  was designed to be compatible with Michal Kowalski's simulator,
+  and it uses this address for another purpose.  Examples that depended
+  on $F005 have been changed to use $F004.
 
 0.18 (2014-01-30)
 -----------------
 
-  - Fixed a bug in RTS where popping $FFFF off the stack would cause
-    the program counter to overflow to $10000.  It now wraps around
-    to $0000 as it should.  Thanks to Gábor Lénárt for reporting it.
+- Fixed a bug in RTS where popping $FFFF off the stack would cause
+  the program counter to overflow to $10000.  It now wraps around
+  to $0000 as it should.  Thanks to Gábor Lénárt for reporting it.
 
-  - Fixed BRK on 65C02 so it clears the decimal flag.  On NMOS 6502, the
-    decimal flag is unaffected on BRK.  On 65C02, it is always cleared.
+- Fixed BRK on 65C02 so it clears the decimal flag.  On NMOS 6502, the
+  decimal flag is unaffected on BRK.  On 65C02, it is always cleared.
 
-  - Assembling now tolerates extra whitespace between opcode and operand.
+- Assembling now tolerates extra whitespace between opcode and operand.
 
-  - Removed page wrap bug from JMP indirect on 65C02.
+- Removed page wrap bug from JMP indirect on 65C02.
 
-  - Removed page wrap bug from indexed indirect (X) operations on 65C02.
+- Removed page wrap bug from indexed indirect (X) operations on 65C02.
 
 0.17 (2013-10-26)
 -----------------
 
-  - Added support for Python 3.2 and 3.3 based on work by David Beazley.
+- Added support for Python 3.2 and 3.3 based on work by David Beazley.
 
 0.16 (2013-04-03)
 -----------------
 
-  - Fixed a bug in the monitor that caused loading from the command
-    line with "--rom" to crash.
+- Fixed a bug in the monitor that caused loading from the command
+  line with "--rom" to crash.
 
 0.15 (2013-01-06)
 -----------------
 
-  - Disassembling can now wrap around memory if the start address
-    given is greater than the end address.
+- Disassembling can now wrap around memory if the start address
+  given is greater than the end address.
 
-  - Fixed the disassembler to accept a range of "start:end" instead of
-    "start:end+1" for consistency with the other commands.
+- Fixed the disassembler to accept a range of "start:end" instead of
+  "start:end+1" for consistency with the other commands.
 
 0.14 (2012-11-30)
 -----------------
 
-  - Assembling now detects syntax errors, overflows, and bad labels
-    separately and shows specific error messages.
+- Assembling now detects syntax errors, overflows, and bad labels
+  separately and shows specific error messages.
 
-  - Fixed assembling 65C02 opcodes whose mnemonics have a digit
-    such as "RMB3".
+- Fixed assembling 65C02 opcodes whose mnemonics have a digit
+  such as "RMB3".
 
-  - Reformatted source code to comply with PEP8.
+- Reformatted source code to comply with PEP8.
 
-  - Fixed a bug where the MPU status display would wrap unexpectedly
-    on some terminals.
+- Fixed a bug where the MPU status display would wrap unexpectedly
+  on some terminals.
 
-  - Added support for 65C02 opcode 0x89: BIT #.
+- Added support for 65C02 opcode 0x89: BIT #.
 
-  - Added support for 65C02 opcode 0x7C: JMP (abs,x).
+- Added support for 65C02 opcode 0x7C: JMP (abs,x).
 
-  - Assembling now shows an Overflow Error if the statement won't
-    fit at the top of memory.
+- Assembling now shows an Overflow Error if the statement won't
+  fit at the top of memory.
 
-  - Fixed a bug in the disassembler where instructions that wrap past
-    the top of memory would not be displayed properly.
+- Fixed a bug in the disassembler where instructions that wrap past
+  the top of memory would not be displayed properly.
 
 0.13 (2012-11-15)
 -----------------
 
-  - Fixed a bug where negative numbers could be entered
-    for addresses in the monitor.
+- Fixed a bug where negative numbers could be entered
+  for addresses in the monitor.
 
 0.12 (2012-02-16)
 -----------------
 
-  - Fixed a bug that caused ``help cd`` to raise an exception
-    in the monitor.
+- Fixed a bug that caused ``help cd`` to raise an exception
+  in the monitor.
 
-  - Fixed a bug in the 65C02 simulation where the opcode 0x7A
-    was named "PHY" instead of "PLY", causing incorrect assembly
-    and disassembly.  Thanks to Brian Cassidy for reporting it.
+- Fixed a bug in the 65C02 simulation where the opcode 0x7A
+  was named "PHY" instead of "PLY", causing incorrect assembly
+  and disassembly.  Thanks to Brian Cassidy for reporting it.
 
-  - Fixed the cycle count of 0xD2 (CMP zero page indirect) in
-    the 65C02 simulation.  Thanks to Brian Cassidy for reporting it.
+- Fixed the cycle count of 0xD2 (CMP zero page indirect) in
+  the 65C02 simulation.  Thanks to Brian Cassidy for reporting it.
 
-  - Added "h" as a monitor shortcut for "help".
+- Added "h" as a monitor shortcut for "help".
 
 0.11 (2012-01-07)
 -----------------
 
-  - Added a new 65Org16 MPU simulation written by Ed Spittles.
+- Added a new 65Org16 MPU simulation written by Ed Spittles.
 
-  - The monitor now accepts command line arguments.  See
-    ``py65mon --help`` for usage.  Contributed by Ed Spittles.
+- The monitor now accepts command line arguments.  See
+  ``py65mon --help`` for usage.  Contributed by Ed Spittles.
 
-  - The monitor's load command can now fetch URLs.
+- The monitor's load command can now fetch URLs.
 
-  - Python versions earlier than 2.6 are no longer supported.
+- Python versions earlier than 2.6 are no longer supported.
 
 0.10 (2011-08-27)
 -----------------
 
-  - Fixed long-standing bugs in relative branch calculations in the
-    assembler and disassembler.  Based on a patch by Ed Spittles.
+- Fixed long-standing bugs in relative branch calculations in the
+  assembler and disassembler.  Based on a patch by Ed Spittles.
 
-  - Zero page operations now have the correct page wrap around.
-    Patch by Martti Kühne.
+- Zero page operations now have the correct page wrap around.
+  Patch by Martti Kühne.
 
 0.9 (2011-03-27)
 ----------------
 
-  - Fixed two monitor tests that were broken under Windows.  Thanks
-    to Oscar Lindberg for reporting this.
+- Fixed two monitor tests that were broken under Windows.  Thanks
+  to Oscar Lindberg for reporting this.
 
-  - Removed use of defaultdict to fix compatibility with Python 2.4.
+- Removed use of defaultdict to fix compatibility with Python 2.4.
 
-  - Decimal mode bugs have been fixed.  Thanks to Ed Spittles who
-    ported Bruce Clark's tests to find failures and then rewrote
-    the decimal handling code.
+- Decimal mode bugs have been fixed.  Thanks to Ed Spittles who
+  ported Bruce Clark's tests to find failures and then rewrote
+  the decimal handling code.
 
 0.8 (2010-03-08)
 ----------------
 
-  - Fixed deprecation warnings on Python 2.6
+- Fixed deprecation warnings on Python 2.6
 
-  - We no longer bundle ez_setup to bootstrap setuptools installation.
+- We no longer bundle ez_setup to bootstrap setuptools installation.
 
-  - Restoring the processor status register from interrupt now correctly
-    set the BREAK and UNUSED flags to be high.  Thanks to Ed Spittles
-    for reporting this.
+- Restoring the processor status register from interrupt now correctly
+  set the BREAK and UNUSED flags to be high.  Thanks to Ed Spittles
+  for reporting this.
 
-  - Applied patch by Ed Spittles that fixes the behavior of the BREAK
-    and UNUSED flags in the processor status register.  Closes #16.
+- Applied patch by Ed Spittles that fixes the behavior of the BREAK
+  and UNUSED flags in the processor status register.  Closes #16.
 
-  - Added ">" as a monitor shortcut for the fill command for
-    consistency with VICE.
+- Added ">" as a monitor shortcut for the fill command for
+  consistency with VICE.
 
 0.7 (2009-09-03)
 ----------------
 
-  - When using the monitor, the nonblocking character input at
-    $F004 should now work on the Microsoft Windows platform.
+- When using the monitor, the nonblocking character input at
+  $F004 should now work on the Microsoft Windows platform.
 
-  - Fixed that relative branch calculations would not use the correct
-    start address when assembling in the monitor.  Closes #10.
+- Fixed that relative branch calculations would not use the correct
+  start address when assembling in the monitor.  Closes #10.
 
-  - The processor status register ("p" or "flags") can now be changed
-    in the monitor using the "registers" command with an argument of
-    "p", such as "registers p=00".
-
-  - MPU objects now return a two-line string as their __repr__ with
-    the processor status register displayed as binary for readability.
-
-  - The processor status register is now initialized to 0 on reset.
-    Previously, its unused bit (bit 5) was set to 1 on reset.
-
-  - Applied patch from Ed Spittles to change the CMP algorithm so that
-    it no longer fails Rob Finch's test suite.  Closes #8.
-
-  - Added a new interactive assembly mode to the monitor.  Entering the
-    the assemble command with a statement such as "a c000 lda #0" works
-    as before.  Entering "a c000" will start the interactive assembler
-    at that address.  Entering "a" alone will start it at the current
-    program counter.
-
-  - Applied patch from Ed Spittles so that SBC now properly sets the
-    Overflow (V) flag.  This fixes a failure in Rob Finch's test suite.
-    Closes #6.
-
-  - Applied patch from Ed Spittles so that SBC now properly sets the
-    Carry (C) and Zero (Z) flags.  This fixes failures caught by Ed's
-    own tests (see http://forum.6502.org/viewtopic.php?p=8854#8854).
-    Closes #15.
+- The processor status register ("p" or "flags") can now be changed
+  in the monitor using the "registers" command with an argument of
+  "p", such as "registers p=00".
+
+- MPU objects now return a two-line string as their __repr__ with
+  the processor status register displayed as binary for readability.
+
+- The processor status register is now initialized to 0 on reset.
+  Previously, its unused bit (bit 5) was set to 1 on reset.
+
+- Applied patch from Ed Spittles to change the CMP algorithm so that
+  it no longer fails Rob Finch's test suite.  Closes #8.
+
+- Added a new interactive assembly mode to the monitor.  Entering the
+  the assemble command with a statement such as "a c000 lda #0" works
+  as before.  Entering "a c000" will start the interactive assembler
+  at that address.  Entering "a" alone will start it at the current
+  program counter.
+
+- Applied patch from Ed Spittles so that SBC now properly sets the
+  Overflow (V) flag.  This fixes a failure in Rob Finch's test suite.
+  Closes #6.
+
+- Applied patch from Ed Spittles so that SBC now properly sets the
+  Carry (C) and Zero (Z) flags.  This fixes failures caught by Ed's
+  own tests (see http://forum.6502.org/viewtopic.php?p=8854#8854).
+  Closes #15.
 
-  - A new "save" command has been added to the monitor that will save
-    a range of memory to a binary file.
+- A new "save" command has been added to the monitor that will save
+  a range of memory to a binary file.
 
 0.6 (2009-08-11)
 ----------------
 
-  - Added monitor shortcut "a" for "assemble".
+- Added monitor shortcut "a" for "assemble".
 
-  - Fixed that ASL would not properly set the Z flag.  Closes #7.
+- Fixed that ASL would not properly set the Z flag.  Closes #7.
 
-  - Fixed that ADC would not properly set the Overflow (V) flag.  The
-    overflow calculation that is now used originated from XGS: Apple
-    IIGS Emulator (cputable.h).  Originally written and Copyright
-    (C)1996 by Joshua M. Thompson.  Copyright (C) 2006 by Samuel A.
-    Falvo II.  http://bitbucket.org/kc5tja/lib65816/src/tip/src/cputable.h
-    Closes #3.
+- Fixed that ADC would not properly set the Overflow (V) flag.  The
+  overflow calculation that is now used originated from XGS: Apple
+  IIGS Emulator (cputable.h).  Originally written and Copyright
+  (C)1996 by Joshua M. Thompson.  Copyright (C) 2006 by Samuel A.
+  Falvo II.  http://bitbucket.org/kc5tja/lib65816/src/tip/src/cputable.h
+  Closes #3.
 
 0.5 (2009-08-06)
 ----------------
 
-  - Fixed signatures of getc/putc callbacks in monitor that were broken
-    when the ObservableMemory interface changed in 0.3.  Closes #1.
+- Fixed signatures of getc/putc callbacks in monitor that were broken
+  when the ObservableMemory interface changed in 0.3.  Closes #1.
 
-  - Fixed that ROL would not properly set the Z flag.  Closes #2.
+- Fixed that ROL would not properly set the Z flag.  Closes #2.
 
 0.4 (2009-06-06)
 ----------------
 
-  - Added ez_setup.py to bootstrap setuptools installation.
+- Added ez_setup.py to bootstrap setuptools installation.
 
 0.3 (2009-06-03)
 ----------------
 
-  - Added shortcuts for monitor commands such as "m" for "memory".  These
-    are mostly the same as the VICE monitor shortcuts.
+- Added shortcuts for monitor commands such as "m" for "memory".  These
+  are mostly the same as the VICE monitor shortcuts.
 
-  - The terminal width can now be changed in the monitor using the new
-    "width" command.  Some commands, like "mem", will wrap to this width.
+- The terminal width can now be changed in the monitor using the new
+  "width" command.  Some commands, like "mem", will wrap to this width.
 
-  - Fixed a bug where BRK would increment PC by 3 instead of 2.  Thanks
-    to Oscar Lindberg.
+- Fixed a bug where BRK would increment PC by 3 instead of 2.  Thanks
+  to Oscar Lindberg.
 
-  - Added a new 65C02 MPU simulation started by Oscar Lindberg.  It is
-    now mostly complete.
+- Added a new 65C02 MPU simulation started by Oscar Lindberg.  It is
+  now mostly complete.
 
-  - Added a new "mpu" command to the monitor.  It will switch between the
-    NMOS 6502 and CMOS 65C02 simulations.
+- Added a new "mpu" command to the monitor.  It will switch between the
+  NMOS 6502 and CMOS 65C02 simulations.
 
-  - A new "devices" module has been added to organize device simulations.
+- A new "devices" module has been added to organize device simulations.
 
-  - The mpu6502 and mpu65c02 devices have been reorganized internally to
-    use Python decorators to build their lookup tables based on an
-    idea by Oscar Lindberg.
+- The mpu6502 and mpu65c02 devices have been reorganized internally to
+  use Python decorators to build their lookup tables based on an
+  idea by Oscar Lindberg.
 
-  - A new "utils" module has been added with various utility functions.
+- A new "utils" module has been added with various utility functions.
 
-  - The ObservableMemory interface has been changed for clarity.
+- The ObservableMemory interface has been changed for clarity.
 
-  - Python 2.4 or later is now required.
+- Python 2.4 or later is now required.
 
 0.2 (2008-11-09)
 ----------------
 
-  - Added a new "disassemble" command to the monitor.  It can disassemble
-    any range of memory ("disassemble c000:c010").  If labels have been
-    defined, the disassembly will show them in the operands.
+- Added a new "disassemble" command to the monitor.  It can disassemble
+  any range of memory ("disassemble c000:c010").  If labels have been
+  defined, the disassembly will show them in the operands.
 
-  - Added a new "assemble" command to the monitor.  It can assemble a
-    single instruction at an address ("assemble c000 jsr $ffd2").
-    Labels in the operands are also supported ("assemble c000 jsr charout").
+- Added a new "assemble" command to the monitor.  It can assemble a
+  single instruction at an address ("assemble c000 jsr $ffd2").
+  Labels in the operands are also supported ("assemble c000 jsr charout").
 
-  - Moved the character I/O area from $E000 to $F000 for compatibility with
-    the EhBASIC binary saved from Michal Kowalski's Windows-based simulator.
-    In a future version of Py65, the I/O area will be configurable.
+- Moved the character I/O area from $E000 to $F000 for compatibility with
+  the EhBASIC binary saved from Michal Kowalski's Windows-based simulator.
+  In a future version of Py65, the I/O area will be configurable.
 
-  - When running a program in the monitor, a read to $F004 will now do a
-    non-blocking read from STDIN.  If no character is available, a null
-    byte ($00) will be returned.
+- When running a program in the monitor, a read to $F004 will now do a
+  non-blocking read from STDIN.  If no character is available, a null
+  byte ($00) will be returned.
 
-  - Fixed a bug where a CMP instruction could crash the simulator due to
-    an undefined variable.
+- Fixed a bug where a CMP instruction could crash the simulator due to
+  an undefined variable.
 
-  - EhBASIC 2.09 now runs in the simulator!
+- EhBASIC 2.09 now runs in the simulator!
 
-  - Documented all remaining monitor commands.  In the monitor, use the
-    command "help command" for help on any command.
+- Documented all remaining monitor commands.  In the monitor, use the
+  command "help command" for help on any command.
 
 0.1 (2008-11-21)
 ----------------
 
-  - First release.
+- First release.
```

### Comparing `py65-1.1.0/setup.py` & `py65-1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 import sys
 
 py_version = sys.version_info[:2]
 PY3 = py_version[0] == 3
 
 if PY3:
-    if py_version < (3, 2):
-        raise RuntimeError('On Python 3, Py65 requires Python 3.2 or later')
+    if py_version < (3, 4):
+        raise RuntimeError('On Python 3, Py65 requires Python 3.4 or later')
 else:
-    if py_version < (2, 6):
-        raise RuntimeError('On Python 2, Py65 requires Python 2.6 or later')
+    if py_version < (2, 7):
+        raise RuntimeError('On Python 2, Py65 requires Python 2.7 or later')
 
 from setuptools import setup, find_packages
 
 DESC = """\
 Simulate 6502-based microcomputer systems in Python."""
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Operating System :: POSIX',
     'Programming Language :: Python',
     'Programming Language :: Python :: 2',
-    'Programming Language :: Python :: 2.6',
     'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.2',
-    'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Programming Language :: Assembly',
     'Topic :: Software Development :: Assemblers',
     'Topic :: Software Development :: Disassemblers',
     'Topic :: Software Development :: Debuggers',
     'Topic :: Software Development :: Embedded Systems',
     'Topic :: Software Development :: Interpreters',
     'Topic :: System :: Emulators',
```

### Comparing `py65-1.1.0/py65.egg-info/PKG-INFO` & `py65-1.2/py65.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: py65
-Version: 1.1.0
+Version: 1.2.0
 Summary: 6502 microprocessor simulation package
 Home-page: https://github.com/mnaberez/py65
 Author: Mike Naberezny
 Author-email: mike@naberezny.com
+Maintainer: Mike Naberezny
+Maintainer-email: mike@naberezny.com
 License: License :: OSI Approved :: BSD License
-Description-Content-Type: UNKNOWN
-Description: Simulate 6502-based microcomputer systems in Python.
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Assembly
 Classifier: Topic :: Software Development :: Assemblers
 Classifier: Topic :: Software Development :: Disassemblers
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Hardware
+License-File: LICENSE.txt
+
+Simulate 6502-based microcomputer systems in Python.
```

### Comparing `py65-1.1.0/py65.egg-info/SOURCES.txt` & `py65-1.2/py65.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CHANGES.txt
+CHANGES.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
@@ -11,28 +11,30 @@
 examples/65Org16.boot.rom
 examples/README.txt
 examples/ehbasic.bin
 examples/swapcase.asm
 examples/swapcase.hex
 py65/__init__.py
 py65/assembler.py
+py65/compat.py
 py65/disassembler.py
 py65/memory.py
 py65/monitor.py
 py65.egg-info/PKG-INFO
 py65.egg-info/SOURCES.txt
 py65.egg-info/dependency_links.txt
 py65.egg-info/entry_points.txt
 py65.egg-info/not-zip-safe
 py65.egg-info/top_level.txt
 py65/devices/__init__.py
 py65/devices/mpu6502.py
 py65/devices/mpu65c02.py
 py65/devices/mpu65org16.py
 py65/tests/__init__.py
+py65/tests/end_to_end.py
 py65/tests/test_assembler.py
 py65/tests/test_disassembler.py
 py65/tests/test_memory.py
 py65/tests/test_monitor.py
 py65/tests/devices/__init__.py
 py65/tests/devices/test_mpu6502.py
 py65/tests/devices/test_mpu65c02.py
```

### Comparing `py65-1.1.0/examples/swapcase.asm` & `py65-1.2/examples/swapcase.asm`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/examples/65Org16.boot.asm` & `py65-1.2/examples/65Org16.boot.asm`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/examples/65Org16.boot.rom` & `py65-1.2/examples/65Org16.boot.rom`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/examples/ehbasic.bin` & `py65-1.2/examples/ehbasic.bin`

 * *Files identical despite different names*

### Comparing `py65-1.1.0/README.rst` & `py65-1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,17 @@
   tests so unexpected results are minimized.
 
 Installation
 ------------
 
 Py65 packages are `available <http://pypi.python.org/pypi/py65>`_ on the
 Python Package Index (PyPI).  You download them from there or you can
-use ``pip`` to automatically install or upgrade Py65::
+use ``pip`` to install Py65::
 
-    $ pip install -U py65
+    $ pip install setuptools py65
 
 Devices
 -------
 
 The following devices are simulated at this time:
 
 - ``mpu6502`` simulates the original NMOS 6502 microprocessor from MOS
@@ -56,21 +56,14 @@
   the popular VICE emulator for Commodore computers.
 
 - Ability to load, dump, and fill memory.
 
 - Simple assemble and disassemble capability, including support for labels
   and labels with offsets.
 
-Documentation
--------------
-
-Py65 documentation is written using `Sphinx <http://sphinx.pocoo.org/>`_ and
-is published to `http://py65.readthedocs.org/
-<http://py65.readthedocs.org/>`_.
-
 Contributors
 ------------
 
 These people are responsible for Py65:
 
 - `Mike Naberezny <https://github.com/mnaberez>`_ is the original author of
   Py65 and is the primary maintainer.
```

### Comparing `py65-1.1.0/LICENSE.txt` & `py65-1.2/LICENSE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-Copyright (c) 2008-2014, Mike Naberezny and contributors.
+BSD 3-Clause License
+
+Copyright (c) 2008-2024, Mike Naberezny and contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-    * Redistributions of source code must retain the above copyright notice,
-      this list of conditions and the following disclaimer.
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in the
-      documentation and/or other materials provided with the distribution.
-    * Neither the name of Mike Naberezny nor the names of the contributors
-      may be used to endorse or promote products derived from this software
-      without specific prior written permission.
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
```

