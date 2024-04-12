# Comparing `tmp/epidemik-0.0.18.tar.gz` & `tmp/epidemik-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.18.tar", last modified: Thu Apr 11 18:43:33 2024, max compression
+gzip compressed data, was "epidemik-0.0.19.tar", last modified: Fri Apr 12 20:36:32 2024, max compression
```

## Comparing `epidemik-0.0.18.tar` & `epidemik-0.0.19.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726635 epidemik-0.0.18/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.18/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5384 2024-04-11 18:43:33.726454 epidemik-0.0.18/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     4683 2024-04-11 18:19:19.000000 epidemik-0.0.18/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      852 2024-04-11 18:43:24.000000 epidemik-0.0.18/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 18:43:33.726678 epidemik-0.0.18/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.724152 epidemik-0.0.18/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.725265 epidemik-0.0.18/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    18065 2024-04-11 18:03:03.000000 epidemik-0.0.18/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)    11348 2024-04-11 17:58:26.000000 epidemik-0.0.18/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.18/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      329 2024-04-11 18:43:28.000000 epidemik-0.0.18/src/epidemik/__init__.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.18/src/epidemik/utils.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726229 epidemik-0.0.18/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5384 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)       72 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726064 epidemik-0.0.18/tests/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.18/tests/tests_EpiModel.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837699 epidemik-0.0.19/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.19/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     6348 2024-04-12 20:36:32.837494 epidemik-0.0.19/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     5647 2024-04-12 20:16:57.000000 epidemik-0.0.19/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      852 2024-04-12 20:34:33.000000 epidemik-0.0.19/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-12 20:36:32.837739 epidemik-0.0.19/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.834674 epidemik-0.0.19/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.836303 epidemik-0.0.19/src/epidemik/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)    18449 2024-04-12 20:04:35.000000 epidemik-0.0.19/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)    11348 2024-04-11 17:58:26.000000 epidemik-0.0.19/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.19/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      329 2024-04-12 20:36:11.000000 epidemik-0.0.19/src/epidemik/__init__.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      264 2024-04-12 20:04:35.000000 epidemik-0.0.19/src/epidemik/utils.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837263 epidemik-0.0.19/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     6348 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       72 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-12 20:36:32.000000 epidemik-0.0.19/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-12 20:36:32.837077 epidemik-0.0.19/tests/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.19/tests/tests_EpiModel.py
```

### Comparing `epidemik-0.0.18/LICENSE` & `epidemik-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.18/PKG-INFO` & `epidemik-0.0.19/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,9 @@
-Metadata-Version: 2.1
-Name: epidemik
-Version: 0.0.18
-Summary: A pakage to simulate compartmental epidemic models
-Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
-Project-URL: Homepage, https://github.com/DataForScience/epidemik
-Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: networkx>=3
-Requires-Dist: numpy>=1.20
-Requires-Dist: pandas>=2.0
-Requires-Dist: scipy>=1.10
-Requires-Dist: tqdm>=4
+<center>
+<img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/epidemik.png" /></center>
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
@@ -49,32 +32,37 @@
 ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#tech)
 
 
 Here's a brief high-level overview of the tech stack the `epidemik` package uses:
 
 - The model is implemented as a directed multigraph using [networkx](https://networkx.org/)
 - Ordinary Differential Equations are numerically integrated using [scipy](https://scipy.org/)
-- Random numbers are generated by[numpy](https://numpy.org/)
-- Model structure visualizations rely on [matplotlib](https://matplotlib.org/)  
+- Random numbers are generated by [numpy](https://numpy.org/)
+- Model structure visualizations rely on [matplotlib](https://matplotlib.org/)
+- Progress bars generated by [tqdm](https://tqdm.github.io/)
 
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
 
 ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
 
-`epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using
+`epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using the module name
 
 ```python
 from epidemik import EpiModel
 ```
 
-To instanciate a new compartmental model we just need to create a `EpiModel` object and add the relevant transitions:
+- __EpiModel__ -e Simple compartmental model in a homogeneously mixed population.
+- __NetworkEpiModel__ - Compartmental model on a network where nodes interact only along edges connecting them.
+- __MetaEpiModel__ - Meta population model where populations interact with one another along the edges of a network. Each sub-population has it's own internal __EpiModel__ instance.
+
+To instantiate a new compartmental model we just need to create a `EpiModel` object and add the relevant transitions:
 
 ```python
 beta = 0.2
 mu = 0.1
 
 SIR = EpiModel()
 SIR.add_interaction('S', 'I', 'I', beta)
@@ -91,29 +79,31 @@
     Epidemic Model with 3 compartments and 2 transitions:
 
 	S + I = I 0.200000
 	I -> R 0.100000
 
 	R0=2.00
 
-or a graphical representation by calling `draw_model`:
+or a graphical representation by calling `draw_model()`:
 
 ```python
 SIR.draw_model()
 ```
 
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png" />
 
 The models value of the Basic Reproductive Number (R~0~) can be determined using the `R0()` function:
 
 ```python
 SIR.R0()
 ```
 
+There are two ways to explore the dynamics of the model, each with it's corresponding method. 
 
+To integrate numerically the Ordinary Differential Equations that describe the model dynamics, we can call the `integrate()` method. The first argument is the number of time steps to integrate over and the remaining arguments are the initial populations of each compartment.
 
 ```python
 N = 10_000
 I0 = 10
 
 SIR.integrate(365, S=N-I0, I=I0, R=0)
 ```
@@ -161,11 +151,11 @@
 Thank you so much for your interest in growing our community!
 
 
 ---
 
 ## License[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#license)
 
-`epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves. Please have a look at the [LICENSE.md](LICENSE) for more details.
+`epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves, Data For Science, Inc. Please have a look at the [LICENSE.md](LICENSE) for more details.
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
```

#### html2text {}

```diff
@@ -1,48 +1,51 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.18 Summary: A pakage to
-simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
-data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
-Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
-Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
-Requires-Dist: tqdm>=4 # epidemik Compartmental Epidemic Models in Python --
-- ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/
-epidemik/main/images/pin.svg)](#toc) - [Installation](#installation) - [Tech
-Stack](#tech) - [Usage](#usage) - [Contributing](#contributing) - [License]
-(#license) --- ## Installation[![](https://raw.githubusercontent.com/
-DataForScience/epidemik/main/images/pin.svg)](#installation) Use the package
-manager [pip](https://pip.pypa.io/en/stable/) to install epidemik. ```bash pip
-install epidemik ```
+    [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+                                 epidemik.png]
+# epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
+(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
+(#usage) - [Contributing](#contributing) - [License](#license) --- ##
+Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
+main/images/pin.svg)](#installation) Use the package manager [pip](https://
+pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
-scipy.org/) - Random numbers are generated by[numpy](https://numpy.org/) -
-Model structure visualizations rely on [matplotlib](https://matplotlib.org/)
+scipy.org/) - Random numbers are generated by [numpy](https://numpy.org/) -
+Model structure visualizations rely on [matplotlib](https://matplotlib.org/) -
+Progress bars generated by [tqdm](https://tqdm.github.io/)
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/
 main/images/pin.svg)](#usage) `epidemik` provides three main modules,
 `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly
-from the `epidemik` package using ```python from epidemik import EpiModel ```
-To instanciate a new compartmental model we just need to create a `EpiModel`
-object and add the relevant transitions: ```python beta = 0.2 mu = 0.1 SIR =
-EpiModel() SIR.add_interaction('S', 'I', 'I', beta) SIR.add_spontaneous('I',
-'R', mu) ``` This fully defines the model. We can get a textual representation
-of the model using ```python print(SIR) ``` resulting in a simple description
-of hte model structure. Epidemic Model with 3 compartments and 2 transitions: S
-+ I = I 0.200000 I -> R 0.100000 R0=2.00 or a graphical representation by
-calling `draw_model`: ```python SIR.draw_model() ``` [https://
-raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png]The
-models value of the Basic Reproductive Number (R~0~) can be determined using
-the `R0()` function: ```python SIR.R0() ``` ```python N = 10_000 I0 = 10
+from the `epidemik` package using the module name ```python from epidemik
+import EpiModel ``` - __EpiModel__ -e Simple compartmental model in a
+homogeneously mixed population. - __NetworkEpiModel__ - Compartmental model on
+a network where nodes interact only along edges connecting them. -
+__MetaEpiModel__ - Meta population model where populations interact with one
+another along the edges of a network. Each sub-population has it's own internal
+__EpiModel__ instance. To instantiate a new compartmental model we just need to
+create a `EpiModel` object and add the relevant transitions: ```python beta =
+0.2 mu = 0.1 SIR = EpiModel() SIR.add_interaction('S', 'I', 'I', beta)
+SIR.add_spontaneous('I', 'R', mu) ``` This fully defines the model. We can get
+a textual representation of the model using ```python print(SIR) ``` resulting
+in a simple description of hte model structure. Epidemic Model with 3
+compartments and 2 transitions: S + I = I 0.200000 I -> R 0.100000 R0=2.00 or a
+graphical representation by calling `draw_model()`: ```python SIR.draw_model()
+``` [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+SIR.png]The models value of the Basic Reproductive Number (R~0~) can be
+determined using the `R0()` function: ```python SIR.R0() ``` There are two ways
+to explore the dynamics of the model, each with it's corresponding method. To
+integrate numerically the Ordinary Differential Equations that describe the
+model dynamics, we can call the `integrate()` method. The first argument is the
+number of time steps to integrate over and the remaining arguments are the
+initial populations of each compartment. ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
@@ -63,10 +66,10 @@
 DataForScience/epidemik/) to the repository to encourage contributors and helps
 to grow our community. - Tweet about the project on your Twitter! - Tag
 [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://
 twitter.com/bgoncalves) Thank you so much for your interest in growing our
 community! --- ## License[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#license) `epidemik` is free and open-source
 software licensed under the [MIT License](https://choosealicense.com/licenses/
-mit/) [2024] - Bruno GonÃ§alves. Please have a look at the [LICENSE.md]
-(LICENSE) for more details.
+mit/) [2024] - Bruno GonÃ§alves, Data For Science, Inc. Please have a look at
+the [LICENSE.md](LICENSE) for more details.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
```

### Comparing `epidemik-0.0.18/pyproject.toml` & `epidemik-0.0.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
- "matplotlib>=3.8",
+ "matplotlib>=3.3",
  "networkx>=3",
  "numpy>=1.20",
  "pandas>=2.0",
  "scipy>=1.10",
  "tqdm>=4"
 ]
 [project.urls]
```

### Comparing `epidemik-0.0.18/src/epidemik/EpiModel.py` & `epidemik-0.0.19/src/epidemik/EpiModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -184,48 +184,59 @@
                     rate *= season
                 
             diff[pos[source]] -= rate
             diff[pos[target]] += rate
             
         return diff
     
-    def plot(self, title=None, normed=True, show=True, **kwargs):
+    def plot(self, title=None, normed=True, show=True, ax=None, **kwargs):
         """
         Convenience function for plotting
         
         Parameters:
         - title: string, optional
             Title of the plot
-        - normed: bool, optional
+        - normed: bool, default=True
             Whether to normalize the values or not
+        - ax: matplotlib Axes object, default=None
+            The Axes object to plot to. If None, a new figure is created.
+        - show: bool, default=True
+            Whether to call plt.show() or not
         - kwargs: keyword arguments
             Additional arguments to pass to the plot function
         
         Returns:
         matplotlib.axes._subplots.AxesSubplot
             The plot object
         """
         try:
             if normed:
                 N = self.values_.iloc[0].sum()
-                ax = (self.values_/N).plot(**kwargs)
             else:
-                ax = self.values_.plot(**kwargs)
-                
+                N = 1
+
+            if ax is None:
+                ax = plt.gca()
+
+            for comp in self.values_.columns:
+                (self.values_[comp]/N).plot(c=epi_colors[comp[0]], **kwargs)
+
+            ax.legend(self.values_.columns)
             ax.set_xlabel('Time')
             ax.set_ylabel('Population')
             
             if title is not None:
                 ax.set_title(title)
             
             if show:
                 plt.show()
 
             return ax
-        except:
+        except Exception as e:
+            print(e)
             raise NotInitialized('You must call integrate() or simulate() first')
     
     def __getattr__(self, name):
         """
         Dynamic method to return the individual compartment values
         
         Parameters:
@@ -458,44 +469,32 @@
 
                 inf[agent][node_i]['target'] = node_j
                 inf[agent][node_i]['rate'] = data['rate']
 
         return inf
 
     def draw_model(self, ax=None, show=True):
+        """
+        Plot the model structure
+
+        - ax: matplotlib Axes object, default=None
+            The Axes object to plot to. If None, a new figure is created.
+        - show: bool, default=True
+            Whether to call plt.show() or not
+        """
         try:
             from networkx.drawing.nx_agraph import graphviz_layout
             pos=graphviz_layout(self.transitions, prog='dot', args='-Grankdir="LR"')
         except:
             pos=nx.layout.spectral_layout(self.transitions)
 
-        colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-
-        S_color = colors[0]
-        E_color = colors[4]
-        I_color = colors[1]
-        R_color = colors[2]
-        D_color = colors[7]
-        default_color = colors[3]
-
         node_colors = []
 
         for node in self.transitions.nodes():
-            if node[0] == 'S':
-                node_colors.append(S_color)
-            elif node[0] == 'E':
-                node_colors.append(E_color)
-            elif node[0] == 'I':
-                node_colors.append(I_color)
-            elif node[0] == 'R':
-                node_colors.append(R_color)
-            elif node[0] == 'D':
-                node_colors.append(D_color)
-            else:
-                node_colors.append(default_color)
+            node_colors.append(epi_colors[node[0]])
 
         edge_labels = {}
 
         for node_i, node_j, data in self.transitions.edges(data=True):
             edge = (node_i, node_j)
 
             if "agent" in data:
@@ -504,24 +503,34 @@
                 else:
                     edge_labels[edge] = edge_labels[edge] + "+" + data["agent"]
             else:
                 edge_labels[edge] = ""
 
 
         if ax is None:
-            fig, ax = plt.subplots(1)
+            fig, ax = plt.subplots(1, figsize=(10, 2))
 
         nx.draw(self.transitions, pos, with_labels=True, arrows=True, node_shape='H', 
         font_color='k', node_color=node_colors, node_size=1000, ax=ax)
         nx.draw_networkx_edge_labels(self.transitions, pos, edge_labels=edge_labels, ax=ax)
 
         if show:
             plt.show()
 
     def R0(self):
+        """
+        Return the value of the basic reproductive ratio, $R_0$, for the model as defined
+
+        The calculation is completely generic as it uses the Next-Generation matrix approach
+        defined in J. R. Soc Interface 7, 873 (2010)
+
+        Returns:
+        R0 - the value of the largest eigenvalue of the next generation matrix
+        """
+
         infected = set()
 
         susceptible = self._get_susceptible()
 
         for node_i, node_j, data in self.transitions.edges(data=True):
             if "agent" in data:
                 infected.add(data['agent'])
```

### Comparing `epidemik-0.0.18/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.19/src/epidemik/MetaEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.18/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.19/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.18/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.19/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.18
+Version: 0.0.19
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: matplotlib>=3.8
+Requires-Dist: matplotlib>=3.3
 Requires-Dist: networkx>=3
 Requires-Dist: numpy>=1.20
 Requires-Dist: pandas>=2.0
 Requires-Dist: scipy>=1.10
 Requires-Dist: tqdm>=4
 
+<center>
+<img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/epidemik.png" /></center>
+
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
 
@@ -49,32 +52,37 @@
 ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#tech)
 
 
 Here's a brief high-level overview of the tech stack the `epidemik` package uses:
 
 - The model is implemented as a directed multigraph using [networkx](https://networkx.org/)
 - Ordinary Differential Equations are numerically integrated using [scipy](https://scipy.org/)
-- Random numbers are generated by[numpy](https://numpy.org/)
-- Model structure visualizations rely on [matplotlib](https://matplotlib.org/)  
+- Random numbers are generated by [numpy](https://numpy.org/)
+- Model structure visualizations rely on [matplotlib](https://matplotlib.org/)
+- Progress bars generated by [tqdm](https://tqdm.github.io/)
 
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
 
 
 ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#usage)
 
-`epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using
+`epidemik` provides three main modules, `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly from the `epidemik` package using the module name
 
 ```python
 from epidemik import EpiModel
 ```
 
-To instanciate a new compartmental model we just need to create a `EpiModel` object and add the relevant transitions:
+- __EpiModel__ -e Simple compartmental model in a homogeneously mixed population.
+- __NetworkEpiModel__ - Compartmental model on a network where nodes interact only along edges connecting them.
+- __MetaEpiModel__ - Meta population model where populations interact with one another along the edges of a network. Each sub-population has it's own internal __EpiModel__ instance.
+
+To instantiate a new compartmental model we just need to create a `EpiModel` object and add the relevant transitions:
 
 ```python
 beta = 0.2
 mu = 0.1
 
 SIR = EpiModel()
 SIR.add_interaction('S', 'I', 'I', beta)
@@ -91,29 +99,31 @@
     Epidemic Model with 3 compartments and 2 transitions:
 
 	S + I = I 0.200000
 	I -> R 0.100000
 
 	R0=2.00
 
-or a graphical representation by calling `draw_model`:
+or a graphical representation by calling `draw_model()`:
 
 ```python
 SIR.draw_model()
 ```
 
 <img src="https://raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png" />
 
 The models value of the Basic Reproductive Number (R~0~) can be determined using the `R0()` function:
 
 ```python
 SIR.R0()
 ```
 
+There are two ways to explore the dynamics of the model, each with it's corresponding method. 
 
+To integrate numerically the Ordinary Differential Equations that describe the model dynamics, we can call the `integrate()` method. The first argument is the number of time steps to integrate over and the remaining arguments are the initial populations of each compartment.
 
 ```python
 N = 10_000
 I0 = 10
 
 SIR.integrate(365, S=N-I0, I=I0, R=0)
 ```
@@ -161,11 +171,11 @@
 Thank you so much for your interest in growing our community!
 
 
 ---
 
 ## License[![](https://raw.githubusercontent.com/DataForScience/epidemik/main/images/pin.svg)](#license)
 
-`epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves. Please have a look at the [LICENSE.md](LICENSE) for more details.
+`epidemik` is free and open-source software licensed under the [MIT License](https://choosealicense.com/licenses/mit/) [2024]  - Bruno Gonçalves, Data For Science, Inc. Please have a look at the [LICENSE.md](LICENSE) for more details.
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
```

#### html2text {}

```diff
@@ -1,48 +1,61 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.18 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.19 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
+LICENSE Requires-Dist: matplotlib>=3.3 Requires-Dist: networkx>=3 Requires-
 Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
-Requires-Dist: tqdm>=4 # epidemik Compartmental Epidemic Models in Python --
-- ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/
-epidemik/main/images/pin.svg)](#toc) - [Installation](#installation) - [Tech
-Stack](#tech) - [Usage](#usage) - [Contributing](#contributing) - [License]
-(#license) --- ## Installation[![](https://raw.githubusercontent.com/
-DataForScience/epidemik/main/images/pin.svg)](#installation) Use the package
-manager [pip](https://pip.pypa.io/en/stable/) to install epidemik. ```bash pip
-install epidemik ```
+Requires-Dist: tqdm>=4
+    [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+                                 epidemik.png]
+# epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
+(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
+(#usage) - [Contributing](#contributing) - [License](#license) --- ##
+Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
+main/images/pin.svg)](#installation) Use the package manager [pip](https://
+pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
-scipy.org/) - Random numbers are generated by[numpy](https://numpy.org/) -
-Model structure visualizations rely on [matplotlib](https://matplotlib.org/)
+scipy.org/) - Random numbers are generated by [numpy](https://numpy.org/) -
+Model structure visualizations rely on [matplotlib](https://matplotlib.org/) -
+Progress bars generated by [tqdm](https://tqdm.github.io/)
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Usage[![](https://raw.githubusercontent.com/DataForScience/epidemik/
 main/images/pin.svg)](#usage) `epidemik` provides three main modules,
 `EpiModel`, `NetworkEpiModel` and `MetaEpiModel`, usually imported directly
-from the `epidemik` package using ```python from epidemik import EpiModel ```
-To instanciate a new compartmental model we just need to create a `EpiModel`
-object and add the relevant transitions: ```python beta = 0.2 mu = 0.1 SIR =
-EpiModel() SIR.add_interaction('S', 'I', 'I', beta) SIR.add_spontaneous('I',
-'R', mu) ``` This fully defines the model. We can get a textual representation
-of the model using ```python print(SIR) ``` resulting in a simple description
-of hte model structure. Epidemic Model with 3 compartments and 2 transitions: S
-+ I = I 0.200000 I -> R 0.100000 R0=2.00 or a graphical representation by
-calling `draw_model`: ```python SIR.draw_model() ``` [https://
-raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png]The
-models value of the Basic Reproductive Number (R~0~) can be determined using
-the `R0()` function: ```python SIR.R0() ``` ```python N = 10_000 I0 = 10
+from the `epidemik` package using the module name ```python from epidemik
+import EpiModel ``` - __EpiModel__ -e Simple compartmental model in a
+homogeneously mixed population. - __NetworkEpiModel__ - Compartmental model on
+a network where nodes interact only along edges connecting them. -
+__MetaEpiModel__ - Meta population model where populations interact with one
+another along the edges of a network. Each sub-population has it's own internal
+__EpiModel__ instance. To instantiate a new compartmental model we just need to
+create a `EpiModel` object and add the relevant transitions: ```python beta =
+0.2 mu = 0.1 SIR = EpiModel() SIR.add_interaction('S', 'I', 'I', beta)
+SIR.add_spontaneous('I', 'R', mu) ``` This fully defines the model. We can get
+a textual representation of the model using ```python print(SIR) ``` resulting
+in a simple description of hte model structure. Epidemic Model with 3
+compartments and 2 transitions: S + I = I 0.200000 I -> R 0.100000 R0=2.00 or a
+graphical representation by calling `draw_model()`: ```python SIR.draw_model()
+``` [https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
+SIR.png]The models value of the Basic Reproductive Number (R~0~) can be
+determined using the `R0()` function: ```python SIR.R0() ``` There are two ways
+to explore the dynamics of the model, each with it's corresponding method. To
+integrate numerically the Ordinary Differential Equations that describe the
+model dynamics, we can call the `integrate()` method. The first argument is the
+number of time steps to integrate over and the remaining arguments are the
+initial populations of each compartment. ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
@@ -63,10 +76,10 @@
 DataForScience/epidemik/) to the repository to encourage contributors and helps
 to grow our community. - Tweet about the project on your Twitter! - Tag
 [@data4sci](https://twitter.com/data4sci) and/or [@bgoncalves](https://
 twitter.com/bgoncalves) Thank you so much for your interest in growing our
 community! --- ## License[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#license) `epidemik` is free and open-source
 software licensed under the [MIT License](https://choosealicense.com/licenses/
-mit/) [2024] - Bruno GonÃ§alves. Please have a look at the [LICENSE.md]
-(LICENSE) for more details.
+mit/) [2024] - Bruno GonÃ§alves, Data For Science, Inc. Please have a look at
+the [LICENSE.md](LICENSE) for more details.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
```

### Comparing `epidemik-0.0.18/tests/tests_EpiModel.py` & `epidemik-0.0.19/tests/tests_EpiModel.py`

 * *Files identical despite different names*

