# Comparing `tmp/sortedintersect-0.2.0.tar.gz` & `tmp/sortedintersect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sortedintersect-0.2.0.tar", last modified: Thu Feb 10 13:30:28 2022, max compression
+gzip compressed data, was "sortedintersect-0.4.0.tar", last modified: Fri Apr 12 15:59:41 2024, max compression
```

## Comparing `sortedintersect-0.2.0.tar` & `sortedintersect-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-02-10 13:30:28.360339 sortedintersect-0.2.0/
--rw-r--r--   0 kezcleal   (501) staff       (20)       42 2022-02-09 10:08:24.000000 sortedintersect-0.2.0/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)     4095 2022-02-10 13:30:28.359980 sortedintersect-0.2.0/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)     2902 2022-02-10 13:30:01.000000 sortedintersect-0.2.0/README.rst
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2022-02-10 13:30:28.360448 sortedintersect-0.2.0/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      817 2022-02-10 13:30:16.000000 sortedintersect-0.2.0/setup.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-02-10 13:30:28.356372 sortedintersect-0.2.0/sortedintersect/
--rw-r--r--   0 kezcleal   (501) staff       (20)       41 2022-02-10 12:24:12.000000 sortedintersect-0.2.0/sortedintersect/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)   331880 2022-02-10 12:37:18.000000 sortedintersect-0.2.0/sortedintersect/intersect.cpp
--rw-r--r--   0 kezcleal   (501) staff       (20)     4712 2022-02-10 12:37:16.000000 sortedintersect-0.2.0/sortedintersect/intersect.pyx
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-02-10 13:30:28.357922 sortedintersect-0.2.0/sortedintersect.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)     4095 2022-02-10 13:30:28.000000 sortedintersect-0.2.0/sortedintersect.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      400 2022-02-10 13:30:28.000000 sortedintersect-0.2.0/sortedintersect.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2022-02-10 13:30:28.000000 sortedintersect-0.2.0/sortedintersect.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        7 2022-02-10 13:30:28.000000 sortedintersect-0.2.0/sortedintersect.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       22 2022-02-10 13:30:28.000000 sortedintersect-0.2.0/sortedintersect.egg-info/top_level.txt
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-02-10 13:30:28.359521 sortedintersect-0.2.0/tests/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2022-02-09 10:05:55.000000 sortedintersect-0.2.0/tests/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    43049 2022-02-10 13:14:11.000000 sortedintersect-0.2.0/tests/benchmark.png
--rw-r--r--   0 kezcleal   (501) staff       (20)     2054 2022-02-10 13:09:53.000000 sortedintersect-0.2.0/tests/benchmark.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     2651 2022-02-10 12:23:50.000000 sortedintersect-0.2.0/tests/test_sortedintersect.py
+drwxr-xr-x   0 sbi8kc2    (502) staff       (20)        0 2024-04-12 15:59:41.406294 sortedintersect-0.4.0/
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     1069 2024-04-10 09:12:44.000000 sortedintersect-0.4.0/LICENSE.md
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)       42 2024-04-10 09:12:44.000000 sortedintersect-0.4.0/MANIFEST.in
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)      228 2024-04-12 15:59:41.404821 sortedintersect-0.4.0/PKG-INFO
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     4471 2024-04-12 15:55:21.000000 sortedintersect-0.4.0/README.md
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)       38 2024-04-12 15:59:41.406343 sortedintersect-0.4.0/setup.cfg
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)      648 2024-04-12 15:58:52.000000 sortedintersect-0.4.0/setup.py
+drwxr-xr-x   0 sbi8kc2    (502) staff       (20)        0 2024-04-12 15:59:41.372124 sortedintersect-0.4.0/sortedintersect/
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)       60 2024-04-12 11:35:56.000000 sortedintersect-0.4.0/sortedintersect/__init__.py
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)   390554 2024-04-12 15:35:36.000000 sortedintersect-0.4.0/sortedintersect/sintersect.cpp
+-rwxr-xr-x   0 sbi8kc2    (502) staff       (20)   130605 2024-04-12 15:35:37.000000 sortedintersect-0.4.0/sortedintersect/sintersect.cpython-310-darwin.so
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     2369 2024-04-12 11:24:34.000000 sortedintersect-0.4.0/sortedintersect/sintersect.hpp
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     7137 2024-04-12 15:35:21.000000 sortedintersect-0.4.0/sortedintersect/sintersect.pyx
+drwxr-xr-x   0 sbi8kc2    (502) staff       (20)        0 2024-04-12 15:59:41.403831 sortedintersect-0.4.0/sortedintersect.egg-info/
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)      228 2024-04-12 15:59:41.000000 sortedintersect-0.4.0/sortedintersect.egg-info/PKG-INFO
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)      539 2024-04-12 15:59:41.000000 sortedintersect-0.4.0/sortedintersect.egg-info/SOURCES.txt
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)        1 2024-04-12 15:59:41.000000 sortedintersect-0.4.0/sortedintersect.egg-info/dependency_links.txt
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)        7 2024-04-12 15:59:41.000000 sortedintersect-0.4.0/sortedintersect.egg-info/requires.txt
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)       22 2024-04-12 15:59:41.000000 sortedintersect-0.4.0/sortedintersect.egg-info/top_level.txt
+drwxr-xr-x   0 sbi8kc2    (502) staff       (20)        0 2024-04-12 15:59:41.401233 sortedintersect-0.4.0/tests/
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)        0 2024-04-10 09:12:44.000000 sortedintersect-0.4.0/tests/__init__.py
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)    31345 2024-04-12 15:39:03.000000 sortedintersect-0.4.0/tests/benchmark.png
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     4779 2024-04-12 15:50:23.000000 sortedintersect-0.4.0/tests/benchmark.py
+-rw-r--r--   0 sbi8kc2    (502) staff       (20) 18662081 2024-04-12 07:59:40.000000 sortedintersect-0.4.0/tests/chr1_reads.bed
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)    10928 2024-04-12 08:07:41.000000 sortedintersect-0.4.0/tests/chr1_ucsc_genes.bed
+-rw-r--r--   0 sbi8kc2    (502) staff       (20)     4525 2024-04-12 14:15:30.000000 sortedintersect-0.4.0/tests/test_sortedintersect.py
```

### Comparing `sortedintersect-0.2.0/setup.py` & `sortedintersect-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from setuptools.extension import Extension
 from setuptools import setup, find_packages
 
 ext_modules = list()
 
-ext_modules.append(Extension("sortedintersect.intersect",
-                             ["sortedintersect/intersect.pyx"],
-                             # extra_compile_args=extras,
+ext_modules.append(Extension("sortedintersect.sintersect",
+                             ["sortedintersect/sintersect.pyx"],
                              language="c++",
                              ))
 
 
-setup(version='0.2.0',
+setup(version='0.4.0',
       name='sortedintersect',
       description="Interval intersection for sorted query and target intervals",
-      long_description=open('README.rst').read(),
       author="Kez Cleal",
       author_email="clealk@cardiff.ac.uk",
       packages=find_packages(),
       setup_requires=['cython'],
       install_requires=['cython'],
       ext_modules=ext_modules,
-      test_suite='nose.collector',
-      tests_require='nose',
 )
```

### Comparing `sortedintersect-0.2.0/sortedintersect/intersect.cpp` & `sortedintersect-0.4.0/sortedintersect/sintersect.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-/* Generated by Cython 0.29.21 */
+/* Generated by Cython 0.29.37 */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_21"
-#define CYTHON_HEX_VERSION 0x001D15F0
+#define CYTHON_ABI "0_29_37"
+#define CYTHON_HEX_VERSION 0x001D25F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -43,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -71,26 +74,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -120,18 +131,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -143,61 +203,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -308,35 +379,96 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -436,27 +568,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -552,18 +692,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -580,16 +720,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -612,23 +754,23 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__sortedintersect__intersect
-#define __PYX_HAVE_API__sortedintersect__intersect
+#define __PYX_HAVE__sortedintersect__sintersect
+#define __PYX_HAVE_API__sortedintersect__sintersect
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
-#include <stdint.h>
+#include <algorithm>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -717,14 +859,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -829,67 +972,82 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "sortedintersect/intersect.pyx",
+  "sortedintersect/sintersect.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_15sortedintersect_9intersect_ISet;
-struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add;
+struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet;
+struct __pyx_t_15sortedintersect_10sintersect_Interval;
+struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add;
 
-/* "sortedintersect/intersect.pyx":38
- *         self.index = 0
+/* "sortedintersect/sintersect.pyx":13
  * 
+ * 
+ * cdef struct Interval:             # <<<<<<<<<<<<<<
+ *     int end
+ *     int covered_end
+ */
+struct __pyx_t_15sortedintersect_10sintersect_Interval {
+  int end;
+  int covered_end;
+};
+
+/* "sortedintersect/sintersect.pyx":48
+ *     def set_distance_threshold(self, threshold):
+ *         self.distance_threshold = threshold
  *     cpdef add(self, int start, int end, value=None):             # <<<<<<<<<<<<<<
- *         assert end >= start
- *         if start < self.last_r_start:
+ *         if end < start:
+ *             raise ValueError("End less than start")
  */
-struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add {
+struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add {
   int __pyx_n;
   PyObject *value;
 };
 
-/* "sortedintersect/intersect.pyx":14
+/* "sortedintersect/sintersect.pyx":18
+ * 
  * 
+ * cdef class IntervalSet:             # <<<<<<<<<<<<<<
+ *     """An interval set for searching with sorted reference intervals and optionally sorted query points/intervals
  * 
- * cdef class ISet:             # <<<<<<<<<<<<<<
- *     """A sorted interval set for searching with sorted query intervals / points"""
- *     cdef vector[int] starts
  */
-struct __pyx_obj_15sortedintersect_9intersect_ISet {
+struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet {
   PyObject_HEAD
-  struct __pyx_vtabstruct_15sortedintersect_9intersect_ISet *__pyx_vtab;
+  struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *__pyx_vtab;
   std::vector<int>  starts;
-  std::vector<int>  ends;
+  std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  ends;
   int last_r_start;
-  int last_r_end;
   int last_q_start;
-  int last_q_end;
-  int current_r_start;
   int current_r_end;
-  int index;
+  int current_r_start;
+  size_t index;
   int add_data;
-  int started_ref;
+  int bool_only;
   PyObject *data;
+  int distance_threshold;
 };
 
 
 
-struct __pyx_vtabstruct_15sortedintersect_9intersect_ISet {
-  PyObject *(*add)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add *__pyx_optional_args);
-  PyObject *(*add_from_iter)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, PyObject *, int __pyx_skip_dispatch);
-  PyObject *(*search_point)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int __pyx_skip_dispatch);
-  PyObject *(*search_interval)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int, int __pyx_skip_dispatch);
+struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet {
+  PyObject *(*add)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add *__pyx_optional_args);
+  PyObject *(*add_from_iter)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, PyObject *, int __pyx_skip_dispatch);
+  void (*_line_scan)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int);
+  void (*_binary_search)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int);
+  void (*_set_reference_index)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int);
+  PyObject *(*search_point)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int __pyx_skip_dispatch);
+  PyObject *(*search_interval)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int, int __pyx_skip_dispatch);
 };
-static struct __pyx_vtabstruct_15sortedintersect_9intersect_ISet *__pyx_vtabptr_15sortedintersect_9intersect_ISet;
+static struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *__pyx_vtabptr_15sortedintersect_10sintersect_IntervalSet;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1009,21 +1167,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
@@ -1032,36 +1198,14 @@
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
-/* BuildPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
-                                                int prepend_sign, char padding_char);
-
-/* CIntToPyUnicode.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* JoinPyUnicode.proto */
-static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
-                                      Py_UCS4 max_char);
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1093,14 +1237,41 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* BuildPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char);
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -1113,22 +1284,19 @@
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod1.proto */
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
-/* append.proto */
-static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
+/* HasAttr.proto */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
@@ -1144,58 +1312,80 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
-
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
-/* HasAttr.proto */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
-
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
@@ -1205,14 +1395,49 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1257,17 +1482,16 @@
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* None.proto */
 #include <new>
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
+struct __pyx_t_15sortedintersect_10sintersect_Interval;
+static PyObject* __pyx_convert__to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(struct __pyx_t_15sortedintersect_10sintersect_Interval s);
 /* CppExceptionConversion.proto */
 #ifndef __Pyx_CppExn2PyErr
 #include <new>
 #include <typeinfo>
 #include <stdexcept>
 #include <ios>
 static void __Pyx_CppExn2PyErr() {
@@ -1303,24 +1527,27 @@
   {
     PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
   }
 }
 #endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
+static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
@@ -1333,160 +1560,189 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_add(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add *__pyx_optional_args); /* proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_add_from_iter(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_iterable, int __pyx_skip_dispatch); /* proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_search_point(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_pos, int __pyx_skip_dispatch); /* proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_search_interval(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add *__pyx_optional_args); /* proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add_from_iter(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_iterable, int __pyx_skip_dispatch); /* proto*/
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__line_scan(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos); /* proto*/
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__binary_search(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos); /* proto*/
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__set_reference_index(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos); /* proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_point(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos, int __pyx_skip_dispatch); /* proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_interval(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from 'libcpp.vector' */
 
-/* Module declarations from 'libc.stdint' */
+/* Module declarations from 'libcpp' */
+
+/* Module declarations from 'libcpp.algorithm' */
 
-/* Module declarations from 'sortedintersect.intersect' */
-static PyTypeObject *__pyx_ptype_15sortedintersect_9intersect_ISet = 0;
-static CYTHON_INLINE int __pyx_f_15sortedintersect_9intersect_is_overlapping(int, int, int, int); /*proto*/
-static struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_f_15sortedintersect_9intersect_IntervalSet(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect___pyx_unpickle_ISet__set_state(struct __pyx_obj_15sortedintersect_9intersect_ISet *, PyObject *); /*proto*/
+/* Module declarations from 'sortedintersect.sintersect' */
+static PyTypeObject *__pyx_ptype_15sortedintersect_10sintersect_IntervalSet = 0;
+static int __pyx_f_15sortedintersect_10sintersect_is_overlapping(int, int, int, int); /*proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet__set_state(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, PyObject *); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(const std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  &); /*proto*/
+static struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(PyObject *); /*proto*/
+static std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(PyObject *); /*proto*/
 static PyObject *__pyx_convert_vector_to_py_int(const std::vector<int>  &); /*proto*/
 static std::vector<int>  __pyx_convert_vector_from_py_int(PyObject *); /*proto*/
-#define __Pyx_MODULE_NAME "sortedintersect.intersect"
-extern int __pyx_module_is_main_sortedintersect__intersect;
-int __pyx_module_is_main_sortedintersect__intersect = 0;
+#define __Pyx_MODULE_NAME "sortedintersect.sintersect"
+extern int __pyx_module_is_main_sortedintersect__sintersect;
+int __pyx_module_is_main_sortedintersect__sintersect = 0;
 
-/* Implementation of 'sortedintersect.intersect' */
+/* Implementation of 'sortedintersect.sintersect' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
-static const char __pyx_k_[] = "-";
+static PyObject *__pyx_builtin_TypeError;
+static PyObject *__pyx_builtin_KeyError;
+static const char __pyx_k__2[] = "-";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_end[] = "end";
+static const char __pyx_k_len[] = "len";
 static const char __pyx_k_new[] = "__new__";
-static const char __pyx_k_ISet[] = "ISet";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_value[] = "value";
-static const char __pyx_k_append[] = "append";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Interval[] = "Interval ";
-static const char __pyx_k_Position[] = "Position ";
+static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_TypeError[] = "TypeError";
+static const char __pyx_k_bool_only[] = "bool_only";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_with_data[] = "with_data";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_IntervalSet[] = "IntervalSet";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_covered_end[] = "covered_end";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_search_point[] = "search_point";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_add_from_iter[] = "add_from_iter";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_search_interval[] = "search_interval";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_pyx_unpickle_ISet[] = "__pyx_unpickle_ISet";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_sortedintersect_intersect[] = "sortedintersect.intersect";
+static const char __pyx_k_distance_threshold[] = "distance_threshold";
+static const char __pyx_k_End_less_than_start[] = "End less than start";
+static const char __pyx_k_pyx_unpickle_IntervalSet[] = "__pyx_unpickle_IntervalSet";
+static const char __pyx_k_sortedintersect_sintersect[] = "sortedintersect.sintersect";
 static const char __pyx_k_is_not_in_sorted_order_last_int[] = " is not in sorted order, last interval seen was ";
-static const char __pyx_k_is_not_in_sorted_order_last_que[] = " is not in sorted order, last query interval seen was ";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x18[] = "Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))";
-static PyObject *__pyx_kp_u_;
-static PyObject *__pyx_n_s_ISet;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x18;
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))";
+static const char __pyx_k_No_value_specified_for_struct_at[] = "No value specified for struct attribute 'end'";
+static const char __pyx_k_No_value_specified_for_struct_at_2[] = "No value specified for struct attribute 'covered_end'";
+static PyObject *__pyx_kp_u_End_less_than_start;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_kp_u_Interval;
+static PyObject *__pyx_n_s_IntervalSet;
 static PyObject *__pyx_n_u_IntervalSet;
+static PyObject *__pyx_n_s_KeyError;
+static PyObject *__pyx_kp_s_No_value_specified_for_struct_at;
+static PyObject *__pyx_kp_s_No_value_specified_for_struct_at_2;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_kp_u_Position;
+static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueError;
+static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s_add;
 static PyObject *__pyx_n_s_add_from_iter;
 static PyObject *__pyx_n_s_all;
-static PyObject *__pyx_n_s_append;
+static PyObject *__pyx_n_s_bool_only;
 static PyObject *__pyx_n_s_cline_in_traceback;
+static PyObject *__pyx_n_s_covered_end;
 static PyObject *__pyx_n_s_dict;
+static PyObject *__pyx_n_s_distance_threshold;
 static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_kp_u_is_not_in_sorted_order_last_int;
-static PyObject *__pyx_kp_u_is_not_in_sorted_order_last_que;
+static PyObject *__pyx_n_u_len;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
-static PyObject *__pyx_n_s_pyx_unpickle_ISet;
+static PyObject *__pyx_n_s_pyx_unpickle_IntervalSet;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_search_interval;
 static PyObject *__pyx_n_s_search_point;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_sortedintersect_intersect;
+static PyObject *__pyx_n_s_sortedintersect_sintersect;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_with_data;
-static int __pyx_pf_15sortedintersect_9intersect_4ISet___init__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_with_data); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_2add(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_4add_from_iter(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_iterable); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_6search_point(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_pos); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_8search_interval(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_10__reduce_cython__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_12__setstate_cython__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_IntervalSet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_with_data); /* proto */
-static PyObject *__pyx_pf_15sortedintersect_9intersect_2__pyx_unpickle_ISet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_15sortedintersect_9intersect_ISet(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_25621563;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_codeobj__3;
+static int __pyx_pf_15sortedintersect_10sintersect_11IntervalSet___init__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_with_data, PyObject *__pyx_v_bool_only, PyObject *__pyx_v_distance_threshold); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_2set_distance_threshold(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_threshold); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_4add(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_6add_from_iter(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_iterable); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_8search_point(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_10search_interval(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_12__reduce_cython__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_14__setstate_cython__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_15sortedintersect_10sintersect_IntervalSet(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_50000;
+static PyObject *__pyx_int_105172298;
+static PyObject *__pyx_int_151996738;
+static PyObject *__pyx_int_262538656;
+static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_codeobj__7;
 /* Late includes */
 
-/* "sortedintersect/intersect.pyx":10
+/* "sortedintersect/sintersect.pyx":9
  * 
  * 
- * cdef inline bint is_overlapping(int x1, int x2, int y1, int y2) nogil:             # <<<<<<<<<<<<<<
+ * cdef bint is_overlapping(int x1, int x2, int y1, int y2):             # <<<<<<<<<<<<<<
  *     return max(x1, y1) <= min(x2, y2)
  * 
  */
 
-static CYTHON_INLINE int __pyx_f_15sortedintersect_9intersect_is_overlapping(int __pyx_v_x1, int __pyx_v_x2, int __pyx_v_y1, int __pyx_v_y2) {
+static int __pyx_f_15sortedintersect_10sintersect_is_overlapping(int __pyx_v_x1, int __pyx_v_x2, int __pyx_v_y1, int __pyx_v_y2) {
   int __pyx_r;
+  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
+  __Pyx_RefNannySetupContext("is_overlapping", 0);
 
-  /* "sortedintersect/intersect.pyx":11
+  /* "sortedintersect/sintersect.pyx":10
  * 
- * cdef inline bint is_overlapping(int x1, int x2, int y1, int y2) nogil:
+ * cdef bint is_overlapping(int x1, int x2, int y1, int y2):
  *     return max(x1, y1) <= min(x2, y2)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = __pyx_v_y1;
   __pyx_t_2 = __pyx_v_x1;
   if (((__pyx_t_1 > __pyx_t_2) != 0)) {
@@ -1500,242 +1756,303 @@
     __pyx_t_4 = __pyx_t_1;
   } else {
     __pyx_t_4 = __pyx_t_2;
   }
   __pyx_r = (__pyx_t_3 <= __pyx_t_4);
   goto __pyx_L0;
 
-  /* "sortedintersect/intersect.pyx":10
+  /* "sortedintersect/sintersect.pyx":9
  * 
  * 
- * cdef inline bint is_overlapping(int x1, int x2, int y1, int y2) nogil:             # <<<<<<<<<<<<<<
+ * cdef bint is_overlapping(int x1, int x2, int y1, int y2):             # <<<<<<<<<<<<<<
  *     return max(x1, y1) <= min(x2, y2)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sortedintersect/intersect.pyx":25
- *     cdef bint started_ref
- *     cdef object data
- *     def __init__(self, with_data):             # <<<<<<<<<<<<<<
- *         if with_data:
- *             self.add_data = True
+/* "sortedintersect/sintersect.pyx":37
+ *     cdef list data
+ *     cdef int distance_threshold
+ *     def __init__(self, with_data=False, bool_only=False, distance_threshold=50_000):             # <<<<<<<<<<<<<<
+ *         self.add_data = with_data
+ *         self.bool_only = bool_only
  */
 
 /* Python wrapper */
-static int __pyx_pw_15sortedintersect_9intersect_4ISet_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_15sortedintersect_9intersect_4ISet_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_15sortedintersect_10sintersect_11IntervalSet_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_15sortedintersect_10sintersect_11IntervalSet_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_with_data = 0;
+  PyObject *__pyx_v_bool_only = 0;
+  PyObject *__pyx_v_distance_threshold = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_with_data,0};
-    PyObject* values[1] = {0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_with_data,&__pyx_n_s_bool_only,&__pyx_n_s_distance_threshold,0};
+    PyObject* values[3] = {0,0,0};
+    values[0] = ((PyObject *)Py_False);
+    values[1] = ((PyObject *)Py_False);
+    values[2] = ((PyObject *)__pyx_int_50000);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_with_data)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_with_data);
+          if (value) { values[0] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bool_only);
+          if (value) { values[1] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_distance_threshold);
+          if (value) { values[2] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 25, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
     }
     __pyx_v_with_data = values[0];
+    __pyx_v_bool_only = values[1];
+    __pyx_v_distance_threshold = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet___init__(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), __pyx_v_with_data);
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet___init__(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), __pyx_v_with_data, __pyx_v_bool_only, __pyx_v_distance_threshold);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_15sortedintersect_9intersect_4ISet___init__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_with_data) {
+static int __pyx_pf_15sortedintersect_10sintersect_11IntervalSet___init__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_with_data, PyObject *__pyx_v_bool_only, PyObject *__pyx_v_distance_threshold) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "sortedintersect/intersect.pyx":26
- *     cdef object data
- *     def __init__(self, with_data):
- *         if with_data:             # <<<<<<<<<<<<<<
- *             self.add_data = True
- *             self.data = []
- */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_with_data); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 26, __pyx_L1_error)
-  if (__pyx_t_1) {
-
-    /* "sortedintersect/intersect.pyx":27
- *     def __init__(self, with_data):
- *         if with_data:
- *             self.add_data = True             # <<<<<<<<<<<<<<
- *             self.data = []
- *         else:
- */
-    __pyx_v_self->add_data = 1;
-
-    /* "sortedintersect/intersect.pyx":28
- *         if with_data:
- *             self.add_data = True
- *             self.data = []             # <<<<<<<<<<<<<<
- *         else:
- *             self.add_data = False
- */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    __Pyx_GOTREF(__pyx_v_self->data);
-    __Pyx_DECREF(__pyx_v_self->data);
-    __pyx_v_self->data = __pyx_t_2;
-    __pyx_t_2 = 0;
-
-    /* "sortedintersect/intersect.pyx":26
- *     cdef object data
- *     def __init__(self, with_data):
- *         if with_data:             # <<<<<<<<<<<<<<
- *             self.add_data = True
- *             self.data = []
- */
-    goto __pyx_L3;
-  }
-
-  /* "sortedintersect/intersect.pyx":30
- *             self.data = []
- *         else:
- *             self.add_data = False             # <<<<<<<<<<<<<<
- *             self.data = None
+  /* "sortedintersect/sintersect.pyx":38
+ *     cdef int distance_threshold
+ *     def __init__(self, with_data=False, bool_only=False, distance_threshold=50_000):
+ *         self.add_data = with_data             # <<<<<<<<<<<<<<
+ *         self.bool_only = bool_only
+ *         self.data = list()
+ */
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_with_data); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_v_self->add_data = __pyx_t_1;
+
+  /* "sortedintersect/sintersect.pyx":39
+ *     def __init__(self, with_data=False, bool_only=False, distance_threshold=50_000):
+ *         self.add_data = with_data
+ *         self.bool_only = bool_only             # <<<<<<<<<<<<<<
+ *         self.data = list()
  *         self.last_r_start = -2_147_483_648
  */
-  /*else*/ {
-    __pyx_v_self->add_data = 0;
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_bool_only); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_v_self->bool_only = __pyx_t_1;
 
-    /* "sortedintersect/intersect.pyx":31
- *         else:
- *             self.add_data = False
- *             self.data = None             # <<<<<<<<<<<<<<
+  /* "sortedintersect/sintersect.pyx":40
+ *         self.add_data = with_data
+ *         self.bool_only = bool_only
+ *         self.data = list()             # <<<<<<<<<<<<<<
  *         self.last_r_start = -2_147_483_648
  *         self.last_q_start = -2_147_483_648
  */
-    __Pyx_INCREF(Py_None);
-    __Pyx_GIVEREF(Py_None);
-    __Pyx_GOTREF(__pyx_v_self->data);
-    __Pyx_DECREF(__pyx_v_self->data);
-    __pyx_v_self->data = Py_None;
-  }
-  __pyx_L3:;
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_2);
+  __Pyx_GOTREF(__pyx_v_self->data);
+  __Pyx_DECREF(__pyx_v_self->data);
+  __pyx_v_self->data = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "sortedintersect/intersect.pyx":32
- *             self.add_data = False
- *             self.data = None
+  /* "sortedintersect/sintersect.pyx":41
+ *         self.bool_only = bool_only
+ *         self.data = list()
  *         self.last_r_start = -2_147_483_648             # <<<<<<<<<<<<<<
  *         self.last_q_start = -2_147_483_648
- *         self.current_r_start = 0
+ *         self.current_r_end = 0
  */
   __pyx_v_self->last_r_start = -2147483648;
 
-  /* "sortedintersect/intersect.pyx":33
- *             self.data = None
+  /* "sortedintersect/sintersect.pyx":42
+ *         self.data = list()
  *         self.last_r_start = -2_147_483_648
  *         self.last_q_start = -2_147_483_648             # <<<<<<<<<<<<<<
- *         self.current_r_start = 0
  *         self.current_r_end = 0
+ *         self.index = 0
  */
   __pyx_v_self->last_q_start = -2147483648;
 
-  /* "sortedintersect/intersect.pyx":34
+  /* "sortedintersect/sintersect.pyx":43
  *         self.last_r_start = -2_147_483_648
  *         self.last_q_start = -2_147_483_648
- *         self.current_r_start = 0             # <<<<<<<<<<<<<<
- *         self.current_r_end = 0
- *         self.index = 0
- */
-  __pyx_v_self->current_r_start = 0;
-
-  /* "sortedintersect/intersect.pyx":35
- *         self.last_q_start = -2_147_483_648
- *         self.current_r_start = 0
  *         self.current_r_end = 0             # <<<<<<<<<<<<<<
  *         self.index = 0
- * 
+ *         self.distance_threshold = distance_threshold
  */
   __pyx_v_self->current_r_end = 0;
 
-  /* "sortedintersect/intersect.pyx":36
- *         self.current_r_start = 0
+  /* "sortedintersect/sintersect.pyx":44
+ *         self.last_q_start = -2_147_483_648
  *         self.current_r_end = 0
  *         self.index = 0             # <<<<<<<<<<<<<<
- * 
- *     cpdef add(self, int start, int end, value=None):
+ *         self.distance_threshold = distance_threshold
+ *     def set_distance_threshold(self, threshold):
  */
   __pyx_v_self->index = 0;
 
-  /* "sortedintersect/intersect.pyx":25
- *     cdef bint started_ref
- *     cdef object data
- *     def __init__(self, with_data):             # <<<<<<<<<<<<<<
- *         if with_data:
- *             self.add_data = True
+  /* "sortedintersect/sintersect.pyx":45
+ *         self.current_r_end = 0
+ *         self.index = 0
+ *         self.distance_threshold = distance_threshold             # <<<<<<<<<<<<<<
+ *     def set_distance_threshold(self, threshold):
+ *         self.distance_threshold = threshold
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_distance_threshold); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_v_self->distance_threshold = __pyx_t_3;
+
+  /* "sortedintersect/sintersect.pyx":37
+ *     cdef list data
+ *     cdef int distance_threshold
+ *     def __init__(self, with_data=False, bool_only=False, distance_threshold=50_000):             # <<<<<<<<<<<<<<
+ *         self.add_data = with_data
+ *         self.bool_only = bool_only
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sortedintersect/intersect.pyx":38
+/* "sortedintersect/sintersect.pyx":46
  *         self.index = 0
- * 
+ *         self.distance_threshold = distance_threshold
+ *     def set_distance_threshold(self, threshold):             # <<<<<<<<<<<<<<
+ *         self.distance_threshold = threshold
+ *     cpdef add(self, int start, int end, value=None):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_3set_distance_threshold(PyObject *__pyx_v_self, PyObject *__pyx_v_threshold); /*proto*/
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_3set_distance_threshold(PyObject *__pyx_v_self, PyObject *__pyx_v_threshold) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("set_distance_threshold (wrapper)", 0);
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_2set_distance_threshold(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), ((PyObject *)__pyx_v_threshold));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_2set_distance_threshold(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_threshold) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_distance_threshold", 0);
+
+  /* "sortedintersect/sintersect.pyx":47
+ *         self.distance_threshold = distance_threshold
+ *     def set_distance_threshold(self, threshold):
+ *         self.distance_threshold = threshold             # <<<<<<<<<<<<<<
+ *     cpdef add(self, int start, int end, value=None):
+ *         if end < start:
+ */
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_threshold); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_v_self->distance_threshold = __pyx_t_1;
+
+  /* "sortedintersect/sintersect.pyx":46
+ *         self.index = 0
+ *         self.distance_threshold = distance_threshold
+ *     def set_distance_threshold(self, threshold):             # <<<<<<<<<<<<<<
+ *         self.distance_threshold = threshold
+ *     cpdef add(self, int start, int end, value=None):
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.set_distance_threshold", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "sortedintersect/sintersect.pyx":48
+ *     def set_distance_threshold(self, threshold):
+ *         self.distance_threshold = threshold
  *     cpdef add(self, int start, int end, value=None):             # <<<<<<<<<<<<<<
- *         assert end >= start
- *         if start < self.last_r_start:
+ *         if end < start:
+ *             raise ValueError("End less than start")
  */
 
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_3add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_add(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add *__pyx_optional_args) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_5add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add *__pyx_optional_args) {
   PyObject *__pyx_v_value = ((PyObject *)Py_None);
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -1743,14 +2060,17 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   Py_ssize_t __pyx_t_10;
   Py_UCS4 __pyx_t_11;
   int __pyx_t_12;
+  int __pyx_t_13;
+  struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_t_14;
+  int __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_value = __pyx_optional_args->value;
@@ -1761,21 +2081,21 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_9intersect_4ISet_3add)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_5add)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -1785,47 +2105,47 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_v_value};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_v_value};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 48, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __Pyx_INCREF(__pyx_v_value);
           __Pyx_GIVEREF(__pyx_v_value);
           PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_value);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -1840,195 +2160,233 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "sortedintersect/intersect.pyx":39
- * 
+  /* "sortedintersect/sintersect.pyx":49
+ *         self.distance_threshold = threshold
+ *     cpdef add(self, int start, int end, value=None):
+ *         if end < start:             # <<<<<<<<<<<<<<
+ *             raise ValueError("End less than start")
+ *         if start < self.last_r_start:
+ */
+  __pyx_t_9 = ((__pyx_v_end < __pyx_v_start) != 0);
+  if (unlikely(__pyx_t_9)) {
+
+    /* "sortedintersect/sintersect.pyx":50
  *     cpdef add(self, int start, int end, value=None):
- *         assert end >= start             # <<<<<<<<<<<<<<
+ *         if end < start:
+ *             raise ValueError("End less than start")             # <<<<<<<<<<<<<<
  *         if start < self.last_r_start:
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_end >= __pyx_v_start) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 39, __pyx_L1_error)
-    }
-  }
-  #endif
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 50, __pyx_L1_error)
 
-  /* "sortedintersect/intersect.pyx":40
+    /* "sortedintersect/sintersect.pyx":49
+ *         self.distance_threshold = threshold
  *     cpdef add(self, int start, int end, value=None):
- *         assert end >= start
+ *         if end < start:             # <<<<<<<<<<<<<<
+ *             raise ValueError("End less than start")
+ *         if start < self.last_r_start:
+ */
+  }
+
+  /* "sortedintersect/sintersect.pyx":51
+ *         if end < start:
+ *             raise ValueError("End less than start")
  *         if start < self.last_r_start:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *         self.starts.push_back(start)
  */
   __pyx_t_9 = ((__pyx_v_start < __pyx_v_self->last_r_start) != 0);
   if (unlikely(__pyx_t_9)) {
 
-    /* "sortedintersect/intersect.pyx":41
- *         assert end >= start
+    /* "sortedintersect/sintersect.pyx":52
+ *             raise ValueError("End less than start")
  *         if start < self.last_r_start:
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')             # <<<<<<<<<<<<<<
  *         self.starts.push_back(start)
- *         self.ends.push_back(end)
+ *         self.current_r_end = max(self.current_r_end, end)
  */
-    __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_10 = 0;
     __pyx_t_11 = 127;
     __Pyx_INCREF(__pyx_kp_u_Interval);
     __pyx_t_10 += 9;
     __Pyx_GIVEREF(__pyx_kp_u_Interval);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Interval);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
     __pyx_t_2 = 0;
-    __Pyx_INCREF(__pyx_kp_u_);
+    __Pyx_INCREF(__pyx_kp_u__2);
     __pyx_t_10 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u_);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__2);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__2);
+    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_kp_u_is_not_in_sorted_order_last_int);
     __pyx_t_10 += 48;
     __Pyx_GIVEREF(__pyx_kp_u_is_not_in_sorted_order_last_int);
     PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_is_not_in_sorted_order_last_int);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_r_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_r_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 6, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 6, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 41, __pyx_L1_error)
+    __PYX_ERR(0, 52, __pyx_L1_error)
 
-    /* "sortedintersect/intersect.pyx":40
- *     cpdef add(self, int start, int end, value=None):
- *         assert end >= start
+    /* "sortedintersect/sintersect.pyx":51
+ *         if end < start:
+ *             raise ValueError("End less than start")
  *         if start < self.last_r_start:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *         self.starts.push_back(start)
  */
   }
 
-  /* "sortedintersect/intersect.pyx":42
+  /* "sortedintersect/sintersect.pyx":53
  *         if start < self.last_r_start:
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *         self.starts.push_back(start)             # <<<<<<<<<<<<<<
- *         self.ends.push_back(end)
- *         self.last_r_start = start
+ *         self.current_r_end = max(self.current_r_end, end)
+ *         self.ends.push_back(Interval(end, self.current_r_end))
  */
   try {
     __pyx_v_self->starts.push_back(__pyx_v_start);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 42, __pyx_L1_error)
+    __PYX_ERR(0, 53, __pyx_L1_error)
   }
 
-  /* "sortedintersect/intersect.pyx":43
+  /* "sortedintersect/sintersect.pyx":54
  *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *         self.starts.push_back(start)
- *         self.ends.push_back(end)             # <<<<<<<<<<<<<<
+ *         self.current_r_end = max(self.current_r_end, end)             # <<<<<<<<<<<<<<
+ *         self.ends.push_back(Interval(end, self.current_r_end))
+ *         self.last_r_start = start
+ */
+  __pyx_t_7 = __pyx_v_end;
+  __pyx_t_12 = __pyx_v_self->current_r_end;
+  if (((__pyx_t_7 > __pyx_t_12) != 0)) {
+    __pyx_t_13 = __pyx_t_7;
+  } else {
+    __pyx_t_13 = __pyx_t_12;
+  }
+  __pyx_v_self->current_r_end = __pyx_t_13;
+
+  /* "sortedintersect/sintersect.pyx":55
+ *         self.starts.push_back(start)
+ *         self.current_r_end = max(self.current_r_end, end)
+ *         self.ends.push_back(Interval(end, self.current_r_end))             # <<<<<<<<<<<<<<
  *         self.last_r_start = start
  *         if self.add_data:
  */
+  __pyx_t_14.end = __pyx_v_end;
+  __pyx_t_14.covered_end = __pyx_v_self->current_r_end;
   try {
-    __pyx_v_self->ends.push_back(__pyx_v_end);
+    __pyx_v_self->ends.push_back(__pyx_t_14);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 43, __pyx_L1_error)
+    __PYX_ERR(0, 55, __pyx_L1_error)
   }
 
-  /* "sortedintersect/intersect.pyx":44
- *         self.starts.push_back(start)
- *         self.ends.push_back(end)
+  /* "sortedintersect/sintersect.pyx":56
+ *         self.current_r_end = max(self.current_r_end, end)
+ *         self.ends.push_back(Interval(end, self.current_r_end))
  *         self.last_r_start = start             # <<<<<<<<<<<<<<
  *         if self.add_data:
  *             self.data.append(value)
  */
   __pyx_v_self->last_r_start = __pyx_v_start;
 
-  /* "sortedintersect/intersect.pyx":45
- *         self.ends.push_back(end)
+  /* "sortedintersect/sintersect.pyx":57
+ *         self.ends.push_back(Interval(end, self.current_r_end))
  *         self.last_r_start = start
  *         if self.add_data:             # <<<<<<<<<<<<<<
  *             self.data.append(value)
  * 
  */
   __pyx_t_9 = (__pyx_v_self->add_data != 0);
   if (__pyx_t_9) {
 
-    /* "sortedintersect/intersect.pyx":46
+    /* "sortedintersect/sintersect.pyx":58
  *         self.last_r_start = start
  *         if self.add_data:
  *             self.data.append(value)             # <<<<<<<<<<<<<<
  * 
  *     cpdef add_from_iter(self, iterable):
  */
-    __pyx_t_12 = __Pyx_PyObject_Append(__pyx_v_self->data, __pyx_v_value); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 46, __pyx_L1_error)
+    if (unlikely(__pyx_v_self->data == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
+      __PYX_ERR(0, 58, __pyx_L1_error)
+    }
+    __pyx_t_15 = __Pyx_PyList_Append(__pyx_v_self->data, __pyx_v_value); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
 
-    /* "sortedintersect/intersect.pyx":45
- *         self.ends.push_back(end)
+    /* "sortedintersect/sintersect.pyx":57
+ *         self.ends.push_back(Interval(end, self.current_r_end))
  *         self.last_r_start = start
  *         if self.add_data:             # <<<<<<<<<<<<<<
  *             self.data.append(value)
  * 
  */
   }
 
-  /* "sortedintersect/intersect.pyx":38
- *         self.index = 0
- * 
+  /* "sortedintersect/sintersect.pyx":48
+ *     def set_distance_threshold(self, threshold):
+ *         self.distance_threshold = threshold
  *     cpdef add(self, int start, int end, value=None):             # <<<<<<<<<<<<<<
- *         assert end >= start
- *         if start < self.last_r_start:
+ *         if end < start:
+ *             raise ValueError("End less than start")
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_3add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_3add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_5add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_5add(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_start;
   int __pyx_v_end;
   PyObject *__pyx_v_value = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2056,141 +2414,145 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add", 0, 2, 3, 1); __PYX_ERR(0, 38, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add", 0, 2, 3, 1); __PYX_ERR(0, 48, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add") < 0)) __PYX_ERR(0, 38, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
-    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
+    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
     __pyx_v_value = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 38, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 48, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_2add(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), __pyx_v_start, __pyx_v_end, __pyx_v_value);
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_4add(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), __pyx_v_start, __pyx_v_end, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_2add(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_4add(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add __pyx_t_2;
+  struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.value = __pyx_v_value;
-  __pyx_t_1 = __pyx_vtabptr_15sortedintersect_9intersect_ISet->add(__pyx_v_self, __pyx_v_start, __pyx_v_end, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_15sortedintersect_10sintersect_IntervalSet->add(__pyx_v_self, __pyx_v_start, __pyx_v_end, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sortedintersect/intersect.pyx":48
+/* "sortedintersect/sintersect.pyx":60
  *             self.data.append(value)
  * 
  *     cpdef add_from_iter(self, iterable):             # <<<<<<<<<<<<<<
  *         cdef int start, end
- *         for item in iterable:
+ *         if hasattr(iterable, "len"):
  */
 
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_5add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_add_from_iter(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_iterable, int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_7add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add_from_iter(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_iterable, int __pyx_skip_dispatch) {
   int __pyx_v_start;
   int __pyx_v_end;
   PyObject *__pyx_v_item = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  int __pyx_t_7;
-  int __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_UCS4 __pyx_t_10;
-  int __pyx_t_11;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *(*__pyx_t_8)(PyObject *);
+  int __pyx_t_9;
+  Py_ssize_t __pyx_t_10;
+  Py_UCS4 __pyx_t_11;
+  int __pyx_t_12;
+  int __pyx_t_13;
+  struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_t_14;
+  int __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_from_iter", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_from_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_from_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_9intersect_4ISet_5add_from_iter)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_7add_from_iter)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_iterable) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_iterable);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2203,359 +2565,939 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "sortedintersect/intersect.pyx":50
+  /* "sortedintersect/sintersect.pyx":62
  *     cpdef add_from_iter(self, iterable):
  *         cdef int start, end
+ *         if hasattr(iterable, "len"):             # <<<<<<<<<<<<<<
+ *             self.starts.reserve(len(iterable))
+ *             self.ends.reserve(len(iterable))
+ */
+  __pyx_t_5 = __Pyx_HasAttr(__pyx_v_iterable, __pyx_n_u_len); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_6 = (__pyx_t_5 != 0);
+  if (__pyx_t_6) {
+
+    /* "sortedintersect/sintersect.pyx":63
+ *         cdef int start, end
+ *         if hasattr(iterable, "len"):
+ *             self.starts.reserve(len(iterable))             # <<<<<<<<<<<<<<
+ *             self.ends.reserve(len(iterable))
+ *         for item in iterable:
+ */
+    __pyx_t_7 = PyObject_Length(__pyx_v_iterable); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_v_self->starts.reserve(__pyx_t_7);
+
+    /* "sortedintersect/sintersect.pyx":64
+ *         if hasattr(iterable, "len"):
+ *             self.starts.reserve(len(iterable))
+ *             self.ends.reserve(len(iterable))             # <<<<<<<<<<<<<<
+ *         for item in iterable:
+ *             start = item[0]
+ */
+    __pyx_t_7 = PyObject_Length(__pyx_v_iterable); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_v_self->ends.reserve(__pyx_t_7);
+
+    /* "sortedintersect/sintersect.pyx":62
+ *     cpdef add_from_iter(self, iterable):
+ *         cdef int start, end
+ *         if hasattr(iterable, "len"):             # <<<<<<<<<<<<<<
+ *             self.starts.reserve(len(iterable))
+ *             self.ends.reserve(len(iterable))
+ */
+  }
+
+  /* "sortedintersect/sintersect.pyx":65
+ *             self.starts.reserve(len(iterable))
+ *             self.ends.reserve(len(iterable))
  *         for item in iterable:             # <<<<<<<<<<<<<<
  *             start = item[0]
  *             end = item[1]
  */
   if (likely(PyList_CheckExact(__pyx_v_iterable)) || PyTuple_CheckExact(__pyx_v_iterable)) {
-    __pyx_t_1 = __pyx_v_iterable; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
+    __pyx_t_1 = __pyx_v_iterable; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
+    __pyx_t_8 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_iterable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_iterable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 65, __pyx_L1_error)
   }
   for (;;) {
-    if (likely(!__pyx_t_6)) {
+    if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 65, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
-        if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 65, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
-      __pyx_t_2 = __pyx_t_6(__pyx_t_1);
+      __pyx_t_2 = __pyx_t_8(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 50, __pyx_L1_error)
+          else __PYX_ERR(0, 65, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "sortedintersect/intersect.pyx":51
- *         cdef int start, end
+    /* "sortedintersect/sintersect.pyx":66
+ *             self.ends.reserve(len(iterable))
  *         for item in iterable:
  *             start = item[0]             # <<<<<<<<<<<<<<
  *             end = item[1]
  *             assert end >= start
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_start = __pyx_t_7;
+    __pyx_v_start = __pyx_t_9;
 
-    /* "sortedintersect/intersect.pyx":52
+    /* "sortedintersect/sintersect.pyx":67
  *         for item in iterable:
  *             start = item[0]
  *             end = item[1]             # <<<<<<<<<<<<<<
  *             assert end >= start
  *             if start < self.last_r_start:
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_end = __pyx_t_7;
+    __pyx_v_end = __pyx_t_9;
 
-    /* "sortedintersect/intersect.pyx":53
+    /* "sortedintersect/sintersect.pyx":68
  *             start = item[0]
  *             end = item[1]
  *             assert end >= start             # <<<<<<<<<<<<<<
  *             if start < self.last_r_start:
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_end >= __pyx_v_start) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 53, __pyx_L1_error)
+        __PYX_ERR(0, 68, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "sortedintersect/intersect.pyx":54
+    /* "sortedintersect/sintersect.pyx":69
  *             end = item[1]
  *             assert end >= start
  *             if start < self.last_r_start:             # <<<<<<<<<<<<<<
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *             self.starts.push_back(start)
  */
-    __pyx_t_8 = ((__pyx_v_start < __pyx_v_self->last_r_start) != 0);
-    if (unlikely(__pyx_t_8)) {
+    __pyx_t_6 = ((__pyx_v_start < __pyx_v_self->last_r_start) != 0);
+    if (unlikely(__pyx_t_6)) {
 
-      /* "sortedintersect/intersect.pyx":55
+      /* "sortedintersect/sintersect.pyx":70
  *             assert end >= start
  *             if start < self.last_r_start:
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')             # <<<<<<<<<<<<<<
  *             self.starts.push_back(start)
- *             self.ends.push_back(end)
+ *             self.current_r_end = max(self.current_r_end, end)
  */
-      __pyx_t_2 = PyTuple_New(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = 0;
-      __pyx_t_10 = 127;
+      __pyx_t_10 = 0;
+      __pyx_t_11 = 127;
       __Pyx_INCREF(__pyx_kp_u_Interval);
-      __pyx_t_9 += 9;
+      __pyx_t_10 += 9;
       __Pyx_GIVEREF(__pyx_kp_u_Interval);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_Interval);
-      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+      __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
       __pyx_t_3 = 0;
-      __Pyx_INCREF(__pyx_kp_u_);
-      __pyx_t_9 += 1;
-      __Pyx_GIVEREF(__pyx_kp_u_);
-      PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_);
-      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __Pyx_INCREF(__pyx_kp_u__2);
+      __pyx_t_10 += 1;
+      __Pyx_GIVEREF(__pyx_kp_u__2);
+      PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u__2);
+      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+      __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_INCREF(__pyx_kp_u_is_not_in_sorted_order_last_int);
-      __pyx_t_9 += 48;
+      __pyx_t_10 += 48;
       __Pyx_GIVEREF(__pyx_kp_u_is_not_in_sorted_order_last_int);
       PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u_is_not_in_sorted_order_last_int);
-      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_r_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_r_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+      __pyx_t_10 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_2, 6, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_2, 6, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 55, __pyx_L1_error)
+      __PYX_ERR(0, 70, __pyx_L1_error)
 
-      /* "sortedintersect/intersect.pyx":54
+      /* "sortedintersect/sintersect.pyx":69
  *             end = item[1]
  *             assert end >= start
  *             if start < self.last_r_start:             # <<<<<<<<<<<<<<
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *             self.starts.push_back(start)
  */
     }
 
-    /* "sortedintersect/intersect.pyx":56
+    /* "sortedintersect/sintersect.pyx":71
  *             if start < self.last_r_start:
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *             self.starts.push_back(start)             # <<<<<<<<<<<<<<
- *             self.ends.push_back(end)
- *             self.last_r_start = start
+ *             self.current_r_end = max(self.current_r_end, end)
+ *             self.ends.push_back(Interval(end, self.current_r_end))
  */
     try {
       __pyx_v_self->starts.push_back(__pyx_v_start);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 56, __pyx_L1_error)
+      __PYX_ERR(0, 71, __pyx_L1_error)
     }
 
-    /* "sortedintersect/intersect.pyx":57
+    /* "sortedintersect/sintersect.pyx":72
  *                 raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
  *             self.starts.push_back(start)
- *             self.ends.push_back(end)             # <<<<<<<<<<<<<<
+ *             self.current_r_end = max(self.current_r_end, end)             # <<<<<<<<<<<<<<
+ *             self.ends.push_back(Interval(end, self.current_r_end))
+ *             self.last_r_start = start
+ */
+    __pyx_t_9 = __pyx_v_end;
+    __pyx_t_12 = __pyx_v_self->current_r_end;
+    if (((__pyx_t_9 > __pyx_t_12) != 0)) {
+      __pyx_t_13 = __pyx_t_9;
+    } else {
+      __pyx_t_13 = __pyx_t_12;
+    }
+    __pyx_v_self->current_r_end = __pyx_t_13;
+
+    /* "sortedintersect/sintersect.pyx":73
+ *             self.starts.push_back(start)
+ *             self.current_r_end = max(self.current_r_end, end)
+ *             self.ends.push_back(Interval(end, self.current_r_end))             # <<<<<<<<<<<<<<
  *             self.last_r_start = start
  *             if self.add_data:
  */
+    __pyx_t_14.end = __pyx_v_end;
+    __pyx_t_14.covered_end = __pyx_v_self->current_r_end;
     try {
-      __pyx_v_self->ends.push_back(__pyx_v_end);
+      __pyx_v_self->ends.push_back(__pyx_t_14);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 57, __pyx_L1_error)
+      __PYX_ERR(0, 73, __pyx_L1_error)
     }
 
-    /* "sortedintersect/intersect.pyx":58
- *             self.starts.push_back(start)
- *             self.ends.push_back(end)
+    /* "sortedintersect/sintersect.pyx":74
+ *             self.current_r_end = max(self.current_r_end, end)
+ *             self.ends.push_back(Interval(end, self.current_r_end))
  *             self.last_r_start = start             # <<<<<<<<<<<<<<
  *             if self.add_data:
  *                 self.data.append(item[2])
  */
     __pyx_v_self->last_r_start = __pyx_v_start;
 
-    /* "sortedintersect/intersect.pyx":59
- *             self.ends.push_back(end)
+    /* "sortedintersect/sintersect.pyx":75
+ *             self.ends.push_back(Interval(end, self.current_r_end))
  *             self.last_r_start = start
  *             if self.add_data:             # <<<<<<<<<<<<<<
  *                 self.data.append(item[2])
  * 
  */
-    __pyx_t_8 = (__pyx_v_self->add_data != 0);
-    if (__pyx_t_8) {
+    __pyx_t_6 = (__pyx_v_self->add_data != 0);
+    if (__pyx_t_6) {
 
-      /* "sortedintersect/intersect.pyx":60
+      /* "sortedintersect/sintersect.pyx":76
  *             self.last_r_start = start
  *             if self.add_data:
  *                 self.data.append(item[2])             # <<<<<<<<<<<<<<
  * 
- *     cpdef search_point(self, int pos):
+ *     cdef void _line_scan(self, int pos):
  */
-      __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+      if (unlikely(__pyx_v_self->data == Py_None)) {
+        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
+        __PYX_ERR(0, 76, __pyx_L1_error)
+      }
+      __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_item, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_11 = __Pyx_PyObject_Append(__pyx_v_self->data, __pyx_t_2); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyList_Append(__pyx_v_self->data, __pyx_t_2); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 76, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "sortedintersect/intersect.pyx":59
- *             self.ends.push_back(end)
+      /* "sortedintersect/sintersect.pyx":75
+ *             self.ends.push_back(Interval(end, self.current_r_end))
  *             self.last_r_start = start
  *             if self.add_data:             # <<<<<<<<<<<<<<
  *                 self.data.append(item[2])
  * 
  */
     }
 
-    /* "sortedintersect/intersect.pyx":50
- *     cpdef add_from_iter(self, iterable):
- *         cdef int start, end
+    /* "sortedintersect/sintersect.pyx":65
+ *             self.starts.reserve(len(iterable))
+ *             self.ends.reserve(len(iterable))
  *         for item in iterable:             # <<<<<<<<<<<<<<
  *             start = item[0]
  *             end = item[1]
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "sortedintersect/intersect.pyx":48
+  /* "sortedintersect/sintersect.pyx":60
  *             self.data.append(value)
  * 
  *     cpdef add_from_iter(self, iterable):             # <<<<<<<<<<<<<<
  *         cdef int start, end
- *         for item in iterable:
+ *         if hasattr(iterable, "len"):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.add_from_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.add_from_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_5add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_5add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_7add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_7add_from_iter(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_from_iter (wrapper)", 0);
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_4add_from_iter(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), ((PyObject *)__pyx_v_iterable));
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_6add_from_iter(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), ((PyObject *)__pyx_v_iterable));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_4add_from_iter(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v_iterable) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_6add_from_iter(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v_iterable) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_from_iter", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_15sortedintersect_9intersect_4ISet_add_from_iter(__pyx_v_self, __pyx_v_iterable, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_15sortedintersect_10sintersect_11IntervalSet_add_from_iter(__pyx_v_self, __pyx_v_iterable, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.add_from_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.add_from_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sortedintersect/intersect.pyx":62
+/* "sortedintersect/sintersect.pyx":78
  *                 self.data.append(item[2])
  * 
+ *     cdef void _line_scan(self, int pos):             # <<<<<<<<<<<<<<
+ *         cdef size_t i
+ *         before = self.index
+ */
+
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__line_scan(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos) {
+  size_t __pyx_v_i;
+  CYTHON_UNUSED size_t __pyx_v_before;
+  __Pyx_RefNannyDeclarations
+  size_t __pyx_t_1;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  __Pyx_RefNannySetupContext("_line_scan", 0);
+
+  /* "sortedintersect/sintersect.pyx":80
+ *     cdef void _line_scan(self, int pos):
+ *         cdef size_t i
+ *         before = self.index             # <<<<<<<<<<<<<<
+ *         if pos < self.last_q_start:
+ *             i = self.index
+ */
+  __pyx_t_1 = __pyx_v_self->index;
+  __pyx_v_before = __pyx_t_1;
+
+  /* "sortedintersect/sintersect.pyx":81
+ *         cdef size_t i
+ *         before = self.index
+ *         if pos < self.last_q_start:             # <<<<<<<<<<<<<<
+ *             i = self.index
+ *             while i > 0 and pos <= self.starts[i]:
+ */
+  __pyx_t_2 = ((__pyx_v_pos < __pyx_v_self->last_q_start) != 0);
+  if (__pyx_t_2) {
+
+    /* "sortedintersect/sintersect.pyx":82
+ *         before = self.index
+ *         if pos < self.last_q_start:
+ *             i = self.index             # <<<<<<<<<<<<<<
+ *             while i > 0 and pos <= self.starts[i]:
+ *                 i -= 1
+ */
+    __pyx_t_1 = __pyx_v_self->index;
+    __pyx_v_i = __pyx_t_1;
+
+    /* "sortedintersect/sintersect.pyx":83
+ *         if pos < self.last_q_start:
+ *             i = self.index
+ *             while i > 0 and pos <= self.starts[i]:             # <<<<<<<<<<<<<<
+ *                 i -= 1
+ *             while True:
+ */
+    while (1) {
+      __pyx_t_3 = ((__pyx_v_i > 0) != 0);
+      if (__pyx_t_3) {
+      } else {
+        __pyx_t_2 = __pyx_t_3;
+        goto __pyx_L6_bool_binop_done;
+      }
+      __pyx_t_3 = ((__pyx_v_pos <= (__pyx_v_self->starts[__pyx_v_i])) != 0);
+      __pyx_t_2 = __pyx_t_3;
+      __pyx_L6_bool_binop_done:;
+      if (!__pyx_t_2) break;
+
+      /* "sortedintersect/sintersect.pyx":84
+ *             i = self.index
+ *             while i > 0 and pos <= self.starts[i]:
+ *                 i -= 1             # <<<<<<<<<<<<<<
+ *             while True:
+ *                 if self.ends[i].covered_end >= pos:
+ */
+      __pyx_v_i = (__pyx_v_i - 1);
+    }
+
+    /* "sortedintersect/sintersect.pyx":85
+ *             while i > 0 and pos <= self.starts[i]:
+ *                 i -= 1
+ *             while True:             # <<<<<<<<<<<<<<
+ *                 if self.ends[i].covered_end >= pos:
+ *                     if i > 0:
+ */
+    while (1) {
+
+      /* "sortedintersect/sintersect.pyx":86
+ *                 i -= 1
+ *             while True:
+ *                 if self.ends[i].covered_end >= pos:             # <<<<<<<<<<<<<<
+ *                     if i > 0:
+ *                         i -= 1
+ */
+      __pyx_t_2 = (((__pyx_v_self->ends[__pyx_v_i]).covered_end >= __pyx_v_pos) != 0);
+      if (__pyx_t_2) {
+
+        /* "sortedintersect/sintersect.pyx":87
+ *             while True:
+ *                 if self.ends[i].covered_end >= pos:
+ *                     if i > 0:             # <<<<<<<<<<<<<<
+ *                         i -= 1
+ *                     else:
+ */
+        __pyx_t_2 = ((__pyx_v_i > 0) != 0);
+        if (__pyx_t_2) {
+
+          /* "sortedintersect/sintersect.pyx":88
+ *                 if self.ends[i].covered_end >= pos:
+ *                     if i > 0:
+ *                         i -= 1             # <<<<<<<<<<<<<<
+ *                     else:
+ *                         break
+ */
+          __pyx_v_i = (__pyx_v_i - 1);
+
+          /* "sortedintersect/sintersect.pyx":87
+ *             while True:
+ *                 if self.ends[i].covered_end >= pos:
+ *                     if i > 0:             # <<<<<<<<<<<<<<
+ *                         i -= 1
+ *                     else:
+ */
+          goto __pyx_L11;
+        }
+
+        /* "sortedintersect/sintersect.pyx":90
+ *                         i -= 1
+ *                     else:
+ *                         break             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     if i < self.ends.size() - 1:
+ */
+        /*else*/ {
+          goto __pyx_L9_break;
+        }
+        __pyx_L11:;
+
+        /* "sortedintersect/sintersect.pyx":86
+ *                 i -= 1
+ *             while True:
+ *                 if self.ends[i].covered_end >= pos:             # <<<<<<<<<<<<<<
+ *                     if i > 0:
+ *                         i -= 1
+ */
+        goto __pyx_L10;
+      }
+
+      /* "sortedintersect/sintersect.pyx":92
+ *                         break
+ *                 else:
+ *                     if i < self.ends.size() - 1:             # <<<<<<<<<<<<<<
+ *                         i += 1
+ *                     break
+ */
+      /*else*/ {
+        __pyx_t_2 = ((__pyx_v_i < (__pyx_v_self->ends.size() - 1)) != 0);
+        if (__pyx_t_2) {
+
+          /* "sortedintersect/sintersect.pyx":93
+ *                 else:
+ *                     if i < self.ends.size() - 1:
+ *                         i += 1             # <<<<<<<<<<<<<<
+ *                     break
+ *             self.index = i
+ */
+          __pyx_v_i = (__pyx_v_i + 1);
+
+          /* "sortedintersect/sintersect.pyx":92
+ *                         break
+ *                 else:
+ *                     if i < self.ends.size() - 1:             # <<<<<<<<<<<<<<
+ *                         i += 1
+ *                     break
+ */
+        }
+
+        /* "sortedintersect/sintersect.pyx":94
+ *                     if i < self.ends.size() - 1:
+ *                         i += 1
+ *                     break             # <<<<<<<<<<<<<<
+ *             self.index = i
+ *         else:
+ */
+        goto __pyx_L9_break;
+      }
+      __pyx_L10:;
+    }
+    __pyx_L9_break:;
+
+    /* "sortedintersect/sintersect.pyx":95
+ *                         i += 1
+ *                     break
+ *             self.index = i             # <<<<<<<<<<<<<<
+ *         else:
+ *             i = self.index
+ */
+    __pyx_v_self->index = __pyx_v_i;
+
+    /* "sortedintersect/sintersect.pyx":81
+ *         cdef size_t i
+ *         before = self.index
+ *         if pos < self.last_q_start:             # <<<<<<<<<<<<<<
+ *             i = self.index
+ *             while i > 0 and pos <= self.starts[i]:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "sortedintersect/sintersect.pyx":97
+ *             self.index = i
+ *         else:
+ *             i = self.index             # <<<<<<<<<<<<<<
+ *             while i < self.ends.size() and pos > self.ends[i].end:
+ *                 i += 1
+ */
+  /*else*/ {
+    __pyx_t_1 = __pyx_v_self->index;
+    __pyx_v_i = __pyx_t_1;
+
+    /* "sortedintersect/sintersect.pyx":98
+ *         else:
+ *             i = self.index
+ *             while i < self.ends.size() and pos > self.ends[i].end:             # <<<<<<<<<<<<<<
+ *                 i += 1
+ *             self.index = i
+ */
+    while (1) {
+      __pyx_t_3 = ((__pyx_v_i < __pyx_v_self->ends.size()) != 0);
+      if (__pyx_t_3) {
+      } else {
+        __pyx_t_2 = __pyx_t_3;
+        goto __pyx_L15_bool_binop_done;
+      }
+      __pyx_t_3 = ((__pyx_v_pos > (__pyx_v_self->ends[__pyx_v_i]).end) != 0);
+      __pyx_t_2 = __pyx_t_3;
+      __pyx_L15_bool_binop_done:;
+      if (!__pyx_t_2) break;
+
+      /* "sortedintersect/sintersect.pyx":99
+ *             i = self.index
+ *             while i < self.ends.size() and pos > self.ends[i].end:
+ *                 i += 1             # <<<<<<<<<<<<<<
+ *             self.index = i
+ * 
+ */
+      __pyx_v_i = (__pyx_v_i + 1);
+    }
+
+    /* "sortedintersect/sintersect.pyx":100
+ *             while i < self.ends.size() and pos > self.ends[i].end:
+ *                 i += 1
+ *             self.index = i             # <<<<<<<<<<<<<<
+ * 
+ *     cdef void _binary_search(self, int pos):
+ */
+    __pyx_v_self->index = __pyx_v_i;
+  }
+  __pyx_L3:;
+
+  /* "sortedintersect/sintersect.pyx":78
+ *                 self.data.append(item[2])
+ * 
+ *     cdef void _line_scan(self, int pos):             # <<<<<<<<<<<<<<
+ *         cdef size_t i
+ *         before = self.index
+ */
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "sortedintersect/sintersect.pyx":102
+ *             self.index = i
+ * 
+ *     cdef void _binary_search(self, int pos):             # <<<<<<<<<<<<<<
+ *         lower = upper_bound(self.starts.begin(), self.starts.end(), pos)
+ *         self.index = lower - self.starts.begin()
+ */
+
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__binary_search(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos) {
+  std::vector<int> ::iterator __pyx_v_lower;
+  __Pyx_RefNannyDeclarations
+  size_t __pyx_t_1;
+  int __pyx_t_2;
+  __Pyx_RefNannySetupContext("_binary_search", 0);
+
+  /* "sortedintersect/sintersect.pyx":103
+ * 
+ *     cdef void _binary_search(self, int pos):
+ *         lower = upper_bound(self.starts.begin(), self.starts.end(), pos)             # <<<<<<<<<<<<<<
+ *         self.index = lower - self.starts.begin()
+ *         self.index = self.index - 1 if self.index else self.index
+ */
+  __pyx_v_lower = std::upper_bound<std::vector<int> ::iterator,int>(__pyx_v_self->starts.begin(), __pyx_v_self->starts.end(), __pyx_v_pos);
+
+  /* "sortedintersect/sintersect.pyx":104
+ *     cdef void _binary_search(self, int pos):
+ *         lower = upper_bound(self.starts.begin(), self.starts.end(), pos)
+ *         self.index = lower - self.starts.begin()             # <<<<<<<<<<<<<<
+ *         self.index = self.index - 1 if self.index else self.index
+ *         while True:
+ */
+  __pyx_v_self->index = (__pyx_v_lower - __pyx_v_self->starts.begin());
+
+  /* "sortedintersect/sintersect.pyx":105
+ *         lower = upper_bound(self.starts.begin(), self.starts.end(), pos)
+ *         self.index = lower - self.starts.begin()
+ *         self.index = self.index - 1 if self.index else self.index             # <<<<<<<<<<<<<<
+ *         while True:
+ *             if self.ends[self.index].covered_end >= pos:
+ */
+  if ((__pyx_v_self->index != 0)) {
+    __pyx_t_1 = (__pyx_v_self->index - 1);
+  } else {
+    __pyx_t_1 = __pyx_v_self->index;
+  }
+  __pyx_v_self->index = __pyx_t_1;
+
+  /* "sortedintersect/sintersect.pyx":106
+ *         self.index = lower - self.starts.begin()
+ *         self.index = self.index - 1 if self.index else self.index
+ *         while True:             # <<<<<<<<<<<<<<
+ *             if self.ends[self.index].covered_end >= pos:
+ *                 if self.index > 0:
+ */
+  while (1) {
+
+    /* "sortedintersect/sintersect.pyx":107
+ *         self.index = self.index - 1 if self.index else self.index
+ *         while True:
+ *             if self.ends[self.index].covered_end >= pos:             # <<<<<<<<<<<<<<
+ *                 if self.index > 0:
+ *                     self.index -= 1
+ */
+    __pyx_t_2 = (((__pyx_v_self->ends[__pyx_v_self->index]).covered_end >= __pyx_v_pos) != 0);
+    if (__pyx_t_2) {
+
+      /* "sortedintersect/sintersect.pyx":108
+ *         while True:
+ *             if self.ends[self.index].covered_end >= pos:
+ *                 if self.index > 0:             # <<<<<<<<<<<<<<
+ *                     self.index -= 1
+ *                 else:
+ */
+      __pyx_t_2 = ((__pyx_v_self->index > 0) != 0);
+      if (__pyx_t_2) {
+
+        /* "sortedintersect/sintersect.pyx":109
+ *             if self.ends[self.index].covered_end >= pos:
+ *                 if self.index > 0:
+ *                     self.index -= 1             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     break
+ */
+        __pyx_v_self->index = (__pyx_v_self->index - 1);
+
+        /* "sortedintersect/sintersect.pyx":108
+ *         while True:
+ *             if self.ends[self.index].covered_end >= pos:
+ *                 if self.index > 0:             # <<<<<<<<<<<<<<
+ *                     self.index -= 1
+ *                 else:
+ */
+        goto __pyx_L6;
+      }
+
+      /* "sortedintersect/sintersect.pyx":111
+ *                     self.index -= 1
+ *                 else:
+ *                     break             # <<<<<<<<<<<<<<
+ *             else:
+ *                 if self.index < self.ends.size() - 1:
+ */
+      /*else*/ {
+        goto __pyx_L4_break;
+      }
+      __pyx_L6:;
+
+      /* "sortedintersect/sintersect.pyx":107
+ *         self.index = self.index - 1 if self.index else self.index
+ *         while True:
+ *             if self.ends[self.index].covered_end >= pos:             # <<<<<<<<<<<<<<
+ *                 if self.index > 0:
+ *                     self.index -= 1
+ */
+      goto __pyx_L5;
+    }
+
+    /* "sortedintersect/sintersect.pyx":113
+ *                     break
+ *             else:
+ *                 if self.index < self.ends.size() - 1:             # <<<<<<<<<<<<<<
+ *                     self.index += 1
+ *                 break
+ */
+    /*else*/ {
+      __pyx_t_2 = ((__pyx_v_self->index < (__pyx_v_self->ends.size() - 1)) != 0);
+      if (__pyx_t_2) {
+
+        /* "sortedintersect/sintersect.pyx":114
+ *             else:
+ *                 if self.index < self.ends.size() - 1:
+ *                     self.index += 1             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+        __pyx_v_self->index = (__pyx_v_self->index + 1);
+
+        /* "sortedintersect/sintersect.pyx":113
+ *                     break
+ *             else:
+ *                 if self.index < self.ends.size() - 1:             # <<<<<<<<<<<<<<
+ *                     self.index += 1
+ *                 break
+ */
+      }
+
+      /* "sortedintersect/sintersect.pyx":115
+ *                 if self.index < self.ends.size() - 1:
+ *                     self.index += 1
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *         # if pos >= self.last_q_start:
+ */
+      goto __pyx_L4_break;
+    }
+    __pyx_L5:;
+  }
+  __pyx_L4_break:;
+
+  /* "sortedintersect/sintersect.pyx":102
+ *             self.index = i
+ * 
+ *     cdef void _binary_search(self, int pos):             # <<<<<<<<<<<<<<
+ *         lower = upper_bound(self.starts.begin(), self.starts.end(), pos)
+ *         self.index = lower - self.starts.begin()
+ */
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "sortedintersect/sintersect.pyx":128
+ *         #                 self.index += 1
+ *         #             break
+ *     cdef void _set_reference_index(self, int pos):             # <<<<<<<<<<<<<<
+ *         # self._binary_search(pos)
+ *         # if self.query_sorted:
+ */
+
+static void __pyx_f_15sortedintersect_10sintersect_11IntervalSet__set_reference_index(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos) {
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_set_reference_index", 0);
+
+  /* "sortedintersect/sintersect.pyx":133
+ *         #     self._line_scan(pos)
+ *         # else:
+ *         if abs(pos - self.last_q_start) > self.distance_threshold:             # <<<<<<<<<<<<<<
+ *             self._binary_search(pos)
+ *         else:
+ */
+  __pyx_t_1 = abs((__pyx_v_pos - __pyx_v_self->last_q_start)); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = ((__pyx_t_1 > __pyx_v_self->distance_threshold) != 0);
+  if (__pyx_t_2) {
+
+    /* "sortedintersect/sintersect.pyx":134
+ *         # else:
+ *         if abs(pos - self.last_q_start) > self.distance_threshold:
+ *             self._binary_search(pos)             # <<<<<<<<<<<<<<
+ *         else:
+ *             self._line_scan(pos)
+ */
+    ((struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self->__pyx_vtab)->_binary_search(__pyx_v_self, __pyx_v_pos);
+
+    /* "sortedintersect/sintersect.pyx":133
+ *         #     self._line_scan(pos)
+ *         # else:
+ *         if abs(pos - self.last_q_start) > self.distance_threshold:             # <<<<<<<<<<<<<<
+ *             self._binary_search(pos)
+ *         else:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "sortedintersect/sintersect.pyx":136
+ *             self._binary_search(pos)
+ *         else:
+ *             self._line_scan(pos)             # <<<<<<<<<<<<<<
+ *     cpdef search_point(self, int pos):
+ *         """Search for reference intervals overlapping single query point
+ */
+  /*else*/ {
+    ((struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self->__pyx_vtab)->_line_scan(__pyx_v_self, __pyx_v_pos);
+  }
+  __pyx_L3:;
+
+  /* "sortedintersect/sintersect.pyx":128
+ *         #                 self.index += 1
+ *         #             break
+ *     cdef void _set_reference_index(self, int pos):             # <<<<<<<<<<<<<<
+ *         # self._binary_search(pos)
+ *         # if self.query_sorted:
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("sortedintersect.sintersect.IntervalSet._set_reference_index", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "sortedintersect/sintersect.pyx":137
+ *         else:
+ *             self._line_scan(pos)
  *     cpdef search_point(self, int pos):             # <<<<<<<<<<<<<<
+ *         """Search for reference intervals overlapping single query point
  * 
- *         cdef uint64_t i = self.index
  */
 
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_7search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos); /*proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_search_point(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_pos, int __pyx_skip_dispatch) {
-  uint64_t __pyx_v_i;
-  int __pyx_v_passed;
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_9search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos); /*proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_point(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos, int __pyx_skip_dispatch) {
+  size_t __pyx_v_size;
+  size_t __pyx_v_i;
+  PyObject *__pyx_v_found = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  int __pyx_t_7;
-  int __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_UCS4 __pyx_t_10;
+  size_t __pyx_t_7;
+  size_t __pyx_t_8;
+  size_t __pyx_t_9;
+  int __pyx_t_10;
+  int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search_point", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_search_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_search_point); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_9intersect_4ISet_7search_point)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_9search_point)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2563,15 +3505,15 @@
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_4, function);
           }
         }
         __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -2584,563 +3526,434 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "sortedintersect/intersect.pyx":64
- *     cpdef search_point(self, int pos):
- * 
- *         cdef uint64_t i = self.index             # <<<<<<<<<<<<<<
- * 
- *         if self.starts.size() == 0 or i >= self.starts.size():
+  /* "sortedintersect/sintersect.pyx":143
+ *         :type pos: int
+ *         """
+ *         cdef size_t size = self.ends.size()             # <<<<<<<<<<<<<<
+ *         cdef size_t i
+ *         if size == 0:
+ */
+  __pyx_v_size = __pyx_v_self->ends.size();
+
+  /* "sortedintersect/sintersect.pyx":145
+ *         cdef size_t size = self.ends.size()
+ *         cdef size_t i
+ *         if size == 0:             # <<<<<<<<<<<<<<
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(pos)
  */
-  __pyx_t_6 = __pyx_v_self->index;
-  __pyx_v_i = __pyx_t_6;
-
-  /* "sortedintersect/intersect.pyx":66
- *         cdef uint64_t i = self.index
- * 
- *         if self.starts.size() == 0 or i >= self.starts.size():             # <<<<<<<<<<<<<<
- *             return False
- * 
- */
-  __pyx_t_8 = ((__pyx_v_self->starts.size() == 0) != 0);
-  if (!__pyx_t_8) {
-  } else {
-    __pyx_t_7 = __pyx_t_8;
-    goto __pyx_L4_bool_binop_done;
-  }
-  __pyx_t_8 = ((__pyx_v_i >= __pyx_v_self->starts.size()) != 0);
-  __pyx_t_7 = __pyx_t_8;
-  __pyx_L4_bool_binop_done:;
-  if (__pyx_t_7) {
+  __pyx_t_6 = ((__pyx_v_size == 0) != 0);
+  if (__pyx_t_6) {
 
-    /* "sortedintersect/intersect.pyx":67
- * 
- *         if self.starts.size() == 0 or i >= self.starts.size():
- *             return False             # <<<<<<<<<<<<<<
- * 
- *         if pos < self.last_q_start:
+    /* "sortedintersect/sintersect.pyx":146
+ *         cdef size_t i
+ *         if size == 0:
+ *             return False if self.bool_only else []             # <<<<<<<<<<<<<<
+ *         self._set_reference_index(pos)
+ *         self.last_q_start = pos
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(Py_False);
-    __pyx_r = Py_False;
+    if ((__pyx_v_self->bool_only != 0)) {
+      __Pyx_INCREF(Py_False);
+      __pyx_t_1 = Py_False;
+    } else {
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = __pyx_t_2;
+      __pyx_t_2 = 0;
+    }
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "sortedintersect/intersect.pyx":66
- *         cdef uint64_t i = self.index
- * 
- *         if self.starts.size() == 0 or i >= self.starts.size():             # <<<<<<<<<<<<<<
- *             return False
- * 
+    /* "sortedintersect/sintersect.pyx":145
+ *         cdef size_t size = self.ends.size()
+ *         cdef size_t i
+ *         if size == 0:             # <<<<<<<<<<<<<<
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(pos)
  */
   }
 
-  /* "sortedintersect/intersect.pyx":69
- *             return False
- * 
- *         if pos < self.last_q_start:             # <<<<<<<<<<<<<<
- *             raise ValueError(f'Position {pos} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
- */
-  __pyx_t_7 = ((__pyx_v_pos < __pyx_v_self->last_q_start) != 0);
-  if (unlikely(__pyx_t_7)) {
-
-    /* "sortedintersect/intersect.pyx":70
- * 
- *         if pos < self.last_q_start:
- *             raise ValueError(f'Position {pos} is not in sorted order, last query interval seen was {self.last_q_start}')             # <<<<<<<<<<<<<<
- * 
- *         cdef bint passed = False
- */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = 0;
-    __pyx_t_10 = 127;
-    __Pyx_INCREF(__pyx_kp_u_Position);
-    __pyx_t_9 += 9;
-    __Pyx_GIVEREF(__pyx_kp_u_Position);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Position);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_pos, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __Pyx_INCREF(__pyx_kp_u_is_not_in_sorted_order_last_que);
-    __pyx_t_9 += 54;
-    __Pyx_GIVEREF(__pyx_kp_u_is_not_in_sorted_order_last_que);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_is_not_in_sorted_order_last_que);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_q_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 70, __pyx_L1_error)
-
-    /* "sortedintersect/intersect.pyx":69
- *             return False
- * 
- *         if pos < self.last_q_start:             # <<<<<<<<<<<<<<
- *             raise ValueError(f'Position {pos} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
- */
-  }
-
-  /* "sortedintersect/intersect.pyx":72
- *             raise ValueError(f'Position {pos} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
- *         cdef bint passed = False             # <<<<<<<<<<<<<<
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]
- */
-  __pyx_v_passed = 0;
-
-  /* "sortedintersect/intersect.pyx":73
- * 
- *         cdef bint passed = False
- *         self.current_r_start = self.starts[i]             # <<<<<<<<<<<<<<
- *         self.current_r_end = self.ends[i]
- *         self.last_q_start = pos
- */
-  __pyx_v_self->current_r_start = (__pyx_v_self->starts[__pyx_v_i]);
-
-  /* "sortedintersect/intersect.pyx":74
- *         cdef bint passed = False
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]             # <<<<<<<<<<<<<<
+  /* "sortedintersect/sintersect.pyx":147
+ *         if size == 0:
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(pos)             # <<<<<<<<<<<<<<
  *         self.last_q_start = pos
- *         if pos > self.current_r_end:
+ *         if not self.bool_only:
  */
-  __pyx_v_self->current_r_end = (__pyx_v_self->ends[__pyx_v_i]);
+  ((struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self->__pyx_vtab)->_set_reference_index(__pyx_v_self, __pyx_v_pos);
 
-  /* "sortedintersect/intersect.pyx":75
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]
+  /* "sortedintersect/sintersect.pyx":148
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(pos)
  *         self.last_q_start = pos             # <<<<<<<<<<<<<<
- *         if pos > self.current_r_end:
- *             i += 1
+ *         if not self.bool_only:
+ *             found = []
  */
   __pyx_v_self->last_q_start = __pyx_v_pos;
 
-  /* "sortedintersect/intersect.pyx":76
- *         self.current_r_end = self.ends[i]
+  /* "sortedintersect/sintersect.pyx":149
+ *         self._set_reference_index(pos)
  *         self.last_q_start = pos
- *         if pos > self.current_r_end:             # <<<<<<<<<<<<<<
- *             i += 1
- *             while i < self.starts.size():
+ *         if not self.bool_only:             # <<<<<<<<<<<<<<
+ *             found = []
+ *             for i in range(self.index, size):
  */
-  __pyx_t_7 = ((__pyx_v_pos > __pyx_v_self->current_r_end) != 0);
-  if (__pyx_t_7) {
+  __pyx_t_6 = ((!(__pyx_v_self->bool_only != 0)) != 0);
+  if (__pyx_t_6) {
 
-    /* "sortedintersect/intersect.pyx":77
+    /* "sortedintersect/sintersect.pyx":150
  *         self.last_q_start = pos
- *         if pos > self.current_r_end:
- *             i += 1             # <<<<<<<<<<<<<<
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]
- */
-    __pyx_v_i = (__pyx_v_i + 1);
-
-    /* "sortedintersect/intersect.pyx":78
- *         if pos > self.current_r_end:
- *             i += 1
- *             while i < self.starts.size():             # <<<<<<<<<<<<<<
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
+ *         if not self.bool_only:
+ *             found = []             # <<<<<<<<<<<<<<
+ *             for i in range(self.index, size):
+ *                 if self.starts[i] <= pos <= self.ends[i].end:
  */
-    while (1) {
-      __pyx_t_7 = ((__pyx_v_i < __pyx_v_self->starts.size()) != 0);
-      if (!__pyx_t_7) break;
-
-      /* "sortedintersect/intersect.pyx":79
- *             i += 1
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]             # <<<<<<<<<<<<<<
- *                 self.current_r_end = self.ends[i]
- *                 if pos < self.current_r_start:
- */
-      __pyx_v_self->current_r_start = (__pyx_v_self->starts[__pyx_v_i]);
-
-      /* "sortedintersect/intersect.pyx":80
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]             # <<<<<<<<<<<<<<
- *                 if pos < self.current_r_start:
- *                     break
- */
-      __pyx_v_self->current_r_end = (__pyx_v_self->ends[__pyx_v_i]);
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_v_found = ((PyObject*)__pyx_t_1);
+    __pyx_t_1 = 0;
 
-      /* "sortedintersect/intersect.pyx":81
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
- *                 if pos < self.current_r_start:             # <<<<<<<<<<<<<<
- *                     break
- *                 elif self.current_r_start <= pos <= self.current_r_end:
- */
-      __pyx_t_7 = ((__pyx_v_pos < __pyx_v_self->current_r_start) != 0);
-      if (__pyx_t_7) {
+    /* "sortedintersect/sintersect.pyx":151
+ *         if not self.bool_only:
+ *             found = []
+ *             for i in range(self.index, size):             # <<<<<<<<<<<<<<
+ *                 if self.starts[i] <= pos <= self.ends[i].end:
+ *                     if self.add_data:
+ */
+    __pyx_t_7 = __pyx_v_size;
+    __pyx_t_8 = __pyx_t_7;
+    for (__pyx_t_9 = __pyx_v_self->index; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
+      __pyx_v_i = __pyx_t_9;
+
+      /* "sortedintersect/sintersect.pyx":152
+ *             found = []
+ *             for i in range(self.index, size):
+ *                 if self.starts[i] <= pos <= self.ends[i].end:             # <<<<<<<<<<<<<<
+ *                     if self.add_data:
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ */
+      __pyx_t_6 = ((__pyx_v_self->starts[__pyx_v_i]) <= __pyx_v_pos);
+      if (__pyx_t_6) {
+        __pyx_t_6 = (__pyx_v_pos <= (__pyx_v_self->ends[__pyx_v_i]).end);
+      }
+      __pyx_t_10 = (__pyx_t_6 != 0);
+      if (__pyx_t_10) {
 
-        /* "sortedintersect/intersect.pyx":82
- *                 self.current_r_end = self.ends[i]
- *                 if pos < self.current_r_start:
- *                     break             # <<<<<<<<<<<<<<
- *                 elif self.current_r_start <= pos <= self.current_r_end:
- *                     passed = True
- */
-        goto __pyx_L9_break;
+        /* "sortedintersect/sintersect.pyx":153
+ *             for i in range(self.index, size):
+ *                 if self.starts[i] <= pos <= self.ends[i].end:
+ *                     if self.add_data:             # <<<<<<<<<<<<<<
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                     else:
+ */
+        __pyx_t_10 = (__pyx_v_self->add_data != 0);
+        if (__pyx_t_10) {
+
+          /* "sortedintersect/sintersect.pyx":154
+ *                 if self.starts[i] <= pos <= self.ends[i].end:
+ *                     if self.add_data:
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))             # <<<<<<<<<<<<<<
+ *                     else:
+ *                         found.append((self.starts[i], self.ends[i].end))
+ */
+          __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->starts[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_self->ends[__pyx_v_i]).end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          if (unlikely(__pyx_v_self->data == Py_None)) {
+            PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+            __PYX_ERR(0, 154, __pyx_L1_error)
+          }
+          __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __Pyx_GIVEREF(__pyx_t_1);
+          PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+          __Pyx_GIVEREF(__pyx_t_2);
+          PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
+          __Pyx_INCREF(PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+          __Pyx_GIVEREF(PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+          PyTuple_SET_ITEM(__pyx_t_4, 2, PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+          __pyx_t_1 = 0;
+          __pyx_t_2 = 0;
+          __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_found, __pyx_t_4); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 154, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "sortedintersect/intersect.pyx":81
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
- *                 if pos < self.current_r_start:             # <<<<<<<<<<<<<<
+          /* "sortedintersect/sintersect.pyx":153
+ *             for i in range(self.index, size):
+ *                 if self.starts[i] <= pos <= self.ends[i].end:
+ *                     if self.add_data:             # <<<<<<<<<<<<<<
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                     else:
+ */
+          goto __pyx_L8;
+        }
+
+        /* "sortedintersect/sintersect.pyx":156
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                     else:
+ *                         found.append((self.starts[i], self.ends[i].end))             # <<<<<<<<<<<<<<
+ *                     # found.append(i)
+ *                     continue
+ */
+        /*else*/ {
+          __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_self->starts[__pyx_v_i])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_self->ends[__pyx_v_i]).end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_GIVEREF(__pyx_t_4);
+          PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
+          __Pyx_GIVEREF(__pyx_t_2);
+          PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+          __pyx_t_4 = 0;
+          __pyx_t_2 = 0;
+          __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_found, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        }
+        __pyx_L8:;
+
+        /* "sortedintersect/sintersect.pyx":158
+ *                         found.append((self.starts[i], self.ends[i].end))
+ *                     # found.append(i)
+ *                     continue             # <<<<<<<<<<<<<<
+ *                 elif pos < self.starts[i] or pos > self.ends[i].covered_end:
  *                     break
- *                 elif self.current_r_start <= pos <= self.current_r_end:
  */
-      }
+        goto __pyx_L5_continue;
 
-      /* "sortedintersect/intersect.pyx":83
- *                 if pos < self.current_r_start:
- *                     break
- *                 elif self.current_r_start <= pos <= self.current_r_end:             # <<<<<<<<<<<<<<
- *                     passed = True
- *                     break
+        /* "sortedintersect/sintersect.pyx":152
+ *             found = []
+ *             for i in range(self.index, size):
+ *                 if self.starts[i] <= pos <= self.ends[i].end:             # <<<<<<<<<<<<<<
+ *                     if self.add_data:
+ *                         found.append((self.starts[i], self.ends[i].end, self.data[i]))
  */
-      __pyx_t_7 = (__pyx_v_self->current_r_start <= __pyx_v_pos);
-      if (__pyx_t_7) {
-        __pyx_t_7 = (__pyx_v_pos <= __pyx_v_self->current_r_end);
       }
-      __pyx_t_8 = (__pyx_t_7 != 0);
-      if (__pyx_t_8) {
 
-        /* "sortedintersect/intersect.pyx":84
- *                     break
- *                 elif self.current_r_start <= pos <= self.current_r_end:
- *                     passed = True             # <<<<<<<<<<<<<<
+      /* "sortedintersect/sintersect.pyx":159
+ *                     # found.append(i)
+ *                     continue
+ *                 elif pos < self.starts[i] or pos > self.ends[i].covered_end:             # <<<<<<<<<<<<<<
  *                     break
- *                 i += 1
+ *             return found
  */
-        __pyx_v_passed = 1;
-
-        /* "sortedintersect/intersect.pyx":85
- *                 elif self.current_r_start <= pos <= self.current_r_end:
- *                     passed = True
+      __pyx_t_6 = ((__pyx_v_pos < (__pyx_v_self->starts[__pyx_v_i])) != 0);
+      if (!__pyx_t_6) {
+      } else {
+        __pyx_t_10 = __pyx_t_6;
+        goto __pyx_L9_bool_binop_done;
+      }
+      __pyx_t_6 = ((__pyx_v_pos > (__pyx_v_self->ends[__pyx_v_i]).covered_end) != 0);
+      __pyx_t_10 = __pyx_t_6;
+      __pyx_L9_bool_binop_done:;
+      if (__pyx_t_10) {
+
+        /* "sortedintersect/sintersect.pyx":160
+ *                     continue
+ *                 elif pos < self.starts[i] or pos > self.ends[i].covered_end:
  *                     break             # <<<<<<<<<<<<<<
- *                 i += 1
- *             self.index = i
+ *             return found
+ *         else:
  */
-        goto __pyx_L9_break;
+        goto __pyx_L6_break;
 
-        /* "sortedintersect/intersect.pyx":83
- *                 if pos < self.current_r_start:
- *                     break
- *                 elif self.current_r_start <= pos <= self.current_r_end:             # <<<<<<<<<<<<<<
- *                     passed = True
+        /* "sortedintersect/sintersect.pyx":159
+ *                     # found.append(i)
+ *                     continue
+ *                 elif pos < self.starts[i] or pos > self.ends[i].covered_end:             # <<<<<<<<<<<<<<
  *                     break
+ *             return found
  */
       }
-
-      /* "sortedintersect/intersect.pyx":86
- *                     passed = True
- *                     break
- *                 i += 1             # <<<<<<<<<<<<<<
- *             self.index = i
- * 
- */
-      __pyx_v_i = (__pyx_v_i + 1);
+      __pyx_L5_continue:;
     }
-    __pyx_L9_break:;
+    __pyx_L6_break:;
 
-    /* "sortedintersect/intersect.pyx":87
+    /* "sortedintersect/sintersect.pyx":161
+ *                 elif pos < self.starts[i] or pos > self.ends[i].covered_end:
  *                     break
- *                 i += 1
- *             self.index = i             # <<<<<<<<<<<<<<
- * 
- *         elif self.current_r_start <= pos <= self.current_r_end:
+ *             return found             # <<<<<<<<<<<<<<
+ *         else:
+ *             return False if self.index >= size else self.starts[self.index] <= pos <= self.ends[self.index].end
  */
-    __pyx_v_self->index = __pyx_v_i;
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_v_found);
+    __pyx_r = __pyx_v_found;
+    goto __pyx_L0;
 
-    /* "sortedintersect/intersect.pyx":76
- *         self.current_r_end = self.ends[i]
+    /* "sortedintersect/sintersect.pyx":149
+ *         self._set_reference_index(pos)
  *         self.last_q_start = pos
- *         if pos > self.current_r_end:             # <<<<<<<<<<<<<<
- *             i += 1
- *             while i < self.starts.size():
- */
-    goto __pyx_L7;
-  }
-
-  /* "sortedintersect/intersect.pyx":89
- *             self.index = i
- * 
- *         elif self.current_r_start <= pos <= self.current_r_end:             # <<<<<<<<<<<<<<
- *             passed = True
- * 
+ *         if not self.bool_only:             # <<<<<<<<<<<<<<
+ *             found = []
+ *             for i in range(self.index, size):
  */
-  __pyx_t_8 = (__pyx_v_self->current_r_start <= __pyx_v_pos);
-  if (__pyx_t_8) {
-    __pyx_t_8 = (__pyx_v_pos <= __pyx_v_self->current_r_end);
   }
-  __pyx_t_7 = (__pyx_t_8 != 0);
-  if (__pyx_t_7) {
-
-    /* "sortedintersect/intersect.pyx":90
- * 
- *         elif self.current_r_start <= pos <= self.current_r_end:
- *             passed = True             # <<<<<<<<<<<<<<
- * 
- *         if passed:
- */
-    __pyx_v_passed = 1;
 
-    /* "sortedintersect/intersect.pyx":89
- *             self.index = i
- * 
- *         elif self.current_r_start <= pos <= self.current_r_end:             # <<<<<<<<<<<<<<
- *             passed = True
- * 
- */
-  }
-  __pyx_L7:;
-
-  /* "sortedintersect/intersect.pyx":92
- *             passed = True
- * 
- *         if passed:             # <<<<<<<<<<<<<<
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- */
-  __pyx_t_7 = (__pyx_v_passed != 0);
-  if (__pyx_t_7) {
-
-    /* "sortedintersect/intersect.pyx":93
+  /* "sortedintersect/sintersect.pyx":163
+ *             return found
+ *         else:
+ *             return False if self.index >= size else self.starts[self.index] <= pos <= self.ends[self.index].end             # <<<<<<<<<<<<<<
  * 
- *         if passed:
- *             if self.add_data:             # <<<<<<<<<<<<<<
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
- */
-    __pyx_t_7 = (__pyx_v_self->add_data != 0);
-    if (__pyx_t_7) {
-
-      /* "sortedintersect/intersect.pyx":94
- *         if passed:
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]             # <<<<<<<<<<<<<<
- *             return self.current_r_start, self.current_r_end
- *         return False
+ *     cpdef search_interval(self, int start, int end):
  */
-      __Pyx_XDECREF(__pyx_r);
-      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    if (((__pyx_v_self->index >= __pyx_v_size) != 0)) {
+      __Pyx_INCREF(Py_False);
+      __pyx_t_1 = Py_False;
+    } else {
+      __pyx_t_10 = ((__pyx_v_self->starts[__pyx_v_self->index]) <= __pyx_v_pos);
+      if (__pyx_t_10) {
+        __pyx_t_10 = (__pyx_v_pos <= (__pyx_v_self->ends[__pyx_v_self->index]).end);
+      }
+      __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_self->data, __pyx_v_self->index, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-      __Pyx_GIVEREF(__pyx_t_2);
-      PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_4);
-      __pyx_t_1 = 0;
+      __pyx_t_1 = __pyx_t_2;
       __pyx_t_2 = 0;
-      __pyx_t_4 = 0;
-      __pyx_r = __pyx_t_3;
-      __pyx_t_3 = 0;
-      goto __pyx_L0;
-
-      /* "sortedintersect/intersect.pyx":93
- * 
- *         if passed:
- *             if self.add_data:             # <<<<<<<<<<<<<<
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
- */
     }
-
-    /* "sortedintersect/intersect.pyx":95
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end             # <<<<<<<<<<<<<<
- *         return False
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
-    __pyx_t_3 = 0;
-    __pyx_t_4 = 0;
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
     goto __pyx_L0;
-
-    /* "sortedintersect/intersect.pyx":92
- *             passed = True
- * 
- *         if passed:             # <<<<<<<<<<<<<<
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- */
   }
 
-  /* "sortedintersect/intersect.pyx":96
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
- *         return False             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(Py_False);
-  __pyx_r = Py_False;
-  goto __pyx_L0;
-
-  /* "sortedintersect/intersect.pyx":62
- *                 self.data.append(item[2])
- * 
+  /* "sortedintersect/sintersect.pyx":137
+ *         else:
+ *             self._line_scan(pos)
  *     cpdef search_point(self, int pos):             # <<<<<<<<<<<<<<
+ *         """Search for reference intervals overlapping single query point
  * 
- *         cdef uint64_t i = self.index
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_found);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_7search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_7search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_9search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos); /*proto*/
+static char __pyx_doc_15sortedintersect_10sintersect_11IntervalSet_8search_point[] = "Search for reference intervals overlapping single query point\n\n        :param pos: The position to search for overlaps\n        :type pos: int\n        ";
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_9search_point(PyObject *__pyx_v_self, PyObject *__pyx_arg_pos) {
   int __pyx_v_pos;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("search_point (wrapper)", 0);
   assert(__pyx_arg_pos); {
-    __pyx_v_pos = __Pyx_PyInt_As_int(__pyx_arg_pos); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+    __pyx_v_pos = __Pyx_PyInt_As_int(__pyx_arg_pos); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 137, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_6search_point(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), ((int)__pyx_v_pos));
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_8search_point(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), ((int)__pyx_v_pos));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_6search_point(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_pos) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_8search_point(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_pos) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search_point", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_15sortedintersect_9intersect_4ISet_search_point(__pyx_v_self, __pyx_v_pos, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_point(__pyx_v_self, __pyx_v_pos, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_point", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "sortedintersect/intersect.pyx":99
- * 
+/* "sortedintersect/sintersect.pyx":165
+ *             return False if self.index >= size else self.starts[self.index] <= pos <= self.ends[self.index].end
  * 
  *     cpdef search_interval(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search for reference intervals overlapping single query interval
  * 
- *         cdef uint64_t i = self.index
  */
 
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_9search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_15sortedintersect_9intersect_4ISet_search_interval(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch) {
-  uint64_t __pyx_v_i;
-  int __pyx_v_passed;
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_11search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_interval(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end, int __pyx_skip_dispatch) {
+  size_t __pyx_v_size;
+  size_t __pyx_v_i;
+  PyObject *__pyx_v_found = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
-  int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_UCS4 __pyx_t_12;
+  size_t __pyx_t_10;
+  size_t __pyx_t_11;
+  size_t __pyx_t_12;
+  int __pyx_t_13;
+  int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search_interval", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_search_interval); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_search_interval); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_9intersect_4ISet_9search_interval)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_11search_interval)) {
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -3150,44 +3963,44 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_4};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 99, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 165, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_4);
           PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -3202,472 +4015,323 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "sortedintersect/intersect.pyx":101
- *     cpdef search_interval(self, int start, int end):
- * 
- *         cdef uint64_t i = self.index             # <<<<<<<<<<<<<<
- *         if self.starts.size() == 0 or i >= self.starts.size():
- *             return False
+  /* "sortedintersect/sintersect.pyx":173
+ *         :type end: int
+ *         """
+ *         cdef size_t size = self.ends.size()             # <<<<<<<<<<<<<<
+ *         cdef size_t i
+ *         if size == 0:
+ */
+  __pyx_v_size = __pyx_v_self->ends.size();
+
+  /* "sortedintersect/sintersect.pyx":175
+ *         cdef size_t size = self.ends.size()
+ *         cdef size_t i
+ *         if size == 0:             # <<<<<<<<<<<<<<
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(start)
  */
-  __pyx_t_7 = __pyx_v_self->index;
-  __pyx_v_i = __pyx_t_7;
-
-  /* "sortedintersect/intersect.pyx":102
- * 
- *         cdef uint64_t i = self.index
- *         if self.starts.size() == 0 or i >= self.starts.size():             # <<<<<<<<<<<<<<
- *             return False
- * 
- */
-  __pyx_t_10 = ((__pyx_v_self->starts.size() == 0) != 0);
-  if (!__pyx_t_10) {
-  } else {
-    __pyx_t_9 = __pyx_t_10;
-    goto __pyx_L4_bool_binop_done;
-  }
-  __pyx_t_10 = ((__pyx_v_i >= __pyx_v_self->starts.size()) != 0);
-  __pyx_t_9 = __pyx_t_10;
-  __pyx_L4_bool_binop_done:;
+  __pyx_t_9 = ((__pyx_v_size == 0) != 0);
   if (__pyx_t_9) {
 
-    /* "sortedintersect/intersect.pyx":103
- *         cdef uint64_t i = self.index
- *         if self.starts.size() == 0 or i >= self.starts.size():
- *             return False             # <<<<<<<<<<<<<<
- * 
- *         if start < self.last_q_start:
+    /* "sortedintersect/sintersect.pyx":176
+ *         cdef size_t i
+ *         if size == 0:
+ *             return False if self.bool_only else []             # <<<<<<<<<<<<<<
+ *         self._set_reference_index(start)
+ *         self.last_q_start = start
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(Py_False);
-    __pyx_r = Py_False;
+    if ((__pyx_v_self->bool_only != 0)) {
+      __Pyx_INCREF(Py_False);
+      __pyx_t_1 = Py_False;
+    } else {
+      __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = __pyx_t_2;
+      __pyx_t_2 = 0;
+    }
+    __pyx_r = __pyx_t_1;
+    __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "sortedintersect/intersect.pyx":102
- * 
- *         cdef uint64_t i = self.index
- *         if self.starts.size() == 0 or i >= self.starts.size():             # <<<<<<<<<<<<<<
- *             return False
- * 
- */
-  }
-
-  /* "sortedintersect/intersect.pyx":105
- *             return False
- * 
- *         if start < self.last_q_start:             # <<<<<<<<<<<<<<
- *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
- */
-  __pyx_t_9 = ((__pyx_v_start < __pyx_v_self->last_q_start) != 0);
-  if (unlikely(__pyx_t_9)) {
-
-    /* "sortedintersect/intersect.pyx":106
- * 
- *         if start < self.last_q_start:
- *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last query interval seen was {self.last_q_start}')             # <<<<<<<<<<<<<<
- * 
- *         cdef bint passed = False
- */
-    __pyx_t_1 = PyTuple_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_11 = 0;
-    __pyx_t_12 = 127;
-    __Pyx_INCREF(__pyx_kp_u_Interval);
-    __pyx_t_11 += 9;
-    __Pyx_GIVEREF(__pyx_kp_u_Interval);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Interval);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __Pyx_INCREF(__pyx_kp_u_);
-    __pyx_t_11 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u_);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __Pyx_INCREF(__pyx_kp_u_is_not_in_sorted_order_last_que);
-    __pyx_t_11 += 54;
-    __Pyx_GIVEREF(__pyx_kp_u_is_not_in_sorted_order_last_que);
-    PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_is_not_in_sorted_order_last_que);
-    __pyx_t_2 = __Pyx_PyUnicode_From_int(__pyx_v_self->last_q_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 6, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 106, __pyx_L1_error)
-
-    /* "sortedintersect/intersect.pyx":105
- *             return False
- * 
- *         if start < self.last_q_start:             # <<<<<<<<<<<<<<
- *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
+    /* "sortedintersect/sintersect.pyx":175
+ *         cdef size_t size = self.ends.size()
+ *         cdef size_t i
+ *         if size == 0:             # <<<<<<<<<<<<<<
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(start)
  */
   }
 
-  /* "sortedintersect/intersect.pyx":108
- *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last query interval seen was {self.last_q_start}')
- * 
- *         cdef bint passed = False             # <<<<<<<<<<<<<<
+  /* "sortedintersect/sintersect.pyx":177
+ *         if size == 0:
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(start)             # <<<<<<<<<<<<<<
  *         self.last_q_start = start
- *         self.current_r_start = self.starts[i]
+ *         found = []
  */
-  __pyx_v_passed = 0;
+  ((struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self->__pyx_vtab)->_set_reference_index(__pyx_v_self, __pyx_v_start);
 
-  /* "sortedintersect/intersect.pyx":109
- * 
- *         cdef bint passed = False
+  /* "sortedintersect/sintersect.pyx":178
+ *             return False if self.bool_only else []
+ *         self._set_reference_index(start)
  *         self.last_q_start = start             # <<<<<<<<<<<<<<
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]
+ *         found = []
+ *         for i in range(self.index, size):
  */
   __pyx_v_self->last_q_start = __pyx_v_start;
 
-  /* "sortedintersect/intersect.pyx":110
- *         cdef bint passed = False
+  /* "sortedintersect/sintersect.pyx":179
+ *         self._set_reference_index(start)
  *         self.last_q_start = start
- *         self.current_r_start = self.starts[i]             # <<<<<<<<<<<<<<
- *         self.current_r_end = self.ends[i]
- *         if start > self.current_r_end:
+ *         found = []             # <<<<<<<<<<<<<<
+ *         for i in range(self.index, size):
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):
  */
-  __pyx_v_self->current_r_start = (__pyx_v_self->starts[__pyx_v_i]);
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_found = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "sortedintersect/intersect.pyx":111
+  /* "sortedintersect/sintersect.pyx":180
  *         self.last_q_start = start
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]             # <<<<<<<<<<<<<<
- *         if start > self.current_r_end:
- *             i = self.index + 1
- */
-  __pyx_v_self->current_r_end = (__pyx_v_self->ends[__pyx_v_i]);
-
-  /* "sortedintersect/intersect.pyx":112
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]
- *         if start > self.current_r_end:             # <<<<<<<<<<<<<<
- *             i = self.index + 1
- *             while i < self.starts.size():
+ *         found = []
+ *         for i in range(self.index, size):             # <<<<<<<<<<<<<<
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):
+ *                 if self.bool_only:
+ */
+  __pyx_t_10 = __pyx_v_size;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = __pyx_v_self->index; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
+
+    /* "sortedintersect/sintersect.pyx":181
+ *         found = []
+ *         for i in range(self.index, size):
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):             # <<<<<<<<<<<<<<
+ *                 if self.bool_only:
+ *                     return True
  */
-  __pyx_t_9 = ((__pyx_v_start > __pyx_v_self->current_r_end) != 0);
-  if (__pyx_t_9) {
-
-    /* "sortedintersect/intersect.pyx":113
- *         self.current_r_end = self.ends[i]
- *         if start > self.current_r_end:
- *             i = self.index + 1             # <<<<<<<<<<<<<<
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]
- */
-    __pyx_v_i = (__pyx_v_self->index + 1);
-
-    /* "sortedintersect/intersect.pyx":114
- *         if start > self.current_r_end:
- *             i = self.index + 1
- *             while i < self.starts.size():             # <<<<<<<<<<<<<<
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
- */
-    while (1) {
-      __pyx_t_9 = ((__pyx_v_i < __pyx_v_self->starts.size()) != 0);
-      if (!__pyx_t_9) break;
+    __pyx_t_9 = (__pyx_f_15sortedintersect_10sintersect_is_overlapping(__pyx_v_start, __pyx_v_end, (__pyx_v_self->starts[__pyx_v_i]), (__pyx_v_self->ends[__pyx_v_i]).end) != 0);
+    if (__pyx_t_9) {
 
-      /* "sortedintersect/intersect.pyx":115
- *             i = self.index + 1
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]             # <<<<<<<<<<<<<<
- *                 self.current_r_end = self.ends[i]
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):
- */
-      __pyx_v_self->current_r_start = (__pyx_v_self->starts[__pyx_v_i]);
-
-      /* "sortedintersect/intersect.pyx":116
- *             while i < self.starts.size():
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]             # <<<<<<<<<<<<<<
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):
- *                     passed = True
- */
-      __pyx_v_self->current_r_end = (__pyx_v_self->ends[__pyx_v_i]);
-
-      /* "sortedintersect/intersect.pyx":117
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):             # <<<<<<<<<<<<<<
- *                     passed = True
- *                     break
+      /* "sortedintersect/sintersect.pyx":182
+ *         for i in range(self.index, size):
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):
+ *                 if self.bool_only:             # <<<<<<<<<<<<<<
+ *                     return True
+ *                 if self.add_data:
  */
-      __pyx_t_9 = (__pyx_f_15sortedintersect_9intersect_is_overlapping(__pyx_v_start, __pyx_v_end, __pyx_v_self->current_r_start, __pyx_v_self->current_r_end) != 0);
+      __pyx_t_9 = (__pyx_v_self->bool_only != 0);
       if (__pyx_t_9) {
 
-        /* "sortedintersect/intersect.pyx":118
- *                 self.current_r_end = self.ends[i]
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):
- *                     passed = True             # <<<<<<<<<<<<<<
- *                     break
- *                 elif self.current_r_start > start:
- */
-        __pyx_v_passed = 1;
-
-        /* "sortedintersect/intersect.pyx":119
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):
- *                     passed = True
- *                     break             # <<<<<<<<<<<<<<
- *                 elif self.current_r_start > start:
- *                     break
+        /* "sortedintersect/sintersect.pyx":183
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):
+ *                 if self.bool_only:
+ *                     return True             # <<<<<<<<<<<<<<
+ *                 if self.add_data:
+ *                     found.append((self.starts[i], self.ends[i].end, self.data[i]))
  */
-        goto __pyx_L9_break;
+        __Pyx_XDECREF(__pyx_r);
+        __Pyx_INCREF(Py_True);
+        __pyx_r = Py_True;
+        goto __pyx_L0;
 
-        /* "sortedintersect/intersect.pyx":117
- *                 self.current_r_start = self.starts[i]
- *                 self.current_r_end = self.ends[i]
- *                 if is_overlapping(start, end, self.current_r_start, self.current_r_end):             # <<<<<<<<<<<<<<
- *                     passed = True
- *                     break
+        /* "sortedintersect/sintersect.pyx":182
+ *         for i in range(self.index, size):
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):
+ *                 if self.bool_only:             # <<<<<<<<<<<<<<
+ *                     return True
+ *                 if self.add_data:
  */
       }
 
-      /* "sortedintersect/intersect.pyx":120
- *                     passed = True
- *                     break
- *                 elif self.current_r_start > start:             # <<<<<<<<<<<<<<
- *                     break
- *                 i += 1
+      /* "sortedintersect/sintersect.pyx":184
+ *                 if self.bool_only:
+ *                     return True
+ *                 if self.add_data:             # <<<<<<<<<<<<<<
+ *                     found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                 else:
  */
-      __pyx_t_9 = ((__pyx_v_self->current_r_start > __pyx_v_start) != 0);
+      __pyx_t_9 = (__pyx_v_self->add_data != 0);
       if (__pyx_t_9) {
 
-        /* "sortedintersect/intersect.pyx":121
- *                     break
- *                 elif self.current_r_start > start:
- *                     break             # <<<<<<<<<<<<<<
- *                 i += 1
- *             self.index = i
- */
-        goto __pyx_L9_break;
+        /* "sortedintersect/sintersect.pyx":185
+ *                     return True
+ *                 if self.add_data:
+ *                     found.append((self.starts[i], self.ends[i].end, self.data[i]))             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     found.append((self.starts[i], self.ends[i].end))
+ */
+        __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->starts[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_self->ends[__pyx_v_i]).end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        if (unlikely(__pyx_v_self->data == Py_None)) {
+          PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+          __PYX_ERR(0, 185, __pyx_L1_error)
+        }
+        __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_GIVEREF(__pyx_t_1);
+        PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+        __Pyx_GIVEREF(__pyx_t_2);
+        PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+        __Pyx_INCREF(PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+        __Pyx_GIVEREF(PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+        PyTuple_SET_ITEM(__pyx_t_5, 2, PyList_GET_ITEM(__pyx_v_self->data, __pyx_v_i));
+        __pyx_t_1 = 0;
+        __pyx_t_2 = 0;
+        __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_found, __pyx_t_5); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 185, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-        /* "sortedintersect/intersect.pyx":120
- *                     passed = True
- *                     break
- *                 elif self.current_r_start > start:             # <<<<<<<<<<<<<<
- *                     break
- *                 i += 1
+        /* "sortedintersect/sintersect.pyx":184
+ *                 if self.bool_only:
+ *                     return True
+ *                 if self.add_data:             # <<<<<<<<<<<<<<
+ *                     found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                 else:
  */
+        goto __pyx_L8;
       }
 
-      /* "sortedintersect/intersect.pyx":122
- *                 elif self.current_r_start > start:
- *                     break
- *                 i += 1             # <<<<<<<<<<<<<<
- *             self.index = i
- * 
- */
-      __pyx_v_i = (__pyx_v_i + 1);
-    }
-    __pyx_L9_break:;
-
-    /* "sortedintersect/intersect.pyx":123
- *                     break
- *                 i += 1
- *             self.index = i             # <<<<<<<<<<<<<<
- * 
- *         elif is_overlapping(start, end, self.current_r_start, self.current_r_end):
- */
-    __pyx_v_self->index = __pyx_v_i;
-
-    /* "sortedintersect/intersect.pyx":112
- *         self.current_r_start = self.starts[i]
- *         self.current_r_end = self.ends[i]
- *         if start > self.current_r_end:             # <<<<<<<<<<<<<<
- *             i = self.index + 1
- *             while i < self.starts.size():
- */
-    goto __pyx_L7;
-  }
-
-  /* "sortedintersect/intersect.pyx":125
- *             self.index = i
- * 
- *         elif is_overlapping(start, end, self.current_r_start, self.current_r_end):             # <<<<<<<<<<<<<<
- *             passed = True
- * 
- */
-  __pyx_t_9 = (__pyx_f_15sortedintersect_9intersect_is_overlapping(__pyx_v_start, __pyx_v_end, __pyx_v_self->current_r_start, __pyx_v_self->current_r_end) != 0);
-  if (__pyx_t_9) {
-
-    /* "sortedintersect/intersect.pyx":126
- * 
- *         elif is_overlapping(start, end, self.current_r_start, self.current_r_end):
- *             passed = True             # <<<<<<<<<<<<<<
- * 
- *         if passed:
- */
-    __pyx_v_passed = 1;
-
-    /* "sortedintersect/intersect.pyx":125
- *             self.index = i
- * 
- *         elif is_overlapping(start, end, self.current_r_start, self.current_r_end):             # <<<<<<<<<<<<<<
- *             passed = True
- * 
- */
-  }
-  __pyx_L7:;
-
-  /* "sortedintersect/intersect.pyx":128
- *             passed = True
- * 
- *         if passed:             # <<<<<<<<<<<<<<
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- */
-  __pyx_t_9 = (__pyx_v_passed != 0);
-  if (__pyx_t_9) {
-
-    /* "sortedintersect/intersect.pyx":129
- * 
- *         if passed:
- *             if self.add_data:             # <<<<<<<<<<<<<<
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
- */
-    __pyx_t_9 = (__pyx_v_self->add_data != 0);
-    if (__pyx_t_9) {
-
-      /* "sortedintersect/intersect.pyx":130
- *         if passed:
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]             # <<<<<<<<<<<<<<
- *             return self.current_r_start, self.current_r_end
- *         return False
- */
-      __Pyx_XDECREF(__pyx_r);
-      __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_self->data, __pyx_v_self->index, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 130, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
-      __Pyx_GIVEREF(__pyx_t_2);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_2);
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_5);
-      __pyx_t_1 = 0;
-      __pyx_t_2 = 0;
-      __pyx_t_5 = 0;
-      __pyx_r = __pyx_t_8;
-      __pyx_t_8 = 0;
-      goto __pyx_L0;
+      /* "sortedintersect/sintersect.pyx":187
+ *                     found.append((self.starts[i], self.ends[i].end, self.data[i]))
+ *                 else:
+ *                     found.append((self.starts[i], self.ends[i].end))             # <<<<<<<<<<<<<<
+ *                 continue
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:
+ */
+      /*else*/ {
+        __pyx_t_5 = __Pyx_PyInt_From_int((__pyx_v_self->starts[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_self->ends[__pyx_v_i]).end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_GIVEREF(__pyx_t_5);
+        PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
+        __Pyx_GIVEREF(__pyx_t_2);
+        PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
+        __pyx_t_5 = 0;
+        __pyx_t_2 = 0;
+        __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_found, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      }
+      __pyx_L8:;
 
-      /* "sortedintersect/intersect.pyx":129
- * 
- *         if passed:
- *             if self.add_data:             # <<<<<<<<<<<<<<
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
+      /* "sortedintersect/sintersect.pyx":188
+ *                 else:
+ *                     found.append((self.starts[i], self.ends[i].end))
+ *                 continue             # <<<<<<<<<<<<<<
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:
+ *                 break
+ */
+      goto __pyx_L4_continue;
+
+      /* "sortedintersect/sintersect.pyx":181
+ *         found = []
+ *         for i in range(self.index, size):
+ *             if is_overlapping(start, end, self.starts[i], self.ends[i].end):             # <<<<<<<<<<<<<<
+ *                 if self.bool_only:
+ *                     return True
  */
     }
 
-    /* "sortedintersect/intersect.pyx":131
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end             # <<<<<<<<<<<<<<
- *         return False
- * 
+    /* "sortedintersect/sintersect.pyx":189
+ *                     found.append((self.starts[i], self.ends[i].end))
+ *                 continue
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:             # <<<<<<<<<<<<<<
+ *                 break
+ *         return False if self.bool_only else found
  */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_5);
-    __pyx_t_8 = 0;
-    __pyx_t_5 = 0;
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
-    goto __pyx_L0;
-
-    /* "sortedintersect/intersect.pyx":128
- *             passed = True
- * 
- *         if passed:             # <<<<<<<<<<<<<<
- *             if self.add_data:
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- */
-  }
+    __pyx_t_14 = ((__pyx_v_start < (__pyx_v_self->starts[__pyx_v_i])) != 0);
+    if (!__pyx_t_14) {
+    } else {
+      __pyx_t_9 = __pyx_t_14;
+      goto __pyx_L9_bool_binop_done;
+    }
+    __pyx_t_14 = ((__pyx_v_start > (__pyx_v_self->ends[__pyx_v_i]).covered_end) != 0);
+    __pyx_t_9 = __pyx_t_14;
+    __pyx_L9_bool_binop_done:;
+    if (__pyx_t_9) {
 
-  /* "sortedintersect/intersect.pyx":132
- *                 return self.current_r_start, self.current_r_end, self.data[self.index]
- *             return self.current_r_start, self.current_r_end
- *         return False             # <<<<<<<<<<<<<<
- * 
- * 
+      /* "sortedintersect/sintersect.pyx":190
+ *                 continue
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:
+ *                 break             # <<<<<<<<<<<<<<
+ *         return False if self.bool_only else found
+ */
+      goto __pyx_L5_break;
+
+      /* "sortedintersect/sintersect.pyx":189
+ *                     found.append((self.starts[i], self.ends[i].end))
+ *                 continue
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:             # <<<<<<<<<<<<<<
+ *                 break
+ *         return False if self.bool_only else found
+ */
+    }
+    __pyx_L4_continue:;
+  }
+  __pyx_L5_break:;
+
+  /* "sortedintersect/sintersect.pyx":191
+ *             elif start < self.starts[i] or start > self.ends[i].covered_end:
+ *                 break
+ *         return False if self.bool_only else found             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(Py_False);
-  __pyx_r = Py_False;
+  if ((__pyx_v_self->bool_only != 0)) {
+    __Pyx_INCREF(Py_False);
+    __pyx_t_1 = Py_False;
+  } else {
+    __Pyx_INCREF(__pyx_v_found);
+    __pyx_t_1 = __pyx_v_found;
+  }
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "sortedintersect/intersect.pyx":99
- * 
+  /* "sortedintersect/sintersect.pyx":165
+ *             return False if self.index >= size else self.starts[self.index] <= pos <= self.ends[self.index].end
  * 
  *     cpdef search_interval(self, int start, int end):             # <<<<<<<<<<<<<<
+ *         """Search for reference intervals overlapping single query interval
  * 
- *         cdef uint64_t i = self.index
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_found);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_9search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_9search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_11search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_15sortedintersect_10sintersect_11IntervalSet_10search_interval[] = "Search for reference intervals overlapping single query interval\n\n        :param start: The start position to search for overlaps\n        :type start: int\n        :param end: The end position to search for overlaps\n        :type end: int\n        ";
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_11search_interval(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_start;
   int __pyx_v_end;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3691,90 +4355,90 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("search_interval", 1, 2, 2, 1); __PYX_ERR(0, 99, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("search_interval", 1, 2, 2, 1); __PYX_ERR(0, 165, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search_interval") < 0)) __PYX_ERR(0, 99, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search_interval") < 0)) __PYX_ERR(0, 165, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
-    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L3_error)
+    __pyx_v_end = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search_interval", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 99, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search_interval", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 165, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_8search_interval(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), __pyx_v_start, __pyx_v_end);
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_10search_interval(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), __pyx_v_start, __pyx_v_end);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_8search_interval(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_10search_interval(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, int __pyx_v_start, int __pyx_v_end) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search_interval", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_15sortedintersect_9intersect_4ISet_search_interval(__pyx_v_self, __pyx_v_start, __pyx_v_end, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_interval(__pyx_v_self, __pyx_v_start, __pyx_v_end, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.search_interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_13__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_10__reduce_cython__(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_12__reduce_cython__(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_10__reduce_cython__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_12__reduce_cython__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -3783,252 +4447,246 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  PyObject *__pyx_t_12 = NULL;
+  int __pyx_t_12;
   int __pyx_t_13;
-  int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
- *     state = (self.add_data, self.current_r_end, self.current_r_start, self.data, self.ends, self.index, self.last_q_end, self.last_q_start, self.last_r_end, self.last_r_start, self.started_ref, self.starts)             # <<<<<<<<<<<<<<
+ *     state = (self.add_data, self.bool_only, self.current_r_end, self.current_r_start, self.data, self.distance_threshold, self.ends, self.index, self.last_q_start, self.last_r_start, self.starts)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
   __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->add_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->bool_only); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_convert_vector_to_py_int(__pyx_v_self->ends); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_self->current_r_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->index); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->distance_threshold); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_self->last_q_end); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(__pyx_v_self->ends); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_self->last_q_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_FromSize_t(__pyx_v_self->index); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->last_r_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->last_q_start); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = __Pyx_PyInt_From_int(__pyx_v_self->last_r_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyBool_FromLong(__pyx_v_self->started_ref); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_10 = __pyx_convert_vector_to_py_int(__pyx_v_self->starts); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_11 = __pyx_convert_vector_to_py_int(__pyx_v_self->starts); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(11); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = PyTuple_New(12); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_11, 3, __pyx_t_4);
   __Pyx_INCREF(__pyx_v_self->data);
   __Pyx_GIVEREF(__pyx_v_self->data);
-  PyTuple_SET_ITEM(__pyx_t_12, 3, __pyx_v_self->data);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_12, 4, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_11, 4, __pyx_v_self->data);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_12, 5, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_11, 5, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_12, 6, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_11, 6, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_12, 7, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_11, 7, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_12, 8, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_11, 8, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_12, 9, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_11, 9, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_12, 10, __pyx_t_10);
-  __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_12, 11, __pyx_t_11);
+  PyTuple_SET_ITEM(__pyx_t_11, 10, __pyx_t_10);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
   __pyx_t_10 = 0;
+  __pyx_v_state = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_v_state = ((PyObject*)__pyx_t_12);
-  __pyx_t_12 = 0;
 
   /* "(tree fragment)":6
  *     cdef bint use_setstate
- *     state = (self.add_data, self.current_r_end, self.current_r_start, self.data, self.ends, self.index, self.last_q_end, self.last_q_start, self.last_r_end, self.last_r_start, self.started_ref, self.starts)
+ *     state = (self.add_data, self.bool_only, self.current_r_end, self.current_r_start, self.data, self.distance_threshold, self.ends, self.index, self.last_q_start, self.last_r_start, self.starts)
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
  *     if _dict is not None:
  *         state += (_dict,)
  */
-  __pyx_t_12 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __pyx_v__dict = __pyx_t_12;
-  __pyx_t_12 = 0;
+  __pyx_t_11 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_v__dict = __pyx_t_11;
+  __pyx_t_11 = 0;
 
   /* "(tree fragment)":7
- *     state = (self.add_data, self.current_r_end, self.current_r_start, self.data, self.ends, self.index, self.last_q_end, self.last_q_start, self.last_r_end, self.last_r_start, self.started_ref, self.starts)
+ *     state = (self.add_data, self.bool_only, self.current_r_end, self.current_r_start, self.data, self.distance_threshold, self.ends, self.index, self.last_q_start, self.last_r_start, self.starts)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
-  __pyx_t_13 = (__pyx_v__dict != Py_None);
-  __pyx_t_14 = (__pyx_t_13 != 0);
-  if (__pyx_t_14) {
+  __pyx_t_12 = (__pyx_v__dict != Py_None);
+  __pyx_t_13 = (__pyx_t_12 != 0);
+  if (__pyx_t_13) {
 
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
  */
-    __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
-    PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_v__dict);
-    __pyx_t_11 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_11));
-    __pyx_t_11 = 0;
+    PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v__dict);
+    __pyx_t_10 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_10));
+    __pyx_t_10 = 0;
 
     /* "(tree fragment)":9
  *     if _dict is not None:
  *         state += (_dict,)
  *         use_setstate = True             # <<<<<<<<<<<<<<
  *     else:
  *         use_setstate = self.data is not None
  */
     __pyx_v_use_setstate = 1;
 
     /* "(tree fragment)":7
- *     state = (self.add_data, self.current_r_end, self.current_r_start, self.data, self.ends, self.index, self.last_q_end, self.last_q_start, self.last_r_end, self.last_r_start, self.started_ref, self.starts)
+ *     state = (self.add_data, self.bool_only, self.current_r_end, self.current_r_start, self.data, self.distance_threshold, self.ends, self.index, self.last_q_start, self.last_r_start, self.starts)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
     goto __pyx_L3;
   }
 
   /* "(tree fragment)":11
  *         use_setstate = True
  *     else:
  *         use_setstate = self.data is not None             # <<<<<<<<<<<<<<
  *     if use_setstate:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, None), state
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, None), state
  */
   /*else*/ {
-    __pyx_t_14 = (__pyx_v_self->data != Py_None);
-    __pyx_v_use_setstate = __pyx_t_14;
+    __pyx_t_13 = (__pyx_v_self->data != ((PyObject*)Py_None));
+    __pyx_v_use_setstate = __pyx_t_13;
   }
   __pyx_L3:;
 
   /* "(tree fragment)":12
  *     else:
  *         use_setstate = self.data is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, None), state
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, None), state
  *     else:
  */
-  __pyx_t_14 = (__pyx_v_use_setstate != 0);
-  if (__pyx_t_14) {
+  __pyx_t_13 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_13) {
 
     /* "(tree fragment)":13
  *         use_setstate = self.data is not None
  *     if use_setstate:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, None), state             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, None), state             # <<<<<<<<<<<<<<
  *     else:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, state)
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, state)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_pyx_unpickle_ISet); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_pyx_unpickle_IntervalSet); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_12, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_25621563);
-    __Pyx_GIVEREF(__pyx_int_25621563);
-    PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_int_25621563);
+    PyTuple_SET_ITEM(__pyx_t_11, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_151996738);
+    __Pyx_GIVEREF(__pyx_int_151996738);
+    PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_151996738);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_12, 2, Py_None);
-    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_11, 2, Py_None);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_GIVEREF(__pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_11);
-    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_11);
-    __Pyx_GIVEREF(__pyx_t_12);
-    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_12);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_11);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_v_state);
-    __pyx_t_11 = 0;
-    __pyx_t_12 = 0;
-    __pyx_r = __pyx_t_10;
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_v_state);
     __pyx_t_10 = 0;
+    __pyx_t_11 = 0;
+    __pyx_r = __pyx_t_9;
+    __pyx_t_9 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
  *     else:
  *         use_setstate = self.data is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, None), state
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, None), state
  *     else:
  */
   }
 
   /* "(tree fragment)":15
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, None), state
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, None), state
  *     else:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, state)             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     __pyx_unpickle_ISet__set_state(self, __pyx_state)
+ *     __pyx_unpickle_IntervalSet__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_pyx_unpickle_ISet); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_pyx_unpickle_IntervalSet); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_12, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_25621563);
-    __Pyx_GIVEREF(__pyx_int_25621563);
-    PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_int_25621563);
+    PyTuple_SET_ITEM(__pyx_t_11, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_INCREF(__pyx_int_151996738);
+    __Pyx_GIVEREF(__pyx_int_151996738);
+    PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_int_151996738);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_v_state);
-    __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_12);
-    PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_12);
-    __pyx_t_10 = 0;
-    __pyx_t_12 = 0;
-    __pyx_r = __pyx_t_11;
+    PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_v_state);
+    __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_11);
+    __pyx_t_9 = 0;
     __pyx_t_11 = 0;
+    __pyx_r = __pyx_t_10;
+    __pyx_t_10 = 0;
     goto __pyx_L0;
   }
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
@@ -4043,192 +4701,102 @@
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, state)
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_ISet__set_state(self, __pyx_state)
+ *     __pyx_unpickle_IntervalSet__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_15sortedintersect_9intersect_4ISet_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_15__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_4ISet_12__setstate_cython__(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect_11IntervalSet_14__setstate_cython__(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_4ISet_12__setstate_cython__(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect_11IntervalSet_14__setstate_cython__(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, state)
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, state)
  * def __setstate_cython__(self, __pyx_state):
- *     __pyx_unpickle_ISet__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_IntervalSet__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_15sortedintersect_9intersect___pyx_unpickle_ISet__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_ISet, (type(self), 0x186f43b, state)
+ *         return __pyx_unpickle_IntervalSet, (type(self), 0x90f4942, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_ISet__set_state(self, __pyx_state)
+ *     __pyx_unpickle_IntervalSet__set_state(self, __pyx_state)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.ISet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "sortedintersect/intersect.pyx":135
- * 
- * 
- * cpdef ISet IntervalSet(with_data):             # <<<<<<<<<<<<<<
- *     """Returns a python friendly IntervalSet for searching with sorted query intervals / points"""
- *     return ISet(with_data)
- */
-
-static PyObject *__pyx_pw_15sortedintersect_9intersect_1IntervalSet(PyObject *__pyx_self, PyObject *__pyx_v_with_data); /*proto*/
-static struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_f_15sortedintersect_9intersect_IntervalSet(PyObject *__pyx_v_with_data, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("IntervalSet", 0);
-
-  /* "sortedintersect/intersect.pyx":137
- * cpdef ISet IntervalSet(with_data):
- *     """Returns a python friendly IntervalSet for searching with sorted query intervals / points"""
- *     return ISet(with_data)             # <<<<<<<<<<<<<<
- */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_15sortedintersect_9intersect_ISet), __pyx_v_with_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = ((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_t_1);
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "sortedintersect/intersect.pyx":135
- * 
- * 
- * cpdef ISet IntervalSet(with_data):             # <<<<<<<<<<<<<<
- *     """Returns a python friendly IntervalSet for searching with sorted query intervals / points"""
- *     return ISet(with_data)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.IntervalSet", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF((PyObject *)__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_1IntervalSet(PyObject *__pyx_self, PyObject *__pyx_v_with_data); /*proto*/
-static char __pyx_doc_15sortedintersect_9intersect_IntervalSet[] = "Returns a python friendly IntervalSet for searching with sorted query intervals / points";
-static PyObject *__pyx_pw_15sortedintersect_9intersect_1IntervalSet(PyObject *__pyx_self, PyObject *__pyx_v_with_data) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("IntervalSet (wrapper)", 0);
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_IntervalSet(__pyx_self, ((PyObject *)__pyx_v_with_data));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_15sortedintersect_9intersect_IntervalSet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_with_data) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("IntervalSet", 0);
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_15sortedintersect_9intersect_IntervalSet(__pyx_v_with_data, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("sortedintersect.intersect.IntervalSet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.IntervalSet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
- * def __pyx_unpickle_ISet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_IntervalSet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_15sortedintersect_9intersect_3__pyx_unpickle_ISet(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_15sortedintersect_9intersect_3__pyx_unpickle_ISet = {"__pyx_unpickle_ISet", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_9intersect_3__pyx_unpickle_ISet, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_15sortedintersect_9intersect_3__pyx_unpickle_ISet(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_1__pyx_unpickle_IntervalSet(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_15sortedintersect_10sintersect_1__pyx_unpickle_IntervalSet = {"__pyx_unpickle_IntervalSet", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_10sintersect_1__pyx_unpickle_IntervalSet, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_15sortedintersect_10sintersect_1__pyx_unpickle_IntervalSet(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__pyx_unpickle_ISet (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_IntervalSet (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -4246,432 +4814,910 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ISet", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_IntervalSet", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ISet", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_IntervalSet", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_ISet") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_IntervalSet") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_ISet", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_IntervalSet", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("sortedintersect.intersect.__pyx_unpickle_ISet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("sortedintersect.sintersect.__pyx_unpickle_IntervalSet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_15sortedintersect_9intersect_2__pyx_unpickle_ISet(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_15sortedintersect_9intersect_2__pyx_unpickle_ISet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_ISet", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_IntervalSet", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x186f43b:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x90f4942, 0xfa605a0, 0x644cd4a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x186f43b) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x186f43b:
+ *     if __pyx_checksum not in (0x90f4942, 0xfa605a0, 0x644cd4a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
- *     __pyx_result = ISet.__new__(__pyx_type)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x186f43b:
+ *     if __pyx_checksum not in (0x90f4942, 0xfa605a0, 0x644cd4a):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)             # <<<<<<<<<<<<<<
- *     __pyx_result = ISet.__new__(__pyx_type)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x18, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x186f43b:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x90f4942, 0xfa605a0, 0x644cd4a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
- *     __pyx_result = ISet.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_15sortedintersect_9intersect_ISet), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_15sortedintersect_10sintersect_IntervalSet), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
- *     __pyx_result = ISet.__new__(__pyx_type)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
- *     __pyx_result = ISet.__new__(__pyx_type)
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)
  *     if __pyx_state is not None:
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_15sortedintersect_9intersect___pyx_unpickle_ISet__set_state(((struct __pyx_obj_15sortedintersect_9intersect_ISet *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet__set_state(((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x186f43b = (add_data, current_r_end, current_r_start, data, ends, index, last_q_end, last_q_start, last_r_end, last_r_start, started_ref, starts))" % __pyx_checksum)
- *     __pyx_result = ISet.__new__(__pyx_type)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
+ *     __pyx_result = IntervalSet.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
   /* "(tree fragment)":10
  *     if __pyx_state is not None:
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  *     return __pyx_result             # <<<<<<<<<<<<<<
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v___pyx_result);
   __pyx_r = __pyx_v___pyx_result;
   goto __pyx_L0;
 
   /* "(tree fragment)":1
- * def __pyx_unpickle_ISet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_IntervalSet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("sortedintersect.intersect.__pyx_unpickle_ISet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("sortedintersect.sintersect.__pyx_unpickle_IntervalSet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":11
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  *     return __pyx_result
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_15sortedintersect_9intersect___pyx_unpickle_ISet__set_state(struct __pyx_obj_15sortedintersect_9intersect_ISet *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_15sortedintersect_10sintersect___pyx_unpickle_IntervalSet__set_state(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  std::vector<int>  __pyx_t_4;
-  Py_ssize_t __pyx_t_5;
-  int __pyx_t_6;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
+  std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  __pyx_t_4;
+  size_t __pyx_t_5;
+  std::vector<int>  __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_ISet__set_state", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_IntervalSet__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]             # <<<<<<<<<<<<<<
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[12])
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[11])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_PyObject_IsTrue(PyTuple_GET_ITEM(__pyx_v___pyx_state, 0)); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_v___pyx_result->add_data = __pyx_t_1;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 1)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->current_r_end = __pyx_t_2;
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(PyTuple_GET_ITEM(__pyx_v___pyx_state, 1)); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_v___pyx_result->bool_only = __pyx_t_1;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 2)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_v___pyx_result->current_r_end = __pyx_t_2;
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 3)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_v___pyx_result->current_r_start = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_3 = PyTuple_GET_ITEM(__pyx_v___pyx_state, 3);
+  if (!(likely(PyList_CheckExact(PyTuple_GET_ITEM(__pyx_v___pyx_state, 4)))||((PyTuple_GET_ITEM(__pyx_v___pyx_state, 4)) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(PyTuple_GET_ITEM(__pyx_v___pyx_state, 4))->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_GET_ITEM(__pyx_v___pyx_state, 4);
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v___pyx_result->data);
   __Pyx_DECREF(__pyx_v___pyx_result->data);
-  __pyx_v___pyx_result->data = __pyx_t_3;
+  __pyx_v___pyx_result->data = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_4 = __pyx_convert_vector_from_py_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 4)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->ends = __pyx_t_4;
-  if (unlikely(__pyx_v___pyx_state == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 12, __pyx_L1_error)
-  }
   __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 5)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->index = __pyx_t_2;
+  __pyx_v___pyx_result->distance_threshold = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 6)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->last_q_end = __pyx_t_2;
+  __pyx_t_4 = __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(PyTuple_GET_ITEM(__pyx_v___pyx_state, 6)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_v___pyx_result->ends = __pyx_t_4;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 7)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->last_q_start = __pyx_t_2;
+  __pyx_t_5 = __Pyx_PyInt_As_size_t(PyTuple_GET_ITEM(__pyx_v___pyx_state, 7)); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_v___pyx_result->index = __pyx_t_5;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 8)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->last_r_end = __pyx_t_2;
+  __pyx_v___pyx_result->last_q_start = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_2 = __Pyx_PyInt_As_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 9)); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_v___pyx_result->last_r_start = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(PyTuple_GET_ITEM(__pyx_v___pyx_state, 10)); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->started_ref = __pyx_t_1;
-  if (unlikely(__pyx_v___pyx_state == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 12, __pyx_L1_error)
-  }
-  __pyx_t_4 = __pyx_convert_vector_from_py_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 11)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_v___pyx_result->starts = __pyx_t_4;
+  __pyx_t_6 = __pyx_convert_vector_from_py_int(PyTuple_GET_ITEM(__pyx_v___pyx_state, 10)); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_v___pyx_result->starts = __pyx_t_6;
 
   /* "(tree fragment)":13
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[12])
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[11])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_6 = ((__pyx_t_5 > 12) != 0);
-  if (__pyx_t_6) {
+  __pyx_t_7 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_8 = ((__pyx_t_7 > 11) != 0);
+  if (__pyx_t_8) {
   } else {
-    __pyx_t_1 = __pyx_t_6;
+    __pyx_t_1 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_6 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_7 = (__pyx_t_6 != 0);
-  __pyx_t_1 = __pyx_t_7;
+  __pyx_t_8 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_9 = (__pyx_t_8 != 0);
+  __pyx_t_1 = __pyx_t_9;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
     /* "(tree fragment)":14
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):
- *         __pyx_result.__dict__.update(__pyx_state[12])             # <<<<<<<<<<<<<<
- */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_update); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[11])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_update); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
-    __pyx_t_8 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-        __Pyx_INCREF(__pyx_t_8);
+    __pyx_t_10 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
+      if (likely(__pyx_t_10)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+        __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, PyTuple_GET_ITEM(__pyx_v___pyx_state, 12)) : __Pyx_PyObject_CallOneArg(__pyx_t_9, PyTuple_GET_ITEM(__pyx_v___pyx_state, 12));
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_3 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_10, PyTuple_GET_ITEM(__pyx_v___pyx_state, 11)) : __Pyx_PyObject_CallOneArg(__pyx_t_11, PyTuple_GET_ITEM(__pyx_v___pyx_state, 11));
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":13
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
- *         __pyx_result.__dict__.update(__pyx_state[12])
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[11])
  */
   }
 
   /* "(tree fragment)":11
- *         __pyx_unpickle_ISet__set_state(<ISet> __pyx_result, __pyx_state)
+ *         __pyx_unpickle_IntervalSet__set_state(<IntervalSet> __pyx_result, __pyx_state)
  *     return __pyx_result
- * cdef __pyx_unpickle_ISet__set_state(ISet __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.current_r_end = __pyx_state[1]; __pyx_result.current_r_start = __pyx_state[2]; __pyx_result.data = __pyx_state[3]; __pyx_result.ends = __pyx_state[4]; __pyx_result.index = __pyx_state[5]; __pyx_result.last_q_end = __pyx_state[6]; __pyx_result.last_q_start = __pyx_state[7]; __pyx_result.last_r_end = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.started_ref = __pyx_state[10]; __pyx_result.starts = __pyx_state[11]
- *     if len(__pyx_state) > 12 and hasattr(__pyx_result, '__dict__'):
+ * cdef __pyx_unpickle_IntervalSet__set_state(IntervalSet __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.add_data = __pyx_state[0]; __pyx_result.bool_only = __pyx_state[1]; __pyx_result.current_r_end = __pyx_state[2]; __pyx_result.current_r_start = __pyx_state[3]; __pyx_result.data = __pyx_state[4]; __pyx_result.distance_threshold = __pyx_state[5]; __pyx_result.ends = __pyx_state[6]; __pyx_result.index = __pyx_state[7]; __pyx_result.last_q_start = __pyx_state[8]; __pyx_result.last_r_start = __pyx_state[9]; __pyx_result.starts = __pyx_state[10]
+ *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("sortedintersect.intersect.__pyx_unpickle_ISet__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_AddTraceback("sortedintersect.sintersect.__pyx_unpickle_IntervalSet__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "vector.to_py":60
  * 
+ * @cname("__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef object __pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(vector[X]& v):             # <<<<<<<<<<<<<<
+ *     return [v[i] for i in range(v.size())]
+ * 
+ */
+
+static PyObject *__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(const std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  &__pyx_v_v) {
+  size_t __pyx_v_i;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  size_t __pyx_t_2;
+  size_t __pyx_t_3;
+  size_t __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", 0);
+
+  /* "vector.to_py":61
+ * @cname("__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef object __pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(vector[X]& v):
+ *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __pyx_v_v.size();
+  __pyx_t_3 = __pyx_t_2;
+  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
+    __pyx_v_i = __pyx_t_4;
+    __pyx_t_5 = __pyx_convert__to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "vector.to_py":60
+ * 
+ * @cname("__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef object __pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(vector[X]& v):             # <<<<<<<<<<<<<<
+ *     return [v[i] for i in range(v.size())]
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "FromPyStructUtility":11
+ * 
+ * @cname("__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef struct_type __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(obj) except *:             # <<<<<<<<<<<<<<
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ */
+
+static struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(PyObject *__pyx_v_obj) {
+  struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_v_result;
+  PyObject *__pyx_v_value = NULL;
+  struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", 0);
+
+  /* "FromPyStructUtility":13
+ * cdef struct_type __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(obj) except *:
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
+ * 
+ */
+  __pyx_t_1 = ((!(PyMapping_Check(__pyx_v_obj) != 0)) != 0);
+  if (__pyx_t_1) {
+
+    /* "FromPyStructUtility":14
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)             # <<<<<<<<<<<<<<
+ * 
+ *     try:
+ */
+    __pyx_t_2 = PyErr_Format(__pyx_builtin_TypeError, ((char const *)"Expected %.16s, got %.200s"), ((char *)"a mapping"), Py_TYPE(__pyx_v_obj)->tp_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "FromPyStructUtility":13
+ * cdef struct_type __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(obj) except *:
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):             # <<<<<<<<<<<<<<
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
+ * 
+ */
+  }
+
+  /* "FromPyStructUtility":16
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['end']
+ *     except KeyError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
+    __Pyx_XGOTREF(__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_5);
+    /*try:*/ {
+
+      /* "FromPyStructUtility":17
+ * 
+ *     try:
+ *         value = obj['end']             # <<<<<<<<<<<<<<
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ */
+      __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 17, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_v_value = __pyx_t_2;
+      __pyx_t_2 = 0;
+
+      /* "FromPyStructUtility":16
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['end']
+ *     except KeyError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    goto __pyx_L9_try_end;
+    __pyx_L4_error:;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "FromPyStructUtility":18
+ *     try:
+ *         value = obj['end']
+ *     except KeyError:             # <<<<<<<<<<<<<<
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ *     result.end = value
+ */
+    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
+    if (__pyx_t_6) {
+      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(1, 18, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_8);
+
+      /* "FromPyStructUtility":19
+ *         value = obj['end']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'end'")             # <<<<<<<<<<<<<<
+ *     result.end = value
+ *     try:
+ */
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 19, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __PYX_ERR(1, 19, __pyx_L6_except_error)
+    }
+    goto __pyx_L6_except_error;
+    __pyx_L6_except_error:;
+
+    /* "FromPyStructUtility":16
+ *         PyErr_Format(TypeError, b"Expected %.16s, got %.200s", b"a mapping", Py_TYPE(obj).tp_name)
+ * 
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['end']
+ *     except KeyError:
+ */
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
+    goto __pyx_L1_error;
+    __pyx_L9_try_end:;
+  }
+
+  /* "FromPyStructUtility":20
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ *     result.end = value             # <<<<<<<<<<<<<<
+ *     try:
+ *         value = obj['covered_end']
+ */
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_v_result.end = __pyx_t_6;
+
+  /* "FromPyStructUtility":21
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ *     result.end = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['covered_end']
+ *     except KeyError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_4, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_5);
+    __Pyx_XGOTREF(__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "FromPyStructUtility":22
+ *     result.end = value
+ *     try:
+ *         value = obj['covered_end']             # <<<<<<<<<<<<<<
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")
+ */
+      __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_obj, __pyx_n_s_covered_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 22, __pyx_L12_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF_SET(__pyx_v_value, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "FromPyStructUtility":21
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ *     result.end = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['covered_end']
+ *     except KeyError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L17_try_end;
+    __pyx_L12_error:;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+
+    /* "FromPyStructUtility":23
+ *     try:
+ *         value = obj['covered_end']
+ *     except KeyError:             # <<<<<<<<<<<<<<
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")
+ *     result.covered_end = value
+ */
+    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
+    if (__pyx_t_6) {
+      __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_7, &__pyx_t_2) < 0) __PYX_ERR(1, 23, __pyx_L14_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_2);
+
+      /* "FromPyStructUtility":24
+ *         value = obj['covered_end']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")             # <<<<<<<<<<<<<<
+ *     result.covered_end = value
+ *     return result
+ */
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 24, __pyx_L14_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_Raise(__pyx_t_9, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __PYX_ERR(1, 24, __pyx_L14_except_error)
+    }
+    goto __pyx_L14_except_error;
+    __pyx_L14_except_error:;
+
+    /* "FromPyStructUtility":21
+ *         raise ValueError("No value specified for struct attribute 'end'")
+ *     result.end = value
+ *     try:             # <<<<<<<<<<<<<<
+ *         value = obj['covered_end']
+ *     except KeyError:
+ */
+    __Pyx_XGIVEREF(__pyx_t_5);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_4, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L17_try_end:;
+  }
+
+  /* "FromPyStructUtility":25
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")
+ *     result.covered_end = value             # <<<<<<<<<<<<<<
+ *     return result
+ * 
+ */
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 25, __pyx_L1_error)
+  __pyx_v_result.covered_end = __pyx_t_6;
+
+  /* "FromPyStructUtility":26
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")
+ *     result.covered_end = value
+ *     return result             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_result;
+  goto __pyx_L0;
+
+  /* "FromPyStructUtility":11
+ * 
+ * @cname("__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef struct_type __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(obj) except *:             # <<<<<<<<<<<<<<
+ *     cdef struct_type result
+ *     if not PyMapping_Check(obj):
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("FromPyStructUtility.__pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef vector[X] __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(PyObject *__pyx_v_o) {
+  std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  struct __pyx_t_15sortedintersect_10sintersect_Interval __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_convert__from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    __pyx_v_v.push_back(__pyx_t_5);
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval")
+ * cdef vector[X] __pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_struct____pyx_t_15sortedintersect_10sintersect_Interval", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":60
+ * 
  * @cname("__pyx_convert_vector_to_py_int")
  * cdef object __pyx_convert_vector_to_py_int(vector[X]& v):             # <<<<<<<<<<<<<<
  *     return [v[i] for i in range(v.size())]
  * 
  */
 
 static PyObject *__pyx_convert_vector_to_py_int(const std::vector<int>  &__pyx_v_v) {
@@ -4848,81 +5894,82 @@
   __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_15sortedintersect_9intersect_ISet __pyx_vtable_15sortedintersect_9intersect_ISet;
+static struct __pyx_vtabstruct_15sortedintersect_10sintersect_IntervalSet __pyx_vtable_15sortedintersect_10sintersect_IntervalSet;
 
-static PyObject *__pyx_tp_new_15sortedintersect_9intersect_ISet(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_15sortedintersect_9intersect_ISet *p;
+static PyObject *__pyx_tp_new_15sortedintersect_10sintersect_IntervalSet(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_15sortedintersect_9intersect_ISet *)o);
-  p->__pyx_vtab = __pyx_vtabptr_15sortedintersect_9intersect_ISet;
+  p = ((struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)o);
+  p->__pyx_vtab = __pyx_vtabptr_15sortedintersect_10sintersect_IntervalSet;
   new((void*)&(p->starts)) std::vector<int> ();
-  new((void*)&(p->ends)) std::vector<int> ();
-  p->data = Py_None; Py_INCREF(Py_None);
+  new((void*)&(p->ends)) std::vector<struct __pyx_t_15sortedintersect_10sintersect_Interval> ();
+  p->data = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_15sortedintersect_9intersect_ISet(PyObject *o) {
-  struct __pyx_obj_15sortedintersect_9intersect_ISet *p = (struct __pyx_obj_15sortedintersect_9intersect_ISet *)o;
+static void __pyx_tp_dealloc_15sortedintersect_10sintersect_IntervalSet(PyObject *o) {
+  struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *p = (struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->starts);
   __Pyx_call_destructor(p->ends);
   Py_CLEAR(p->data);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_15sortedintersect_9intersect_ISet(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_15sortedintersect_10sintersect_IntervalSet(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_15sortedintersect_9intersect_ISet *p = (struct __pyx_obj_15sortedintersect_9intersect_ISet *)o;
+  struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *p = (struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)o;
   if (p->data) {
     e = (*v)(p->data, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_15sortedintersect_9intersect_ISet(PyObject *o) {
+static int __pyx_tp_clear_15sortedintersect_10sintersect_IntervalSet(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_15sortedintersect_9intersect_ISet *p = (struct __pyx_obj_15sortedintersect_9intersect_ISet *)o;
+  struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *p = (struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *)o;
   tmp = ((PyObject*)p->data);
-  p->data = Py_None; Py_INCREF(Py_None);
+  p->data = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_15sortedintersect_9intersect_ISet[] = {
-  {"add", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_9intersect_4ISet_3add, METH_VARARGS|METH_KEYWORDS, 0},
-  {"add_from_iter", (PyCFunction)__pyx_pw_15sortedintersect_9intersect_4ISet_5add_from_iter, METH_O, 0},
-  {"search_point", (PyCFunction)__pyx_pw_15sortedintersect_9intersect_4ISet_7search_point, METH_O, 0},
-  {"search_interval", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_9intersect_4ISet_9search_interval, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_15sortedintersect_9intersect_4ISet_11__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_15sortedintersect_9intersect_4ISet_13__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_15sortedintersect_10sintersect_IntervalSet[] = {
+  {"set_distance_threshold", (PyCFunction)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_3set_distance_threshold, METH_O, 0},
+  {"add", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_5add, METH_VARARGS|METH_KEYWORDS, 0},
+  {"add_from_iter", (PyCFunction)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_7add_from_iter, METH_O, 0},
+  {"search_point", (PyCFunction)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_9search_point, METH_O, __pyx_doc_15sortedintersect_10sintersect_11IntervalSet_8search_point},
+  {"search_interval", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_11search_interval, METH_VARARGS|METH_KEYWORDS, __pyx_doc_15sortedintersect_10sintersect_11IntervalSet_10search_interval},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_13__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_15sortedintersect_10sintersect_11IntervalSet_15__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_15sortedintersect_9intersect_ISet = {
+static PyTypeObject __pyx_type_15sortedintersect_10sintersect_IntervalSet = {
   PyVarObject_HEAD_INIT(0, 0)
-  "sortedintersect.intersect.ISet", /*tp_name*/
-  sizeof(struct __pyx_obj_15sortedintersect_9intersect_ISet), /*tp_basicsize*/
+  "sortedintersect.sintersect.IntervalSet", /*tp_name*/
+  sizeof(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_15sortedintersect_9intersect_ISet, /*tp_dealloc*/
+  __pyx_tp_dealloc_15sortedintersect_10sintersect_IntervalSet, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -4940,71 +5987,73 @@
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
-  "A sorted interval set for searching with sorted query intervals / points", /*tp_doc*/
-  __pyx_tp_traverse_15sortedintersect_9intersect_ISet, /*tp_traverse*/
-  __pyx_tp_clear_15sortedintersect_9intersect_ISet, /*tp_clear*/
+  "An interval set for searching with sorted reference intervals and optionally sorted query points/intervals\n\n    Reference intervals must be added in sorted order\n    If query points are not sorted, a binary search is used, otherwise a lineary search is used\n\n    :param with_data: Whether to record additional data along with an interval\n    :type with_data: bool\n    :return: IntervalSet class for performing intersections\n    :rtype: IntervalSet\n    ", /*tp_doc*/
+  __pyx_tp_traverse_15sortedintersect_10sintersect_IntervalSet, /*tp_traverse*/
+  __pyx_tp_clear_15sortedintersect_10sintersect_IntervalSet, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_15sortedintersect_9intersect_ISet, /*tp_methods*/
+  __pyx_methods_15sortedintersect_10sintersect_IntervalSet, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
-  __pyx_pw_15sortedintersect_9intersect_4ISet_1__init__, /*tp_init*/
+  __pyx_pw_15sortedintersect_10sintersect_11IntervalSet_1__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_15sortedintersect_9intersect_ISet, /*tp_new*/
+  __pyx_tp_new_15sortedintersect_10sintersect_IntervalSet, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
-  {"IntervalSet", (PyCFunction)__pyx_pw_15sortedintersect_9intersect_1IntervalSet, METH_O, __pyx_doc_15sortedintersect_9intersect_IntervalSet},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_intersect(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_sintersect(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_intersect},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_sintersect},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "intersect",
+    "sintersect",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -5025,92 +6074,152 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
-  {&__pyx_n_s_ISet, __pyx_k_ISet, sizeof(__pyx_k_ISet), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x18, __pyx_k_Incompatible_checksums_s_vs_0x18, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x18), 0, 0, 1, 0},
+  {&__pyx_kp_u_End_less_than_start, __pyx_k_End_less_than_start, sizeof(__pyx_k_End_less_than_start), 0, 1, 0, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_kp_u_Interval, __pyx_k_Interval, sizeof(__pyx_k_Interval), 0, 1, 0, 0},
+  {&__pyx_n_s_IntervalSet, __pyx_k_IntervalSet, sizeof(__pyx_k_IntervalSet), 0, 0, 1, 1},
   {&__pyx_n_u_IntervalSet, __pyx_k_IntervalSet, sizeof(__pyx_k_IntervalSet), 0, 1, 0, 1},
+  {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
+  {&__pyx_kp_s_No_value_specified_for_struct_at, __pyx_k_No_value_specified_for_struct_at, sizeof(__pyx_k_No_value_specified_for_struct_at), 0, 0, 1, 0},
+  {&__pyx_kp_s_No_value_specified_for_struct_at_2, __pyx_k_No_value_specified_for_struct_at_2, sizeof(__pyx_k_No_value_specified_for_struct_at_2), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Position, __pyx_k_Position, sizeof(__pyx_k_Position), 0, 1, 0, 0},
+  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
+  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
   {&__pyx_n_s_add_from_iter, __pyx_k_add_from_iter, sizeof(__pyx_k_add_from_iter), 0, 0, 1, 1},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
-  {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
+  {&__pyx_n_s_bool_only, __pyx_k_bool_only, sizeof(__pyx_k_bool_only), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+  {&__pyx_n_s_covered_end, __pyx_k_covered_end, sizeof(__pyx_k_covered_end), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+  {&__pyx_n_s_distance_threshold, __pyx_k_distance_threshold, sizeof(__pyx_k_distance_threshold), 0, 0, 1, 1},
   {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_kp_u_is_not_in_sorted_order_last_int, __pyx_k_is_not_in_sorted_order_last_int, sizeof(__pyx_k_is_not_in_sorted_order_last_int), 0, 1, 0, 0},
-  {&__pyx_kp_u_is_not_in_sorted_order_last_que, __pyx_k_is_not_in_sorted_order_last_que, sizeof(__pyx_k_is_not_in_sorted_order_last_que), 0, 1, 0, 0},
+  {&__pyx_n_u_len, __pyx_k_len, sizeof(__pyx_k_len), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
-  {&__pyx_n_s_pyx_unpickle_ISet, __pyx_k_pyx_unpickle_ISet, sizeof(__pyx_k_pyx_unpickle_ISet), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_IntervalSet, __pyx_k_pyx_unpickle_IntervalSet, sizeof(__pyx_k_pyx_unpickle_IntervalSet), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_search_interval, __pyx_k_search_interval, sizeof(__pyx_k_search_interval), 0, 0, 1, 1},
   {&__pyx_n_s_search_point, __pyx_k_search_point, sizeof(__pyx_k_search_point), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_sortedintersect_intersect, __pyx_k_sortedintersect_intersect, sizeof(__pyx_k_sortedintersect_intersect), 0, 0, 1, 1},
+  {&__pyx_n_s_sortedintersect_sintersect, __pyx_k_sortedintersect_sintersect, sizeof(__pyx_k_sortedintersect_sintersect), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_with_data, __pyx_k_with_data, sizeof(__pyx_k_with_data), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 61, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 14, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 18, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "sortedintersect/sintersect.pyx":50
+ *     cpdef add(self, int start, int end, value=None):
+ *         if end < start:
+ *             raise ValueError("End less than start")             # <<<<<<<<<<<<<<
+ *         if start < self.last_r_start:
+ *             raise ValueError(f'Interval {start}-{end} is not in sorted order, last interval seen was {self.last_r_start}')
+ */
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_End_less_than_start); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x90f4942, 0xfa605a0, 0x644cd4a):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x90f4942, 0xfa605a0, 0x644cd4a) = (add_data, bool_only, current_r_end, current_r_start, data, distance_threshold, ends, index, last_q_start, last_r_start, starts))" % __pyx_checksum)
+ */
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_151996738, __pyx_int_262538656, __pyx_int_105172298); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "FromPyStructUtility":19
+ *         value = obj['end']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'end'")             # <<<<<<<<<<<<<<
+ *     result.end = value
+ *     try:
+ */
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
+  /* "FromPyStructUtility":24
+ *         value = obj['covered_end']
+ *     except KeyError:
+ *         raise ValueError("No value specified for struct attribute 'covered_end'")             # <<<<<<<<<<<<<<
+ *     result.covered_end = value
+ *     return result
+ */
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_2); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+
   /* "(tree fragment)":1
- * def __pyx_unpickle_ISet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_IntervalSet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__2 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ISet, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntervalSet, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  __pyx_int_25621563 = PyInt_FromLong(25621563L); if (unlikely(!__pyx_int_25621563)) __PYX_ERR(0, 1, __pyx_L1_error)
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_50000 = PyInt_FromLong(50000L); if (unlikely(!__pyx_int_50000)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_105172298 = PyInt_FromLong(105172298L); if (unlikely(!__pyx_int_105172298)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_151996738 = PyInt_FromLong(151996738L); if (unlikely(!__pyx_int_151996738)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_262538656 = PyInt_FromLong(262538656L); if (unlikely(!__pyx_int_262538656)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -5147,30 +6256,33 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_15sortedintersect_9intersect_ISet = &__pyx_vtable_15sortedintersect_9intersect_ISet;
-  __pyx_vtable_15sortedintersect_9intersect_ISet.add = (PyObject *(*)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_9intersect_4ISet_add *__pyx_optional_args))__pyx_f_15sortedintersect_9intersect_4ISet_add;
-  __pyx_vtable_15sortedintersect_9intersect_ISet.add_from_iter = (PyObject *(*)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, PyObject *, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_9intersect_4ISet_add_from_iter;
-  __pyx_vtable_15sortedintersect_9intersect_ISet.search_point = (PyObject *(*)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_9intersect_4ISet_search_point;
-  __pyx_vtable_15sortedintersect_9intersect_ISet.search_interval = (PyObject *(*)(struct __pyx_obj_15sortedintersect_9intersect_ISet *, int, int, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_9intersect_4ISet_search_interval;
-  if (PyType_Ready(&__pyx_type_15sortedintersect_9intersect_ISet) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_vtabptr_15sortedintersect_10sintersect_IntervalSet = &__pyx_vtable_15sortedintersect_10sintersect_IntervalSet;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet.add = (PyObject *(*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int, int __pyx_skip_dispatch, struct __pyx_opt_args_15sortedintersect_10sintersect_11IntervalSet_add *__pyx_optional_args))__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet.add_from_iter = (PyObject *(*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, PyObject *, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_10sintersect_11IntervalSet_add_from_iter;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet._line_scan = (void (*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int))__pyx_f_15sortedintersect_10sintersect_11IntervalSet__line_scan;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet._binary_search = (void (*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int))__pyx_f_15sortedintersect_10sintersect_11IntervalSet__binary_search;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet._set_reference_index = (void (*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int))__pyx_f_15sortedintersect_10sintersect_11IntervalSet__set_reference_index;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet.search_point = (PyObject *(*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_point;
+  __pyx_vtable_15sortedintersect_10sintersect_IntervalSet.search_interval = (PyObject *(*)(struct __pyx_obj_15sortedintersect_10sintersect_IntervalSet *, int, int, int __pyx_skip_dispatch))__pyx_f_15sortedintersect_10sintersect_11IntervalSet_search_interval;
+  if (PyType_Ready(&__pyx_type_15sortedintersect_10sintersect_IntervalSet) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_15sortedintersect_9intersect_ISet.tp_print = 0;
+  __pyx_type_15sortedintersect_10sintersect_IntervalSet.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_15sortedintersect_9intersect_ISet.tp_dictoffset && __pyx_type_15sortedintersect_9intersect_ISet.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_15sortedintersect_9intersect_ISet.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_15sortedintersect_10sintersect_IntervalSet.tp_dictoffset && __pyx_type_15sortedintersect_10sintersect_IntervalSet.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_15sortedintersect_10sintersect_IntervalSet.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_15sortedintersect_9intersect_ISet.tp_dict, __pyx_vtabptr_15sortedintersect_9intersect_ISet) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ISet, (PyObject *)&__pyx_type_15sortedintersect_9intersect_ISet) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_15sortedintersect_9intersect_ISet) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
-  __pyx_ptype_15sortedintersect_9intersect_ISet = &__pyx_type_15sortedintersect_9intersect_ISet;
+  if (__Pyx_SetVtable(__pyx_type_15sortedintersect_10sintersect_IntervalSet.tp_dict, __pyx_vtabptr_15sortedintersect_10sintersect_IntervalSet) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_IntervalSet, (PyObject *)&__pyx_type_15sortedintersect_10sintersect_IntervalSet) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_15sortedintersect_10sintersect_IntervalSet) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_ptype_15sortedintersect_10sintersect_IntervalSet = &__pyx_type_15sortedintersect_10sintersect_IntervalSet;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5213,19 +6325,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initintersect(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initintersect(void)
+__Pyx_PyMODINIT_FUNC initsintersect(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initsintersect(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_intersect(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_intersect(void)
+__Pyx_PyMODINIT_FUNC PyInit_sintersect(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_sintersect(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -5284,42 +6396,42 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_intersect(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_sintersect(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'intersect' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'sintersect' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_intersect(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_sintersect(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5339,51 +6451,49 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("intersect", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("sintersect", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_sortedintersect__intersect) {
+  if (__pyx_module_is_main_sortedintersect__sintersect) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "sortedintersect.intersect")) {
-      if (unlikely(PyDict_SetItemString(modules, "sortedintersect.intersect", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "sortedintersect.sintersect")) {
+      if (unlikely(PyDict_SetItemString(modules, "sortedintersect.sintersect", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5396,40 +6506,40 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "sortedintersect/intersect.pyx":7
- * 
+  /* "sortedintersect/sintersect.pyx":6
+ * from libcpp.algorithm cimport upper_bound
  * 
  * __all__ = ["IntervalSet"]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_IntervalSet);
   __Pyx_GIVEREF(__pyx_n_u_IntervalSet);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_u_IntervalSet);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":1
- * def __pyx_unpickle_ISet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ * def __pyx_unpickle_IntervalSet(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15sortedintersect_9intersect_3__pyx_unpickle_ISet, NULL, __pyx_n_s_sortedintersect_intersect); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15sortedintersect_10sintersect_1__pyx_unpickle_IntervalSet, NULL, __pyx_n_s_sortedintersect_sintersect); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ISet, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_IntervalSet, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "sortedintersect/intersect.pyx":1
+  /* "sortedintersect/sintersect.pyx":1
  * #cython: language_level=3, boundscheck=False, wraparound=False             # <<<<<<<<<<<<<<
  * #distutils: language=c++
  * from libcpp.vector cimport vector
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5446,19 +6556,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init sortedintersect.intersect", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init sortedintersect.sintersect", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init sortedintersect.intersect");
+    PyErr_SetString(PyExc_ImportError, "init sortedintersect.sintersect");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -5823,15 +6933,15 @@
 }
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -5839,14 +6949,197 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* CIntToDigits */
 static const char DIGIT_PAIRS_10[2*10*10+1] = {
     "00010203040506070809"
     "10111213141516171819"
     "20212223242526272829"
     "30313233343536373839"
     "40414243444546474849"
@@ -5908,15 +7201,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -5942,41 +7235,27 @@
         Py_XDECREF(sign);
     }
 #endif
     return uval;
 }
 
 /* CIntToPyUnicode */
-#ifdef _MSC_VER
-    #ifndef _MSC_STDINT_H_
-        #if _MSC_VER < 1300
-           typedef unsigned short    uint16_t;
-        #else
-           typedef unsigned __int16  uint16_t;
-        #endif
-    #endif
-#else
-   #include <stdint.h>
-#endif
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define GCC_DIAGNOSTIC
-#endif
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char) {
     char digits[sizeof(int)*3+2];
     char *dpos, *end = digits + sizeof(int)*3+2;
     const char *hex_digits = DIGITS_HEX;
     Py_ssize_t length, ulength;
     int prepend_sign, last_one_off;
     int remaining;
-#ifdef GCC_DIAGNOSTIC
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef GCC_DIAGNOSTIC
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (format_char == 'X') {
         hex_digits += 16;
         format_char = 'x';
     }
@@ -5986,22 +7265,22 @@
     do {
         int digit_pos;
         switch (format_char) {
         case 'o':
             digit_pos = abs((int)(remaining % (8*8)));
             remaining = (int) (remaining / (8*8));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_8)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 8);
             break;
         case 'd':
             digit_pos = abs((int)(remaining % (10*10)));
             remaining = (int) (remaining / (10*10));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_10)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 10);
             break;
         case 'x':
             *(--dpos) = hex_digits[abs((int)(remaining % 16))];
             remaining = (int) (remaining / 16);
             break;
         default:
@@ -6134,15 +7413,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+        } else if (__Pyx_PyFastCFunction_Check(func)) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -6152,197 +7431,14 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -6364,139 +7460,43 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || (Py_TYPE(descr) == &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (descr != NULL) {
-        *method = descr;
-        return 0;
-    }
-    PyErr_Format(PyExc_AttributeError,
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, name);
-#else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(name));
-#endif
-    return 0;
+    if (likely(PyUnicode_Check(n)))
 #else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
+    if (likely(PyString_Check(n)))
 #endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
+        return __Pyx_PyObject_GetAttrStr(o, n);
 #endif
-    *method = attr;
-    return 0;
+    return PyObject_GetAttr(o, n);
 }
 
-/* PyObjectCallMethod1 */
-static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
-    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
-    Py_DECREF(method);
-    return result;
-}
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
-    PyObject *method = NULL, *result;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_Call2Args(method, obj, arg);
-        Py_DECREF(method);
-        return result;
+/* HasAttr */
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
     }
-    if (unlikely(!method)) return NULL;
-    return __Pyx__PyObject_CallMethod1(method, arg);
-}
-
-/* append */
-static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x) {
-    if (likely(PyList_CheckExact(L))) {
-        if (unlikely(__Pyx_PyList_Append(L, x) < 0)) return -1;
+    r = __Pyx_GetAttr(o, n);
+    if (unlikely(!r)) {
+        PyErr_Clear();
+        return 0;
     } else {
-        PyObject* retval = __Pyx_PyObject_CallMethod1(L, __pyx_n_s_append, x);
-        if (unlikely(!retval))
-            return -1;
-        Py_DECREF(retval);
+        Py_DECREF(r);
+        return 1;
     }
-    return 0;
 }
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
@@ -6578,14 +7578,54 @@
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* PyErrExceptionMatches */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
@@ -6603,27 +7643,14 @@
     if (unlikely(!exc_type)) return 0;
     if (unlikely(PyTuple_Check(err)))
         return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
     return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
 }
 #endif
 
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
 /* GetAttr3 */
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
@@ -6745,30 +7772,166 @@
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
-/* HasAttr */
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
-    PyObject *r;
-    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "hasattr(): attribute name must be string");
-        return -1;
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
     }
-    r = __Pyx_GetAttr(o, n);
-    if (unlikely(!r)) {
-        PyErr_Clear();
-        return 0;
-    } else {
-        Py_DECREF(r);
-        return 1;
+    Py_INCREF(value);
+    return value;
+}
+#endif
+
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
     }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
 }
 
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
@@ -6873,25 +8036,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -6928,26 +8109,28 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -6969,15 +8152,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -7063,41 +8246,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -7108,34 +8298,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -7144,45 +8349,14 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -7197,48 +8371,78 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+static PyObject* __pyx_convert__to_py_struct____pyx_t_15sortedintersect_10sintersect_Interval(struct __pyx_t_15sortedintersect_10sintersect_Interval s) {
+  PyObject* res;
+  PyObject* member;
+  res = __Pyx_PyDict_NewPresized(2); if (unlikely(!res)) return NULL;
+  member = __Pyx_PyInt_From_int(s.end); if (unlikely(!member)) goto bad;
+  if (unlikely(PyDict_SetItem(res, __pyx_n_s_end, member) < 0)) goto bad;
+  Py_DECREF(member);
+  member = __Pyx_PyInt_From_int(s.covered_end); if (unlikely(!member)) goto bad;
+  if (unlikely(PyDict_SetItem(res, __pyx_n_s_covered_end, member) < 0)) goto bad;
+  Py_DECREF(member);
+  return res;
+  bad:
+  Py_XDECREF(member);
+  Py_DECREF(res);
+  return NULL;
+}
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -7281,15 +8485,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7418,163 +8622,170 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
+        if (sizeof(size_t) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (long) val;
+            return (size_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
+                case  0: return (size_t) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
+                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
+                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
+                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (long) -1;
+                    return (size_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
+            if (sizeof(size_t) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
+                case  0: return (size_t) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
+            if (sizeof(size_t) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
 #if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
                             "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
 #else
-            long val;
+            size_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -7586,184 +8797,191 @@
                                               bytes, sizeof(val),
                                               is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
 #endif
-            return (long) -1;
+            return (size_t) -1;
         }
     } else {
-        long val;
+        size_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (long) -1;
-        val = __Pyx_PyInt_As_long(tmp);
+        if (!tmp) return (size_t) -1;
+        val = __Pyx_PyInt_As_size_t(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to long");
-    return (long) -1;
+        "value too large to convert to size_t");
+    return (size_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to long");
-    return (long) -1;
+        "can't convert negative value to size_t");
+    return (size_t) -1;
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(size_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
+        if (sizeof(long) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (size_t) val;
+            return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
+                case  0: return (long) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
                 case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
+                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
+                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
+                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (size_t) -1;
+                    return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(size_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
+            if (sizeof(long) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             const digit* digits = ((PyLongObject*)x)->ob_digit;
             switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
+                case  0: return (long) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
                 case -2:
-                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -3:
-                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case -4:
-                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
                 case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
+                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
                         if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
                     }
                     break;
             }
 #endif
-            if (sizeof(size_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
+            if (sizeof(long) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
 #if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
             PyErr_SetString(PyExc_RuntimeError,
                             "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
 #else
-            size_t val;
+            long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
  #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -7775,32 +8993,70 @@
                                               bytes, sizeof(val),
                                               is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
 #endif
-            return (size_t) -1;
+            return (long) -1;
         }
     } else {
-        size_t val;
+        long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (size_t) -1;
-        val = __Pyx_PyInt_As_size_t(tmp);
+        if (!tmp) return (long) -1;
+        val = __Pyx_PyInt_As_long(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to size_t");
-    return (size_t) -1;
+        "value too large to convert to long");
+    return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to size_t");
-    return (size_t) -1;
+        "can't convert negative value to long");
+    return (long) -1;
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
@@ -7897,19 +9153,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -8159,14 +9437,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

