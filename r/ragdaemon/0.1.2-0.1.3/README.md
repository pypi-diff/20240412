# Comparing `tmp/ragdaemon-0.1.2.tar.gz` & `tmp/ragdaemon-0.1.3.tar.gz`

## Comparing `ragdaemon-0.1.2.tar` & `ragdaemon-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/app.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/context.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/errors.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/llm.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_context.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_daemon.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_database.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_sample.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/app.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/context.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/errors.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/test_context.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/test_daemon.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/test_database.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/test_sample.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 ragdaemon-0.1.3/PKG-INFO
```

### Comparing `ragdaemon-0.1.2/.github/workflows/run-tests.yml` & `ragdaemon-0.1.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/app.py` & `ragdaemon-0.1.3/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/context.py` & `ragdaemon-0.1.3/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/daemon.py` & `ragdaemon-0.1.3/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/utils.py` & `ragdaemon-0.1.3/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.3/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.1.3/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.3/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.3/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.3/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.3/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.3/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.3/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/database/__init__.py` & `ragdaemon-0.1.3/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/database/chroma_database.py` & `ragdaemon-0.1.3/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/database/database.py` & `ragdaemon-0.1.3/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.3/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.3/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.3/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/js/main.js` & `ragdaemon-0.1.3/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.3/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.3/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.3/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/ragdaemon/templates/index.html` & `ragdaemon-0.1.3/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/conftest.py` & `ragdaemon-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/test_context.py` & `ragdaemon-0.1.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/test_daemon.py` & `ragdaemon-0.1.3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/test_sample.py` & `ragdaemon-0.1.3/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/annotators/test_chunker.py` & `ragdaemon-0.1.3/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/annotators/test_diff.py` & `ragdaemon-0.1.3/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.3/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.3/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/data/chunker_graph.json` & `ragdaemon-0.1.3/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/data/context_message.txt` & `ragdaemon-0.1.3/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/data/diff_graph.json` & `ragdaemon-0.1.3/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.3/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.3/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/tests/sample/src/interface.py` & `ragdaemon-0.1.3/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/LICENSE` & `ragdaemon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/README.md` & `ragdaemon-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.2/pyproject.toml` & `ragdaemon-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.2"
+version = "0.1.3"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
-    "spiceai==0.1.8",
+    "spiceai==0.1.9",
     "starlette==0.36.3",
+    "tiktoken==0.6.0",
     "tqdm==4.66.2",
     "uvicorn==0.27.1",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ragdaemon-0.1.2/PKG-INFO` & `ragdaemon-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
-Requires-Dist: spiceai==0.1.8
+Requires-Dist: spiceai==0.1.9
 Requires-Dist: starlette==0.36.3
+Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: uvicorn==0.27.1
 Description-Content-Type: text/markdown
 
 # Ragdaemon
 
 Ragdaemon is a Retrieval-Augmented Generation (RAG) system for code. It runs a daemon (background process) to watch your active code, put it in a knowledge graph, and query the knowledge graph to (among other things) generate context for LLM completions.
```

