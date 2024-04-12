# Comparing `tmp/scicom-0.2.1.tar.gz` & `tmp/scicom-0.2.5.tar.gz`

## Comparing `scicom-0.2.1.tar` & `scicom-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scicom-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 scicom-0.2.1/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scicom-0.2.1/requirements_dev.txt
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 scicom-0.2.1/setup.cfg
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 scicom-0.2.1/tox.ini
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/authors.rst
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/conf.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/historicalletters.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/index.rst
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/knowledgespread.rst
--rw-r--r--   0        0        0   272329 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/letterModel.png
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/license.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/make.bat
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/randomletters.rst
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/randomlettersDoc.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/readme.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/requirements.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/usingmesa.rst
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/_static/bmbf.png
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/_static/logo.png
--rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.2.1/docs/_static/mpiwg.png
--rw-r--r--   0        0        0    50988 2020-02-02 00:00:00.000000 scicom-0.2.1/examples/RunModel.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/run.py
--rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/data/relPop_plosOne.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/__init__.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/agents.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/model.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/server.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/space.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/historicalletters/utils.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/SimpleContinuousModule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/__init__.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/agents.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/app.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/model.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/server.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/simple_continuous_canvas.js
--rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/knowledgespread/utils.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/SimpleContinuousModule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/__init__.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/agents.py
--rw-r--r--   0        0        0   182427 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/map.png
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/model.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/server.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/randomletters/simple_continuous_canvas.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/utilities/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scicom-0.2.1/src/scicom/utilities/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scicom-0.2.1/.gitignore
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.2.1/AUTHORS.rst
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 scicom-0.2.1/README.md
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 scicom-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 scicom-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 scicom-0.2.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 scicom-0.2.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.5/MANIFEST.in
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scicom-0.2.5/tox.ini
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/authors.rst
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/conf.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/historicalletters.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/index.rst
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/knowledgespread.rst
+-rw-r--r--   0        0        0   272329 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/letterModel.png
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/license.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/make.bat
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/randomletters.rst
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/randomlettersDoc.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/readme.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/requirements.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/usingmesa.rst
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/bmbf.png
+-rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/logo.png
+-rw-r--r--   0        0        0    37002 2020-02-02 00:00:00.000000 scicom-0.2.5/docs/_static/mpiwg.png
+-rw-r--r--   0        0        0    50988 2020-02-02 00:00:00.000000 scicom-0.2.5/examples/RunModel.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/run.py
+-rw-r--r--   0        0        0   389859 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/NUTS_RG_60M_2021_3857_LEVL_2.geojson
+-rw-r--r--   0        0        0   327135 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson
+-rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/pone.0162678.s003.csv
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/data/relPop_plosOne.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/__init__.py
+-rw-r--r--   0        0        0    11281 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/agents.py
+-rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/model.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/server.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/space.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/historicalletters/utils.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/SimpleContinuousModule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/__init__.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/agents.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/app.py
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/model.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/server.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/simple_continuous_canvas.js
+-rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/knowledgespread/utils.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/SimpleContinuousModule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/__init__.py
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/agents.py
+-rw-r--r--   0        0        0   182427 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/map.png
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/model.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/server.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/randomletters/simple_continuous_canvas.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/utilities/__init__.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scicom-0.2.5/src/scicom/utilities/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scicom-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 scicom-0.2.5/tests/test_historicalletters.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 scicom-0.2.5/.gitignore
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scicom-0.2.5/AUTHORS.rst
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scicom-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 scicom-0.2.5/README.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 scicom-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 scicom-0.2.5/PKG-INFO
```

### Comparing `scicom-0.2.1/.gitlab-ci.yml` & `scicom-0.2.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/tox.ini` & `scicom-0.2.5/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py310
+envlist = py311, p310
 isolated_build = true
 
 [pytest]
 minversion = 6.0
 addopts = -ra -q
 testpaths =
     tests
```

### Comparing `scicom-0.2.1/docs/Makefile` & `scicom-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/conf.py` & `scicom-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/index.rst` & `scicom-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/letterModel.png` & `scicom-0.2.5/docs/letterModel.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/make.bat` & `scicom-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/randomlettersDoc.rst` & `scicom-0.2.5/docs/randomlettersDoc.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/usingmesa.rst` & `scicom-0.2.5/docs/usingmesa.rst`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/_static/bmbf.png` & `scicom-0.2.5/docs/_static/bmbf.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/_static/logo.png` & `scicom-0.2.5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/docs/_static/mpiwg.png` & `scicom-0.2.5/docs/_static/mpiwg.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/examples/RunModel.ipynb` & `scicom-0.2.5/examples/RunModel.ipynb`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/run.py` & `scicom-0.2.5/src/scicom/run.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson` & `scicom-0.2.5/src/scicom/data/nuts_rg_60M_2013_lvl_2.geojson`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/data/relPop_plosOne.csv` & `scicom-0.2.5/src/scicom/data/relPop_plosOne.csv`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/historicalletters/model.py` & `scicom-0.2.5/src/scicom/historicalletters/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 import random
 from pathlib import Path
-from statistics import mean
+#from statistics import mean
 from tqdm import tqdm
+from numpy import mean
 
 import mesa
 import networkx as nx
 import mesa_geo as mg
+from shapely import contains
 
 from scicom.utilities.statistics import prune
 from scicom.historicalletters.utils import createData
 
 from scicom.historicalletters.agents import SenderAgent, RegionAgent
 from scicom.historicalletters.space import Nuts2Eu
 
@@ -19,15 +21,15 @@
     """Model reporter for simulation of archiving.
     
     Returns statistics of ledger network of model run
     and various iterations of statistics of pruned networks. 
     """
     # TODO: Add all model params
     if model.runPruning is True:
-        ledgerColumns= ['sender', 'receiver', 'sender_location', 'receiver_location', 'topic', 'step']
+        ledgerColumns = ['sender', 'receiver', 'sender_location', 'receiver_location', 'topic', 'step']
         modelparams = {
             "population": model.population,
             "moveRange": model.moveRange,
             "letterRange": model.letterRange,
             "useActivation": model.useActivation,
             "useSocialNetwork": model.useSocialNetwork,
         }
@@ -36,14 +38,26 @@
             network=model.letterLedger,
             columns=ledgerColumns
         )
     else:
         result = model.letterLedger
     return result
 
+def getComponents(model):
+    """Model reporter to get number of components.
+    
+    The MultiDiGraph is converted to undirected, 
+    considering only edges that are reciprocal, ie.
+    edges are established if sender and receiver have 
+    exchanged at least a letter in each direction.
+    """
+    newG = model.G.to_undirected(reciprocal=True)
+    comp = nx.number_connected_components(newG)
+    return comp
+
 
 class HistoricalLetters(mesa.Model):
     """A letter sending model with historical informed initital positions.
     
     Each agent has an initial topic vector, expressed as a RGB value. The 
     initial positions of the agents is based on a weighted random draw
     based on data from [1]
@@ -54,88 +68,99 @@
     the sender is updated as a random rotation towards the receivers topic.
 
     [1] J. Lobo et al, Population-Area Relationship for Medieval European Cities,
         PLoS ONE 11(10): e0162678.
     """
     def __init__(
         self,
-        population=100,
-        moveRange=0.5,
-        letterRange=0.5,
-        similarityThreshold=0.5,
-        updateTopic=0.1,
+        population: int = 100,
+        moveRange: float = 0.05,
+        letterRange: float = 0.2,
+        similarityThreshold: float = 0.2,
+        updateTopic: float = 0.1,
         useActivation=False,
         useSocialNetwork=False,
         longRangeNetworkFactor=0.3,
         shortRangeNetworkFactor=0.8,
         runPruning=False,
-        datafolder: str = Path(__file__).parent.parent.resolve(),
+        regionData: str = Path(Path(__file__).parent.parent.resolve(), "data/NUTS_RG_60M_2021_3857_LEVL_2.geojson"),
+        populationDistributionData: str = Path(Path(__file__).parent.parent.resolve(), "data/pone.0162678.s003.csv"),
         tempfolder: str = "./",
         debug=False
     ):
         super().__init__()
 
-        self.schedule = mesa.time.RandomActivation(self)
-        self.space = Nuts2Eu()
+        # Control variables
         self.population = population
-        self.letterLedger = []
+        self.moveRange = moveRange
+        self.letterRange = letterRange
+        self.useActivation = useActivation
         # Initialize social network
         self.useSocialNetwork = useSocialNetwork
-        self.G = nx.DiGraph()
+        self.G = nx.MultiDiGraph()
         self.longRangeNetworkFactor = longRangeNetworkFactor
         self.shortRangeNetworkFactor = shortRangeNetworkFactor
-        # 
-        self.moveRange = moveRange
-        self.letterRange = letterRange
-        self.useActivation = useActivation
+        # Collected output variables
+        self.letterLedger = []
         self.runPruning = runPruning
         self.movements = 0
         self.updatedTopic = 0
+        # Internal variables
+        self.schedule = mesa.time.RandomActivation(self)
+        self.scaleSendInput = {}
+        self.updatedTopicsDict = {}
+        self.space = Nuts2Eu()
         self.personRegionMap = {}
-        self.datafolder = datafolder
         self.tempfolder = tempfolder
         self.debug = debug
 
-        initSenderFile, _, _ = createData(
+        initSenderGeoDf = createData(
             population,
-            outputfolder=self.tempfolder,
-            datafolder=self.datafolder
+            populationDistribution=populationDistributionData
         )
 
+        # Calculate mean of mean distances for each agent. 
+        # This is used as a measure for the range of exchanges.
+        distances = []
+        for idx, row in initSenderGeoDf.iterrows():
+            p1 = row['geometry']
+            distances.append(
+                initSenderGeoDf.geometry.apply(lambda x: p1.distance(x)).mean()
+            )
+        self.meandistance = mean(distances)
+
         self.factors = dict(
             updateTopic=updateTopic,
             similarityThreshold=similarityThreshold,
             moveRange=moveRange,
             letterRange=letterRange,
         )
 
         # Set up the grid with patches for every NUTS region
         ac = mg.AgentCreator(RegionAgent, model=self)
         self.regions = ac.from_file(
-            Path(self.datafolder, "data/nuts_rg_60M_2013_lvl_2.geojson"),
+            regionData,
             unique_id="NUTS_ID"
         )
         self.space.add_regions(self.regions)
 
         # Set up agent creator for senders
         ac_senders = mg.AgentCreator(
             SenderAgent,
             model=self,
             agent_kwargs=self.factors
         )
 
         # Create agents based on random coordinates generated 
         # in the createData step above, see util.py file.
-        senders = ac_senders.from_file(
-            initSenderFile,
+        senders = ac_senders.from_GeoDataFrame(
+            initSenderGeoDf,
             unique_id="unique_id"
         )
 
-        Path.unlink(initSenderFile)
-
         # Create random set of initial topic vectors.
         topics = [
             tuple(
                 [random.random() for x in range(3)]
             ) for x in range(self.population)
         ]
 
@@ -144,80 +169,93 @@
         for idx, sender in enumerate(senders):
             self.G.add_node(
                 sender.unique_id,
                 numLettersSend=0,
                 numLettersReceived=0    
             )
             sender.topicVec = topics[idx]
+            # Add current topic to dict
+            self.updatedTopicsDict.update(
+                {sender.unique_id: topics[idx]}
+            )
             if useActivation is True:
                 sender.activationWeight = random.random()
 
         for agent in senders:
-            self.space.add_sender(agent)
+            regionID = [
+                x.unique_id for x in self.regions if contains(x.geometry, agent.geometry)
+            ]
+            try:
+                self.space.add_sender(agent, regionID[0])
+            except IndexError:
+                raise IndexError(f"Problem finding region for {agent.geometry}.")
             self.schedule.add(agent)
 
         # Add graph to network grid for potential visualization.
+        # TODO: Not yet implemented. Maybe use Solara backend for this? 
         self.grid = mesa.space.NetworkGrid(self.G)
 
-        # Calculate mean of mean distances for each agent. 
-        # This is used as a measure for the range of exchanges.
-        borderAgent = self.population - 1
-        agentsp = self.space.get_agents_as_GeoDataFrame()[-borderAgent:]
-        distances = []
-        for source in agentsp.geometry.values:
-            agentdistances = [source.distance(x) for x in agentsp.geometry.values]
-            meanDist = mean(agentdistances)
-            distances.append(meanDist)
-        self.meandistance = mean(distances)
-
         # Create social network
         if useSocialNetwork is True:
             for agent in self.schedule.agents:
                 if isinstance(agent, SenderAgent):
                     self._createSocialEdges(agent, self.G)
 
         # TODO: What comparitive values are useful for visualizations?
         self.datacollector = mesa.DataCollector(
             model_reporters={
-                "Ledger": getPrunedLedger
+                "Ledger": getPrunedLedger,
+                "Letters": lambda x: len(self.letterLedger),
+                "Movements": lambda x: self.movements,
+                "Clusters": getComponents
             },
         )
 
     def _createSocialEdges(self, agent, graph):
+        """Create social edges with the different wiring factors.
+
+        Define a close range by using the moveRange parameter. Among
+        these neighbors, create a connection with probability set by
+        the shortRangeNetworkFactor. 
+
+        For all other agents, that are not in this closeRange group,
+        create a connection with the probability set by the longRangeNetworkFactor.
+        """
         closerange = [x for x in self.space.get_neighbors_within_distance(
             agent,
             distance=self.moveRange * self.meandistance,
             center=False
         ) if isinstance(x, SenderAgent)]
         for neighbor in closerange:
             if neighbor.unique_id != agent.unique_id:
                 connect = random.choices(
                     population=[True, False],
                     weights=[self.shortRangeNetworkFactor, 1 - self.shortRangeNetworkFactor],
                     k=1
                 )
                 if connect[0] is True:
-                    graph.add_edge(agent.unique_id, neighbor.unique_id)
-                    graph.add_edge(neighbor.unique_id, agent.unique_id)
+                    graph.add_edge(agent.unique_id, neighbor.unique_id, step=0)
+                    graph.add_edge(neighbor.unique_id, agent.unique_id, step=0)
         longrange = [x for x in self.schedule.agents if x not in closerange and isinstance(x, SenderAgent)]
         for neighbor in longrange:
             if neighbor.unique_id != agent.unique_id:
                 connect = random.choices(
                     population=[True, False],
                     weights=[self.longRangeNetworkFactor, 1 - self.longRangeNetworkFactor],
                     k=1
                 )
                 if connect[0] is True:
-                    graph.add_edge(agent.unique_id, neighbor.unique_id)
-                    graph.add_edge(neighbor.unique_id, agent.unique_id)
+                    graph.add_edge(agent.unique_id, neighbor.unique_id, step=0)
+                    graph.add_edge(neighbor.unique_id, agent.unique_id, step=0)
 
     def step(self):
+        self.scaleSendInput.update(
+            **{x.unique_id: x.numLettersReceived for x in self.schedule.agents}
+        )
         self.schedule.step()
-        #if self.useSocialNetwork is True:
-        #    nx.spring_layout(self.G)
         self.datacollector.collect(self)
 
     def run(self, n):
         """Run the model for n steps."""
         if self.debug is True:
             for _ in tqdm(range(n)):
                 self.step()
```

### Comparing `scicom-0.2.1/src/scicom/historicalletters/server.py` & `scicom-0.2.5/src/scicom/historicalletters/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,47 +4,42 @@
 import mesa_geo as mg
 from mesa.visualization.modules import ChartVisualization
 
 from scicom.historicalletters.agents import SenderAgent, RegionAgent
 from scicom.historicalletters.model import HistoricalLetters
 
 model_params = {
-    "population": 100,
-    # "population": mesa.visualization.Slider(
-    #     "Number of persons",
-    #     100, 10, 200, 10,
-    #     description="Choose how many persons to include in the model.",
-    # ),
+    #"population": 100,
+    "population": mesa.visualization.Slider(
+         "Number of persons",
+         50, 10, 100, 10,
+         description="Choose how many senders to include in the model.",
+     ),
     "useSocialNetwork": mesa.visualization.Checkbox(
         "Create initial social network of agents",
         False
     ),
     "useActivation": mesa.visualization.Checkbox(
         "Use heterogenous activations",
         False
     ),
-    "updateTopic": mesa.visualization.Slider(
-        "Strength of adoption",
-        0.05, 0.01, 0.3, 0.05,
-        description="Choose how strongly letter sending changes ones topics.",
-    ),
     "similarityThreshold": mesa.visualization.Slider(
         "Similarity threshold",
         0.5, 0.0, 1.0, 0.1,
-        description="Choose how similar two persons topics have to be, to send a letter.",
+        description="Choose how similar two agents topics have to be, to send a letter.",
     ),
     "moveRange": mesa.visualization.Slider(
         "Range for moving position</br>(% of mean agent distances)",
-        0.5, 0.0, 1.0, 0.1,
+        0.1, 0.05, 0.75, 0.05,
         description="Choose the visibility range for finding potential locations to move to.",
     ),
     "letterRange": mesa.visualization.Slider(
         "Range for letter sending</br>(% of mean agent distances)",
-        0.5, 0.0, 1.0, 0.1,
-        description="Choose the visibility range for finding potential receipients.",
+        0.2, 0.1,1.0, 0.1,
+        description="Choose the visibility range for finding potential recipients.",
     ),
 }
 
 
 def topic_draw(agent):
     portrayal = {}
     if isinstance(agent, RegionAgent):
@@ -63,22 +58,23 @@
     return portrayal
 
 
 map_element = mg.visualization.MapModule(
     portrayal_method=topic_draw,
     view=[52, 12],
     zoom=4,
-    map_width=500,
-    map_height=300,
+    map_width=700,
+    map_height=500,
 )
 
 chart = ChartVisualization.ChartModule(
     [
-        {"Label": "Movements", "Color": "tab:red"},
-        {"Label": "Graph components", "Color": "black"}
+        {"Label": "Movements", "Color": "red"},
+        {"Label": "Clusters", "Color": "black"},
+        {'Label': "Letters", "Color": "green"}
     ],
     data_collector_name='datacollector',
 )
 
 
 server = mesa.visualization.ModularServer(
     HistoricalLetters,
```

### Comparing `scicom-0.2.1/src/scicom/historicalletters/space.py` & `scicom-0.2.5/src/scicom/historicalletters/space.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,70 +6,47 @@
 import mesa_geo as mg
 from shapely.geometry import Point
 
 from scicom.historicalletters.agents import RegionAgent, SenderAgent
 
 
 class Nuts2Eu(mg.GeoSpace):
+    """Define regions containing senders of letters.
+    
+    This is modified from a mesa-geo example, here
+    https://github.com/projectmesa/mesa-examples/blob/main/gis/geo_schelling_points/geo_schelling_points/space.py
+    """
     _id_region_map: Dict[str, RegionAgent]
-    _senders_pos_map: DefaultDict[mesa.space.FloatCoordinate, Set[SenderAgent]]
-    _sender_id_map: Dict[int, SenderAgent]
-    num_people: int
 
     def __init__(self):
-        super().__init__(warn_crs_conversion=False)
+        super().__init__(warn_crs_conversion=True)
         self._id_region_map = {}
-        self._senders_pos_map = defaultdict(set)
-        self._sender_id_map = dict()
-        self.num_people = 0
 
     def add_regions(self, agents):
         super().add_agents(agents)
         total_area = 0
         for agent in agents:
             self._id_region_map[agent.unique_id] = agent
-            total_area += agent.SHAPE_AREA
-        for _, agent in self._id_region_map.items():
-            agent.SHAPE_AREA = agent.SHAPE_AREA / total_area * 100.0
-
-    def add_person_to_region(self, person, region_id):
-        person.region_id = region_id
-        self._id_region_map[region_id].add_person(person)
-        self.num_people += 1
-
-    def remove_person_from_region(self, person):
-        self._id_region_map[person.region_id].remove_person(person)
-        person.region_id = None
-        self.num_people -= 1
 
-    def add_sender(self, agent: SenderAgent) -> None:
+    def add_sender_to_region(self, agent, region_id):
+        agent.region_id = region_id
+        self._id_region_map[region_id].add_sender(agent)
+
+    def remove_sender_from_region(self, agent):
+        self._id_region_map[agent.region_id].remove_sender(agent)
+        agent.region_id = None
+
+    def add_sender(self, agent: SenderAgent, regionID: str) -> None:
         super().add_agents([agent])
-        localregion = [x for x in self._id_region_map.values() if x.geometry.contains(agent.geometry)]
-        # FIXME: Some new geometries are not contained in the nuts regions. 
-        try:
-            next_region = localregion[0].unique_id
-        except:
-            next_region = self.get_random_region_id()
-        self.add_person_to_region(agent, next_region)
-        self._senders_pos_map[(agent.geometry.x, agent.geometry.y)].add(agent)
-        self._sender_id_map[agent.unique_id] = agent
+        self.add_sender_to_region(agent, regionID)
         
     def move_sender(
-        self, agent: SenderAgent, pos: mesa.space.FloatCoordinate
+        self, agent: SenderAgent, pos: mesa.space.FloatCoordinate, regionID: str
     ) -> None:
         self.__remove_sender(agent)
         agent.geometry = pos
-        self.add_sender(agent)
+        self.add_sender(agent, regionID)
 
     def __remove_sender(self, agent: SenderAgent) -> None:
         super().remove_agent(agent)
-        del self._sender_id_map[agent.unique_id]
-        self.remove_person_from_region(agent)
-        self._senders_pos_map[(agent.geometry.x, agent.geometry.y)].remove(
-            agent
-        )
-
-    def get_random_region_id(self) -> str:
-        return random.choice(list(self._id_region_map.keys()))
+        self.remove_sender_from_region(agent)
 
-    def get_region_by_id(self, region_id) -> RegionAgent:
-        return self._id_region_map.get(region_id)
```

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/SimpleContinuousModule.py` & `scicom-0.2.5/src/scicom/knowledgespread/SimpleContinuousModule.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/agents.py` & `scicom-0.2.5/src/scicom/knowledgespread/agents.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/app.py` & `scicom-0.2.5/src/scicom/knowledgespread/app.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/model.py` & `scicom-0.2.5/src/scicom/knowledgespread/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         edges = self._setupSocialSpace()
         self.socialNetwork = nx.from_pandas_edgelist(
             edges,
             source='from_id',
             target='to_id',
             edge_attr=["time", "dist"]
         )
-        self.grid = mesa.space.MultiGrid(100, 100, torus=False) 
+        # TODO: What is the effect of the GRID dimensions on social dynamics?
+        self.grid = mesa.space.MultiGrid(1000, 1000, torus=False) 
 
         # Add agents to epistemic space and schedule.
         for agent in agents:
             self.space.place_agent(
                 agent, pos=agent.pos
             )
             x = self.random.randrange(self.grid.width)
```

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/server.py` & `scicom-0.2.5/src/scicom/knowledgespread/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/simple_continuous_canvas.js` & `scicom-0.2.5/src/scicom/knowledgespread/simple_continuous_canvas.js`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/knowledgespread/utils.py` & `scicom-0.2.5/src/scicom/knowledgespread/utils.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/SimpleContinuousModule.py` & `scicom-0.2.5/src/scicom/randomletters/SimpleContinuousModule.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/agents.py` & `scicom-0.2.5/src/scicom/randomletters/agents.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/map.png` & `scicom-0.2.5/src/scicom/randomletters/map.png`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/model.py` & `scicom-0.2.5/src/scicom/randomletters/model.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/server.py` & `scicom-0.2.5/src/scicom/randomletters/server.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/randomletters/simple_continuous_canvas.js` & `scicom-0.2.5/src/scicom/randomletters/simple_continuous_canvas.js`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/src/scicom/utilities/statistics.py` & `scicom-0.2.5/src/scicom/utilities/statistics.py`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/LICENSE.md` & `scicom-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/README.md` & `scicom-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `scicom-0.2.1/pyproject.toml` & `scicom-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SciCom"
-version = "0.2.1"
+version = "0.2.5"
 authors = [
   { name="Bernardo S. Buarque", email="bernardo.buarque@motu.org.nz"},
   { name="Malte Vogl", email="vogl@gea.mpg.de"}
 ]
 description = "Simulating various aspects of scientific communication via Agent-based models."
 readme = "README.md"
+license = {file = "LICENSE.md"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "mesa >= 2",
   "mesa-geo",
   "shapely >=2",
   "pandas",
+  "geopandas",
   "networkx",
   "numpy",
+  "sympy",
   "semanticlayertools",
-  "convert2geojson",
   "solara",
   "altair",
   "nx_altair"
 ]
 
 [project.urls]
 "Project Homepage" = "https://modelsen.mpiwg-berlin.mpg.de"
```

