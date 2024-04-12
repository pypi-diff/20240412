# Comparing `tmp/caustic.lexer-0.1.0.tar.gz` & `tmp/caustic_lexer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.lexer-0.1.0.tar", last modified: Fri Apr 12 07:45:54 2024, max compression
+gzip compressed data, was "caustic_lexer-0.2.tar", last modified: Fri Apr 12 16:55:52 2024, max compression
```

## Comparing `caustic.lexer-0.1.0.tar` & `caustic_lexer-0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 07:45:54.492154 caustic.lexer-0.1.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-0.1.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     6026 2024-04-12 07:45:54.492154 caustic.lexer-0.1.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     5094 2024-04-12 00:45:38.000000 caustic.lexer-0.1.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      998 2024-04-12 01:29:08.000000 caustic.lexer-0.1.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 07:45:54.492154 caustic.lexer-0.1.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 07:45:54.482154 caustic.lexer-0.1.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 07:45:54.482154 caustic.lexer-0.1.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 07:45:54.488821 caustic.lexer-0.1.0/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)      382 2024-04-12 05:50:13.000000 caustic.lexer-0.1.0/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-0.1.0/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     7333 2024-04-12 01:47:08.000000 caustic.lexer-0.1.0/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)    13527 2024-04-12 07:32:22.000000 caustic.lexer-0.1.0/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)    10440 2024-04-12 07:45:51.000000 caustic.lexer-0.1.0/src/caustic/lexer/precompiled.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 07:45:54.488821 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     6026 2024-04-12 07:45:54.000000 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      392 2024-04-12 07:45:54.000000 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 07:45:54.000000 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 07:45:54.000000 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 07:45:54.000000 caustic.lexer-0.1.0/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.111069 caustic_lexer-0.2/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic_lexer-0.2/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     6301 2024-04-12 16:55:52.111069 caustic_lexer-0.2/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     5369 2024-04-12 16:38:47.000000 caustic_lexer-0.2/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      998 2024-04-12 15:57:16.000000 caustic_lexer-0.2/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 16:55:52.111069 caustic_lexer-0.2/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.104403 caustic_lexer-0.2/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.104403 caustic_lexer-0.2/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.107736 caustic_lexer-0.2/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)      446 2024-04-12 16:38:09.000000 caustic_lexer-0.2/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic_lexer-0.2/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     7195 2024-04-12 16:37:41.000000 caustic_lexer-0.2/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)    13053 2024-04-12 16:27:38.000000 caustic_lexer-0.2/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     9939 2024-04-12 16:55:48.000000 caustic_lexer-0.2/src/caustic/lexer/precompiled.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic_lexer-0.2/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      267 2024-04-12 16:38:58.000000 caustic_lexer-0.2/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.111069 caustic_lexer-0.2/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     6301 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      449 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic.lexer-0.1.0/LICENSE` & `caustic_lexer-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.lexer-0.1.0/PKG-INFO` & `caustic_lexer-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,18 @@
 
 The `compiler` module compiles grammars from Caustic grammar (`.cag`) files into nodes,
 and uses a grammer system built in Caustic grammar format and compiled with the `basic_compiler` module
 
 The `nodes` module provides the nodes themselves, and allows manually building grammar by
 supplying nodes
 
+The `serialize` module provides functions for serializing and deserializing nodes
+
+The `util` module provides small utilities
+
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
 ### Include / Import
@@ -168,7 +172,14 @@
 
 Denoted by an `@`, followed by a node name (as a string of alphanumeric characters and underscore)
 
 Matches the value of the targeted node, and returns the result of that
 
 Must be bound using either its `.bind()` method, or automatically through the
 default compilers
+
+
+# Changelog
+
+## 0.2.0
+- Implemented node saving and loading through the `serialize` module
+- Moved `compiler.bind_nodes()` to `util.bind_nodes()`
```

### Comparing `caustic.lexer-0.1.0/README.md` & `caustic_lexer-0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 The `compiler` module compiles grammars from Caustic grammar (`.cag`) files into nodes,
 and uses a grammer system built in Caustic grammar format and compiled with the `basic_compiler` module
 
 The `nodes` module provides the nodes themselves, and allows manually building grammar by
 supplying nodes
 
+The `serialize` module provides functions for serializing and deserializing nodes
+
+The `util` module provides small utilities
+
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
 ### Include / Import
@@ -144,7 +148,14 @@
 
 Denoted by an `@`, followed by a node name (as a string of alphanumeric characters and underscore)
 
 Matches the value of the targeted node, and returns the result of that
 
 Must be bound using either its `.bind()` method, or automatically through the
 default compilers
+
+
+# Changelog
+
+## 0.2.0
+- Implemented node saving and loading through the `serialize` module
+- Moved `compiler.bind_nodes()` to `util.bind_nodes()`
```

### Comparing `caustic.lexer-0.1.0/pyproject.toml` & `caustic_lexer-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
```

### Comparing `caustic.lexer-0.1.0/src/caustic/lexer/basic_compiler.py` & `caustic_lexer-0.2/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-0.1.0/src/caustic/lexer/compiler.py` & `caustic_lexer-0.2/src/caustic/lexer/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,14 @@
         cnodes = {name: compile_node(b'group', expr) for name,expr in data.items()}
     except Exception as e:
         e.add_note(f'Whilst compiling grammar from: {"<dict>" if source is None else source}')
         raise e
     bind_nodes(cnodes)
     return cnodes
 
-def bind_nodes(nodes: dict[bytes, nodes.Node]) -> None:
-    '''Cross-binds all nodes'''
-    for node in nodes.values(): node.bind(nodes)
-
 def compile_node_name(name: bytes | str | None, expr: dict) -> nodes.Node:
     '''Compiles a node and names it'''
     node = compile_node(**expr)
     node.name = None if name is None else name if isinstance(name, str) else name.decode()
     return node
     
 def compile_node(type: typing.Literal[b'group', b'group_ws_sensitive', b'union', b'range', b'range_ws_sensitive',
```

### Comparing `caustic.lexer-0.1.0/src/caustic/lexer/nodes.py` & `caustic_lexer-0.2/src/caustic/lexer/nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,33 +54,28 @@
     def __init__(self, *, name: str | None = None):
         self.name = name
 
     def bind(self, nodes: dict[bytes, typing.Self]) -> None:
         '''Binds all sub-nodes, if possible'''
         if not hasattr(self, 'nodes'): return
         for node in self.nodes: node.bind(nodes)
+    def unbind(self) -> None:
+        '''Unbinds all sub-nodes'''
+        if not hasattr(self, 'nodes'): return
+        for node in self.nodes: node.unbind()
 
     @abstractmethod
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> object | dict[str, typing.Any]:
         '''Executes this node on `data`'''
 
     @abstractmethod
     def __str__(self) -> str: pass
     @abstractmethod
     def __repr__(self) -> str: pass
 
-    @classmethod
-    def from_kwargs(cls, kwargs: dict) -> typing.Self:
-        '''Constructs the class from `kwargs` (for pickling)'''
-        return cls(**kwargs)
-    def __reduce__(self) -> tuple[cabc.Callable, tuple[dict]]:
-        return (self.from_kwargs, (
-            {n: getattr(self, n) for n in sum((c.__slots__ for c in type(self).mro()
-                                               if hasattr(c, '__slots__')), start=())},))
-
 ## Groups
 class NodeGroup(Node):
     '''
         A group of nodes
         Discards whitespace between nodes if `keep_whitespace` is false
     '''
     __slots__ = ('nodes', 'keep_whitespace')
@@ -143,18 +138,14 @@
         return results
 
     def __str__(self) -> str:
         return f'{"" if self.name is None else f"{self.name}:"}{"({"[self.keep_whitespace]} {" ".join(map(str, self.nodes))} {")}"[self.keep_whitespace]}'
     def __repr__(self) -> str:
         return f'<{type(self).__qualname__} {self.name!r}{" [keep_whitespace]" if self.keep_whitespace else ""} {self.nodes!r}>'
 
-    @classmethod
-    def from_kwargs(cls, kwargs: dict) -> typing.Self:
-        return cls(*kwargs['nodes'], name=kwargs['name'])
-
 class NodeUnion(Node):
     '''Matches any of its nodes'''
     __slots__ = ('nodes',)
 
     nodes: tuple[Node, ...]
 
     def __init__(self, *nodes: Node, **kwargs):
@@ -329,24 +320,24 @@
             If `.target_name` is not found in the dict, `False` is returned,
                 otherwise `.target` is set to that node and `True` is returned
             Note: if this node was previously bound, that binding is removed,
                 even if rebinding fails
         '''
         self.target = targets.get(self.target_name)
         return self.target is not None
+    def unbind(self) -> None:
+        '''Unbinds this node'''
+        self.target = None
 
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> typing.Any:
         if not self.bound:
             raise TypeError(f'Cannot call an unbound NodeRef (node target {self.target_name} was never bound)')
         try: return self.target(bm, stealer)
         except NodeSyntaxError as nse:
             nse.add_note(f'Under reference {self}')
             raise nse
 
     def __str__(self) -> str:
         return f'@{self.target_name!r}'
     def __repr__(self) -> str:
         return (f'<{type(self).__qualname__} {self.name!r} target:{self.target_name!r} '
                 f'{"[unbound]" if self.target is None else repr(self.target)}>')
-
-    def __reduce__(self) -> tuple[cabc.Callable, tuple[dict]]:
-        return (self.from_kwargs, ({'name': self.name, 'target': self.target_name},))
```

### Comparing `caustic.lexer-0.1.0/src/caustic/lexer/precompiled.py` & `caustic_lexer-0.2/src/caustic/lexer/precompiled.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,51 +22,51 @@
 __all__ = ('builtin_path', 'DEFAULT_GRAMMAR',
            'compile_path', 'compile_file', 'compile_bytes', 'compile_buffermatcher', 'compile_dict',
            'compile_node_name', 'compile_node')
 
 builtin_path = Path(__file__).parent/'grammar.cag'
 
 # LOAD PRECOMPILED GRAMMAR
-DEFAULT_GRAMMAR = __import__('pickle').loads(
-    __import__('lzma').decompress(
-        b'\xfd7zXZ\x00\x00\x04\xe6\xd6\xb4F\x02\x00!\x01\x16\x00\x00\x00t/\xe5\xa3\xe0\r\xd9\x03\x91]'
-        b'\x00@\x01\x0ez\xe4,\xe2\xe9\x84\x0f\xcc\xd5\xcd\xd8\x13\x9d\x00=\x12\xea\x8d\x1b~\xfd\xc1\\]3\x10'
-        b'\x12\xd5\xc9"\xdfeE\xf1Q\x9d-$_T\xf2Q\xb6b\xe7^\xf8\x8f\xd6\x03,N\xa2+\x03"'
-        b'\xec\xc2q6%\xa4\x84\xad\x17\xbb\x0fv\xeb\xe9c\xc5\xc8,\x8d\x1c[\xc7\xc8\xe2tc\xf7\xd9\xe5W'
-        b'\x80\x07\x12\xd8s\xa2\x92\xcc\xfb\xab\xdfd#\x8c\xe6\xcbq\xccU(\xf0\xa7\x96\xda\x16R\xbc\xb5\xdf\x1c'
-        b'{cj\xd2\xcf\xa6Y\x915/\x18\x92\xc3\x87b\x97\xd6\xf3n\xa3q\x10a\xe4* \x02\x85"\xaa'
-        b'1\xb5\x85I\\Y2\n\x1a\x81\x11\x1f\xb4\x9a?\x05\xeeA\xe8_\x10\x06\xbf\xb8\xe5\xce\xb0\xcf\x06\xbb'
-        b'i\xae\xf0\x86\xfdPL!/\x83\x01Dp\x13\xe2\xd2)@\xc6\x96\x08}B0h\xaa\xe7\x15&5'
-        b'\xa5Mr8\xd91j\x83\xfb\xe1\x1e\xb5\xbd\xd1A\x9d\x16N\x9a\x9fu\xebw\xa5\xb8,\xac>\xbe\xac'
-        b'\xc5\x8a\xbd*\xc96[9\xb8\xfe\x86]\xfaP\x1b\x1b\x83`\xdcy\x7f\xd7\xffC\x88s\xfa\x9c>l'
-        b'\xa1dtw\xbb\x97\xbe*\x9aI\xd5r\xed\xeb\xfb\x89X\xb9\x89k%\x0b\xe9^\x03\xd0A\xd0A\xa5'
-        b"\x9a\x82\x97\x15*'\x01k\x8e\xc4\xb2\x0b\xd5\xedF\r\xe1\xac\x91\x10\xa08<\xe9\x1fC\xf9\xa8-\xab"
-        b'\x1f\x17\xd3\xe1\x99\r\xf8iz\xffa\xa9FQ"}b]?<D\xd5\xdf}\x9c\xe6\xfe\x1aTH'
-        b"\xb0u\x12\x81\xff\xc5m\xbc\xdf(i]\x89\x81\xbf\x13\xbf '\xe4\x94\x8dm\x9c\xcb)i\xbfc\x89"
-        b'?\x1b\xda\xe4\x9aM\xb0Gn0o\xc2\xa7\x9975\xd4d\x12\x86\xe4\xa8"O_\x81(\xb3q\x87'
-        b'\xeeF\xe8\xe9\xaf\xcf\xb3\xa4\xc8\xb9\xc8u96\x8c\xd7{\xa0\x1e+\xbbo\xb1\xb2*\xb3\x14\x0b\xdc\xab'
-        b'\xee\xf8_\xea\t\x97\x04\x1b\x9d\x029&\xa5y\x17\xc2\xd2\x10\xcf\xc2\xcdU_\xf5(Q\x11\xc3\xb9\xac'
-        b'\x07%\xcc\x9ca}w\x94&\x9d\x07q\x8fb!v\xb61\xbe$E\x0b\x90\x1f,H\xfc\xc1\x9e\xe5'
-        b"B|mP\xd4h8p\xb2\xfd\xaf\x1e\xc2`E\x00\xd4\xb6\x9eUc\x9dA'\xb8\xda\xe1l\xf5\x03"
-        b"\xe1\xd98\xd3'\xc0b\xcc\xd4`\xbbns\xd1\xf5'\xcf\x94\x10zk9\xb0\xfe~LOy\xfd`"
-        b'\xc7\xdc9k\x86\xe2\xbe\x00\xb3\x17Y=c\xf4\\\xdf\xa4\xbd\xe4\xf6\xed\x8c\x01\xda\xa1;\x99(\xde\xcc'
-        b'\xf4\xfd8B\xd4\xb46\x92\xce\xea\xf2ST\xc36\x8ep>\x97\x14\xfa\xd3\xbf=;\xba\x1a\xd9\xa0\x01'
-        b'\xd8\x04\xe4\x84ab+\x05\xda\x8a&\x11\xf8\x89\xa7:\n\xbc\x13\x89\xfd_(w\x05_t\x9c\xfbm'
-        b'n\xe5\xf0\xe0B\xfb\xe4\xda\x90\xb4TB\x15M\xb9%\tX\x81p)\xc6\xeeV\x1a.\xa0I\xa3\x80'
-        b'\xda\x07\xfa\x0b.\x89\x8bk\xb6\x06G}b?\xe4\x8bu\xf8\xda\xc5yv\x1f"\xaa\t\x05\x86\x8f '
-        b'$\xde\xedY\xf806n\xbd\x99\xaf\x06_\xdb\xb5\x97\xb4\x9e\xcf~\x84\x7f\x99:\xf6\xdd\xc5\xe2\xa4\xc1'
-        b'\xfeO\xea\xbf\xba\x9a\xe3"\x91M\xcdK\xd4}\xdf\xa1\xc3\x88\xb0\xec\x88\r\xb6I\xdblyZ\xe4\x06'
-        b'\xdbN\xc0["\x14c\xb0\x1cc\xb2\xc6(jo\xc9\xae\x9f^[\xc4\x12\xab\xb7\xdf\x9d0\xe4$\xa7'
-        b'n\xf3r\x87X\xa3\xf7\x88\x9b\xe03\xa5Q\xa5\xf8,`\xbe#G&l\xc2\xf8`\x94E\xd5\xf6V'
-        b'\xf6tG.\x14\xcc\xd3\xa3\x89\xec\x1b\xfb\xf6s\x0eo\x069\x0b\t\x81\x80(\x18.~\xf6\xf6\x97D'
-        b']\xcf\xb6\xb86\x03\xac\x94\x80\xdb\xc6\xff\x92\xbb\\F-\x16\x1a(\xab\xceJ{\r\xb7\xc7B,\xdb'
-        b'\xcfZ\xc0<J\x87\x89#R4\xf5.x\x00\x00\x00\x00\x00\xba\x8b\xc3\xc1\x81\xa1\xb1v\x00\x01\xad\x07'
-        b'\xda\x1b\x00\x00\x91\x1fm\x8d\xb1\xc4g\xfb\x02\x00\x00\x00\x00\x04YZ'
-    )
-)
+from .serialize import deserialize as __deserialize
+DEFAULT_GRAMMAR = _deserialize(__import__('lzma').decompress(
+    b'\xfd7zXZ\x00\x00\x04\xe6\xd6\xb4F\x02\x00!\x01\x16\x00\x00\x00t/\xe5\xa3\xe0\x0c\xa4\x03<]'
+    b'\x00@\x01\x0ew{q\xcb `\xff\xc2\xb3\xc6Y\x9f\xa5\xc7uf\xfb\xd3\x89>\xb9!\x7flF\xad'
+    b'+\xaf\x8b\xbc\xe8\xe8\xff1J\x11m"\x9bu*\x9f\xaawX?\xeeFs\x00\x13\xca3\xa6\xb0\xcb'
+    b'rt\xd2\xd0P\xc2~>\xac\xefy>@\xf3\xe1\xed\x82y\x06\xca\x06\x0e\x06\x95N\xf7\xca\xb2?\xe1'
+    b'\xff\x87\xa1\xd7szC\x1c\xfe\x841j\x05\xea9\x05<\xc3\x0b\xf1\x95X\xff\xcf\x1fgAb\t\x85'
+    b' [\x16\xd6\xa0\xfe7N\xd9\xe5\xf1Cu\xff\xa9\x91\xba\xf3\x12\xf8\xd4s\xc9w\x9f\x85t\x9ehj'
+    b'\n.\x02\x9cX\x07\x08\xcfV2\x95\xa9\xa9\x89\x8eEfy }\xc1\x86\x88\xe1B[\xc1\xf9\x87\xdd'
+    b"'a\x92\xa3[l\xd72\x18p\xec@J\xddG\\@y\xa1\xed\x17\xd5\xb0H5ni[mn"
+    b'\xb2n\xf2<\xce\xf0]_`\x00\x04\x95\x8fW\x14\x13\x84\xb3\x00\xc9\xbf_\x99r\x91\xf5^\x0e\xf3\xf4'
+    b'7]\xc6\xab\x9d4,\x13\x1b\x14\xae\xfc\x90\x10\xa93V\xa8\xc5\t\xba1\x1e$Q\xba\xf2\x9d\x9e\x15'
+    b'\x8e&\xa3\xfd"&4\xca1%\xdf\xd7\nA\xfa(\xce\x07\xd9v\xe7\x18T\xa1#\x0b><_\xe7'
+    b"\x87\x01\xa7\x92-\\\x8b\x15\xfb%50\x18\x8e;5p'C_\xc2LF~\xb2{\xef/\xb5\xe8"
+    b'\x0c8\xaa~T$J\xda\x0f\x86\x15\x13\xfc\x82\xb6\xfa\xa19\x07\x83Fe\x92\x96\xc4\x11\x15J\xfb\xa1'
+    b'\xd4\xee\xdd\x13`f\xa2\xc4.\xb9S\xbc\xae\xffOf\xd6\x13mmB$\x1aJ\x85~ \xfc\x89\xe8'
+    b'\xfc<\x04\x1a\xc6\xf92\xfa>\xb0\xc6\x82\xcd_:\xe3"$n\xfe\xb3\xd3\xc1\xd49\x13\xf0\xdeup'
+    b'\xb2N+x\x97\x9dYY\x02\x08Pe\x14t\xe6\x9f\xd4\x8di\x94\x0c\x1f|aw\xbcE"\x02n'
+    b'\x02\xc6\xd1\xe9_\x9b\x11>[\x18\xff[mG\x1e\xb0\xf7\x95V\xf4\x87W\xe3\x14\xdf\x85\xb2\x02\x00\xb5'
+    b'%\xb9\x1dM?A\xc5.p\xe4@\xacv\xa8Y\x8f\x9a)\x9b\x10u\xaf\xa7\xa5\xc5\xa9\xc9\xda\xd5-'
+    b'/u\xd3$\xe0\x81!^\xe3g\xcf\xaf\xdfgp"A\xb1\x1f\xcc\xb6`>x\xfe\xc0\x0c9\x1f?'
+    b'\x80\xee\x1c\x10\x14\xa1\xbe\xc69\x05\xd1p(\xdc\x8eW\xe1\xc4\x01\x812\x93\x89k\x92p\x87I=\xfc'
+    b'\x1f\x15\xbc\xf1\x00@\xa7zH\t\x11P#\x0c\xe6\xc9\xdfv\xfa\xeaE\xadQ\xcc/\xf6 V\xa8\xcf'
+    b"\x86\xa7w\xb3\x95\xc3#\xd9\x1f\xa7\x87F\xa4\xc6rS\x83\xbe\xae&\xb9\xad\x9bL\x02\xdc\x81\xd1\xe4'"
+    b'\xecB\xe6b\xccu\xf8\xca*R/\x07\xce*~J\xcf\xa2Xo\xd3\x07\xe8\x99\x8c\x17\xe0\x05\x17\xb1'
+    b'\x9a\xbbES\xb9N#\x07\xf3\x1dS\xb75*\xc5X\x85Q\xbe\x99\x92B\x82\xc5\x1cn\xc7\xd6/#'
+    b'\xe20t\xab\x10k\x1c\xfe\xce\xf7:\x93\xd4\xb6\xbe\xde\xc1\xbd~\xf5\x81w\x97bF\x08\xb8w\xe3\x17'
+    b'\xb3\xf5-?\ro\xa56\xb37{\xe8\x7f@\x0f\x10\xc4?\x05>\xd7"\x84\xac\xb7\xc3\xe3w\x91\x1e'
+    b'!\xb1\xf8\x80=]\xa5\x939$\xc1\x8f\xdeY\xb4\x8aS5\xc3%+\xb3\xcb\xf1\x12\x84\t\x16\xdc\xbb'
+    b'%\x1e\x06\xac\x98\xa2V\x11\x11\xed\xa2\xc8\x1aC\xb3\x8cE\rX\xd0\x13\xe6\x10pM\xab\x87\xb1\xe9\xd7'
+    b'@\xf9UK\x85\x1a\xebC\x15\x8a\xdc\xf3\xb6\x07S\\\x08\xe0\xb0\x00\xd1"&\xee\x15F%\xb6\x00\x01'
+    b'\xd8\x06\xa5\x19\x00\x00\xf7\xce:\xdb\xb1\xc4g\xfb\x02\x00\x00\x00\x00\x04YZ'
+))
+del __deserialize
+from .util import bind_nodes as __bind_nodes
+__bind_nodes(DEFAULT_GRAMMAR)
+del __bind_nodes
 
 @singledispatch
 def compile(src: Path | typing.BinaryIO | bytes | buffer_matcher.SimpleBufferMatcher | dict, *,
             source: Path | str | None = None, grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
     '''Compiles a `Path`, file, `bytes`, or buffer-matcher into a grammar'''
     raise TypeError(f'Cannot compile type of {bad}, must be a Path, file, bytes, or buffer-matcher')
 
@@ -137,18 +137,14 @@
         cnodes = {name: compile_node(b'group', expr) for name,expr in data.items()}
     except Exception as e:
         e.add_note(f'Whilst compiling grammar from: {"<dict>" if source is None else source}')
         raise e
     bind_nodes(cnodes)
     return cnodes
 
-def bind_nodes(nodes: dict[bytes, nodes.Node]) -> None:
-    '''Cross-binds all nodes'''
-    for node in nodes.values(): node.bind(nodes)
-
 def compile_node_name(name: bytes | str | None, expr: dict) -> nodes.Node:
     '''Compiles a node and names it'''
     node = compile_node(**expr)
     node.name = None if name is None else name if isinstance(name, str) else name.decode()
     return node
     
 def compile_node(type: typing.Literal[b'group', b'group_ws_sensitive', b'union', b'range', b'range_ws_sensitive',
@@ -179,11 +175,7 @@
             if ctx is None:
                 ctx = codecs.escape_decode(val['str'])[0]
             return nodes.Context(ctx)
         case b'noderef':
             return nodes.NodeRef(val)
         case _:
             raise TypeError(f'Unknown node type {type!r}')
-
-
-# BIND PRECOMPILED DEFAULT_GRAMMAR
-bind_nodes(DEFAULT_GRAMMAR)
```

### Comparing `caustic.lexer-0.1.0/src/caustic.lexer.egg-info/PKG-INFO` & `caustic_lexer-0.2/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -29,14 +29,18 @@
 
 The `compiler` module compiles grammars from Caustic grammar (`.cag`) files into nodes,
 and uses a grammer system built in Caustic grammar format and compiled with the `basic_compiler` module
 
 The `nodes` module provides the nodes themselves, and allows manually building grammar by
 supplying nodes
 
+The `serialize` module provides functions for serializing and deserializing nodes
+
+The `util` module provides small utilities
+
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
 ### Include / Import
@@ -168,7 +172,14 @@
 
 Denoted by an `@`, followed by a node name (as a string of alphanumeric characters and underscore)
 
 Matches the value of the targeted node, and returns the result of that
 
 Must be bound using either its `.bind()` method, or automatically through the
 default compilers
+
+
+# Changelog
+
+## 0.2.0
+- Implemented node saving and loading through the `serialize` module
+- Moved `compiler.bind_nodes()` to `util.bind_nodes()`
```

