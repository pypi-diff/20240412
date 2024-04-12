# Comparing `tmp/kgprim-0.1.0.tar.gz` & `tmp/kgprim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgprim-0.1.0.tar", last modified: Mon Sep  5 16:03:23 2022, max compression
+gzip compressed data, was "kgprim-0.1.1.tar", last modified: Fri Apr 12 13:06:05 2024, max compression
```

## Comparing `kgprim-0.1.0.tar` & `kgprim-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     1505 2022-07-15 14:33:22.000000 kgprim-0.1.0/LICENSE
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     1978 2022-09-05 16:03:23.475985 kgprim-0.1.0/PKG-INFO
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      514 2022-09-05 15:59:49.000000 kgprim-0.1.0/pyproject.toml
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)       38 2022-09-05 16:03:23.475985 kgprim-0.1.0/setup.cfg
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.471985 kgprim-0.1.0/src/
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.471985 kgprim-0.1.0/src/kgprim/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)       64 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/__init__.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     4095 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/core.py
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/src/kgprim/ct/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      534 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/__init__.py
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/src/kgprim/ct/backend/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      307 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/backend/__init__.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      797 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/ct/backend/numeric.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     3032 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/ct/backend/symbolic.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     6768 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/frommotions.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     5921 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/metadata.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     4085 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/models.py
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/src/kgprim/ct/repr/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      268 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/repr/__init__.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      593 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/ct/repr/homogeneous.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     1753 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/ct/repr/mxcommon.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     5500 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/ct/repr/mxrepr.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     4779 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/ct/repr/spatial.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     8546 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/kgprim/motions.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     7896 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/kgprim/values.py
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/src/kgprim.egg-info/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     1978 2022-09-05 16:03:23.000000 kgprim-0.1.0/src/kgprim.egg-info/PKG-INFO
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)      717 2022-09-05 16:03:23.000000 kgprim-0.1.0/src/kgprim.egg-info/SOURCES.txt
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)        1 2022-09-05 16:03:23.000000 kgprim-0.1.0/src/kgprim.egg-info/dependency_links.txt
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)       27 2022-09-05 16:03:23.000000 kgprim-0.1.0/src/kgprim.egg-info/requires.txt
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)       17 2022-09-05 16:03:23.000000 kgprim-0.1.0/src/kgprim.egg-info/top_level.txt
-drwxrwxr-x   0 marco-rov  (1004) marco-rov  (1004)        0 2022-09-05 16:03:23.475985 kgprim-0.1.0/src/motiondsl/
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     1405 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/motiondsl/__init__.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     4566 2022-07-15 14:33:22.000000 kgprim-0.1.0/src/motiondsl/motiondsl.py
--rw-rw-r--   0 marco-rov  (1004) marco-rov  (1004)     2129 2020-08-04 13:22:45.000000 kgprim-0.1.0/src/motiondsl/motiondsl.tx
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     1505 2024-04-12 12:57:17.000000 kgprim-0.1.1/LICENSE
+-rw-r--r--   0 marco-irs  (1001) marco-irs  (1001)     2065 2024-04-12 13:06:05.131988 kgprim-0.1.1/PKG-INFO
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      514 2024-04-12 12:59:05.000000 kgprim-0.1.1/pyproject.toml
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)       38 2024-04-12 13:06:05.131988 kgprim-0.1.1/setup.cfg
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.127988 kgprim-0.1.1/src/
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.127988 kgprim-0.1.1/src/kgprim/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)       64 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/__init__.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     4095 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/core.py
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/src/kgprim/ct/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      552 2023-09-19 10:20:19.000000 kgprim-0.1.1/src/kgprim/ct/__init__.py
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/src/kgprim/ct/backend/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      307 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/backend/__init__.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      813 2024-04-12 12:31:59.000000 kgprim-0.1.1/src/kgprim/ct/backend/numeric.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     3032 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/backend/symbolic.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     6768 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/frommotions.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     9366 2024-04-12 12:54:43.000000 kgprim-0.1.1/src/kgprim/ct/metadata.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     4085 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/models.py
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/src/kgprim/ct/repr/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      268 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/repr/__init__.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      593 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/repr/homogeneous.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     1753 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/repr/mxcommon.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     5500 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/repr/mxrepr.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     4779 2022-12-16 13:47:13.000000 kgprim-0.1.1/src/kgprim/ct/repr/spatial.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     9733 2024-04-12 12:54:43.000000 kgprim-0.1.1/src/kgprim/motions.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     7962 2024-04-12 12:54:00.000000 kgprim-0.1.1/src/kgprim/values.py
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/src/kgprim.egg-info/
+-rw-r--r--   0 marco-irs  (1001) marco-irs  (1001)     2065 2024-04-12 13:06:05.000000 kgprim-0.1.1/src/kgprim.egg-info/PKG-INFO
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)      717 2024-04-12 13:06:05.000000 kgprim-0.1.1/src/kgprim.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)        1 2024-04-12 13:06:05.000000 kgprim-0.1.1/src/kgprim.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)       27 2024-04-12 13:06:05.000000 kgprim-0.1.1/src/kgprim.egg-info/requires.txt
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)       17 2024-04-12 13:06:05.000000 kgprim-0.1.1/src/kgprim.egg-info/top_level.txt
+drwxrwxr-x   0 marco-irs  (1001) marco-irs  (1001)        0 2024-04-12 13:06:05.131988 kgprim-0.1.1/src/motiondsl/
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     1510 2024-04-12 12:54:00.000000 kgprim-0.1.1/src/motiondsl/__init__.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     5950 2024-04-12 12:54:43.000000 kgprim-0.1.1/src/motiondsl/motiondsl.py
+-rw-rw-r--   0 marco-irs  (1001) marco-irs  (1001)     2154 2024-04-12 12:54:00.000000 kgprim-0.1.1/src/motiondsl/motiondsl.tx
```

### Comparing `kgprim-0.1.0/LICENSE` & `kgprim-0.1.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2022, Marco Frigerio
+Copyright (c) 2020-2024, Marco Frigerio
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
```

### Comparing `kgprim-0.1.0/PKG-INFO` & `kgprim-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kgprim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Kinematics/geometric primitives
 Author-email: Marco Frigerio <marco.frigerio17@pm.me>
-License: Copyright (c) 2020-2022, Marco Frigerio
+License: Copyright (c) 2020-2024, Marco Frigerio
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright
            notice, this list of conditions and the following disclaimer.
@@ -30,7 +30,11 @@
         ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: home, https://github.com/mfrigerio17/kgprim
 Requires-Python: >=3.3
 License-File: LICENSE
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: textX
```

### Comparing `kgprim-0.1.0/pyproject.toml` & `kgprim-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name        = "kgprim"
-version     = "0.1.0"
+version     = "0.1.1"
 description = "Kinematics/geometric primitives"
 authors     = [
     { name = "Marco Frigerio", email = "marco.frigerio17@pm.me" }
 ]
 
 license = { file = "LICENSE" }
```

### Comparing `kgprim-0.1.0/src/kgprim/core.py` & `kgprim-0.1.1/src/kgprim/core.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/__init__.py` & `kgprim-0.1.1/src/kgprim/ct/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 This package contains facilities to represent coordinate-transform objects, with
 explicit semantics. The subpackages `kgprim.ct.repr` and `kgprim.ct.backend`
 allow to get the concrete matrix representation of a transform.
 
 The module `kgprim.ct.frommotions` allows to compute the coordinate transform(s)
 associated with a rigid motion model from the module `kgprim.motions`.
 
-See the file `test/ct/sample.py`:
+See the file `sample/kgprim/ct/sample.py`:
 
 ```python
-.. include:: ../../../test/ct/sample.py
+.. include:: ../../../sample/kgprim/ct/sample.py
 ```
 
 '''
```

### Comparing `kgprim-0.1.0/src/kgprim/ct/backend/numeric.py` & `kgprim-0.1.1/src/kgprim/ct/backend/numeric.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,12 +16,12 @@
         mx = self.identity()
         for p in ct.primitives :
             amount = p.amount
             if isinstance(amount, myexpr.Expression) :
                 try:
                     amount = amount.evalf()
                 except RuntimeError as e:
-                    raise RuntimeError('Could not compute numeric matrix representation: ' + e.msg())
+                    raise RuntimeError('Could not compute the numeric matrix representation of the transform') from e
             mx = mx @ self.matrix[p.kind](p.axis, p.polarity, amount)
         return mx
     # self.matrix comes from the MatrixRepresentationMixin
```

### Comparing `kgprim-0.1.0/src/kgprim/ct/backend/symbolic.py` & `kgprim-0.1.1/src/kgprim/ct/backend/symbolic.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/frommotions.py` & `kgprim-0.1.1/src/kgprim/ct/frommotions.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/metadata.py` & `kgprim-0.1.1/src/kgprim/ct/metadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,43 +9,121 @@
     Metadata of a single coordinate transform model.
 
     A metadata object contains the set of variables, parameters and constants
     which are part of the transform, and also two flags to tell whether the
     transform is parametric or constant.
     '''
 
-    def __init__(self, coordinateTransform):
+    def __init__(self, coordinateTransform, customName=None):
         self.vars, self.pars, self.consts =\
                                symbolicArgumentsOf(coordinateTransform)
         self.ct = coordinateTransform
         self.parametric = (len(self.pars)>0)
         self.constant   = (len(self.vars)==0 and len(self.pars)==0)
+        self._name      = customName or str(self.ct)
 
     @property
-    def name(self): return str(self.ct)
+    def name(self): return self._name
+
+    @property
+    def is_parametric(self): return self.parametric
+
+    @property
+    def is_constant(self): return self.constant
+
+    @property
+    def is_dependent(self):
+        '''Tell whether this transform depends on any Variable.'''
+        return len(self.vars)>0
+
+    @property
+    def variables(self):
+        '''
+        Return a view of the set of Variables this transform depends on.
+        The set is ordered. See the description of the keys of the dictionaries
+        in `symbolicArgumentsOf()`.
+        '''
+        return self.vars.keys()
+
+    @property
+    def parameters(self):
+        '''
+        Return a view of the set of Parameters this transform depends on.
+        The set is ordered. See the description of the keys of the dictionaries
+        in `symbolicArgumentsOf()`.
+        '''
+        return self.pars.keys()
+
+    @property
+    def constants(self):
+        '''
+        Return a view of the set of Constants that appear in this transform.
+        The set is ordered. See the description of the keys of the dictionaries
+        in `symbolicArgumentsOf()`.
+        '''
+        return self.consts.keys()
+
+    @property
+    def variable_expressions(self):
+        '''
+        The dictionary with the variables and the corresponding expressions
+        appearing in this transform.
+        See `symbolicArgumentsOf()` for the format of the dictionary.
+        '''
+        return self.vars
+
+    @property
+    def parameter_expressions(self):
+        '''
+        The dictionary with the parameters and the corresponding expressions
+        appearing in this transform.
+        See `symbolicArgumentsOf()` for the format of the dictionary.
+        '''
+        return self.pars
+
+    @property
+    def constant_expressions(self):
+        '''
+        The dictionary with the constants and the corresponding expressions
+        appearing in this transform.
+        See `symbolicArgumentsOf()` for the format of the dictionary.
+        '''
+        return self.consts
 
 
 class TransformsModelMetadata:
     '''
     Metadata for a whole transforms-model (that is, a set of transforms)
     '''
 
-    def __init__(self, ctmodel):
+    def __init__(self, ctmodel, tfNamesMap=None):
+        '''
+        Arguments
+          - `ctmodel`: the coordinate-transforms container, an instance of
+            `models.CTransformsModel`
+          - `tfNamesMap`: an optional dictionary with custom names for each
+            transform in the given model. The dictionary is keyed with tuples
+            with the left and right-frame (in this order) of the transform to
+            be named.
+        '''
+
         variables    = OrderedDict()
         parameters   = OrderedDict()
         constants    = OrderedDict()
         transforms = []
         def add(container, argument, expressions):
             if argument not in container.keys():
                 container[ argument ] = expressions
             else :
                 container[ argument ].update( expressions )
 
+        names = tfNamesMap or {}
         for transf in ctmodel.transforms :
-            tinfo = TransformMetadata(transf)
+            name  = names.get( (transf.leftFrame, transf.rightFrame) ) # 'get' defaults to None
+            tinfo = TransformMetadata(transf, customName=name)
             for var, expressions in tinfo.vars.items() :
                 add( variables, var, expressions )
                 #rotOrTr(tinfo, var)
             for par, expressions in tinfo.pars.items() :
                 add( parameters, par, expressions )
 #                     if rotOrTr(tinfo, par) : #it is a rotation
 #                         rotationPars.append( par )
@@ -73,33 +151,43 @@
 class UniqueExpression:
     '''
     Wraps a `kgprim.values.Expression` after stripping any leading minus.
     Expressions like `2*x` and `-2*x` would lead to two instances
     of this class that compare equal.
 
     Arguments:
-    - `ctPrimitive` a primitive transform having an expression as argument
-    '''
-
-    def __init__(self, ctPrimitive ):
-        if not isinstance(ctPrimitive.amount, numeric_argument.Expression) :
-            raise RuntimeError('Need to pass a transform with an Expression as argument')
-
-        original = ctPrimitive.amount
-        # Sympy specifics here... might not be very robust...
-        # Essentially we want to isolate the same Expression but without any
-        # '-' in front
-        # We rely on the fact that the sympy epressions coming from an input
-        # geometry model are not more complicated than 'coefficient * symbol'
-        (mult, rest) = original.expr.as_coeff_mul()
-        sympynew = abs(mult) * rest[0] # [0] here, assumption is that there is only one term other than the multiplier
-        expression = numeric_argument.Expression(argument=original.arg, sympyExpr=sympynew)
-
-        self.expression = expression
-        self.rotation   = (ctPrimitive.kind == MotionStep.Kind.Rotation)
+    - `arg` a `kgprim.ct.models.PrimitiveCTransform` whose motion-step has an
+      expression as argument; alternatively, a `kgprim.motions.MotionStep`
+      object right away
+    '''
+
+    def __init__(self, arg ):
+        try:
+            src_expr = arg.amount # works for both PrimitiveCTransform and MotionStep
+
+            # Sympy specifics here... might not be very robust...
+            # Essentially we want to isolate the same Expression but without any
+            # '-' in front
+            # We rely on the fact that the sympy epressions coming from an input
+            # geometry model are not more complicated than 'coefficient * symbol'.
+            # Explicitly passing 'symbol' makes it work also when the
+            # coefficient is a float rather than rational (e.g. "0.5*pi" as
+            # opposed to "pi/2").
+
+            (mult, rest) = src_expr.expr.as_coeff_mul( src_expr.arg.symbol )
+            if len(rest) > 1 :
+                raise RuntimeError("Could not separate the coefficient in expression {}".format(src_expr.expr))
+            # we assume there is only one term other than the multiplier
+            sympynew = abs(mult) * rest[0]
+            expression = numeric_argument.Expression(argument=src_expr.arg, sympyExpr=sympynew)
+
+            self.expression = expression
+            self.rotation   = (arg.kind == MotionStep.Kind.Rotation)
+        except AttributeError as e:
+            raise ValueError("Incompatible argument type given to UniqueExpression()") from e
 
     @property
     def symbolicExpr(self):
         '''The underlying Sympy expression'''
         return self.expression.expr
 
     def isRotation(self): return self.rotation
@@ -125,37 +213,41 @@
     (`kgprim.values.Variable`, `kgprim.values.Parameter`, and
     `kgprim.values.Constant`). Occurrences of pi and raw floating point values
     are never included.
     The keys are stored in the same order as they appear in the transform (e.g.
     if the transform is a rotation of r radians followed by a translation of t
     meters, r will appear before t).
 
-    The values in the dictionaries are sets, containing all the unique
-    expressions having the corresponding key as an argument. Expressions
+    The values in the dictionaries are also sorted containers, with all the
+    unique expressions having the corresponding key as an argument. Expressions
     differing only for the sign are considered the same.
     For example, if the transform is defined as `rotx(2r) roty(3r) rotz(-2r)`,
-    the set corresponding to `r` will contain `2r` and `3r`.
+    the container corresponding to `r` will contain `2r` and `3r`.
     '''
     varss = OrderedDict()
     pars  = OrderedDict()
     consts= OrderedDict()
     for pct in coordinateTransform.primitives :
         if isinstance(pct.amount, numeric_argument.Expression) :
             arg = pct.amount.arg
             rtexpr = UniqueExpression(pct)
 
+        # Use ordered dictionaries with no values to emulate sorted sets.
+        # Iteration over a dictionary itself (no keys() nor values() ) defaults
+        # to iteration over the keys, so it would appear to be an ordered
+        # sequence, with no duplicates, as I want.
             if isinstance(arg, numeric_argument.Variable) :
-                if arg not in varss : varss[ arg ] = set()
-                varss.get( arg ).add( rtexpr )
+                if arg not in varss : varss[ arg ] = OrderedDict()
+                varss.get( arg ) [rtexpr] = None
             elif isinstance(arg, numeric_argument.Parameter) :
-                if arg not in pars : pars[ arg ] = set()
-                pars.get( arg ).add( rtexpr )
+                if arg not in pars : pars[ arg ] = OrderedDict()
+                pars.get( arg ) [rtexpr] = None
             elif isinstance(arg, numeric_argument.Constant) :
-                if arg not in consts : consts[ arg ] = set()
-                consts.get( arg ).add( rtexpr )
+                if arg not in consts : consts[ arg ] = OrderedDict()
+                consts.get( arg ) [rtexpr] = None
     return varss, pars, consts
```

### Comparing `kgprim-0.1.0/src/kgprim/ct/models.py` & `kgprim-0.1.1/src/kgprim/ct/models.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/repr/homogeneous.py` & `kgprim-0.1.1/src/kgprim/ct/repr/homogeneous.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/repr/mxcommon.py` & `kgprim-0.1.1/src/kgprim/ct/repr/mxcommon.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/repr/mxrepr.py` & `kgprim-0.1.1/src/kgprim/ct/repr/mxrepr.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/ct/repr/spatial.py` & `kgprim-0.1.1/src/kgprim/ct/repr/spatial.py`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/kgprim/motions.py` & `kgprim-0.1.1/src/kgprim/motions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 '''
-Rigid motion models: "primitive" motions like pure
-translations/rotations, and sequences of them.
+This module contains types to represent symbolically rigid motions.
+Motions are pure translations/rotations ("primitive" motions), and sequences
+of them.
 
 A sequence of rigid motions is really a specification of a relative pose
 between Cartesian frames: the motions required to move from A to B identify
 the pose of B relative to A. Conversely, the pose of B relative to A could be
 _defined_ with a sequence of rigid motions that bring A to coincide with B.
+Therefore, these docs may use the term 'motion' and 'pose-specification'
+interchangeably.
 
-Therefore, in this and related modules the term 'motion' and
-'pose-specification' may be used as synonyms.
+Rigid motion models (relative poses) can be turned into concrete
+representations such as coordinate transforms. This is in fact a typical use
+case. See the package `kgprim.ct` and the module `kgprim.ct.frommotions`.
+
+The package `motiondsl` offers a simple textual format to conveniently load
+motion objects.
 '''
 
 from enum import Enum
 from kgprim.core import Frame
 from kgprim.core import Pose
 
 
@@ -179,48 +186,71 @@
     A relative Pose augmented with the corresponding motion description.
 
     A sequence of rigid motions is really a specification of a relative pose
     between Cartesian frames: the motions required to move from A to B identify
     the pose of B relative to A.
     '''
 
-    def __init__(self, pose, motion):
+    def __init__(self, pose, motion, name=None):
+        '''
+        Arguments:
+        - pose: the `kgprim.core.Pose` instance you want to describe
+        - motion: an instance of `MotionSequence` or `MotionPath`, which lists
+          the motion-steps defining the pose
+        '''
         self._pose   = pose
         self._motion = motion
+        self._name = name
+
     @property
     def pose(self): return self._pose
 
     @property
     def motion(self): return self._motion
 
-
+    @property
+    def name(self): return self._name
 
 def inversePoseSpec(poseSpec):
     pose = Pose(target=poseSpec.pose.reference, reference=poseSpec.pose.target)
     motion = reverse(poseSpec.motion)
-    return PoseSpec(pose, motion)
+    name = None
+    if poseSpec.name is not None:
+        name = f"inverse-of-{poseSpec.name}"
+    return PoseSpec(pose, motion, name)
 
 
 
 class PosesSpec:
     '''
     A simple named container for a list of `PoseSpec` instances.
     '''
 
     def __init__(self, name, poses):
-        self.name = name
-        self.poses = poses
+        self._name = name
+        self._poses = poses
 
     def mergeModel(self, otherModel, name=None):
         if name is None:
             name = self.name + '_' + otherModel.name
         poses = self.poses.copy() # A shallow copy
         poses.extend( otherModel.poses ) # only works for lists !
         return PosesSpec(name, poses)
 
+    @property
+    def name(self):
+        '''The name given to this container'''
+        return self._name
+
+    @property
+    def poses(self):
+        '''The list of `PoseSpec` in this container'''
+        return self._poses
+
+    #TODO operator[] and such, to make it act as the list
 
 
 import networkx as nx
 
 class ConnectedFramesInspector:
     '''
     An inspector to determine which additional poses can be induced from an
@@ -259,9 +289,10 @@
         motions = []
         for v1,v2 in zip(path, path[1:]) :
             edgedata = self.graph.edges[v1,v2]
             motions.append(edgedata['motion'])
 
         pose = Pose(target=targetFrame, reference=referenceFrame)
         return PoseSpec(pose=pose, motion=MotionPath(motions))
-
+        # TODO: return the original PoseSpec, if there is one that matches the
+        # given frames, instead of recreating it
```

### Comparing `kgprim-0.1.0/src/kgprim/values.py` & `kgprim-0.1.1/src/kgprim/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     Like `Variable`, this class is also a simple wrapper of a Sympy symbol.
     '''
 
     def __init__(self, name, symbol=None, defValue=None):
         self.name_   = name
         self.symbol_ = symbol or sp.Symbol(name=name)
-        self.defaultValue = defValue
+        self.dvalue_ = defValue
 
     @property
     def name(self):
         return self.name_
 
     @property
     def symbol(self):
@@ -82,14 +82,18 @@
     @property
     def expr(self):
         return self.symbol
     @property
     def constant(self):
         return False
 
+    @property
+    def defaultValue(self):
+        return self.dvalue_
+
     def __eq__(self, rhs):
         return (isinstance(rhs, Parameter)
                 and (self.name == rhs.name)
                 and (self.symbol  == rhs.symbol))
     def __hash__(self) :
         return 101*hash(self.name) + 11*hash(self.symbol)
     def __str__(self):
```

### Comparing `kgprim-0.1.0/src/kgprim.egg-info/PKG-INFO` & `kgprim-0.1.1/src/kgprim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kgprim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Kinematics/geometric primitives
 Author-email: Marco Frigerio <marco.frigerio17@pm.me>
-License: Copyright (c) 2020-2022, Marco Frigerio
+License: Copyright (c) 2020-2024, Marco Frigerio
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright
            notice, this list of conditions and the following disclaimer.
@@ -30,7 +30,11 @@
         ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: home, https://github.com/mfrigerio17/kgprim
 Requires-Python: >=3.3
 License-File: LICENSE
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: textX
```

### Comparing `kgprim-0.1.0/src/kgprim.egg-info/SOURCES.txt` & `kgprim-0.1.1/src/kgprim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kgprim-0.1.0/src/motiondsl/__init__.py` & `kgprim-0.1.1/src/motiondsl/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     fF -> fG : roty(q1)
 
 Identifiers appearing as the argument of a motion step are interpreted as
 variables. The corresponding `kgprim.motions.MotionStep` object created when
 loading the document will have a `kgprim.values.Variable` instance as the value
 of its `amount` member.
 
-See the file `sample/sample.motdsl` for a slightly larger sample.
+See the file `sample/motiondsl/model.motdsl` for a slightly larger sample. See
+also `sample/motiondsl/sample.py` for an example of how to read the model with
+Python code.
 
 While this package depends on the `kgprim.motions` module, the
 converse is not true.
 
 We use [textX](https://github.com/textX/textX) to create the parser of the
 language.
 '''
```

### Comparing `kgprim-0.1.0/src/motiondsl/motiondsl.py` & `kgprim-0.1.1/src/motiondsl/motiondsl.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 
 The module-level member `dsl` is the default instance of the `MotionDSL` class.
 Normally, you will only need this preallocated instance to load a document in
 the MotionDSL format.
 
 For example:
 
-    import os, sys
-    import motiondsl.motiondsl as motdsl
+```python
+import os, sys
+import motiondsl.motiondsl as motdsl
+
+def main():
+    if len(sys.argv) > 1 :
+        ifile = sys.argv[1]
+    else :
+        ifile = os.path.join( os.path.dirname(__file__), 'sample.motdsl')
+
+    # Load the motions-model from the input file
+    motionsModel = motdsl.dsl.modelFromFile(ifile)
+
+    print("Motions (poses) model name: ", motionsModel.name)
+
+    # Convert the motions-model to a pose-specification model
+    posesModel = motdsl.toPosesSpecification(motionsModel)
+```
 
-    def main():
-        if len(sys.argv) > 1 :
-            ifile = sys.argv[1]
-        else :
-            ifile = os.path.join( os.path.dirname(__file__), 'sample.motdsl')
-
-        # Load the motions-model from the input file
-        motionsModel = motdsl.dsl.modelFromFile(ifile)
-
-        print("Motions (poses) model name: ", motionsModel.name)
-
-        # Convert the motions-model to a pose-specification model
-        posesModel = motdsl.toPosesSpecification(motionsModel)
+See also the files in the `sample/motiondsl` folder.
 '''
 
 import sympy as sp
 import os
 import textx
 import kgprim.core as primitives
 from kgprim.values import Variable
@@ -47,19 +51,22 @@
         return arg
     else:
         return Expression(arg)
 
 class MotionDSL:
     def __init__(self):
         here = os.path.dirname(os.path.abspath(__file__))
-        self.mm = textx.metamodel_from_file(here+"/motiondsl.tx")
+        self.mm = textx.metamodel_from_file(here+"/motiondsl.tx", auto_init_attributes=False)
+        # disable auto-init so that optional attributes (like the default value
+        # of a parameter) will be 'None' when not specified in the input model
+
         obj_processors = {
             'PILiteral': lambda _ : MyPI.instance(),
             'Variable' : lambda x : Variable(name=x.name),
-            'Parameter': lambda x : Parameter(name=x.name),
+            'Parameter': lambda x : Parameter(name=x.name, defValue=x.defvalue),
             'UserConstant': lambda x : Constant(name=x.name, value=x.value),
             'RefToConstant': lambda x : Constant(name=x.actual.name, value=x.actual.value),
 
             # the following result in a float or an Expression object
             'PlainExpr' : lambda e: (-1 if e.minus else 1) * _argValue( e.arg ),
             'MultExpr'  : lambda e: e.mult * _argValue( e.arg ),
             'DivExpr'   : lambda e: (-1 if e.minus else 1)* _argValue( e.arg ) / e.div,
@@ -80,14 +87,18 @@
 
         Arguments:
           - `file`: path of a MotionDSL document (i.e. a text file)
         '''
         return self.mm.model_from_file(file)
 
 
+    def modelFromText(self, text):
+        return self.mm.model_from_str(text)
+
+
 dsl = MotionDSL()
 
 __mode_map = {
     "currentFrame" : MotionSequence.Mode.currentFrame,
     "fixedFrame"   : MotionSequence.Mode.fixedFrame
 }
 
@@ -102,15 +113,15 @@
     mode = __mode_map[ dslmodel.convention ]
     poses = []
     for m in dslmodel.motions :
         ref  = primitives.Frame(m.start.name)
         tgt  = primitives.Frame(m.end.name)
         pose = primitives.Pose(target=tgt, reference=ref)
         motSeq = MotionSequence( m.primitiveMotions, mode)
-        poses.append( PoseSpec(pose=pose, motion=motSeq) )
+        poses.append( PoseSpec(pose=pose, motion=motSeq, name=m.userName) )
 
     return PosesSpec(name=dslmodel.name, poses=poses)
 
 
 
 __ser_map = {
     MotionStep.Kind.Translation : {
@@ -121,17 +132,49 @@
     MotionStep.Kind.Rotation : {
         Axis.X : 'rotx',
         Axis.Y : 'roty',
         Axis.Z : 'rotz',
     },
 }
 
+
+def _isIdentity(expr):
+    return expr.expr == expr.arg.symbol
+
+def expressionToMotionDSLSnippet(expr):
+    if isinstance(expr, float):
+        return expr.__str__()
+    if expr.constant() :
+        if expr.arg.name == "pi":
+            return expr.__str__()
+        if _isIdentity(expr):
+            return "c:{}:{}".format(expr.arg.name, expr.evalf())
+        else:
+            cref = "c:" + expr.arg.name
+            return expr.__str__().replace(expr.arg.name, cref)
+    elif isinstance(expr.arg, Parameter):
+        pref = "p:" + expr.arg.name
+        if expr.arg.defaultValue is not None:
+            pref = pref + f"[{expr.arg.defaultValue}]"
+        return expr.__str__().replace(expr.arg.name, pref)
+    else:
+        return expr.__str__()
+
 def poseSpecToMotionDSLSnippet(poseSpec):
     tgtF = poseSpec.pose.target
     refF = poseSpec.pose.reference
-    path = ""
+    steps = []
     for seq in poseSpec.motion.sequences :
         for step in seq.steps :
-            path = path + ' {step}({amount})'.format(step=__ser_map[step.kind][step.axis], amount=step.amount.__str__())
-    ret = '{ref} -> {tgt} : {path}'.format(ref=refF.name, tgt=tgtF.name, path=path)
+            steps.append("{step}({amount})".format(
+                step   = __ser_map[step.kind][step.axis],
+                amount = expressionToMotionDSLSnippet(step.amount))
+            )
+    ret = '{ref} -> {tgt} : {path}'.format(ref=refF.name, tgt=tgtF.name, path=" ".join(steps))
     return ret
 
+
+def snippetToPoseSpec(text):
+    preable = '''Model __tmp__\nConvention = currentFrame\n\n'''
+    model_text = preable + text
+    poses = toPosesSpecification( dsl.mm.model_from_str(model_text) )
+    return poses.poses[0]
```

### Comparing `kgprim-0.1.0/src/motiondsl/motiondsl.tx` & `kgprim-0.1.1/src/motiondsl/motiondsl.tx`

 * *Files 5% similar despite different names*

```diff
@@ -66,11 +66,11 @@
 Value : Constant | Parameter | Variable;
 
 Constant : FLOAT | PILiteral | UserConstant | RefToConstant;
 
 PILiteral : /[P|p][I|i]/ ;
 UserConstant : "c:" name=ID ":" value=FLOAT;
 RefToConstant: "c:" actual=[UserConstant];
-Parameter : !PILiteral "p:"name=ID;
+Parameter : !PILiteral "p:"name=ID ('['defvalue=NUMBER']')?;
 Variable  : !PILiteral !Parameter name=ID;
 
 Comment: /\/\/.*$/;
```

