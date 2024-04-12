# Comparing `tmp/codegen_2-2.1.1.tar.gz` & `tmp/codegen_2-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegen_2-2.1.1.tar", max compression
+gzip compressed data, was "codegen_2-2.1.2.tar", max compression
```

## Comparing `codegen_2-2.1.1.tar` & `codegen_2-2.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-04-11 00:16:20.368382 codegen_2-2.1.1/LICENSE
--rw-r--r--   0        0        0       27 2024-04-11 00:16:20.368382 codegen_2-2.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/__init__.py
--rw-r--r--   0        0        0      457 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/__init__.py
--rw-r--r--   0        0        0     7702 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/ast.py
--rw-r--r--   0        0        0     5273 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/expr.py
--rw-r--r--   0        0        0     4471 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/program.py
--rw-r--r--   0        0        0     2899 2024-04-11 00:16:20.368382 codegen_2-2.1.1/codegen/models/statement.py
--rw-r--r--   0        0        0      178 2024-04-11 00:16:20.372382 codegen_2-2.1.1/codegen/models/types.py
--rw-r--r--   0        0        0     1771 2024-04-11 00:16:20.372382 codegen_2-2.1.1/codegen/models/var.py
--rw-r--r--   0        0        0      422 2024-04-11 00:16:20.372382 codegen_2-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 codegen_2-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-12 15:33:51.405367 codegen_2-2.1.2/LICENSE
+-rw-r--r--   0        0        0       27 2024-04-12 15:33:51.405367 codegen_2-2.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/__init__.py
+-rw-r--r--   0        0        0     7816 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/ast.py
+-rw-r--r--   0        0        0     5273 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/expr.py
+-rw-r--r--   0        0        0     4471 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/program.py
+-rw-r--r--   0        0        0     2899 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/statement.py
+-rw-r--r--   0        0        0      178 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/types.py
+-rw-r--r--   0        0        0     1771 2024-04-12 15:33:51.405367 codegen_2-2.1.2/codegen/models/var.py
+-rw-r--r--   0        0        0      422 2024-04-12 15:33:51.405367 codegen_2-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 codegen_2-2.1.2/PKG-INFO
```

### Comparing `codegen_2-2.1.1/LICENSE` & `codegen_2-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.1/codegen/models/ast.py` & `codegen_2-2.1.2/codegen/models/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     DefFuncStatement,
     ElseStatement,
     ExceptionStatement,
     ForLoopStatement,
     IfStatement,
     ImportStatement,
     LineBreak,
+    NoStatement,
     PythonStatement,
     ReturnStatement,
     SingleExprStatement,
     Statement,
 )
 from codegen.models.types import AST_ID
 from codegen.models.var import DeferredVar, Var, VarScope
@@ -172,14 +173,15 @@
     def find_ast_to(self, id: AST_ID):
         """Iterate through ASTs that lead to the AST with the given id (inclusive)"""
         if self.id == id:
             yield self
         else:
             for ast in self.children:
                 if ast.find_ast(id) is not None:
+                    yield self
                     yield from ast.find_ast_to(id)
                     break
 
     def find_ast(self, id: AST_ID) -> Optional[AST]:
         """Find the AST with the given id"""
         if len(self.id) > len(id):
             # the ast that we are looking for is not in the subtree of this ast
@@ -207,12 +209,14 @@
         return self.id + (len(self.children), 0)
 
     def next_var_scope(self) -> VarScope:
         """Get a scope for the next variable that will be have if it is assigned to this AST"""
         return VarScope(self.id, len(self.children))
 
     def _add_stmt(self, stmt: Statement):
+        if isinstance(stmt, NoStatement):
+            return self
         if self._is_frozen:
             raise Exception("The AST is frozen and cannot be modified")
         ast = AST(self.next_child_id(), self.prog, stmt)
         self.children.append(ast)
         return ast
```

### Comparing `codegen_2-2.1.1/codegen/models/expr.py` & `codegen_2-2.1.2/codegen/models/expr.py`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.1/codegen/models/program.py` & `codegen_2-2.1.2/codegen/models/program.py`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.1/codegen/models/statement.py` & `codegen_2-2.1.2/codegen/models/statement.py`

 * *Files identical despite different names*

### Comparing `codegen_2-2.1.1/codegen/models/var.py` & `codegen_2-2.1.2/codegen/models/var.py`

 * *Files identical despite different names*

