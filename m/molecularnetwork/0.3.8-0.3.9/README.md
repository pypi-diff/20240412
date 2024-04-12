# Comparing `tmp/molecularnetwork-0.3.8.tar.gz` & `tmp/molecularnetwork-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.3.8.tar", last modified: Tue Apr  9 09:17:09 2024, max compression
+gzip compressed data, was "molecularnetwork-0.3.9.tar", last modified: Fri Apr 12 19:10:26 2024, max compression
```

## Comparing `molecularnetwork-0.3.8.tar` & `molecularnetwork-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806924 molecularnetwork-0.3.8/
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.8/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.8/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     4756 2024-04-09 09:17:09.806699 molecularnetwork-0.3.8/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     4333 2024-04-09 09:16:01.000000 molecularnetwork-0.3.8/README.md
--rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.8/banner.png
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.802566 molecularnetwork-0.3.8/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2306 2024-04-09 09:16:19.000000 molecularnetwork-0.3.8/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806402 molecularnetwork-0.3.8/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     4756 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)    94575 2024-04-09 08:17:30.000000 molecularnetwork-0.3.8/net.png
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.8/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-09 09:17:09.806975 molecularnetwork-0.3.8/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-09 09:16:33.000000 molecularnetwork-0.3.8/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806109 molecularnetwork-0.3.8/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.8/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.535608 molecularnetwork-0.3.9/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.9/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.9/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 19:10:26.535405 molecularnetwork-0.3.9/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4344 2024-04-12 12:25:50.000000 molecularnetwork-0.3.9/README.md
+-rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.9/banner.png
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.531990 molecularnetwork-0.3.9/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2857 2024-04-12 19:00:24.000000 molecularnetwork-0.3.9/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.535128 molecularnetwork-0.3.9/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)    28978 2024-04-09 11:48:31.000000 molecularnetwork-0.3.9/net.png
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.9/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-12 19:10:26.535650 molecularnetwork-0.3.9/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-12 13:12:06.000000 molecularnetwork-0.3.9/setup.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.534764 molecularnetwork-0.3.9/test/
+-rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.9/test/test.csv
+-rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/test/test.gpickle
+-rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/test/test.py
```

### Comparing `molecularnetwork-0.3.8/.gitignore` & `molecularnetwork-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/LICENSE` & `molecularnetwork-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/PKG-INFO` & `molecularnetwork-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -53,34 +53,34 @@
 
 # Graph `Node` Attributes
 graph.nodes[0]['fp'] # Returns ECFP4 fingerprint for node 0 ["CCO"].
 graph.nodes[0]['smiles'] # Returns SMILES for node 0 ["CCO"].
 graph.nodes[0]['categorical_label'] # Returns `alcohol`
 
 # Graph `Edge` Attributes
-graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+graph[0][1]['similarity'] # Returns the edge weight attribute which is the similarity between node 0 and 1
 # Returns 0.3333333333333333
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ### Plot Molecular Network
 ```py
-def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='weight'):
+def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='similarity'):
     """
-    Draws a molecular network graph with node colors based on categorical labels and edge widths based on edge weights.
+    Draws a molecular network graph with node colors based on categorical labels and edge widths based on similarity.
 
     Args:
       G: NetworkX graph representing the molecular network.
       node_attribute: Name of the node attribute containing categorical labels (default: 'categorical_label').
-      edge_attribute: Name of the edge attribute containing weights (default: 'weight').
+      edge_attribute: Name of the edge attribute containing similarity (default: 'similarity').
     """
 
     # Extract unique categorical labels
     unique_labels = set(nx.get_node_attributes(G, node_attribute).values())
     num_labels = len(unique_labels)
 
     # Define a colormap
@@ -89,15 +89,15 @@
     # Create a dictionary mapping labels to colors and a list of label names for legend
     color_map = {label: colormap(i) for i, label in enumerate(unique_labels)}
     label_names = list(color_map.keys())
 
     # Extract node colors based on categorical labels
     node_colors = [color_map[G.nodes[n][node_attribute]] for n in G.nodes]
 
-    # Extract edge widths based on edge weights
+    # Extract edge widths based on similarity
     edge_widths = [G[u][v][edge_attribute] for u, v in G.edges]
 
     # Draw the graph
     plt.figure(figsize=(8, 6))
     pos = nx.spring_layout(G, k=0.2)  # you can choose different layout algorithms
 
     # Draw nodes
```

### Comparing `molecularnetwork-0.3.8/README.md` & `molecularnetwork-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,34 +39,34 @@
 
 # Graph `Node` Attributes
 graph.nodes[0]['fp'] # Returns ECFP4 fingerprint for node 0 ["CCO"].
 graph.nodes[0]['smiles'] # Returns SMILES for node 0 ["CCO"].
 graph.nodes[0]['categorical_label'] # Returns `alcohol`
 
 # Graph `Edge` Attributes
-graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+graph[0][1]['similarity'] # Returns the edge weight attribute which is the similarity between node 0 and 1
 # Returns 0.3333333333333333
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ### Plot Molecular Network
 ```py
-def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='weight'):
+def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='similarity'):
     """
-    Draws a molecular network graph with node colors based on categorical labels and edge widths based on edge weights.
+    Draws a molecular network graph with node colors based on categorical labels and edge widths based on similarity.
 
     Args:
       G: NetworkX graph representing the molecular network.
       node_attribute: Name of the node attribute containing categorical labels (default: 'categorical_label').
-      edge_attribute: Name of the edge attribute containing weights (default: 'weight').
+      edge_attribute: Name of the edge attribute containing similarity (default: 'similarity').
     """
 
     # Extract unique categorical labels
     unique_labels = set(nx.get_node_attributes(G, node_attribute).values())
     num_labels = len(unique_labels)
 
     # Define a colormap
@@ -75,15 +75,15 @@
     # Create a dictionary mapping labels to colors and a list of label names for legend
     color_map = {label: colormap(i) for i, label in enumerate(unique_labels)}
     label_names = list(color_map.keys())
 
     # Extract node colors based on categorical labels
     node_colors = [color_map[G.nodes[n][node_attribute]] for n in G.nodes]
 
-    # Extract edge widths based on edge weights
+    # Extract edge widths based on similarity
     edge_widths = [G[u][v][edge_attribute] for u, v in G.edges]
 
     # Draw the graph
     plt.figure(figsize=(8, 6))
     pos = nx.spring_layout(G, k=0.2)  # you can choose different layout algorithms
 
     # Draw nodes
```

### Comparing `molecularnetwork-0.3.8/banner.png` & `molecularnetwork-0.3.9/banner.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/molecularnetwork/featurizer.py` & `molecularnetwork-0.3.9/molecularnetwork/featurizer.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/molecularnetwork/graph.py` & `molecularnetwork-0.3.9/molecularnetwork/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,56 +4,64 @@
 import numpy as np
 from joblib import dump, load
 from .featurizer import FingerprintCalculator
 from .similarity import SimilarityCalculator
 
 
 class MolecularNetwork:
-    def __init__(self, descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.7):
+    def __init__(self, 
+                 descriptor="morgan2", 
+                 sim_metric="tanimoto", 
+                 sim_threshold=0.7,
+                 node_descriptor="morgan2"):
         self.sim_threshold = sim_threshold
         self.fingerprint_calculator = FingerprintCalculator(descriptor)
         self.similarity_calculator = SimilarityCalculator(sim_metric)
         self.graph = networkx.Graph()
+        self.node_fp_calculator = FingerprintCalculator(node_descriptor)
 
     def _create_graph(self, smiles_list, classes):
         if classes is None:
             classes = np.full(len(smiles_list), 0)
-        fps = self._calculate_fingerprints(smiles_list)
-        self._add_nodes(smiles_list, fps, classes)
+        fps = self._calculate_fingerprints(self.fingerprint_calculator, smiles_list)
+        model_fps = self._calculate_fingerprints(self.node_fp_calculator, smiles_list)
+        self._add_nodes(smiles_list, model_fps, classes)
         self._add_edges(fps)
 
-    def _calculate_fingerprints(self, smiles_list):
+    def _calculate_fingerprints(self, fp_calculator, smiles_list):
         return [
-            self.fingerprint_calculator.calculate_fingerprint(smi)
+            fp_calculator.calculate_fingerprint(smi)
             for smi in smiles_list
         ]
 
-    def _add_nodes(self, smiles_list, fps, classes):
+    def _add_nodes(self, smiles_list, model_fps, classes):
         num_nodes = len(smiles_list)
         nodes = range(num_nodes)
         weighted_nodes = [
             (
                 node,
                 {
                     "smiles": smiles_list[node],
                     "categorical_label": str(value),
-                    "fp": np.array(fps[node])
+                    "fp": np.array(model_fps[node])
                 },
             )
             for node, value in zip(nodes, classes)
         ]
         self.graph.add_nodes_from(weighted_nodes)
 
     def _add_edges(self, fps):
         num_nodes = len(fps)
         for i in range(num_nodes):
             for j in range(i + 1, num_nodes):
                 sim_val = self._calculate_similarity(fps[i], fps[j])
                 if sim_val > self.sim_threshold:
-                    self.graph.add_edge(i, j, weight=sim_val)
+                    # Check if nodes are from same class or not (True if nodes are from same class)
+                    same_class = self.graph.nodes[i]['categorical_label'] == self.graph.nodes[j]['categorical_label']
+                    self.graph.add_edge(i, j, similarity=sim_val, same_class=same_class)
 
     def _calculate_similarity(self, fp1, fp2):
         return self.similarity_calculator.calculate_similarity(fp1, fp2)
 
     def create_graph(self, smiles_list, classes=None):
         self._create_graph(smiles_list, classes)
         return self.graph
```

### Comparing `molecularnetwork-0.3.8/molecularnetwork/similarity.py` & `molecularnetwork-0.3.9/molecularnetwork/similarity.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/molecularnetwork.egg-info/PKG-INFO` & `molecularnetwork-0.3.9/molecularnetwork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.8
+Version: 0.3.9
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -53,34 +53,34 @@
 
 # Graph `Node` Attributes
 graph.nodes[0]['fp'] # Returns ECFP4 fingerprint for node 0 ["CCO"].
 graph.nodes[0]['smiles'] # Returns SMILES for node 0 ["CCO"].
 graph.nodes[0]['categorical_label'] # Returns `alcohol`
 
 # Graph `Edge` Attributes
-graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+graph[0][1]['similarity'] # Returns the edge weight attribute which is the similarity between node 0 and 1
 # Returns 0.3333333333333333
 
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
 
 ### Plot Molecular Network
 ```py
-def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='weight'):
+def draw_graph_with_attributes(G, node_attribute='categorical_label', edge_attribute='similarity'):
     """
-    Draws a molecular network graph with node colors based on categorical labels and edge widths based on edge weights.
+    Draws a molecular network graph with node colors based on categorical labels and edge widths based on similarity.
 
     Args:
       G: NetworkX graph representing the molecular network.
       node_attribute: Name of the node attribute containing categorical labels (default: 'categorical_label').
-      edge_attribute: Name of the edge attribute containing weights (default: 'weight').
+      edge_attribute: Name of the edge attribute containing similarity (default: 'similarity').
     """
 
     # Extract unique categorical labels
     unique_labels = set(nx.get_node_attributes(G, node_attribute).values())
     num_labels = len(unique_labels)
 
     # Define a colormap
@@ -89,15 +89,15 @@
     # Create a dictionary mapping labels to colors and a list of label names for legend
     color_map = {label: colormap(i) for i, label in enumerate(unique_labels)}
     label_names = list(color_map.keys())
 
     # Extract node colors based on categorical labels
     node_colors = [color_map[G.nodes[n][node_attribute]] for n in G.nodes]
 
-    # Extract edge widths based on edge weights
+    # Extract edge widths based on similarity
     edge_widths = [G[u][v][edge_attribute] for u, v in G.edges]
 
     # Draw the graph
     plt.figure(figsize=(8, 6))
     pos = nx.spring_layout(G, k=0.2)  # you can choose different layout algorithms
 
     # Draw nodes
```

### Comparing `molecularnetwork-0.3.8/setup.py` & `molecularnetwork-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

### Comparing `molecularnetwork-0.3.8/test/test.csv` & `molecularnetwork-0.3.9/test/test.csv`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.8/test/test.gpickle` & `molecularnetwork-0.3.9/test/test.gpickle`

 * *Files identical despite different names*

