# Comparing `tmp/gmalglib-0.3.1.tar.gz` & `tmp/gmalglib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.3.1.tar", last modified: Sun Apr  7 12:11:40 2024, max compression
+gzip compressed data, was "gmalglib-0.4.0.tar", last modified: Fri Apr 12 13:01:22 2024, max compression
```

## Comparing `gmalglib-0.3.1.tar` & `gmalglib-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-07 12:11:30.000000 gmalglib-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 12:11:40.880397 gmalglib-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 12:11:30.000000 gmalglib-0.3.1/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 12:11:30.000000 gmalglib-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.872397 gmalglib-0.3.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-07 12:11:30.000000 gmalglib-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:11:40.880397 gmalglib-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-07 12:11:30.000000 gmalglib-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 13:01:16.000000 gmalglib-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 13:01:22.727690 gmalglib-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:01:16.000000 gmalglib-0.4.0/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:01:16.000000 gmalglib-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.719690 gmalglib-0.4.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.723690 gmalglib-0.4.0/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 13:01:16.000000 gmalglib-0.4.0/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 13:01:16.000000 gmalglib-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:01:22.727690 gmalglib-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 13:01:16.000000 gmalglib-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.719690 gmalglib-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.723690 gmalglib-0.4.0/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19150 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28068 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 13:01:16.000000 gmalglib-0.4.0/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:01:22.727690 gmalglib-0.4.0/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 13:01:22.000000 gmalglib-0.4.0/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.3.1/LICENSE` & `gmalglib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/PKG-INFO` & `gmalglib-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.3.1/include/gmalglib/sm3.h` & `gmalglib-0.4.0/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/pyproject.toml` & `gmalglib-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/src/gmalglib/core/sm3.c` & `gmalglib-0.4.0/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/src/gmalglib/core/sm4.c` & `gmalglib-0.4.0/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/src/gmalglib/core/zuc.c` & `gmalglib-0.4.0/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.3.1/src/gmalglib/sm3.pyi` & `gmalglib-0.4.0/src/gmalglib/sm3.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 SM3_MAX_MSG_BITLEN: int
 SM3_DIGEST_LENGTH: int
 
 
 class SM3:
-    """SM3 Algorithm."""
+    """SM3 算法对象."""
 
     def __init__(self, data: bytes = b"") -> None:
-        """SM3 Algorithm.
+        """SM3 算法对象.
 
         Args:
-            data: Initial data.
+            data: 初始化数据.
         """
 
     def update(self, data: bytes) -> None:
-        """Update state.
-
-        Args:
-            data: Bytes data.
-        """
+        """更新内部状态."""
 
     def digest(self) -> bytes:
-        """Get digest.
-
-        Returns:
-            digest: Digest in bytes.
-        """
+        """获取当前状态哈希值."""
 
     def reset(self) -> None:
-        """Reset internal state."""
+        """重置内部状态."""
 
     def copy(self) -> SM3:
-        """Copy a new SM3 object with identical state.
-
-        Returns:
-            sm3_obj: A new SM3 object.
-        """
+        """拷贝当前对象及其内部状态."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gmalglib-0.3.1/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.4.0/src/gmalglib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.3.1/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.4.0/src/gmalglib.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 LICENSE
 README.en.md
 README.md
 pyproject.toml
 setup.py
+include/gmalglib/bignum.h
+include/gmalglib/random.h
+include/gmalglib/sm2.h
+include/gmalglib/sm2curve.h
 include/gmalglib/sm3.h
 include/gmalglib/sm4.h
 include/gmalglib/zuc.h
 src/gmalglib/__init__.py
 src/gmalglib/coremodule.c
+src/gmalglib/sm2.py
+src/gmalglib/sm2.pyi
 src/gmalglib/sm3.py
 src/gmalglib/sm3.pyi
 src/gmalglib/sm4.py
 src/gmalglib/sm4.pyi
 src/gmalglib/zuc.py
 src/gmalglib/zuc.pyi
 src/gmalglib.egg-info/PKG-INFO
 src/gmalglib.egg-info/SOURCES.txt
 src/gmalglib.egg-info/dependency_links.txt
 src/gmalglib.egg-info/top_level.txt
+src/gmalglib/core/bignum.c
+src/gmalglib/core/random.c
+src/gmalglib/core/sm2.c
+src/gmalglib/core/sm2curve.c
 src/gmalglib/core/sm3.c
 src/gmalglib/core/sm4.c
 src/gmalglib/core/zuc.c
```

