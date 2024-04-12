# Comparing `tmp/pldag-0.5.0.tar.gz` & `tmp/pldag-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.5.0.tar", max compression
+gzip compressed data, was "pldag-0.5.1.tar", max compression
```

## Comparing `pldag-0.5.0.tar` & `pldag-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.5.0/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.5.0/README.md
--rw-r--r--   0        0        0    13024 2024-04-10 19:55:10.697572 pldag-0.5.0/pldag/__init__.py
--rw-r--r--   0        0        0      278 2024-04-10 19:49:45.884510 pldag-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.5.1/README.md
+-rw-r--r--   0        0        0    13013 2024-04-11 09:14:19.089430 pldag-0.5.1/pldag/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-11 09:15:59.480136 pldag-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.5.1/PKG-INFO
```

### Comparing `pldag-0.5.0/LICENSE` & `pldag-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.5.0/README.md` & `pldag-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.5.0/pldag/__init__.py` & `pldag-0.5.1/pldag/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,23 +71,27 @@
         """
         return self._icalias(alias) - (~self._cvec).sum()
     
     def get(self, *alias: str) -> np.ndarray:
         """Get the bounds of the given alias"""
         return self._dvec[list(map(self._icalias, alias))]
     
+    def exists(self, alias: str) -> bool:
+        """Check if the given alias exists"""
+        return (alias in self._amap) or (alias in self._imap)
+    
     def dependencies(self, alias: str) -> Dict[str, Set[str]]:
         """
             Get the dependencies of the given alias or ID.
             A mapping of ID -> {Alias} is returned, where each ID
             is a dependency to `alias`.
         """
         return dict(
             map(
-                lambda x: (x, self._rev_amap[x]),
+                lambda x: (x, self._rev_amap.get(x, set())),
                 map(
                     lambda x: list(self._imap)[x],
                     np.argwhere(self._amat[self._iralias(alias)] == 1).T[0]
                 )
             )
         )
     
@@ -102,40 +106,35 @@
         # Remove the primitive prime for all composite primes
         # May be changed later. Now we just set everything to 0
         # but keep the rows and columns
         self._amat[:, idx] = 0
     
     def set_primitive(self, alias: str, bound: complex = complex(0,1)) -> str:
         """Add a primitive prime factor matrix"""
-        if alias in self._amap:
+        if alias in self._imap:
             # Update value if already in map
             self._dvec[self._icalias(alias)] = bound
         else:
             self._amat = np.hstack((self._amat, np.zeros((self._amat.shape[0], 1), dtype=np.uint8)))
             self._dvec = np.append(self._dvec, bound)
             self._cvec = np.append(self._cvec, False)
             self._imap[alias] = self._amat.shape[1] - 1
-            self._amap[alias] = alias
 
         return alias
 
     def set_primitives(self, aliases: List[str], bound: complex = complex(0,1)) -> List[str]:
         """Add multiple primitive prime factor matrices"""
         for alias in aliases:
             self.set_primitive(alias, bound)
         return aliases
 
-    def _set_gelineq(self, children: list, bias: int, negate: bool = False, aliases: List[str] = [], force_id: Optional[str] = None) -> str:
+    def _set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
         """
             Add a composite constraint of at least `value`.
         """
-        for child_alias in children:
-            if child_alias not in self._imap:
-                self.set_primitive(child_alias)
-
         _bias = complex(*repeat(bias * (1-negate) + (bias + 1) * negate * -1, 2))
         _id = sha1(("".join(sorted(children)) + str(negate)).encode()).hexdigest() if force_id is None else force_id
         if _id in self._imap:
             arr = np.zeros(self._amat.shape[1], dtype=np.int8)
             arr[[self._imap[child] for child in children]] = 1
             self._amat[self._iralias(_id)] = arr
             self._bvec[self._iralias(_id)] = _bias
@@ -149,25 +148,19 @@
             self._amat[self._amat.shape[0] - 1] = arr
             self._dvec = np.append(self._dvec, complex(0, 1))
             self._bvec = np.append(self._bvec, _bias)
             self._nvec = np.append(self._nvec, negate)
             self._cvec = np.append(self._cvec, True)
             self._imap[_id] = self._amat.shape[1] - 1
         
-        for alias in aliases:
+        if alias is not None:
             self._amap[alias] = _id
 
         return _id
     
-    def set_atleast(self, children: list, value: int, aliases: List[str] = [], force_id: Optional[str] = None) -> str:
-        return self._set_gelineq(children, -1 * value, False, aliases, force_id)
-    
-    def set_atmost(self, children: list, value: int, aliases: List[str] = [], force_id: Optional[str] = None) -> str:
-        return self._set_gelineq(children, -1 * (value + 1), True, aliases, force_id)
-    
     @staticmethod
     def _prop_algo(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, F: np.ndarray, forced: np.ndarray, max_iterations: int = 100):
 
         """
             Propagation algorithm.
 
             A: the adjacency matrix
@@ -244,37 +237,43 @@
 
             query:  what nodes and their bound to start propagating from
 
             Returns the selected propagated bounds.
         """
         return dict(zip(self._imap.keys(), self._test(query)))
     
-    def set_or(self, references: List[str], aliases: List[str] = []) -> str:
-        return self.set_atleast(references, 1, aliases=aliases)
+    def set_atleast(self, children: list, value: int, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
+        return self._set_gelineq(children, -1 * value, False, alias, force_id)
+    
+    def set_atmost(self, children: list, value: int, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
+        return self._set_gelineq(children, -1 * (value + 1), True, alias, force_id)
+    
+    def set_or(self, references: List[str], alias: Optional[str] = None) -> str:
+        return self.set_atleast(references, 1, alias=alias)
     
-    def set_and(self, references: List[str], aliases: List[str] = []) -> str:
-        return self.set_atleast(references, len(references), aliases=aliases)
+    def set_and(self, references: List[str], alias: Optional[str] = None) -> str:
+        return self.set_atleast(references, len(references), alias=alias)
     
-    def set_not(self, references: List[str], aliases: List[str] = []) -> str:
-        return self.set_atmost(references, 0, aliases=aliases)
+    def set_not(self, references: List[str], alias: Optional[str] = None) -> str:
+        return self.set_atmost(references, 0, alias=alias)
     
-    def set_xor(self, references: List[str], aliases: List[str] = []) -> str:
+    def set_xor(self, references: List[str], alias: Optional[str] = None) -> str:
         return self.set_and([
             self.set_atleast(references, 1),
             self.set_atmost(references, 1),
-        ], aliases=aliases)
+        ], alias=alias)
     
-    def set_imply(self, condition: str, consequence: str, aliases: List[str] = []) -> str:
-        return self.set_or([self.set_not([condition]), consequence], aliases=aliases)
+    def set_imply(self, condition: str, consequence: str, alias: Optional[str] = None) -> str:
+        return self.set_or([self.set_not([condition]), consequence], alias=alias)
 
     def to_polyhedron(self, fix: dict = {}) -> tuple:
 
         """
             Returns a polyhedron of a tuple (A, b, variables) representation of the PL-DAG.
-            The variables list consists of tuples of (ID, set of aliases, bound as complex number).
+            The variables list consists of tuples of (ID, alias, bound as complex number).
 
             fix: dict of aliases to fix in the polyhedron. E.g. {"A": 1, "B": 0} fix A=1 and B=0.
         """
 
         # Create the matrix
         A = np.zeros(self._amat.shape, dtype=np.int64)
 
@@ -324,15 +323,15 @@
 
         # Create the variable list
         variables = np.array(
             list(
                 map(
                     lambda i: (
                         rimap[i],
-                        self._rev_amap.get(rimap[i], rimap[i]),
+                        self._rev_amap.get(rimap[i], {}),
                         self._dvec[i],
                     ),
                     np.array(list(self._imap.values()))
                 )
             )
         )
```

### Comparing `pldag-0.5.0/PKG-INFO` & `pldag-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

