# Comparing `tmp/niaarm-0.3.8.tar.gz` & `tmp/niaarm-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niaarm-0.3.8.tar", max compression
+gzip compressed data, was "niaarm-0.3.9.tar", max compression
```

## Comparing `niaarm-0.3.8.tar` & `niaarm-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    15279 2024-03-13 19:37:50.679193 niaarm-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     1095 2024-03-13 19:37:50.680193 niaarm-0.3.8/LICENSE
--rw-r--r--   0        0        0    13841 2024-03-13 19:37:50.680193 niaarm-0.3.8/README.md
--rw-r--r--   0        0        0      355 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/__init__.py
--rw-r--r--   0        0        0       88 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/__main__.py
--rw-r--r--   0        0        0    10948 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/cli.py
--rw-r--r--   0        0        0     4157 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/dataset.py
--rw-r--r--   0        0        0     1565 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/feature.py
--rw-r--r--   0        0        0     4663 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/mine.py
--rw-r--r--   0        0        0     7166 2024-03-13 19:37:50.689193 niaarm-0.3.8/niaarm/niaarm.py
--rw-r--r--   0        0        0     2636 2024-03-13 19:37:50.690193 niaarm-0.3.8/niaarm/preprocessing.py
--rw-r--r--   0        0        0    14458 2024-03-13 19:37:50.690193 niaarm-0.3.8/niaarm/rule.py
--rw-r--r--   0        0        0     3858 2024-03-13 19:37:50.690193 niaarm-0.3.8/niaarm/rule_list.py
--rw-r--r--   0        0        0    12627 2024-03-13 19:37:50.690193 niaarm-0.3.8/niaarm/text.py
--rw-r--r--   0        0        0     3837 2024-03-13 19:37:50.690193 niaarm-0.3.8/niaarm/visualize.py
--rw-r--r--   0        0        0     1542 2024-03-13 19:37:50.688193 niaarm-0.3.8/niaarm.1
--rw-r--r--   0        0        0     1334 2024-03-13 19:37:50.695193 niaarm-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    14867 1970-01-01 00:00:00.000000 niaarm-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    15279 2024-04-12 12:13:25.409123 niaarm-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0      479 2024-04-12 12:13:25.409123 niaarm-0.3.9/CITATION.cff
+-rw-r--r--   0        0        0     1095 2024-04-12 12:13:25.410123 niaarm-0.3.9/LICENSE
+-rw-r--r--   0        0        0    17375 2024-04-12 12:13:25.410123 niaarm-0.3.9/README.md
+-rw-r--r--   0        0        0      355 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/__main__.py
+-rw-r--r--   0        0        0    10948 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/cli.py
+-rw-r--r--   0        0        0     4157 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/dataset.py
+-rw-r--r--   0        0        0     1565 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/feature.py
+-rw-r--r--   0        0        0     4663 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/mine.py
+-rw-r--r--   0        0        0     7166 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm/niaarm.py
+-rw-r--r--   0        0        0     2636 2024-04-12 12:13:25.415123 niaarm-0.3.9/niaarm/preprocessing.py
+-rw-r--r--   0        0        0    15340 2024-04-12 12:13:25.415123 niaarm-0.3.9/niaarm/rule.py
+-rw-r--r--   0        0        0     3858 2024-04-12 12:13:25.415123 niaarm-0.3.9/niaarm/rule_list.py
+-rw-r--r--   0        0        0    12627 2024-04-12 12:13:25.415123 niaarm-0.3.9/niaarm/text.py
+-rw-r--r--   0        0        0     3837 2024-04-12 12:13:25.415123 niaarm-0.3.9/niaarm/visualize.py
+-rw-r--r--   0        0        0     1542 2024-04-12 12:13:25.414123 niaarm-0.3.9/niaarm.1
+-rw-r--r--   0        0        0     1372 2024-04-12 12:13:25.418123 niaarm-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    18400 1970-01-01 00:00:00.000000 niaarm-0.3.9/PKG-INFO
```

### Comparing `niaarm-0.3.8/CHANGELOG.md` & `niaarm-0.3.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/LICENSE` & `niaarm-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/README.md` & `niaarm-0.3.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 [![GitHub license](https://img.shields.io/github/license/firefly-cpp/niaarm.svg)](https://github.com/firefly-cpp/NiaARM/blob/main/LICENSE)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/niaarm.svg)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/niaarm.svg)](http://isitmaintained.com/project/firefly-cpp/niaarm "Average time to resolve an issue")
 [![Fedora package](https://img.shields.io/fedora/v/python3-niaarm?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-niaarm)
 [![AUR package](https://img.shields.io/aur/version/python-niaarm?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-niaarm)
 [![Packaging status](https://repology.org/badge/tiny-repos/python:niaarm.svg)](https://repology.org/project/python:niaarm/versions)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04448/status.svg)](https://doi.org/10.21105/joss.04448)
+[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 
 * **Documentation:** https://niaarm.readthedocs.io/en/latest
 * **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**
 
 ## About 📋
 NiaARM is a framework for Association Rule Mining based on nature-inspired algorithms for optimization. 🌿 The framework is written fully in Python and runs on all platforms. NiaARM allows users to preprocess the data in a transaction database automatically, to search for association rules and provide a pretty output of the rules found. 📊 This framework also supports integral and real-valued types of attributes besides the categorical ones. Mining the association rules is defined as an optimization problem, and solved using the nature-inspired algorithms that come from the related framework called [NiaPy](https://github.com/NiaOrg/NiaPy). 🔗
 
@@ -309,7 +310,34 @@
 ## Disclaimer
 
 This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
 
 ## Cite us
 
 Stupan, Ž., & Fister Jr., I. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://www.theoj.org/joss-papers/joss.04448/10.21105.joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zStupan"><img src="https://avatars.githubusercontent.com/u/48752988?v=4?s=100" width="100px;" alt="zStupan"/><br /><sub><b>zStupan</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=zStupan" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3AzStupan" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/NiaARM/commits?author=zStupan" title="Documentation">📖</a> <a href="#content-zStupan" title="Content">🖋</a> <a href="#ideas-zStupan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#example-zStupan" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok.xyz"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=firefly-cpp" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://erkankarabulut.github.io"><img src="https://avatars.githubusercontent.com/u/15374776?v=4?s=100" width="100px;" alt="Erkan Karabulut"/><br /><sub><b>Erkan Karabulut</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=erkankarabulut" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3Aerkankarabulut" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=lahovniktadej" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/musicinmybrain"><img src="https://avatars.githubusercontent.com/u/6898909?v=4?s=100" width="100px;" alt="Ben Beasley"/><br /><sub><b>Ben Beasley</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=musicinmybrain" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.dusanfister.com"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="Dusan Fister"/><br /><sub><b>Dusan Fister</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

### Comparing `niaarm-0.3.8/niaarm/cli.py` & `niaarm-0.3.9/niaarm/cli.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/dataset.py` & `niaarm-0.3.9/niaarm/dataset.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/feature.py` & `niaarm-0.3.9/niaarm/feature.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/mine.py` & `niaarm-0.3.9/niaarm/mine.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/niaarm.py` & `niaarm-0.3.9/niaarm/niaarm.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/preprocessing.py` & `niaarm-0.3.9/niaarm/preprocessing.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/rule.py` & `niaarm-0.3.9/niaarm/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,24 @@
 
          **Range:** :math:`[-1, 1]` (-1 reflects total negative association, 1 reflects perfect positive association
          and 0 reflects independence)
 
          **Reference:** T. Zhang, “Association Rules,” in Knowledge Discovery and Data Mining. Current Issues and New
          Applications, 2000, pp. 245–256. doi: 10.1007/3-540-45571-X_31.
 
+        leverage: difference between the frequency of antecedent and the consequent appearing together and the expected
+        frequency of them appearing separately based on their individual support
+
+        :math: `leverage(X \implies Y) = support(X \implies Y) - (support(X) \times support(Y))`
+
+        **Range:** :math: `[-1, 1]` (-1 reflects total negative association, 1 reflects perfect positive association
+         and 0 reflects independence)
+
+        **Reference:** Gregory Piatetsky-Shapiro. 1991. Discovery, Analysis, and Presentation of Strong Rules. In
+        Knowledge Discovery in Databases, Gregory Piatetsky-Shapiro and William J. Frawley (Eds.). AAAI/MIT Press, 229–248.
     """
 
     __slots__ = (
         "antecedent",
         "consequent",
         "fitness",
         "num_transactions",
@@ -323,14 +333,19 @@
         denominator = (
             max(support * (1 - support_x), support_x * (support_y - support))
             + 2.220446049250313e-16
         )
 
         return numerator / denominator
 
+    @property
+    def leverage(self):
+        return self.support - (
+                (self.antecedent_count / self.num_transactions) * (self.consequent_count / self.num_transactions))
+
     def __eq__(self, other):
         return (
             self.antecedent == other.antecedent and self.consequent == other.consequent
         )
 
     def __repr__(self):
         return f"{self.antecedent} => {self.consequent}"
```

### Comparing `niaarm-0.3.8/niaarm/rule_list.py` & `niaarm-0.3.9/niaarm/rule_list.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/text.py` & `niaarm-0.3.9/niaarm/text.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm/visualize.py` & `niaarm-0.3.9/niaarm/visualize.py`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/niaarm.1` & `niaarm-0.3.9/niaarm.1`

 * *Files identical despite different names*

### Comparing `niaarm-0.3.8/pyproject.toml` & `niaarm-0.3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "niaarm"
-version = "0.3.8"
+version = "0.3.9"
 description = "A minimalistic framework for numerical association rule mining"
 authors = ["Žiga Stupan <ziga.stupan1@student.um.si>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
 keywords = ['association rule mining', 'data science', 'numerical association rule mining', 'preprocessing', 'visualization']
 homepage = "https://github.com/firefly-cpp/NiaARM"
 repository = "https://github.com/firefly-cpp/NiaARM"
 documentation = "https://niaarm.readthedocs.io/en/latest/"
 license = "MIT"
 readme = "README.md"
 
 include = [
     { path="LICENSE", format="sdist" },
     { path="CHANGELOG.md", format="sdist" },
+    { path="CITATION.cff", format="sdist" },
     { path="niaarm.1", format="sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = "^3.9"
 niapy = "^2.0.5"
 numpy = "^1.26.1"
 pandas = "^2.1.1"
 nltk = "^3.8.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `niaarm-0.3.8/PKG-INFO` & `niaarm-0.3.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: niaarm
-Version: 0.3.8
+Version: 0.3.9
 Summary: A minimalistic framework for numerical association rule mining
 Home-page: https://github.com/firefly-cpp/NiaARM
 License: MIT
 Keywords: association rule mining,data science,numerical association rule mining,preprocessing,visualization
 Author: Žiga Stupan
 Author-email: ziga.stupan1@student.um.si
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: niapy (>=2.0.5,<3.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
@@ -35,14 +35,15 @@
 [![GitHub license](https://img.shields.io/github/license/firefly-cpp/niaarm.svg)](https://github.com/firefly-cpp/NiaARM/blob/main/LICENSE)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/niaarm.svg)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/niaarm.svg)](http://isitmaintained.com/project/firefly-cpp/niaarm "Average time to resolve an issue")
 [![Fedora package](https://img.shields.io/fedora/v/python3-niaarm?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/python-niaarm)
 [![AUR package](https://img.shields.io/aur/version/python-niaarm?color=blue&label=Arch%20Linux&logo=arch-linux)](https://aur.archlinux.org/packages/python-niaarm)
 [![Packaging status](https://repology.org/badge/tiny-repos/python:niaarm.svg)](https://repology.org/project/python:niaarm/versions)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04448/status.svg)](https://doi.org/10.21105/joss.04448)
+[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 
 * **Documentation:** https://niaarm.readthedocs.io/en/latest
 * **Tested OS:** Windows, Ubuntu, Fedora, Alpine, Arch, macOS. **However, that does not mean it does not work on others**
 
 ## About 📋
 NiaARM is a framework for Association Rule Mining based on nature-inspired algorithms for optimization. 🌿 The framework is written fully in Python and runs on all platforms. NiaARM allows users to preprocess the data in a transaction database automatically, to search for association rules and provide a pretty output of the rules found. 📊 This framework also supports integral and real-valued types of attributes besides the categorical ones. Mining the association rules is defined as an optimization problem, and solved using the nature-inspired algorithms that come from the related framework called [NiaPy](https://github.com/NiaOrg/NiaPy). 🔗
 
@@ -334,7 +335,34 @@
 
 This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
 
 ## Cite us
 
 Stupan, Ž., & Fister Jr., I. (2022). [NiaARM: A minimalistic framework for Numerical Association Rule Mining](https://www.theoj.org/joss-papers/joss.04448/10.21105.joss.04448.pdf). Journal of Open Source Software, 7(77), 4448.
 
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zStupan"><img src="https://avatars.githubusercontent.com/u/48752988?v=4?s=100" width="100px;" alt="zStupan"/><br /><sub><b>zStupan</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=zStupan" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3AzStupan" title="Bug reports">🐛</a> <a href="https://github.com/firefly-cpp/NiaARM/commits?author=zStupan" title="Documentation">📖</a> <a href="#content-zStupan" title="Content">🖋</a> <a href="#ideas-zStupan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#example-zStupan" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.iztok.xyz"><img src="https://avatars.githubusercontent.com/u/1633361?v=4?s=100" width="100px;" alt="Iztok Fister Jr."/><br /><sub><b>Iztok Fister Jr.</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=firefly-cpp" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3Afirefly-cpp" title="Bug reports">🐛</a> <a href="#mentoring-firefly-cpp" title="Mentoring">🧑‍🏫</a> <a href="#maintenance-firefly-cpp" title="Maintenance">🚧</a> <a href="#ideas-firefly-cpp" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://erkankarabulut.github.io"><img src="https://avatars.githubusercontent.com/u/15374776?v=4?s=100" width="100px;" alt="Erkan Karabulut"/><br /><sub><b>Erkan Karabulut</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=erkankarabulut" title="Code">💻</a> <a href="https://github.com/firefly-cpp/NiaARM/issues?q=author%3Aerkankarabulut" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lahovniktadej"><img src="https://avatars.githubusercontent.com/u/57890734?v=4?s=100" width="100px;" alt="Tadej Lahovnik"/><br /><sub><b>Tadej Lahovnik</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=lahovniktadej" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/musicinmybrain"><img src="https://avatars.githubusercontent.com/u/6898909?v=4?s=100" width="100px;" alt="Ben Beasley"/><br /><sub><b>Ben Beasley</b></sub></a><br /><a href="https://github.com/firefly-cpp/NiaARM/commits?author=musicinmybrain" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.dusanfister.com"><img src="https://avatars.githubusercontent.com/u/3198785?v=4?s=100" width="100px;" alt="Dusan Fister"/><br /><sub><b>Dusan Fister</b></sub></a><br /><a href="#design-rhododendrom" title="Design">🎨</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
```

