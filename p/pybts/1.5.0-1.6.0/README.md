# Comparing `tmp/pybts-1.5.0.tar.gz` & `tmp/pybts-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.5.0.tar", max compression
+gzip compressed data, was "pybts-1.6.0.tar", max compression
```

## Comparing `pybts-1.5.0.tar` & `pybts-1.6.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0   157658 2024-04-11 19:12:46.142182 pybts-1.5.0/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-11 19:12:46.142182 pybts-1.5.0/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-11 19:12:46.146182 pybts-1.5.0/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-11 19:12:46.146182 pybts-1.5.0/README.md
--rw-r--r--   0        0        0      393 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/board.py
--rw-r--r--   0        0        0     9994 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/board/server.py
--rw-r--r--   0        0        0     7780 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/builder.py
--rw-r--r--   0        0        0      548 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8666 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/composite.py
--rw-r--r--   0        0        0     2175 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5661 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/parallel.py
--rw-r--r--   0        0        0      944 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/selector.py
--rw-r--r--   0        0        0     2541 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/sequence.py
--rw-r--r--   0        0        0      182 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/composites/template.py
--rw-r--r--   0        0        0     3243 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/constants.py
--rw-r--r--   0        0        0     3618 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    19980 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/main.py
--rw-r--r--   0        0        0    10981 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/node.py
--rw-r--r--   0        0        0       63 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/__init__.py
--rw-r--r--   0        0        0     9353 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/base_class.py
--rw-r--r--   0        0        0      268 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/common.py
--rw-r--r--   0        0        0    15319 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/nodes.py
--rw-r--r--   0        0        0     6137 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/off_policy.py
--rw-r--r--   0        0        0     7295 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1183 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-11 19:12:46.150182 pybts-1.5.0/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-11 19:12:46.162182 pybts-1.5.0/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     1553 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/tree.py
--rw-r--r--   0        0        0    10044 2024-04-11 19:12:46.166182 pybts-1.5.0/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-11 19:12:46.166182 pybts-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-12 21:31:23.883104 pybts-1.6.0/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-12 21:31:23.883104 pybts-1.6.0/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-12 21:31:23.887104 pybts-1.6.0/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-12 21:31:23.887104 pybts-1.6.0/README.md
+-rw-r--r--   0        0        0      385 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/board.py
+-rw-r--r--   0        0        0     9994 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/board/server.py
+-rw-r--r--   0        0        0     8003 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/builder.py
+-rw-r--r--   0        0        0      596 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     9344 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2175 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      945 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     1510 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/switcher.py
+-rw-r--r--   0        0        0      182 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/composites/template.py
+-rw-r--r--   0        0        0     3243 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/constants.py
+-rw-r--r--   0        0        0     4548 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    22175 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/main.py
+-rw-r--r--   0        0        0    14150 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/nodes.py
+-rw-r--r--   0        0        0       63 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     8862 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/common.py
+-rw-r--r--   0        0        0    15448 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     5688 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     7196 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1184 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-12 21:31:23.891104 pybts-1.6.0/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     2140 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/tree.py
+-rw-r--r--   0        0        0    10045 2024-04-12 21:31:23.903104 pybts-1.6.0/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-12 21:31:23.903104 pybts-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.6.0/PKG-INFO
```

### Comparing `pybts-1.5.0/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.6.0/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/README.assets/image-20240329031220580.png` & `pybts-1.6.0/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/README.assets/image-20240329031233459.png` & `pybts-1.6.0/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/README.assets/image-20240401211552611.png` & `pybts-1.6.0/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/README.assets/image-20240401211609525.png` & `pybts-1.6.0/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/README.md` & `pybts-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/board/board.py` & `pybts-1.6.0/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/board/server.py` & `pybts-1.6.0/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/builder.py` & `pybts-1.6.0/pybts/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import json
 import os.path
 from typing import Callable
 import xml.etree.ElementTree as ET
 import copy
-from pybts.node import *
+from pybts.nodes import *
 from pybts.composites import *
 from pybts.decorators import *
 import uuid
 from pybts.utility import camel_case_to_snake_case
 
 
 class Builder:
@@ -69,20 +69,21 @@
             if os.path.exists(folder_filepath) and os.path.isfile(folder_filepath):
                 return folder_filepath
 
         return ''
 
     def read_text_from_file(self, filepath: str) -> str:
         # 从folder中找文件
+        init_filepath = filepath
         filepath = self.find_filepath(filepath=filepath)
         if filepath != '' and os.path.exists(filepath) and os.path.isfile(filepath):
             with open(filepath, 'r', encoding='utf-8') as file:
                 return file.read()
 
-        raise Exception(f'Cannot find file: {filepath}')
+        raise Exception(f'Cannot find file: {init_filepath}')
 
     def build_from_file(self, filepath: str, attrs: dict = None):
         """
         attrs: 传递给每个节点的参数，优先级弱于节点本身设置的参数，高于builder设置的global_attrs参数
         """
         text = self.read_text_from_file(filepath=filepath)
         if filepath.endswith('.json'):
@@ -157,23 +158,28 @@
                 Selector,
                 ReactiveSelector,
                 SelectorWithMemory,
                 ConditionBranch,
                 Template,
                 PreCondition,
                 PostCondition,
-                Print
+                Switcher,
+                ReactiveSwitcher,
         )
 
         self.register_node(
                 Failure,
                 Success,
                 Running,
                 IsChanged,
-                IsMatchRule
+                IsMatchRule,
+                IsEqual,
+                Print,
+                RandomIntValue,
+                RandomFloatValue
         )
 
         self.register_node(
                 Inverter,
                 RunningUntilCondition,
                 OneShot,
                 Count,
@@ -181,14 +187,15 @@
                 RunningIsSuccess,
                 FailureIsSuccess,
                 FailureIsRunning,
                 SuccessIsFailure,
                 SuccessIsRunning,
                 Timeout,
                 Throttle,
+                IsStatusChanged
         )
 
         # 且或非
         self.register('And', Sequence)
         self.register('Or', Selector)
         self.register('Not', Inverter)
         self.register('Root', Parallel)  # 可以作为根节点
```

### Comparing `pybts-1.5.0/pybts/composites/__init__.py` & `pybts-1.6.0/pybts/composites/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .composite import Composite
 from .parallel import Parallel
 from .selector import Selector, SelectorWithMemory, ReactiveSelector
 from .sequence import Sequence, SequenceWithMemory, ReactiveSequence
 from .condition_branch import ConditionBranch
 from .template import Template
 from .ppa import PreCondition, PostCondition
-
+from .switcher import Switcher, ReactiveSwitcher
 # TODO: RUNNING节点的打断操作应该怎么在行为树上体现出来
 # 通过ReactiveSelector/ReactiveSequence来起到打断后续节点的效果
 # ReactiveSequence: 前面的节点条件如果满足，则会一直
```

### Comparing `pybts-1.5.0/pybts/composites/composite.py` & `pybts-1.6.0/pybts/composites/composite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import py_trees
-from pybts.node import Node
+from pybts.nodes import Node
 from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 import itertools
 import uuid
 
@@ -254,7 +254,24 @@
 
         # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
         # if new_status != Status.RUNNING:
         #     self.stop(new_status)
 
         self.status = new_status
         yield self
+
+    def switch_tick(self, index: int, tick_again_status: list[Status]) -> typing.Iterator[py_trees.behaviour.Behaviour]:
+        if self.status in tick_again_status:
+            # 重新执行上次执行的子节点
+            assert self.current_child is not None
+        else:
+            self.current_child = self.children[index]  # 执行对应的index
+
+        yield from self.current_child.tick()
+        for child in self.children:
+            if child != self.current_child:
+                # 清除子节点的状态（停止正在执行的子节点）
+                child.stop(Status.INVALID)
+
+        self.status = self.current_child.status
+        yield self
+
```

### Comparing `pybts-1.5.0/pybts/composites/condition_branch.py` & `pybts-1.6.0/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/composites/parallel.py` & `pybts-1.6.0/pybts/composites/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 from pybts.composites.composite import Composite
-from pybts.composites.sequence import Sequence
-from pybts.composites.selector import Selector
 import py_trees
-from pybts.node import Node
-from abc import ABC
 import typing
 from py_trees.common import Status
-from py_trees import behaviour
-import itertools
-import uuid
 
 
 class Parallel(Composite):
     """
     组合节点：并行节点
     同时执行所有子节点，并根据成功阈值来决定返回状态
     - 如果有子节点返回 RUNNING 状态，节点本身返回 RUNNING
@@ -73,14 +66,15 @@
 
     def to_data(self):
         return {
             **super().to_data(),
             'success_threshold': self.success_threshold
         }
 
+
 # class ReactiveParallel(Parallel):
 #     """
 #     反应式并行节点
 #     忽略RUNNING节点的并行节点
 #     """
 #
 #     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
```

### Comparing `pybts-1.5.0/pybts/composites/ppa.py` & `pybts-1.6.0/pybts/composites/ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import py_trees
 import typing
 from py_trees.common import Status
 from pybts.composites.parallel import Parallel
-from pybts.node import Condition
+from pybts.nodes import Condition
 
 
 class PreCondition(Parallel, Condition):
     """前置条件"""
 
     @property
     def success_count(self) -> int:
```

### Comparing `pybts-1.5.0/pybts/composites/selector.py` & `pybts-1.6.0/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/composites/sequence.py` & `pybts-1.6.0/pybts/composites/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import py_trees
-from pybts.node import Node
-from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
-import itertools
 from pybts.composites.composite import Composite
 
 
 class Sequence(Composite):
     """
     组合节点：顺序节点
     依次顺序执行子节点
```

### Comparing `pybts-1.5.0/pybts/constants.py` & `pybts-1.6.0/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/converter.py` & `pybts-1.6.0/pybts/converter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import typing
 import jinja2
 import json
+from py_trees.common import Status
+from typing import Union
+
+_STATUS_MAP = {
+    'SUCCESS': Status.SUCCESS,
+    'FAILURE': Status.FAILURE,
+    'RUNNING': Status.RUNNING,
+    'INVALID': Status.INVALID
+}
 
 
 class Converter:
 
     def __init__(self, node):
         self.node = node
 
@@ -56,14 +65,33 @@
         if context is not None:
             ctx.update(context)
         for key in ctx:
             if callable(ctx[key]):
                 ctx[key] = ctx[key]()
         return eval(value, ctx)
 
+    @classmethod
+    def status(cls, value: Union[str, Status]) -> Status:
+        if isinstance(value, Status):
+            return value
+        value = value.upper()
+        if value not in _STATUS_MAP:
+            raise Exception(f'{value} is not a valid status')
+        return _STATUS_MAP[value]
+
+    @classmethod
+    def status_list(cls, value: Union[str, Status, list[Status]]) -> list[Status]:
+        if isinstance(value, Status):
+            return [value]
+        elif isinstance(value, list):
+            return [cls.status(value=item) for item in value]
+        elif isinstance(value, str):
+            value_list = value.split(',')
+            return [cls.status(value=item) for item in value_list if item != '']
+
     def render(self, value: str, context: dict = None) -> str:
         ctx = { }
         # if self.node.attrs is not None:
         #     ctx.update(self.node.attrs)
         if self.node.context is not None:
             ctx.update(self.node.context)
         if context is not None:
```

### Comparing `pybts-1.5.0/pybts/decorators/nodes.py` & `pybts-1.6.0/pybts/decorators/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 import py_trees
-from pybts.node import Node
+
+import pybts
+from pybts.nodes import Node
 from abc import ABC
 from py_trees.common import Status
 import typing
 
 
 class Decorator(Node, ABC):
     """
@@ -581,7 +583,68 @@
         now_time = self.get_time()
         if now_time - self.last_time >= self.duration:
             self.last_time = now_time
             yield from Decorator.tick(self)
         else:
             yield from Node.tick(self)
 
+
+class IsStatusChanged(Decorator):
+    """
+    子节点的状态变化后才会认为是成功
+
+    如果指定了from_status和to_status，则只有子节点的状态由from_status转变到to_status，才会认为是触发了状态变化
+    from_status和to_status均可以由多个状态组成，用逗号分隔
+
+    immediate: 一开始是否会触发一次IsChanged
+    """
+
+    def __init__(self, from_status: str | Status = '', to_status: str | Status = '', immediate: bool | str = False,
+                 **kwargs):
+        super().__init__(**kwargs)
+
+        self.from_status: list[Status] = self.converter.status_list(from_status)
+        self.to_status: list[Status] = self.converter.status_list(to_status)
+        self.immediate: bool = immediate
+        self.last_status = None
+        self.changed_count = 0
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.immediate = self.converter.bool(self.immediate)
+
+    def reset(self):
+        super().reset()
+        self.last_status = None
+        self.changed_count = 0
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'from_status'  : self.from_status,
+            'to_status'    : self.to_status,
+            'immediate'    : self.immediate,
+            'changed_count': self.changed_count
+        }
+
+    def check_is_changed(self):
+        if len(self.from_status) > 0 and self.last_status not in self.from_status:
+            return False
+
+        if len(self.to_status) > 0 and self.decorated.status not in self.to_status:
+            return False
+
+        if self.last_status != self.decorated.status:
+            return True
+        else:
+            return False
+
+    def update(self) -> Status:
+        self.logger.debug("%s.update() %s -> %s" % (self.__class__.__name__, self.last_status, self.decorated.status))
+        if not self.immediate and self.last_status is None:
+            self.last_status = self.decorated.status
+        is_changed = self.check_is_changed()
+        self.last_status = self.decorated.status
+        if is_changed:
+            return Status.SUCCESS
+        else:
+            return Status.FAILURE
```

### Comparing `pybts-1.5.0/pybts/display.py` & `pybts-1.6.0/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/main.py` & `pybts-1.6.0/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/node.py` & `pybts-1.6.0/pybts/nodes.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from py_trees import behaviour, common
 from py_trees.behaviour import Behaviour
 
 from pybts.constants import *
 import typing
 import py_trees
 import itertools
+import random
 
 
 class Node(py_trees.behaviour.Behaviour, ABC):
     """
     Base class for all nodes in the behavior tree
 
     被唤起的生命周期：
@@ -71,16 +72,17 @@
         if self._updater_iter is None:
             self._updater_iter = self.updater()
         new_status = Status.INVALID
         for _ in range(2):
             try:
                 new_status = next(self._updater_iter)
                 break
-            except:
+            except StopIteration:
                 self._updater_iter = self.updater()
+        assert isinstance(new_status, Status), f'{self.name}: {new_status} is not a valid status'
         return new_status
 
     def updater(self) -> typing.Iterator[Status]:
         # 提出Status.RUNNING/Status.SUCCESS/Status.FAILURE 会继续运行该迭代器
         # 提出Status.INVALID会停止该迭代器
 
         yield Status.INVALID
@@ -92,15 +94,15 @@
 
         if self.status != Status.RUNNING:
             # 开始的状态不是RUNNING
             self.initialise()
 
         # don't set self.status yet, terminate() may need to check what the current state is first
         new_status = self.update()
-
+        assert isinstance(new_status, Status), f'{self.name}: {new_status} is not a valid status'
         if new_status != Status.RUNNING:
             self.stop(new_status)
 
         self.status = new_status
         yield self
 
     def stop(self, new_status: Status) -> None:
@@ -273,73 +275,116 @@
     rule: 判断规则，默认的规则是 curr_value != last_value，可以自定义新的规则，例如 abs(curr_value - last_value) >= 10，需要确保rule返回的值是bool类型
         - rule里面也可以使用模版语法，比如 abs(curr_value - last_value) >= {{min_value}}，模版语法里的min_value需要提前在context里定义好，不然会报错
     用法示例：
     <IsChanged value="{{agent.x}}" immediate="true">
     <IsChanged value="{{agent.y}}" immediate="false" rule="abs(curr_value - last_value) >= 10">
     """
 
-    def __init__(self, value: str, immediate: bool | str = False, rule: str = '', **kwargs):
+    def __init__(self, value: typing.Any, immediate: bool | str = False, rule: str = '', **kwargs):
         super().__init__(**kwargs)
         self.value = value  # 监听的值
         self.immediate = immediate
         self.last_value = None  # 上一次的值
-        self.curr_value = None  # 当前值
+        self.curr_value = None
         self.changed_count = 0  # 改变次数
         self.rule = rule  # 默认是 curr_value != last_value
 
     def setup(self, **kwargs: typing.Any) -> None:
         super().setup(**kwargs)
         self.immediate = self.converter.bool(self.immediate)
 
     def reset(self):
         super().reset()
         self.last_value = None
         self.curr_value = None
         self.changed_count = 0
 
-    @property
-    def is_changed(self):
+    def check_is_changed(self, curr_value: typing.Any, last_value: typing.Any):
         if self.rule == '':
-            return self.curr_value != self.last_value
+            return curr_value != last_value
         else:
             rule = self.converter.render(self.rule)
             is_changed_value = eval(rule, {
                 **(self.context or { }),
-                'curr_value': self.curr_value,
-                'last_value': self.last_value
+                'curr_value'   : curr_value,
+                'last_value'   : last_value,
+                'changed_count': self.changed_count
             })
             assert isinstance(is_changed_value, bool), 'IsChanged: invalid rule'
             return is_changed_value
 
+    def compute_curr_value(self):
+        if isinstance(self.value, str):
+            return self.converter.render(self.value)
+        else:
+            return self.value
+
     def update(self) -> Status:
-        self.curr_value = self.converter.render(self.value)
+        self.curr_value = self.compute_curr_value()
         if not self.immediate and self.last_value is None:
             # 刚开始不触发
             self.last_value = self.curr_value
 
-        if self.is_changed:
+        is_changed = self.check_is_changed(curr_value=self.curr_value, last_value=self.last_value)
+
+        self.logger.debug(f'{self.last_value} -> {self.curr_value}: {is_changed}')
+
+        self.last_value = self.curr_value
+        if is_changed:
             # 发生了变化
             self.changed_count += 1
-            self.last_value = self.curr_value
             return Status.SUCCESS
         else:
             # 没有发生变化
             return Status.FAILURE
 
     def to_data(self):
         return {
             **super().to_data(),
             "immediate"    : self.immediate,
             "last_value"   : self.last_value,
-            "curr_value"   : self.curr_value,
+            'curr_value'   : self.curr_value,
             'changed_count': self.changed_count,
-            'is_changed'   : self.is_changed
         }
 
 
+class IsEqual(Node, Condition):
+    """
+    检查两个值是否相等，值本身可以从context中拿到
+    """
+
+    def __init__(self, a: str, b: str, **kwargs):
+        super().__init__(**kwargs)
+        self.a = a
+        self.b = b
+
+        self.curr_a = None
+        self.curr_b = None
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'curr_a': self.curr_a,
+            'curr_b': self.curr_b
+        }
+
+    def reset(self):
+        super().reset()
+        self.curr_a = None
+        self.curr_b = None
+
+    def update(self):
+        self.curr_a = self.converter.render(self.a)
+        self.curr_b = self.converter.render(self.b)
+        if self.curr_a == self.curr_b:
+            return Status.SUCCESS
+        else:
+            return Status.FAILURE
+
+
 class Print(Action):
     def __init__(self, msg: str, **kwargs):
         super().__init__(**kwargs)
         self.msg = msg
 
     def update(self) -> Status:
         print(self.converter.render(self.msg))
@@ -347,7 +392,74 @@
 
     def to_data(self):
         return {
             **super().to_data(),
             "msg": self.converter.render(self.msg)
         }
 
+
+class RandomIntValue(Node):
+    """
+    生成随机整数到context里
+
+    随机数范围: [low, high], including both end points.
+    """
+
+    def __init__(self, key: str, high: int | str, low: int | str = 0, **kwargs):
+        super().__init__(**kwargs)
+        self.high = high
+        self.low = low
+        self.key = key
+        self.value = None
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.key = self.converter.render(self.key)
+
+    def update(self) -> Status:
+        low = self.converter.int(self.low)
+        high = self.converter.int(self.high)
+
+        self.value = random.randint(low, high)
+        self.context[self.key] = self.value
+        return Status.SUCCESS
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'key'  : self.key,
+            'value': self.value
+        }
+
+
+class RandomFloatValue(Node):
+    """
+    生成随机浮点数到context里
+
+    随机数范围: [low, high), 不包括high
+    """
+
+    def __init__(self, key: str, high: float | str = 1, low: float | str = 0, **kwargs):
+        super().__init__(**kwargs)
+        self.high = high
+        self.low = low
+        self.key = key
+        self.value = None
+
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.key = self.converter.render(self.key)
+
+    def update(self) -> Status:
+        low = self.converter.float(self.low)
+        high = self.converter.float(self.high)
+
+        self.value = random.random() * (high - low) + low
+        self.context[self.key] = self.value
+        return Status.SUCCESS
+
+    def to_data(self):
+        return {
+            **super().to_data(),
+            'key'  : self.key,
+            'value': self.value
+        }
```

### Comparing `pybts-1.5.0/pybts/rl/base_class.py` & `pybts-1.6.0/pybts/rl/base_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-import numpy as np
-from gymnasium import spaces
-from stable_baselines3.common.on_policy_algorithm import OnPolicyAlgorithm
-from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
-from stable_baselines3.common.utils import (
-    explained_variance, get_schedule_fn, safe_mean, obs_as_tensor,
-    configure_logger
-)
-from stable_baselines3 import PPO
-import typing
-import torch as th
-from pybts.node import Node
-import time
-from collections import deque
-import sys
-import gymnasium as gym
-from abc import ABC, abstractmethod
-from pybts.rl.common import DummyEnv
+from pybts.nodes import Node
 from stable_baselines3.common.policies import ActorCriticPolicy
-from typing import Union
 from pybts.rl.off_policy import *
 from pybts.rl.on_policy import *
+from abc import ABC, abstractmethod
+import gymnasium as gym
+from typing import Union
 
 
 class RLPolicyNode(ABC):
     """强化学习在线策略节点，拿来跟其他的Node多继承用"""
 
     def __init__(self):
         self.rl_collector = None
```

### Comparing `pybts-1.5.0/pybts/rl/nodes.py` & `pybts-1.6.0/pybts/rl/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
-from pybts.node import Status, Success, Node
+from pybts.nodes import Status, Success, Node
 from pybts.decorators.nodes import Decorator
 from collections import defaultdict
 from pybts.rl.off_policy import *
 from pybts.rl.on_policy import *
 from stable_baselines3.common.base_class import BaseAlgorithm
 from stable_baselines3.common.policies import ActorCriticPolicy
+from abc import ABC, abstractmethod
+from typing import Union, Type
+import gymnasium as gym
+from pybts.rl.common import DummyEnv
 
 
 class Reward(Node):
     """
     奖励节点，返回的状态一直是SUCCESS
     当走到这个节点时，会将给定的奖励累计
```

### Comparing `pybts-1.5.0/pybts/rl/off_policy.py` & `pybts-1.6.0/pybts/rl/off_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-import numpy as np
-from gymnasium import spaces
 from stable_baselines3.common.off_policy_algorithm import OffPolicyAlgorithm
 from stable_baselines3.common.utils import (
-    explained_variance, get_schedule_fn, safe_mean, obs_as_tensor,
     configure_logger, TrainFreq
 )
-from stable_baselines3 import SAC
 import typing
 from collections import deque
-import sys
-import gymnasium as gym
-from abc import ABC, abstractmethod
-from pybts.rl.common import DummyEnv
-import sys
 import time
 import warnings
-from copy import deepcopy
-from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
-
+from typing import Optional
 import numpy as np
-from stable_baselines3.common.buffers import DictReplayBuffer, ReplayBuffer
-from stable_baselines3.common.noise import ActionNoise, VectorizedActionNoise
+from stable_baselines3.common.buffers import ReplayBuffer
+from stable_baselines3.common.noise import ActionNoise
 from stable_baselines3.common.type_aliases import (
-    GymEnv, MaybeCallback, RolloutReturn, Schedule, TrainFreq,
-    TrainFrequencyUnit
+    RolloutReturn, TrainFreq,
 )
-from stable_baselines3.common.utils import safe_mean, should_collect_more_steps
+from stable_baselines3.common.utils import should_collect_more_steps
+
 
 def bt_off_policy_setup_learn(
         self: OffPolicyAlgorithm,
         tb_log_name: str = 'run',
         reset_num_timesteps: bool = True,
         total_timesteps: int = 10000,
 ):
@@ -150,8 +139,7 @@
                     action_noise.reset()
 
                 # Log training infos
                 if log_interval is not None and self._episode_num % log_interval == 0:
                     self._dump_logs()
 
     return RolloutReturn(num_collected_steps * env_num_envs, num_collected_episodes, continue_training)
-
```

### Comparing `pybts-1.5.0/pybts/rl/on_policy.py` & `pybts-1.6.0/pybts/rl/on_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import numpy as np
 from gymnasium import spaces
 from stable_baselines3.common.on_policy_algorithm import OnPolicyAlgorithm
 from stable_baselines3.common.utils import (
-    explained_variance, get_schedule_fn, safe_mean, obs_as_tensor,
+    safe_mean, obs_as_tensor,
     configure_logger
 )
-from stable_baselines3 import PPO
 import typing
 import torch as th
-from pybts.node import Node
 import time
 from collections import deque
 import sys
 
 
 def bt_on_policy_setup_learn(
         self: OnPolicyAlgorithm,
```

### Comparing `pybts-1.5.0/pybts/rl/tree.py` & `pybts-1.6.0/pybts/rl/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import typing
 
 from py_trees.trees import BehaviourTree
 
 from pybts.tree import Tree
 import py_trees
-from pybts.node import Node
+from pybts.nodes import Node
 from collections import defaultdict
 
 
 class RLTree(Tree):
     """
     强化学习树
     """
```

### Comparing `pybts-1.5.0/pybts/templates/favicon.ico` & `pybts-1.6.0/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.6.0/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.6.0/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.6.0/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.5.0/pybts/tree.py` & `pybts-1.6.0/pybts/tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typing
 
 import py_trees
 from py_trees import common, visitors
-from pybts.node import Node
+from py_trees.trees import BehaviourTree
+
+from pybts.nodes import Node
 from pybts.builder import Builder
 
 
 class Tree(py_trees.trees.BehaviourTree):
     def __init__(self, root: py_trees.behaviour.Behaviour, name: str = '', context: dict = None):
         super().__init__(root=root)
         self.name = name or root.name
@@ -15,38 +17,54 @@
         ] = []
 
         self.context = {
             'round': 0,
             **(context or { }),
         }  # 环境字典
 
+        self._has_setup = False
+
     @property
     def round(self):
         """第几轮"""
         return self.context['round']
 
     @round.setter
     def round(self, value):
         self.context['round'] = value
 
     def setup(
             self,
             timeout: typing.Union[float, common.Duration] = common.Duration.INFINITE,
             visitor: typing.Optional[visitors.VisitorBase] = None,
-            builder: typing.Optional[Builder] = None,
             **kwargs: any,
-    ) -> None:
+    ) -> 'Tree':
+        assert not self._has_setup, f'Tree {self.name} already has setup'
+        self._has_setup = True
         for node in self.root.iterate():
             node.context = self.context
-        super().setup(timeout=timeout, visitor=visitor, builder=builder, **kwargs)
+        super().setup(timeout=timeout, visitor=visitor, **kwargs)
+        return self
 
     def reset(self):
         self.count = 0
         self.round += 1
         for node in self.root.iterate():
             if isinstance(node, Node):
                 node.reset()
         for handler in self.reset_handlers:
             handler(self)
 
     def add_reset_handler(self, handler: typing.Callable[["Tree"], None]):
         self.reset_handlers.append(handler)
+
+    def tick(
+            self: 'Tree',
+            pre_tick_handler: typing.Optional[
+                typing.Callable[['Tree'], None]
+            ] = None,
+            post_tick_handler: typing.Optional[
+                typing.Callable[['Tree'], None]
+            ] = None,
+    ) -> None:
+        assert self._has_setup, f'Tree {self.name} has not been setup'
+        super().tick(pre_tick_handler=pre_tick_handler, post_tick_handler=post_tick_handler)
```

### Comparing `pybts-1.5.0/pybts/utility.py` & `pybts-1.6.0/pybts/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import py_trees.blackboard
 
-from pybts.node import *
+from pybts.nodes import *
 from pybts.constants import *
 import yaml
 from queue import Queue
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 import os
 import json
```

### Comparing `pybts-1.5.0/pyproject.toml` & `pybts-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.5.0"
+version = "1.6.0"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.5.0/PKG-INFO` & `pybts-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.5.0
+Version: 1.6.0
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

