# Comparing `tmp/pysel-lang-0.0.4.tar.gz` & `tmp/pysel-lang-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysel-lang-0.0.4.tar", last modified: Fri Apr  5 20:06:44 2024, max compression
+gzip compressed data, was "pysel-lang-0.0.5.tar", last modified: Fri Apr 12 15:27:28 2024, max compression
```

## Comparing `pysel-lang-0.0.4.tar` & `pysel-lang-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-05 20:06:44.943045 pysel-lang-0.0.4/
--rw-r--r--   0 othompson   (501) staff       (20)     1062 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/LICENSE
--rw-r--r--   0 othompson   (501) staff       (20)      117 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/MANIFEST.in
--rw-r--r--   0 othompson   (501) staff       (20)    10377 2024-04-05 20:06:44.942725 pysel-lang-0.0.4/PKG-INFO
--rw-r--r--   0 othompson   (501) staff       (20)     9216 2024-04-05 20:03:47.000000 pysel-lang-0.0.4/README.md
--rw-r--r--   0 othompson   (501) staff       (20)      180 2024-04-02 22:21:32.000000 pysel-lang-0.0.4/pyproject.toml
-drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-05 20:06:44.939483 pysel-lang-0.0.4/pysel/
--rw-r--r--   0 othompson   (501) staff       (20)     2828 2024-04-05 20:06:27.000000 pysel-lang-0.0.4/pysel/__init__.py
--rw-r--r--   0 othompson   (501) staff       (20)    16802 2024-04-05 20:06:02.000000 pysel-lang-0.0.4/pysel/ast.py
--rw-r--r--   0 othompson   (501) staff       (20)     1695 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/pysel/errors.py
--rw-r--r--   0 othompson   (501) staff       (20)     4822 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/pysel/lexer.py
--rw-r--r--   0 othompson   (501) staff       (20)        0 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/pysel/py.typed
--rw-r--r--   0 othompson   (501) staff       (20)     4014 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/pysel/tokens.py
-drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-05 20:06:44.942406 pysel-lang-0.0.4/pysel_lang.egg-info/
--rw-r--r--   0 othompson   (501) staff       (20)    10377 2024-04-05 20:06:44.000000 pysel-lang-0.0.4/pysel_lang.egg-info/PKG-INFO
--rw-r--r--   0 othompson   (501) staff       (20)      392 2024-04-05 20:06:44.000000 pysel-lang-0.0.4/pysel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 othompson   (501) staff       (20)        1 2024-04-05 20:06:44.000000 pysel-lang-0.0.4/pysel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 othompson   (501) staff       (20)        6 2024-04-05 20:06:44.000000 pysel-lang-0.0.4/pysel_lang.egg-info/top_level.txt
--rw-r--r--   0 othompson   (501) staff       (20)       38 2024-04-05 20:06:44.943088 pysel-lang-0.0.4/setup.cfg
--rw-r--r--   0 othompson   (501) staff       (20)     3328 2024-04-02 22:25:16.000000 pysel-lang-0.0.4/setup.py
-drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-05 20:06:44.942085 pysel-lang-0.0.4/tests/
--rw-r--r--   0 othompson   (501) staff       (20)      318 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/tests/test_accessor.py
--rw-r--r--   0 othompson   (501) staff       (20)      139 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/tests/test_environment_substitution.py
--rw-r--r--   0 othompson   (501) staff       (20)     1190 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/tests/test_getitem.py
--rw-r--r--   0 othompson   (501) staff       (20)      671 2024-04-02 22:18:41.000000 pysel-lang-0.0.4/tests/test_method_call.py
+drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-12 15:27:28.170381 pysel-lang-0.0.5/
+-rw-r--r--   0 othompson   (501) staff       (20)     1062 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/LICENSE
+-rw-r--r--   0 othompson   (501) staff       (20)      117 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/MANIFEST.in
+-rw-r--r--   0 othompson   (501) staff       (20)    10377 2024-04-12 15:27:28.170014 pysel-lang-0.0.5/PKG-INFO
+-rw-r--r--   0 othompson   (501) staff       (20)     9216 2024-04-05 20:03:47.000000 pysel-lang-0.0.5/README.md
+-rw-r--r--   0 othompson   (501) staff       (20)      180 2024-04-02 22:21:32.000000 pysel-lang-0.0.5/pyproject.toml
+drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-12 15:27:28.166992 pysel-lang-0.0.5/pysel/
+-rw-r--r--   0 othompson   (501) staff       (20)     2920 2024-04-12 15:26:52.000000 pysel-lang-0.0.5/pysel/__init__.py
+-rw-r--r--   0 othompson   (501) staff       (20)    19193 2024-04-12 15:22:58.000000 pysel-lang-0.0.5/pysel/ast.py
+-rw-r--r--   0 othompson   (501) staff       (20)     1695 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/pysel/errors.py
+-rw-r--r--   0 othompson   (501) staff       (20)     4822 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/pysel/lexer.py
+-rw-r--r--   0 othompson   (501) staff       (20)        0 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/pysel/py.typed
+-rw-r--r--   0 othompson   (501) staff       (20)     4014 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/pysel/tokens.py
+-rw-r--r--   0 othompson   (501) staff       (20)     6438 2024-04-12 15:26:52.000000 pysel-lang-0.0.5/pysel/vm.py
+drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-12 15:27:28.169802 pysel-lang-0.0.5/pysel_lang.egg-info/
+-rw-r--r--   0 othompson   (501) staff       (20)    10377 2024-04-12 15:27:28.000000 pysel-lang-0.0.5/pysel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 othompson   (501) staff       (20)      404 2024-04-12 15:27:28.000000 pysel-lang-0.0.5/pysel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 othompson   (501) staff       (20)        1 2024-04-12 15:27:28.000000 pysel-lang-0.0.5/pysel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 othompson   (501) staff       (20)        6 2024-04-12 15:27:28.000000 pysel-lang-0.0.5/pysel_lang.egg-info/top_level.txt
+-rw-r--r--   0 othompson   (501) staff       (20)       38 2024-04-12 15:27:28.170423 pysel-lang-0.0.5/setup.cfg
+-rw-r--r--   0 othompson   (501) staff       (20)     3328 2024-04-02 22:25:16.000000 pysel-lang-0.0.5/setup.py
+drwxr-xr-x   0 othompson   (501) staff       (20)        0 2024-04-12 15:27:28.168533 pysel-lang-0.0.5/tests/
+-rw-r--r--   0 othompson   (501) staff       (20)      318 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/tests/test_accessor.py
+-rw-r--r--   0 othompson   (501) staff       (20)      139 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/tests/test_environment_substitution.py
+-rw-r--r--   0 othompson   (501) staff       (20)     1190 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/tests/test_getitem.py
+-rw-r--r--   0 othompson   (501) staff       (20)      671 2024-04-02 22:18:41.000000 pysel-lang-0.0.5/tests/test_method_call.py
```

### Comparing `pysel-lang-0.0.4/LICENSE` & `pysel-lang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/PKG-INFO` & `pysel-lang-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysel-lang
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple but powerful embedded expression language for Python
 Home-page: https://github.com/tandemdude/pysel
 Author: tandemdude
 Author-email: tandemdude1@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pysel-lang-0.0.4/README.md` & `pysel-lang-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/pysel/__init__.py` & `pysel-lang-0.0.5/pysel/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,58 +21,62 @@
 import types
 import typing as t
 
 from pysel import ast
 from pysel import errors
 from pysel import lexer
 from pysel import tokens
+from pysel import vm
 
 __all__ = ["ast", "lexer", "tokens", "Expression"]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 T = t.TypeVar("T")
 
 
 class Expression(t.Generic[T]):
-    __slots__ = ("raw", "ast", "py_code", "code_obj")
+    __slots__ = ("raw", "ast", "bytecode", "vm")
 
     def __init__(self, raw: str) -> None:
         self.raw: str = raw
 
         self.ast: t.Optional[ast.Node] = None
-        self.py_code: t.Optional[str] = None
-        self.code_obj: t.Optional[types.CodeType] = None
+        self.bytecode: t.Optional[t.List[vm.Instruction]] = None
+        self.vm: t.Optional[vm.VirtualMachine[T]] = None
 
-    def compile(self) -> types.CodeType:
-        if self.code_obj is not None:
-            return self.code_obj
+    def compile(self) -> vm.VirtualMachine:
+        if self.vm is not None:
+            return self.vm
 
         self.ast = ast.Parser(self.raw, lexer.Lexer(self.raw).tokenize()).compilation_unit()
-        self.py_code = self.ast.compile()
-        self.code_obj = compile(self.py_code, "pysel_expr", "single")
 
-        return self.code_obj
+        symbol_table = vm.SymbolTable()
+        self.bytecode = self.ast.compile(symbol_table)
+        self.vm = vm.VirtualMachine(self.bytecode, symbol_table)
+
+        return self.vm
 
     def evaluate(self, env: t.Optional[t.Dict[str, t.Any]] = None, use_ast: bool = False) -> T:
         """
         Evaluate this expression under the given environment.
 
         Args:
             env (dict | None): Environment to use to resolve references in the expression.
-            use_ast (bool): Whether to run as an AST walker instead of transpiling the AST to python and running
-                using ``eval`` instead.
+            use_ast (bool): Whether to run as an AST walker instead of compiling to PySEL bytecode and using
+                the bytecode virtual machine.
 
         Returns:
             The output of the expression.
         """
+        if self.ast is None:
+            self.compile()
 
         env = env or {}
         for primitive in (bool, float, int, str):
             env.setdefault(primitive.__name__, primitive)
         env.setdefault("None", None)
 
         if use_ast:
-            self.compile()
             return t.cast(T, self.ast.evaluate(env))
 
-        return t.cast(T, eval(self.compile(), env))
+        return t.cast(T, self.vm.run(env))
```

### Comparing `pysel-lang-0.0.4/pysel/ast.py` & `pysel-lang-0.0.5/pysel/ast.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 import abc
 import collections
 import operator as operator_
 import typing as t
 
 from pysel import errors
 from pysel import tokens as tokens_
+from pysel.vm import Instruction
+from pysel.vm import Opcode
+from pysel.vm import SymbolTable
 
 __all__ = [
     "Node",
     "Literal",
     "Reference",
     "UnaryOp",
     "BinaryOp",
@@ -38,40 +41,40 @@
     "Accessor",
     "MethodCall",
     "Parser",
 ]
 
 T = t.TypeVar("T")
 UNARY_OPERATOR_MAPPING = {
-    "!": operator_.not_,
-    "-": operator_.neg,
-    "+": operator_.pos,
+    "!": (operator_.not_, Opcode.NOT),
+    "-": (operator_.neg, Opcode.NEGATE),
+    "+": (operator_.pos, Opcode.POSITIVE),
 }
 BINARY_OPERATOR_MAPPING = {
-    "==": operator_.eq,
-    "!=": operator_.ne,
-    ">": operator_.gt,
-    "<": operator_.lt,
-    ">=": operator_.ge,
-    "<=": operator_.le,
-    "+": operator_.add,
-    "-": operator_.sub,
-    "*": operator_.mul,
-    "/": operator_.truediv,
-    "//": operator_.floordiv,
-    "%": operator_.mod,
-    "**": operator_.pow,
+    "==": (operator_.eq, Opcode.EQUALS),
+    "!=": (operator_.ne, Opcode.NOT_EQUALS),
+    ">": (operator_.gt, Opcode.GREATER_THAN),
+    "<": (operator_.lt, Opcode.LESS_THAN),
+    ">=": (operator_.ge, Opcode.GREATER_THAN_EQUALS),
+    "<=": (operator_.le, Opcode.LESS_THAN_EQUALS),
+    "+": (operator_.add, Opcode.ADD),
+    "-": (operator_.sub, Opcode.SUBTRACT),
+    "*": (operator_.mul, Opcode.MULTIPLY),
+    "/": (operator_.truediv, Opcode.TRUEDIV),
+    "//": (operator_.floordiv, Opcode.FLOORDIV),
+    "%": (operator_.mod, Opcode.MODULO),
+    "**": (operator_.pow, Opcode.POWER),
 }
 
 
 class Node(abc.ABC):
     __slots__ = ()
 
     @abc.abstractmethod
-    def compile(self) -> str:
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
         ...
 
     @abc.abstractmethod
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         ...
 
 
@@ -80,32 +83,32 @@
 
     def __init__(self, value: T) -> None:
         self.value: T = value
 
     def __repr__(self) -> str:
         return f"Literal({self.value!r})"
 
-    def compile(self) -> str:
-        return repr(self.value)
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        return [Instruction(Opcode.LOAD_CONST, st.add_literal(self.value))]
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> T:
         return self.value
 
 
 class Reference(Node):
     __slots__ = ("name",)
 
     def __init__(self, name: str) -> None:
         self.name = name
 
     def __repr__(self) -> str:
         return f"Reference({self.name!r})"
 
-    def compile(self) -> str:
-        return self.name
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        return [Instruction(Opcode.LOAD_REF, st.add_reference(self.name))]
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         return env[self.name]
 
 
 class UnaryOp(Node):
     __slots__ = ("operator", "operand")
@@ -113,62 +116,87 @@
     def __init__(self, operator: str, operand: Node) -> None:
         self.operator = operator
         self.operand = operand
 
     def __repr__(self) -> str:
         return f"UnaryOp({self.operator}, {self.operand})"
 
-    def compile(self) -> str:
-        return f"{self.operator}({self.operand.compile()})" if self.operator != "!" else f"not ({self.operand.compile()})"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        return [*self.operand.compile(st), Instruction(UNARY_OPERATOR_MAPPING[self.operator][1], None)]
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
-        return UNARY_OPERATOR_MAPPING[self.operator](self.operand.evaluate(env))  # type: ignore[operator]
+        return UNARY_OPERATOR_MAPPING[self.operator][0](self.operand.evaluate(env))  # type: ignore[operator]
 
 
 class BinaryOp(Node):
     __slots__ = ("lh", "operator", "rh")
 
     def __init__(self, lh: Node, operator: str, rh: Node) -> None:
         self.lh = lh
         self.operator = operator
         self.rh = rh
 
     def __repr__(self) -> str:
         return f"BinaryOp({self.lh}, {self.operator}, {self.rh})"
 
-    def compile(self) -> str:
-        # special case && , ||
-        if self.operator == "&&" or self.operator == "||":
-            return f"({self.lh.compile()}) {'and' if self.operator == '&&' else 'or'} ({self.rh.compile()})"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        lh_instruction = self.lh.compile(st)
+        rh_instruction = self.rh.compile(st)
+
+        # Special cases
+        if self.operator == "||" or self.operator == "&&":
+            return [
+                *lh_instruction,
+                Instruction(
+                    Opcode.JUMP_IF_TRUE if self.operator == "||" else Opcode.JUMP_IF_FALSE, len(rh_instruction) + 1
+                ),
+                Instruction(Opcode.POP, None),
+                *rh_instruction,
+            ]
 
-        return f"({self.lh.compile()}) {self.operator} ({self.rh.compile()})"
+        return [*rh_instruction, *lh_instruction, Instruction(BINARY_OPERATOR_MAPPING[self.operator][1], None)]
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         # We process 'or' and 'and' separately to allow operator short-circuiting
         if self.operator == "||":
             return self.lh.evaluate(env) or self.rh.evaluate(env)
         elif self.operator == "&&":
             return self.lh.evaluate(env) and self.rh.evaluate(env)
 
-        return BINARY_OPERATOR_MAPPING[self.operator](self.lh.evaluate(env), self.rh.evaluate(env))
+        return BINARY_OPERATOR_MAPPING[self.operator][0](self.lh.evaluate(env), self.rh.evaluate(env))
 
 
 class TernaryOp(Node):
     __slots__ = ("condition", "when_true", "when_false")
 
     def __init__(self, condition: Node, when_true: Node, when_false: Node) -> None:
         self.condition = condition
         self.when_true = when_true
         self.when_false = when_false
 
     def __repr__(self) -> str:
         return f"TernaryOp({self.condition} ? {self.when_true} : {self.when_false})"
 
-    def compile(self) -> str:
-        return f"({self.when_true.compile()}) if ({self.condition.compile()}) else ({self.when_false.compile()})"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        instructions = [*self.condition.compile(st)]
+
+        when_true_instructions = self.when_true.compile(st)
+        when_false_instruction = self.when_false.compile(st)
+
+        instructions.extend(
+            [
+                Instruction(Opcode.POP_JUMP_IF_FALSE, len(when_true_instructions) + 2),
+                Instruction(Opcode.POP, None),
+                *when_true_instructions,
+                Instruction(Opcode.JUMP, len(when_false_instruction)),
+                *when_false_instruction,
+            ]
+        )
+
+        return instructions
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         if self.condition.evaluate(env):
             return self.when_true.evaluate(env)
         return self.when_false.evaluate(env)
 
 
@@ -178,16 +206,20 @@
     def __init__(self, operand: Node, attr: str) -> None:
         self.operand = operand
         self.attr = attr
 
     def __repr__(self) -> str:
         return f"Accessor({self.operand}, {self.attr!r})"
 
-    def compile(self) -> str:
-        return f"({self.operand.compile()}).{self.attr}"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        return [
+            Instruction(Opcode.LOAD_CONST, st.add_literal(self.attr)),
+            *self.operand.compile(st),
+            Instruction(Opcode.GETATTR, None),
+        ]
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         return getattr(self.operand.evaluate(env), self.attr)
 
 
 class MethodCall(Node):
     __slots__ = ("operand", "arguments")
@@ -195,38 +227,61 @@
     def __init__(self, operand: Node, arguments: t.Sequence[Node]) -> None:
         self.operand = operand
         self.arguments = arguments
 
     def __repr__(self) -> str:
         return f"MethodCall({self.operand}, args={self.arguments})"
 
-    def compile(self) -> str:
-        return f"({self.operand.compile()})({','.join(a.compile() for a in self.arguments)})"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        instructions: t.List[Instruction] = []
+        for argument in self.arguments[::-1]:
+            instructions.extend(argument.compile(st))
+
+        instructions.extend(self.operand.compile(st))
+        instructions.append(Instruction(Opcode.CALL, len(self.arguments)))
+
+        return instructions
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         return self.operand.evaluate(env)(*(a.evaluate(env) for a in self.arguments))
 
 
 class Getitem(Node):
     __slots__ = ("operand", "params")
 
     def __init__(self, operand: Node, params: t.Sequence[t.Optional[Node]]) -> None:
         self.operand = operand
         self.params: t.List[t.Optional[Node]] = list(params)
 
+        if len(self.params) > 1:
+            self.params.extend([None] * (3 - len(self.params)))
+
     def __repr__(self) -> str:
         return f"Getitem({self.operand}, params={self.params})"
 
-    def compile(self) -> str:
-        params = ":".join("" if p is None else p.compile() for p in self.params)
-        return f"({self.operand.compile()})[{params}]"
+    def compile(self, st: SymbolTable) -> t.List[Instruction]:
+        none_const_id = st.add_literal(None)
+
+        instructions: t.List[Instruction] = []
+        if len(self.params) > 1:
+            for param in self.params[::-1]:
+                if param is None:
+                    instructions.append(Instruction(Opcode.LOAD_CONST, none_const_id))
+                else:
+                    instructions.extend(param.compile(st))
+        else:
+            instructions.extend(self.params[0].compile(st))
+
+        instructions.extend(self.operand.compile(st))
+        instructions.append(Instruction(Opcode.GETITEM, len(self.params)))
+
+        return instructions
 
     def evaluate(self, env: t.Mapping[str, t.Any]) -> t.Any:
         if len(self.params) > 1:
-            self.params.extend([None] * (3 - len(self.params)))
             return self.operand.evaluate(env)[slice(*(p.evaluate(env) if p else None for p in self.params))]
         assert len(self.params) == 1 and self.params[0] is not None
         return self.operand.evaluate(env)[self.params[0].evaluate(env)]
 
 
 class Parser:
     __slots__ = ("raw", "tokens", "idx", "error_stack")
```

### Comparing `pysel-lang-0.0.4/pysel/errors.py` & `pysel-lang-0.0.5/pysel/errors.py`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/pysel/lexer.py` & `pysel-lang-0.0.5/pysel/lexer.py`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/pysel/tokens.py` & `pysel-lang-0.0.5/pysel/tokens.py`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/pysel_lang.egg-info/PKG-INFO` & `pysel-lang-0.0.5/pysel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysel-lang
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple but powerful embedded expression language for Python
 Home-page: https://github.com/tandemdude/pysel
 Author: tandemdude
 Author-email: tandemdude1@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pysel-lang-0.0.4/setup.py` & `pysel-lang-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/tests/test_getitem.py` & `pysel-lang-0.0.5/tests/test_getitem.py`

 * *Files identical despite different names*

### Comparing `pysel-lang-0.0.4/tests/test_method_call.py` & `pysel-lang-0.0.5/tests/test_method_call.py`

 * *Files identical despite different names*

