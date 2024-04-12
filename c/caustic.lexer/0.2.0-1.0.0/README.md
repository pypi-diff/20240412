# Comparing `tmp/caustic_lexer-0.2.tar.gz` & `tmp/caustic_lexer-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic_lexer-0.2.tar", last modified: Fri Apr 12 16:55:52 2024, max compression
+gzip compressed data, was "caustic_lexer-1.tar", last modified: Fri Apr 12 20:00:23 2024, max compression
```

## Comparing `caustic_lexer-0.2.tar` & `caustic_lexer-1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.111069 caustic_lexer-0.2/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic_lexer-0.2/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     6301 2024-04-12 16:55:52.111069 caustic_lexer-0.2/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     5369 2024-04-12 16:38:47.000000 caustic_lexer-0.2/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      998 2024-04-12 15:57:16.000000 caustic_lexer-0.2/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 16:55:52.111069 caustic_lexer-0.2/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.104403 caustic_lexer-0.2/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.104403 caustic_lexer-0.2/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.107736 caustic_lexer-0.2/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)      446 2024-04-12 16:38:09.000000 caustic_lexer-0.2/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic_lexer-0.2/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     7195 2024-04-12 16:37:41.000000 caustic_lexer-0.2/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)    13053 2024-04-12 16:27:38.000000 caustic_lexer-0.2/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)     9939 2024-04-12 16:55:48.000000 caustic_lexer-0.2/src/caustic/lexer/precompiled.py
--rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic_lexer-0.2/src/caustic/lexer/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)      267 2024-04-12 16:38:58.000000 caustic_lexer-0.2/src/caustic/lexer/util.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 16:55:52.111069 caustic_lexer-0.2/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     6301 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      449 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 16:55:52.000000 caustic_lexer-0.2/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:00:23.824034 caustic_lexer-1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic_lexer-1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     6297 2024-04-12 20:00:23.820701 caustic_lexer-1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     5365 2024-04-12 19:59:11.000000 caustic_lexer-1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      998 2024-04-12 19:59:27.000000 caustic_lexer-1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 20:00:23.824034 caustic_lexer-1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:00:23.810701 caustic_lexer-1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:00:23.810701 caustic_lexer-1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:00:23.820701 caustic_lexer-1/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic_lexer-1/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic_lexer-1/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     5521 2024-04-12 19:58:35.000000 caustic_lexer-1/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)    12964 2024-04-12 17:20:19.000000 caustic_lexer-1/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic_lexer-1/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic_lexer-1/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:00:23.820701 caustic_lexer-1/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     6297 2024-04-12 20:00:23.000000 caustic_lexer-1/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      416 2024-04-12 20:00:23.000000 caustic_lexer-1/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 20:00:23.000000 caustic_lexer-1/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 20:00:23.000000 caustic_lexer-1/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 20:00:23.000000 caustic_lexer-1/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic_lexer-0.2/LICENSE` & `caustic_lexer-1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic_lexer-0.2/PKG-INFO` & `caustic_lexer-1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 0.2.0
+Version: 1.0.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,28 +39,25 @@
 
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
-### Include / Import
-> `$include [path]`, `$import [path]`
+### Include
+> `$include [path]`
 
 Allows putting multiple grammar files together
 
 Relative paths provided as `[path]` will be checked against the following
 directories, in order:
 - The path of the includer/importer (if possible)
 - The `builtin_path` of the `compiler` module (the location of `compiler.py`)
 - The current directory
 
-The difference between include and import is that included nodes will be bound
-with the rest of the nodes from the includer, whilst imported nodes will not
-
 ## Comments
 Comments may start with a `#`
 
 ## Statements
 A statement begins with an [identifier](#identifier), followed by an `=`,
 then an [expression](#expression), and finally a `;`
 
@@ -179,7 +176,13 @@
 
 
 # Changelog
 
 ## 0.2.0
 - Implemented node saving and loading through the `serialize` module
 - Moved `compiler.bind_nodes()` to `util.bind_nodes()`
+
+## 1.0.0
+- Completely reworked compiler caching
+- Removed `$import` pragma
+- Moved `WHITESPACE_PATT` to `.util`
+- Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
```

### Comparing `caustic_lexer-0.2/README.md` & `caustic_lexer-1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,25 @@
 
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
-### Include / Import
-> `$include [path]`, `$import [path]`
+### Include
+> `$include [path]`
 
 Allows putting multiple grammar files together
 
 Relative paths provided as `[path]` will be checked against the following
 directories, in order:
 - The path of the includer/importer (if possible)
 - The `builtin_path` of the `compiler` module (the location of `compiler.py`)
 - The current directory
 
-The difference between include and import is that included nodes will be bound
-with the rest of the nodes from the includer, whilst imported nodes will not
-
 ## Comments
 Comments may start with a `#`
 
 ## Statements
 A statement begins with an [identifier](#identifier), followed by an `=`,
 then an [expression](#expression), and finally a `;`
 
@@ -155,7 +152,13 @@
 
 
 # Changelog
 
 ## 0.2.0
 - Implemented node saving and loading through the `serialize` module
 - Moved `compiler.bind_nodes()` to `util.bind_nodes()`
+
+## 1.0.0
+- Completely reworked compiler caching
+- Removed `$import` pragma
+- Moved `WHITESPACE_PATT` to `.util`
+- Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
```

### Comparing `caustic_lexer-0.2/pyproject.toml` & `caustic_lexer-1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "0.2.0"
+version = "1.0.0"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
```

### Comparing `caustic_lexer-0.2/src/caustic/lexer/basic_compiler.py` & `caustic_lexer-1/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic_lexer-0.2/src/caustic/lexer/compiler.py` & `caustic_lexer-1/src/caustic/lexer/compiler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,127 @@
 #!/bin/python3
 
-'''
-    Uses `basic_compiler` and `./grammar.cag` to create a
-        more advanced/resilient grammar compiler
-'''
+'''Provides the `Compiler` class'''
 
 #> Imports
 import re
 import codecs
 import typing
-import warnings
 import buffer_matcher
 from pathlib import Path
-from functools import singledispatch
+from functools import singledispatchmethod
+from collections import abc as cabc
 
 from . import nodes
-from . import basic_compiler
+from . import util
 #</Imports
 
 #> Header >/
-__all__ = ('builtin_path', 'DEFAULT_GRAMMAR',
-           'compile_path', 'compile_file', 'compile_bytes', 'compile_buffermatcher', 'compile_dict',
-           'compile_node_name', 'compile_node')
-
-builtin_path = Path(__file__).parent/'grammar.cag'
-
-#DEFAULT_GRAMMAR_START
-if builtin_path.is_file():
-    DEFAULT_GRAMMAR = basic_compiler.compile(
-        buffer_matcher.DynamicBufferMatcher(builtin_path.read_bytes()))
-else:
-    warnings.warn(f'Builtin grammar file {builtin_path.as_posix()} does not exist')
-    DEFAULT_GRAMMAR = None
-#DEFAULT_GRAMMAR_END
-
-@singledispatch
-def compile(src: Path | typing.BinaryIO | bytes | buffer_matcher.SimpleBufferMatcher | dict, *,
-            source: Path | str | None = None, grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
-    '''Compiles a `Path`, file, `bytes`, or buffer-matcher into a grammar'''
-    raise TypeError(f'Cannot compile type of {bad}, must be a Path, file, bytes, or buffer-matcher')
-
-@compile.register
-def compile_path(path: Path, *, source: Path | str | None = None,
-                 grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
-    '''Reads a path and compiles its contents'''
-    return compile_bytes(path.read_bytes(), source=(path if source is None else source), grammar=grammar)
-@compile.register
-def compile_file(file: typing.BinaryIO, source: Path | str | None = None,
-                 grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
-    '''Reads a binary file and compiles its contents'''
-    if source is None:
-        source = Path(file.name)
-        if not source.is_file(): source = file.name
-    return compile_bytes(file.read(), source=source, grammar=grammar)
-
-@compile.register
-def compile_bytes(data: bytes, *, source: Path | str | None = '<bytes>',
-                  grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
-    '''Compiles bytes'''
-    if source is None: source = '<bytes>'
-    return compile_buffermatcher(buffer_matcher.DynamicBufferMatcher(data), source=source, grammar=grammar)
-@compile.register
-def compile_buffermatcher(bm: buffer_matcher.SimpleBufferMatcher, source: Path | str | None = '<buffermatcher>',
-                          grammar: dict[bytes, nodes.Node] | None = None) -> dict[bytes, nodes.Node]:
-    '''Compiles a buffermatcher'''
-    if grammar is None: grammar = DEFAULT_GRAMMAR
-    if grammar is None:
-        raise FileNotFoundError('The default grammar did not exist at module import and as such can not be used')
-    grammars = {}
-    imports = {}; includes = {}
-    try:
-        while (bm.peek(1)):
-            while bm.match(nodes.WHITESPACE_PATT) or (grammar[b'COMMENT'](bm) is not nodes.Node.NO_RETURN): pass
-            if not bm.peek(1): break
-            if (p := grammar[b'PRAGMA'](bm)) is not nodes.Node.NO_RETURN:
-                match p['type']:
-                    case b'import' | b'include':
-                        f = Path(p['args'].decode())
-                        if not f.is_absolute():
-                            if isinstance(source, Path) and (nf := (source.parent / f)).is_file(): f = nf
-                            elif (nf := (Path.cwd() / f)).is_file(): f = nf
-                            elif (nf := (builtin_path.parent / f)).is_file(): f = nf
-                            else: raise FileNotFoundError(f'Cannot parse include: {f}')
-                        try: (includes if p['type'] == b'include' else imports).update(compile(f))
-                        except Exception as e:
-                            e.add_note(f'In {p["type"].decode()}')
-                            raise e
-                    case _ as t:
-                        raise TypeError(f'Unknown pragma type {t!r}')
+__all__ = ('Compiler',)
+
+class Compiler:
+    '''Compiles grammars'''
+    __slots__ = ('grammar', 'base_path')
+
+    grammar: dict[bytes, nodes.Node]
+    base_path: Path
+
+    def __init__(self, grammar: dict[bytes, nodes.Node],
+                 base_path: Path = Path(__file__).parent):
+        self.grammar = grammar
+        self.base_path = base_path
+
+    # Compiling
+    @singledispatchmethod
+    def compile(self, src: Path | typing.BinaryIO | bytes | buffer_matcher.SimpleBufferMatcher | dict, *,
+                source: Path | str | None = None, bind: bool = True) -> dict[bytes, nodes.Node]:
+        '''Compiles grammars from various sources'''
+        raise TypeError(f'Cannot compile from type {type(src).__qualname__}')
+
+    ## Intermediate source types
+    @compile.register
+    def compile_path(self, path: Path, *, source: Path | str | None = None, **kwargs) -> dict[bytes, nodes.Node]:
+        '''
+            Compiles from a path
+            See `.compile()` or `.compile_buffermatcher()` for `kwargs`
+        '''
+        return self.compile_bytes(path.read_bytes(), source=path if source is None else source, **kwargs)
+    @compile.register
+    def compile_file(self, file: typing.BinaryIO, *, source: Path | str | None = None, **kwargs) -> dict[bytes, nodes.Node]:
+        '''
+            Compiles from a file
+            See `.compile()` or `.compile_buffermatcher()` for `kwargs`
+        '''
+        return self.compile_bytes(file.read(), source=file.name if source is None else source, **kwargs)
+    @compile.register
+    def compile_bytes(self, data: bytes, *, source: Path | str | None = None, **kwargs) -> dict[bytes, nodes.Node]:
+        '''
+            Compiles from bytes
+            See `.compile()` or `.compile_buffermatcher()` for `kwargs`
+        '''
+        return self.compile_buffermatcher(buffer_matcher.DynamicBufferMatcher(data),
+                                          source='<bytes>' if source is None else source, **kwargs)
+    @compile.register
+    def compile_buffermatcher(self, bm: buffer_matcher.SimpleBufferMatcher,
+                              source: Path | str | None = None, bind: bool = True,
+                              precompile_only: bool = False) -> dict[bytes, nodes.Node]:
+        '''Compiles a grammar (dict of names and nodes) from a buffer matcher'''
+        if source is None: source = '<buffermatcher>'
+        try: pre = self.pre_process(bm, source=source, bind=bind)
+        except Exception as e:
+            e.add_note(f'Whilst pre-processing grammar from: {source}')
+            raise e
+        if precompile_only: return pre
+        try: return self.post_process_compile(pre, bind=bind)
+        except Exception as e:
+            e.add_note(f'Whilst post-process compiling grammar from: {source}')
+            raise e
+
+    ## Pre-process
+    def pre_process(self, bm: buffer_matcher.SimpleBufferMatcher,
+                    source: Path | str | None = None) -> dict[bytes, dict]:
+        '''
+            Reads a buffer matcher and parses it into a format suitable for compilation
+            Also handles pragmas
+        '''
+        working = {}
+        while True:
+            # Discard junk characters and check for EOF
+            while bm.match(util.WHITESPACE_PATT) or self.grammar[b'COMMENT'](bm):
+                pass # ignore whitespace and comments
+            if not bm.peek(1): break # EOF
+            # Handle pragmas
+            if p := self.grammar[b'PRAGMA'](bm):
+                try: self.handle_pragma(p['type'], p['args'], working=working, bm=bm, source=source)
+                except Exception as e:
+                    e.add_note(f'In pragma at {bm.pos} ({bm.lno}:{bm.cno})')
+                    raise e
                 continue
-            stmt = grammar[b'STATEMENT'](bm)
-            if stmt is nodes.Node.NO_RETURN:
-                raise SyntaxError(f'Unexpected character: {c!r}')
-            grammars[stmt['name']] = stmt['expr']
-    except Exception as e:
-        e.add_note(f'Whilst parsing grammar from: {"<buffermatcher>" if source is None else source}')
-        e.add_note(f'At position {bm.pos} ({bm.lno+1}:{bm.cno})')
-        raise e
-    grammars = compile_dict(grammars, source=source, grammar=grammar) | includes
-    bind_nodes(grammars)
-    return grammars | imports
-@compile.register
-def compile_dict(data: dict, *, source: Path | str | None = '<dict>', grammar: dict[bytes, nodes.Node] = None) -> dict[bytes, nodes.Node]:
-    '''Compiles a dictionary of preprocessed tokens'''
-    try:
-        cnodes = {name: compile_node(b'group', expr) for name,expr in data.items()}
-    except Exception as e:
-        e.add_note(f'Whilst compiling grammar from: {"<dict>" if source is None else source}')
-        raise e
-    bind_nodes(cnodes)
-    return cnodes
-
-def compile_node_name(name: bytes | str | None, expr: dict) -> nodes.Node:
-    '''Compiles a node and names it'''
-    node = compile_node(**expr)
-    node.name = None if name is None else name if isinstance(name, str) else name.decode()
-    return node
-    
-def compile_node(type: typing.Literal[b'group', b'group_ws_sensitive', b'union', b'range', b'range_ws_sensitive',
-                                      b'string', b'pattern', 'stealer', b'context', b'noderef'], val: typing.Any | None = None) -> nodes.Node:
-    '''Compiles a single node (or recursive nodes) given its type and a value'''
-    match type:
-        case b'group':
-            return nodes.NodeGroup(*(compile_node_name(**n) for n in val))
-        case b'group_ws_sensitive':
-            return nodes.NodeGroup(*(compile_node_name(**n) for n in val), keep_whitespace=True)
-        case b'union':
-            return nodes.NodeUnion(*(compile_node_name(**n) for n in val))
-        case b'range':
-            return nodes.NodeRange(compile_node_name(**val['node']), int(val['min'] or 0), int(val['max']) if val['max'] else None)
-        case b'range_ws_sensitive':
-            return nodes.NodeRange(compile_node_name(**val['node']), int(val['min'] or 0), int(val['max']) if val['max'] else None, keep_whitespace=True)
-        case b'string':
-            return nodes.StringNode(codecs.escape_decode(val)[0])
-        case b'pattern':
-            flags = re.NOFLAG
-            for k,f in basic_compiler.RE_FLAGS.items():
-                if k in val['flags']: flags |= f
-            return nodes.PatternNode(re.compile(val['pattern'], flags), int(val['group']) if val['group'] else None)
-        case b'stealer':
-            return nodes.Stealer()
-        case b'context':
-            ctx = val.get('raw', None)
-            if ctx is None:
-                ctx = codecs.escape_decode(val['str'])[0]
-            return nodes.Context(ctx)
-        case b'noderef':
-            return nodes.NodeRef(val)
-        case _:
-            raise TypeError(f'Unknown node type {type!r}')
+            # Parse statements
+            stmt = self.grammar[b'STATEMENT'](bm, stealer=True)
+            working[stmt['name']] = stmt['expr']
+        return working
+    ### Pragma
+    def handle_pragma(self, type_: bytes, args: bytes, *, working: dict[bytes, dict],
+                      bm: buffer_matcher.SimpleBufferMatcher, source: Path | str | None = None) -> None:
+        '''Handles a pragma statement during compilation'''
+        match type_:
+            case b'include':
+                if not args:
+                    raise SyntaxError('Include pragma requires args')
+                f = Path(args.decode())
+                if f.is_absolute():
+                    working.update(self.compile_path(f, bind=False, precompile_only=True))
+                    return
+                if isinstance(source, Path) and (nf := (source.parent / f)).is_file(): pass
+                elif (nf := (Path.cwd() / f)).is_file(): pass
+                elif (nf := (self.base_path / f)).is_file(): pass
+                else: raise FileNotFoundError(f'Cannot resolve relative file from include: {f}')
+                working.update(self.compile_path(nf, bind=False, precompile_only=True))
+            case _:
+                raise TypeError(f'Unknown pragma type {type_!r}')
+
+    ## Compile
+    def post_process_compile(working: dict[bytes, dict], *, bind: bool = True) -> dict[bytes, nodes.Node]:
+        '''Compiles pre-processed grammar into nodes'''
+        for k,v in working.items():
+            print(k, v)
```

### Comparing `caustic_lexer-0.2/src/caustic/lexer/nodes.py` & `caustic_lexer-1/src/caustic/lexer/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 #> Imports
 import io
 import re
 import typing
 from abc import ABCMeta, abstractmethod
 from buffer_matcher import SimpleBufferMatcher
 from collections import abc as cabc
+
+from .util import WHITESPACE_PATT
+from .util import NO_MATCH
 #</Imports
 
 #> Header >/
-__all__ = ('WHITESPACE_PATT', 'NodeSyntaxError',
+__all__ = ('NodeSyntaxError',
            'Node', 'NodeGroup', 'NodeUnion', 'NodeRange',
            'StringNode', 'PatternNode',
            'Stealer', 'Context', 'NodeRef')
 
-WHITESPACE_PATT = re.compile(rb'\s+')
-
 # Exceptions
 class NodeSyntaxError(SyntaxError):
     '''For when nodes fail to match something that must be matched'''
     __slots__ = ('node',)
 
     node: 'Node'
     bm: SimpleBufferMatcher
@@ -43,16 +44,14 @@
             return sio.getvalue()
 # Nodes
 ## Base
 class Node(metaclass=ABCMeta):
     '''The base class for all nodes'''
     __slots__ = ('name',)
 
-    NO_RETURN = object()
-
     name: str | None
 
     def __init__(self, *, name: str | None = None):
         self.name = name
 
     def bind(self, nodes: dict[bytes, typing.Self]) -> None:
         '''Binds all sub-nodes, if possible'''
@@ -104,18 +103,18 @@
                 stealer = True
                 after = self.nodes[-1]
                 continue
             # Execute node
             try: res = n(bm, stealer=stealer)
             except NodeSyntaxError as nse:
                 raise NodeSyntaxError(self, bm, f'Node {i} failed underneath node-group') from nse
-            if res is self.NO_RETURN:
+            if res is NO_MATCH:
                 assert not stealer
                 bm.load_pos(save)
-                return self.NO_RETURN
+                return NO_MATCH
             # Check how we should return results
             if n.name is None: # not assigned a name ("[name]:<node>")
                 if isinstance(results, dict): continue # don't add it
                 if not single_result: results.append(res)
             elif n.name: # name is not blank ("<name>:<node>")
                 if isinstance(results, dict):
                     results[n.name] = res
@@ -150,18 +149,18 @@
 
     def __init__(self, *nodes: Node, **kwargs):
         super().__init__(**kwargs)
         self.nodes = nodes
 
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> object | dict[str, typing.Any]:
         for n in self.nodes:
-            if (res := n(bm)) is not self.NO_RETURN:
+            if (res := n(bm)) is not NO_MATCH:
                 return res
         if stealer: raise NodeSyntaxError(self, bm, f'Expected union {self}')
-        return self.NO_RETURN
+        return NO_MATCH
 
     def __str__(self) -> str:
         return f'{"" if self.name is None else f"{self.name}:"}[ {" ".join(map(str, self.nodes))} ]'
     def __repr__(self) -> str:
         return f'<{type(self).__qualname__} {self.name!r} {self.nodes!r}>'
 
     @classmethod
@@ -192,28 +191,28 @@
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> object | list[typing.Any]:
         results = []
         save = bm.save_pos()
         for _ in range(self.min):
             try: results.append(self.node(bm, stealer=stealer))
             except NodeSyntaxError as nse:
                 raise NodeSyntaxError(self, bm, f'Expected at least {self.min} of {self.node}') from nse
-            if results[-1] is self.NO_RETURN:
+            if results[-1] is NO_MATCH:
                 self.load_pos()
-                return self.NO_RETURN
+                return NO_MATCH
             if not self.keep_whitespace:
                 bm.match(WHITESPACE_PATT)
         if self.max is None:
-            while (res := self.node(bm)) is not self.NO_RETURN:
+            while (res := self.node(bm)) is not NO_MATCH:
                 results.append(res)
                 if not self.keep_whitespace:
                     bm.match(WHITESPACE_PATT)
         else:
             for _ in range(self.min, self.max):
                 res = self.node(bm)
-                if res is self.NO_RETURN: break
+                if res is NO_MATCH: break
                 results.append(res)
                 if not self.keep_whitespace:
                     bm.match(WHITESPACE_PATT)
         return results
 
     def __str__(self) -> str:
         return f'{self.min or ""}-{"" if self.max is None else {self.max}} {self.node}'
@@ -234,15 +233,15 @@
             raise ValueError('Cannot use an empty string')
 
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> object | bytes:
         if bm.match(self.string):
             return self.string
         if stealer:
             raise NodeSyntaxError(self, bm, f'Expected string {self}')
-        return self.NO_RETURN
+        return NO_MATCH
 
     def __str__(self) -> str:
         return f'"{"" if self.name is None else f"{self.name}:"}{self.string.decode(errors="backslashreplace").replace("\"", "\\\"")}"'
     def __repr__(self) -> str:
         return f'<{type(self).__qualname__} {self.name!r} {self.string!r}>'
 class PatternNode(Node):
     '''Matches a pattern (regular expression)'''
@@ -257,15 +256,15 @@
         self.group = group
 
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> object | re.Match | bytes:
         if (m := bm.match(self.pattern)) is not None:
             return m.group(self.group) if self.group is not None else m
         if stealer:
             raise NodeSyntaxError(self, bm, f'Expected pattern {self}')
-        return self.NO_RETURN
+        return NO_MATCH
 
     FLAGS = {'i': re.IGNORECASE, 'm': re.MULTILINE, 's': re.DOTALL}
     def __str__(self) -> str:
         return (f'{"" if self.name is None else f"{self.name}:"}'
                 f'{"" if self.group is None else self.group}/'
                 f'{self.pattern.pattern.decode(errors="backslashreplace").replace("/", "\\/")}/'
                 f'{"".join(f for f,v in self.FLAGS.items() if v & self.pattern.flags)}')
@@ -285,15 +284,15 @@
 class Context(Node):
     '''Marks a special "context" node that always matches'''
     __slots__ = ('val',)
 
     val: typing.Any
 
     def __init__(self, val: typing.Any, **kwargs):
-        assert val is not self.NO_RETURN, 'Cannot use NO_RETURN marker object for Context val'
+        assert val is not NO_MATCH, 'Cannot use NO_MATCH marker object for Context val'
         super().__init__(**kwargs)
         self.val = val
 
     def __call__(self, bm: SimpleBufferMatcher, *, stealer: bool = False) -> typing.Any:
         return self.val
 
     def __str__(self) -> str:
```

### Comparing `caustic_lexer-0.2/src/caustic/lexer/serialize.py` & `caustic_lexer-1/src/caustic/lexer/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic_lexer-0.2/src/caustic.lexer.egg-info/PKG-INFO` & `caustic_lexer-1/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 0.2.0
+Version: 1.0.0
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,28 +39,25 @@
 
 # The `.cag` specification
 
 ## Pragmas
 Pragmas are special directives embedded in the grammar  
 These are only supported on the bootstrapped `compile` module
 
-### Include / Import
-> `$include [path]`, `$import [path]`
+### Include
+> `$include [path]`
 
 Allows putting multiple grammar files together
 
 Relative paths provided as `[path]` will be checked against the following
 directories, in order:
 - The path of the includer/importer (if possible)
 - The `builtin_path` of the `compiler` module (the location of `compiler.py`)
 - The current directory
 
-The difference between include and import is that included nodes will be bound
-with the rest of the nodes from the includer, whilst imported nodes will not
-
 ## Comments
 Comments may start with a `#`
 
 ## Statements
 A statement begins with an [identifier](#identifier), followed by an `=`,
 then an [expression](#expression), and finally a `;`
 
@@ -179,7 +176,13 @@
 
 
 # Changelog
 
 ## 0.2.0
 - Implemented node saving and loading through the `serialize` module
 - Moved `compiler.bind_nodes()` to `util.bind_nodes()`
+
+## 1.0.0
+- Completely reworked compiler caching
+- Removed `$import` pragma
+- Moved `WHITESPACE_PATT` to `.util`
+- Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
```

