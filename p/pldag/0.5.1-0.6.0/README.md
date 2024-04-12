# Comparing `tmp/pldag-0.5.1.tar.gz` & `tmp/pldag-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.5.1.tar", max compression
+gzip compressed data, was "pldag-0.6.0.tar", max compression
```

## Comparing `pldag-0.5.1.tar` & `pldag-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.5.1/LICENSE
--rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.5.1/README.md
--rw-r--r--   0        0        0    13013 2024-04-11 09:14:19.089430 pldag-0.5.1/pldag/__init__.py
--rw-r--r--   0        0        0      278 2024-04-11 09:15:59.480136 pldag-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3760 2024-02-18 14:10:43.601434 pldag-0.6.0/README.md
+-rw-r--r--   0        0        0    11356 2024-04-11 15:47:57.209985 pldag-0.6.0/pldag/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-12 07:24:31.257762 pldag-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 pldag-0.6.0/PKG-INFO
```

### Comparing `pldag-0.5.1/LICENSE` & `pldag-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.5.1/README.md` & `pldag-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.5.1/pldag/__init__.py` & `pldag-0.6.0/pldag/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,141 +23,123 @@
         self._dvec = np.zeros((0, ),    dtype=complex)
         # Bias vector
         self._bvec = np.zeros((0, ),    dtype=complex)
         # Boolean vector indicating if the node is a composition
         self._cvec = np.zeros((0, ),    dtype=bool)
         # Maps id's to index
         self._imap = {}
-        # Maps alias to id's
-        self._amap = {}
 
     @property
     def bounds(self) -> np.ndarray:
         """Get the bounds of all aliases"""
         return self._dvec
     
     @property
-    def aliases(self) -> List[str]:
-        """Get all aliases"""
-        return list(self._amap.keys())
+    def ids(self) -> List[str]:
+        """Get all ids"""
+        return list(self._imap.keys())
     
     @property
     def _toposort(self) -> iter:
         return TopologicalSorter(
             dict(
                 map(
                     lambda x: (x[0], set(map(lambda y: y[1], x[1]))), 
                     groupby(np.argwhere(self._amat), key=lambda x: x[0])
                 )
             )
         ).static_order()
     
-    @property
-    def _rev_amap(self) -> dict:
-        # Reversing the dictionary
-        reversed_dict = {}
-        for key, value in self._amap.items():
-            reversed_dict.setdefault(value, set()).add(key)
-        return reversed_dict
-    
-    def _icalias(self, alias: str) -> int:
+    def _icol(self, id: str) -> int:
         """
-            Returns the column index of the given alias or ID.
+            Returns the column index of the given ID.
         """
-        return self._imap[self._amap.get(alias, alias)]
+        return self._imap[id]
     
-    def _iralias(self, alias: str) -> int:
+    def _irow(self, id: str) -> int:
         """
-            Returns the row index of the given alias or ID.
+            Returns the row index of the given ID.
         """
-        return self._icalias(alias) - (~self._cvec).sum()
+        return self._icol(id) - (~self._cvec).sum()
     
-    def get(self, *alias: str) -> np.ndarray:
-        """Get the bounds of the given alias"""
-        return self._dvec[list(map(self._icalias, alias))]
+    def get(self, *id: str) -> np.ndarray:
+        """Get the bounds of the given ID(s)"""
+        return self._dvec[list(map(self._icol, id))]
     
-    def exists(self, alias: str) -> bool:
-        """Check if the given alias exists"""
-        return (alias in self._amap) or (alias in self._imap)
+    def exists(self, id: str) -> bool:
+        """Check if the given id exists"""
+        return (id in self._imap)
     
-    def dependencies(self, alias: str) -> Dict[str, Set[str]]:
+    def dependencies(self, id: str) -> Set[str]:
         """
-            Get the dependencies of the given alias or ID.
-            A mapping of ID -> {Alias} is returned, where each ID
-            is a dependency to `alias`.
+            Get the dependencies of the given ID.
         """
-        return dict(
+        return set(
             map(
-                lambda x: (x, self._rev_amap.get(x, set())),
-                map(
-                    lambda x: list(self._imap)[x],
-                    np.argwhere(self._amat[self._iralias(alias)] == 1).T[0]
-                )
+                lambda x: list(self._imap)[x],
+                np.argwhere(self._amat[self._irow(id)] == 1).T[0]
             )
         )
     
-    def negated(self, alias: str) -> bool:
-        """Get the negated state of the given alias"""
-        return bool(self._nvec[self._iralias(alias)])
-    
-    def delete(self, alias: str) -> None:
-        """Delete the given alias"""
-        idx = self._icalias(alias)
+    def negated(self, id: str) -> bool:
+        """Get the negated state of the given id"""
+        return bool(self._nvec[self._irow(id)])
+    
+    def delete(self, id: str) -> None:
+        """Delete the given id"""
+        idx = self._icol(id)
 
         # Remove the primitive prime for all composite primes
         # May be changed later. Now we just set everything to 0
         # but keep the rows and columns
         self._amat[:, idx] = 0
     
-    def set_primitive(self, alias: str, bound: complex = complex(0,1)) -> str:
+    def set_primitive(self, id: str, bound: complex = complex(0,1)) -> str:
         """Add a primitive prime factor matrix"""
-        if alias in self._imap:
+        if id in self._imap:
             # Update value if already in map
-            self._dvec[self._icalias(alias)] = bound
+            self._dvec[self._icol(id)] = bound
         else:
             self._amat = np.hstack((self._amat, np.zeros((self._amat.shape[0], 1), dtype=np.uint8)))
             self._dvec = np.append(self._dvec, bound)
             self._cvec = np.append(self._cvec, False)
-            self._imap[alias] = self._amat.shape[1] - 1
+            self._imap[id] = self._amat.shape[1] - 1
 
-        return alias
+        return id
 
-    def set_primitives(self, aliases: List[str], bound: complex = complex(0,1)) -> List[str]:
+    def set_primitives(self, ids: List[str], bound: complex = complex(0,1)) -> List[str]:
         """Add multiple primitive prime factor matrices"""
-        for alias in aliases:
-            self.set_primitive(alias, bound)
-        return aliases
+        for id in ids:
+            self.set_primitive(id, bound)
+        return ids
 
-    def _set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
+    def _set_gelineq(self, children: list, bias: int, negate: bool = False) -> str:
         """
             Add a composite constraint of at least `value`.
         """
         _bias = complex(*repeat(bias * (1-negate) + (bias + 1) * negate * -1, 2))
-        _id = sha1(("".join(sorted(children)) + str(negate)).encode()).hexdigest() if force_id is None else force_id
+        _id = sha1(("".join(sorted(children)) + str(negate)).encode()).hexdigest()
         if _id in self._imap:
             arr = np.zeros(self._amat.shape[1], dtype=np.int8)
             arr[[self._imap[child] for child in children]] = 1
-            self._amat[self._iralias(_id)] = arr
-            self._bvec[self._iralias(_id)] = _bias
-            self._nvec[self._iralias(_id)] = negate
+            self._amat[self._irow(_id)] = arr
+            self._bvec[self._irow(_id)] = _bias
+            self._nvec[self._irow(_id)] = negate
             self._dvec[self._imap[_id]] = complex(0, 1)
             self._cvec[self._imap[_id]] = True
         else:
             self._amat = np.pad(self._amat, ((0, 1), (0, 1)), mode='constant')
             arr = np.zeros(self._amat.shape[1], dtype=np.int8)
-            arr[[self._icalias(child) for child in children]] = 1
+            arr[[self._icol(child) for child in children]] = 1
             self._amat[self._amat.shape[0] - 1] = arr
             self._dvec = np.append(self._dvec, complex(0, 1))
             self._bvec = np.append(self._bvec, _bias)
             self._nvec = np.append(self._nvec, negate)
             self._cvec = np.append(self._cvec, True)
             self._imap[_id] = self._amat.shape[1] - 1
-        
-        if alias is not None:
-            self._amap[alias] = _id
 
         return _id
     
     @staticmethod
     def _prop_algo(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, F: np.ndarray, forced: np.ndarray, max_iterations: int = 100):
 
         """
@@ -201,81 +183,70 @@
         B: np.ndarray = self._bvec
         C: np.ndarray = self._cvec
         D: np.ndarray = self._dvec
         F: np.ndarray = self._nvec
 
         # Propagate the graph and store the result as new bounds
         self._dvec = self._prop_algo(A, B, C, D, F, np.zeros(D.shape[0], dtype=bool))
-    
-    def _test(self, query: Dict[str, complex]) -> np.ndarray:
-        
+
+    def test(self, query: Dict[str, complex]) -> Dict[str, complex]:
+
         """
-            Propagates the graph and returns the propagated bounds.
+            Propagates the graph and returns the selected result.
 
-            query: what nodes and their bound to start propagating from
+            query:  what nodes and their bound to start propagating from
 
-            Returns the propagated bounds.
+            Returns the selected propagated bounds.
         """
         A: np.ndarray = self._amat
         B: np.ndarray = self._bvec
         C: np.ndarray = self._cvec
         D: np.ndarray = self._dvec.copy()
         F: np.ndarray = self._nvec
 
         # Query translation into primes
         qprimes = np.zeros(D.shape[0], dtype=bool)
         qprimes[[self._imap[q] for q in query]] = True
 
         # Replace the observed bounds
         D[qprimes] = np.array(list(query.values()))
 
-        return self._prop_algo(A, B, C, D, F, qprimes)
-
-    def test(self, query: Dict[str, complex]) -> Dict[str, complex]:
-
-        """
-            Propagates the graph and returns the selected result.
-
-            query:  what nodes and their bound to start propagating from
-
-            Returns the selected propagated bounds.
-        """
-        return dict(zip(self._imap.keys(), self._test(query)))
+        return dict(zip(self._imap.keys(), self._prop_algo(A, B, C, D, F, qprimes)))
     
-    def set_atleast(self, children: list, value: int, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
-        return self._set_gelineq(children, -1 * value, False, alias, force_id)
+    def set_atleast(self, children: list, value: int) -> str:
+        return self._set_gelineq(children, -1 * value, False)
     
-    def set_atmost(self, children: list, value: int, alias: Optional[str] = None, force_id: Optional[str] = None) -> str:
-        return self._set_gelineq(children, -1 * (value + 1), True, alias, force_id)
+    def set_atmost(self, children: list, value: int) -> str:
+        return self._set_gelineq(children, -1 * (value + 1), True)
     
-    def set_or(self, references: List[str], alias: Optional[str] = None) -> str:
-        return self.set_atleast(references, 1, alias=alias)
+    def set_or(self, references: List[str]) -> str:
+        return self.set_atleast(references, 1)
     
-    def set_and(self, references: List[str], alias: Optional[str] = None) -> str:
-        return self.set_atleast(references, len(references), alias=alias)
+    def set_and(self, references: List[str]) -> str:
+        return self.set_atleast(references, len(references))
     
-    def set_not(self, references: List[str], alias: Optional[str] = None) -> str:
-        return self.set_atmost(references, 0, alias=alias)
+    def set_not(self, references: List[str]) -> str:
+        return self.set_atmost(references, 0)
     
-    def set_xor(self, references: List[str], alias: Optional[str] = None) -> str:
+    def set_xor(self, references: List[str]) -> str:
         return self.set_and([
             self.set_atleast(references, 1),
             self.set_atmost(references, 1),
-        ], alias=alias)
+        ])
     
-    def set_imply(self, condition: str, consequence: str, alias: Optional[str] = None) -> str:
-        return self.set_or([self.set_not([condition]), consequence], alias=alias)
+    def set_imply(self, condition: str, consequence: str) -> str:
+        return self.set_or([self.set_not([condition]), consequence])
 
     def to_polyhedron(self, fix: dict = {}) -> tuple:
 
         """
             Returns a polyhedron of a tuple (A, b, variables) representation of the PL-DAG.
-            The variables list consists of tuples of (ID, alias, bound as complex number).
+            The variables list consists of tuples of (ID, bound as complex number).
 
-            fix: dict of aliases to fix in the polyhedron. E.g. {"A": 1, "B": 0} fix A=1 and B=0.
+            fix: dict of ids to fix in the polyhedron. E.g. {"A": 1, "B": 0} fix A=1 and B=0.
         """
 
         # Create the matrix
         A = np.zeros(self._amat.shape, dtype=np.int64)
 
         # Adjacent points
         adj_points = np.argwhere(self._amat == 1)
@@ -305,15 +276,15 @@
         # by the flipped minimum value
         b = eq_bounds.real - self._bvec.real
 
         # Fix the columns in `fix`
         for i, vs in groupby(zip(fix.values(), fix.keys()), key=lambda x: x[0]):
             v = list(map(lambda x: x[1], vs))
             a = np.zeros(A.shape[1], dtype=np.int64)
-            a[np.array(list(map(self._icalias, v)))] = 1
+            a[np.array(list(map(self._icol, v)))] = 1
             if i > 0 or i < 0:
                 _b = a.sum() * i
             else:
                 _b = 0
 
             A = np.vstack([A, a])
             b = np.append(b, _b)
@@ -323,15 +294,14 @@
 
         # Create the variable list
         variables = np.array(
             list(
                 map(
                     lambda i: (
                         rimap[i],
-                        self._rev_amap.get(rimap[i], {}),
                         self._dvec[i],
                     ),
                     np.array(list(self._imap.values()))
                 )
             )
         )
```

### Comparing `pldag-0.5.1/PKG-INFO` & `pldag-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

