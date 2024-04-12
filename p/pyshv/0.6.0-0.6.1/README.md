# Comparing `tmp/pyshv-0.6.0.tar.gz` & `tmp/pyshv-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshv-0.6.0.tar", last modified: Sat Apr  6 19:04:33 2024, max compression
+gzip compressed data, was "pyshv-0.6.1.tar", last modified: Fri Apr 12 10:29:20 2024, max compression
```

## Comparing `pyshv-0.6.0.tar` & `pyshv-0.6.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.682715 pyshv-0.6.0/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1078 2023-10-11 09:25:34.000000 pyshv-0.6.0/LICENSE
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3776 2024-04-06 19:04:33.681715 pyshv-0.6.0/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1332 2024-04-06 18:44:22.000000 pyshv-0.6.0/README.rst
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3077 2024-04-06 18:44:22.000000 pyshv-0.6.0/pyproject.toml
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.681715 pyshv-0.6.0/pyshv.egg-info/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3776 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1080 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/SOURCES.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/dependency_links.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       93 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/entry_points.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      153 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/requires.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       14 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/top_level.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2024-04-06 19:04:33.682715 pyshv-0.6.0/setup.cfg
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.677715 pyshv-0.6.0/shv/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3919 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      782 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/__version__.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.677715 pyshv-0.6.0/shv/broker/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      162 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1829 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/__main__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    30962 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/broker.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12306 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/config.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14153 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/chainpack.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7573 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/commonpack.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.678715 pyshv-0.6.0/shv/cpconv/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      137 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2365 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/__main__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2100 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/cpconv.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    16319 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpon.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.6.0/shv/py.typed
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    13972 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4181 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcerrors.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5580 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpclogin.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14516 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcmessage.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6877 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcmethod.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5873 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcparams.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6118 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcprotocol.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    11841 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcserver.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5898 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcsubscription.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7318 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcurl.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      117 2023-10-11 09:25:34.000000 pyshv-0.6.0/shv/shvversion.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    19508 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simplebase.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8646 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simpleclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2637 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simpledevice.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      393 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/tools.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7912 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/value.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12299 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/valueclient.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.680715 pyshv-0.6.0/tests/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3321 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_chainpack.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      536 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_cpconv.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5066 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_cpon.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      387 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_crc32.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1012 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_errors.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5954 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_example.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6818 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1115 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcparam.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2423 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcsubscription.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4117 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcurl.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7424 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_simpleclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3034 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_simpledevice.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4744 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_value.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5647 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_valueclient.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.538310 pyshv-0.6.1/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1078 2023-10-11 09:25:34.000000 pyshv-0.6.1/LICENSE
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3784 2024-04-12 10:29:20.537310 pyshv-0.6.1/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1332 2024-04-06 20:23:20.000000 pyshv-0.6.1/README.rst
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3087 2024-04-12 10:23:34.000000 pyshv-0.6.1/pyproject.toml
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.536310 pyshv-0.6.1/pyshv.egg-info/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3784 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1080 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/SOURCES.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/dependency_links.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       93 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/entry_points.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      161 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/requires.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       14 2024-04-12 10:29:20.000000 pyshv-0.6.1/pyshv.egg-info/top_level.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2024-04-12 10:29:20.538310 pyshv-0.6.1/setup.cfg
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.532310 pyshv-0.6.1/shv/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3660 2024-04-09 12:10:30.000000 pyshv-0.6.1/shv/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      782 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/__version__.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.533310 pyshv-0.6.1/shv/broker/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      162 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/broker/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1829 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/broker/__main__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    30962 2024-04-09 12:03:13.000000 pyshv-0.6.1/shv/broker/broker.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12306 2024-04-09 08:59:24.000000 pyshv-0.6.1/shv/broker/config.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14153 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/chainpack.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7573 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/commonpack.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.533310 pyshv-0.6.1/shv/cpconv/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      137 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/cpconv/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2365 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/cpconv/__main__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2100 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/cpconv/cpconv.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    16319 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/cpon.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.6.1/shv/py.typed
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    13972 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4181 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcerrors.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5580 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpclogin.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14516 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcmessage.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7149 2024-04-12 10:20:39.000000 pyshv-0.6.1/shv/rpcmethod.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5873 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcparams.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6118 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcprotocol.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    11841 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcserver.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5951 2024-04-11 18:44:46.000000 pyshv-0.6.1/shv/rpcsubscription.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7318 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/rpcurl.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      117 2023-10-11 09:25:34.000000 pyshv-0.6.1/shv/shvversion.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    19534 2024-04-09 12:10:55.000000 pyshv-0.6.1/shv/simplebase.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8646 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/simpleclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2637 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/simpledevice.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      393 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/tools.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8564 2024-04-09 12:10:30.000000 pyshv-0.6.1/shv/value.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12299 2024-04-06 18:39:22.000000 pyshv-0.6.1/shv/valueclient.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-12 10:29:20.536310 pyshv-0.6.1/tests/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3321 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_chainpack.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      536 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_cpconv.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5066 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_cpon.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      387 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_crc32.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1012 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_errors.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5954 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_example.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6818 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_rpcclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1115 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_rpcparam.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2423 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_rpcsubscription.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4117 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_rpcurl.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7707 2024-04-11 18:44:46.000000 pyshv-0.6.1/tests/test_simpleclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3034 2024-04-06 18:39:22.000000 pyshv-0.6.1/tests/test_simpledevice.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5522 2024-04-09 12:10:30.000000 pyshv-0.6.1/tests/test_value.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5562 2024-04-11 18:44:46.000000 pyshv-0.6.1/tests/test_valueclient.py
```

### Comparing `pyshv-0.6.0/LICENSE` & `pyshv-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/PKG-INFO` & `pyshv-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 License: MIT License
         
         Copyright (c) 2022-2023 Elektroline a.s.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: aioserial
 Requires-Dist: asyncinotify; sys_platform == "linux"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-multiversion; extra == "docs"
 
 ============================================
```

### Comparing `pyshv-0.6.0/README.rst` & `pyshv-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/pyproject.toml` & `pyshv-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyshv"
-version = "0.6.0"
+version = "0.6.1"
 description = "Pure Python SHV implementation"
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
@@ -29,15 +29,15 @@
 "Homepage" = "https://gitlab.com/silicon-heaven/pyshv"
 "Bug Tracker" = "https://gitlab.com/silicon-heaven/pyshv/-/issues"
 "Github" = "https://github.com/silicon-heaven/libshv-py"
 
 [project.optional-dependencies]
 test = [
   "pytest",
-  "pytest-asyncio",
+  "pytest-asyncio == 0.21.1",
   "pytest-cov",
 ]
 docs = [
   "sphinx",
   "sphinx_rtd_theme",
   "sphinx-multiversion",
 ]
```

### Comparing `pyshv-0.6.0/pyshv.egg-info/PKG-INFO` & `pyshv-0.6.1/pyshv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.6.0
+Version: 0.6.1
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 License: MIT License
         
         Copyright (c) 2022-2023 Elektroline a.s.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: aioserial
 Requires-Dist: asyncinotify; sys_platform == "linux"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-multiversion; extra == "docs"
 
 ============================================
```

### Comparing `pyshv-0.6.0/pyshv.egg-info/SOURCES.txt` & `pyshv-0.6.1/pyshv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/__init__.py` & `pyshv-0.6.1/shv/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,72 +71,63 @@
     SHVType,
     SHVUInt,
     decimal_rexp,
     is_shvbool,
     is_shvimap,
     is_shvmap,
     is_shvnull,
+    is_shvtype,
     shvmeta,
     shvmeta_eq,
 )
 from .valueclient import ValueClient
 
 __all__ = [
-    # shvversion
     "SHV_VERSION_MAJOR",
     "SHV_VERSION_MINOR",
     "VERSION",
-    # chainpack
     "ChainPack",
     "ChainPackReader",
     "ChainPackWriter",
-    # cpon
     "Cpon",
     "CponReader",
     "CponWriter",
     "DefaultRpcSubscription",
     "RpcClient",
     "RpcClientPipe",
     "RpcClientTCP",
     "RpcClientTTY",
     "RpcClientUnix",
     "RpcError",
-    # rpcerror
     "RpcErrorCode",
     "RpcInternalError",
     "RpcInvalidParamsError",
     "RpcInvalidRequestError",
-    # rpclogin
     "RpcLogin",
     "RpcLoginRequiredError",
     "RpcLoginType",
     "RpcLoginType",
-    # rpcmessage
     "RpcMessage",
     "RpcMethodAccess",
     "RpcMethodCallCancelledError",
     "RpcMethodCallExceptionError",
     "RpcMethodCallTimeoutError",
     "RpcMethodDesc",
-    # rpcmethod
     "RpcMethodFlags",
     "RpcMethodNotFoundError",
     "RpcParseError",
-    # rpcurl
     "RpcProtocol",
     "RpcProtocolSerial",
     "RpcProtocolSerialCRC",
     "RpcProtocolStream",
     "RpcServer",
     "RpcServerTCP",
     "RpcServerTTY",
     "RpcServerUnix",
-    # rpcsubscription
     "RpcSubscription",
-    # rpcprotocol
     "RpcTransportProtocol",
     "RpcUrl",
     "RpcUserIDRequiredError",
     "SHVBool",
     "SHVBoolType",
     "SHVBytes",
     "SHVDatetime",
@@ -146,42 +137,35 @@
     "SHVIMap",
     "SHVIMapType",
     "SHVInt",
     "SHVList",
     "SHVListType",
     "SHVMap",
     "SHVMapType",
-    # value
     "SHVMeta",
     "SHVMetaType",
     "SHVNull",
     "SHVNullType",
     "SHVStr",
     "SHVType",
     "SHVUInt",
-    # simplebase
     "SimpleBase",
-    # simpleclient
     "SimpleClient",
-    # simpledevice
     "SimpleDevice",
-    # valueclient
     "ValueClient",
     "connect_rpc_client",
-    # rpcserver
     "create_rpc_server",
     "decimal_rexp",
-    # rpcclient
     "init_rpc_client",
     "is_shvbool",
     "is_shvimap",
     "is_shvmap",
     "is_shvnull",
+    "is_shvtype",
     "shvarg",
     "shvargt",
     "shvget",
     "shvgett",
     "shvmeta",
     "shvmeta_eq",
-    # rpcparams
     "shvt",
 ]
```

### Comparing `pyshv-0.6.0/shv/__version__.py` & `pyshv-0.6.1/shv/__version__.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/broker/__main__.py` & `pyshv-0.6.1/shv/broker/__main__.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/broker/broker.py` & `pyshv-0.6.1/shv/broker/broker.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/broker/config.py` & `pyshv-0.6.1/shv/broker/config.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/chainpack.py` & `pyshv-0.6.1/shv/chainpack.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/commonpack.py` & `pyshv-0.6.1/shv/commonpack.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/cpconv/__main__.py` & `pyshv-0.6.1/shv/cpconv/__main__.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/cpconv/cpconv.py` & `pyshv-0.6.1/shv/cpconv/cpconv.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/cpon.py` & `pyshv-0.6.1/shv/cpon.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcclient.py` & `pyshv-0.6.1/shv/rpcclient.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcerrors.py` & `pyshv-0.6.1/shv/rpcerrors.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpclogin.py` & `pyshv-0.6.1/shv/rpclogin.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcmessage.py` & `pyshv-0.6.1/shv/rpcmessage.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcmethod.py` & `pyshv-0.6.1/shv/rpcmethod.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,18 +71,22 @@
 @dataclasses.dataclass
 class RpcMethodDesc:
     """Description of the SHV RPC method.
 
     This is implemented as :func:`dataclasses.dataclass`.
 
     :param name: Name of the method.
-    :param signature: Calling signature for this method.
     :param flags: Flags assigned to the method.
+    :param param: Parameter type that should be provided to the method.
+    :param result: Result type that is provided by the method.
     :param access: Minimal granted access level for this method.
-    :param description: Short description of the method.
+    :param signals: Mapping of signal name to data type they cary. These are
+      signals emited by this method.
+    :param extra: Additional fields to be provied in some cases. The most common
+      one is ``"description"`` with method description.
     """
 
     class Key(enum.IntEnum):
         """Key in the description IMap."""
 
         NAME = 1
         FLAGS = 2
```

### Comparing `pyshv-0.6.0/shv/rpcparams.py` & `pyshv-0.6.1/shv/rpcparams.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcprotocol.py` & `pyshv-0.6.1/shv/rpcprotocol.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcserver.py` & `pyshv-0.6.1/shv/rpcserver.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/rpcsubscription.py` & `pyshv-0.6.1/shv/rpcsubscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,18 @@
         res: dict[str, SHVType] = {}
         if compatible:
             pth, _, tail = self.paths.rpartition("/")
             if "*" in pth or tail != "**":
                 res["paths"] = self.paths
             else:
                 res["path"] = pth
-            if "*" in self.signal:
+            if "*" in self.signal and self.signal != "*":
                 res["methods"] = self.signal
             else:
-                res["method"] = self.signal
+                res["method"] = "" if self.signal == "*" else self.signal
         else:
             if self.paths != "**":
                 res["paths"] = self.paths
             if self.signal != "*":
                 res["signal"] = self.signal
         if self.source != "*":
             res["source"] = self.source
```

### Comparing `pyshv-0.6.0/shv/rpcurl.py` & `pyshv-0.6.1/shv/rpcurl.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/simplebase.py` & `pyshv-0.6.1/shv/simplebase.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,17 @@
                     tasks.add(asyncio.create_task(self._message(msg)))
                 else:
                     logger.info("%s: Dropped invalid message: %s", self.client, msg)
                 # Drop finished tasks
                 done = {t for t in tasks if t.done()}
                 self.__task_done(done)
                 tasks -= done
-        done, _ = await asyncio.wait(tasks)
-        self.__task_done(done)
+        if tasks:
+            done, _ = await asyncio.wait(tasks)
+            self.__task_done(done)
 
     def __task_done(self, tasks: collections.abc.Iterable[asyncio.Task]) -> None:
         for task in tasks:
             if exc := task.exception():
                 logger.info("%s: Message handlig failed", self.client, exc_info=exc)
 
     def _reset(self) -> None:
```

### Comparing `pyshv-0.6.0/shv/simpleclient.py` & `pyshv-0.6.1/shv/simpleclient.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/simpledevice.py` & `pyshv-0.6.1/shv/simpledevice.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/shv/value.py` & `pyshv-0.6.1/shv/value.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,19 +230,40 @@
     """Dictionary with :class:`SHVMeta`."""
 
 
 class SHVIMap(dict[int, SHVType], SHVMeta):
     """Dictionary with :class:`SHVMeta`."""
 
 
+def is_shvlist(value: object) -> typing.TypeGuard[SHVListType]:
+    """Check if given value can be SHV List."""
+    return isinstance(value, collections.abc.Sequence) and all(
+        is_shvtype(v) for v in value
+    )
+
+
 def is_shvmap(value: object) -> typing.TypeGuard[SHVMapType]:
     """Check if given value can be SHV Map."""
     return isinstance(value, collections.abc.Mapping) and all(
-        isinstance(k, str) for k in value.keys()
+        isinstance(k, str) and is_shvtype(v) for k, v in value.items()
     )
 
 
 def is_shvimap(value: object) -> typing.TypeGuard[SHVIMapType]:
     """Check if given value can be SHV IMap."""
     return isinstance(value, collections.abc.Mapping) and all(
-        isinstance(k, int) for k in value.keys()
+        isinstance(k, int) and is_shvtype(v) for k, v in value.items()
+    )
+
+
+def is_shvtype(value: object) -> typing.TypeGuard[SHVType]:
+    """Validate type of the value as SHVType."""
+    return (
+        is_shvnull(value)
+        or is_shvbool(value)
+        or isinstance(
+            value, int | float | decimal.Decimal | bytes | str | datetime.datetime
+        )
+        or is_shvlist(value)
+        or is_shvimap(value)
+        or is_shvmap(value)
     )
```

### Comparing `pyshv-0.6.0/shv/valueclient.py` & `pyshv-0.6.1/shv/valueclient.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_chainpack.py` & `pyshv-0.6.1/tests/test_chainpack.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_cpconv.py` & `pyshv-0.6.1/tests/test_cpconv.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_cpon.py` & `pyshv-0.6.1/tests/test_cpon.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_errors.py` & `pyshv-0.6.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_example.py` & `pyshv-0.6.1/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_rpcclient.py` & `pyshv-0.6.1/tests/test_rpcclient.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_rpcparam.py` & `pyshv-0.6.1/tests/test_rpcparam.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_rpcsubscription.py` & `pyshv-0.6.1/tests/test_rpcsubscription.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_rpcurl.py` & `pyshv-0.6.1/tests/test_rpcurl.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_simpleclient.py` & `pyshv-0.6.1/tests/test_simpleclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pytest
 
 from shv import (
     RpcLoginType,
     RpcMessage,
     RpcMethodAccess,
     RpcMethodDesc,
+    RpcMethodFlags,
     SimpleClient,
     shvmeta,
 )
 
 
 @pytest.mark.parametrize(
     "path,method,params,result",
@@ -23,22 +24,24 @@
         (
             "",
             "dir",
             None,
             [
                 {
                     1: "dir",
+                    2: 0,
                     3: "DirParam",
                     4: "DirResult",
                     5: 1,
                     6: {},
                     7: {"description": "", "label": ""},
                 },
                 {
                     1: "ls",
+                    2: 0,
                     3: "LsParam",
                     4: "LsResult",
                     5: 1,
                     6: {},
                     7: {"description": "", "label": ""},
                 },
             ],
@@ -94,91 +97,95 @@
         (
             ".broker/currentClient",
             [
                 RpcMethodDesc("dir", param="DirParam", result="DirResult"),
                 RpcMethodDesc("ls", param="LsParam", result="LsResult"),
                 RpcMethodDesc(
                     name="clientId",
-                    param="void",
-                    result="ret",
+                    param="Null",
+                    result="Int",
                     access=RpcMethodAccess.READ,
                     signals={},
                     extra={},
                 ),
                 RpcMethodDesc(
                     name="mountPoint",
-                    param="void",
-                    result="ret",
+                    param="Null",
+                    result="String",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="userRoles",
-                    param="void",
-                    result="ret",
+                    param="Null",
+                    result="List",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="userProfile",
-                    param="void",
-                    result="ret",
+                    param="Null",
+                    result="RpcValue",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="accessGrantForMethodCall",
-                    param="param",
-                    result="ret",
+                    param="List",
+                    result="String",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="accessLevelForMethodCall",
-                    param="param",
-                    result="ret",
+                    param="List",
+                    result="Int",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="accesLevelForMethodCall",
-                    param="param",
-                    result="ret",
+                    param="List",
+                    result="Int",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     name="changePassword",
-                    param="param",
-                    result="ret",
+                    param="List",
+                    result="Bool",
                     access=RpcMethodAccess.WRITE,
                 ),
             ],
         ),
         (
             ".broker/app/log",
             [
                 RpcMethodDesc("dir", param="DirParam", result="DirResult"),
                 RpcMethodDesc("ls", param="LsParam", result="LsResult"),
                 RpcMethodDesc(
                     "getSendLogAsSignalEnabled",
-                    param="void",
-                    result="ret",
+                    flags=RpcMethodFlags.GETTER,
+                    param="Null",
+                    result="Bool",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     "setSendLogAsSignalEnabled",
-                    param="param",
-                    result="ret",
+                    flags=RpcMethodFlags.SETTER,
+                    param="Bool",
+                    result="Bool",
                     access=RpcMethodAccess.WRITE,
                 ),
                 RpcMethodDesc(
                     "verbosity",
-                    param="void",
-                    result="ret",
+                    flags=RpcMethodFlags.GETTER,
+                    param="Null",
+                    result="String",
                     access=RpcMethodAccess.READ,
                 ),
                 RpcMethodDesc(
                     "setVerbosity",
-                    param="ret",
-                    result="param",
+                    flags=RpcMethodFlags.SETTER,
+                    param="Bool",
+                    result="String",
                     access=RpcMethodAccess.COMMAND,
                 ),
             ],
         ),
     ),
 )
 async def test_dir(client, path, result):
```

### Comparing `pyshv-0.6.0/tests/test_simpledevice.py` & `pyshv-0.6.1/tests/test_simpledevice.py`

 * *Files identical despite different names*

### Comparing `pyshv-0.6.0/tests/test_value.py` & `pyshv-0.6.1/tests/test_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     SHVMap,
     SHVMeta,
     SHVNull,
     SHVStr,
     SHVUInt,
     is_shvbool,
     is_shvnull,
+    is_shvtype,
     shvmeta_eq,
 )
 
 CLASSES: list = [
     (SHVNull, []),
     (SHVBool, [True]),
     (SHVInt, []),
@@ -170,14 +171,42 @@
         (0, False),
     ),
 )
 def test_is_shvbool(value, expected):
     assert is_shvbool(value) is expected
 
 
+@pytest.mark.parametrize(
+    "value,expected",
+    (
+        (None, True),
+        (SHVNull(), True),
+        (True, True),
+        (False, True),
+        (SHVBool(True), True),
+        (SHVBool(False), True),
+        (42, True),
+        (0.42, True),
+        (decimal.Decimal("0.42"), True),
+        (b"foo", True),
+        ("foo", True),
+        (datetime.datetime.now(), True),
+        ([4, 2], True),
+        (["foo", datetime.datetime.now(), None, False], True),
+        ({10: 4, 1: 2}, True),
+        ({"tenth": 4, "cent": 2}, True),
+        ({10: 4, "cent": 2}, False),
+        ([{10: 4, 1: [2, 0]}, {"tenth": 4, "cent": 2}], True),
+        (datetime.UTC, False),
+    ),
+)
+def test_is_shvtype(value, expected):
+    assert is_shvtype(value) is expected
+
+
 @pytest.mark.parametrize("cls,args", CLASSES)
 def test_meta_eq(cls, args):
     """meta_eq should compare metas to each other."""
     obj1 = cls(*args)
     obj2 = cls(*args)
     assert shvmeta_eq(obj1, obj2)
     meta = {"foo": 42}
```

### Comparing `pyshv-0.6.0/tests/test_valueclient.py` & `pyshv-0.6.1/tests/test_valueclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     """Check get_snapshot without arguments."""
     await value_client.subscribe(RpcSubscription("test/device/**"))
     await value_client.get_snapshot()
     assert "test/device/track/1" in value_client
     assert len(value_client) == 8
 
 
-@pytest.mark.xfail(reason="libshv doesn't support subscribe to fixed path for now.")
 async def test_get_snapshot_lower_subscribe(value_client, example_device):
     """Check that get_snapshot caches only subscribed paths."""
     await value_client.subscribe(RpcSubscription("test/device/track/2"))
     await value_client.get_snapshot("test")
     assert len(value_client) == 1
     assert "test/device/track/2" in value_client
```

