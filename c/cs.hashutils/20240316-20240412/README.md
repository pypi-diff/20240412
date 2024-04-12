# Comparing `tmp/cs.hashutils-20240316.tar.gz` & `tmp/cs.hashutils-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.hashutils-20240316.tar", last modified: Sat Mar 16 06:59:47 2024, max compression
+gzip compressed data, was "cs.hashutils-20240412.tar", last modified: Fri Apr 12 05:20:06 2024, max compression
```

## Comparing `cs.hashutils-20240316.tar` & `cs.hashutils-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:47.073861 cs.hashutils-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:59:43.000000 cs.hashutils-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     1570 2024-03-16 06:59:47.073496 cs.hashutils-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     2435 2024-03-16 06:59:44.000000 cs.hashutils-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:47.068274 cs.hashutils-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:47.068564 cs.hashutils-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:47.070629 cs.hashutils-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)     6212 2024-03-16 06:59:34.000000 cs.hashutils-20240316/lib/python/cs/hashutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:59:47.072980 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     1570 2024-03-16 06:59:46.000000 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-03-16 06:59:47.000000 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:59:46.000000 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:59:46.000000 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:59:46.000000 cs.hashutils-20240316/lib/python/cs.hashutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     1932 2024-03-16 06:59:45.000000 cs.hashutils-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:59:47.073983 cs.hashutils-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:20:06.297880 cs.hashutils-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:20:02.000000 cs.hashutils-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3731 2024-04-12 05:20:06.297623 cs.hashutils-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2993 2024-04-12 05:20:03.000000 cs.hashutils-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:20:06.294229 cs.hashutils-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:20:06.294506 cs.hashutils-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:20:06.295687 cs.hashutils-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)     6970 2024-04-12 05:19:46.000000 cs.hashutils-20240412/lib/python/cs/hashutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:20:06.297218 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3731 2024-04-12 05:20:05.000000 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-12 05:20:06.000000 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:20:05.000000 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       55 2024-04-12 05:20:06.000000 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:20:06.000000 cs.hashutils-20240412/lib/python/cs.hashutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4117 2024-04-12 05:20:04.000000 cs.hashutils-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:20:06.297975 cs.hashutils-20240412/setup.cfg
```

### Comparing `cs.hashutils-20240316/README.md` & `cs.hashutils-20240412/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Convenience hashing facilities.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+* BaseHashCode.hashclass(hashname): fall back to looking for blake3 from the blake3 module.
+* BaseHashCode: new get_hashfunc(hashname) static method.
 
 ## Class `BaseHashCode(builtins.bytes)`
 
 Base class for hashcodes, subclassed by `SHA1`, `SHA256` et al.
 
+You can obtain the class for a particular hasher by name, example:
+
+    SHA256 = BaseHashCode.hashclass('sha256')
+
+*Method `BaseHashCode.__str__(self)`*:
+Return `f'{self.hashname}:{self.hex()}'`.
+
 *Method `BaseHashCode.from_buffer(bfr: cs.buffer.CornuCopyBuffer)`*:
 Compute hashcode from the contents of the `CornuCopyBuffer` `bfr`.
 
 *Method `BaseHashCode.from_data(bs)`*:
 Compute hashcode from the data `bs`.
 
 *Method `BaseHashCode.from_fspath(fspath, **kw)`*:
@@ -28,14 +36,17 @@
 from the hash type name and the hash bytes hex text.
 
 *Method `BaseHashCode.from_prefixed_hashbytes_hex(hashtext: str)`*:
 Factory function returning a `BaseHashCode` object
 from the hash bytes hex text prefixed by the hashname.
 This is the reverse of `__str__`.
 
+*Method `BaseHashCode.get_hashfunc(hashname: str)`*:
+Fetch the hash function implied by `hashname`.
+
 *Method `BaseHashCode.hashclass(hashname: str, hashfunc=None, **kw)`*:
 Return the class for the hash function named `hashname`.
 
 Parameters:
 * `hashname`: the name of the hash function
 * `hashfunc`: optional hash function for the class
 
@@ -44,52 +55,56 @@
 
 *Method `BaseHashCode.hex(self) -> str`*:
 Return the hashcode bytes transcribes as a hexadecimal ASCII `str`.
 
 *Method `BaseHashCode.promote(obj)`*:
 Promote to a `BaseHashCode` instance.
 
-## Class `MD5(BaseHashCode, builtins.bytes)`
+## Class `MD5(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'md5' algorithm.
 
 *`MD5.hashfunc`*
 
-## Class `SHA1(BaseHashCode, builtins.bytes)`
+## Class `SHA1(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'sha1' algorithm.
 
 *`SHA1.hashfunc`*
 
-## Class `SHA224(BaseHashCode, builtins.bytes)`
+## Class `SHA224(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'sha224' algorithm.
 
 *`SHA224.hashfunc`*
 
-## Class `SHA256(BaseHashCode, builtins.bytes)`
+## Class `SHA256(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'sha256' algorithm.
 
 *`SHA256.hashfunc`*
 
-## Class `SHA384(BaseHashCode, builtins.bytes)`
+## Class `SHA384(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'sha384' algorithm.
 
 *`SHA384.hashfunc`*
 
-## Class `SHA512(BaseHashCode, builtins.bytes)`
+## Class `SHA512(BaseHashCode)`
 
-Hash class implementation.
+Hash class for the 'sha512' algorithm.
 
 *`SHA512.hashfunc`*
 
 # Release Log
 
 
 
+*Release 20240412*:
+* BaseHashCode.hashclass(hashname): fall back to looking for blake3 from the blake3 module.
+* BaseHashCode: new get_hashfunc(hashname) static method.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240211*:
 Initial PyPI release: BaseHashCode(bytes) and subclasses for various hash algorithms.
```

### Comparing `cs.hashutils-20240316/lib/python/cs/hashutils.py` & `cs.hashutils-20240412/lib/python/cs/hashutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,106 +3,129 @@
 ''' Convenience hashing facilities.
 '''
 
 from binascii import hexlify, unhexlify
 import hashlib
 import mmap
 import os
+from typing import Optional
 
 from cs.buffer import CornuCopyBuffer
 from cs.deco import promote
+from cs.lex import r
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.buffer',
         'cs.deco',
+        'cs.lex',
     ],
 }
 
 class BaseHashCode(bytes):
   ''' Base class for hashcodes, subclassed by `SHA1`, `SHA256` et al.
+
+      You can obtain the class for a particular hasher by name, example:
+
+          SHA256 = BaseHashCode.hashclass('sha256')
   '''
 
   __slots__ = ()
 
   # registry of classes
   by_hashname = {}
 
+  @staticmethod
+  def get_hashfunc(hashname: str):
+    ''' Fetch the hash function implied by `hashname`.
+    '''
+    try:
+      hashfunc = getattr(hashlib, hashname)
+    except AttributeError:
+      if hashname == 'blake3':
+        # see if the blake3 module is around
+        # pylint:disable=import-outside-toplevel
+        from blake3 import blake3 as hashfunc
+      else:
+        raise
+    return hashfunc
+
   @classmethod
   def hashclass(cls, hashname: str, hashfunc=None, **kw):
     ''' Return the class for the hash function named `hashname`.
 
         Parameters:
         * `hashname`: the name of the hash function
         * `hashfunc`: optional hash function for the class
     '''
     try:
       hashcls = cls.by_hashname[hashname]
     except KeyError:
-
       if hashfunc is None:
-        hashfunc = getattr(hashlib, hashname)
+        hashfunc = cls.get_hashfunc(hashname)
 
       class hashcls(
           cls,
-          hashfunc=getattr(hashlib, hashname),
+          hashfunc=hashfunc,
           hashname=hashname,
           **kw,
       ):
         ''' Hash class implementation.
         '''
         __slots__ = ()
 
       hashcls.__name__ = hashname.upper()
+      hashcls.__doc__ = f'Hash class for the {hashname!r} algorithm.'
     else:
       if hashfunc is not None:
         if hashfunc is not hashcls.hashfunc:
           raise ValueError(
               f'class {hashcls.__name__} already exists with a different hash function {hashcls.hashfunc} from supplied {hashfunc=}'
           )
 
     return hashcls
 
   @classmethod
   def __init_subclass__(
-      cls, *, hashfunc, hashname=None, by_hashname=None, **kw
+      cls, *, hashname: Optional[str] = None, hashfunc=None, **kw
   ):
     super().__init_subclass__(**kw)
-    if hashname is None:
+    if hashname is None and hashfunc is None:
+      # we're a superclass of another base class
       return
-    if by_hashname is None:
-      by_hashname = cls.by_hashname
+    if hashfunc is None:
+      hashfunc = cls.get_hashfunc(hashname)
+    by_hashname = cls.by_hashname
     try:
       hashcls = by_hashname[hashname]
     except KeyError:
-      hashcls = None
+      # new hash class, register it
+      by_hashname[hashname] = cls
     else:
-      if hashcls is not cls:
-        raise ValueError(
-            f'class {hashcls} already exists for hashname {hashname!r}'
-        )
+      raise ValueError(
+          f'hashname {hashname!r}: class {hashcls} already exists for hashname'
+      )
     cls.hashname = hashname
     cls.hashfunc = hashfunc
     cls.hashlen = len(hashfunc(b'').digest())
     if not cls.__doc__:
       cls.__doc__ = f'{hashfunc.__name__} hashcode class, subclass of `bytes`.'
-    if hashcls is None:
-      # new hash class, register it
-      by_hashname[hashname] = cls
 
   hashfunc = lambda bs=None: None  # pylint: disable=unnecessary-lambda-assignment
 
   def __str__(self):
+    ''' Return `f'{self.hashname}:{self.hex()}'`.
+    '''
     return f'{self.hashname}:{self.hex()}'
 
   @property
   def hashname(self):
     ''' The hash code type name, derived from the class name.
     '''
     return self.__class__.__name__.lower()
```

