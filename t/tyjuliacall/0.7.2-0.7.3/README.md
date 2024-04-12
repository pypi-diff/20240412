# Comparing `tmp/tyjuliacall-0.7.2.tar.gz` & `tmp/tyjuliacall-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyjuliacall-0.7.2.tar", max compression
+gzip compressed data, was "tyjuliacall-0.7.3.tar", max compression
```

## Comparing `tyjuliacall-0.7.2.tar` & `tyjuliacall-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1123 2024-03-01 10:08:01.178528 tyjuliacall-0.7.2/LICENSE
--rw-r--r--   0        0        0      499 2024-03-02 00:54:00.867266 tyjuliacall-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4302 2024-03-01 10:08:01.178528 tyjuliacall-0.7.2/README.md
--rw-r--r--   0        0        0      172 2024-03-01 10:08:01.180527 tyjuliacall-0.7.2/tyjuliacall/__init__.py
--rw-r--r--   0        0        0    11608 2024-03-02 00:53:45.283266 tyjuliacall-0.7.2/tyjuliasetup/__init__.py
--rw-r--r--   0        0        0     1291 2024-03-01 10:08:01.181527 tyjuliacall-0.7.2/tyjuliasetup/compat.py
--rw-r--r--   0        0        0    15195 2024-03-01 10:08:01.182530 tyjuliacall-0.7.2/tyjuliasetup/julia_src_binding.py
--rw-r--r--   0        0        0     5207 2024-03-01 10:08:01.182530 tyjuliacall-0.7.2/tyjuliasetup/jv.py
--rw-r--r--   0        0        0       84 2024-03-01 10:08:01.180527 tyjuliacall-0.7.2/tyjuliasetup/Project.toml
--rw-r--r--   0        0        0    15097 2024-03-01 10:08:01.182530 tyjuliacall-0.7.2/tyjuliasetup/src/TyJuliaSetup.jl
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 tyjuliacall-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-12 02:27:39.100720 tyjuliacall-0.7.3/LICENSE
+-rw-r--r--   0        0        0      499 2024-04-12 03:31:40.491352 tyjuliacall-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     4302 2024-04-12 02:27:39.101720 tyjuliacall-0.7.3/README.md
+-rw-r--r--   0        0        0      172 2024-04-12 02:27:39.102720 tyjuliacall-0.7.3/tyjuliacall/__init__.py
+-rw-r--r--   0        0        0    11608 2024-04-12 02:27:39.103720 tyjuliacall-0.7.3/tyjuliasetup/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-12 02:27:39.103720 tyjuliacall-0.7.3/tyjuliasetup/compat.py
+-rw-r--r--   0        0        0    16175 2024-04-12 03:31:23.911075 tyjuliacall-0.7.3/tyjuliasetup/julia_src_binding.py
+-rw-r--r--   0        0        0     5207 2024-04-12 02:27:39.104721 tyjuliacall-0.7.3/tyjuliasetup/jv.py
+-rw-r--r--   0        0        0       84 2024-04-12 02:27:39.102720 tyjuliacall-0.7.3/tyjuliasetup/Project.toml
+-rw-r--r--   0        0        0    16077 2024-04-12 03:31:23.911075 tyjuliacall-0.7.3/tyjuliasetup/src/TyJuliaSetup.jl
+-rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 tyjuliacall-0.7.3/PKG-INFO
```

### Comparing `tyjuliacall-0.7.2/LICENSE` & `tyjuliacall-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.2/README.md` & `tyjuliacall-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.2/tyjuliasetup/__init__.py` & `tyjuliacall-0.7.3/tyjuliasetup/__init__.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.2/tyjuliasetup/compat.py` & `tyjuliacall-0.7.3/tyjuliasetup/compat.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.2/tyjuliasetup/julia_src_binding.py` & `tyjuliacall-0.7.3/tyjuliasetup/src/TyJuliaSetup.jl`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# this file is auto-generated from build.py
-JL_SRC = {}
-
-JL_SRC["TyJuliaSetup"] = r"""
 module TyJuliaSetup
 using TyPython
 using TyPython.CPython
 using TyPython.CPython: PyAPI, Py_NULLPTR, py_throw
 using TyPython: C
 
 if isdefined(Base, :Experimental) && isdefined(Base.Experimental, Symbol("@compiler_options"))
@@ -35,14 +31,21 @@
     tuple::Py
     int::Py
     float::Py
     str::Py
     bool::Py
     ndarray::Py
     complex::Py
+    npint32::Py
+    npint64::Py
+    npfloat64::Py
+    npfloat32::Py
+    npcomplex128::Py
+    npbool::Py
+    npstr::Py
     RequiredFromPythonAPIStruct() = new()
 end
 
 const MyPyAPI = RequiredFromPythonAPIStruct()
 
 function classof(x::Py)::Py
     Py(
@@ -155,14 +158,29 @@
             end
         end
     end
     if is_type_exact(py, MyPyAPI.tuple)
         n = length(py)
         return Tuple(reasonable_unbox(py[py_cast(Py, i-1)]) for i in 1:n)
     end
+    if is_type_exact(py, MyPyAPI.npint32) || is_type_exact(py, MyPyAPI.npint64)
+        return py_cast(Int, MyPyAPI.int(py))
+    end
+    if is_type_exact(py, MyPyAPI.npfloat64) || is_type_exact(py, MyPyAPI.npfloat32)
+        return py_cast(Float64, MyPyAPI.float(py))
+    end
+    if is_type_exact(py, MyPyAPI.npcomplex128)
+        return py_cast(ComplexF64, MyPyAPI.complex(py))
+    end
+    if is_type_exact(py, MyPyAPI.npbool)
+        return py_cast(Bool, MyPyAPI.bool(py))
+    end
+    if is_type_exact(py, MyPyAPI.npstr)
+        return py_cast(String, MyPyAPI.str(py))
+    end
     error("unbox failed: cannot convert a Python object (type: $(classof(py))) to julia value.")
 end
 
 const JNumPySupportedNumPyArrayBoxingElementTypes = Union{
     Int8, Int16, Int32, Int64, UInt8, UInt16, UInt32, UInt64,
     Float16, Float32, Float64,
     ComplexF16, ComplexF32, ComplexF64, Bool
@@ -503,14 +521,22 @@
     MyPyAPI.int = builtins.int
     MyPyAPI.float = builtins.float
     MyPyAPI.bool = builtins.bool
     MyPyAPI.str = builtins.str
     MyPyAPI.object = builtins.object
     MyPyAPI.complex = builtins.complex
     MyPyAPI.ndarray = numpy.ndarray
+    MyPyAPI.npint32 = numpy.int32
+    MyPyAPI.npint64 = numpy.int64
+    MyPyAPI.npfloat64 = numpy.float64
+    MyPyAPI.npfloat32 = numpy.float32
+    MyPyAPI.npcomplex128 = numpy.complex128
+    MyPyAPI.npbool = numpy.bool_
+    MyPyAPI.npstr = numpy.str_
+
     @export_pymodule _tyjuliacall_jnumpy begin
         setup_jv = Pyfunc(setup_jv)
         setup_basics = Pyfunc(setup_basics)
     end
     nothing
 end
 
@@ -518,9 +544,8 @@
 
 function __init__()
     empty!(_store_string_symbols)
     empty!(JlValuePools)
     empty!(JlValueUnusedSlots)
 end
 
-end
-"""
+end
```

### Comparing `tyjuliacall-0.7.2/tyjuliasetup/jv.py` & `tyjuliacall-0.7.3/tyjuliasetup/jv.py`

 * *Files identical despite different names*

### Comparing `tyjuliacall-0.7.2/tyjuliasetup/src/TyJuliaSetup.jl` & `tyjuliacall-0.7.3/tyjuliasetup/julia_src_binding.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# this file is auto-generated from build.py
+JL_SRC = {}
+
+JL_SRC["TyJuliaSetup"] = r"""
 module TyJuliaSetup
 using TyPython
 using TyPython.CPython
 using TyPython.CPython: PyAPI, Py_NULLPTR, py_throw
 using TyPython: C
 
 if isdefined(Base, :Experimental) && isdefined(Base.Experimental, Symbol("@compiler_options"))
@@ -31,14 +35,21 @@
     tuple::Py
     int::Py
     float::Py
     str::Py
     bool::Py
     ndarray::Py
     complex::Py
+    npint32::Py
+    npint64::Py
+    npfloat64::Py
+    npfloat32::Py
+    npcomplex128::Py
+    npbool::Py
+    npstr::Py
     RequiredFromPythonAPIStruct() = new()
 end
 
 const MyPyAPI = RequiredFromPythonAPIStruct()
 
 function classof(x::Py)::Py
     Py(
@@ -151,14 +162,29 @@
             end
         end
     end
     if is_type_exact(py, MyPyAPI.tuple)
         n = length(py)
         return Tuple(reasonable_unbox(py[py_cast(Py, i-1)]) for i in 1:n)
     end
+    if is_type_exact(py, MyPyAPI.npint32) || is_type_exact(py, MyPyAPI.npint64)
+        return py_cast(Int, MyPyAPI.int(py))
+    end
+    if is_type_exact(py, MyPyAPI.npfloat64) || is_type_exact(py, MyPyAPI.npfloat32)
+        return py_cast(Float64, MyPyAPI.float(py))
+    end
+    if is_type_exact(py, MyPyAPI.npcomplex128)
+        return py_cast(ComplexF64, MyPyAPI.complex(py))
+    end
+    if is_type_exact(py, MyPyAPI.npbool)
+        return py_cast(Bool, MyPyAPI.bool(py))
+    end
+    if is_type_exact(py, MyPyAPI.npstr)
+        return py_cast(String, MyPyAPI.str(py))
+    end
     error("unbox failed: cannot convert a Python object (type: $(classof(py))) to julia value.")
 end
 
 const JNumPySupportedNumPyArrayBoxingElementTypes = Union{
     Int8, Int16, Int32, Int64, UInt8, UInt16, UInt32, UInt64,
     Float16, Float32, Float64,
     ComplexF16, ComplexF32, ComplexF64, Bool
@@ -499,14 +525,22 @@
     MyPyAPI.int = builtins.int
     MyPyAPI.float = builtins.float
     MyPyAPI.bool = builtins.bool
     MyPyAPI.str = builtins.str
     MyPyAPI.object = builtins.object
     MyPyAPI.complex = builtins.complex
     MyPyAPI.ndarray = numpy.ndarray
+    MyPyAPI.npint32 = numpy.int32
+    MyPyAPI.npint64 = numpy.int64
+    MyPyAPI.npfloat64 = numpy.float64
+    MyPyAPI.npfloat32 = numpy.float32
+    MyPyAPI.npcomplex128 = numpy.complex128
+    MyPyAPI.npbool = numpy.bool_
+    MyPyAPI.npstr = numpy.str_
+
     @export_pymodule _tyjuliacall_jnumpy begin
         setup_jv = Pyfunc(setup_jv)
         setup_basics = Pyfunc(setup_basics)
     end
     nothing
 end
 
@@ -514,8 +548,9 @@
 
 function __init__()
     empty!(_store_string_symbols)
     empty!(JlValuePools)
     empty!(JlValueUnusedSlots)
 end
 
-end
+end
+"""
```

### Comparing `tyjuliacall-0.7.2/PKG-INFO` & `tyjuliacall-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyjuliacall
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python-Julia interops.
 Author: Suzhou-Tongyuan
 Author-email: support@tongyuan.cc
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

