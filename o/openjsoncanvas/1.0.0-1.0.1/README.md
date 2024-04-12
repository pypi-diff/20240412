# Comparing `tmp/openjsoncanvas-1.0.0.tar.gz` & `tmp/openjsoncanvas-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-1.0.0.tar` & `openjsoncanvas-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.0/LICENSE
--rw-r--r--   0        0        0     3918 2024-04-12 12:51:17.779560 openjsoncanvas-1.0.0/openjsoncanvas.py
--rw-r--r--   0        0        0      368 2024-04-12 13:08:22.206321 openjsoncanvas-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2207 2024-04-12 13:30:02.375683 openjsoncanvas-1.0.1/README
+-rw-r--r--   0        0        0     4799 2024-04-12 14:04:05.401592 openjsoncanvas-1.0.1/openjsoncanvas.py
+-rw-r--r--   0        0        0      368 2024-04-12 13:08:22.206321 openjsoncanvas-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.1/PKG-INFO
```

### Comparing `openjsoncanvas-1.0.0/LICENSE` & `openjsoncanvas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.0/openjsoncanvas.py` & `openjsoncanvas-1.0.1/openjsoncanvas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,28 @@
-"""A python implmentation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md"""
+"""A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md"""
 import dataclasses
 import json
 import pathlib
 import re
 import typing
-__version__: str = '1.0.0'
+import functools
+import pprint
+__version__: str = '1.0.1'
 
 camel_to_name = lambda x: re.sub(r'(?<!^)(?=[A-Z])', '_', x).lower()
 
+@functools.lru_cache
+def get_leaf_subclass(cls, name):
+    if cls.__subclasses__():
+        for subcls in cls.__subclasses__():
+            if subcls.__subclasses__():
+                return get_leaf_subclass(subcls, name)
+            if subcls.__name__ == name:
+                return subcls
+    return cls
 class CanvasData(typing.MutableMapping):
     __getattr__ = __getitem__ = lambda self, key: super().__getattribute__(camel_to_name(key))
     __setattr__ = __setitem__ = lambda self, key, value: super().__setattr__(camel_to_name(key), value)
     __delattr__ = __delitem__ = lambda self, key: super().__delattr__(camel_to_name(key))
     __len__ = lambda self: len(self.__dict__)
     __contains__ = lambda self, key: camel_to_name(key) in self.__dict__
     __iter__ = lambda self: iter(self.__dict__)
@@ -34,15 +45,14 @@
     color: typing.Optional[str] = None
 
 @dataclasses.dataclass(kw_only=True)
 class TextNode(Node):
     text: str
     type: str = 'text'
     
-    
 @dataclasses.dataclass(kw_only=True)
 class FileNode(Node):
     file: str
     type: str = 'file'
     subpath: typing.Optional[str] = None
     
 @dataclasses.dataclass(kw_only=True)
@@ -57,19 +67,19 @@
     background: typing.Optional[str] = None
     backgroundStyle: typing.Optional[str] = None
     
 @dataclasses.dataclass(kw_only=True)
 class Edge(CanvasData):
     id: str
     fromNode: str
-    fromSide: typing.Optional[str] = None
-    fromEnd: typing.Optional[str] = None
     toNode: str
-    toSide: typing.Optional[str] = None
-    toEnd: typing.Optional[str] = None
+    fromSide: typing.Optional[typing.Literal['top', 'right', 'bottom', 'left']] = None
+    toSide: typing.Optional[typing.Literal['top', 'right', 'bottom', 'left']] = None
+    fromEnd: typing.Optional[typing.Literal['none', 'arrow']] = None
+    toEnd: typing.Optional[typing.Literal['none', 'arrow']] = None
     color: typing.Optional[str] = None
     label: typing.Optional[str] = None
     
 @dataclasses.dataclass(kw_only=True)
 class Canvas:
     nodes: typing.List[Node] = dataclasses.field(default_factory=list)
     edges: typing.List[Edge] = dataclasses.field(default_factory=list)
@@ -92,29 +102,39 @@
         self.edges.append(edge)
         return self
     
     @classmethod
     def from_json(cls, json_str):
         data = json.loads(json_str)
         return cls(
-                nodes=[globals()[node_data['type'].title() + 'Node'](**node_data) for node_data in (data).get('nodes', [])], 
+                nodes=[
+                        get_leaf_subclass(Node, node_data['type'].title() + "Node")(**node_data) 
+                        for node_data in data.get('nodes', [])
+                ],
                 edges=[Edge(**edge_data) for edge_data in data.get('edges', [])]
         )
     
     def to_file(self, path):
         path = pathlib.Path(path)
         path.write_text(self.to_json())
-        
     @classmethod
     def from_file(cls, path):
         path = pathlib.Path(path)
         content = path.read_text()
         if not content:
             return cls()
         return cls.from_json(content)
+    
+    def __str__(self):
+        nodes = pprint.pformat(self.nodes)
+        edges = pprint.pformat(self.edges)
+        # properly indent the nodes and edges
+        nodes = '\n'.join('    ' + line for line in nodes.splitlines())
+        edges = '\n'.join('    ' + line for line in edges.splitlines())
+        return f'Canvas(\n  nodes=\n{nodes}\n  ,\n  edges=\n{edges}\n  \n)'
 
     
 if __name__ == '__main__':
     path = r"G:\vault\Wiki\Untitled.canvas"
-    canvas = Canvas.from_file(path)
-    canvas.add_node(TextNode(id='1', x=100, y=100, width=100, height=100, text='Hello World'))
-    canvas.to_file(path)
+    #canvas = Canvas.from_file(path)
+    #print(canvas)
+    print(json.load(open(path)))
```

