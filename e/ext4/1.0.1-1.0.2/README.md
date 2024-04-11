# Comparing `tmp/ext4-1.0.1.tar.gz` & `tmp/ext4-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext4-1.0.1.tar", last modified: Thu Jan  4 07:30:39 2024, max compression
+gzip compressed data, was "ext4-1.0.2.tar", last modified: Thu Apr 11 22:19:49 2024, max compression
```

## Comparing `ext4-1.0.1.tar` & `ext4-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 07:30:39.491788 ext4-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-04 07:30:30.000000 ext4-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-04 07:30:39.491788 ext4-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-04 07:30:30.000000 ext4-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 07:30:39.487788 ext4-1.0.1/ext4/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/blockdescriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/htree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/inode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/superblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-01-04 07:30:30.000000 ext4-1.0.1/ext4/xattr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 07:30:39.487788 ext4-1.0.1/ext4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-04 07:30:39.000000 ext4-1.0.1/ext4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-04 07:30:39.000000 ext4-1.0.1/ext4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 07:30:39.000000 ext4-1.0.1/ext4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-04 07:30:39.000000 ext4-1.0.1/ext4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-04 07:30:39.000000 ext4-1.0.1/ext4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-04 07:30:30.000000 ext4-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-04 07:30:30.000000 ext4-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 07:30:39.491788 ext4-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 22:19:45.000000 ext4-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 22:19:49.406913 ext4-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 22:19:45.000000 ext4-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/ext4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/blockdescriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/htree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/inode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/superblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/xattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/ext4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-11 22:19:45.000000 ext4-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 22:19:45.000000 ext4-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:19:49.406913 ext4-1.0.2/setup.cfg
```

### Comparing `ext4-1.0.1/LICENSE` & `ext4-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/PKG-INFO` & `ext4-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ext4-1.0.1/ext4/__init__.py` & `ext4-1.0.2/ext4/__init__.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/block.py` & `ext4-1.0.2/ext4/block.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/blockdescriptor.py` & `ext4-1.0.2/ext4/blockdescriptor.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/directory.py` & `ext4-1.0.2/ext4/directory.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/enum.py` & `ext4-1.0.2/ext4/enum.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/extent.py` & `ext4-1.0.2/ext4/extent.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/htree.py` & `ext4-1.0.2/ext4/htree.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/inode.py` & `ext4-1.0.2/ext4/inode.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/struct.py` & `ext4-1.0.2/ext4/struct.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/superblock.py` & `ext4-1.0.2/ext4/superblock.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4/volume.py` & `ext4-1.0.2/ext4/volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         elif mode == io.SEEK_CUR:
             seek = self.cursor + offset
 
         elif mode == io.SEEK_END:
             seek = len(self) - offset
 
         if seek < 0:
-            raise OSError()
+            raise OSError(errno.EINVAL, os.strerror(errno.EINVAL))
 
         self.cursor = seek
         return self.cursor
 
     def read(self, size):
         self.stream.seek(self.offset + self.cursor)
         return self.stream.read(size)
@@ -202,15 +202,15 @@
         paths = list(self.path_tuple(path))
         cwd = self.root
         if not paths:
             return cwd
 
         while paths:
             if not isinstance(cwd, Directory):
-                raise OSError(errno.ENOTDIR)
+                raise OSError(errno.ENOTDIR, os.strerror(errno.ENOTDIR))
 
             name = paths.pop(0)
             inode = None
             for dirent, _ in cwd.opendir():
                 if dirent.name_bytes == name:
                     inode = self.inodes[dirent.inode]
                     break
```

### Comparing `ext4-1.0.1/ext4/xattr.py` & `ext4-1.0.2/ext4/xattr.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.1/ext4.egg-info/PKG-INFO` & `ext4-1.0.2/ext4.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `ext4-1.0.1/pyproject.toml` & `ext4-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ext4"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Library for read only interactions with an ext4 filesystem"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
```

