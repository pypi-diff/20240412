# Comparing `tmp/ragdaemon-0.1.4.tar.gz` & `tmp/ragdaemon-0.1.5.tar.gz`

## Comparing `ragdaemon-0.1.4.tar` & `ragdaemon-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/app.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/context.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/errors.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/llm.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/test_context.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/test_daemon.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/test_database.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/test_sample.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/README.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 ragdaemon-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/app.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/context.py
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/errors.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_context.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_daemon.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_database.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_sample.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/README.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/PKG-INFO
```

### Comparing `ragdaemon-0.1.4/.github/workflows/run-tests.yml` & `ragdaemon-0.1.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/app.py` & `ragdaemon-0.1.5/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/context.py` & `ragdaemon-0.1.5/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/daemon.py` & `ragdaemon-0.1.5/ragdaemon/daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,28 +31,32 @@
     def __init__(
         self,
         cwd: Path,
         annotators: Optional[dict[str, dict]] = None,
         verbose: bool = False,
         graph_path: Optional[Path] = None,
         spice_client: Optional[Spice] = None,
+        model: str = DEFAULT_EMBEDDING_MODEL,
+        provider: Optional[str] = None,
     ):
         self.cwd = cwd
         self.verbose = verbose
         if graph_path is not None:
             self.graph_path = (cwd / graph_path).resolve()
         else:
             self.graph_path = self.cwd / ".ragdaemon" / "graph.json"
         self.graph_path.parent.mkdir(exist_ok=True)
         if spice_client is None:
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
                 default_embeddings_model=DEFAULT_EMBEDDING_MODEL,
             )
         self.spice_client = spice_client
+        self.model = model
+        self.provider = provider
 
         # Initialize an empty graph
         self.graph = nx.MultiDiGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
@@ -75,15 +79,20 @@
             print(f"Saved updated graph to {self.graph_path}")
 
     async def update(self, refresh=False):
         """Iteratively build the knowledge graph"""
 
         # Establish a dedicated database client for this instance
         if self.db is None:
-            self.db = get_db(self.cwd, spice_client=self.spice_client)
+            self.db = get_db(
+                self.cwd,
+                spice_client=self.spice_client,
+                model=self.model,
+                provider=self.provider,
+            )
 
         _graph = self.graph.copy()
         self.graph.graph["refreshing"] = True
         for annotator in self.pipeline.values():
             if refresh or not annotator.is_complete(_graph, self.db):
                 _graph = await annotator.annotate(_graph, self.db, refresh=refresh)
         self.graph = _graph
```

### Comparing `ragdaemon-0.1.4/ragdaemon/utils.py` & `ragdaemon-0.1.5/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.5/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.1.5/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.5/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.5/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.5/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.5/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.5/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.5/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/database/chroma_database.py` & `ragdaemon-0.1.5/ragdaemon/database/chroma_database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 from pathlib import Path
-from typing import TYPE_CHECKING
 from timeit import default_timer
+from typing import TYPE_CHECKING, Optional
 
 from spice import Spice
+from spice.spice import Model, Provider
 
 from ragdaemon.database.database import Database
 
 MAX_INPUTS_PER_CALL = 2048
 
 if TYPE_CHECKING:
     from chromadb.api.types import Embeddable, EmbeddingFunction, Embeddings
 
 
 class ChromaDB(Database):
-    def __init__(self, cwd: Path, db_path: Path, spice_client: Spice) -> None:
+    def __init__(
+        self,
+        cwd: Path,
+        db_path: Path,
+        spice_client: Spice,
+        model: str,
+        provider: Optional[str] = None,
+    ) -> None:
         self.cwd = cwd
         self.db_path = db_path
-        self.model = spice_client._default_embeddings_model.name
+        self.model = model
 
         import chromadb  # Imports are slow so do it lazily
         from chromadb.api.types import Embeddable, EmbeddingFunction, Embeddings
 
         class SpiceEmbeddingFunction(EmbeddingFunction[Embeddable]):
             def __call__(self, input_texts: Embeddable) -> Embeddings:
                 if isinstance(input_texts, str):
                     input_texts = [input_texts]
                 # Embed in batches
                 _inputs = input_texts
                 outputs = list[list[float]]()
                 while _inputs:
                     inputs = _inputs[:MAX_INPUTS_PER_CALL]
                     _inputs = _inputs[MAX_INPUTS_PER_CALL:]
-                    embeddings = spice_client.get_embeddings_sync(input_texts=inputs)
+                    embeddings = spice_client.get_embeddings_sync(
+                        input_texts=inputs, model=model, provider=provider
+                    ).embeddings
                     outputs.extend(embeddings)
                 return outputs
 
         embedding_function = SpiceEmbeddingFunction()
 
         _client = chromadb.PersistentClient(path=str(db_path))
         name = f"ragdaemon-{self.cwd.name}-{self.model}"
```

### Comparing `ragdaemon-0.1.4/ragdaemon/database/database.py` & `ragdaemon-0.1.5/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.5/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.5/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.5/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/js/main.js` & `ragdaemon-0.1.5/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.5/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.5/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.5/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/ragdaemon/templates/index.html` & `ragdaemon-0.1.5/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/conftest.py` & `ragdaemon-0.1.5/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import subprocess
 import tempfile
 from pathlib import Path
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
-from ragdaemon.database import get_db
+from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, get_db
 
 
 @pytest.fixture
 def cwd():
     return Path("tests/sample")
 
 
 @pytest.fixture
 def mock_db(cwd):
-    return get_db(cwd, spice_client=AsyncMock())
+    return get_db(cwd, spice_client=AsyncMock(), model=DEFAULT_EMBEDDING_MODEL)
 
 
 @pytest.fixture
 def mock_get_llm_response():
     with patch(
         "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
         return_value={"chunks": []},
```

### Comparing `ragdaemon-0.1.4/tests/test_context.py` & `ragdaemon-0.1.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/test_daemon.py` & `ragdaemon-0.1.5/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/test_sample.py` & `ragdaemon-0.1.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/annotators/test_chunker.py` & `ragdaemon-0.1.5/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/annotators/test_diff.py` & `ragdaemon-0.1.5/tests/annotators/test_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     tests = [
         ("HEAD", "HEAD", "None", None),
         ("DEFAULT:main.py", "DEFAULT", "main.py", None),
         ("HEAD HEAD~1:path/to/file:1-2", "HEAD HEAD~1", "path/to/file", {1, 2}),
     ]
     for id, expected_ref, expected_path, expected_lines in tests:
         actual_ref, actual_path, actual_lines = parse_diff_id(id)
+        actual_path = actual_path.as_posix() if actual_path else "None"
         assert actual_ref == expected_ref
-        assert str(actual_path) == expected_path
+        assert actual_path == expected_path
         assert actual_lines == expected_lines
 
 
 @pytest.mark.asyncio
 async def test_diff_annotate(git_history, mock_db):
     with open("tests/data/chunker_graph.json", "r") as f:
         data = json.load(f)
```

### Comparing `ragdaemon-0.1.4/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.5/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.5/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/data/chunker_graph.json` & `ragdaemon-0.1.5/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/data/context_message.txt` & `ragdaemon-0.1.5/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/data/diff_graph.json` & `ragdaemon-0.1.5/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.5/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.5/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/tests/sample/src/interface.py` & `ragdaemon-0.1.5/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/LICENSE` & `ragdaemon-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/README.md` & `ragdaemon-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.4/pyproject.toml` & `ragdaemon-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.4"
+version = "0.1.5"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
```

### Comparing `ragdaemon-0.1.4/PKG-INFO` & `ragdaemon-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

