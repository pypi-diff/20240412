# Comparing `tmp/remarkable_update_fuse-1.0.5.tar.gz` & `tmp/remarkable_update_fuse-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remarkable_update_fuse-1.0.5.tar", last modified: Thu Apr 11 18:31:10 2024, max compression
+gzip compressed data, was "remarkable_update_fuse-1.0.6.tar", last modified: Thu Apr 11 22:00:26 2024, max compression
```

## Comparing `remarkable_update_fuse-1.0.5.tar` & `remarkable_update_fuse-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:31:10.242525 remarkable_update_fuse-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 18:31:10.242525 remarkable_update_fuse-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:31:10.242525 remarkable_update_fuse-1.0.5/remarkable_update_fuse/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 18:31:04.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse/update_metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:31:10.242525 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 18:31:10.000000 remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 18:30:57.000000 remarkable_update_fuse-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:31:10.242525 remarkable_update_fuse-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:00:26.226717 remarkable_update_fuse-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 22:00:26.226717 remarkable_update_fuse-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:00:26.226717 remarkable_update_fuse-1.0.6/remarkable_update_fuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 22:00:19.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse/update_metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:00:26.226717 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 22:00:26.000000 remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:00:13.000000 remarkable_update_fuse-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:00:26.226717 remarkable_update_fuse-1.0.6/setup.cfg
```

### Comparing `remarkable_update_fuse-1.0.5/LICENSE` & `remarkable_update_fuse-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.5/PKG-INFO` & `remarkable_update_fuse-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.5
+Version: 1.0.6
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `remarkable_update_fuse-1.0.5/README.md` & `remarkable_update_fuse-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.5/pyproject.toml` & `remarkable_update_fuse-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "remarkable_update_fuse"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Userspace filesystem for remarkable update files"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse/fuse.py` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse/fuse.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,19 @@
 
         except UpdateImageSignatureException:
             warnings.warn("Signature doesn't match contents", RuntimeWarning)
 
         except FileNotFoundError:
             warnings.warn("Public key missing", RuntimeWarning)
 
+        except OSError as e:
+            if e.errno != errno.ENOTDIR:
+                raise
+            warnings.warn("Unable to open public key", RuntimeWarning)
+
         threads = self.start_cache_threads()
         fuse.Fuse.main(self, args)
         self.exit_threads = True
         _ = [t.kill() for t in threads]
         _ = [t.join() for t in threads]
 
     def start_cache_threads(self):
```

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse/image.py` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse/image.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse/threads.py` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse/threads.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse/update_metadata_pb2.py` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse/update_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/PKG-INFO` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.5
+Version: 1.0.6
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `remarkable_update_fuse-1.0.5/remarkable_update_fuse.egg-info/SOURCES.txt` & `remarkable_update_fuse-1.0.6/remarkable_update_fuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

