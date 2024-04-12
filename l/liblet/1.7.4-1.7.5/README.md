# Comparing `tmp/liblet-1.7.4.tar.gz` & `tmp/liblet-1.7.5.tar.gz`

## Comparing `liblet-1.7.4.tar` & `liblet-1.7.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/api.rst
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/conf.py
--rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples.ipynb
--rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples.rst
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/index.rst
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/installation.rst
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/stg.svg
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/tree.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_static/custom.css
--rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_static/logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/_templates/project.html
--rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_70_0.svg
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_71_0.svg
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_82_0.svg
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_83_0.svg
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.4/docs/examples_files/examples_8_0.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.4/src/scripts.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/__init__.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/antlr.py
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/automaton.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/const.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/decorators.py
--rw-r--r--   0        0        0    20902 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/display.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/grammar.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/llvm.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 liblet-1.7.4/src/liblet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/antlr_test.py
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/automaton_test.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/decorators_test.py
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/grammar_test.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/run.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.4/src/tests/utils_test.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.4/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.4/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.4/LICENSE-GPL.txt
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.4/README.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     8113 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/api.rst
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/conf.py
+-rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples.ipynb
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples.rst
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/index.rst
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/installation.rst
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/stg.svg
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/tree.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_static/custom.css
+-rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_static/logo.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/_templates/project.html
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_70_0.svg
+-rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_71_0.svg
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_82_0.svg
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_83_0.svg
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.5/docs/examples_files/examples_8_0.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.5/src/scripts.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/__init__.py
+-rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/antlr.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/automaton.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/const.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/decorators.py
+-rw-r--r--   0        0        0    21005 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/display.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/grammar.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/llvm.py
+-rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 liblet-1.7.5/src/liblet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/__init__.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/antlr_test.py
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/automaton_test.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/decorators_test.py
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/grammar_test.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/run.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.5/src/tests/utils_test.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.5/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.5/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.5/LICENSE-GPL.txt
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.5/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.5/PKG-INFO
```

### Comparing `liblet-1.7.4/docs/api.rst` & `liblet-1.7.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/conf.py` & `liblet-1.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples.ipynb` & `liblet-1.7.5/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples.rst` & `liblet-1.7.5/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/index.rst` & `liblet-1.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/installation.rst` & `liblet-1.7.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/stg.svg` & `liblet-1.7.5/docs/stg.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/tree.svg` & `liblet-1.7.5/docs/tree.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/_static/logo.png` & `liblet-1.7.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/_templates/project.html` & `liblet-1.7.5/docs/_templates/project.html`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples_files/examples_70_0.svg` & `liblet-1.7.5/docs/examples_files/examples_70_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples_files/examples_71_0.svg` & `liblet-1.7.5/docs/examples_files/examples_71_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples_files/examples_82_0.svg` & `liblet-1.7.5/docs/examples_files/examples_82_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples_files/examples_83_0.svg` & `liblet-1.7.5/docs/examples_files/examples_83_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/docs/examples_files/examples_8_0.svg` & `liblet-1.7.5/docs/examples_files/examples_8_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/liblet/__init__.py` & `liblet-1.7.5/src/liblet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.7.4'
+__version__ = '1.7.5'
 
 from liblet.antlr import ANTLR, AnnotatedTreeWalker
 from liblet.automaton import (
   Automaton,
   BottomUpInstantaneousDescription,
   InstantaneousDescription,
   TopDownInstantaneousDescription,
@@ -40,15 +40,14 @@
   peek,
   suffixes,
   uc,
   union_of,
   warn,
 )
 
-
 __all__ = [
   '__version__',
   'animate_derivation',
   'AnnotatedTreeWalker',
   'ANTLR',
   'AttrDict',
   'Automaton',
```

### Comparing `liblet-1.7.4/src/liblet/antlr.py` & `liblet-1.7.5/src/liblet/antlr.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,16 @@
     Unless a *simple* tree is required, the returned is an *annotated* tree whose nodes store
     context information from the parsing process, more precisely, nodes are :obj:`dicts <dict>` with the following keys:
 
     - ``type``: can be ``rule`` or ``token``,
     - ``name``: the *rule label* or *token name* (or the rule name if it has no label: or, similarly, the token itself if it has no name),
     - ``value``: the *token* value (only present for *tokens* named in the *lexer* part of the grammar),
     - ``rule``: the *rule* name (only present for *rules*, will be different from ``name`` for labelled rules).
-    - ``src``: the first (and last token, in case of a rule), corredponding to the node.
+    - ``src``: the first (and last token, in case of a rule), corresponding to the node.
+    - ``line``: the line number of the (first) token.
 
     Note that the values are strings (so if the *value* is a number, it should be converted before usage).
 
     This method removes any ``<EOF>`` tree returned in the underlying parse tree (unless a simple tree is required).
 
     Args:
       text (str): the text to be parsed.
@@ -213,28 +214,28 @@
     def _rule(ctx):
       rule = self.Parser.ruleNames[ctx.getRuleIndex()]
       if simple:
         return rule
       name = ctx.__class__.__name__
       name = name[:-7]  # remove trailing 'Context'
       name = name[0].lower() + name[1:]
-      return {'type': 'rule', 'name': name, 'rule': rule, 'src': ctx.getSourceInterval()}
+      return {'type': 'rule', 'name': name, 'rule': rule, 'src': ctx.getSourceInterval(), 'line': ctx.start.line} 
 
     def _token(token):
       ts = token.symbol
       text = r'\\n' if ts.text == '\n' else ts.text
       if simple:
         return text
       try:
         name = self.Parser.symbolicNames[ts.type]
       except IndexError:
         name = '<INVALID>'
       if name == '<INVALID>':
         name = self.Parser.literalNames[ts.type][1:-1]
-      return {'type': 'token', 'name': name, 'value': text, 'src': token.symbol.tokenIndex}
+      return {'type': 'token', 'name': name, 'value': text, 'src': ts.tokenIndex, 'line': ts.line}
 
     class TreeVisitor(ParseTreeVisitor):
       def visitTerminal(self, t):
         if t.symbol.type == -1:
           return None
         return Tree(_token(t))
```

### Comparing `liblet-1.7.4/src/liblet/automaton.py` & `liblet-1.7.5/src/liblet/automaton.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
     """Attempts a prediction move, given the specified production, and returns the corresponding new instantaneous description."""
     if P in self.G.P and self.top() == P.lhs:
       c = copy(self)
       c.stack = copy(c.stack)
       c.stack.pop()
       c.steps += (P,)
       for X in reversed(P.rhs):
-        c.stack.push(X)
+        if X !=  ε :c.stack.push(X)
       return c
     raise ValueError('The top of the stack does not correspond to the production lhs.')
 
 
 class BottomUpInstantaneousDescription(InstantaneousDescription):
   """An Instantaneous Description for a *bottom-up* parsing automaton.
```

### Comparing `liblet-1.7.4/src/liblet/decorators.py` & `liblet-1.7.5/src/liblet/decorators.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/liblet/display.py` & `liblet-1.7.5/src/liblet/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 from warnings import warn as wwarn
 
 import svgutils.transform as svg_ttransform
 from graphviz import Digraph
 from IPython.display import HTML, SVG, display
 from ipywidgets import IntSlider, interactive
 
-
-from liblet.const import ε, FONT_NAME
+from liblet.const import GV_FONT_NAME, GV_FONT_SIZE, HTML_FONT_NAME, ε
 from liblet.grammar import HAIR_SPACE, Derivation, Productions
 from liblet.utils import AttrDict, CYKTable, compose, letstr
 
 
 def _escape(label):
   return sub(r'\]', '&#93;', sub(r'\[', '&#91;', escape(str(label))))
 
@@ -109,18 +108,18 @@
 
   return NodeWrapper
 
 
 class GVWrapper:
   def __init__(self, gv_graph_args=None, node_wrapper=None):
     gv_graph_args = gv_graph_args or {}
-    gv_graph_args['node_attr'] = {'fontname': f"'{FONT_NAME}'"} | (
+    gv_graph_args['node_attr'] = {'fontname': GV_FONT_NAME, 'fontsize': GV_FONT_SIZE} | (
       gv_graph_args['node_attr'] if 'node_attr' in gv_graph_args else {}
     )
-    gv_graph_args['edge_attr'] = {'fontname': f"'{FONT_NAME}'"} | (
+    gv_graph_args['edge_attr'] = {'fontname': GV_FONT_NAME, 'fontsize': GV_FONT_SIZE} | (
       gv_graph_args['edge_attr'] if 'edge_attr' in gv_graph_args else {}
     )
     node_wrapper = node_wrapper or make_node_wrapper()
     self.G = Digraph(**gv_graph_args)
     self.node_wrapper = node_wrapper
     self.nodes = set()
 
@@ -572,15 +571,19 @@
   return ui
 
 
 # HTML/SVG stuff
 
 
 def __bordered_table__(content):  # noqa: N807
-  return HTML(f'<style>td, th {{border: 1pt solid lightgray !important;}} * {{font-family: "{FONT_NAME}";}}</style><table>' + content + '</table>')
+  return HTML(
+    f'<style>td, th {{border: 1pt solid lightgray !important;}} table * {{font-family: "{HTML_FONT_NAME}";}}</style><table>'
+    + content
+    + '</table>'
+  )
 
 
 def resized_svg_repr(obj, width=800, height=600):
   if hasattr(obj, '_repr_image_svg_xml'):
     svg_str = obj._repr_image_svg_xml()
   elif hasattr(obj, '_repr_svg_'):
     svg_str = obj._repr_svg_()
```

### Comparing `liblet-1.7.4/src/liblet/grammar.py` & `liblet-1.7.5/src/liblet/grammar.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/liblet/llvm.py` & `liblet-1.7.5/src/liblet/llvm.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/liblet/utils.py` & `liblet-1.7.5/src/liblet/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from collections.abc import MutableMapping, Set  #  noqa: PYI025
 from functools import partial, reduce
 from html import escape
 from itertools import chain
 from sys import stderr
 from warnings import warn as wwarn
 
-from liblet.const import FONT_NAME
+from liblet.const import HTML_FONT_NAME
+
 
 def suffixes(α):
   for i in range(len(α)):
     yield α[i:]
 
 
 def warn(msg):
@@ -156,15 +157,15 @@
     del self.__store[key]
 
   def __iter__(self):
     return iter(self.__store)
 
   def __len__(self):
     return len(self.__store)
-  
+
   def __repr__(self):
     return f'AttrDict({self.__store})'
 
 
 class Table:
   """A one or two-dimensional *table* able to detect conflicts and with a nice HTML representation, based on :obj:`~collections.defaultdict`."""
 
@@ -252,15 +253,15 @@
           if c in self.data[r]:
             R.data[r][c] = self.data[r][c]
     return R
 
   def _repr_html_(self):
     def _table(content):
       return (
-        f'<style>td, th {{border: 1pt solid lightgray !important; text-align: left !important;}} * {{font-family: "{FONT_NAME}";}}</style><table>'
+        f'<style>td, th {{border: 1pt solid lightgray !important; text-align: left !important;}} table * {{font-family: "{HTML_FONT_NAME}";}}</style><table>'
         + content
         + '</table>'
       )
 
     def _fmt(r, c):
       if c not in self.data[r]:
         return '&nbsp;'
```

### Comparing `liblet-1.7.4/src/tests/antlr_test.py` & `liblet-1.7.5/src/tests/antlr_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,45 +77,45 @@
       OP: '+' | '-' ;
       ID: [a-z];
     """
     )
     tree = str(Bad.tree('z-a+a*x', 'start'))
     self.assertEqual(
       tree,
-      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 6)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 6)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 4)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 2)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0)}: ({'type': 'token', 'name': 'ID', 'value': 'z', 'src': 0})), ({'type': 'token', 'name': 'OP', 'value': '-', 'src': 1}), ({'type': 'token', 'name': 'ID', 'value': 'a', 'src': 2})), ({'type': 'token', 'name': 'OP', 'value': '+', 'src': 3}), ({'type': 'token', 'name': 'ID', 'value': 'a', 'src': 4})), ({'type': 'token', 'name': '*', 'value': '*', 'src': 5}), ({'type': 'token', 'name': 'ID', 'value': 'x', 'src': 6})))",
+      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 6), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 6), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 4), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 2), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0), 'line': 1}: ({'type': 'token', 'name': 'ID', 'value': 'z', 'src': 0, 'line': 1})), ({'type': 'token', 'name': 'OP', 'value': '-', 'src': 1, 'line': 1}), ({'type': 'token', 'name': 'ID', 'value': 'a', 'src': 2, 'line': 1})), ({'type': 'token', 'name': 'OP', 'value': '+', 'src': 3, 'line': 1}), ({'type': 'token', 'name': 'ID', 'value': 'a', 'src': 4, 'line': 1})), ({'type': 'token', 'name': '*', 'value': '*', 'src': 5, 'line': 1}), ({'type': 'token', 'name': 'ID', 'value': 'x', 'src': 6, 'line': 1})))",
     )
 
   def test_nolexersym(self):
     NoSym = ANTLR(
       r"""
       grammar NoSym ;
 
       start: expr * ;
       expr: 'a';
     """
     )
     tree = str(NoSym.tree('aa', 'start'))
     self.assertEqual(
       tree,
-      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 1)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0)}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 0})), ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (1, 1)}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 1})))",
+      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 1), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0), 'line': 1}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 0, 'line': 1})), ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (1, 1), 'line': 1}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 1, 'line': 1})))",
     )
 
   def test_eof(self):
     NoSym = ANTLR(
       r"""
       grammar NoSym ;
 
       start: expr * EOF;
       expr: 'a';
     """
     )
     tree = str(NoSym.tree('aa', 'start'))
     self.assertEqual(
       tree,
-      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 1)}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0)}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 0})), ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (1, 1)}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 1})))",
+      r"({'type': 'rule', 'name': 'start', 'rule': 'start', 'src': (0, 1), 'line': 1}: ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (0, 0), 'line': 1}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 0, 'line': 1})), ({'type': 'rule', 'name': 'expr', 'rule': 'expr', 'src': (1, 1), 'line': 1}: ({'type': 'token', 'name': 'a', 'value': 'a', 'src': 1, 'line': 1})))",
     )
 
   def test_diag(self):
     with unittest.mock.patch('liblet.antlr.warn') as mock_warn:
       Ambig = ANTLR(
         r"""
         grammar Ambig;
```

### Comparing `liblet-1.7.4/src/tests/automaton_test.py` & `liblet-1.7.5/src/tests/automaton_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/tests/decorators_test.py` & `liblet-1.7.5/src/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/tests/grammar_test.py` & `liblet-1.7.5/src/tests/grammar_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/src/tests/utils_test.py` & `liblet-1.7.5/src/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/LICENSE-CC.txt` & `liblet-1.7.5/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/LICENSE-GPL.txt` & `liblet-1.7.5/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/README.md` & `liblet-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/pyproject.toml` & `liblet-1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liblet-1.7.4/PKG-INFO` & `liblet-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liblet
-Version: 1.7.4
+Version: 1.7.5
 Summary: A teaching aid library for formal languages and compiler courses.
 Project-URL: Documentation, https://liblet.readthedocs.io/
 Project-URL: Source code, https://github.com/let-unimi/liblet
 Project-URL: Changelog, https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt
 Project-URL: Bug Tracker, https://github.com/let-unimi/liblet/issues
 Author-email: Massimo Santini <massimo.santini@unimi.it>
 License-File: LICENSE-CC.txt
```

