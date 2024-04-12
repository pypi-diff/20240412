# Comparing `tmp/cs.buffer-20240316.tar.gz` & `tmp/cs.buffer-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.buffer-20240316.tar", last modified: Sat Mar 16 06:36:48 2024, max compression
+gzip compressed data, was "cs.buffer-20240412.tar", last modified: Fri Apr 12 05:09:25 2024, max compression
```

## Comparing `cs.buffer-20240316.tar` & `cs.buffer-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:36:48.692614 cs.buffer-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:36:22.000000 cs.buffer-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    12858 2024-03-16 06:36:48.692271 cs.buffer-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    26258 2024-03-16 06:36:31.000000 cs.buffer-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:36:48.686436 cs.buffer-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:36:48.686751 cs.buffer-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:36:48.689021 cs.buffer-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    45423 2024-03-16 06:36:09.000000 cs.buffer-20240316/lib/python/cs/buffer.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:36:48.691751 cs.buffer-20240316/lib/python/cs.buffer.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    12858 2024-03-16 06:36:48.000000 cs.buffer-20240316/lib/python/cs.buffer.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-03-16 06:36:48.000000 cs.buffer-20240316/lib/python/cs.buffer.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:36:48.000000 cs.buffer-20240316/lib/python/cs.buffer.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       57 2024-03-16 06:36:48.000000 cs.buffer-20240316/lib/python/cs.buffer.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:36:48.000000 cs.buffer-20240316/lib/python/cs.buffer.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    13247 2024-03-16 06:36:47.000000 cs.buffer-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:36:48.692719 cs.buffer-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:09:25.698275 cs.buffer-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:09:01.000000 cs.buffer-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    27194 2024-04-12 05:09:25.697986 cs.buffer-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26347 2024-04-12 05:09:09.000000 cs.buffer-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:09:25.693675 cs.buffer-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:09:25.693940 cs.buffer-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:09:25.695183 cs.buffer-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    45507 2024-04-12 05:08:32.000000 cs.buffer-20240412/lib/python/cs/buffer.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:09:25.697558 cs.buffer-20240412/lib/python/cs.buffer.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    27194 2024-04-12 05:09:25.000000 cs.buffer-20240412/lib/python/cs.buffer.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-12 05:09:25.000000 cs.buffer-20240412/lib/python/cs.buffer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:09:25.000000 cs.buffer-20240412/lib/python/cs.buffer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       57 2024-04-12 05:09:25.000000 cs.buffer-20240412/lib/python/cs.buffer.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:09:25.000000 cs.buffer-20240412/lib/python/cs.buffer.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    27591 2024-04-12 05:09:24.000000 cs.buffer-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:09:25.698377 cs.buffer-20240412/setup.cfg
```

### Comparing `cs.buffer-20240316/README.md` & `cs.buffer-20240412/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Facilities to do with buffers, particularly CornuCopyBuffer,
 an automatically refilling buffer to support parsing of data streams.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+CornuCopyBuffer.buf: return b"" if nothing is buffered.
 
 ## Class `CopyingIterator`
 
 Wrapper for an iterator that copies every item retrieved to a callable.
 
 *Method `CopyingIterator.__init__(self, it, copy_to)`*:
 Initialise with the iterator `it` and the callable `copy_to`.
@@ -212,15 +212,15 @@
 which does this automatically.
 
 Also, because the new buffer may buffer some of the unconsumed
 data from this buffer, use of the original buffer should
 be suspended.
 
 *Property `CornuCopyBuffer.buf`*:
-The first buffer.
+The first buffer, or `b''` if nothing is buffered.
 
 *Method `CornuCopyBuffer.byte0(self)`*:
 Consume the leading byte and return it as an `int` (`0`..`255`).
 
 *Method `CornuCopyBuffer.close(self)`*:
 Close the buffer.
 This calls the `close` callable supplied
@@ -527,26 +527,26 @@
 * `align`: whether to align reads by default: if true then
   the iterator will do a short read to bring the `offset`
   into alignment with `readsize`; the default is `False`
 
 *Method `FileIterator.close(self)`*:
 Detach from the file. Does *not* call `fp.close()`.
 
-## Class `SeekableFDIterator(FDIterator, _Iterator, SeekableIteratorMixin)`
+## Class `SeekableFDIterator(FDIterator, SeekableIteratorMixin)`
 
 An iterator over the data of a seekable file descriptor.
 
 *Note*: the iterator works with an `os.dup()` of the file
 descriptor so that it can close it with impunity; this requires
 the caller to close their descriptor.
 
 *Property `SeekableFDIterator.end_offset`*:
 The end offset of the file.
 
-## Class `SeekableFileIterator(FileIterator, _Iterator, SeekableIteratorMixin)`
+## Class `SeekableFileIterator(FileIterator)`
 
 An iterator over the data of a seekable file object.
 
 *Note*: the iterator closes the file on __del__ or if its
 .close method is called.
 
 *Method `SeekableFileIterator.__init__(self, fp, offset=None, **kw)`*:
@@ -600,14 +600,17 @@
 *Property `SeekableMMapIterator.end_offset`*:
 The end offset of the mmap memoryview.
 
 # Release Log
 
 
 
+*Release 20240412*:
+CornuCopyBuffer.buf: return b"" if nothing is buffered.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 CornuCopyBuffer: read1() method shorthand for read(..,one_fetch=True).
 
 *Release 20230401*:
```

### Comparing `cs.buffer-20240316/lib/python/cs/buffer.py` & `cs.buffer-20240412/lib/python/cs/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import sys
 from threading import Thread
 
 from cs.deco import Promotable
 from cs.gimmicks import r
 from cs.py3 import pread
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Development Status :: 5 - Production/Stable",
@@ -177,17 +177,20 @@
     ), msgpfx + ": self.buflen != sum of .bufs"
     assert all(
         len(buf) > 0 for buf in self.bufs
     ), msgpfx + ": not all .bufs are nonempty"
 
   @property
   def buf(self):
-    ''' The first buffer.
+    ''' The first buffer, or `b''` if nothing is buffered.
     '''
-    return self.bufs[0]
+    try:
+      return self.bufs[0]
+    except IndexError:
+      return b''
 
   def close(self):
     ''' Close the buffer.
         This calls the `close` callable supplied
         when the buffer was initialised, if any,
         in order to release resources such as open file descriptors.
         The callable will be called only on the first `close()` call.
```

