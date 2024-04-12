# Comparing `tmp/retried-7.0.0.tar.gz` & `tmp/retried-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-7.0.0.tar", last modified: Thu Apr 11 16:54:20 2024, max compression
+gzip compressed data, was "retried-7.1.0.tar", last modified: Fri Apr 12 20:04:43 2024, max compression
```

## Comparing `retried-7.0.0.tar` & `retried-7.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      102 2024-04-11 16:54:03.856699 retried-7.0.0/README.md
--rw-r--r--   0        0        0     1061 2024-04-11 16:54:20.036707 retried-7.0.0/pyproject.toml
--rw-r--r--   0        0        0      162 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/aretry.py
--rw-r--r--   0        0        0     3270 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/retry.py
--rw-r--r--   0        0        0        0 2024-04-11 16:54:03.856699 retried-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-04-11 16:54:03.856699 retried-7.0.0/tests/test_aretry.py
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-12 20:04:28.778867 retried-7.1.0/README.md
+-rw-r--r--   0        0        0     1061 2024-04-12 20:04:43.339006 retried-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2024-04-12 20:04:28.778867 retried-7.1.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-12 20:04:28.778867 retried-7.1.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-04-12 20:04:28.778867 retried-7.1.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     3287 2024-04-12 20:04:28.778867 retried-7.1.0/src/retried/retry.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:04:28.778867 retried-7.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-12 20:04:28.778867 retried-7.1.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.1.0/PKG-INFO
```

### Comparing `retried-7.0.0/pyproject.toml` & `retried-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retried"
-version = "7.0.0"
+version = "7.1.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
 dependencies = []
 
 [build-system]
 requires = [
```

### Comparing `retried-7.0.0/src/retried/aretry.py` & `retried-7.1.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-7.0.0/src/retried/retry.py` & `retried-7.1.0/src/retried/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     delays = cycle(delays)
     if first_delay is None:
         first_delay = next(delays)
     if not isinstance(logger, logging.Logger):
         logger = DummyLogger(logger)
 
     def _default_error_callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: FuncT):
-        log_prefix = f'tried {i} of {r}: {f.__code__.co_filename}:{f.__code__.co_firstlineno} {e!r}'
+        log_prefix = f'{f.__qualname__} tried {i} of {r}: {f.__code__.co_filename}:{f.__code__.co_firstlineno} {e!r}'
         is_last = i == r
         if not is_last:
             logger.info(f'{log_prefix} -> sleep {d} seconds')
         else:
             logger.warning(log_prefix)
 
     error_callback = error_callback or _default_error_callback
```

### Comparing `retried-7.0.0/tests/test_aretry.py` & `retried-7.1.0/tests/test_aretry.py`

 * *Files identical despite different names*

