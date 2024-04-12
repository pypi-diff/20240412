# Comparing `tmp/tinynarm-0.2.0.tar.gz` & `tmp/tinynarm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinynarm-0.2.0.tar", max compression
+gzip compressed data, was "tinynarm-0.2.1.tar", max compression
```

## Comparing `tinynarm-0.2.0.tar` & `tinynarm-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-09-19 07:51:04.133461 tinynarm-0.2.0/LICENSE
--rw-r--r--   0        0        0     3572 2023-09-19 07:51:04.133461 tinynarm-0.2.0/README.md
--rw-r--r--   0        0        0      645 2023-09-19 07:51:04.136461 tinynarm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      283 2023-09-19 07:51:04.140461 tinynarm-0.2.0/tinynarm/__init__.py
--rw-r--r--   0        0        0      959 2023-09-19 07:51:04.140461 tinynarm-0.2.0/tinynarm/comparison.py
--rw-r--r--   0        0        0     3057 2023-09-19 07:51:04.141461 tinynarm-0.2.0/tinynarm/discretization.py
--rw-r--r--   0        0        0      196 2023-09-19 07:51:04.141461 tinynarm-0.2.0/tinynarm/item.py
--rw-r--r--   0        0        0     2491 2023-09-19 07:51:04.141461 tinynarm-0.2.0/tinynarm/tinynarm.py
--rw-r--r--   0        0        0     2366 2023-09-19 07:51:04.141461 tinynarm-0.2.0/tinynarm/utils.py
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 tinynarm-0.2.0/setup.py
--rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 tinynarm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      624 2024-04-12 15:31:56.450526 tinynarm-0.2.1/CITATION.cff
+-rw-r--r--   0        0        0     1079 2024-04-12 15:31:56.450526 tinynarm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3554 2024-04-12 15:31:56.451526 tinynarm-0.2.1/README.md
+-rw-r--r--   0        0        0      700 2024-04-12 15:31:56.465526 tinynarm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      283 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/__init__.py
+-rw-r--r--   0        0        0      959 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/comparison.py
+-rw-r--r--   0        0        0     3057 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/discretization.py
+-rw-r--r--   0        0        0      196 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/item.py
+-rw-r--r--   0        0        0     2491 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/tinynarm.py
+-rw-r--r--   0        0        0     2366 2024-04-12 15:31:56.474526 tinynarm-0.2.1/tinynarm/utils.py
+-rw-r--r--   0        0        0     4235 1970-01-01 00:00:00.000000 tinynarm-0.2.1/PKG-INFO
```

### Comparing `tinynarm-0.2.0/LICENSE` & `tinynarm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinynarm-0.2.0/README.md` & `tinynarm-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,27 +56,27 @@
 from tinynarm.discretization import Discretization
 
 dataset = Discretization("datasets/sportydatagen.csv", 5)
 data = dataset.generate_dataset()
 dataset.dataset_to_csv(data, "new_dataset.csv")
 ```
 
-## NARM references
+## References
 
 [1] I. Fister Jr., A. Iglesias, A. Gálvez, J. Del Ser, E. Osaba, I Fister. [Differential evolution for association rule mining using categorical and numerical attributes](http://www.iztok-jr-fister.eu/static/publications/231.pdf) In: Intelligent data engineering and automated learning - IDEAL 2018, pp. 79-88, 2018.
 
 [2] I. Fister Jr., V. Podgorelec, I. Fister. [Improved Nature-Inspired Algorithms for Numeric Association Rule Mining](https://link.springer.com/chapter/10.1007/978-3-030-68154-8_19). In: Vasant P., Zelinka I., Weber GW. (eds) Intelligent Computing and Optimization. ICO 2020. Advances in Intelligent Systems and Computing, vol 1324. Springer, Cham.
 
 [3] I. Fister Jr., I. Fister [A brief overview of swarm intelligence-based algorithms for numerical association rule mining](https://arxiv.org/abs/2010.15524). arXiv preprint arXiv:2010.15524 (2020).
 
 [4] Stupan, Ž., Fister, I. Jr. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://joss.theoj.org/papers/10.21105/joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.
 
 ## Cite us
 
-Fister Jr, I., Fister, I., Galvez, A., & Iglesias, A. (2023, August). [TinyNARM: Simplifying Numerical Association Rule Mining for Running on Microcontrollers](https://link.springer.com/chapter/10.1007/978-3-031-42529-5_12). In International Conference on Soft Computing Models in Industrial and Environmental Applications (pp. 122-131). Cham: Springer Nature Switzerland.
+Fister Jr, I., Fister, I., Galvez, A., & Iglesias, A. (2023, August). [TinyNARM: Simplifying Numerical Association Rule Mining for Running on Microcontrollers](https://www.iztok.xyz/static/publications/313.pdf). In International Conference on Soft Computing Models in Industrial and Environmental Applications (pp. 122-131). Cham: Springer Nature Switzerland.
 
 ## License
 
 This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
 
 ## Disclaimer
```

### Comparing `tinynarm-0.2.0/tinynarm/comparison.py` & `tinynarm-0.2.1/tinynarm/comparison.py`

 * *Files identical despite different names*

### Comparing `tinynarm-0.2.0/tinynarm/discretization.py` & `tinynarm-0.2.1/tinynarm/discretization.py`

 * *Files identical despite different names*

### Comparing `tinynarm-0.2.0/tinynarm/tinynarm.py` & `tinynarm-0.2.1/tinynarm/tinynarm.py`

 * *Files identical despite different names*

### Comparing `tinynarm-0.2.0/tinynarm/utils.py` & `tinynarm-0.2.1/tinynarm/utils.py`

 * *Files identical despite different names*

### Comparing `tinynarm-0.2.0/setup.py` & `tinynarm-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,101 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tinynarm
+Version: 0.2.1
+Summary: Simplify numerical association rule mining
+Home-page: https://gitlab.com/firefly-cpp/tinynarm
+Keywords: association rule mining,data science,numerical association rule mining,tinyML
+Author: Iztok Fister Jr.
+Author-email: iztok@iztok-jr-fister.eu
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: niaarm (>=0.3.9,<0.4.0)
+Project-URL: Repository, https://gitlab.com/firefly-cpp/tinynarm
+Description-Content-Type: text/markdown
 
-packages = \
-['tinynarm']
+# tinyNARM
 
-package_data = \
-{'': ['*']}
+---
 
-install_requires = \
-['niaarm>=0.3.1,<0.4.0']
-
-setup_kwargs = {
-    'name': 'tinynarm',
-    'version': '0.2.0',
-    'description': 'Simplify numerical association rule mining',
-    'long_description': '# tinyNARM\n\n---\n\n[![PyPI Version](https://img.shields.io/pypi/v/tinynarm.svg)](https://pypi.python.org/pypi/tinynarm)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinynarm.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/tinynarm.svg)\n[![Downloads](https://pepy.tech/badge/tinynarm)](https://pepy.tech/project/tinynarm)\n\n## About\n\ntinyNARM is an experimental effort in approaching/tailoring the classical Numerical Association Rule Mining (NARM) to limited hardware devices, e.g., ESP32 microcontrollers so that devices do not need to depend on remote servers for making decisions. Motivation mainly lies in smart agriculture, where Internet connectivity is unavailable in rural areas.\n\nThe current repository hosts a tinyNARM algorithm prototype initially developed in Python for fast prototyping.\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- loading datasets in CSV format,\n- discretizing numerical features to discrete classes,\n- association rule mining using the tinynarm approach,\n- easy comparison with the NiaARM approach.\n\n## Installation\n\n### pip\n\nInstall tinyNARM with pip:\n\n```sh\npip install tinynarm\n```\n\n## Usage\n\n### Basic run\n\n```python\nfrom tinynarm import TinyNarm\nfrom tinynarm.utils import Utils\n\ntnarm = TinyNarm("new_dataset.csv")\ntnarm.create_rules()\n\npostprocess = Utils(tnarm.rules)\npostprocess.add_fitness()\npostprocess.sort_rules()\npostprocess.rules_to_csv("rules.csv")\npostprocess.generate_statistics()\npostprocess.generate_stats_report(20)\n```\n\n### Discretization\n\n```python\nfrom tinynarm.discretization import Discretization\n\ndataset = Discretization("datasets/sportydatagen.csv", 5)\ndata = dataset.generate_dataset()\ndataset.dataset_to_csv(data, "new_dataset.csv")\n```\n\n## NARM references\n\n[1] I. Fister Jr., A. Iglesias, A. Gálvez, J. Del Ser, E. Osaba, I Fister. [Differential evolution for association rule mining using categorical and numerical attributes](http://www.iztok-jr-fister.eu/static/publications/231.pdf) In: Intelligent data engineering and automated learning - IDEAL 2018, pp. 79-88, 2018.\n\n[2] I. Fister Jr., V. Podgorelec, I. Fister. [Improved Nature-Inspired Algorithms for Numeric Association Rule Mining](https://link.springer.com/chapter/10.1007/978-3-030-68154-8_19). In: Vasant P., Zelinka I., Weber GW. (eds) Intelligent Computing and Optimization. ICO 2020. Advances in Intelligent Systems and Computing, vol 1324. Springer, Cham.\n\n[3] I. Fister Jr., I. Fister [A brief overview of swarm intelligence-based algorithms for numerical association rule mining](https://arxiv.org/abs/2010.15524). arXiv preprint arXiv:2010.15524 (2020).\n\n[4] Stupan, Ž., Fister, I. Jr. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://joss.theoj.org/papers/10.21105/joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.\n\n## Cite us\n\nFister Jr, I., Fister, I., Galvez, A., & Iglesias, A. (2023, August). [TinyNARM: Simplifying Numerical Association Rule Mining for Running on Microcontrollers](https://link.springer.com/chapter/10.1007/978-3-031-42529-5_12). In International Conference on Soft Computing Models in Industrial and Environmental Applications (pp. 122-131). Cham: Springer Nature Switzerland.\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
-    'author': 'Iztok Fister Jr.',
-    'author_email': 'iztok@iztok-jr-fister.eu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/firefly-cpp/tinynarm',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+[![PyPI Version](https://img.shields.io/pypi/v/tinynarm.svg)](https://pypi.python.org/pypi/tinynarm)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinynarm.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tinynarm.svg)
+[![Downloads](https://pepy.tech/badge/tinynarm)](https://pepy.tech/project/tinynarm)
 
+## About
+
+tinyNARM is an experimental effort in approaching/tailoring the classical Numerical Association Rule Mining (NARM) to limited hardware devices, e.g., ESP32 microcontrollers so that devices do not need to depend on remote servers for making decisions. Motivation mainly lies in smart agriculture, where Internet connectivity is unavailable in rural areas.
+
+The current repository hosts a tinyNARM algorithm prototype initially developed in Python for fast prototyping.
+
+## Detailed insights
+The current version includes (but is not limited to) the following functions:
+
+- loading datasets in CSV format,
+- discretizing numerical features to discrete classes,
+- association rule mining using the tinynarm approach,
+- easy comparison with the NiaARM approach.
+
+## Installation
+
+### pip
+
+Install tinyNARM with pip:
+
+```sh
+pip install tinynarm
+```
+
+## Usage
+
+### Basic run
+
+```python
+from tinynarm import TinyNarm
+from tinynarm.utils import Utils
+
+tnarm = TinyNarm("new_dataset.csv")
+tnarm.create_rules()
+
+postprocess = Utils(tnarm.rules)
+postprocess.add_fitness()
+postprocess.sort_rules()
+postprocess.rules_to_csv("rules.csv")
+postprocess.generate_statistics()
+postprocess.generate_stats_report(20)
+```
+
+### Discretization
+
+```python
+from tinynarm.discretization import Discretization
+
+dataset = Discretization("datasets/sportydatagen.csv", 5)
+data = dataset.generate_dataset()
+dataset.dataset_to_csv(data, "new_dataset.csv")
+```
+
+## References
+
+[1] I. Fister Jr., A. Iglesias, A. Gálvez, J. Del Ser, E. Osaba, I Fister. [Differential evolution for association rule mining using categorical and numerical attributes](http://www.iztok-jr-fister.eu/static/publications/231.pdf) In: Intelligent data engineering and automated learning - IDEAL 2018, pp. 79-88, 2018.
+
+[2] I. Fister Jr., V. Podgorelec, I. Fister. [Improved Nature-Inspired Algorithms for Numeric Association Rule Mining](https://link.springer.com/chapter/10.1007/978-3-030-68154-8_19). In: Vasant P., Zelinka I., Weber GW. (eds) Intelligent Computing and Optimization. ICO 2020. Advances in Intelligent Systems and Computing, vol 1324. Springer, Cham.
+
+[3] I. Fister Jr., I. Fister [A brief overview of swarm intelligence-based algorithms for numerical association rule mining](https://arxiv.org/abs/2010.15524). arXiv preprint arXiv:2010.15524 (2020).
+
+[4] Stupan, Ž., Fister, I. Jr. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://joss.theoj.org/papers/10.21105/joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.
+
+## Cite us
+
+Fister Jr, I., Fister, I., Galvez, A., & Iglesias, A. (2023, August). [TinyNARM: Simplifying Numerical Association Rule Mining for Running on Microcontrollers](https://www.iztok.xyz/static/publications/313.pdf). In International Conference on Soft Computing Models in Industrial and Environmental Applications (pp. 122-131). Cham: Springer Nature Switzerland.
+
+## License
+
+This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
+
+## Disclaimer
+
+This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
 
-setup(**setup_kwargs)
```

