# Comparing `tmp/bnlearn-0.8.6.tar.gz` & `tmp/bnlearn-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.8.6.tar", last modified: Tue Apr  9 19:51:11 2024, max compression
+gzip compressed data, was "bnlearn-0.8.7.tar", last modified: Fri Apr 12 20:57:24 2024, max compression
```

## Comparing `bnlearn-0.8.6.tar` & `bnlearn-0.8.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.528980 bnlearn-0.8.6/
--rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.6/LICENSE
--rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0    12276 2024-04-09 19:51:11.528980 bnlearn-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.479159 bnlearn-0.8.6/bnlearn/
--rw-rw-rw-   0        0        0     4729 2024-04-09 19:32:51.000000 bnlearn-0.8.6/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    72560 2024-04-09 19:32:38.000000 bnlearn-0.8.6/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.512926 bnlearn-0.8.6/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.512926 bnlearn-0.8.6/bnlearn/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/discretize/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.6/bnlearn/discretize/discretize.py
--rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.6/bnlearn/discretize/learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    52338 2024-03-28 11:59:09.000000 bnlearn-0.8.6/bnlearn/examples.py
--rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/examples_discretize.py
--rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/network.py
--rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.6/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.522962 bnlearn-0.8.6/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.522962 bnlearn-0.8.6/bnlearn/tests/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/test_discretize.py
--rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.6/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.510914 bnlearn-0.8.6/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    12276 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      204 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 19:51:11.528980 bnlearn-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     2088 2024-04-09 19:29:59.000000 bnlearn-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.777326 bnlearn-0.8.7/
+-rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    12768 2024-04-12 20:57:24.777326 bnlearn-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.698762 bnlearn-0.8.7/bnlearn/
+-rw-rw-rw-   0        0        0     4729 2024-04-12 20:43:39.000000 bnlearn-0.8.7/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    72952 2024-04-12 20:42:15.000000 bnlearn-0.8.7/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.745638 bnlearn-0.8.7/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.763303 bnlearn-0.8.7/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.7/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.7/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    53337 2024-04-12 20:21:18.000000 bnlearn-0.8.7/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.7/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.763303 bnlearn-0.8.7/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.777326 bnlearn-0.8.7/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.7/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.745638 bnlearn-0.8.7/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12768 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 20:57:24.777326 bnlearn-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2024-04-09 19:29:59.000000 bnlearn-0.8.7/setup.py
```

### Comparing `bnlearn-0.8.6/LICENSE` & `bnlearn-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/MANIFEST.in` & `bnlearn-0.8.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/PKG-INFO` & `bnlearn-0.8.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: bnlearn
-Version: 0.8.6
-Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
-Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.6 Summary: Python package for
-learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
-Library for Bayesian network learning and inference [![Python](https://
-img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+# bnlearn - Library for Bayesian network learning and inference [![Python]
+(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
 (https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
 img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
 img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
 bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
 erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
 Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
```

### Comparing `bnlearn-0.8.6/README.md` & `bnlearn-0.8.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: bnlearn
+Version: 0.8.7
+Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pgmpy>=0.1.18
+Requires-Dist: networkx>=2.7.1
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: numpy>=1.24.1
+Requires-Dist: pandas==1.5.3
+Requires-Dist: tqdm
+Requires-Dist: ismember
+Requires-Dist: scikit-learn
+Requires-Dist: funcsigs
+Requires-Dist: statsmodels
+Requires-Dist: python-louvain
+Requires-Dist: packaging
+Requires-Dist: df2onehot
+Requires-Dist: fsspec
+Requires-Dist: pypickle
+Requires-Dist: tabulate
+Requires-Dist: ipywidgets
+Requires-Dist: datazets
+
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,17 +1,31 @@
-# bnlearn - Library for Bayesian network learning and inference [![Python]
-(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
-pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
-(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
-img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
-img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
-bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
-erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
-Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
-github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.7 Summary: Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist: tqdm
+Requires-Dist: ismember Requires-Dist: scikit-learn Requires-Dist: funcsigs
+Requires-Dist: statsmodels Requires-Dist: python-louvain Requires-Dist:
+packaging Requires-Dist: df2onehot Requires-Dist: fsspec Requires-Dist:
+pypickle Requires-Dist: tabulate Requires-Dist: ipywidgets Requires-Dist:
+datazets # bnlearn - Library for Bayesian network learning and inference [!
+[Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
+img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
+(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.6/bnlearn/__init__.py` & `bnlearn-0.8.7/bnlearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.8.6'
+__version__ = '0.8.7'
 
 import pgmpy
 # Check version pgmpy
 if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
     raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
```

### Comparing `bnlearn-0.8.6/bnlearn/bnlearn.py` & `bnlearn-0.8.7/bnlearn/bnlearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -960,15 +960,15 @@
          interactive=False,
          title='bnlearn Directed Acyclic Graph (DAG)',
          node_color=None,
          node_size=None,
          node_properties=None,
          edge_properties=None,
          params_interactive={'minmax_distance': [100, 250], 'figsize': (1500, 800), 'notebook': False, 'font_color': 'node_color', 'bgcolor': '#ffffff', 'show_slider': True, 'filepath': None},
-         params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spring_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True},
+         params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spectral_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True},
          verbose=3):
     """Plot the learned stucture.
 
     Parameters
     ----------
     model : dict
         Learned model from the .fit() function.
@@ -1046,15 +1046,15 @@
     if model['adjmat'].sum().sum()==0:
         if verbose>=3: print('[bnlearn]> Nothing to plot because no edges are present between nodes. ')
         return None
 
     # Plot properties
     defaults = {'minmax_distance': [100, 250], 'figsize': (1500, 800), 'notebook': False, 'font_color': 'node_color', 'bgcolor': '#ffffff', 'directed': True, 'show_slider': True, 'filepath': None}
     params_interactive = {**defaults, **params_interactive}
-    defaults = {'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'height': None, 'width': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'layout': 'spring_layout', 'font_color': 'k', 'facecolor': '#ffffff', 'node_shape': 'o', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True}
+    defaults = {'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'height': None, 'width': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'layout': 'spectral_layout', 'font_color': 'k', 'facecolor': '#ffffff', 'node_shape': 'o', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True}
     params_static = {**defaults, **params_static}
 
     # DEPRECATED IN LATER VERSION
     if (params_static.get('width') is not None) or (params_static.get('height') is not None):
         # if verbose>=2: print('[bnlearn]> Warning: [height] and [width] will be removed in further version. Please use: params_static={"figsize": (15, 10)}.')
         params_static['figsize'] = (15 if params_static['width'] is None else params_static['width'], 10 if params_static['height'] is None else params_static['height'])
 
@@ -1071,14 +1071,23 @@
         edge_properties = bnlearn.get_edge_properties(model, minscale=params_static['minscale'], maxscale=params_static['maxscale'])
 
     # Set default node size based on interactive True/False
     for key in node_properties.keys():
         if node_properties[key]['node_size'] is None:
             node_properties[key]['node_size']=node_size_default
 
+    # Add edges with weights based on independence test results
+    for edge, properties in edge_properties.items():
+        strength = properties.get("weight", 0)
+        G.add_edge(*edge, weight = strength)
+
+    # Update the dataframe with the weights
+    for (source, target), value in edge_properties.items():
+        model['adjmat'].loc[source, target] = value['weight']
+
     # Extract model if in dict
     if 'dict' in str(type(model)):
         bnmodel = model.get('model', None)
     else:
         bnmodel = model.copy()
 
     # get node properties
@@ -1106,15 +1115,15 @@
                                 tooltip,
                                 verbose=verbose)
     else:
         # Bayesian model
         if ('bayes' in str(type(bnmodel)).lower()) or ('pgmpy' in str(type(bnmodel)).lower()):
             if verbose>=3: print('[bnlearn] >Plot based on Bayesian model')
             # positions for all nodes
-            G = nx.DiGraph(model['adjmat'])
+            # G = nx.DiGraph(model['adjmat'])
             pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
         elif 'networkx' in str(type(bnmodel)):
             if verbose>=3: print('[bnlearn] >Plot based on networkx model')
             G = bnmodel
             pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
         else:
             if verbose>=3: print('[bnlearn] >Plot based on adjacency matrix')
```

### Comparing `bnlearn-0.8.6/bnlearn/confmatrix.py` & `bnlearn-0.8.7/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/discretize/discretize.py` & `bnlearn-0.8.7/bnlearn/discretize/discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/discretize/learn_discrete_bayes_net.py` & `bnlearn-0.8.7/bnlearn/discretize/learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/examples.py` & `bnlearn-0.8.7/bnlearn/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+# %% issue #93
+
+import bnlearn as bn
+
+# Load example mixed dataset
+df = bn.import_example(data='titanic')
+
+# Convert to onehot
+dfhot, dfnum = bn.df2onehot(df)
+
+# Structure learning
+# model = bn.structure_learning.fit(dfnum, methodtype='cl', black_list=['Embarked','Parch','Name'], root_node='Survived', bw_list_method='nodes')
+model = bn.structure_learning.fit(dfnum)
+# Plot
+G = bn.plot(model, interactive=False)
+
+# Compute edge strength with the chi_square test statistic
+model = bn.independence_test(model, dfnum, test='chi_square', prune=True)
+
+# Plot
+bn.plot(model, interactive=False, pos=G['pos'], params_static={'layout': 'spectral_layout'})
+# 'spring_layout', 'planar_layout', 'shell_layout', 'spectral_layout', 'pydot_layout', 'graphviz_layout', 'circular_layout', 'spring_layout', 'random_layout', 'bipartite_layout', 'multipartite_layout',
+# bn.plot(model, interactive=True, pos=G['pos'])
+
+# Parameter learning
+model = bn.parameter_learning.fit(model, dfnum)
+
+
 # %% compute causalities
 import bnlearn as bn
 # Load asia DAG
 df = bn.import_example('asia', verbose=0)
 # print(tabulate(df.head(), tablefmt="grid", headers="keys"))
 # print(df)
```

### Comparing `bnlearn-0.8.6/bnlearn/examples_discretize.py` & `bnlearn-0.8.7/bnlearn/examples_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/inference.py` & `bnlearn-0.8.7/bnlearn/inference.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/network.py` & `bnlearn-0.8.7/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/parameter_learning.py` & `bnlearn-0.8.7/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/structure_learning.py` & `bnlearn-0.8.7/bnlearn/structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/tests/discretize/test_discretize.py` & `bnlearn-0.8.7/bnlearn/tests/discretize/test_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py` & `bnlearn-0.8.7/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.7/bnlearn/tests/test_bnlearn.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.7/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.7/bnlearn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pgmpy>=0.1.18
+Requires-Dist: networkx>=2.7.1
+Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: numpy>=1.24.1
+Requires-Dist: pandas==1.5.3
+Requires-Dist: tqdm
+Requires-Dist: ismember
+Requires-Dist: scikit-learn
+Requires-Dist: funcsigs
+Requires-Dist: statsmodels
+Requires-Dist: python-louvain
+Requires-Dist: packaging
+Requires-Dist: df2onehot
+Requires-Dist: fsspec
+Requires-Dist: pypickle
+Requires-Dist: tabulate
+Requires-Dist: ipywidgets
+Requires-Dist: datazets
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,25 +1,31 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.6 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.7 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz Author:
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
-Library for Bayesian network learning and inference [![Python](https://
-img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
-pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
-(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
-img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
-img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
-bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
-erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
-Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
-github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
+Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist: tqdm
+Requires-Dist: ismember Requires-Dist: scikit-learn Requires-Dist: funcsigs
+Requires-Dist: statsmodels Requires-Dist: python-louvain Requires-Dist:
+packaging Requires-Dist: df2onehot Requires-Dist: fsspec Requires-Dist:
+pypickle Requires-Dist: tabulate Requires-Dist: ipywidgets Requires-Dist:
+datazets # bnlearn - Library for Bayesian network learning and inference [!
+[Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
+img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
+img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
+Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
+(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.6/bnlearn.egg-info/SOURCES.txt` & `bnlearn-0.8.7/bnlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.6/setup.py` & `bnlearn-0.8.7/setup.py`

 * *Files identical despite different names*

