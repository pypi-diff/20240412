# Comparing `tmp/starsim-0.1.5.tar.gz` & `tmp/starsim-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starsim-0.1.5.tar", last modified: Mon Jan 22 23:27:20 2024, max compression
+gzip compressed data, was "starsim-0.3.2.tar", last modified: Fri Apr 12 07:22:13 2024, max compression
```

## Comparing `starsim-0.1.5.tar` & `starsim-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.034353 starsim-0.1.5/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2023-10-21 14:33:38.000000 starsim-0.1.5/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3492 2024-01-22 23:27:20.034353 starsim-0.1.5/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2696 2024-01-22 23:27:07.000000 starsim-0.1.5/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-01-22 23:27:20.034353 starsim-0.1.5/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1468 2024-01-22 20:05:46.000000 starsim-0.1.5/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.030353 starsim-0.1.5/starsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      699 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      271 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/analyzers.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/connectors.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20161 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/demographics.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.030353 starsim-0.1.5/starsim/diseases/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16960 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/disease.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     8998 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/examples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3288 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/gonorrhea.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4379 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    11915 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/diseases/syphilis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15359 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      557 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4013 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/modules.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.030353 starsim-0.1.5/starsim/networks/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       47 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/networks/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    37473 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/networks/networks.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3549 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/networks/randnet.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4119 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14081 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9159 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/random.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1129 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/results.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7799 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    36484 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19430 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/states.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    10716 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2024-01-22 20:05:46.000000 starsim-0.1.5/starsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.030353 starsim-0.1.5/starsim.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3492 2024-01-22 23:27:19.000000 starsim-0.1.5/starsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      950 2024-01-22 23:27:20.000000 starsim-0.1.5/starsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-01-22 23:27:19.000000 starsim-0.1.5/starsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       74 2024-01-22 23:27:19.000000 starsim-0.1.5/starsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-01-22 23:27:19.000000 starsim-0.1.5/starsim.egg-info/top_level.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-01-22 23:27:20.034353 starsim-0.1.5/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3310 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5825 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_baselines.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4727 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_demographics.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5671 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_distributions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2267 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_examples.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3210 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_random.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5512 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_rngcontainer.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3437 2024-01-22 20:05:46.000000 starsim-0.1.5/tests/test_syphilis.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1088 2024-03-30 07:25:13.000000 starsim-0.3.2/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-12 07:22:13.627713 starsim-0.3.2/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2705 2024-03-30 07:25:13.000000 starsim-0.3.2/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2024-04-12 07:22:13.627713 starsim-0.3.2/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1619 2024-04-03 13:56:26.000000 starsim-0.3.2/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.623713 starsim-0.3.2/starsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1046 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1191 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/connectors.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    19926 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    16370 2024-04-06 16:25:59.000000 starsim-0.3.2/starsim/disease.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/starsim/diseases/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      285 2024-04-02 03:48:03.000000 starsim-0.3.2/starsim/diseases/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     9033 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/cholera.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5876 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/ebola.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3385 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/diseases/gonorrhea.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4668 2024-04-05 21:02:35.000000 starsim-0.3.2/starsim/diseases/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3283 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/measles.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3423 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/diseases/ncd.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5895 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/sir.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    14752 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/diseases/syphilis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28830 2024-04-03 14:06:30.000000 starsim-0.3.2/starsim/distributions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22027 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6672 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/modules.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    42277 2024-04-06 16:25:59.000000 starsim-0.3.2/starsim/network.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3979 2024-04-02 04:22:31.000000 starsim-0.3.2/starsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15132 2024-04-12 07:22:08.000000 starsim-0.3.2/starsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5869 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/products.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2080 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/results.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    15347 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13972 2024-04-02 03:48:00.000000 starsim-0.3.2/starsim/samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7608 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    45922 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24451 2024-04-12 07:22:08.000000 starsim-0.3.2/starsim/states.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13010 2024-04-03 13:56:26.000000 starsim-0.3.2/starsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      239 2024-04-11 11:28:46.000000 starsim-0.3.2/starsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/starsim.egg-info/
+-rw-r--r--   0 cliffk    (1000) cliffk    (1000)     3610 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1014 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        8 2024-04-12 07:22:13.000000 starsim-0.3.2/starsim.egg-info/top_level.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2024-04-12 07:22:13.627713 starsim-0.3.2/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3550 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5666 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      973 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dcp.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5702 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_demographics.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3274 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_diseases.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7721 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dist.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5914 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_dists.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1420 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_samples.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     5576 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_simple.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6159 2024-04-03 13:56:26.000000 starsim-0.3.2/tests/test_syphilis.py
```

### Comparing `starsim-0.1.5/LICENSE` & `starsim-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starsim-0.1.5/PKG-INFO` & `starsim-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.1.5
+Version: 0.3.2
 Summary: Starsim
-Author: Robyn Stuart, Romesh Abeysuriya, Jamie Cohen, Cliff Kerr, Daniel Klein
+Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Starsim
 =======
 
+**Warning! Starsim is still in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used for real research or policy questions.**
+
 Starsim is an agent-based disease modeling framework in which users can design and configure simulations of pathogens that progress over time within each agent and pass from one agent to the next along dynamic transmission networks. The framework explicitly supports co-transmission of multiple pathogens, allowing users to concurrently simulate several diseases while capturing behavioral and biological interactions. Non-communicable diseases can easily be included as well, either as a co-factor for transmissible pathogens or as an independent exploration. Detailed modeling of mother-child relationships can be simulated from the timepoint of conception, enabling study of congenital diseases and associated birth outcomes. Finally, Starsim facilitates the comparison of one or more intervention scenarios to a baseline scenario in evaluating the impact of various products like vaccines, therapeutics, and novel diagnostics delivered via flexible routes including mass campaigns, screen and treat, and targeted outreach.
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
-**WARNING! This library is in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used and any results produced using it will be invalid.** 
-
-
 Installation
 ------------
 
 To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
 
 
 Usage and documentation
 -----------------------
 
-Documentation is not yet available. Usage examples are available in the ``tests`` folder.
+Documentation is available at https://docs.starsim.org. 
+
+Usage examples are available in the ``tests`` folder.
 
 
 Contributing
 ------------
 
 If you wish to contribute, please see the code of conduct and contributing documents.
```

### Comparing `starsim-0.1.5/README.rst` & `starsim-0.3.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Starsim
 =======
 
+**Warning! Starsim is still in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used for real research or policy questions.**
+
 Starsim is an agent-based disease modeling framework in which users can design and configure simulations of pathogens that progress over time within each agent and pass from one agent to the next along dynamic transmission networks. The framework explicitly supports co-transmission of multiple pathogens, allowing users to concurrently simulate several diseases while capturing behavioral and biological interactions. Non-communicable diseases can easily be included as well, either as a co-factor for transmissible pathogens or as an independent exploration. Detailed modeling of mother-child relationships can be simulated from the timepoint of conception, enabling study of congenital diseases and associated birth outcomes. Finally, Starsim facilitates the comparison of one or more intervention scenarios to a baseline scenario in evaluating the impact of various products like vaccines, therapeutics, and novel diagnostics delivered via flexible routes including mass campaigns, screen and treat, and targeted outreach.
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
-**WARNING! This library is in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used and any results produced using it will be invalid.** 
-
-
 Installation
 ------------
 
 To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
 
 
 Usage and documentation
 -----------------------
 
-Documentation is not yet available. Usage examples are available in the ``tests`` folder.
+Documentation is available at https://docs.starsim.org. 
+
+Usage examples are available in the ``tests`` folder.
 
 
 Contributing
 ------------
 
 If you wish to contribute, please see the code of conduct and contributing documents.
```

### Comparing `starsim-0.1.5/setup.py` & `starsim-0.3.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,35 +15,35 @@
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Development Status :: 5 - Production/Stable",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 setup(
     name="starsim",
     version=version,
-    author="Robyn Stuart, Romesh Abeysuriya, Jamie Cohen, Cliff Kerr, Daniel Klein",
+    author="Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective",
     description="Starsim",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     keywords=["agent-based model", "simulation", "disease", "epidemiology"],
     platforms=["OS Independent"],
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     include_package_data=True,
-    install_requires=[
+    install_requires=[ # NB: remember to update __init__.py if these requirements change
         'numpy',
         'scipy',
         'pandas>=2.0.0',
-        'sciris>=3.0.0',
+        'sciris>=3.1.6',
         'matplotlib',
-        'seaborn',
         'numba',
         'networkx',
     ],
 )
```

### Comparing `starsim-0.1.5/starsim/connectors.py` & `starsim-0.3.2/starsim/connectors.py`

 * *Files identical despite different names*

### Comparing `starsim-0.1.5/starsim/demographics.py` & `starsim-0.3.2/starsim/demographics.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 Define pregnancy, deaths, migration, etc.
 """
 
 import numpy as np
 import starsim as ss
 import sciris as sc
 import pandas as pd
-import scipy.stats as sps
 
-__all__ = ['DemographicModule', 'births', 'background_deaths', 'Pregnancy']
+__all__ = ['Demographics', 'Births', 'Deaths', 'Pregnancy']
 
 
-class DemographicModule(ss.Module):
+class Demographics(ss.Module):
     # A demographic module typically handles births/deaths/migration and takes
     # place at the start of the timestep, before networks are updated and before
     # any disease modules are executed
 
     def initialize(self, sim):
         super().initialize(sim)
         self.init_results(sim)
@@ -25,29 +24,30 @@
         pass
 
     def update(self, sim):
         # Note that for demographic modules, any result updates should be
         # carried out inside this function
         pass
 
-class births(DemographicModule):
-    def __init__(self, pars=None, metadata=None):
-        super().__init__(pars)
+
+class Births(Demographics):
+    def __init__(self, pars=None, metadata=None, **kwargs):
+        super().__init__(pars, **kwargs)
 
         # Set defaults
-        self.pars = ss.omerge({
-            'birth_rate': 0,
-            'rel_birth': 1,
-            'units': 1e-3  # assumes birth rates are per 1000. If using percentages, switch this to 1
-        }, self.pars)
+        self.pars = ss.omergeleft(self.pars,
+            birth_rate = 0,
+            rel_birth = 1,
+            units = 1e-3,  # assumes birth rates are per 1000. If using percentages, switch this to 1
+        )
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omerge({
-            'data_cols': {'year': 'Year', 'cbr': 'CBR'},
-        }, metadata)
+        self.metadata = ss.omergeleft(metadata,
+            data_cols = dict(year='Year', cbr='CBR'),
+        )
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
         self.pars.birth_rate = self.standardize_birth_data()
         return
 
     def initialize(self, sim):
@@ -61,17 +61,19 @@
 
     def standardize_birth_data(self):
         """ Standardize/validate birth rates - handled in an external file due to shared functionality """
         birth_rate = ss.standardize_data(data=self.pars.birth_rate, metadata=self.metadata)
         return birth_rate
 
     def init_results(self, sim):
-        self.results += ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False)
+        self.results += [
+            ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False),
+        ]
         return
 
     def update(self, sim):
         new_uids = self.add_births(sim)
         self.update_results(len(new_uids), sim)
         return new_uids
 
@@ -83,15 +85,15 @@
         if sc.isnumber(p.birth_rate):
             this_birth_rate = p.birth_rate
         elif sc.checktype(p.birth_rate, 'arraylike'):
             this_birth_rate = p.birth_rate[sim.ti]
 
         scaled_birth_prob = this_birth_rate * p.units * p.rel_birth * sim.pars.dt
         scaled_birth_prob = np.clip(scaled_birth_prob, a_min=0, a_max=1)
-        n_new = int(np.floor(np.count_nonzero(sim.people.alive) * scaled_birth_prob))
+        n_new = int(np.floor(sim.people.alive.count() * scaled_birth_prob))
         return n_new
 
     def add_births(self, sim):
         # Add n_new births to each state in the sim
         n_new = self.get_births(sim)
         new_uids = sim.people.grow(n_new)
         sim.people.age[new_uids] = 0
@@ -102,16 +104,16 @@
 
     def finalize(self, sim):
         super().finalize(sim)
         self.results['cumulative'] = np.cumsum(self.results['new'])
         self.results['cbr'] = 1/self.pars.units*np.divide(self.results['new'], sim.results['n_alive'], where=sim.results['n_alive']>0)
 
 
-class background_deaths(DemographicModule):
-    def __init__(self, pars=None, metadata=None):
+class Deaths(Demographics):
+    def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
         """
         Configure disease-independent "background" deaths.
 
         The probability of death for each agent on each timestep is determined
         by the `death_rate` parameter and the time step. The default value of
         this parameter is 0.02, indicating that all agents will
         face a 2% chance of death per year.
@@ -120,76 +122,81 @@
         for the `death_rate` parameter, to allow it to vary by year, sex, and
         age.  The separate 'metadata' argument can be used to configure the
         details of the input datafile.
 
         Alternatively, it is possible to override the `death_rate` parameter
         with a bernoulli distribution containing a constant value of function of
         your own design.
-        
-        :param pars: dict with arguments including:
-            rel_death: constant used to scale all death rates
-            death_rate: float, dict, or pandas dataframe/series containing mortality data
-            units: units for death rates (see in-line comment on par dict below)
-
-        :param metadata: data about the data contained within the data input.
-            "data_cols" is is a dictionary mapping standard keys, like "year" to the
-            corresponding column name in data. Similar for "sex_keys". Finally,
-        """
-        super().__init__(pars)
-
-        self.pars = ss.omerge({
-            'rel_death': 1,
-            'death_rate': 0.02,  # Default = a fixed rate of 2%/year, overwritten if data provided
-            'units': 1,  # units for death rates. If using percentages, leave as 1. If using a CMR (e.g. 12 deaths per 1000), change to 1/1000
-        }, self.pars)
+
+        Args:
+            pars: dict with arguments including:
+                rel_death: constant used to scale all death rates
+                death_rate: float, dict, or pandas dataframe/series containing mortality data
+                units: units for death rates (see in-line comment on par dict below)
+
+            par_dists: dict
+
+            metadata: data about the data contained within the data input.
+                "data_cols" is is a dictionary mapping standard keys, like "year" to the
+                corresponding column name in data. Similar for "sex_keys". Finally,
+        """
+        super().__init__(pars, **kwargs)
+
+        self.pars = ss.omergeleft(self.pars,
+            rel_death = 1,
+            death_rate = 20,  # Default = a fixed rate of 2%/year, overwritten if data provided
+            units = 1e-3,  # assumes death rates are per 1000. If using percentages, switch this to 1
+        )
+
+        self.par_dists = ss.omergeleft(par_dists,
+            death_rate = ss.bernoulli
+        )
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omerge({
-            'data_cols': {'year': 'Time', 'sex': 'Sex', 'age': 'AgeGrpStart', 'value': 'mx'},
-            'sex_keys': {'f': 'Female', 'm': 'Male'},
-        }, metadata)
+        self.metadata = ss.omergeleft(metadata,
+            data_cols = dict(year='Time', sex='Sex', age='AgeGrpStart', value='mx'),
+            sex_keys = dict(f='Female', m='Male'),
+        )
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
-        self.pars.death_rate = self.standardize_death_data()
-
-        # Create death_prob_fn, a function which returns a probability of death for each requested uid
-        self.death_prob_fn = self.make_death_prob_fn
-        self.death_dist = sps.bernoulli(p=self.death_prob_fn)
+        self.death_rate_data = self.standardize_death_data()
+        self.pars.death_rate = self.make_death_prob_fn
 
         return
 
     @staticmethod
     def make_death_prob_fn(module, sim, uids):
         """ Take in the module, sim, and uids, and return the probability of death for each UID on this timestep """
 
-        if sc.isnumber(module.pars.death_rate):
-            death_rate = module.pars.death_rate
+        if sc.isnumber(module.death_rate_data):
+            death_rate = module.death_rate_data
 
         else:
-            year_label = module.metadata.data_cols['year']
-            age_label = module.metadata.data_cols['age']
-            sex_label = module.metadata.data_cols['sex']
-            val_label = module.metadata.data_cols['value']
+            data_cols = sc.objdict(module.metadata.data_cols)
+            year_label = data_cols.year
+            age_label  = data_cols.age
+            sex_label  = data_cols.sex
+            val_label  = data_cols.value
             sex_keys = module.metadata.sex_keys
 
-            available_years = module.pars.death_rate[year_label].unique()
+            available_years = module.death_rate_data[year_label].unique()
             year_ind = sc.findnearest(available_years, sim.year)
             nearest_year = available_years[year_ind]
 
-            df = module.pars.death_rate.loc[module.pars.death_rate[year_label] == nearest_year]
+            df = module.death_rate_data.loc[module.death_rate_data[year_label] == nearest_year]
             age_bins = df[age_label].unique()
             age_inds = np.digitize(sim.people.age[uids], age_bins) - 1
 
             f_arr = df[val_label].loc[df[sex_label] == sex_keys['f']].values
             m_arr = df[val_label].loc[df[sex_label] == sex_keys['m']].values
 
             # Initialize
             death_rate_df = pd.Series(index=uids)
-            death_rate_df[uids[sim.people.female[uids]]] = f_arr[age_inds[sim.people.female[uids]]]
+            death_rate_df[uids[sim.people.female[uids]]] = f_arr[age_inds[sim.people.female[uids]]] # TODO: avoid double indexing
             death_rate_df[uids[sim.people.male[uids]]] = m_arr[age_inds[sim.people.male[uids]]]
             death_rate_df[uids[sim.people.age[uids] < 0]] = 0  # Don't use background death rates for unborn babies
 
             death_rate = death_rate_df.values
 
         # Scale from rate to probability. Consider an exponential here.
         death_prob = death_rate * (module.pars.units * module.pars.rel_death * sim.pars.dt)
@@ -199,113 +206,118 @@
 
     def standardize_death_data(self):
         """ Standardize/validate death rates - handled in an external file due to shared functionality """
         death_rate = ss.standardize_data(data=self.pars.death_rate, metadata=self.metadata)
         return death_rate
 
     def init_results(self, sim):
-        self.results += ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'cmr', sim.npts, dtype=int, scale=False)
+        self.results += [
+            ss.Result(self.name, 'new', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cumulative', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cmr', sim.npts, dtype=int, scale=False),
+        ]
         return
 
     def update(self, sim):
         n_deaths = self.apply_deaths(sim)
         self.update_results(n_deaths, sim)
         return
 
     def apply_deaths(self, sim):
         """ Select people to die """
         alive_uids = ss.true(sim.people.alive)
-        death_uids = self.death_dist.filter(alive_uids)
+        death_uids = self.pars.death_rate.filter(alive_uids)
         sim.people.request_death(death_uids)
         return len(death_uids)
 
     def update_results(self, n_deaths, sim):
         self.results['new'][sim.ti] = n_deaths
+        return
 
     def finalize(self, sim):
         super().finalize(sim)
         self.results['cumulative'] = np.cumsum(self.results['new'])
         self.results['cmr'] = 1/self.pars.units*np.divide(self.results['new'], sim.results['n_alive'], where=sim.results['n_alive']>0)
+        return
 
 
-class Pregnancy(DemographicModule):
+class Pregnancy(Demographics):
 
-    def __init__(self, pars=None, metadata=None):
-        super().__init__(pars)
+    def __init__(self, pars=None, par_dists=None, metadata=None, **kwargs):
+        super().__init__(pars, **kwargs)
 
         # Other, e.g. postpartum, on contraception...
-        self.infertile = ss.State('infertile', bool, False)  # Applies to girls and women outside the fertility window
-        self.susceptible = ss.State('fecund', bool, True)  # Applies to girls and women inside the fertility window
-        self.pregnant = ss.State('pregnant', bool, False)  # Currently pregnant
-        self.postpartum = ss.State('postpartum', bool, False)  # Currently post-partum
-        self.ti_pregnant = ss.State('ti_pregnant', int, ss.INT_NAN)  # Time pregnancy begins
-        self.ti_delivery = ss.State('ti_delivery', int, ss.INT_NAN)  # Time of delivery
-        self.ti_postpartum = ss.State('ti_postpartum', int, ss.INT_NAN)  # Time postpartum ends
-        self.ti_dead = ss.State('ti_dead', int, ss.INT_NAN)  # Maternal mortality
-        self.conception_probs = ss.State('conception_probs', float, 0)
-
-        self.pars = ss.omerge({
-            'dur_pregnancy': 0.75,  # Make this a distribution?
-            'dur_postpartum': 0.5,  # Make this a distribution?
-            'fertility_rate': 0,    # Usually this will be provided in CSV format
-            'rel_fertility': 1,
-            'maternal_death_rate': 0,
-            'sex_ratio': 0.5,       # Ratio of babies born female
-            'units': 1e-3,          # Assumes fertility rates are per 1000. If using percentages, switch this to 1
-        }, self.pars)
+        self.add_states(
+            ss.State('infertile', bool, False),  # Applies to girls and women outside the fertility window
+            ss.State('fecund', bool, True),  # Applies to girls and women inside the fertility window
+            ss.State('pregnant', bool, False),  # Currently pregnant
+            ss.State('postpartum', bool, False),  # Currently post-partum
+            ss.State('ti_pregnant', int, ss.INT_NAN),  # Time pregnancy begins
+            ss.State('ti_delivery', int, ss.INT_NAN),  # Time of delivery
+            ss.State('ti_postpartum', int, ss.INT_NAN),  # Time postpartum ends
+            ss.State('ti_dead', int, ss.INT_NAN),  # Maternal mortality
+        )
+
+        self.pars = ss.omergeleft(self.pars,
+            dur_pregnancy = 0.75,
+            dur_postpartum = 0.5,
+            fertility_rate = 0,    # Usually this will be provided in CSV format
+            rel_fertility = 1,
+            maternal_death_rate = 0,
+            sex_ratio = 0.5,       # Ratio of babies born female
+            units = 1e-3,          # Assumes fertility rates are per 1000. If using percentages, switch this to 1
+        )
+
+        self.par_dists = ss.omergeleft(par_dists,
+            fertility_rate = ss.bernoulli,
+            maternal_death_rate = ss.bernoulli,
+            sex_ratio = ss.bernoulli
+        )
 
         # Process metadata. Defaults here are the labels used by UN data
-        self.metadata = ss.omerge({
-            'data_cols': {'year': 'Time', 'age': 'AgeGrp', 'value': 'ASFR'},
-        }, metadata)
+        self.metadata = ss.omergeleft(metadata,
+            data_cols = dict(year='Time', age='AgeGrp', value='ASFR'),
+        )
 
-        self.choose_slots = sps.randint(low=0, high=1) # Low and high will be reset upon initialization
+        self.choose_slots = ss.randint() # Low and high will be reset upon initialization
 
         # Process data, which may be provided as a number, dict, dataframe, or series
         # If it's a number it's left as-is; otherwise it's converted to a dataframe
-        self.pars.fertility_rate = self.standardize_fertility_data()
-
-        # Create fertility_prob_fn, a function which returns a probability of death for each requested uid
-        self.fertility_prob_fn = self.make_fertility_prob_fn
-        self.fertility_dist = sps.bernoulli(p=self.fertility_prob_fn)
-
-        # Add other sampling functions
-        self.sex_dist = sps.bernoulli(p=self.pars.sex_ratio)
-        self.death_dist = sps.bernoulli(p=self.pars.maternal_death_rate)
+        self.fertility_rate_data = self.standardize_fertility_data()
+        self.pars.fertility_rate = self.make_fertility_prob_fn
 
         return
 
     @staticmethod
     def make_fertility_prob_fn(module, sim, uids):
         """ Take in the module, sim, and uids, and return the conception probability for each UID on this timestep """
 
-        if sc.isnumber(module.pars.fertility_rate):
-            fertility_rate = module.pars.fertility_rate
+        if sc.isnumber(module.fertility_rate_data):
+            fertility_rate = module.fertility_rate_data
 
         else:
             # Abbreviate key variables
-            year_label = module.metadata.data_cols['year']
-            age_label = module.metadata.data_cols['age']
-            val_label = module.metadata.data_cols['value']
+            data_cols = sc.objdict(module.metadata.data_cols)
+            year_label = data_cols.year
+            age_label  = data_cols.age
+            val_label  = data_cols.value
 
-            available_years = module.pars.fertility_rate[year_label].unique()
+            available_years = module.fertility_rate_data[year_label].unique()
             year_ind = sc.findnearest(available_years, sim.year-module.pars.dur_pregnancy)
             nearest_year = available_years[year_ind]
 
-            df = module.pars.fertility_rate.loc[module.pars.fertility_rate[year_label] == nearest_year]
+            df = module.fertility_rate_data.loc[module.fertility_rate_data[year_label] == nearest_year]
             df_arr = df[val_label].values  # Pull out dataframe values
             df_arr = np.append(df_arr, 0)  # Add zeros for those outside data range
 
             # Process age data
             age_bins = df[age_label].unique()
-            age_bins = np.append(age_bins, 50)
+            age_bins = np.append(age_bins, age_bins[-1]+1) # WARNING: Assumes one year age bins! TODO: More robust handling.
             age_inds = np.digitize(sim.people.age[uids], age_bins) - 1
-            age_inds[age_inds >= max(age_inds)] = -1  # This ensures women outside the data range will get a value of 0
+            age_inds[age_inds == len(age_bins)-1] = -1  # This ensures women outside the data range will get a value of 0
 
             # Adjust rates: rates are based on the entire population, but we need to remove
             # anyone already pregnant and then inflate the rates for the remainder
             pregnant_uids = ss.true(module.pregnant[uids])  # Find agents who are already pregnant
             pregnant_age_counts, _ = np.histogram(sim.people.age[pregnant_uids], age_bins)  # Count them by age
             age_counts, _ = np.histogram(sim.people.age[uids], age_bins)  # Count overall number per age bin
             new_denom = age_counts - pregnant_age_counts  # New denominator for rates
@@ -328,27 +340,30 @@
     def standardize_fertility_data(self):
         """ Standardize/validate fertility rates - handled in an external file due to shared functionality """
         fertility_rate = ss.standardize_data(data=self.pars.fertility_rate, metadata=self.metadata)
         return fertility_rate
 
     def initialize(self, sim):
         super().initialize(sim)
-        self.choose_slots.kwds['low'] = sim.pars['n_agents']+1
-        self.choose_slots.kwds['high'] = int(sim.pars['slot_scale']*sim.pars['n_agents'])
+        low = sim.pars.n_agents + 1
+        high = int(sim.pars.slot_scale*sim.pars.n_agents)
+        self.choose_slots.set(low=low, high=high)
         return
 
     def init_results(self, sim):
         """
         Results could include a range of birth outcomes e.g. LGA, stillbirths, etc.
         Still unclear whether this logic should live in the pregnancy module, the
         individual disease modules, the connectors, or the sim.
         """
-        self.results += ss.Result(self.name, 'pregnancies', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'births', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False)
+        self.results += [
+            ss.Result(self.name, 'pregnancies', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'births', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cbr', sim.npts, dtype=int, scale=False),
+        ]
         return
 
     def update(self, sim):
         """
         Perform all updates
         """
         self.update_states(sim)
@@ -362,20 +377,20 @@
         Update states
         """
 
         # Check for new deliveries
         deliveries = self.pregnant & (self.ti_delivery <= sim.ti)
         self.pregnant[deliveries] = False
         self.postpartum[deliveries] = True
-        self.susceptible[deliveries] = False
+        self.fecund[deliveries] = False
 
         # Check for new women emerging from post-partum
         postpartum = ~self.pregnant & (self.ti_postpartum <= sim.ti)
         self.postpartum[postpartum] = False
-        self.susceptible[postpartum] = True
+        self.fecund[postpartum] = True
 
         # Maternal deaths
         maternal_deaths = ss.true(self.ti_dead <= sim.ti)
         sim.people.request_death(maternal_deaths)
 
         return
 
@@ -386,15 +401,15 @@
         # Abbreviate
         ppl = sim.people
 
         # People eligible to become pregnant. We don't remove pregnant people here, these
         # are instead handled in the fertility_dist logic as the rates need to be adjusted
         denom_conds = ppl.female & ppl.alive
         inds_to_choose_from = ss.true(denom_conds)
-        conceive_uids = self.fertility_dist.filter(inds_to_choose_from)
+        conceive_uids = self.pars.fertility_rate.filter(inds_to_choose_from)
 
         # Set prognoses for the pregnancies
         if len(conceive_uids) > 0:
             self.set_prognoses(sim, conceive_uids)
 
         return conceive_uids
 
@@ -403,23 +418,23 @@
         n_unborn_agents = len(conceive_uids)
         if n_unborn_agents > 0:
 
             # Choose slots for the unborn agents
             new_slots = self.choose_slots.rvs(conceive_uids)
 
             # Grow the arrays and set properties for the unborn agents
-            new_uids = sim.people.grow(len(new_slots))
+            new_uids = sim.people.grow(len(new_slots), new_slots)
             sim.people.age[new_uids] = -self.pars.dur_pregnancy
             sim.people.slot[new_uids] = new_slots  # Before sampling female_dist
-            sim.people.female[new_uids] = self.sex_dist.rvs(new_uids)
+            sim.people.female[new_uids] = self.pars.sex_ratio.rvs(new_uids)
 
             # Add connections to any vertical transmission layers
             # Placeholder code to be moved / refactored. The maternal network may need to be
             # handled separately to the sexual networks, TBC how to handle this most elegantly
-            for lkey, layer in sim.people.networks.items():
+            for lkey, layer in sim.networks.items():
                 if layer.vertical:  # What happens if there's more than one vertical layer?
                     durs = np.full(n_unborn_agents, fill_value=self.pars.dur_pregnancy + self.pars.dur_postpartum)
                     layer.add_pairs(conceive_uids, new_uids, dur=durs)
 
         return
 
     def set_prognoses(self, sim, uids):
@@ -427,26 +442,26 @@
         Make pregnancies
         Add miscarriage/termination logic here
         Also reconciliation with birth rates
         Q, is this also a good place to check for other conditions and set prognoses for the fetus?
         """
 
         # Change states for the newly pregnant woman
-        self.susceptible[uids] = False
+        self.fecund[uids] = False
         self.pregnant[uids] = True
         self.ti_pregnant[uids] = sim.ti
 
         # Outcomes for pregnancies
         dur = np.full(len(uids), sim.ti + self.pars.dur_pregnancy / sim.dt)
-        dead = self.death_dist.rvs(uids)
+        dead = self.pars.maternal_death_rate.rvs(uids)
         self.ti_delivery[uids] = dur  # Currently assumes maternal deaths still result in a live baby
         dur_post_partum = np.full(len(uids), dur + self.pars.dur_postpartum / sim.dt)
         self.ti_postpartum[uids] = dur_post_partum
 
-        if np.count_nonzero(dead):
+        if np.any(dead): # NB: 100x faster than np.sum(), 10x faster than np.count_nonzero()
             self.ti_dead[uids[dead]] = dur[dead]
         return
 
     def update_results(self, sim):
         self.results['pregnancies'][sim.ti] = np.count_nonzero(self.ti_pregnant == sim.ti)
         self.results['births'][sim.ti] = np.count_nonzero(self.ti_delivery == sim.ti)
         return
```

### Comparing `starsim-0.1.5/starsim/diseases/disease.py` & `starsim-0.3.2/starsim/disease.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,120 +1,37 @@
 """
 Base classes for diseases
 """
 
 import numpy as np
 import sciris as sc
 import starsim as ss
-import scipy.stats as sps
 import networkx as nx
 from operator import itemgetter
 import pandas as pd
 
-__all__ = ['InfectionLog', 'Disease', 'STI']
-
-class InfectionLog(nx.MultiDiGraph):
-    """
-    Record infections
-
-    The infection log records transmission events and optionally other data
-    associated with each transmission. Basic functionality is to track
-    transmission with
-
-    >>> Disease.log.append(source, target, t)
-
-    Seed infections can be recorded with a source of `None`, although all infections
-    should have a target and a time. Other data can be captured in the log, either at
-    the time of creation, or later on. For example
-
-    >>> Disease.log.append(source, target, t, network='msm')
-
-    could be used by a module to track the network in which transmission took place.
-    Modules can optionally add per-infection outcomes later as well, for example
-
-    >>> Disease.log.add_data(source, t_dead=2024.25)
-
-    This would be equivalent to having specified the data at the original time the log
-    entry was created - however, it is more useful for tracking events that may or may
-    not occur after the infection and could be modified by interventions (e.g., tracking
-    diagnosis, treatment, notification etc.)
-
-    A table of outcomes can be returned using `InfectionLog.line_list()`
-    """
-    # Add entries
-    # Add items to the most recent infection for an agent
-
-    def add_data(self, uids, **kwargs):
-        """
-        Record extra infection data
-
-        This method can be used to add data to an existing transmission event.
-        The most recent transmission event will be used
-
-        :param uid: The UID of the target node (the agent that was infected)
-        :param kwargs: Remaining arguments are stored as edge data
-        """
-        for uid in sc.promotetoarray(uids):
-            source, target, key = max(self.in_edges(uid, keys=True), key=itemgetter(2,0)) # itemgetter twice as fast as lambda apparently
-            self[source][target][key].update(**kwargs)
-
-    def append(self, source, target, t, **kwargs):
-        self.add_edge(source, target, key=t, **kwargs)
-
-    @property
-    def line_list(self):
-        """
-        Return a tabular representation of the log
-
-        This function returns a dataframe containing columns for all quantities
-        recorded in the log. Note that the log will contain `NaN` for quantities
-        that are defined for some edges and not others (and which are missing for
-        a particular entry)
-        """
-        if len(self) == 0:
-            return pd.DataFrame(columns=['t','source','target'])
-
-        entries = []
-        for source, target, t, data in self.edges(keys=True, data=True):
-            d = data.copy()
-            d.update(source=source, target=target, t=t)
-            entries.append(d)
-        df = pd.DataFrame.from_records(entries)
-        df = df.sort_values(['t','source','target'])
-        df = df.reset_index(drop=True)
-
-        # Use Pandas "Int64" type to allow nullable integers. This allows the 'source' column
-        # to have an integer type corresponding to UIDs while simultaneously supporting the use
-        # of null values to represent exogenous/seed infections
-        df = df.fillna(pd.NA)
-        df['source'] = df['source'].astype("Int64")
-        df['target'] = df['target'].astype("Int64")
-
-        return df
+__all__ = ['Disease', 'Infection', 'InfectionLog']
 
 
 class Disease(ss.Module):
     """ Base module class for diseases """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.results = ss.ndict(type=ss.Result)
-        self.log = InfectionLog()
-        self.new_cases_RNG = ss.MultiRNG(name=f'New cases of {self.name}')
+        self.results = ss.Results(self.name)
+        self.log = InfectionLog()  # See below for definition
         return
 
     @property
     def _boolean_states(self):
         """
         Iterator over states with boolean type
 
         For diseases, these states typically represent attributes like 'susceptible',
         'infectious', 'diagnosed' etc. These variables are typically useful to
-
-        :return:
         """
         for state in self.states:
             if state.dtype == bool:
                 yield state
         return
 
     def initialize(self, sim):
@@ -127,19 +44,34 @@
     def finalize(self, sim):
         super().finalize(sim)
         return
 
     def validate_pars(self, sim):
         """
         Perform any parameter validation
-
-        :return: None if parameters are all valid
-        :raises: Exception if there are any invalid parameters (or if the initialization is otherwise invalid in some way)
         """
-        pass
+        if sim.networks is not None and len(sim.networks) > 0:
+
+            # If there's no beta, make a default one
+            if 'beta' not in self.pars or self.pars.beta is None:
+                self.pars.beta = sc.objdict({k: [1, 1] for k in sim.networks})
+                msg = f'Beta not supplied for disease "{self.name}"; defaulting to 1'
+                ss.warn(msg)
+
+            # If beta is a scalar, apply this bi-directionally to all networks
+            if sc.isnumber(self.pars.beta):
+                orig_beta = self.pars.beta
+                self.pars.beta = sc.objdict({k: [orig_beta] * 2 for k in sim.networks})
+
+            # If beta is a dict, check all entries are bi-directional
+            elif isinstance(self.pars.beta, dict):
+                for k, v in self.pars.beta.items():
+                    if sc.isnumber(v):
+                        self.pars.beta[k] = [v, v]
+        return
 
     def set_initial_states(self, sim):
         """
         Set initial values for states
 
         This could involve passing in a full set of initial conditions,
         or using init_prev, or other. Note that this is different to initialization of the State objects
@@ -160,17 +92,14 @@
         for state in self._boolean_states:
             self.results += ss.Result(self.name, f'n_{state.name}', sim.npts, dtype=int, scale=True)
         return
 
     def update_pre(self, sim):
         """
         Carry out autonomous updates at the start of the timestep (prior to transmission)
-
-        :param sim:
-        :return:
         """
         pass
 
     def update_death(self, sim, uids):
         """
         Carry out state changes upon death
 
@@ -180,247 +109,304 @@
         upon death (e.g., clearing an `infected` flag) are executed in this function. That also
         allows an intervention to avert a death scheduled on the same timestep, without having
         to undo any state changes that have already been applied (because they only run via this
         function if the death actually occurs).
 
         Depending on the module and the results it produces, it may or may not be necessary
         to implement this.
-
-        :param sim:
-        :param uids:
-        :return:
         """
         pass
 
     def make_new_cases(self, sim):
         """
         Add new cases of the disease
 
         This method is agnostic as to the mechanism by which new cases occur. This
         could be through transmission (parametrized in different ways, which may or
         may not use the contact networks) or it may be based on risk factors/seeding,
         as may be the case for non-communicable diseases.
 
         It is expected that this method will internally call Disease.set_prognoses()
         at some point.
-
         """
         pass
 
-
     def set_prognoses(self, sim, target_uids, source_uids=None):
         """
         Set prognoses upon infection/acquisition
 
         This function assigns state values upon infection or acquisition of
         the disease. It would normally be called somewhere towards the end of
         `Disease.make_new_cases()`. Infections will automatically be added to
         the log as part of this operation.
 
         The from_uids are relevant for infectious diseases, but would be left
         as `None` for NCDs.
 
-        :param sim:
-        :param uids: UIDs for agents to assign disease progoses to
-        :param from_uids: Optionally specify the infecting agent
-        :return:
+        Args:
+            sim (Sim): the STarsim simulation object
+            uids (array): UIDs for agents to assign disease progoses to
+            from_uids (array): Optionally specify the infecting agent
         """
         if source_uids is None:
             for target in target_uids:
                 self.log.append(np.nan, target, sim.year)
         else:
             for target, source in zip(target_uids, source_uids):
                 self.log.append(source, target, sim.year)
-
+        return
 
     def update_results(self, sim):
         """
         Update results
 
         This function is executed after transmission in all modules has been resolved.
         This allows result updates at this point to capture outcomes dependent on multiple
         modules, where relevant.
         """
         for state in self._boolean_states:
             self.results[f'n_{state.name}'][sim.ti] = np.count_nonzero(state & sim.people.alive)
         return
 
 
-
-class STI(Disease):
+class Infection(Disease):
     """
-    Base class for STIs used in STIsim
+    Base class for infectious diseases used in Starsim
 
-    This class contains specializations for STI transmission (i.e., implements network-based
-    transmission with directional beta values) and defines attributes that STIsim connectors
+    This class contains specializations for infectious transmission (i.e., implements network-based
+    transmission with directional beta values) and defines attributes that connectors
     operate on to capture co-infection
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.rel_sus     = ss.State('rel_sus', float, 1)
-        self.rel_sev     = ss.State('rel_sev', float, 1)
-        self.rel_trans   = ss.State('rel_trans', float, 1)
-        self.susceptible = ss.State('susceptible', bool, True)
-        self.infected    = ss.State('infected', bool, False)
-        self.ti_infected = ss.State('ti_infected', int, ss.INT_NAN)
+        self.add_states(
+            ss.State('susceptible', bool, True),
+            ss.State('infected', bool, False),
+            ss.State('rel_sus', float, 1.0),
+            ss.State('rel_trans', float, 1.0),
+            ss.State('ti_infected', int, ss.INT_NAN),
+        )
+
+        self.rng_target = ss.random(name='target')
+        self.rng_source = ss.random(name='source')
+
         return
 
     @property
     def infectious(self):
         """
         Generally defined as an alias for infected, although these may differ in some diseases.
         Transmission comes from infectious people; prevalence estimates may include infected people who don't transmit
         """
         return self.infected
 
-
-    def validate_pars(self, sim):
-        """
-        Perform any parameter validation
-        """
-        super().validate_pars(sim)
-        if 'beta' not in self.pars:
-            self.pars.beta = sc.objdict({k: [1, 1] for k in sim.people.networks})
-        return
-
     def set_initial_states(self, sim):
         """
         Set initial values for states. This could involve passing in a full set of initial conditions,
         or using init_prev, or other. Note that this is different to initialization of the State objects
         i.e., creating their dynamic array, linking them to a People instance. That should have already
         taken place by the time this method is called.
         """
-        if self.pars['seed_infections'] is None:
+        if self.pars.init_prev is None:
             return
 
         alive_uids = ss.true(sim.people.alive)  # Maybe just sim.people.uid?
-        initial_cases = self.pars['seed_infections'].filter(alive_uids)
+        initial_cases = self.pars.init_prev.filter(alive_uids)
         self.set_prognoses(sim, initial_cases)  # TODO: sentinel value to indicate seeds?
         return
 
     def init_results(self, sim):
         """
         Initialize results
         """
         super().init_results(sim)
-        self.results += ss.Result(self.name, 'prevalence', sim.npts, dtype=float, scale=False)
-        self.results += ss.Result(self.name, 'new_infections', sim.npts, dtype=int, scale=True)
-        return
+        self.results += [
+            ss.Result(self.name, 'prevalence', sim.npts, dtype=float, scale=False),
+            ss.Result(self.name, 'new_infections', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'cum_infections', sim.npts, dtype=int, scale=True),
+        ]
+        return
+
+    def _check_betas(self, sim):
+        """ Check that there's a network for each beta key """
+        # Ensure keys are lowercase
+        if isinstance(self.pars.beta, dict): # TODO: check if needed
+            self.pars.beta = {k.lower(): v for k, v in self.pars.beta.items()}
+
+        # Create a mapping between beta and networks, and populate it
+        betapars = self.pars.beta
+        betamap = sc.objdict()
+        netkeys = list(sim.networks.keys())
+        if netkeys: # Skip if no networks
+            for bkey in betapars.keys():
+                orig_bkey = bkey[:]
+                if bkey in netkeys: # TODO: CK: could tidy up logic
+                    betamap[bkey] = betapars[orig_bkey]
+                else:
+                    if 'net' not in bkey:
+                        bkey += 'net'  # Add 'net' suffix if not already there
+                    if bkey in netkeys:
+                        betamap[bkey] = betapars[orig_bkey]
+                    else:
+                        errormsg = f'No network for beta parameter "{bkey}"; your beta should match network keys:\n{sc.newlinejoin(netkeys)}'
+                        raise ValueError(errormsg)
+        return betamap
 
-    def update_pre(self, sim):
+    def make_new_cases(self, sim):
         """
-        Carry out autonomous updates at the start of the timestep (prior to transmission)
-
-        :param sim:
-        :return:
+        Add new cases of module, through transmission, incidence, etc.
+        
+        Common-random-number-safe transmission code works by mapping edges onto
+        slots.
         """
-        pass
-
-    def _make_new_cases_singlerng(self, people):
-        # Not common-random-number-safe, but more efficient for when not using the multirng feature
         new_cases = []
         sources = []
-        for k, layer in people.networks.items():
-            if k in self.pars['beta']:
-                contacts = layer.contacts
-                rel_trans = (self.infectious & people.alive) * self.rel_trans
-                rel_sus = (self.susceptible & people.alive) * self.rel_sus
-                for a, b, beta in [[contacts.p1, contacts.p2, self.pars.beta[k][0]],
-                                   [contacts.p2, contacts.p1, self.pars.beta[k][1]]]:
-                    if beta == 0:
-                        continue
-                    # probability of a->b transmission
-                    p_transmit = rel_trans[a] * rel_sus[b] * contacts.beta * beta * people.dt  # Remove - beta should be per dt
-                    new_cases_bool = np.random.random(len(a)) < p_transmit  # As this class is not common-random-number safe anyway, calling np.random is perfectly fine!
-                    new_cases.append(b[new_cases_bool])
-                    sources.append(a[new_cases_bool])
-        return np.concatenate(new_cases), np.concatenate(sources)
-
-    def _make_new_cases_multirng(self, people):
-        '''
-        Common-random-number-safe transmission code works by computing the
-        probability of each _node_ acquiring a case rather than checking if each
-        _edge_ transmits.
-        Subsequent step uses a roulette wheel with slotted RNG to determine
-        infection source.
-        '''
-        n = len(people.uid)  # TODO: possibly could be shortened to just the people who are alive
-        p_acq_node = np.zeros(n)
-
-        dfs = []
-        for lkey, layer in people.networks.items():
-            if lkey in self.pars['beta']:
-                contacts = layer.contacts
-                rel_trans = self.rel_trans * (self.infectious & people.alive)
-                rel_sus = self.rel_sus * (self.susceptible & people.alive)
-
-                a_to_b = ['p1', 'p2', self.pars.beta[lkey][0]]
-                b_to_a = ['p2', 'p1', self.pars.beta[lkey][1]]
-                for lbl_src, lbl_tgt, beta in [a_to_b, b_to_a]:  # Transmission from a --> b
-                    if beta == 0:
-                        continue
-
-                    a, b = contacts[lbl_src], contacts[lbl_tgt]
-                    df = pd.DataFrame({'p1': a, 'p2': b})
-                    df['p'] = (rel_trans[a] * rel_sus[b] * contacts.beta * beta * people.dt).values
-                    df = df.loc[df['p'] > 0]
-                    dfs.append(df)
-
-        df = pd.concat(dfs)
-        if len(df) == 0:
-            return [], []
-
-        p_acq_node = df.groupby('p2').apply(lambda x: 1 - np.prod(1 - x['p']))
-        uids = p_acq_node.index.values
-
-        # Slotted draw, need to find a long-term place for this logic
-        slots = people.slot[uids]
-        new_cases_bool = sps.uniform.rvs(size=np.max(slots) + 1)[slots] < p_acq_node.values
-        new_cases = uids[new_cases_bool]
-
-        # Now choose infection source for new cases
-        def choose_source(df):
-            if len(df) == 1:  # Easy if only one possible source
-                src_idx = 0
-            else:
-                # Roulette selection using slotted draw r associated with this new case
-                cumsum = df['p'] / df['p'].sum()
-                src_idx = np.argmax(cumsum >= df['r'])
-            return df['p1'].iloc[src_idx]
+        people = sim.people
+        betamap = self._check_betas(sim)
 
-        df['r'] = sps.uniform.rvs(size=np.max(slots) + 1)[slots]
-        sources = df.set_index('p2').loc[new_cases].groupby('p2').apply(choose_source)
-
-        return new_cases, sources[new_cases].values
-
-    def make_new_cases(self, sim):
-        """ Add new cases of module, through transmission, incidence, etc. """
-        if not ss.options.multirng:
-            # Determine new cases for singlerng
-            new_cases, sources = self._make_new_cases_singlerng(sim.people)
+        for nkey,net in sim.networks.items():
+            if not len(net):
+                break
+
+            nbetas = betamap[nkey]
+            contacts = net.contacts
+            rel_trans = (self.infectious & people.alive) * self.rel_trans
+            rel_sus = (self.susceptible & people.alive) * self.rel_sus
+            p1p2b0 = [contacts.p1, contacts.p2, nbetas[0]]
+            p2p1b1 = [contacts.p2, contacts.p1, nbetas[1]]
+            for src, trg, beta in [p1p2b0, p2p1b1]:
+
+                # Skip networks with no transmission
+                if beta == 0:
+                    continue
+
+                # Calculate probability of a->b transmission.
+                beta_per_dt = net.beta_per_dt(disease_beta=beta, dt=people.dt) # TODO: should this be sim.dt?
+                p_transmit = rel_trans[src] * rel_sus[trg] * beta_per_dt
+
+                # Generate a new random number based on the two other random numbers -- 3x faster than `rvs = np.remainder(rvs_s + rvs_t, 1)`
+                rvs_s = self.rng_source.rvs(src)
+                rvs_t = self.rng_target.rvs(trg)
+                rvs = rvs_s + rvs_t
+                inds = np.where(rvs>1.0)[0]
+                rvs[inds] -= 1
+                
+                new_cases_bool = rvs < p_transmit
+                new_cases.append(trg[new_cases_bool])
+                sources.append(src[new_cases_bool])
+                
+        # Tidy up
+        if len(new_cases) and len(sources):
+            new_cases = np.concatenate(new_cases)
+            sources = np.concatenate(sources)
         else:
-            # Determine new cases for multirng
-            new_cases, sources = self._make_new_cases_multirng(sim.people)
-
+            new_cases = np.empty(0, dtype=int)
+            sources = np.empty(0, dtype=int)
+            
         if len(new_cases):
             self._set_cases(sim, new_cases, sources)
+            
+        return new_cases, sources
 
     def _set_cases(self, sim, target_uids, source_uids=None):
-        congenital = sim.people.age[target_uids] <= sim.dt
-        if len(ss.true(congenital))>0:
+        congenital = sim.people.age[target_uids] <= 0
+        if len(ss.true(congenital)) > 0:
             src_c = source_uids[congenital] if source_uids is not None else None
             self.set_congenital(sim, target_uids[congenital], src_c)
         src_p = source_uids[~congenital] if source_uids is not None else None
         self.set_prognoses(sim, target_uids[~congenital], src_p)
         return
 
-    def set_prognoses(self, sim, target_uids, source_uids=None):
-        pass
-
     def set_congenital(self, sim, target_uids, source_uids=None):
         pass
 
     def update_results(self, sim):
         super().update_results(sim)
-        self.results['prevalence'][sim.ti] = self.results.n_infected[sim.ti] / np.count_nonzero(sim.people.alive)
-        self.results['new_infections'][sim.ti] = np.count_nonzero(self.ti_infected == sim.ti)
+        res = self.results
+        ti = sim.ti
+        res.prevalence[ti] = res.n_infected[ti] / np.count_nonzero(sim.people.alive)
+        res.new_infections[ti] = np.count_nonzero(self.ti_infected == ti)
+        res.cum_infections[ti] = np.sum(res['new_infections'][:ti+1])
+        return
+
+
+class InfectionLog(nx.MultiDiGraph):
+    """
+    Record infections
+
+    The infection log records transmission events and optionally other data
+    associated with each transmission. Basic functionality is to track
+    transmission with
+
+    >>> Disease.log.append(source, target, t)
+
+    Seed infections can be recorded with a source of `None`, although all infections
+    should have a target and a time. Other data can be captured in the log, either at
+    the time of creation, or later on. For example
+
+    >>> Disease.log.append(source, target, t, network='msm')
+
+    could be used by a module to track the network in which transmission took place.
+    Modules can optionally add per-infection outcomes later as well, for example
+
+    >>> Disease.log.add_data(source, t_dead=2024.25)
+
+    This would be equivalent to having specified the data at the original time the log
+    entry was created - however, it is more useful for tracking events that may or may
+    not occur after the infection and could be modified by interventions (e.g., tracking
+    diagnosis, treatment, notification etc.)
+
+    A table of outcomes can be returned using `InfectionLog.line_list()`
+    """
+
+    # Add entries
+    # Add items to the most recent infection for an agent
+
+    def add_data(self, uids, **kwargs):
+        """
+        Record extra infection data
+
+        This method can be used to add data to an existing transmission event.
+        The most recent transmission event will be used
+
+        :param uid: The UID of the target node (the agent that was infected)
+        :param kwargs: Remaining arguments are stored as edge data
+        """
+        for uid in sc.promotetoarray(uids):
+            source, target, key = max(self.in_edges(uid, keys=True),
+                                      key=itemgetter(2, 0))  # itemgetter twice as fast as lambda apparently
+            self[source][target][key].update(**kwargs)
+
+    def append(self, source, target, t, **kwargs):
+        self.add_edge(source, target, key=t, **kwargs)
+
+    @property
+    def line_list(self):
+        """
+        Return a tabular representation of the log
+
+        This function returns a dataframe containing columns for all quantities
+        recorded in the log. Note that the log will contain `NaN` for quantities
+        that are defined for some edges and not others (and which are missing for
+        a particular entry)
+        """
+        if len(self) == 0:
+            return sc.dataframe(columns=['t', 'source', 'target'])
+
+        entries = []
+        for source, target, t, data in self.edges(keys=True, data=True):
+            d = data.copy()
+            d.update(source=source, target=target, t=t)
+            entries.append(d)
+        df = sc.dataframe.from_records(entries)
+        df = df.sort_values(['t', 'source', 'target'])
+        df = df.reset_index(drop=True)
+
+        # Use Pandas "Int64" type to allow nullable integers. This allows the 'source' column
+        # to have an integer type corresponding to UIDs while simultaneously supporting the use
+        # of null values to represent exogenous/seed infections
+        df = df.fillna(pd.NA)
+        df['source'] = df['source'].astype("Int64")
+        df['target'] = df['target'].astype("Int64")
+
+        return df
```

### Comparing `starsim-0.1.5/starsim/diseases/gonorrhea.py` & `starsim-0.3.2/starsim/diseases/gonorrhea.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 """
 Define default gonorrhea disease module and related interventions
 """
 
 import numpy as np
 import starsim as ss
-from .disease import STI
-import scipy.stats as sps
-
 
 __all__ = ['Gonorrhea']
 
+class Gonorrhea(ss.Infection):
 
-class Gonorrhea(STI):
-
-    def __init__(self, pars=None):
-        super().__init__(pars)
+    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
 
         # States additional to the default disease states (see base class)
-        self.symptomatic = ss.State('symptomatic', bool, False)
-        self.ti_clearance = ss.State('ti_clearance', int, ss.INT_NAN)
-        self.p_symp = ss.State('p_symp', float, 1)
-
-        # Parameters
-        self.pars = ss.omerge({
-            'dur_inf_in_days': sps.lognorm(s=0.6, scale=10),  # median of 10 days (IQR 7–15 days) https://sti.bmj.com/content/96/8/556
-            'p_symp': sps.bernoulli(p=0.5),  # Share of infections that are symptomatic. Placeholder value
-            'p_clear': sps.bernoulli(p=0.2),  # Share of infections that spontaneously clear: https://sti.bmj.com/content/96/8/556
-            'seed_infections': sps.bernoulli(p=0.1),
-        }, self.pars)
-
         # Additional states dependent on parameter values, e.g. self.p_symp?
         # These might be useful for connectors to target, e.g. if HIV reduces p_clear
+        self.add_states(
+            ss.State('symptomatic', bool, False),
+            ss.State('ti_clearance', int, ss.INT_NAN),
+            ss.State('p_symp', float, 1),
+        )
+
+        # Parameters
+        pars = ss.omergeleft(pars,
+            dur_inf_in_days = ss.lognorm_ex(mean=10, stdev=0.6),  # median of 10 days (IQR 7–15 days) https://sti.bmj.com/content/96/8/556
+            p_symp = 0.5,  # Share of infections that are symptomatic. Placeholder value
+            p_clear = 0.2,  # Share of infections that spontaneously clear: https://sti.bmj.com/content/96/8/556
+            init_prev = 0.1,
+        )
+
+        par_dists = ss.omergeleft(par_dists,
+            dur_inf_in_days = ss.lognorm_ex,
+            p_symp          = ss.bernoulli,
+            p_clear         = ss.bernoulli,
+            init_prev       = ss.bernoulli,
+        )
 
+        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
         return
 
     def init_results(self, sim):
         """
         Initialize results
         """
         super().init_results(sim)
-        self.results += ss.Result(self.name, 'n_symptomatic', sim.npts, dtype=int)
         self.results += ss.Result(self.name, 'new_clearances', sim.npts, dtype=int)
         return
 
     def update_results(self, sim):
+        ti = sim.ti
         super(Gonorrhea, self).update_results(sim)
-        self.results['n_symptomatic'][sim.ti] = np.count_nonzero(self.symptomatic)
-        self.results['new_clearances'][sim.ti] = np.count_nonzero(self.ti_clearance == sim.ti)
+        self.results.n_symptomatic[ti] = self.symptomatic.count()
+        self.results.new_clearances[ti] = np.count_nonzero(self.ti_clearance == ti)
         return
 
     def update_pre(self, sim):
         # What if something in here should depend on another module?
         # I guess we could just check for it e.g., 'if HIV in sim.modules' or
         # 'if 'hiv' in sim.people' or something
         # Natural clearance
@@ -79,14 +83,14 @@
 
         # Set infection status
         symp_uids = self.pars.p_symp.filter(target_uids)
         self.symptomatic[symp_uids] = True
 
         # Set natural clearance
         clear_uids = self.pars.p_clear.filter(target_uids)
-        dur = sim.ti + self.pars['dur_inf_in_days'].rvs(clear_uids)/365/sim.pars.dt # Convert from days to years and then adjust for dt
+        dur = sim.ti + self.pars.dur_inf_in_days.rvs(clear_uids)/365/sim.dt # Convert from days to years and then adjust for dt
         self.ti_clearance[clear_uids] = dur
 
         return
 
     def set_congenital(self, sim, target_uids, source_uids=None):
         pass
```

### Comparing `starsim-0.1.5/starsim/diseases/hiv.py` & `starsim-0.3.2/starsim/diseases/hiv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 """
 Define default HIV disease module and related interventions
 """
 
 import numpy as np
 import sciris as sc
 import starsim as ss
-from .disease import STI
-import scipy.stats as sps
 
 __all__ = ['HIV', 'ART', 'CD4_analyzer']
 
+class HIV(ss.Infection):
 
-class HIV(STI):
+    def __init__(self, pars=None, par_dists=None, *args, **kwargs):
 
-    def __init__(self, pars=None):
-        super().__init__(pars)
-
-        self.on_art      = ss.State('on_art', bool, False)
-        self.ti_art      = ss.State('ti_art', int, ss.INT_NAN)
-        self.cd4         = ss.State('cd4', float, 500)
-        self.ti_dead     = ss.State('ti_dead', int, ss.INT_NAN) # Time of HIV-cause death
-
-        self.death_prob_per_dt = sps.bernoulli(p=self.death_prob)
-
-        self.pars = ss.omerge({
-            'cd4_min': 100,
-            'cd4_max': 500,
-            'cd4_rate': 5,
-            'seed_infections': sps.bernoulli(p=0.05),
-            'eff_condoms': 0.7,
-            'art_efficacy': 0.96,
-        }, self.pars)
+        # States
+        self.add_states(
+            ss.State('on_art', bool, False),
+            ss.State('ti_art', int, ss.INT_NAN),
+            ss.State('cd4', float, 500),
+            ss.State('ti_dead', int, ss.INT_NAN), # Time of HIV-cause death
+        )
+
+        pars = ss.omergeleft(pars,
+            cd4_min = 100,
+            cd4_max = 500,
+            cd4_rate = 5,
+            init_prev = 0.05,
+            eff_condoms = 0.7,
+            art_efficacy = 0.96,
+            death_prob = 0.05,
+        )
+
+        par_dists = ss.omergeleft(par_dists,
+            init_prev  = ss.bernoulli,
+            death_prob = ss.bernoulli,
+        )
+
+        super().__init__(pars=pars, par_dists=par_dists, *args, **kwargs)
+        self.death_prob_data = sc.dcp(self.pars.death_prob)
+        self.pars.death_prob = self.make_death_prob
 
         return
 
     @staticmethod
-    def death_prob(self, sim, uids):
-        return 0.05 / (self.pars.cd4_min - self.pars.cd4_max)**2 *  (self.cd4[uids] - self.pars.cd4_max)**2
+    def make_death_prob(module, sim, uids):
+        p = module.pars
+        out = sim.dt * module.death_prob_data / (p.cd4_min - p.cd4_max)**2 *  (module.cd4[uids] - p.cd4_max)**2
+        out = np.array(out)
+        return out
 
     def update_pre(self, sim):
         """ Update CD4 """
         self.cd4[sim.people.alive & self.infected & self.on_art] += (self.pars.cd4_max - self.cd4[sim.people.alive & self.infected & self.on_art])/self.pars.cd4_rate
         self.cd4[sim.people.alive & self.infected & ~self.on_art] += (self.pars.cd4_min - self.cd4[sim.people.alive & self.infected & ~self.on_art])/self.pars.cd4_rate
 
         self.rel_trans[sim.people.alive & self.infected & self.on_art] = 1 - self.pars['art_efficacy']
 
         can_die = ss.true(sim.people.alive & sim.people.hiv.infected)
-        hiv_deaths = self.death_prob_per_dt.filter(can_die)
+        hiv_deaths = self.pars.death_prob.filter(can_die)
         
         sim.people.request_death(hiv_deaths)
         self.ti_dead[hiv_deaths] = sim.ti
         return
 
     def init_results(self, sim):
         """
         Initialize results
         """
         super().init_results(sim)
         self.results += ss.Result(self.name, 'new_deaths', sim.npts, dtype=int)
         return
 
     def update_results(self, sim):
-        super(HIV, self).update_results(sim)
+        super().update_results(sim)
         self.results['new_deaths'][sim.ti] = np.count_nonzero(self.ti_dead == sim.ti)
         return 
 
     def make_new_cases(self, sim):
         # eff_condoms = sim.pars[self.name]['eff_condoms'] # TODO figure out how to add this
         super().make_new_cases(sim)
         return
@@ -82,32 +92,32 @@
         return self.set_prognoses(sim, target_uids, source_uids)
 
 
 # %% HIV-related interventions
 
 class ART(ss.Intervention):
 
-    def __init__(self, t: np.array, coverage: np.array, **kwargs):
+    def __init__(self, year: np.array, coverage: np.array, **kwargs):
         self.requires = HIV
-        self.t = sc.promotetoarray(t)
+        self.year = sc.promotetoarray(year)
         self.coverage = sc.promotetoarray(coverage)
 
         super().__init__(**kwargs)
 
-        self.prob_art_at_infection = sps.bernoulli(p=lambda self, sim, uids: np.interp(sim.year, self.t, self.coverage))
+        self.prob_art_at_infection = ss.bernoulli(p=lambda self, sim, uids: np.interp(sim.year, self.year, self.coverage))
         return
 
     def initialize(self, sim):
         super().initialize(sim)
         self.results += ss.Result(self.name, 'n_art', sim.npts, dtype=int)
         self.initialized = True
         return
 
     def apply(self, sim):
-        if sim.ti < self.t[0]:
+        if sim.year < self.year[0]:
             return
 
         ti_delay = 1 # 1 time step delay TODO
         recently_infected = ss.true((sim.people.hiv.ti_infected == sim.ti-ti_delay) & sim.people.alive)
 
         n_added = 0
         if len(recently_infected) > 0:
```

### Comparing `starsim-0.1.5/starsim/diseases/syphilis.py` & `starsim-0.3.2/starsim/diseases/syphilis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,177 @@
 """
 Define default syphilis disease module
 """
 
 import numpy as np
 import sciris as sc
-import pandas as pd
-from sciris import randround as rr
-import scipy.stats as sps
-
+from sciris import randround as rr # Since used frequently
 import starsim as ss
-from .disease import STI
 
 __all__ = ['Syphilis']
 
-
-class Syphilis(STI):
+class Syphilis(ss.Infection):
 
     def __init__(self, pars=None):
         super().__init__(pars)
 
-        # Adult syphilis states
-        self.adult_states = ['exposed', 'primary', 'secondary', 'latent_temp', 'latent_long', 'tertiary', 'immune']
-        self.exposed = ss.State('exposed', bool, False)  # AKA incubating. Free of symptoms, not transmissible
-        self.primary = ss.State('primary', bool, False)  # Primary chancres
-        self.secondary = ss.State('secondary', bool, False)  # Inclusive of those who may still have primary chancres
-        self.latent_temp = ss.State('latent_temp', bool, False)  # Relapses to secondary (~1y)
-        self.latent_long = ss.State('latent_long', bool, False)  # Can progress to tertiary or remain here
-        self.tertiary = ss.State('tertiary', bool, False)  # Includes complications (cardio/neuro/disfigurement)
-        self.immune = ss.State('immune', bool, False)  # After effective treatment people may acquire temp immunity
-
-        # Congenital syphilis states
-        self.congenital = ss.State('congenital', bool, False)
-
-        # Duration of stages
-        self.dur_exposed = ss.State('dur_exposed', float, np.nan)
-        self.dur_primary = ss.State('dur_primary', float, np.nan)
-        self.dur_secondary = ss.State('dur_secondary', float, np.nan)
-        self.dur_latent_temp = ss.State('dur_latent_temp', float, np.nan)
-        self.dur_latent_long = ss.State('dur_latent_long', float, np.nan)
-        self.dur_tertiary = ss.State('dur_tertiary', float, np.nan)
-        self.dur_infection = ss.State('dur_infection', float, np.nan)  # Sum of all the stages
-
-        # Timestep of state changes
-        self.ti_exposed = ss.State('ti_exposed', int, ss.INT_NAN)
-        self.ti_primary = ss.State('ti_primary', int, ss.INT_NAN)
-        self.ti_secondary = ss.State('ti_secondary', int, ss.INT_NAN)
-        self.ti_latent_temp = ss.State('ti_latent_temp', int, ss.INT_NAN)
-        self.ti_latent_long = ss.State('ti_latent_long', int, ss.INT_NAN)
-        self.ti_tertiary = ss.State('ti_tertiary', int, ss.INT_NAN)
-        self.ti_immune = ss.State('ti_immune', int, ss.INT_NAN)
-        self.ti_miscarriage = ss.State('ti_miscarriage', int, ss.INT_NAN)
-        self.ti_nnd = ss.State('ti_nnd', int, ss.INT_NAN)
-        self.ti_stillborn = ss.State('ti_stillborn', int, ss.INT_NAN)
-        self.ti_congenital = ss.State('ti_congenital', int, ss.INT_NAN)
+        self.add_states(
+            # Adult syphilis states
+            ss.State('exposed', bool, False),  # AKA incubating. Free of symptoms, not transmissible
+            ss.State('primary', bool, False),  # Primary chancres
+            ss.State('secondary', bool, False),  # Inclusive of those who may still have primary chancres
+            ss.State('latent_temp', bool, False),  # Relapses to secondary (~1y)
+            ss.State('latent_long', bool, False),  # Can progress to tertiary or remain here
+            ss.State('tertiary', bool, False),  # Includes complications (cardio/neuro/disfigurement)
+            ss.State('immune', bool, False),  # After effective treatment people may acquire temp immunity
+            ss.State('ever_exposed', bool, False),  # Anyone ever exposed - stays true after treatment
+    
+            # Congenital syphilis states
+            ss.State('congenital', bool, False),
+    
+            # Timestep of state changes
+            ss.State('ti_exposed', int, ss.INT_NAN),
+            ss.State('ti_primary', int, ss.INT_NAN),
+            ss.State('ti_secondary', int, ss.INT_NAN),
+            ss.State('ti_latent_temp', int, ss.INT_NAN),
+            ss.State('ti_latent_long', int, ss.INT_NAN),
+            ss.State('ti_tertiary', int, ss.INT_NAN),
+            ss.State('ti_immune', int, ss.INT_NAN),
+            ss.State('ti_miscarriage', int, ss.INT_NAN),
+            ss.State('ti_nnd', int, ss.INT_NAN),
+            ss.State('ti_stillborn', int, ss.INT_NAN),
+            ss.State('ti_congenital', int, ss.INT_NAN),
+        )
 
         # Parameters
         default_pars = dict(
             # Adult syphilis natural history, all specified in years
-            dur_exposed=ss.lognorm(mean=1 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            dur_primary=ss.lognorm(mean=1.5 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            dur_secondary=sps.norm(loc=3.6 / 12, scale=1.5 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            dur_latent_temp=ss.lognorm(mean=1, stdev=6 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            dur_latent_long=ss.lognorm(mean=20, stdev=8),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            p_latent_temp=sps.bernoulli(p=0.25),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
-            p_tertiary=sps.bernoulli(p=0.35),  # https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4917057/
+            dur_exposed = ss.lognorm_ex(mean=1 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            dur_primary = ss.lognorm_ex(mean=1.5 / 12, stdev=1 / 36),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            dur_secondary = ss.normal(loc=3.6 / 12, scale=1.5 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            dur_latent_temp = ss.lognorm_ex(mean=1, stdev=6 / 12),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            dur_latent_long = ss.lognorm_ex(mean=20, stdev=8),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            p_latent_temp = ss.bernoulli(p=0.25),  # https://pubmed.ncbi.nlm.nih.gov/9101629/
+            p_tertiary = ss.bernoulli(p=0.35),  # https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4917057/
+
+            # Transmission by stage
+            rel_trans = dict(
+                exposed=1,
+                primary=1,
+                secondary=1,
+                latent_temp=0.075,
+                latent_long=0.075,
+                tertiary=0.05,
+            ),
 
             # Congenital syphilis outcomes
             # Birth outcomes coded as:
             #   0: Neonatal death
             #   1: Stillborn
             #   2: Congenital syphilis
             #   3: Live birth without syphilis-related complications
             # Source: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5973824/)
             birth_outcomes=sc.objdict(
-                active=sps.rv_discrete(values=([0, 1, 2, 3, 4], [0.125, 0.125, 0.20, 0.35, 0.200])),
-                latent=sps.rv_discrete(values=([0, 1, 2, 3, 4], [0.050, 0.075, 0.10, 0.05, 0.725])),
+                active = ss.choice(a=5, p=np.array([0.125, 0.125, 0.20, 0.35, 0.200])), # Probabilities of active by birth outcome
+                latent = ss.choice(a=5, p=np.array([0.050, 0.075, 0.10, 0.05, 0.725])), # Probabilities of latent
             ),
             birth_outcome_keys=['miscarriage', 'nnd', 'stillborn', 'congenital'],
 
             # Initial conditions
-            seed_infections=sps.bernoulli(p=0.03),
+            init_prev=ss.bernoulli(p=0.03),
         )
-        self.pars = ss.omerge(default_pars, self.pars)
+        self.pars = ss.omerge(default_pars, self.pars) # NB: regular omerge rather than omergeleft
 
         return
 
     @property
+    def naive(self):
+        """ Never exposed """
+        return ~self.ever_exposed
+
+    @property
+    def sus_not_naive(self):
+        """ Susceptible but with syphilis antibodies, which persist after treatment """
+        return self.susceptible & self.ever_exposed
+
+    @property
     def active(self):
-        """ Active - only active infections can transmit through sexual contact """
+        """ Active infection includes primary and secondary stages """
         return self.primary | self.secondary
 
     @property
     def latent(self):
-        """ Latent """
+        """ Latent infection """
         return self.latent_temp | self.latent_long
 
     @property
     def infectious(self):
-        """ Infectious - includes latent infections, which can transmit vertically but not sexually """
-        return self.active | self.latent
+        """ Infectious """
+        return self.active | self.latent | self.exposed
 
     def init_results(self, sim):
         """ Initialize results """
         super().init_results(sim)
-        self.results += ss.Result(self.name, 'new_nnds', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'new_stillborns', sim.npts, dtype=int, scale=True)
-        self.results += ss.Result(self.name, 'new_congenital', sim.npts, dtype=int, scale=True)
-        return
-
-    def update_results(self, sim):
-        """ Update results """
-        super(Syphilis, self).update_results(sim)
+        self.results += [
+            ss.Result(self.name, 'new_nnds',       sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'new_stillborns', sim.npts, dtype=int, scale=True),
+            ss.Result(self.name, 'new_congenital', sim.npts, dtype=int, scale=True),
+        ]
         return
 
     def update_pre(self, sim):
         """ Updates prior to interventions """
 
         # Primary
         primary = self.exposed & (self.ti_primary <= sim.ti)
         self.primary[primary] = True
         self.exposed[primary] = False
+        self.rel_trans[primary] = self.pars.rel_trans['primary']
 
         # Secondary from primary
         secondary_from_primary = self.primary & (self.ti_secondary <= sim.ti)
-        self.secondary[secondary_from_primary] = True
-        self.primary[secondary_from_primary] = False
-        self.set_secondary_prognoses(sim, ss.true(secondary_from_primary))
+        if len(ss.true(secondary_from_primary)) > 0:
+            self.secondary[secondary_from_primary] = True
+            self.primary[secondary_from_primary] = False
+            self.set_secondary_prognoses(sim, ss.true(secondary_from_primary))
+            self.rel_trans[secondary_from_primary] = self.pars.rel_trans['secondary']
+
+        # Hack to reset the MultiRNGs in set_secondary_prognoses so that they can be called again in this timestep. TODO: Refactor
+        self.pars.p_latent_temp.jump(sim.ti+1)
+        self.pars.dur_secondary.jump(sim.ti+1)
 
         # Secondary reactivation from latent
         secondary_from_latent = self.latent_temp & (self.ti_secondary <= sim.ti)
-        self.secondary[secondary_from_latent] = True
-        self.latent_temp[secondary_from_latent] = False
-        self.set_secondary_prognoses(sim, ss.true(secondary_from_latent))
+        if len(ss.true(secondary_from_latent)) > 0:
+            self.secondary[secondary_from_latent] = True
+            self.latent_temp[secondary_from_latent] = False
+            self.set_secondary_prognoses(sim, ss.true(secondary_from_latent))
+            self.rel_trans[secondary_from_latent] = self.pars.rel_trans['secondary']
 
         # Latent
         latent_temp = self.secondary & (self.ti_latent_temp <= sim.ti)
-        self.latent_temp[latent_temp] = True
-        self.secondary[latent_temp] = False
-        self.set_latent_temp_prognoses(sim, ss.true(latent_temp))
+        if len(ss.true(latent_temp)) > 0:
+            self.latent_temp[latent_temp] = True
+            self.secondary[latent_temp] = False
+            self.set_latent_temp_prognoses(sim, ss.true(latent_temp))
+            self.rel_trans[latent_temp] = self.pars.rel_trans['latent_temp']
 
         # Latent long
         latent_long = self.secondary & (self.ti_latent_long <= sim.ti)
-        self.latent_long[latent_long] = True
-        self.secondary[latent_long] = False
-        self.set_latent_long_prognoses(sim, ss.true(latent_long))
+        if len(ss.true(latent_long)) > 0:
+            self.latent_long[latent_long] = True
+            self.secondary[latent_long] = False
+            self.set_latent_long_prognoses(sim, ss.true(latent_long))
+            self.rel_trans[latent_long] = self.pars.rel_trans['latent_long']
 
         # Tertiary
         tertiary = self.latent_long & (self.ti_tertiary <= sim.ti)
         self.tertiary[tertiary] = True
         self.latent_long[tertiary] = False
+        self.rel_trans[tertiary] = self.pars.rel_trans['tertiary']
 
         # Congenital syphilis deaths
         nnd = self.ti_nnd == sim.ti
         stillborn = self.ti_stillborn == sim.ti
         sim.people.request_death(nnd)
         sim.people.request_death(stillborn)
 
@@ -161,91 +180,83 @@
         self.congenital[congenital] = True
         self.susceptible[congenital] = False
 
         return
 
     def update_results(self, sim):
         super(Syphilis, self).update_results(sim)
-        self.results['new_nnds'][sim.ti] = np.count_nonzero(self.ti_nnd == sim.ti)
-        self.results['new_stillborns'][sim.ti] = np.count_nonzero(self.ti_stillborn == sim.ti)
-        self.results['new_congenital'][sim.ti] = np.count_nonzero(self.ti_congenital == sim.ti)
+        ti = sim.ti
+        self.results.new_nnds[ti]       = np.count_nonzero(self.ti_nnd == ti)
+        self.results.new_stillborns[ti] = np.count_nonzero(self.ti_stillborn == ti)
+        self.results.new_congenital[ti] = np.count_nonzero(self.ti_congenital == ti)
         return
 
     def make_new_cases(self, sim):
-        # TODO: for now, still using generic transmission method, but could replace here if needed
         super(Syphilis, self).make_new_cases(sim)
         return
 
-    def set_prognoses(self, sim, target_uids, source_uids=None):
+    def set_prognoses(self, sim, uids, source_uids=None):
         """
         Set initial prognoses for adults newly infected with syphilis
         """
 
-        # Subset target_uids to only include ones with active infection
-        if source_uids is not None:
-            active_sources = self.active[source_uids].values.nonzero()[-1]
-            uids = target_uids[active_sources]
-        else:
-            uids = target_uids
-
         self.susceptible[uids] = False
+        self.ever_exposed[uids] = True
         self.exposed[uids] = True
         self.infected[uids] = True
         self.ti_exposed[uids] = sim.ti
         self.ti_infected[uids] = sim.ti
 
         # Set future dates and probabilities
         # Exposed to primary
         dur_exposed = self.pars.dur_exposed.rvs(uids)
-        self.dur_exposed[uids] = dur_exposed
         self.ti_primary[uids] = sim.ti + rr(dur_exposed / sim.dt)
-        self.dur_infection[uids] = dur_exposed
 
         # Primary to secondary
         dur_primary = self.pars.dur_primary.rvs(uids)
         self.ti_secondary[uids] = self.ti_primary[uids] + rr(dur_primary / sim.dt)
-        self.dur_infection[uids] += dur_primary
 
         return
 
     def set_secondary_prognoses(self, sim, uids):
         """ Set prognoses for people who have just progressed to secondary infection """
 
+        dur_secondary = self.pars.dur_secondary.rvs(uids)
+
         # Secondary to latent_temp or latent_long
-        latent_temp_uids = self.pars.p_latent_temp.filter(uids)
-        latent_long_uids = np.setdiff1d(uids, latent_temp_uids)
+        latent_temp = self.pars.p_latent_temp.rvs(uids)
+        latent_temp_uids = uids[latent_temp]
+        latent_long_uids = uids[~latent_temp]
 
-        dur_secondary_temp = self.pars.dur_secondary.rvs(latent_temp_uids)
+        dur_secondary_temp = dur_secondary[latent_temp]
         self.ti_latent_temp[latent_temp_uids] = self.ti_secondary[latent_temp_uids] + rr(dur_secondary_temp / sim.dt)
-        self.dur_infection[latent_temp_uids] += dur_secondary_temp
 
-        dur_secondary_long = self.pars.dur_secondary.rvs(latent_long_uids)
+        dur_secondary_long = dur_secondary[~latent_temp]
         self.ti_latent_long[latent_long_uids] = self.ti_secondary[latent_long_uids] + rr(dur_secondary_long / sim.dt)
-        self.dur_infection[latent_long_uids] += dur_secondary_long
 
         return
 
     def set_latent_temp_prognoses(self, sim, uids):
         # Primary to secondary
         dur_latent_temp = self.pars.dur_latent_temp.rvs(uids)
         self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_temp / sim.dt)
-        self.dur_infection[uids] += dur_latent_temp
         return
 
     def set_latent_long_prognoses(self, sim, uids):
+
+        dur_latent = self.pars.dur_latent_long.rvs(uids)
+
         # Primary to secondary
-        dur_latent_long = self.pars.dur_latent_long.rvs(uids)
+        dur_latent_long = dur_latent
         self.ti_secondary[uids] = self.ti_latent_temp[uids] + rr(dur_latent_long / sim.dt)
-        self.dur_infection[uids] += dur_latent_long
 
         # Latent_long to tertiary
-        tertiary_uids = self.pars.p_tertiary.filter(uids)
-        dur_latent_long = self.pars.dur_latent_long.rvs(tertiary_uids)
-        self.ti_tertiary[tertiary_uids] = self.ti_latent_long[tertiary_uids] + rr(dur_latent_long / sim.dt)
-        self.dur_infection[tertiary_uids] += dur_latent_long
+        tertiary = self.pars.p_tertiary.rvs(uids)
+        tertiary_uids = uids[tertiary]
+        self.ti_tertiary[tertiary_uids] = self.ti_latent_long[tertiary_uids] + rr(dur_latent_long[tertiary] / sim.dt)
 
         return
 
     def set_congenital(self, sim, target_uids, source_uids=None):
         """
         Natural history of syphilis for congenital infection
         """
@@ -256,21 +267,116 @@
             source_state_inds = getattr(self, state)[source_uids].values.nonzero()[-1]
             uids = target_uids[source_state_inds]
 
             if len(uids) > 0:
 
                 # Birth outcomes must be modified to add probability of susceptible birth
                 birth_outcomes = self.pars.birth_outcomes[state]
-                assigned_outcomes = birth_outcomes.rvs(uids)-uids  # WHY??
+                assigned_outcomes = birth_outcomes.rvs(len(uids))
                 time_to_birth = -sim.people.age
 
                 # Schedule events
                 for oi, outcome in enumerate(self.pars.birth_outcome_keys):
                     o_uids = uids[assigned_outcomes == oi]
                     if len(o_uids) > 0:
                         ti_outcome = f'ti_{outcome}'
                         vals = getattr(self, ti_outcome)
                         vals[o_uids] = sim.ti + rr(time_to_birth[o_uids].values / sim.dt)
                         setattr(self, ti_outcome, vals)
 
         return
 
+
+# %% Syphilis-related interventions
+
+__all__ += ['syph_screening', 'syph_treatment']
+
+datafiles = sc.objdict()
+for key in ['dx', 'tx', 'vx']:
+    datafiles[key] = sc.thispath() / f'../data/products/syph_{key}.csv' # CK: may want to make this more robust if we keep using it
+
+
+def load_syph_dx():
+    """
+    Create default diagnostic products
+    """
+    df = sc.dataframe.read_csv(datafiles.dx)
+    hierarchy = ['positive', 'inadequate', 'negative']
+    dxprods = dict(
+        rpr = ss.Dx(df[df.name == 'rpr'], hierarchy=hierarchy),
+        rst = ss.Dx(df[df.name == 'rst'], hierarchy=hierarchy),
+    )
+    return dxprods
+
+
+def load_syph_tx():
+    """
+    Create default treatment products
+    """
+    df = sc.dataframe.read_csv(datafiles.tx)  # Read in dataframe with parameters
+    txprods = dict()
+    for name in df.name.unique():
+        txprods[name] = ss.Tx(df[df.name == name])
+    return txprods
+
+
+class syph_screening(ss.routine_screening):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # self.requires = Syphilis  # not currently working
+        return
+
+    def _parse_product_str(self, product):
+        products = load_syph_dx()
+        if product not in products:
+            errormsg = f'Could not find diagnostic product {product} in the standard list ({sc.strjoin(products.keys())})'
+            raise ValueError(errormsg)
+        else:
+            return products[product]
+
+    def check_eligibility(self, sim):
+        """
+        Return an array of indices of agents eligible for screening at time t, i.e. sexually active
+        females in age range, plus any additional user-defined eligibility
+        """
+        if self.eligibility is not None:
+            is_eligible = self.eligibility(sim)
+        else:
+            is_eligible = sim.people.alive  # Probably not required
+        return is_eligible
+
+    def initialize(self, sim):
+        super().initialize(sim)
+        self.results += [
+            ss.Result('syphilis', 'n_screened', sim.npts, dtype=int, scale=True),
+            ss.Result('syphilis', 'n_dx', sim.npts, dtype=int, scale=True),
+        ]
+        return
+
+
+class syph_treatment(ss.treat_num):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # self.requires = Syphilis
+        return
+
+    def _parse_product_str(self, product):
+        products = load_syph_tx()
+        if product not in products:
+            errormsg = f'Could not find treatment product {product} in the standard list ({sc.strjoin(products.keys())})'
+            raise ValueError(errormsg)
+        else:
+            return products[product]
+
+    def initialize(self, sim):
+        super().initialize(sim)
+        self.results += ss.Result('syphilis', 'n_tx', sim.npts, dtype=int, scale=True)
+        return
+
+    def apply(self, sim):
+        treat_inds = super().apply(sim)
+        sim.people.syphilis.infected[treat_inds] = False
+        self.results['n_tx'][sim.ti] += len(treat_inds)
+
+
```

### Comparing `starsim-0.1.5/starsim/networks/networks.py` & `starsim-0.3.2/starsim/network.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 '''
 Networks that connect people within a population
 '''
 
-# %% Imports
+import networkx as nx
 import numpy as np
+import numba as nb
 import sciris as sc
 import starsim as ss
 import scipy.optimize as spo
-import scipy.stats as sps
 import scipy.spatial as spsp
-import pandas as pd
-from scipy.stats._distn_infrastructure import rv_frozen
-import scipy.stats as sps
 
+# CK: need to remove this, but slows down the code otherwise
+ss_float_ = ss.dtypes.float
+ss_int_ = ss.dtypes.int
 
-# Specify all externally visible functions this file defines
-__all__ = ['Networks', 'Network', 'NetworkConnector', 'SexualNetwork', 'mf', 'msm', 'mf_msm', 'hpv_network', 'maternal', 'embedding', 'static']
+# Specify all externally visible functions this file defines; see also more definitions below
+__all__ = ['Network', 'Networks', 'DynamicNetwork', 'SexualNetwork']
 
 
+# %% General network classes
+
 class Network(ss.Module):
     """
     A class holding a single network of contact edges (connections) between people
     as well as methods for updating these.
 
     The input is typically arrays including: person 1 of the connection, person 2 of
     the connection, the weight of the connection, the duration and start/end times of
@@ -60,37 +62,47 @@
 
     def __init__(self, pars=None, key_dict=None, vertical=False, *args, **kwargs):
 
         # Initialize as a module
         super().__init__(pars, *args, **kwargs)
 
         # Each relationship is characterized by these default set of keys, plus any user- or network-supplied ones
-        default_keys = {
-            'p1': ss.int_,
-            'p2': ss.int_,
-            'beta': ss.float_,
-        }
+        default_keys = dict(
+            p1 = ss_int_,
+            p2 = ss_int_,
+            beta = ss_float_,
+        )
         self.meta = ss.omerge(default_keys, key_dict)
         self.vertical = vertical  # Whether transmission is bidirectional
 
         # Initialize the keys of the network
         self.contacts = sc.objdict()
         for key, dtype in self.meta.items():
             self.contacts[key] = np.empty((0,), dtype=dtype)
 
         # Set data, if provided
         for key, value in kwargs.items():
             self.contacts[key] = np.array(value, dtype=self.meta.get(key))
             self.initialized = True
 
         # Define states using placeholder values
-        self.participant = ss.State('participant', bool, fill_value=False)
-        self.debut = ss.State('debut', float, fill_value=0)
+        self.participant = ss.State('participant', bool, default=False)
         return
+    
+    @property
+    def p1(self):
+        return self.contacts['p1'] if 'p1' in self.contacts else None
+    
+    @property
+    def p2(self):
+        return self.contacts['p2'] if 'p2' in self.contacts else None
 
+    @property
+    def beta(self):
+        return self.contacts['beta'] if 'beta' in self.contacts else None
 
     def initialize(self, sim):
         super().initialize(sim)
         return
 
     def __len__(self):
         try:
@@ -246,15 +258,15 @@
             inds = sc.promotetoarray(inds)
         if inds.dtype != np.int64:  # pragma: no cover # This is int64 since indices often come from utils.true(), which returns int64
             inds = np.array(inds, dtype=np.int64)
 
         # Find the contacts
         contact_inds = ss.find_contacts(self.contacts.p1, self.contacts.p2, inds)
         if as_array:
-            contact_inds = np.fromiter(contact_inds, dtype=ss.int_)
+            contact_inds = np.fromiter(contact_inds, dtype=ss_int_)
             contact_inds.sort()
 
         return contact_inds
 
     def add_pairs(self):
         """ Define how pairs of people are formed """
         pass
@@ -269,33 +281,23 @@
         This method is typically called via `People.remove()` and
         is specifically used when removing agents from the simulation.
         """
         keep = ~(np.isin(self.contacts.p1, uids) | np.isin(self.contacts.p2, uids))
         for k in self.meta_keys():
             self.contacts[k] = self.contacts[k][keep]
 
-
-class DynamicNetwork(Network):
-    def __init__(self, pars=None, key_dict=None):
-        key_dict = ss.omerge({'dur': ss.float_}, key_dict)
-        super().__init__(pars, key_dict=key_dict)
-
-    def end_pairs(self, people):
-        dt = people.dt
-        self.contacts.dur = self.contacts.dur - dt
-
-        # Non-alive agents are removed
-        active = (self.contacts.dur > 0) & people.alive[self.contacts.p1] & people.alive[self.contacts.p2]
-        self.contacts.p1 = self.contacts.p1[active]
-        self.contacts.p2 = self.contacts.p2[active]
-        self.contacts.beta = self.contacts.beta[active]
-        self.contacts.dur = self.contacts.dur[active]
+    def beta_per_dt(self, disease_beta=None, dt=None, uids=None):
+        if uids is None: uids = Ellipsis
+        return self.contacts.beta[uids] * disease_beta * dt
 
 
 class Networks(ss.ndict):
+    """
+    Container for networks
+    """
     def __init__(self, *args, type=Network, connectors=None, **kwargs):
         self.setattribute('_connectors', ss.ndict(connectors))
         super().__init__(*args, type=type, **kwargs)
         return
 
     def initialize(self, sim):
         for nw in self.values():
@@ -308,141 +310,336 @@
         for nw in self.values():
             nw.update(people)
         for cn in self._connectors.values():
             cn.update(people)
         return
 
 
+class DynamicNetwork(Network):
+    """ A network where partnerships update dynamically """
+    def __init__(self, pars=None, key_dict=None, **kwargs):
+        key_dict = ss.omerge({'dur': ss_float_}, key_dict)
+        super().__init__(pars, key_dict=key_dict, **kwargs)
+        return
+
+    def end_pairs(self, people):
+        dt = people.dt
+        self.contacts.dur = self.contacts.dur - dt
+
+        # Non-alive agents are removed
+        active = (self.contacts.dur > 0) & people.alive[self.contacts.p1] & people.alive[self.contacts.p2]
+        for k in self.meta_keys():
+            self.contacts[k] = self.contacts[k][active]
+        return
+
+
 class SexualNetwork(Network):
     """ Base class for all sexual networks """
-    def __init__(self, pars=None):
-        super().__init__(pars)
+    def __init__(self, pars=None, key_dict=None, **kwargs):
+        key_dict = ss.omerge({'acts': ss_int_}, key_dict)
+        super().__init__(pars, key_dict=key_dict, **kwargs)
+        self.debut = ss.State('debut', float, default=0)
+        return
 
     def active(self, people):
         # Exclude people who are not alive
         return self.participant & (people.age > self.debut) & people.alive
 
     def available(self, people, sex):
         # Currently assumes unpartnered people are available
         # Could modify this to account for concurrency
         # This property could also be overwritten by a NetworkConnector
         # which could incorporate information about membership in other
         # contact networks
         return np.setdiff1d(ss.true(people[sex] & self.active(people)), self.members) # ss.true instead of people.uid[]?
 
+    def beta_per_dt(self, disease_beta=None, dt=None, uids=None):
+        if uids is None: uids = Ellipsis
+        return self.contacts.beta[uids] * (1 - (1 - disease_beta) ** (self.contacts.acts[uids] * dt))
+
+
+# %% Specific instances of networks
+__all__ += ['StaticNet', 'RandomNet', 'MFNet', 'MSMNet', 'EmbeddingNet', 'MaternalNet', 'HPVNet']
 
-class mf(SexualNetwork, DynamicNetwork):
+
+class StaticNet(Network):
     """
-    This network is built by **randomly pairing** males and female with variable
-    relationship durations.
+    A network class of static partnerships converted from a networkx graph. There's no formation of new partnerships
+    and initialized partnerships only end when one of the partners dies. The networkx graph can be created outside Starsim
+    if population size is known. Or the graph can be created by passing a networkx generator function to Starsim.
+
+    If "seed=True" is passed as a parameter, it is replaced with the built-in RNG.
+    The parameter "n" is supplied automatically to be equal to n_agents.
+    
+    **Examples**::
+
+        # Generate a networkx graph and pass to Starsim
+        import networkx as nx
+        import starsim as ss
+        g = nx.scale_free_graph(n=10000)
+        ss.StaticNet(graph=g)
+
+        # Pass a networkx graph generator to Starsim
+        ss.StaticNet(graph=nx.erdos_renyi_graph, p=0.0001, seed=True)
+        
+        # Just create a default graph
     """
 
-    def __init__(self, pars=None, key_dict=None):
+    def __init__(self, graph=None, pars=None, **kwargs):
+        super().__init__(**kwargs)
+        self.graph = graph
+        self.pars = ss.omerge(dict(seed=True), pars)
+        self.dist = ss.Dist(name='StaticNet').initialize()
+        return
+
+    def initialize(self, sim):
+        n_agents = sim.pars.n_agents
+        if self.graph is None:
+            self.graph = nx.fast_gnp_random_graph # Fast random (Erdos-Renyi) graph creator
+            if 'p' not in self.pars and 'n_contacts' not in self.pars: # TODO: refactor
+                self.pars.n_contacts = 10
+        if 'n_contacts' in self.pars: # Convert from n_contacts to probability
+            self.pars.p = self.pars.pop('n_contacts')/n_agents
+        if 'seed' in self.pars and self.pars.seed is True:
+            self.pars.seed = self.dist.rng
+        if callable(self.graph):
+            self.graph = self.graph(n=n_agents, **self.pars)
+        self.validate_pop(n_agents)
+        super().initialize(sim)
+        self.get_contacts()
+        return
+
+    def validate_pop(self, popsize):
+        n_nodes = self.graph.number_of_nodes()
+        if n_nodes > popsize:
+            errormsg = f'Please ensure the number of nodes in graph {n_nodes} is smaller than population size {popsize}.'
+            raise ValueError(errormsg)
+
+    def get_contacts(self):
+        p1s = []
+        p2s = []
+        for edge in self.graph.edges():
+            p1, p2 = edge
+            p1s.append(p1)
+            p2s.append(p2)
+        self.contacts.p1 = np.concatenate([self.contacts.p1, p1s])
+        self.contacts.p2 = np.concatenate([self.contacts.p2, p2s])
+        self.contacts.beta = np.concatenate([self.contacts.beta, np.ones_like(p1s)])
+        return
+
+
+class RandomNet(DynamicNetwork):
+    """ Random connectivity between agents """
+
+    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
+        """ Initialize """
         pars = ss.omerge({
-            'duration_dist': ss.lognorm(mean=15, stdev=15), # Can vary by age, year, and individual pair. Set scale=exp(mu) and s=sigma where mu,sigma are of the underlying normal distribution.
-            'participation_dist': sps.bernoulli(p=0.9),  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
-            'debut_dist': sps.norm(loc=16, scale=2),  # Age of debut can vary by using callable parameter values
-            'rel_part_rates': 1.0,
+            'n_contacts': 10,  # Distribution or int. If int, interpreted as the mean of the dist listed in par_dists
+            'dur': 1,
         }, pars)
 
-        DynamicNetwork.__init__(self, key_dict)
-        SexualNetwork.__init__(self, pars)
+        super().__init__(pars=pars, key_dict=key_dict, **kwargs)
+        
+        # Default RNG
+        self.dist = ss.Dist(distname='RandomNet')
+
+        return
+
+    def initialize(self, sim):
+        super().initialize(sim)
+        self.add_pairs(sim.people)
+        return
+
+    @staticmethod
+    @nb.njit(cache=True)
+    def get_source(inds, n_contacts):
+        """ Optimized helper function for getting contacts """
+        total_number_of_half_edges = np.sum(n_contacts)
+        count = 0
+        source = np.zeros((total_number_of_half_edges,), dtype=ss_int_)
+        for i, person_id in enumerate(inds):
+            n = n_contacts[i]
+            source[count: count + n] = person_id
+            count += n
+        return source
+    
+    def get_contacts(self, inds, n_contacts):
+        """
+        Efficiently generate contacts
+
+        Note that because of the shuffling operation, each person is assigned 2N contacts
+        (i.e. if a person has 5 contacts, they appear 5 times in the 'source' array and 5
+        times in the 'target' array). Therefore, the `number_of_contacts` argument to this
+        function should be HALF of the total contacts a person is expected to have, if both
+        the source and target array outputs are used (e.g. for social contacts)
+
+        adjusted_number_of_contacts = np.round(number_of_contacts / 2).astype(cvd.default_int)
+
+        Whereas for asymmetric contacts (e.g. staff-public interactions) it might not be necessary
+
+        Args:
+            inds: List/array of person indices
+            number_of_contacts: List/array the same length as `inds` with the number of unidirectional
+            contacts to assign to each person. Therefore, a person will have on average TWICE this number
+            of random contacts.
+
+        Returns: Two arrays, for source and target
+        """
+        source = self.get_source(inds, n_contacts)
+        target = self.dist.rng.permutation(source)
+        self.dist.jump() # Reset the RNG manually # TODO, think if there's a better way
+        return source, target
+
+    def update(self, people, dt=None):
+        self.end_pairs(people)
+        self.add_pairs(people)
+        return
+
+    def add_pairs(self, people):
+        """ Generate contacts """
+        if isinstance(self.pars.n_contacts, ss.Dist):
+            number_of_contacts = self.pars.n_contacts.rvs(people.uid[people.alive])  # or people.uid?
+        else:
+            number_of_contacts = np.full(len(people), self.pars.n_contacts)
+
+        number_of_contacts = np.round(number_of_contacts / 2).astype(ss_int_)  # One-way contacts
+
+        p1, p2 = self.get_contacts(people.uid.__array__(), number_of_contacts)
+        beta = np.ones(len(p1), dtype=ss_float_)
+
+        if isinstance(self.pars.dur, ss.Dist):
+            dur = self.pars.dur.rvs(p1)
+        else:
+            dur = np.full(len(p1), self.pars.dur)
+
+        self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
+        self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
+        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
+        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
+
+        return
+
+
+class MFNet(SexualNetwork, DynamicNetwork):
+    """
+    This network is built by **randomly pairing** males and female with variable
+    relationship durations.
+    """
+
+    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
+        pars = ss.omergeleft(pars,
+            duration = 15,  # Can vary by age, year, and individual pair. Set scale=exp(mu) and s=sigma where mu,sigma are of the underlying normal distribution.
+            participation = 0.9,  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
+            debut = 16,  # Age of debut can vary by using callable parameter values
+            acts = 80,
+            rel_part_rates = 1.0,
+        )
+
+        par_dists = ss.omergeleft(par_dists,
+            duration      = ss.lognorm_ex,
+            participation = ss.bernoulli,
+            debut         = ss.normal,
+            acts          = ss.poisson,
+        )
+
+        DynamicNetwork.__init__(self, key_dict=key_dict, **kwargs)
+        SexualNetwork.__init__(self, pars, key_dict=key_dict, **kwargs)
+
+        self.dist = ss.choice(name='MFNet', replace=False) # Set the array later
+        self.par_dists = par_dists
+
         return
 
     def initialize(self, sim):
         super().initialize(sim)
-        
         self.set_network_states(sim.people)
         self.add_pairs(sim.people, ti=0)
         return
 
     def set_network_states(self, people, upper_age=None):
         """ Set network states including age of entry into network and participation rates """
         self.set_debut(people, upper_age=upper_age)
         self.set_participation(people, upper_age=upper_age)
 
     def set_participation(self, people, upper_age=None):
         # Set people who will participate in the network at some point
-        year = people.year
         if upper_age is None: uids = people.uid
         else: uids = people.uid[(people.age < upper_age)]
-        self.participant[uids] = self.pars.participation_dist.rvs(uids)
+        self.participant[uids] = self.pars.participation.rvs(uids)
 
     def set_debut(self, people, upper_age=None):
         # Set debut age
         if upper_age is None: uids = people.uid
         else: uids = people.uid[(people.age < upper_age)]
-        self.debut[uids] = self.pars.debut_dist.rvs(uids)
-        uids_to_update = uids[np.isnan(people.debut[uids])]
-        people.debut[uids_to_update] = self.debut[uids_to_update]
+        self.debut[uids] = self.pars.debut.rvs(uids)
         return
 
     def add_pairs(self, people, ti=None):
         available_m = self.available(people, 'male')
         available_f = self.available(people, 'female')
 
         # random.choice is not common-random-number safe, and therefore we do
         # not try to Stream-ify the following draws at this time.
         if len(available_m) <= len(available_f):
+            self.dist.set(a=available_f)
             p1 = available_m
-            p2 = np.random.choice(a=available_f, size=len(p1), replace=False)
+            p2 = self.dist.rvs(n=len(p1)) # TODO: not fully stream safe
         else:
+            self.dist.set(a=available_m)
             p2 = available_f
-            p1 = np.random.choice(a=available_m, size=len(p2), replace=False)
+            p1 = self.dist.rvs(n=len(p2))
+        self.dist.jump() # TODO: think if there's a better way
 
         beta = np.ones_like(p1)
 
-        # Figure out durations
-        # print('DJK TODO')
-        if ss.options.multirng and (len(p1) == len(np.unique(p1))):
+        # Figure out durations and acts
+        if (len(p1) == len(np.unique(p1))):
             # No duplicates and user has enabled multirng, so use slotting based on p1
-            dur_vals = self.pars.duration_dist.rvs(p1)
+            dur_vals = self.pars.duration.rvs(p1)
+            act_vals = self.pars.acts.rvs(p1)
         else:
-            dur_vals = self.pars.duration_dist.rvs(len(p1))  # Just use len(p1) to say how many draws are needed
+            # If multirng is enabled, we're here because some individuals in p1
+            # are starting multiple relationships on this timestep. If using
+            # slotted draws, as above, repeated relationships will get the same
+            # duration and act rates, which is scientifically undesirable.
+            # Instead, we fall back to a not-CRN safe approach:
+            dur_vals = self.pars.duration.rvs(len(p1))  # Just use len(p1) to say how many draws are needed
+            act_vals = self.pars.acts.rvs(len(p1))
 
         self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
         self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
         self.contacts.beta = np.concatenate([self.contacts.beta, beta])
         self.contacts.dur = np.concatenate([self.contacts.dur, dur_vals])
+        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
+
         return len(p1)
 
     def update(self, people, dt=None):
         self.end_pairs(people)
         self.set_network_states(people, upper_age=people.dt)
         self.add_pairs(people)
         return
 
 
-class msm(SexualNetwork, DynamicNetwork):
+class MSMNet(SexualNetwork, DynamicNetwork):
     """
     A network that randomly pairs males
     """
 
-    def __init__(self, pars=None):
-        default_pars = {
-            'part_rates': 0.1,  # Participation rates - can vary by sex and year
-            'rel_part_rates': 1.0,
-        }
-
-        desired_mean = 5
-        desired_std = 3
-        mu = np.log(desired_mean**2 / np.sqrt(desired_mean**2 + desired_std**2))
-        sigma = np.sqrt(np.log(1 + desired_std**2 / desired_mean**2))
-        default_pars['duration_dist'] = sps.lognorm(s=sigma, scale=np.exp(mu)) # Can vary by age, year, and individual pair. Set scale=exp(mu) and s=sigma where mu,sigma are of the underlying normal distribution.
-
-        desired_mean = 18
-        desired_std = 2
-        mu = np.log(desired_mean**2 / np.sqrt(desired_mean**2 + desired_std**2))
-        sigma = np.sqrt(np.log(1 + desired_std**2 / desired_mean**2))
-        default_pars['debut_dist'] = sps.lognorm(s=sigma, scale=np.exp(mu))
-
-        pars = ss.omerge(default_pars, pars)
-        DynamicNetwork.__init__(self)
-        SexualNetwork.__init__(self, pars)
-
+    def __init__(self, pars=None, key_dict=None, **kwargs):
+        pars = ss.omergeleft(pars,
+            duration_dist = ss.lognorm_ex(mean=15, stdev=15),
+            participation_dist = ss.bernoulli(p=0.1),  # Probability of participating in this network - can vary by individual properties (age, sex, ...) using callable parameter values
+            debut_dist = ss.normal(loc=16, scale=2),
+            acts = ss.lognorm_ex(mean=80, stdev=20),
+            rel_part_rates = 1.0,
+        )
+        DynamicNetwork.__init__(self, key_dict, **kwargs)
+        SexualNetwork.__init__(self, pars, key_dict)
+        self.dist = ss.bernoulli(name='MSMNet')
         return
 
     def initialize(self, sim):
         # Add more here in line with MF network, e.g. age of debut
         # Or if too much replication then perhaps both these networks
         # should be subclasss of a specific network type (ask LY/DK)
         super().initialize(sim)
@@ -453,278 +650,230 @@
     def set_network_states(self, people, upper_age=None):
         """ Set network states including age of entry into network and participation rates """
         if upper_age is None: uids = people.uid[people.male]
         else: uids = people.uid[people.male & (people.age < upper_age)]
 
         # Participation
         self.participant[people.female] = False
-        pr = self.pars.part_rates
-        dist = sps.bernoulli.rvs(p=pr, size=len(uids))
-        self.participant[uids] = dist
+        pr = self.pars.rel_part_rates
+        self.dist.set(p=pr)
+        self.participant[uids] = self.dist.rvs(uids) # Should be CRN safe?
 
         # Debut
         self.debut[uids] = self.pars.debut_dist.rvs(len(uids)) # Just pass len(uids) as this network is not crn safe anyway
-        uids_to_update = uids[np.isnan(people.debut[uids])]
-        people.debut[uids_to_update] = self.debut[uids_to_update]
         return
 
     def add_pairs(self, people, ti=None):
         # Pair all unpartnered MSM
         available_m = self.available(people, 'm')
         n_pairs = int(len(available_m)/2)
         p1 = available_m[:n_pairs]
         p2 = available_m[n_pairs:n_pairs*2]
 
         # Figure out durations
-        # print('DJK TODO')
-        if ss.options.multirng and (len(p1) == len(np.unique(p1))):
-            # No duplicates and user has enabled multirng, so use slotting based on p1
-            dur = self.pars['duration_dist'].rvs(p1)
+        if (len(p1) == len(np.unique(p1))):
+            # No duplicates, so use slotting based on p1
+            dur = self.pars.duration.rvs(p1)
+            act_vals = self.pars.acts.rvs(p1)
         else:
-            dur = self.pars['duration_dist'].rvs(len(p1)) # Just use len(p1) to say how many draws are needed
+            dur = self.pars.duration.rvs(len(p1)) # Just use len(p1) to say how many draws are needed
+            act_vals = self.pars.acts.rvs(len(p1))
 
         self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
         self.contacts.p2 = np.concatenate([self.contacts.p2, p2])
         self.contacts.beta = np.concatenate([self.contacts.beta, np.ones_like(p1)])
         self.contacts.dur = np.concatenate([self.contacts.dur, dur])
+        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
         return len(p1)
 
     def update(self, people, dt=None):
         self.end_pairs(people)
         self.set_network_states(people, upper_age=people.dt)
         self.add_pairs(people)
         return
 
 
-class embedding(mf):
+class EmbeddingNet(MFNet):
     """
     Heterosexual age-assortative network based on a one-dimensional embedding. Could be made more generic.
     """
 
     def __init__(self, pars=None, **kwargs):
         """
         Create a sexual network from a 1D embedding based on age
 
         male_shift is the average age that males are older than females in partnerships
         std is the standard deviation of noise added to the age of each individual when seeking a pair. Larger values will created more diversity in age gaps.
         
         """
         pars = ss.omerge({
-            'embedding_func': sps.norm(loc=self.embedding_loc, scale=2),
+            'embedding_func': ss.normal(name='EmbeddingNet', loc=self.embedding_loc, scale=2),
+            'male_shift': 5,
         }, pars)
         super().__init__(pars, **kwargs)
         return
 
     @staticmethod
-    def embedding_loc(self, sim, uids):
+    def embedding_loc(module, sim, uids):
         loc = sim.people.age[uids].values
-        loc[sim.people.female[uids]] += 5 # Shift females so they will be paired with older men
+        loc[sim.people.female[uids]] += module.pars.male_shift  # Shift females so they will be paired with older men
         return loc
 
     def add_pairs(self, people, ti=None):
         available_m = self.available(people, 'male')
         available_f = self.available(people, 'female')
 
         if not len(available_m) or not len(available_f):
             if ss.options.verbose > 1:
                 print('No pairs to add')
             return 0
 
         available = np.concatenate((available_m, available_f))
-        loc = self.pars['embedding_func'].rvs(available)
+        loc = self.pars.embedding_func.rvs(available)
         loc_f = loc[people.female[available]]
         loc_m = loc[~people.female[available]]
 
         dist_mat = spsp.distance_matrix(loc_m[:, np.newaxis], loc_f[:, np.newaxis])
 
         ind_m, ind_f = spo.linear_sum_assignment(dist_mat)
         # loc_f[ind_f[0]] is close to loc_m[ind_m[0]]
 
         n_pairs = len(ind_f)
 
         beta = np.ones(n_pairs)
 
         # Figure out durations
         p1 = available_m[ind_m]
-        dur_vals = self.pars['duration_dist'].rvs(p1)
+        dur_vals = self.pars.duration.rvs(p1)
+        act_vals = self.pars.acts.rvs(p1)
 
         self.contacts.p1 = np.concatenate([self.contacts.p1, p1])
         self.contacts.p2 = np.concatenate([self.contacts.p2, available_f[ind_f]])
         self.contacts.beta = np.concatenate([self.contacts.beta, beta])
         self.contacts.dur = np.concatenate([self.contacts.dur, dur_vals])
+        self.contacts.acts = np.concatenate([self.contacts.acts, act_vals])
         return len(beta)
 
 
-class NetworkConnector(ss.Module):
+class MaternalNet(Network):
     """
-    Template for a connector between networks.
+    Vertical (birth-related) transmission network
     """
-    def __init__(self, *args, networks=None, pars=None, **kwargs):
-        super().__init__(pars, requires=networks, *args, **kwargs)
+    def __init__(self, key_dict=None, vertical=True, **kwargs):
+        """
+        Initialized empty and filled with pregnancies throughout the simulation
+        """
+        key_dict = sc.mergedicts({'dur': ss_float_}, key_dict)
+        super().__init__(key_dict=key_dict, vertical=vertical, **kwargs)
         return
 
-    def set_participation(self, people, upper_age=None):
-        pass
-
-    def update(self, people):
-        pass
-
-
-class mf_msm(NetworkConnector):
-    """ Combines the MF and MSM networks """
-    def __init__(self, pars=None):
-        networks = [ss.mf, ss.msm]
-        pars = ss.omerge({
-            'prop_bi': 0.5,  # Could vary over time -- but not by age or sex or individual
-        }, pars)
-        super().__init__(networks=networks, pars=pars)
-
-        self.bi_dist = sps.bernoulli(p=self.pars.prop_bi)
+    def update(self, people, dt=None):
+        if dt is None: dt = people.dt
+        # Set beta to 0 for women who complete post-partum period
+        # Keep connections for now, might want to consider removing
+        self.contacts.dur = self.contacts.dur - dt
+        inactive = self.contacts.dur <= 0
+        self.contacts.beta[inactive] = 0
         return
 
     def initialize(self, sim):
-        super().initialize(sim)
-        self.set_participation(sim.people)
-        return
-
-    def set_participation(self, people, upper_age=None):
-        if upper_age is None:
-            uids = people.uid
-        else:
-            uids = people.uid[(people.age < upper_age)]
-        uids = ss.true(people.male[uids])
-
-        # Get networks and overwrite default participation
-        mf = people.networks['mf']
-        msm = people.networks['msm']
-        mf.participant[uids] = False
-        msm.participant[uids] = False
-
-        # Male participation rate uses info about cross-network participation.
-        # First, we determine who's participating in the MSM network
-        pr = msm.pars.part_rates
-        dist = sps.bernoulli.rvs(p=pr, size=len(uids))
-        msm.participant[uids] = dist
+        """ No pairs added upon initialization """
+        pass
 
-        # Now we take the MSM participants and determine which are also in the MF network
-        msm_uids = ss.true(msm.participant[uids])  # Males in the MSM network
-        bi_uids = self.bi_dist.filter(msm_uids)  # Males in both MSM and MF networks
-        mf_excl_set = np.setdiff1d(uids, msm_uids)  # Set of males who aren't in the MSM network
+    def add_pairs(self, mother_inds, unborn_inds, dur):
+        """
+        Add connections between pregnant women and their as-yet-unborn babies
+        """
+        beta = np.ones_like(mother_inds)
+        self.contacts.p1 = np.concatenate([self.contacts.p1, mother_inds])
+        self.contacts.p2 = np.concatenate([self.contacts.p2, unborn_inds])
+        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
+        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
+        return len(mother_inds)
 
-        # What remaining share to we need?
-        mf_df = mf.pars.part_rates.loc[mf.pars.part_rates.sex == 'm']  # Male participation in the MF network
-        mf_pr = np.interp(people.year, mf_df['year'], mf_df['part_rates']) * mf.pars.rel_part_rates
-        remaining_pr = max(mf_pr*len(uids)-len(bi_uids), 0)/len(mf_excl_set)
 
-        # Don't love the following new syntax:
-        mf_excl_uids = mf_excl_set[sps.uniform.rvs(size=len(mf_excl_set)) < remaining_pr]
+class HPVNet(MFNet):
+    """
+    WARNING: not CRN safe!
+    """
+    def __init__(self, pars=None, par_dists=None, key_dict=None, **kwargs):
+        pars = ss.omergeleft(pars,
+            duration = 15,
+            participation = 0.9,
+            debut = 16,
+            acts = 80,
+            rel_part_rates = 1.0,
+            cross_layer = 0.05,
+            concurrency = 0.05,
+            condoms = 0.2,
+            mixing = None,
+        )
 
-        mf.participant[bi_uids] = True
-        mf.participant[mf_excl_uids] = True
-        return
+        self.par_dists = ss.omergeleft(par_dists,
+            duration      = ss.lognorm,
+            participation = ss.bernoulli,
+            debut         = ss.norm,
+            acts          = ss.lognorm,
+            cross_layer   = ss.bernoulli,
+            concurrency   = ss.bernoulli,
+        )
 
-    def update(self, people):
-        self.set_participation(people, upper_age=people.dt)
-        return
+        key_dict = dict(
+            acts = ss_float_,
+            start = ss_float_,
+        )
 
+        DynamicNetwork.__init__(self, key_dict)
+        SexualNetwork.__init__(self, pars, key_dict)
 
-class hpv_network(mf):
-    def __init__(self, pars=None):
+        super().__init__(pars, key_dict=key_dict, **kwargs)
 
-        key_dict = {
-            'acts': ss.float_,
-            'start': ss.float_,
-        }
-
-        # Define default parameters
-        default_pars = dict()
-        default_pars['cross_layer']   = 0.05  # Proportion of agents who have concurrent cross-layer relationships
-        default_pars['partner_dist']  = sps.poisson(mu=0.01)  # The number of concurrent sexual partners
-
-        # TODO: Wrap so user can provide mean and dispersion directly - see #168
-        mu = 80 # Mean
-        alpha = 40 # Dispersion
-        sigma2 = mu + alpha * mu**2
-        n = mu**2 / (sigma2 - mu)
-        p = mu / sigma2
-        default_pars['act_dist']      = sps.nbinom(n=n, p=p)  # The number of sexual acts per year
-
-        default_pars['age_act_pars']  = dict(peak=30, retirement=100, debut_ratio=0.5,
-                                         retirement_ratio=0.1)  # Parameters describing changes in coital frequency over agent lifespans
-        default_pars['condoms']       = 0.2  # The proportion of acts in which condoms are used
-
-        low = 0
-        loc = 1
-        scale = 1
-        a = (low - loc) / scale
-        default_pars['duration_dist'] = sps.truncnorm(a=a, b=np.inf, loc=loc, scale=scale)  # Duration of partnerships
-
-        #default_pars['participation'] = None  # Incidence of partnership formation by age
-        default_pars['mixing']        = None  # Mixing matrices for storing age differences in partnerships
-
-        self.agebins = [0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75]
-        # Share of females of each age newly having casual relationships
-        self.f_participation = [0, 0, 0.10, 0.7, 0.8, 0.6, 0.6, 0.4, 0.1, 0.05, 0.001, 0.001, 0.001, 0.001, 0.001, 0.001]
-        # Share of males of each age newly having casual relationships
-        self.m_participation = [0, 0, 0.05, 0.7, 0.8, 0.6, 0.6, 0.4, 0.4, 0.3, 0.1, 0.05, 0.01, 0.01, 0.001, 0.001]
-
-        default_pars['participation_dist'] = sps.bernoulli(p=self.participation)
-
-        pars = ss.omerge(default_pars, pars)
-        super().__init__(pars, key_dict)
- 
         self.get_layer_probs()
-        self.validate_pars()
 
         return
 
     def initialize(self, sim):
         super().initialize(sim)
-        return self.add_pairs(sim.people, ti=0)
-
-    def validate_pars(self):
-        for par in ['partner_dist', 'act_dist', 'duration_dist', 'participation_dist']:
-            if not isinstance(self.pars[par], rv_frozen):
-                raise Exception(f'Network parameter {par} must be an instance of a scipy frozen distribution')
+        return self.add_pairs(sim.people)
 
     def update_pars(self, pars):
         if pars is not None:
             for k, v in pars.items():
                 self.pars[k] = v
         return
 
     @staticmethod
     def participation(self, sim, uids):
-        p = np.ones_like(uids, dtype=ss.float_)
+        p = np.ones_like(uids, dtype=ss_float_)
         fem = sim.people.female[uids]
         p[fem] = np.interp(sim.people.age[uids[fem]], self.agebins, self.f_participation)
         p[~fem] = np.interp(sim.people.age[uids[~fem]], self.agebins, self.m_participation)
         return p
 
     def get_layer_probs(self):
 
         defaults = {}
         mixing = np.array([
-            #       0,  5,  10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75
-            [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [5, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [10, 0, 0, .1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [15, 0, 0, .1, .1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [20, 0, 0, .1, .1, .1, .1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [25, 0, 0, .5, .1, .5, .1, .1, 0, 0, 0, 0, 0, 0, 0, 0, 0],
-            [30, 0, 0, 1, .5, .5, .5, .5, .1, 0, 0, 0, 0, 0, 0, 0, 0],
-            [35, 0, 0, .5, 1, 1, .5, 1, 1, .5, 0, 0, 0, 0, 0, 0, 0],
-            [40, 0, 0, 0, .5, 1, 1, 1, 1, 1, .5, 0, 0, 0, 0, 0, 0],
-            [45, 0, 0, 0, 0, .1, 1, 1, 2, 1, 1, .5, 0, 0, 0, 0, 0],
-            [50, 0, 0, 0, 0, 0, .1, 1, 1, 1, 1, 2, .5, 0, 0, 0, 0],
-            [55, 0, 0, 0, 0, 0, 0, .1, 1, 1, 1, 1, 2, .5, 0, 0, 0],
-            [60, 0, 0, 0, 0, 0, 0, 0, .1, .5, 1, 1, 1, 2, .5, 0, 0],
-            [65, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 2, .5, 0],
-            [70, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, .5],
-            [75, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
+            # 0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55, 60, 65, 70, 75, 75+
+            [0 , 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [5 , 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [10, 0,  0, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [15, 0,  0, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [20, 0,  0, .1, .1, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [25, 0,  0, .5, .1, .5, .1, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [30, 0,  0, 1 , .5, .5, .5, .5, .1, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [35, 0,  0, .5, 1 , 1 , .5, 1 , 1 , .5, 0 , 0 , 0 , 0 , 0 , 0 , 0] ,
+            [40, 0,  0, 0 , .5, 1 , 1 , 1 , 1 , 1 , .5, 0 , 0 , 0 , 0 , 0 , 0] ,
+            [45, 0,  0, 0 , 0 , .1, 1 , 1 , 2 , 1 , 1 , .5, 0 , 0 , 0 , 0 , 0] ,
+            [50, 0,  0, 0 , 0 , 0 , .1, 1 , 1 , 1 , 1 , 2 , .5, 0 , 0 , 0 , 0] ,
+            [55, 0,  0, 0 , 0 , 0 , 0 , .1, 1 , 1 , 1 , 1 , 2 , .5, 0 , 0 , 0] ,
+            [60, 0,  0, 0 , 0 , 0 , 0 , 0 , .1, .5, 1 , 1 , 1 , 2 , .5, 0 , 0] ,
+            [65, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 2 , .5, 0] ,
+            [70, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 1 , .5],
+            [75, 0,  0, 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 0 , 1 , 1 , 1 , 1] ,
         ])
 
         defaults['mixing'] = mixing
 
         for pkey, pval in defaults.items():
             if self.pars[pkey] is None:
                 self.pars[pkey] = pval
@@ -743,93 +892,95 @@
         current_partners = np.zeros((len(people)))
         current_partners[f_partnered_inds] = f_partnered_counts
         current_partners[m_partnered_inds] = m_partnered_counts
         partners = self.pars.partner_dist.rvs(len(people)) + 1
         underpartnered = current_partners < partners  # Indices of underpartnered people
 
         # Set people who will participate in the network at some point
-        can_participate = ss.true(people.active * underpartnered)
+        can_participate = ss.true(self.active(people) * underpartnered)
         self.participant[uids] = self.pars.participation_dist.rvs(can_participate)
         return
 
     def add_pairs(self, people, ti=0):
-        participating = ss.true(self.participant) # Will be the same people each time, with participation decided once per person
+        participating = ss.true(
+            self.participant)  # Will be the same people each time, with participation decided once per person
         f = participating[people.female[participating]]
         m = participating[~people.female[participating]]
 
         # Create preference matrix between eligible females and males that combines age and geo mixing
         age_bins_f = np.digitize(people.age[f],
                                  bins=self.agebins) - 1  # Age bins of females that are entering new relationships
         age_bins_m = np.digitize(people.age[m], bins=self.agebins) - 1  # Age bins of active and participating males
         age_f, age_m = np.meshgrid(age_bins_f, age_bins_m)
-        pair_probs = self.pars['mixing'][age_m, age_f + 1]
+        pair_probs = self.pars.mixing[age_m, age_f + 1]
 
         f_to_remove = pair_probs.max(axis=0) == 0  # list of female inds to remove if no male partners are found for her
-        #f = [i for i, flag in zip(f, f_to_remove) if ~flag]  # remove the inds who don't get paired on this timestep
+        # f = [i for i, flag in zip(f, f_to_remove) if ~flag]  # remove the inds who don't get paired on this timestep
         f = f[~f_to_remove]
         selected_males = []
         if len(f):
             pair_probs = pair_probs[:, np.invert(f_to_remove)]
             choices = []
             fems = np.arange(len(f))
             f_paired_bools = np.full(len(fems), True, dtype=bool)
-            np.random.shuffle(fems) # TODO: Stream-ify?
+            np.random.shuffle(fems)  # TODO: Stream-ify?
             for fem in fems:
                 m_col = pair_probs[:, fem]
                 if m_col.sum() > 0:
                     m_col_norm = m_col / m_col.sum()
-                    choice = np.random.choice(len(m_col_norm), p=m_col_norm) # TODO: Stream-ify?
+                    choice = np.random.choice(len(m_col_norm), p=m_col_norm)  # TODO: Stream-ify?
                     choices.append(choice)
                     pair_probs[choice, :] = 0  # Once male partner is assigned, remove from eligible pool
                 else:
                     f_paired_bools[fem] = False
             selected_males = m[np.array(choices).flatten()]
             f = f[f_paired_bools]
 
-        p1 = f
-        p2 = selected_males
-        n_partnerships = len(p1)
-        dur = self.pars.duration_dist.rvs(n_partnerships)
-        acts = self.pars.act_dist.rvs(n_partnerships)
+        p1 = selected_males
+        p2 = f
+        n_partnerships = len(p2)
+        dur = self.pars.duration.rvs(n_partnerships)
+        acts = self.pars.acts.rvs(n_partnerships)
         age_p1 = people.age[p1]
         age_p2 = people.age[p2]
 
-        age_debut_p1 = people.debut[p1]
-        age_debut_p2 = people.debut[p2]
+        age_debut_p1 = self.debut[p1] # TODO: Check that this still works - it was previously people.debut
+        age_debut_p2 = self.debut[p2]
 
         # For each couple, get the average age they are now and the average age of debut
         avg_age = np.array([age_p1, age_p2]).mean(axis=0)
         avg_debut = np.array([age_debut_p1, age_debut_p2]).mean(axis=0)
 
         # Shorten parameter names
-        dr = self.pars['age_act_pars']['debut_ratio']
-        peak = self.pars['age_act_pars']['peak']
-        rr = self.pars['age_act_pars']['retirement_ratio']
-        retire = self.pars['age_act_pars']['retirement']
+        aap = self.pars.age_act_pars
+        dr = aap['debut_ratio']
+        peak = aap['peak']
+        rr = aap['retirement_ratio']
+        retire = aap['retirement']
+        peak = aap['peak']
 
         # Get indices of people at different stages
-        below_peak_inds = avg_age <= self.pars['age_act_pars']['peak']
-        above_peak_inds = (avg_age > self.pars['age_act_pars']['peak']) & (
-                avg_age < self.pars['age_act_pars']['retirement'])
-        retired_inds = avg_age > self.pars['age_act_pars']['retirement']
+        below_peak_inds = avg_age <= peak
+        above_peak_inds = (avg_age > peak) & (avg_age < retire)
+        retired_inds = avg_age > retire
 
         # Set values by linearly scaling the number of acts for each partnership according to
         # the age of the couple at the commencement of the relationship
         below_peak_vals = acts[below_peak_inds] * (dr + (1 - dr) / (peak - avg_debut[below_peak_inds]) * (
                 avg_age[below_peak_inds] - avg_debut[below_peak_inds]))
         above_peak_vals = acts[above_peak_inds] * (
                 rr + (1 - rr) / (peak - retire) * (avg_age[above_peak_inds] - retire))
         retired_vals = 0
 
         # Set values and return
-        scaled_acts = np.full(len(acts), np.nan, dtype=ss.float_)
+        scaled_acts = np.full(len(acts), np.nan, dtype=ss_float_)
         scaled_acts[below_peak_inds] = below_peak_vals
         scaled_acts[above_peak_inds] = above_peak_vals
         scaled_acts[retired_inds] = retired_vals
-        start = np.array([ti] * n_partnerships, dtype=ss.float_)
+        start = np.array([ti] * n_partnerships, dtype=ss_float_)
         beta = np.ones(n_partnerships)
 
         new_contacts = dict(
             p1=p1,
             p2=p2,
             dur=dur,
             acts=scaled_acts,
@@ -849,91 +1000,83 @@
             self.contacts[key] = self.contacts[key][active]
 
         # Then add new relationships
         self.add_pairs(people, ti=ti)
         return
 
 
-class maternal(Network):
-    def __init__(self, key_dict=None, vertical=True, **kwargs):
-        """
-        Initialized empty and filled with pregnancies throughout the simulation
-        """
-        key_dict = sc.mergedicts({'dur': ss.float_}, key_dict)
-        super().__init__(key_dict=key_dict, vertical=vertical, **kwargs)
-        return
+# %% Network connectors
+__all__ += ['NetworkConnector', 'MF_MSM']
 
-    def update(self, people, dt=None):
-        if dt is None: dt = people.dt
-        # Set beta to 0 for women who complete post-partum period
-        # Keep connections for now, might want to consider removing
-        self.contacts.dur = self.contacts.dur - dt
-        inactive = self.contacts.dur <= 0
-        self.contacts.beta[inactive] = 0
+class NetworkConnector(ss.Module):
+    """
+    Template for a connector between networks.
+    """
+    def __init__(self, *args, networks=None, pars=None, **kwargs):
+        super().__init__(pars, requires=networks, *args, **kwargs)
         return
 
-    def initialize(self, sim):
-        """ No pairs added upon initialization """
+    def set_participation(self, people, upper_age=None):
         pass
 
-    def add_pairs(self, mother_inds, unborn_inds, dur):
-        """
-        Add connections between pregnant women and their as-yet-unborn babies
-        """
-        beta = np.ones_like(mother_inds)
-        self.contacts.p1 = np.concatenate([self.contacts.p1, mother_inds])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, unborn_inds])
-        self.contacts.beta = np.concatenate([self.contacts.beta, beta])
-        self.contacts.dur = np.concatenate([self.contacts.dur, dur])
-        return len(mother_inds)
-
-class static(Network):
-    """
-    A network class of static partnerships converted from a networkx graph. There's no formation of new partnerships
-    and initialized partnerships only end when one of the partners dies. The networkx graph can be created outside Starsim
-    if population size is known. Or the graph can be created by passing a networkx generator function to Starsim.
-
-    **Examples**::
+    def update(self, people):
+        pass
 
-    # Generate a networkx graph and pass to Starsim
-    import networkx as nx
-    import starsim as ss
-    g = nx.scale_free_graph(n=10000)
-    ss.static(graph=g)
 
-    # Pass a networkx graph generator to Starsim
-    ss.static(graph=nx.erdos_renyi_graph, p=0.0001)
+class MF_MSM(NetworkConnector):
+    """ Combines the MF and MSM networks """
+    def __init__(self, pars=None):
+        networks = [ss.MFNet, ss.MSMNet]
+        pars = ss.omergeleft(pars,
+            prop_bi = 0.5,  # Could vary over time -- but not by age or sex or individual
+        )
+        super().__init__(networks=networks, pars=pars)
 
-    """
-    def __init__(self, graph, **kwargs):
-        self.graph = graph
-        self.kwargs = kwargs
-        super().__init__()
+        self.bi_dist = ss.bernoulli(p=self.pars.prop_bi)
         return
 
     def initialize(self, sim):
-        popsize = sim.pars['n_agents']
-        if callable(self.graph):
-            self.graph = self.graph(n = popsize, **self.kwargs)
-        self.validate_pop(popsize)
         super().initialize(sim)
-        self.get_contacts()
+        self.set_participation(sim.people)
         return
 
-    def validate_pop(self, popsize):
-        n_nodes =  self.graph.number_of_nodes()
-        if n_nodes > popsize:
-            errormsg = f'Please ensure the number of nodes in graph {n_nodes} is smaller than population size {popsize}.'
-            raise ValueError(errormsg)
+    def set_participation(self, people, upper_age=None):
+        if upper_age is None:
+            uids = people.uid
+        else:
+            uids = people.uid[(people.age < upper_age)]
+        uids = ss.true(people.male[uids])
 
-    def get_contacts(self):
-        p1s = []
-        p2s = []
-        for edge in self.graph.edges():
-            p1, p2 = edge
-            p1s.append(p1)
-            p2s.append(p2)
-        self.contacts.p1 = np.concatenate([self.contacts.p1, p1s])
-        self.contacts.p2 = np.concatenate([self.contacts.p2, p2s])
-        self.contacts.beta = np.concatenate([self.contacts.beta, np.ones_like(p1s)])
+        # Get networks and overwrite default participation
+        mf = people.networks.mf
+        msm = people.networks.msm
+        mf.participant[uids] = False
+        msm.participant[uids] = False
+
+        # Male participation rate uses info about cross-network participation.
+        # First, we determine who's participating in the MSM network
+        pr = msm.pars.part_rates
+        dist = ss.bernoulli.rvs(p=pr, size=len(uids))
+        msm.participant[uids] = dist
+
+        # Now we take the MSM participants and determine which are also in the MF network
+        msm_uids = ss.true(msm.participant[uids])  # Males in the MSM network
+        bi_uids = self.bi_dist.filter(msm_uids)  # Males in both MSM and MF networks
+        mf_excl_set = np.setdiff1d(uids, msm_uids)  # Set of males who aren't in the MSM network
+
+        # What remaining share to we need?
+        mf_df = mf.pars.part_rates.loc[mf.pars.part_rates.sex == 'm']  # Male participation in the MF network
+        mf_pr = np.interp(people.year, mf_df['year'], mf_df['part_rates']) * mf.pars.rel_part_rates
+        remaining_pr = max(mf_pr*len(uids)-len(bi_uids), 0)/len(mf_excl_set)
+
+        # Don't love the following new syntax:
+        mf_excl_uids = mf_excl_set[ss.random().rvs(size=len(mf_excl_set)) < remaining_pr] # TODO: not RNG safe and yes ugly!
+
+        mf.participant[bi_uids] = True
+        mf.participant[mf_excl_uids] = True
         return
 
+    def update(self, people):
+        self.set_participation(people, upper_age=people.dt)
+        return
+
+
```

### Comparing `starsim-0.1.5/starsim/parameters.py` & `starsim-0.3.2/starsim/parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 Set parameters
 """
 
 import sciris as sc
 import starsim as ss
 
-
 __all__ = ['Parameters', 'make_pars']
 
-
 class Parameters(sc.objdict):
     """
     Create the parameters for the simulation. Typically, this function is used
     internally rather than called by the user; e.g. typical use would be to do
     sim = ss.Sim() and then inspect sim.pars, rather than calling this function
     directly.
 
@@ -22,40 +20,41 @@
         pars (dict): the parameters of the simulation
     """
 
     def __init__(self, **kwargs):
 
         # Population parameters
         self.n_agents        = 10e3  # Number of agents
-        self.total_pop       = 10e3  # If defined, used for calculating the scale factor
+        self.total_pop       = None  # If defined, used for calculating the scale factor
         self.pop_scale       = None  # How much to scale the population
-        self.remove_dead     = True          # Remove dead agents each timestep
+        self.remove_dead     = 10    # How many timesteps to go between removing dead agents (0 to not remove)
 
-        # Demographic parameters: NOT CURRENTLY FUNCTIONAL
-        # TBC whether these parameters live here or in separate demographic modules
-        self.location    = None  # What demographics to use
+        # Demographic parameters
+        self.location    = None  #  NOT CURRENTLY FUNCTIONAL - what demographics to use
+        self.birth_rate = None
+        self.death_rate = None
 
         # Simulation parameters
-        self.start           = 1995.         # Start of the simulation
+        self.start           = 2000          # Start of the simulation
         self.end             = None          # End of the simulation
-        self.n_years         = 35            # Number of years to run, if end isn't specified. Note that this includes burn-in
-        self.burnin          = 25            # Number of years of burnin. NB, this is doesn't affect the start and end dates of the simulation, but it is possible remove these years from plots
+        self.n_years         = 49            # Number of years to run, if end isn't specified. Note that this includes burn-in
+        self.burnin          = 0             # Number of years of burnin. NB, this is doesn't affect the start and end dates of the simulation, but it is possible remove these years from plots
         self.dt              = 1.0           # Timestep (in years)
         self.dt_demog        = 1.0           # Timestep for demographic updates (in years)
         self.rand_seed       = 1             # Random seed, if None, don't reset
         self.slot_scale      = 5             # Random slots will be assigned to newborn agents between min=n_agents and max=slot_scale*n_agents. Choosing a larger value here will reduce the probability of two agents using the same slot (and hence random draws), but increase the number of random numbers that are required.
         self.verbose         = ss.options.verbose # Whether or not to display information during the run -- options are 0 (silent), 0.1 (some; default), 1 (default), 2 (everything)
 
-        # Events and interventions
-        self.connectors = sc.autolist()
-        self.interventions = sc.autolist()  # The interventions present in this simulation; populated by the user
-        self.analyzers = sc.autolist()  # The functions present in this simulation; populated by the user
-
-        # Network parameters, generally initialized after the population has been constructed
-        self.networks        = sc.autolist()  # Network types and parameters
+        # Plug-ins: demographics, diseases, connectors, networks, analyzers, and interventions
+        self.demographics = ss.ndict()
+        self.diseases = ss.ndict()
+        self.networks = ss.ndict()
+        self.connectors = ss.ndict()
+        self.interventions = ss.ndict()
+        self.analyzers = ss.ndict()
 
         # Update with any supplied parameter values and generate things that need to be generated
         self.update(kwargs)
 
         if self.slot_scale < 1:
             raise Exception('The value of the "slot_scale" parameter must be a number >= 1.0')
 
@@ -80,8 +79,8 @@
                     errormsg = f'Key(s) {mismatches} not found; available keys are {available_keys}'
                     raise sc.KeyNotFoundError(errormsg)
             self.update(pars)
         return
 
 
 def make_pars(**kwargs):
-    return Parameters(**kwargs)
+    return Parameters(**kwargs)
```

### Comparing `starsim-0.1.5/starsim/people.py` & `starsim-0.3.2/starsim/people.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 """
 
 # %% Imports
 import numpy as np
 import pandas as pd
 import sciris as sc
 import starsim as ss
-import scipy.stats as sps
 
 __all__ = ['BasePeople', 'People']
 
 # %% Main people class
 class BasePeople(sc.prettyobj):
     """
     A class to handle all the boilerplate for people -- everything interesting 
     happens in the People class, whereas this class exists to handle the less 
     interesting implementation details.
     """
 
-    def __init__(self, n):
+    def __init__(self, n_agents):
 
         self.initialized = False
-        self._uid_map = ss.DynamicView(int, fill_value=ss.INT_NAN)  # This variable tracks all UIDs ever created
-        self.uid = ss.DynamicView(int, fill_value=ss.INT_NAN)  # This variable tracks all UIDs currently in use
+        self._uid_map = ss.ArrayView(int, default=ss.INT_NAN)  # This variable tracks all UIDs ever created
+        self.uid = ss.ArrayView(int, default=ss.INT_NAN)  # This variable tracks all UIDs currently in use
+
+        n = int(n_agents)
 
         self._uid_map.grow(n)
         self._uid_map[:] = np.arange(0, n)
         self.uid.grow(n)
         self.uid[:] = np.arange(0, n)
 
         # A slot is a special state managed internally by BasePeople
@@ -44,42 +45,43 @@
         # We also internally store states in a dict keyed by the memory ID of the state, so that we can have colliding names
         # e.g., across modules, but we will never change the size of a State multiple times in the same iteration over
         # _states. This is a hidden variable because it is internally used to synchronize the size of all States contained
         # within the sim, regardless of where they are. In contrast, `People.states` offers a more user-friendly way to access
         # a selection of the states e.g., module states could be added in there, while intervention states might not
         self._states = {}
 
-    @property
-    def rngs(self):
-        return [x for x in self.__dict__.values() if isinstance(x, (ss.MultiRNG, ss.SingleRNG))]
-
     def __len__(self):
         """ Length of people """
         return len(self.uid)
 
-    def add_state(self, state, die=True):
+    def register_state(self, state, die=True):
+        """
+        Register a state with the People instance for dynamic resizing
+
+        All states should be registered by this function for the purpose of connecting them to the
+        People's UIDs and to have them be automatically resized when the number of agents changes.
+        This operation is normally triggered as part of initializing the state (via `State.initialize()`)
+        """
         if id(state) not in self._states:
             self._states[id(state)] = state
-            self.states.append(state)  # Expose these states with their original names
-            setattr(self, state.name, state)
         elif die:
             errormsg = f'Cannot add state {state} since already added'
             raise ValueError(errormsg)
         return
 
     def grow(self, n, new_slots=None):
         """
         Increase the number of agents
 
         :param n: Integer number of agents to add
         :param new_slots: Optionally specify the slots to assign for the new agents. Otherwise, it will default to the new UIDs
         """
 
         if n == 0:
-            return np.array([], dtype=ss.int_)
+            return np.array([], dtype=ss.dtypes.int)
 
         start_uid = len(self._uid_map)
         start_idx = len(self.uid)
 
         new_uids = np.arange(start_uid, start_uid + n)
         new_inds = np.arange(start_idx, start_idx + n)
 
@@ -114,18 +116,14 @@
         for state in self._states.values(): # includes self.slot
             state._trim(keep_inds)
 
         # Update the UID map
         self._uid_map[:] = ss.INT_NAN  # Clear out all previously used UIDs
         self._uid_map[keep_uids] = np.arange(0, len(keep_uids))  # Assign the array indices for all of the current UIDs
 
-        # Remove the UIDs from the network too
-        for network in self.networks.values():
-            network.remove_uids(uids_to_remove)
-
         return
 
     def __getitem__(self, key):
         """
         Allow people['attr'] instead of getattr(people, 'attr')
         If the key is an integer, alias `people.person()` to return a `Person` instance
         """
@@ -139,14 +137,25 @@
         return self.__setattr__(key, value)
 
     def __iter__(self):
         """ Iterate over people """
         for i in range(len(self)):
             yield self[i]
 
+    def __setstate__(self, state):
+        """
+        Set the state upon unpickling/deepcopying
+
+        If a People instance is copied (by any mechanism) then the keys in the `_states`
+        registry will no longer match the memory addresses of the new copied states. Therefore,
+        after copying, we need to re-create the states registry with the new object IDs
+        """
+        state['_states'] =  {id(v):v for v in state['_states'].values()}
+        self.__dict__ = state
+
 
 class People(BasePeople):
     """
     A class to perform all the operations on the people
     This class is usually created automatically by the sim. The only required input
     argument is the population size, but typically the full parameters dictionary
     will get passed instead since it will be needed before the People object is
@@ -162,88 +171,101 @@
         pop_trend (dataframe): a dataframe of years and population sizes, if available
         kwargs (dict): the actual data, e.g. from a popdict, being specified
 
     **Examples**::
         ppl = ss.People(2000)
     """
 
-    def __init__(self, n, age_data=None, extra_states=None, networks=None, rand_seed=0):
+    def __init__(self, n_agents, age_data=None, extra_states=None, rand_seed=0):
         """ Initialize """
 
-        super().__init__(n)
+        super().__init__(n_agents)
 
         self.initialized = False
         self.version = ss.__version__  # Store version info
 
         # Handle states
         states = [
             ss.State('age', float, np.nan), # NaN until conceived
-            ss.State('female', bool, sps.bernoulli(p=0.5)),
-            ss.State('debut', float),
+            ss.State('female', bool, ss.bernoulli(name='female', p=0.5)),
             ss.State('ti_dead', int, ss.INT_NAN),  # Time index for death
             ss.State('alive', bool, True),  # Time index for death
             ss.State('scale', float, 1.0),
         ]
         states.extend(sc.promotetolist(extra_states))
+
+        # Expose states with their original names directly as people attributes (e.g., `People.age`) and nested under states
+        # (e.g., `People.states.age`)
         for state in states:
-            self.add_state(state)
-        self._initialize_states(sim=None) # No sim yet, but initialize what we can
-        
-        self.networks = ss.Networks(networks)
+            self.states.append(state, overwrite=False)
+            setattr(self, state.name, state)
 
         # Set initial age distribution - likely move this somewhere else later
         self.age_data_dist = self.get_age_dist(age_data)
 
         return
 
     @staticmethod
     def get_age_dist(age_data):
         """ Return an age distribution based on provided data """
         if age_data is None:
-            dist = sps.uniform(loc=0, scale=100)  # loc and width
-            return ss.ScipyDistribution(dist, 'Age distribution')
+            dist = ss.uniform(low=0, high=100, name='Age distribution')
+            return dist
 
         if sc.checktype(age_data, pd.DataFrame):
-            bb = np.append(age_data['age'].values, age_data['age'].values[-1] + 1)
-            vv = age_data['value'].values
-            return ss.ScipyHistogram((vv, bb), density=False, rng='Age distribution')
+            age_bins = age_data['age'].values
+            age_props = age_data['value'].values
+            age_props = age_props / age_props.sum()
+            return ss.choice(a=age_bins, p=age_props)
 
-    def _initialize_states(self, sim=None):
-        for state in self.states.values():
-            state.initialize(sim=sim, people=self)  # Connect the state to this people instance
-        return
 
     def initialize(self, sim):
         """ Initialization """
-    
+
+        if self.initialized:
+            return
+        else:
+            self.initialized = True # Expected by state.initialize()
+        
         # For People initialization, first initialize slots, then initialize RNGs, then initialize remaining states
         # This is because some states may depend on RNGs being initialized to generate initial values
         self.slot.initialize(sim)
         self.slot[:] = self.uid
-    
-        # Initialize all RNGs (noting that includes those that are declared in child classes)
-        for rng in self.rngs:
-            rng.initialize(sim.rng_container, self.slot)
-
-        self.age_data_dist.initialize(sim, self)
-            
-        # Define age (CK: why is age handled differently than sex?)
-        self._initialize_states(sim=sim)  # Now initialize with the sim
-        self.age[:] = self.age_data_dist.rvs(size=self.uid)
-        self.initialized = True
+
+        # Initialize states
+        # Age is handled separately because the default value for new agents is NaN until they are concieved/born whereas
+        # the initial values need to depend on the current age distribution for the setting. In contrast, the sex for new
+        # agents can be sampled from the same distribution used to initialize the population
+        for state in self.states.values():
+            state.initialize(sim)
+
+        # Assign initial ages based on the current age distribution
+        self.age_data_dist.initialize(module=self, sim=sim)
+        self.age[:] = self.age_data_dist.rvs(self.uid)
         return
 
     def add_module(self, module, force=False):
+        """
+        Add a Module to the People instance
+
+        This method is used to add a module to the People. It will register any module states with this
+        people instance for dynamic resizing, and expose the states contained in the module to the user
+        via `People.states.<module_name>.<state_name>`
+        :param module:
+        :param force:
+        :return:
+        """
         # Map the module's states into the People state ndict
         if hasattr(self, module.name) and not force:
             raise Exception(f'Module {module.name} already added')
         self.__setattr__(module.name, sc.objdict())
 
         # The entries created below make it possible to do `sim.people.hiv.susceptible` or
         # `sim.people.states['hiv.susceptible']` and have both of them work
+
         module_states = sc.objdict()
         setattr(self, module.name, module_states)
         self._register_module_states(module, module_states)
         return
 
     def _register_module_states(self, module, module_states):
         """Enable dot notation for module specific states:
@@ -269,14 +291,19 @@
     def remove_dead(self, sim):
         """
         Remove dead agents
         """
         uids_to_remove = ss.true(self.dead)
         if len(uids_to_remove):
             self.remove(uids_to_remove)
+
+        # Remove the UIDs from the network too
+        for network in sim.networks.values():
+            network.remove_uids(uids_to_remove)
+
         return
 
     def update_post(self, sim):
         """
         Final updates at the very end of the timestep
 
         :param sim:
@@ -291,24 +318,14 @@
 
         :return:
         """
         death_uids = ss.true(self.ti_dead <= self.ti)
         self.alive[death_uids] = False
         return death_uids
 
-    def update_networks(self):
-        """
-        Update networks
-        """
-        return self.networks.update(self)
-
-    @property
-    def active(self):
-        """ Indices of everyone sexually active  """
-        return (self.age >= self.debut) & self.alive
 
     @property
     def dead(self):
         """ Dead boolean """
         return ~self.alive
 
     @property
@@ -323,21 +340,26 @@
 
     @property
     def m(self):
         """ Shorthand for male """
         return self.male
 
     def init_results(self, sim):
-        sim.results += ss.Result(None, 'n_alive', sim.npts, ss.int_, scale=True)
-        sim.results += ss.Result(None, 'new_deaths', sim.npts, ss.int_, scale=True)
+        sim.results += [
+            ss.Result(None, 'n_alive', sim.npts, ss.dtypes.int, scale=True),
+            ss.Result(None, 'new_deaths', sim.npts, ss.dtypes.int, scale=True),
+            ss.Result(None, 'cum_deaths', sim.npts, ss.dtypes.int, scale=True),
+        ]
         return
 
     def update_results(self, sim):
-        sim.results.n_alive[self.ti] = np.count_nonzero(self.alive)
-        sim.results.new_deaths[self.ti] = np.count_nonzero(self.ti_dead == self.ti)
+        res = sim.results
+        res.n_alive[self.ti] = np.count_nonzero(self.alive)
+        res.new_deaths[self.ti] = np.count_nonzero(self.ti_dead == self.ti)
+        res.cum_deaths[self.ti] = np.sum(res.new_deaths[:sim.ti])
         return
 
     def request_death(self, uids):
         """
         External-facing function to request an agent die at the current timestep
 
         In general, users should not directly interact with `People.ti_dead` to minimize
```

### Comparing `starsim-0.1.5/starsim/settings.py` & `starsim-0.3.2/starsim/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,25 @@
 """
 
 import os
 import numpy as np
 import sciris as sc
 
 
-__all__ = ['options', 'float_', 'int_']
+__all__ = ['INT_NAN', 'dtypes', 'options']
 
+INT_NAN = 2147483647 # From np.iinfo(np.int32).max: value to use to flag invalid content (i.e., an integer value we are treating like NaN, since NaN can't be stored in an integer array)
+
+# Define Starsim-default data types
+dtypes = sc.objdict(
+    bool = bool,
+    int = np.int64,
+    float = np.float64,
+    result_float = np.float64,
+)
 
 # Not public to avoid confusion with ss.options
 class Options(sc.objdict):
     """
     Set options for Starsim.
 
     Use ``ss.options.set('defaults')`` to reset all values to default, or ``ss.options.set(dpi='default')``
@@ -52,31 +61,25 @@
         ``ss.options.set('defaults')`` instead.
         """
 
         # Options acts like a class, but is actually an objdict for simplicity
         optdesc = sc.objdict()  # Help for the options
         options = sc.objdict()  # The options
 
-        optdesc.multirng = 'Set True to use multiple random number generators\
-            via the MultiRNG class, which is compatible with common random\
-            numbers. The default value is False, which instead uses a single\
-            centralized random number generator.'
-        options.multirng = False
-
         optdesc.verbose = 'Set default level of verbosity (i.e. logging detail): e.g., 0.1 is an update every 10 simulated timesteps.'
         options.verbose = float(os.getenv('STARSIM_VERBOSE', 0.1))
 
         optdesc.warnings = 'How warnings are handled: options are "warn" (default), "print", and "error"'
         options.warnings = str(os.getenv('STARSIM_WARNINGS', 'warn'))
 
         optdesc.sep = 'Set thousands seperator for text output'
         options.sep = str(os.getenv('STARSIM_SEP', ','))
 
         optdesc.precision = 'Set arithmetic precision -- 32-bit by default for efficiency'
-        options.precision = int(os.getenv('STARSIM_PRECISION', 32))
+        options.precision = int(os.getenv('STARSIM_PRECISION', 64))
 
         return optdesc, options
 
     def __call__(self, *args, **kwargs):
         """Allow ``ss.options(dpi=150)`` instead of ``ss.options.set(dpi=150)`` """
 
         return self.set(*args, **kwargs)
@@ -147,39 +150,38 @@
                 keys = '\n'.join(keylist)
                 errormsg = f'Option "{key}" not recognized; options are "defaults" or:\n{keys}\n\nSee help(ss.options.set) for more information.'
                 raise sc.KeyNotFoundError(errormsg)
             else:
                 if value in [None, 'default']:
                     value = self.orig_options[key]
                 self[key] = value
+                
+                # Handle special cases
+                if key == 'precision':
+                    self.reset_precision()
 
         return
 
     def context(self, **kwargs):
         """
-        Alias to set() for non-plotting options, for use in a "with" block.
-
-        Note: for plotting options, use ``ss.options.with_style()``, which is linked
-        to Matplotlib's context manager. If you set plotting options with this,
-        they won't have any effect.
+        Alias to set(), for use in a "with" block.
 
         **Examples**::
 
             # Silence all output
             with ss.options.context(verbose=0):
                 ss.Sim().run()
 
             # Convert warnings to errors
             with ss.options.context(warnings='error'):
                 ss.Sim(location='not a location').initialize()
 
             # Use with_style(), not context(), for plotting options
             with ss.options.with_style(dpi=50):
                 ss.Sim().run().plot()
-
         """
 
         # Store current settings
         on_entry = {k: self[k] for k in kwargs.keys()}
         self.setattribute('on_entry', on_entry)
 
         # Make changes
@@ -192,25 +194,23 @@
 
     def changed(self, key):
         """ Check if current setting has been changed from default """
         if key in self.orig_options:
             return self[key] != self.orig_options[key]
         else:
             return None
+    
+    def set_precision(self):
+        if self.precision == 32:
+            dtypes.int = np.int32
+            dtypes.float = np.float32
+        elif self.precision == 64:
+            dtypes.int = np.int64
+            dtypes.float = np.float64
+        else:
+            errormsg = f'Precision {self.precision} not recognized; must be 32 or 64'
+            raise ValueError(errormsg)
+        return
 
 
-# Create the options on module load, and load the fonts
+# Create the options on module load
 options = Options()
-
-# Default for precision
-# Used in various places throughout the code, generally as:
-#   import stisim.settings as sss
-#   arr = np.full(100, 0, sss.float_)
-result_float = np.float64  # Always use float64 for results, for simplicity
-if options.precision == 32:
-    float_ = np.float32
-    int_ = np.int32
-elif options.precision == 64:  # pragma: no cover
-    float_ = np.float64
-    int_ = np.int64
-else:
-    raise NotImplementedError(f'Precision must be either 32 bit or 64 bit, not {options.precision}')
```

### Comparing `starsim-0.1.5/starsim/sim.py` & `starsim-0.3.2/starsim/sim.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,109 +3,113 @@
 """
 
 # Imports
 import numpy as np
 import sciris as sc
 import starsim as ss
 import itertools
-import numba as nb
+import matplotlib.pyplot as pl
 
-__all__ = ['Sim', 'AlreadyRunError', 'diff_sims']
+__all__ = ['Sim', 'AlreadyRunError', 'demo', 'diff_sims']
 
-@nb.njit
-def set_numba_seed(value):
-    # Needed to ensure reproducibility when using random calls in numba, e.g. RandomNetwork
-    # Note, these random numbers are not currently common-random-number safe
-    np.random.seed(value)
 
 class Sim(sc.prettyobj):
 
-    def __init__(self, pars=None, label=None, people=None, demographics=None, diseases=None, connectors=None, **kwargs):
+    def __init__(self, pars=None, label=None, people=None, demographics=None, diseases=None, networks=None,
+                 connectors=None, interventions=None, analyzers=None, **kwargs):
 
         # Set attributes
         self.label = label  # The label/name of the simulation
         self.created = None  # The datetime the sim was created
         self.people = people  # People object
-        self.demographics  = ss.ndict(demographics, type=ss.DemographicModule)
-        self.diseases      = ss.ndict(diseases, type=ss.Disease)
-        self.connectors    = ss.ndict(connectors, type=ss.Connector)
-        self.results       = ss.ndict(type=ss.Result)  # For storing results
-        self.summary       = None  # For storing a summary of the results
-        self.initialized   = False  # Whether initialization is complete
-        self.complete      = False  # Whether a simulation has completed running # TODO: replace with finalized?
+        self.results = ss.Results(module='sim')  # For storing results
+        self.summary = None  # For storing a summary of the results
+        self.initialized = False  # Whether initialization is complete
+        self.complete = False  # Whether a simulation has completed running # TODO: replace with finalized?
         self.results_ready = False  # Whether results are ready
-        self.filename      = None
+        self.filename = None
 
         # Time indexing
-        self.ti      = None  # The time index, e.g. 0, 1, 2 # TODO: do we need all of these?
+        self.ti = None  # The time index, e.g. 0, 1, 2 # TODO: do we need all of these?
         self.yearvec = None
-        self.tivec   = None
-        self.npts    = None
+        self.tivec = None
+        self.npts = None
 
         # Make default parameters (using values from parameters.py)
         self.pars = ss.make_pars()  # Start with default pars
         self.pars.update_pars(sc.mergedicts(pars, kwargs))  # Update the parameters
 
-        # Initialize other quantities
-        self.interventions = ss.ndict(type=ss.Intervention)
-        self.analyzers = ss.ndict(type=ss.Analyzer)
+        # Placeholders for plug-ins: demographics, diseases, connectors, analyzers, and interventions
+        # Products are not here because they are stored within interventions
+        if demographics == True: demographics = [ss.Births(), ss.Deaths()]  # Use default assumptions for demographics
+        self.demographics  = ss.ndict(demographics, type=ss.Demographics)
+        self.diseases      = ss.ndict(diseases, type=ss.Disease)
+        self.networks      = ss.ndict(networks, type=ss.Network)
+        self.connectors    = ss.ndict(connectors, type=ss.Connector)
+        self.interventions = ss.ndict(interventions, type=ss.Intervention, strict=False) # strict=False since can be a function
+        self.analyzers     = ss.ndict(analyzers, type=ss.Analyzer, strict=False)
 
         # Initialize the random number generator container
-        self.rng_container = ss.RNGContainer()
+        self.dists = ss.Dists(obj=self)
 
         return
 
     @property
     def dt(self):
-        return self.pars['dt']
+        if 'dt' in self.pars:
+            return self.pars['dt']
+        else:
+            return np.nan
 
     @property
     def year(self):
-        return self.yearvec[self.ti]
+        try:
+            return self.yearvec[self.ti]
+        except:
+            return np.nan
 
     @property
     def modules(self):
         # Return iterator over all Module instances (stored in standard places) in the Sim
+        products = [intv.product for intv in self.interventions.values() if
+                    hasattr(intv, 'product') and isinstance(intv.product, ss.Product)]
         return itertools.chain(
             self.demographics.values(),
-            self.people.networks.values(),
+            self.networks.values(),
             self.diseases.values(),
             self.connectors.values(),
             self.interventions.values(),
+            products,
             self.analyzers.values(),
         )
 
-    def initialize(self, popdict=None, reset=False, **kwargs):
+    def initialize(self, reset=False, **kwargs):
         """
         Perform all initializations on the sim.
         """
         # Validation and initialization
         self.ti = 0  # The current time index
         self.validate_pars()  # Ensure parameters have valid values
         self.validate_dt()
         self.init_time_vecs()  # Initialize time vecs
-        ss.set_seed(self.pars['rand_seed'])  # Reset the random seed before the population is created
-        set_numba_seed(self.pars['rand_seed'])
+        ss.set_seed(self.pars.rand_seed)  # Reset the seed before the population is created -- shouldn't matter if only using Dist objects
 
         # Initialize the core sim components
-        self.rng_container.initialize(self.pars['rand_seed'] + 2) # +2 ensures that seeds from the above population initialization and the +1-offset below are not reused within the rng_container
         self.init_people(reset=reset, **kwargs)  # Create all the people (the heaviest step)
+
+        # Initialize plug-ins
         self.init_demographics()
         self.init_networks()
         self.init_diseases()
         self.init_connectors()
         self.init_interventions()
         self.init_analyzers()
 
-        # Perform post-initialization validation
-        self.validate_post_init()
-
-        # Reset the random seed to the default run seed, so that if the simulation is run with
-        # reset_seed=False right after initialization, it will still produce the same output
-        ss.set_seed(self.pars['rand_seed'] + 1) # Hopefully not used now that we can use multiple random number generators
+        # Initialize all distributions now that everything else is in place
+        self.dists.initialize(obj=self, base_seed=self.pars.rand_seed, force=True)
 
         # Final steps
         self.initialized = True
         self.complete = False
         self.results_ready = False
 
         return self
@@ -117,64 +121,63 @@
         """
         dt = self.dt
         reciprocal = 1.0 / dt  # Compute the reciprocal of dt
         if not reciprocal.is_integer():  # Check if reciprocal is not a whole (integer) number
             # Round the reciprocal
             reciprocal = int(reciprocal)
             rounded_dt = 1.0 / reciprocal
-            self.pars['dt'] = rounded_dt
-            if self.pars['verbose']:
+            self.pars.dt = rounded_dt
+            if self.pars.verbose:
                 warnmsg = f"Warning: Provided time step dt: {dt} resulted in a non-integer number of steps per year. Rounded to {rounded_dt}."
                 print(warnmsg)
         return
 
     def validate_pars(self):
         """
         Some parameters can take multiple types; this makes them consistent.
         """
         # Handle n_agents
         if self.people is not None:
-            self.pars['n_agents'] = len(self.people)
-        #elif self.popdict is not None: # Starsim does not currenlty support self.popdict
-            #self.pars['n_agents'] = len(self.popdict)
-        elif self.pars['n_agents'] is not None:
-            self.pars['n_agents'] = int(self.pars['n_agents'])
+            self.pars.n_agents = len(self.people)
+        # elif self.popdict is not None: # Starsim does not currenlty support self.popdict
+        # self.pars.n_agents = len(self.popdict)
+        elif self.pars.n_agents is not None:
+            self.pars.n_agents = int(self.pars.n_agents)
         else:
             errormsg = 'Must supply n_agents, a people object, or a popdict'
             raise ValueError(errormsg)
 
         # Handle end and n_years
-        if self.pars['end']:
-            self.pars['n_years'] = int(self.pars['end'] - self.pars['start'])
-            if self.pars['n_years'] <= 0:
-                errormsg = f"Number of years must be >0, but you supplied start={str(self.pars['start'])} and " \
-                           f"end={str(self.pars['end'])}, which gives n_years={self.pars['n_years']}"
+        if self.pars.end:
+            self.pars.n_years = self.pars.end - self.pars.start
+            if self.pars.n_years <= 0:
+                errormsg = f"Number of years must be >0, but you supplied start={str(self.pars.start)} and " \
+                           f"end={str(self.pars.end)}, which gives n_years={self.pars.n_years}"
                 raise ValueError(errormsg)
         else:
-            if self.pars['n_years']:
-                self.pars['end'] = self.pars['start'] + self.pars['n_years']
+            if self.pars.n_years:
+                self.pars.end = self.pars.start + self.pars.n_years
             else:
                 errormsg = 'You must supply one of n_years and end."'
                 raise ValueError(errormsg)
 
         # Handle verbose
-        if self.pars['verbose'] == 'brief':
-            self.pars['verbose'] = -1
-        if not sc.isnumber(self.pars['verbose']):  # pragma: no cover
-            errormsg = f'Verbose argument should be either "brief", -1, or a float, not {type(self.pars["verbose"])} "{self.pars["verbose"]}"'
+        if self.pars.verbose == 'brief':
+            self.pars.verbose = -1
+        if not sc.isnumber(self.pars.verbose):  # pragma: no cover
+            errormsg = f'Verbose argument should be either "brief", -1, or a float, not {type(self.par.verbose)} "{self.par.verbose}"'
             raise ValueError(errormsg)
 
         return
 
     def init_time_vecs(self):
         """
         Construct vectors things that keep track of time
         """
-        self.yearvec = sc.inclusiverange(start=self.pars['start'], stop=self.pars['end'] + 1 - self.pars['dt'],
-                                         step=self.pars['dt'])  # Includes all the timepoints in the last year
+        self.yearvec = np.arange(start=self.pars.start, stop=self.pars.end + self.pars.dt, step=self.pars.dt)
         self.npts = len(self.yearvec)
         self.tivec = np.arange(self.npts)
         return
 
     def init_people(self, reset=False, verbose=None, **kwargs):
         """
         Initialize people within the sim
@@ -184,199 +187,314 @@
             reset           (bool): whether to regenerate the people even if they already exist
             verbose         (int):  detail to print
             kwargs          (dict): passed to ss.make_people()
         """
 
         # Handle inputs
         if verbose is None:
-            verbose = self.pars['verbose']
+            verbose = self.pars.verbose
         if verbose > 0:
             resetstr = ''
             if self.people and reset:
                 resetstr = ' (resetting people)'
             print(f'Initializing sim{resetstr} with {self.pars["n_agents"]:0n} agents')
 
         # If people have not been supplied, make them
         if self.people is None or reset:
-            self.people = ss.People(n=self.pars['n_agents'], **kwargs)  # This just assigns UIDs and length
+            self.people = ss.People(n_agents=self.pars.n_agents, **kwargs)  # This just assigns UIDs and length
 
         # If a popdict has not been supplied, we can make one from location data
-        if self.pars['location'] is not None:
+        if self.pars.location is not None:
             # Check where to get total_pop from
-            if self.pars['total_pop'] is not None:  # If no pop_scale has been provided, try to get it from the location
+            if self.pars.total_pop is not None:  # If no pop_scale has been provided, try to get it from the location
                 errormsg = 'You can either define total_pop explicitly or via the location, but not both'
                 raise ValueError(errormsg)
 
         else:
-            if self.pars['total_pop'] is not None:  # If no pop_scale has been provided, try to get it from the location
-                total_pop = self.pars['total_pop']
+            if self.pars.total_pop is not None:  # If no pop_scale has been provided, try to get it from the location
+                total_pop = self.pars.total_pop
             else:
-                if self.pars['pop_scale'] is not None:
-                    total_pop = self.pars['pop_scale'] * self.pars['n_agents']
+                if self.pars.pop_scale is not None:
+                    total_pop = self.pars.pop_scale * self.pars.n_agents
                 else:
-                    total_pop = self.pars['n_agents']
+                    total_pop = self.pars.n_agents
 
-        self.pars['total_pop'] = total_pop
-        if self.pars['pop_scale'] is None:
-            self.pars['pop_scale'] = total_pop / self.pars['n_agents']
+        self.pars.total_pop = total_pop
+        if self.pars.pop_scale is None:
+            self.pars.pop_scale = total_pop / self.pars.n_agents
 
         # Any other initialization
         if not self.people.initialized:
             self.people.initialize(self)
 
         # Set time attributes
         self.people.ti = self.ti
         self.people.dt = self.dt
         self.people.year = self.year
         self.people.init_results(self)
         return self
 
+    def convert_plugins(self, plugin_class, plugin_name=None):
+        """
+        Common logic for converting plug-ins to a standard format
+        Used for networks, demographics, diseases, connectors, analyzers, and interventions
+        Args:
+            plugin: class
+        """
+
+        if plugin_name is None: plugin_name = plugin_class.__name__.lower()
+
+        # Get lower-case names of all subclasses
+        known_plugins = {n.__name__.lower():n for n in ss.all_subclasses(plugin_class)}
+        if plugin_name == 'networks': # Allow "msm" or "msmnet"
+            known_plugins.update({k.removesuffix('net'):v for k,v in known_plugins.items()})
+
+        # Figure out if it's in the sim pars or provided directly
+        attr_plugins = getattr(self, plugin_name)  # Get any plugins that have been provided directly
+
+        # See if they've been provided in the pars dict
+        if self.pars.get(plugin_name):
+
+            par_plug = self.pars[plugin_name]
+
+            # String: convert to ndict
+            if isinstance(par_plug, str):
+                plugins = ss.ndict(dict(name=par_plug))
+
+            # List or dict: convert to ndict
+            elif sc.isiterable(par_plug) and len(par_plug):
+                if isinstance(par_plug, dict) and 'type' in par_plug and 'name' not in par_plug:
+                    par_plug['name'] = par_plug['type'] # TODO: simplify/remove this
+                plugins = ss.ndict(par_plug)
+
+        else:  # Not provided directly or in pars
+            plugins = {}
+
+        # Check that we don't have two copies
+        for attr_key in attr_plugins.keys():
+            if plugins.get(attr_key):
+                errormsg = f'Sim was created with {attr_key} module, cannot create another through the pars dict.'
+                raise ValueError(errormsg)
+
+        plugins = sc.mergedicts(plugins, attr_plugins)
+
+        # Process
+        processed_plugins = sc.autolist()
+        for plugin in plugins.values():
+
+            if not isinstance(plugin, plugin_class):
+
+                if isinstance(plugin, dict):
+                    ptype = (plugin.get('type') or plugin.get('name') or '').lower()
+                    name = plugin.get('name') or ptype
+                    if ptype in known_plugins:
+                        # Make an instance of the requested plugin
+                        plugin_pars = {k: v for k, v in plugin.items() if k not in ['type', 'name']}
+                        pclass = known_plugins[ptype]
+                        plugin = pclass(name=name, pars=plugin_pars) # TODO: does this handle par_dists, etc?
+                    else:
+                        errormsg = (f'Could not convert {plugin} to an instance of class {plugin_name}.'
+                                    f'Try specifying it directly rather than as a dictionary.')
+                        raise ValueError(errormsg)
+                elif plugin_name in ['analyzers', 'interventions'] and callable(plugin):
+                    pass # This is ok, it's a function instead of an Intervention object
+                else:
+                    errormsg = (
+                        f'{plugin_name.capitalize()} must be provided as either class instances or dictionaries with a '
+                        f'"name" key corresponding to one of these known subclasses: {known_plugins}.')
+                    raise ValueError(errormsg)
+
+            processed_plugins += plugin
+
+        return processed_plugins
+
     def init_demographics(self):
-        for module in self.demographics.values():
-            module.initialize(self)
-            self.results[module.name] = module.results
+        """ Initialize demographics """
+
+        # Demographics can be provided via sim.demographics or sim.pars - this methods reconciles them
+        demographics = self.convert_plugins(ss.Demographics, plugin_name='demographics')
+
+        # We also allow users to add vital dynamics by entering birth_rate and death_rate parameters directly to the sim
+        if self.pars.birth_rate is not None:
+            births = ss.Births(pars={'birth_rate': self.pars.birth_rate})
+            demographics += births
+        if self.pars.death_rate is not None:
+            background_deaths = ss.Deaths(pars={'death_rate': self.pars.death_rate})
+            demographics += background_deaths
+
+        # Iterate over demographic modules and initialize them
+        for dem_mod in demographics:
+            dem_mod.initialize(self)
+            self.results[dem_mod.name] = dem_mod.results
+
+        # Count how many of each kind of demographic module we have
+        demdict = {'births': ss.Births, 'pregnancy': ss.Pregnancy, 'deaths': ss.Deaths}
+        mod_names = dict()
+        for demname, demtype in demdict.items():
+            mod_names[demname] = [d.name for d in demographics if isinstance(d, demtype)]
+
+            # Validation
+            if len(mod_names[demname]) > 1:
+                if len(mod_names[demname]) == len(set(mod_names[demname])):  # No duplicate names, raise warning
+                    ss.warn(f'Two instances of {demname} module added to the sim; was this intentional?')
+                else:
+                    errormsg = (f'Cannot add two identically-named {demname} modules to a sim.\n '
+                                f'Demographic modules are: \n{sc.newlinejoin(mod_names[demname])}.\n'
+                                f'Tip: if using demographic modules, do not use birth and death rates in the sim pars.')
+                    raise ValueError(errormsg)
+
+        # Ensure they're stored at the sim level
+        self.demographics = ss.ndict(*demographics)
 
     def init_diseases(self):
-        """ Initialize modules and connectors to be simulated """
-        for disease in self.diseases.values():
+        """ Initialize diseases """
+
+        # Diseases can be provided in sim.demographics or sim.pars
+        diseases = self.convert_plugins(ss.Disease, plugin_name='diseases')
+
+        # Interate over diseases and initialize them
+        for disease in diseases:
             disease.initialize(self)
 
             # Add the disease's parameters and results into the Sim's dicts
             self.pars[disease.name] = disease.pars
             self.results[disease.name] = disease.results
 
             # Add disease states to the People's dicts
             self.people.add_module(disease)
 
+        # Store diseases in the sim
+        self.diseases = ss.ndict(*diseases)
+
         return
 
     def init_connectors(self):
         for connector in self.connectors.values():
             connector.initialize(self)
 
     def init_networks(self):
         """ Initialize networks if these have been provided separately from the people """
 
-        # One possible workflow is that users will provide a location and a set of networks but not people.
-        # This means networks will be stored in self.pars['networks'] and we'll need to copy them to the people.
-        if self.people.networks is None or len(self.people.networks) == 0:
-            if self.pars['networks'] is not None:
-                self.people.networks = ss.Networks(self.pars['networks'])
-
-        if not isinstance(self.people.networks, ss.Networks):
-            self.people.networks = ss.Networks(networks=self.people.networks)
-
-        self.people.networks.initialize(self)
-
-        # for key, network in self.people.networks.networks.items():  # TODO rename
-            # if network.label is not None:
-            #     layer_name = network.label
-            # else:
-            #     layer_name = key
-            #     network.label = layer_name
-            # network.initialize(self)
-
-            # Add network states to the People's dicts
-            # self.people.add_module(network)
-            # self.people.networks[network.name] = network
+        processed_networks = self.convert_plugins(ss.Network, plugin_name='networks')
+
+        # Now store the networks in a Networks object, which also allows for connectors between networks
+        if not isinstance(processed_networks, ss.Networks):
+            self.networks = ss.Networks(*processed_networks)
+        self.networks.initialize(self)
 
         return
 
     def init_interventions(self):
         """ Initialize and validate the interventions """
 
+        interventions = self.convert_plugins(ss.Intervention, plugin_name='interventions')
+
         # Translate the intervention specs into actual interventions
-        for i, intervention in enumerate(self.pars['interventions']):
+        for i, intervention in enumerate(interventions):
             if isinstance(intervention, type) and issubclass(intervention, ss.Intervention):
                 intervention = intervention()  # Convert from a class to an instance of a class
             if isinstance(intervention, ss.Intervention):
                 intervention.initialize(self)
-                self.interventions += intervention
             elif callable(intervention):
-                self.interventions += intervention
+                intv_func = intervention
+                intervention = ss.Intervention(name=f'intervention_func_{i}')
+                intervention.apply = intv_func # Monkey-patch together an intervention from a function
             else:
                 errormsg = f'Intervention {intervention} does not seem to be a valid intervention: must be a function or Intervention subclass'
                 raise TypeError(errormsg)
-
-            for rng in intervention.rngs:
-                rng.initialize(self.rng_container, self.people.slot)
+            
+            if intervention.name not in self.interventions:
+                self.interventions += intervention
 
             # Add the intervention parameters and results into the Sim's dicts
             self.pars[intervention.name] = intervention.pars
             self.results[intervention.name] = intervention.results
 
             # Add intervention states to the People's dicts
             self.people.add_module(intervention)
 
+            # If there's a product module present, initialize and add it
+            if hasattr(intervention, 'product') and isinstance(intervention.product, ss.Product):
+                intervention.product.initialize(self)
+
+                self.people.add_module(intervention.product)
+        
+        # TODO: combine this with the code above
+        for k,intervention in self.interventions.items():
+            if not isinstance(intervention, ss.Intervention):
+                intv_func = intervention
+                intervention = ss.Intervention(name=f'intervention_func_{k}')
+                intervention.apply = intv_func # Monkey-patch together an intervention from a function
+                self.interventions[k] = intervention
+
         return
 
     def init_analyzers(self):
         """ Initialize the analyzers """
+        
+        analyzers = self.pars.analyzers
+        if not np.iterable(analyzers):
+            analyzers = sc.tolist(analyzers)
 
         # Interpret analyzers
-        for ai, analyzer in enumerate(self.pars['analyzers']):
+        for ai, analyzer in enumerate(analyzers):
             if isinstance(analyzer, type) and issubclass(analyzer, ss.Analyzer):
                 analyzer = analyzer()  # Convert from a class to an instance of a class
             if not (isinstance(analyzer, ss.Analyzer) or callable(analyzer)):
                 errormsg = f'Analyzer {analyzer} does not seem to be a valid analyzer: must be a function or Analyzer subclass'
                 raise TypeError(errormsg)
             self.analyzers += analyzer  # Add it in
 
-        for analyzer in self.analyzers.values():
+        # TODO: should tidy/remove this code
+        for k,analyzer in self.analyzers.items():
+            if not isinstance(analyzer, ss.Analyzer) and callable(analyzer):
+                ana_func = analyzer
+                analyzer = ss.Analyzer(name=f'analyzer_func_{k}')
+                analyzer.apply = ana_func # Monkey-patch together an intervention from a function
+                self.analyzers[k] = analyzer
             if isinstance(analyzer, ss.Analyzer):
                 analyzer.initialize(self)
 
         return
 
-    def validate_post_init(self):
-        """
-        Validate inputs again once everything has been initialized.
-        TBC whether we keep this or incorporate the checks into the init methods
-        """
-        # Make sure that there's a contact network if any diseases are present
-        if self.diseases and not self.people.networks:
-            warnmsg = f'Warning: simulation has {len(self.diseases)} diseases but no contact network(s).'
-            ss.warn(warnmsg, die=False)
-        return
-
     def step(self):
         """ Step through time and update values """
 
         # Set the time and if we have reached the end of the simulation, then do nothing
         if self.complete:
             raise AlreadyRunError('Simulation already complete (call sim.initialize() to re-run)')
 
         # Advance random number generators forward to prepare for any random number calls that may be necessary on this step
-        self.rng_container.step(self.ti+1) # +1 offset because ti=0 is used on initialization
+        self.dists.jump(to=self.ti+1)  # +1 offset because ti=0 is used on initialization
 
         # Clean up dead agents, if removing agents is enabled
-        if self.pars.remove_dead:
+        if self.pars.remove_dead and (self.ti % self.pars.remove_dead == 0):
             self.people.remove_dead(self)
 
         # Update demographic modules (create new agents from births/immigration, schedule non-disease deaths and emigration)
-        for module in self.demographics.values():
-            module.update(self)
+        for dem_mod in self.demographics.values():
+            dem_mod.update(self)
 
         # Carry out autonomous state changes in the disease modules. This allows autonomous state changes/initializations
         # to be applied to newly created agents
         for disease in self.diseases.values():
             disease.update_pre(self)
 
         # Update connectors -- TBC where this appears in the ordering
         for connector in self.connectors.values():
             connector.update(self)
 
         # Update networks - this takes place here in case autonomous state changes at this timestep
         # affect eligibility for contacts
-        self.people.update_networks()
+        self.networks.update(self.people)
 
         # Apply interventions - new changes to contacts will be visible and so the final networks can be customized by
         # interventions, by running them at this point
         for intervention in self.interventions.values():
-            intervention.apply(self)
+            intervention(self)
 
         # Carry out transmission/new cases
         for disease in self.diseases.values():
             disease.make_new_cases(self)
 
         # Execute deaths that took place this timestep (i.e., changing the `alive` state of the agents). This is executed
         # before analyzers have run so that analyzers are able to inspect and record outcomes for agents that died this timestep
@@ -387,40 +505,37 @@
         # Update results
         self.people.update_results(self)
 
         for disease in self.diseases.values():
             disease.update_results(self)
 
         for analyzer in self.analyzers.values():
-            analyzer.update_results(self)
+            analyzer(self)
 
         # Tidy up
         self.ti += 1
         self.people.ti = self.ti
         self.people.update_post(self)
 
         if self.ti == self.npts:
             self.complete = True
 
         return
 
-    def run(self, until=None, reset_seed=True, verbose=None):
+    def run(self, until=None, verbose=None):
         """ Run the model once """
 
         # Initialization steps
         T = sc.timer()
         if not self.initialized:
             self.initialize()
             self._orig_pars = sc.dcp(self.pars)  # Create a copy of the parameters to restore after the run
 
         if verbose is None:
-            verbose = self.pars['verbose']
-
-        if reset_seed:
-            ss.set_seed(self.pars['rand_seed'] + 1)
+            verbose = self.pars.verbose
 
         # Check for AlreadyRun errors
         errormsg = None
         if until is None: until = self.npts
         if until > self.npts:
             errormsg = f'Requested to run until t={until} but the simulation end is ti={self.npts}'
         if self.ti >= until:  # NB. At the start, self.t is None so this check must occur after initialization
@@ -463,33 +578,78 @@
             # Because the results are rescaled in-place, finalizing the sim cannot be run more than once or
             # otherwise the scale factor will be applied multiple times
             raise AlreadyRunError('Simulation has already been finalized')
 
         # Scale the results
         for reskey, res in self.results.items():
             if isinstance(res, ss.Result) and res.scale:
-                self.results[reskey] = self.results[reskey]*self.pars.pop_scale
+                self.results[reskey] = self.results[reskey] * self.pars.pop_scale
 
         for module in self.modules:
             module.finalize(self)
 
         self.summarize()
         self.results_ready = True  # Set this first so self.summary() knows to print the results
         self.ti -= 1  # During the run, this keeps track of the next step; restore this be the final day of the sim
         return
-    
-    def summarize(self):
+
+    def summarize(self, how='default'):
+        """
+        Provide a quick summary of the sim
+        
+        Args:
+            how (str): how to summarize: can be 'mean', 'median', 'last', or a mapping of result keys to those
+        
+        Returns the last entry for count and cumulative results, and the mean otherwise
+        """
+        
+        def get_func(key, how, default='mean'):
+            """
+            Find the right function by matching the "how" key with the result key
+            
+            For example, hkey="cum_ " will match result key "cum_infections"
+            """
+            func = None
+            for hkey,hfunc in how.items():
+                if hkey in key:
+                    func = hfunc
+                    break
+            if func is None:
+                func = default
+            return func
+            
+        def get_result(res, func):
+            """ Convert a string to the actual function to use, e.g. "median" maps to np.median() """
+            if   func == 'mean':   return res.mean()
+            elif func == 'median': return np.median(res)
+            elif func == 'last':   return res[-1]
+            elif callable(func):   return func(res)
+            else: raise Exception(f'"{func}" is not a valid function')
+        
+        # Convert "how" from a string to a dict
+        if how == 'default':
+            how = {'n_':'mean', 'new_':'mean', 'cum_':'last', '':'mean'}
+        elif isinstance(how, str):
+            how = {'':how} # Match everything
+        
         summary = sc.objdict()
         flat = sc.flattendict(self.results, sep='_')
-        for k,v in flat.items():
-            summary[k] = v.mean()
+        for key, res in flat.items():
+            try:
+                func = get_func(key, how)
+                entry = get_result(res, func)
+            except Exception as E:
+                entry = f'N/A {E}'
+            summary[key] = entry
         self.summary = summary
         return summary
-        
-
+    
+    def disp(self):
+        print(self.summary)
+    
     def shrink(self, skip_attrs=None, in_place=True):
         """
         "Shrinks" the simulation by removing the people and other memory-intensive
         attributes (e.g., some interventions and analyzers), and returns a copy of
         the "shrunken" simulation. Used to reduce the memory required for RAM or
         for saved files.
 
@@ -519,22 +679,22 @@
         else:
             return shrunken
 
     def _get_ia(self, which, label=None, partial=False, as_list=False, as_inds=False, die=True, first=False):
         """ Helper method for get_interventions() and get_analyzers(); see get_interventions() docstring """
 
         # Handle inputs
-        if which not in ['interventions', 'analyzers']: # pragma: no cover
+        if which not in ['interventions', 'analyzers']:  # pragma: no cover
             errormsg = f'This method is only defined for interventions and analyzers, not "{which}"'
             raise ValueError(errormsg)
 
-        ia_ndict = self.analyzers if which == 'analyzers' else self.interventions # List of interventions or analyzers
+        ia_ndict = self.analyzers if which == 'analyzers' else self.interventions  # List of interventions or analyzers
         n_ia = len(ia_ndict)  # Number of interventions/analyzers
 
-        position = 0 if first else -1 # Choose either the first or last element
+        position = 0 if first else -1  # Choose either the first or last element
         if label is None:  # Get all interventions if no label is supplied, e.g. sim.get_interventions()
             label = np.arange(n_ia)
         if isinstance(label, np.ndarray):  # Allow arrays to be provided
             label = label.tolist()
         labels = sc.promotetolist(label)
 
         # Calculate the matches
@@ -550,32 +710,33 @@
                 for ind, ia_key, ia_obj in ia_ndict.enumitems():
                     if sc.isstring(label) and ia_obj.label == label or (partial and (label in str(ia_obj.label))):
                         matches.append(ia_obj)
                         match_inds.append(ind)
                     elif isinstance(label, type) and isinstance(ia_obj, label):
                         matches.append(ia_obj)
                         match_inds.append(ind)
-            else: # pragma: no cover
+            else:  # pragma: no cover
                 errormsg = f'Could not interpret label type "{type(label)}": should be str, int, list, or {which} class'
                 raise TypeError(errormsg)
 
         # Parse the output options
         if as_inds:
             output = match_inds
-        elif as_list: # Used by get_interventions()
+        elif as_list:  # Used by get_interventions()
             output = matches
         else:
-            if len(matches) == 0: # pragma: no cover
+            if len(matches) == 0:  # pragma: no cover
                 if die:
                     errormsg = f'No {which} matching "{label}" were found'
                     raise ValueError(errormsg)
                 else:
                     output = None
             else:
-                output = matches[position] # Return either the first or last match (usually), used by get_intervention()
+                output = matches[
+                    position]  # Return either the first or last match (usually), used by get_intervention()
 
         return output
 
     def get_interventions(self, label=None, partial=False, as_inds=False):
         """
         Find the matching intervention(s) by label, index, or type. If None, return
         all interventions. If the label provided is "summary", then print a summary
@@ -584,28 +745,55 @@
         Args:
             label (str, int, Intervention, list): the label, index, or type of intervention to get; if a list, iterate over one of those types
             partial (bool): if true, return partial matches (e.g. 'beta' will match all beta interventions)
             as_inds (bool): if true, return matching indices instead of the actual interventions
         """
         return self._get_ia('interventions', label=label, partial=partial, as_inds=as_inds, as_list=True)
 
-
     def get_intervention(self, label=None, partial=False, first=False, die=True):
         """
         Find the matching intervention(s) by label, index, or type.
         If more than one intervention matches, return the last by default.
         If no label is provided, return the last intervention in the list.
 
         Args:
             label (str, int, Intervention, list): the label, index, or type of intervention to get; if a list, iterate over one of those types
             partial (bool): if true, return partial matches
             first (bool): if true, return first matching intervention (otherwise, return last)
             die (bool): whether to raise an exception if no intervention is found
         """
-        return self._get_ia('interventions', label=label, partial=partial, first=first, die=die, as_inds=False, as_list=False)
+        return self._get_ia('interventions', label=label, partial=partial, first=first, die=die, as_inds=False,
+                            as_list=False)
+
+    def export_df(self):
+        """
+        Export results as a Pandas dataframe
+
+        :return:
+
+        """
+
+        if not self.results_ready:  # pragma: no cover
+            errormsg = 'Please run the sim before exporting the results'
+            raise RuntimeError(errormsg)
+
+        def flatten_results(d, prefix=''):
+            flat = {}
+            for key, val in d.items():
+                if isinstance(val, dict):
+                    flat.update(flatten_results(val, prefix=prefix+key+'.'))
+                else:
+                    flat[prefix+key] = val
+            return flat
+
+        resdict = flatten_results(self.results)
+        resdict['t'] = self.yearvec
+
+        df = sc.dataframe.from_dict(resdict).set_index('t')
+        return df
 
     def save(self, filename=None, keep_people=None, skip_attrs=None, **kwargs):
         """
         Save to disk as a gzipped pickle.
 
         Args:
             filename (str or None): the name or path of the file to save to; if None, uses stored
@@ -728,142 +916,183 @@
                 else:
                     d['summary'] = 'Summary not available (Sim has not yet been run)'
             elif key == 'short_summary':
                 if self.results_ready:
                     d['short_summary'] = dict(sc.dcp(self.short_summary))
                 else:
                     d['short_summary'] = 'Full summary not available (Sim has not yet been run)'
-            else: # pragma: no cover
+            else:  # pragma: no cover
                 try:
                     d[key] = sc.sanitizejson(getattr(self, key))
                 except Exception as E:
                     errormsg = f'Could not convert "{key}" to JSON: {str(E)}; continuing...'
                     print(errormsg)
 
         if filename is None:
             output = sc.jsonify(d, tostring=tostring, indent=indent, verbose=verbose, *args, **kwargs)
         else:
             output = sc.savejson(filename=filename, obj=d, indent=indent, *args, **kwargs)
 
         return output
-    
+
     def plot(self):
-        flat = sc.flattendict(self.results, sep=': ')
-        fig, axs = sc.getrowscols(len(flat), make=True)
-        for ax,(k,v) in zip(axs.flatten(), flat.items()):
-            ax.plot(v)
-            ax.set_title(k)
+        with sc.options.with_style('fancy'):
+            flat = sc.flattendict(self.results, sep=': ')
+            fig, axs = sc.getrowscols(len(flat), make=True)
+            for ax, (k, v) in zip(axs.flatten(), flat.items()):
+                ax.plot(self.yearvec, v)
+                ax.set_title(k)
+                ax.set_xlabel('Year')
         return fig
-            
+
 
 class AlreadyRunError(RuntimeError):
     """
     This error is raised if a simulation is run in such a way that no timesteps
     will be taken. This error is a distinct type so that it can be safely caught
     and ignored if required, but it is anticipated that most of the time, calling
     :py:func:`Sim.run` and not taking any timesteps, would be an inadvertent error.
     """
     pass
 
 
+def demo(run=True, plot=True, summary=True, show=True, **kwargs):
+    """
+    Create a simple demo simulation for Starsim
+    
+    Defaults to using the SIR model with a random network, but these can be configured.
+    
+    Args:
+        run (bool): whether to run the sim
+        plot (bool): whether to plot the results
+        summary (bool): whether to print a summary of the results
+        kwargs (dict): passed to ``ss.Sim()``
+    
+    **Examples**::
+        
+        ss.demo() # Run, plot, and show results
+        ss.demo(diseases='hiv', networks='mf') # Run with different defaults
+    """
+    pars = sc.mergedicts(dict(diseases='sir', networks='random'), kwargs)
+    sim = Sim(pars)
+    if run:
+        sc.heading('Running demo:')
+        sim.run()
+        if summary:
+            sc.heading('Results:')
+            print(sim.summary)
+            if plot:
+                sim.plot()
+                if show:
+                    pl.show()
+    return sim
+
+
 def diff_sims(sim1, sim2, skip_key_diffs=False, skip=None, full=False, output=False, die=False):
     '''
     Compute the difference of the summaries of two simulations, and print any
     values which differ.
 
     Args:
         sim1 (sim/dict): either a simulation object or the sim.summary dictionary
         sim2 (sim/dict): ditto
         skip_key_diffs (bool): whether to skip keys that don't match between sims
         skip (list): a list of values to skip
-        full (bool): whether to use the full summary (else, brief)
+        full (bool): whether to print out all values (not just those that differ)
         output (bool): whether to return the output as a string (otherwise print)
         die (bool): whether to raise an exception if the sims don't match
         require_run (bool): require that the simulations have been run
 
     **Example**::
 
-        s1 = hpv.Sim(rand_seed=1).run()
-        s2 = hpv.Sim(rand_seed=2).run()
-        hpv.diff_sims(s1, s2)
+        s1 = ss.Sim(rand_seed=1).run()
+        s2 = ss.Sim(rand_seed=2).run()
+        ss.diff_sims(s1, s2)
     '''
 
     if isinstance(sim1, Sim):
         sim1 = sim1.summarize()
     if isinstance(sim2, Sim):
         sim2 = sim2.summarize()
     for sim in [sim1, sim2]:
-        if not isinstance(sim, dict): # pragma: no cover
+        if not isinstance(sim, dict):  # pragma: no cover
             errormsg = f'Cannot compare object of type {type(sim)}, must be a sim or a sim.summary dict'
             raise TypeError(errormsg)
 
     # Compare keys
     keymatchmsg = ''
     sim1_keys = set(sim1.keys())
     sim2_keys = set(sim2.keys())
-    if sim1_keys != sim2_keys and not skip_key_diffs: # pragma: no cover
+    if sim1_keys != sim2_keys and not skip_key_diffs:  # pragma: no cover
         keymatchmsg = "Keys don't match!\n"
         missing = list(sim1_keys - sim2_keys)
-        extra   = list(sim2_keys - sim1_keys)
+        extra = list(sim2_keys - sim1_keys)
         if missing:
             keymatchmsg += f'  Missing sim1 keys: {missing}\ns'
         if extra:
             keymatchmsg += f'  Extra sim2 keys: {extra}\n'
 
     # Compare values
     valmatchmsg = ''
     mismatches = {}
+    n_mismatch = 0
     skip = sc.tolist(skip)
-    for key in sim2.keys(): # To ensure order
-        if key in sim1_keys and key not in skip: # If a key is missing, don't count it as a mismatch
+    for key in sim2.keys():  # To ensure order
+        if key in sim1_keys and key not in skip:  # If a key is missing, don't count it as a mismatch
             sim1_val = sim1[key] if key in sim1 else 'not present'
             sim2_val = sim2[key] if key in sim2 else 'not present'
-            if not np.isclose(sim1_val, sim2_val, equal_nan=True):
+            mm = not np.isclose(sim1_val, sim2_val, equal_nan=True)
+            n_mismatch += mm
+            if mm or full:
                 mismatches[key] = {'sim1': sim1_val, 'sim2': sim2_val}
 
     if len(mismatches):
-        valmatchmsg = '\nThe following values differ between the two simulations:\n'
+        valmatchmsg = '\nThe following values differ between the two simulations:\n' if not full else ''
         df = sc.dataframe.from_dict(mismatches).transpose()
-        diff   = []
-        ratio  = []
+        diff = []
+        ratio = []
         change = []
-        small_change = 1e-3 # Define a small change, e.g. a rounding error
+        small_change = 1e-3  # Define a small change, e.g. a rounding error
         for mdict in mismatches.values():
             old = mdict['sim1']
             new = mdict['sim2']
             numeric = sc.isnumber(sim1_val) and sc.isnumber(sim2_val)
-            if numeric and old>0:
-                this_diff  = new - old
-                this_ratio = new/old
-                abs_ratio  = max(this_ratio, 1.0/this_ratio)
+            if numeric and old > 0:
+                this_diff = new - old
+                this_ratio = new / old
+                abs_ratio = max(this_ratio, 1.0 / this_ratio)
 
                 # Set the character to use
-                if abs_ratio<small_change:
+                if abs_ratio < small_change:
                     change_char = '≈'
                 elif new > old:
                     change_char = '↑'
                 elif new < old:
                     change_char = '↓'
+                elif new == old:
+                    change_char = '='
                 else:
                     errormsg = f'Could not determine relationship between sim1={old} and sim2={new}'
                     raise ValueError(errormsg)
 
                 # Set how many repeats it should have
                 repeats = 1
+                if abs_ratio == 0:
+                    repeats = 0
                 if abs_ratio >= 1.1:
                     repeats = 2
                 if abs_ratio >= 2:
                     repeats = 3
                 if abs_ratio >= 10:
                     repeats = 4
 
-                this_change = change_char*repeats
-            else: # pragma: no cover
-                this_diff   = np.nan
-                this_ratio  = np.nan
+                this_change = change_char * repeats
+            else:  # pragma: no cover
+                this_diff = np.nan
+                this_ratio = np.nan
                 this_change = 'N/A'
 
             diff.append(this_diff)
             ratio.append(this_ratio)
             change.append(this_change)
 
         df['diff'] = diff
@@ -871,18 +1100,18 @@
         for col in ['sim1', 'sim2', 'diff', 'ratio']:
             df[col] = df[col].round(decimals=3)
         df['change'] = change
         valmatchmsg += str(df)
 
     # Raise an error if mismatches were found
     mismatchmsg = keymatchmsg + valmatchmsg
-    if mismatchmsg: # pragma: no cover
-        if die:
+    if mismatchmsg:  # pragma: no cover
+        if die and n_mismatch: # To catch full=True case
             raise ValueError(mismatchmsg)
         elif output:
-            return mismatchmsg
+            return df
         else:
             print(mismatchmsg)
     else:
         if not output:
             print('Sims match')
     return
```

### Comparing `starsim-0.1.5/starsim/states.py` & `starsim-0.3.2/starsim/states.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,285 @@
-import pandas as pd
+"""
+Define array-handling classes, including agent states
+"""
+
 import numpy as np
 import sciris as sc
 import numba as nb
-from starsim.utils import INT_NAN
-from starsim.distributions import ScipyDistribution
-from starsim.utils import warn
+import starsim as ss
+from starsim.settings import INT_NAN
+from starsim.settings import dtypes as sdt
 from numpy.lib.mixins import NDArrayOperatorsMixin  # Inherit from this to automatically gain operators like +, -, ==, <, etc.
-from scipy.stats._distn_infrastructure import rv_frozen
 
-__all__ = ['State', 'DynamicView']
 
+__all__ = ['check_dtype', 'UIDArray', 'State', 'ArrayView']
 
 
-class FusedArray(NDArrayOperatorsMixin):
-    # This is a class that allows indexing by UID but does not support dynamic growth
-    # It's kind of like a Pandas series but one that only supports a monotonically increasing
-    # unique integer index, and that we can customize and optimize indexing for.
-    #
-    # We explictly do NOT support slicing (except for `[:]`), as these arrays are indexed by UID and slicing
-    # by UID can be confusing/ambiguous when there are missing values. Indexing with a list/array returns
-    # another FusedArray instance which enables chained filtering
+def check_dtype(dtype, default=None):
+    """ Check that the supplied dtype is one of the supported options """
+    
+    # Handle dtype
+    if dtype is None:
+        if default is None:
+            errormsg = 'Must supply either a dtype or a default value'
+            raise ValueError(errormsg)
+        else:
+            dtype = type(default)
+    
+    if dtype in ['float', float, np.float64, np.float32]:
+        dtype = sdt.float
+    elif dtype in ['int', int, np.int64, np.int32]:
+        dtype = sdt.int
+    elif dtype in ['bool', bool, np.bool_]:
+        dtype = sdt.bool
+    else:
+        warnmsg = f'Data type {type(default)} not a supported data type; set warn=False to suppress warning'
+        ss.warn(warnmsg)
+    
+    return dtype
+
+
+class UIDArray(NDArrayOperatorsMixin):
+    """
+    This is a class that allows indexing by UID but does not support dynamic growth
+    It's kind of like a Pandas series but one that only supports a monotonically increasing
+    unique integer index, and that we can customize and optimize indexing for.
+    
+    We explictly do NOT support slicing (except for `[:]`), as these arrays are indexed by UID and slicing
+    by UID can be confusing/ambiguous when there are missing values. Indexing with a list/array returns
+    another UIDArray instance which enables chained filtering
+    """
 
-    __slots__ = ('values','_uid_map', 'uid')
+    __slots__ = ('values', '_uid_map', 'uid')
 
-    def __init__(self, values, uid, uid_map=None):
+    def __init__(self, values=None, uid=None, uid_map=None):
 
         self.values = values
         self.uid = uid
 
         if uid_map is None and uid is not None:
             # Construct a local UID map as opposed to using a shared one (i.e., the one for all agents contained in the People instance)
-            self.uid_map = np.full(np.max(uid) + 1, fill_value=INT_NAN, dtype=int)
-            self.uid_map[uid] = np.arange(len(uid))
+            self._uid_map = np.full(np.max(uid) + 1, fill_value=ss.INT_NAN, dtype=sdt.int)
+            self._uid_map[uid] = np.arange(len(uid))
         else:
             self._uid_map = uid_map
+        return
 
     def __repr__(self):
-        # TODO - optimize? Don't really need to create a dataframe just to print it, but on the other hand, it's fast enough and very easy
-        df = pd.DataFrame(self.values.T, index=self.uid, columns=['Quantity'])
-        df.index.name = 'UID'
+        if len(self) == 0:
+            return f'<{self.__class__.__name__} (empty)>'
+        df = self.to_df()
         return df.__repr__()
+    
+    def to_df(self):
+        """ Convert to a dataframe """
+        df = sc.dataframe({'Quantity':self.values.T}, index=self.uid)
+        df.index.name = 'UID'
+        return df
 
     @property
     def dtype(self):
         return self.values.dtype
 
     @staticmethod
-    @nb.njit
+    @nb.njit(cache=True)
     def _get_vals_uids(vals, key, uid_map):
         """
         Extract values from a collection of UIDs
 
-        This function is used to retrieve values based on UID. As indexing a FusedArray returns a new FusedArray,
-        this method also populates the new UID map for use in the subsequently created FusedArray, avoiding the
+        This function is used to retrieve values based on UID. As indexing a UIDArray returns a new UIDArray,
+        this method also populates the new UID map for use in the subsequently created UIDArray, avoiding the
         need to re-compute it separately.
 
-        :param vals: A 1D np.ndarray containing the values
-        :param key: A 1D np.ndnarray of integers containing the UIDs to query
-        :param uid_map: A 1D np.ndarray of integers mapping UID to array position in ``vals``
-        :return: A tuple of (values, uids, new_uid_map) suitable for passing into the FusedArray constructor
+        Args:
+            vals: A 1D np.ndarray containing the values
+            key: A 1D np.ndnarray of integers containing the UIDs to query
+            uid_map: A 1D np.ndarray of integers mapping UID to array position in ``vals``
+        
+        Returns:
+            A tuple of (values, uids, new_uid_map) suitable for passing into the UIDArray constructor
         """
         out = np.empty(len(key), dtype=vals.dtype)
         new_uid_map = np.full(uid_map.shape[0], fill_value=INT_NAN, dtype=np.int64)
 
-        for i in range(len(key)):
-            idx = uid_map[key[i]]
+        for i,kv in enumerate(key):
+            idx = uid_map[kv]
             if idx == INT_NAN:
                 raise IndexError('UID not present in array')
             out[i] = vals[idx]
-            new_uid_map[key[i]] = i
+            new_uid_map[kv] = i
+        return out, key, new_uid_map
+    
+    @staticmethod
+    @nb.njit(cache=True, parallel=True)
+    def _get_vals_uids_par(vals, key, uid_map):
+        """
+        Parallelized version of _get_vals_uids() -- need both because this is much slower for small arrays
+        """
+        len_key = len(key)
+        out = np.empty(len_key, dtype=vals.dtype)
+        new_uid_map = np.full(uid_map.shape[0], fill_value=INT_NAN, dtype=np.int64)
+
+        for i in nb.prange(len_key):
+            kv = key[i]
+            idx = uid_map[kv]
+            out[i] = vals[idx]
+            new_uid_map[kv] = i
         return out, key, new_uid_map
 
     @staticmethod
-    @nb.njit
+    @nb.njit(cache=True)
     def _set_vals_uids_multiple(vals, key, uid_map, value):
         """
         Insert an array of values based on UID
 
-        :param vals: A reference to a 1D np.ndarray in which to insert the values
-        :param key: A 1D np.ndnarray of integers containing the UIDs to add values for
-        :param uid_map:  A 1D np.ndarray of integers mapping UID to array position in ``vals``
-        :param value: A 1D np.ndarray the same length as ``key`` containing values to insert
-        :return:
+        Args:
+            vals: A reference to a 1D np.ndarray in which to insert the values
+            key: A 1D np.ndnarray of integers containing the UIDs to add values for
+            uid_map:  A 1D np.ndarray of integers mapping UID to array position in ``vals``
+            value: A 1D np.ndarray the same length as ``key`` containing values to insert
         """
 
-        for i in range(len(key)):
-            if key[i] >= len(uid_map):
-                raise IndexError('UID not present in array (requested UID is larger than the maximum UID in use)')
-            idx = uid_map[key[i]]
+        for i,kv in enumerate(key):
+            if kv >= len(uid_map):
+                errormsg = f'UID not present in array (requested UID ({key[i]}) is larger than the maximum UID in use ({len(uid_map)}))'
+                raise IndexError(errormsg)
+            idx = uid_map[kv]
             if idx == INT_NAN:
                 raise IndexError('UID not present in array')
             elif idx >= len(vals):
-                raise Exception(f'Attempted to write to a non-existant index - this can happen if attempting to write to new entries that have not yet been allocated via grow()')
+                errormsg = f'Attempted to write to a non-existant index ({idx}) - this can happen if attempting to write to new entries that have not yet been allocated via grow()'
+                raise IndexError(errormsg)
             vals[idx] = value[i]
+        return
 
     @staticmethod
-    @nb.njit
+    @nb.njit(cache=True)
     def _set_vals_uids_single(vals, key, uid_map, value):
         """
         Insert a single value into multiple UIDs
 
-        :param vals: A reference to a 1D np.ndarray in which to insert the values
-        :param key: A 1D np.ndnarray of integers containing the UIDs to add values for
-        :param uid_map:  A 1D np.ndarray of integers mapping UID to array position in ``vals``
-        :param value: A scalar value to insert at every position specified by ``key``
-        :return:
+        Args:
+            vals: A reference to a 1D np.ndarray in which to insert the values
+            key: A 1D np.ndnarray of integers containing the UIDs to add values for
+            uid_map:  A 1D np.ndarray of integers mapping UID to array position in ``vals``
+            value: A scalar value to insert at every position specified by ``key``
         """
-        for i in range(len(key)):
-            if key[i] >= len(uid_map):
+        for i,kv in enumerate(key):
+            if kv >= len(uid_map):
                 raise IndexError('UID not present in array (requested UID is larger than the maximum UID in use)')
-            idx = uid_map[key[i]]
+            idx = uid_map[kv]
             if idx == INT_NAN:
                 raise IndexError('UID not present in array')
             elif idx >= len(vals):
                 raise Exception('Attempted to write to a non-existant index - this can happen if attempting to write to new entries that have not yet been allocated via grow()')
             vals[idx] = value
 
     def __getitem__(self, key):
+        if np.iterable(key) and len(key) > 10_000: # Approximate cutoff for when the overhead becomes worthwhile
+            gvu_func = self._get_vals_uids_par
+        else:
+            gvu_func = self._get_vals_uids
+            
         try:
             if isinstance(key, (int, np.integer)):
                 # Handle getting a single item by UID
                 return self.values[self._uid_map[key]]
-            elif isinstance(key, (np.ndarray, FusedArray, DynamicView)):
+            elif isinstance(key, (np.ndarray, UIDArray, ArrayView)):
                 if key.dtype.kind == 'b':
                     # Handle accessing items with a logical array. Surprisingly, it seems faster to use nonzero() to convert
                     # it to indices first. Also, the pure Python implementation is difficult to improve upon using numba
                     mapped_key = key.__array__().nonzero()[0]
                     uids = self.uid.__array__()[mapped_key]
                     new_uid_map = np.full(len(self._uid_map), fill_value=INT_NAN, dtype=int)
                     new_uid_map[uids] = np.arange(len(uids))
                     values = self.values[mapped_key]
                 else:
                     # Access items by an array of integers. We do get a decent performance boost from using numba here
-                    values, uids, new_uid_map = self._get_vals_uids(self.values, key.__array__(), self._uid_map.__array__())
+                    values, uids, new_uid_map = gvu_func(self.values, key.__array__(), self._uid_map.__array__())
             elif isinstance(key, slice):
                 if key.start is None and key.stop is None and key.step is None:
                     return sc.dcp(self)
                 else:
                     raise Exception('Slicing not supported - slice the .values attribute by index instead e.g., x.values[0:5], not x[0:5]')
             else:
                 # This branch is specifically handling the user passing in a list of integers instead of an array, therefore
                 # we need an additional conversion to an array first using np.fromiter to improve numba performance
-                values, uids, new_uid_map = self._get_vals_uids(self.values, np.fromiter(key, dtype=int), self._uid_map.__array__())
-            return FusedArray(values=values, uid=uids, uid_map=new_uid_map)
+                values, uids, new_uid_map = gvu_func(self.values, np.fromiter(key, dtype=int), self._uid_map.__array__())
+            return UIDArray(values=values, uid=uids, uid_map=new_uid_map)
         except IndexError as e:
             if str(INT_NAN) in str(e):
-                raise IndexError(f'UID not present in array')
+                raise IndexError(f'UID {key} not present in array')
             else:
                 raise e
 
     def __setitem__(self, key, value):
-        # nb. the use of .__array__() calls is to access the array interface and thereby treat both np.ndarray and DynamicView instances
-        # in the same way without needing an additional type check. This is also why the FusedArray.dtype property is defined. Noting
-        # that for a State, the uid_map is a dynamic view attached to the People, but after an indexing operation, it will be a bare
-        # FusedArray that has an ordinary numpy array as the uid_map
+        """
+        NB: the use of .__array__() calls is to access the array interface and thereby treat both np.ndarray and ArrayView instances
+        in the same way without needing an additional type check. This is also why the UIDArray.dtype property is defined. Noting
+        that for a State, the uid_map is a dynamic view attached to the People, but after an indexing operation, it will be a bare
+        UIDArray that has an ordinary numpy array as the uid_map.
+        """
         try:
             if isinstance(key, (int, np.integer)):
                 return self.values.__setitem__(self._uid_map[key], value)
-            elif isinstance(key, (np.ndarray, FusedArray)):
+            elif isinstance(key, (np.ndarray, UIDArray)):
                 if key.dtype.kind == 'b':
                     self.values.__setitem__(key.__array__().nonzero()[0], value)
                 else:
-                    if isinstance(value, (np.ndarray, FusedArray)):
+                    if isinstance(value, (np.ndarray, UIDArray)):
                         return self._set_vals_uids_multiple(self.values, key, self._uid_map.__array__(), value.__array__())
                     else:
                         return self._set_vals_uids_single(self.values, key, self._uid_map.__array__(), value)
             elif isinstance(key, slice):
                 if key.start is None and key.stop is None and key.step is None:
                     return self.values.__setitem__(key, value)
                 else:
                     raise Exception('Slicing not supported - slice the .values attribute by index instead e.g., x.values[0:5], not x[0:5]')
             else:
-                if isinstance(value, (np.ndarray, FusedArray)):
+                if isinstance(value, (np.ndarray, UIDArray)):
                     return self._set_vals_uids_multiple(self.values, np.fromiter(key, dtype=int), self._uid_map.__array__(), value.__array__())
                 else:
                     return self._set_vals_uids_single(self.values, np.fromiter(key, dtype=int), self._uid_map.__array__(), value)
         except IndexError as e:
             if str(INT_NAN) in str(e):
-                raise IndexError(f'UID not present in array')
+                raise IndexError(f'UID {key} not present in array')
             else:
                 raise e
 
+    def __getattr__(self, attr):
+        """ Make it behave like a regular array mostly -- enables things like sum(), mean(), etc. """
+        if attr in ['__deepcopy__', '__getstate__', '__setstate__']:
+            return self.__getattribute__(attr)
+        else:
+            return getattr(self.values, attr)
+
     # Make it behave like a regular array mostly
     def __len__(self):
         return len(self.values)
 
     def __contains__(self, *args, **kwargs):
         return self.values.__contains__(*args, **kwargs)
 
     def astype(self, *args, **kwargs):
-        return FusedArray(values=self.values.astype(*args, **kwargs), uid=self.uid, uid_map=self._uid_map)
+        return UIDArray(values=self.values.astype(*args, **kwargs), uid=self.uid, uid_map=self._uid_map)
 
     def sum(self, *args, **kwargs):
         return self.values.sum(*args, **kwargs)
 
     def mean(self, *args, **kwargs):
         return self.values.mean(*args, **kwargs)
 
     def any(self, *args, **kwargs):
         return self.values.any(*args, **kwargs)
 
     def all(self, *args, **kwargs):
         return self.values.all(*args, **kwargs)
 
-    def count_nonzero(self, *args, **kwargs):
+    def count(self, *args, **kwargs):
         return np.count_nonzero(self.values, *args, **kwargs)
 
     @property
     def shape(self):
         return self.values.shape
 
     @property
@@ -228,87 +300,105 @@
         if 'out' in kwargs and kwargs['out'][0] is self:
             # In-place operations like += use this branch
             kwargs['out'] = self.values
             args[0](*args[2:], **kwargs)
             return self
         else:
             out = args[0](*args[2:], **kwargs)
-            if isinstance(out, FusedArray):
-                # For some operations (e.g., those involving two FusedArrays) the result of the ufunc will already be a FusedArray
-                # In particular, operating on two states will result in a FusedArray where the references to the original People uid_map and uids
-                # are still intact. In such cases, we can return the resulting FusedArray directly
+            if isinstance(out, UIDArray):
+                # For some operations (e.g., those involving two UIDArrays) the result of the ufunc will already be a UIDArray
+                # In particular, operating on two states will result in a UIDArray where the references to the original People uid_map and uids
+                # are still intact. In such cases, we can return the resulting UIDArray directly
                 return out
             else:
                 # Otherwise, if the result of the ufunc is an array (e.g., because one of the arguments was an array) then
-                # we need to wrap it up in a new FusedArray. With '__call__' the dimensions should hopefully be the same and we should
+                # we need to wrap it up in a new UIDArray. With '__call__' the dimensions should hopefully be the same and we should
                 # be able to reuse the UID arrays directly
-                return FusedArray(values=out, uid=self.uid, uid_map=self._uid_map)
+                return UIDArray(values=out, uid=self.uid, uid_map=self._uid_map)
 
     def __array_wrap__(self, out_arr, context=None):
-        # This allows numpy operations addition etc. to return instances of FusedArray
+        # This allows numpy operations addition etc. to return instances of UIDArray
         if out_arr.ndim == 0:
             return out_arr.item()
-        return FusedArray(values=out_arr, uid=self.uid, uid_map=self._uid_map) # Hardcoding class means State can inherit from FusedArray but return FusedArray base instances
+        return UIDArray(values=out_arr, uid=self.uid, uid_map=self._uid_map) # Hardcoding class means State can inherit from UIDArray but return UIDArray base instances
 
 
-class DynamicView(NDArrayOperatorsMixin):
-    def __init__(self, dtype, fill_value=None):
+class ArrayView(NDArrayOperatorsMixin):
+
+    __slots__ = ('_data', '_view', 'n', 'default')
+
+    def __init__(self, dtype, default=None, coerce=True):
         """
         Args:
-            name: name of the result as used in the model
-            dtype: datatype
-            fill_value: default value for this state upon model initialization. If not provided, it will use the default value for the dtype
-            shape: If not none, set to match a string in `pars` containing the dimensionality
-            label: text used to construct labels for the result for displaying on plots and other outputs
-        """
-        self.fill_value = fill_value if fill_value is not None else dtype()
+            dtype (class): The dtype to use for this instance (if None, infer from value)
+            default (any): Specify default value for new agents. This can be
+            coerce (bool): Whether to ensure the the data is one of the supported data types
+        """
+        if coerce:
+            dtype = check_dtype(dtype, default)
+        self.default = default if default is not None else dtype()
         self.n = 0  # Number of agents currently in use
         self._data = np.empty(0, dtype=dtype)  # The underlying memory array (length at least equal to n)
         self._view = None  # The view corresponding to what is actually accessible (length equal to n)
         self._map_arrays()
         return
 
     @property
     def _s(self):
-        # Return the size of the underlying array (maximum number of agents that can be stored without reallocation)
+        """ Return the size of the underlying array (maximum number of agents that can be stored without reallocation) """
         return len(self._data)
 
     @property
     def dtype(self):
-        # The specified dtype and the underlying array dtype can be different. For instance, the user might pass in
-        # DynamicView(dtype=int) but the underlying array's dtype will be np.dtype('int32'). This distinction is important
-        # because the numpy dtype has attributes like 'kind' that the input dtype may not have. We need the DynamicView's
-        # dtype to match that of the underlying array so that it can be more seamlessly exchanged with direct numpy arrays
-        # Therefore, we retain the original dtype in DynamicView._dtype() and use
+        """
+        The specified dtype and the underlying array dtype can be different. For instance, the user might pass in
+        ArrayView(dtype=int) but the underlying array's dtype will be np.dtype('int32'). This distinction is important
+        because the numpy dtype has attributes like 'kind' that the input dtype may not have. We need the ArrayView's
+        dtype to match that of the underlying array so that it can be more seamlessly exchanged with direct numpy arrays
+        Therefore, we retain the original dtype in ArrayView._dtype() and use
+        """
         return self._data.dtype
 
     def __len__(self):
-        # Return the number of active elements
+        """ Return the number of active elements """
         return self.n
 
     def __repr__(self):
-        # Print out the numpy view directly
+        """ Print out the numpy view directly """
         return self._view.__repr__()
 
     def grow(self, n):
-        # If the total number of agents exceeds the array size, extend the underlying arrays
+        """ If the total number of agents exceeds the array size, extend the underlying arrays """
         if self.n + n > self._s:
             n_new = max(n, int(self._s / 2))  # Minimum 50% growth
-            self._data = np.concatenate([self._data, np.full(n_new, dtype=self.dtype, fill_value=self.fill_value)], axis=0)
+            self._data = np.concatenate([self._data, np.full(n_new, dtype=self.dtype, fill_value=self.default)], axis=0)
         self.n += n  # Increase the count of the number of agents by `n` (the requested number of new agents)
         self._map_arrays()
+        return
 
     def _trim(self, inds):
-        # Keep only specified indices
+        """ Keep only specified indices """
         # Note that these are indices, not UIDs!
         n = len(inds)
         self._data[:n] = self._data[inds]
-        self._data[n:self.n] = self.fill_value
+        self._data[n:self.n] = self.default
         self.n = n
         self._map_arrays()
+        return
+
+    def __getstate__(self):
+        """ When pickling, skip storing the `._view` attribute, which should be re-linked after unpickling """
+        return {k:getattr(self, k) for k in self.__slots__ if k != '_view'}
+
+    def __setstate__(self, state):
+        """ Re-map arrays after unpickling so that `.view` is a reference to the correct array in-memory """
+        for k,v in state.items():
+            setattr(self, k, v)
+        self._map_arrays()
+        return
 
     def _map_arrays(self):
         """
         Set main simulation attributes to be views of the underlying data
 
         This method should be called whenever the number of agents required changes
         (regardless of whether or not the underlying arrays have been resized)
@@ -316,105 +406,154 @@
         self._view = self._data[:self.n]
 
     def __getitem__(self, key):
         return self._view.__getitem__(key)
 
     def __setitem__(self, key, value):
         self._view.__setitem__(key, value)
+        
+    def __getattr__(self, attr):
+        """ Make it behave like a regular array mostly -- enables things like sum(), mean(), etc. """
+        if attr in ['__deepcopy__', '__getstate__', '__setstate__']:
+            return self.__getattribute__(attr)
+        else:
+            return getattr(self._view, attr)
 
     @property
     def __array_interface__(self):
         return self._view.__array_interface__
 
     def __array__(self):
         return self._view
 
     def __array_ufunc__(self, *args, **kwargs):
         args = [(x if x is not self else self._view) for x in args]
         kwargs = {k: v if v is not self else self._view for k, v in kwargs.items()}
         return self._view.__array_ufunc__(*args, **kwargs)
 
 
-class State(FusedArray):
+class State(UIDArray):
+
+    __slots__ = ('values', '_uid_map', 'uid', 'default', 'name', 'label', '_data', 'values', '_initialized')
 
-    def __init__(self, name, dtype, fill_value=None, label=None):
+    def __init__(self, name, dtype=None, default=None, label=None, coerce=True):
         """
+        Store a state of the agents (e.g. age, infection status, etc.)
 
-        :param name: A string name for the state
-        :param dtype: The dtype to use for this instance
-        :param fill_value: Specify default value for new agents. This can be
+        Args: 
+            name (str): The name for the state (also used as the dictionary key, so should not have spaces etc.)
+            dtype (class): The dtype to use for this instance (if None, infer from value)
+            default (any): Specify default value for new agents. This can be
             - A scalar with the same dtype (or castable to the same dtype) as the State
             - A callable, with a single argument for the number of values to produce
-            - An ss.ScipyDistribution instance
-        :param label:
-        """
-
-        super().__init__(values=None, uid=None, uid_map=None)  # Call the FusedArray constructor
-
-        self.fill_value = fill_value
-
-        self._data = DynamicView(dtype=dtype)
+            - A ``ss.Dist`` instance
+            label (str): The human-readable name for the state
+            coerce (bool): Whether to ensure the the data is one of the supported data types
+        """
+        super().__init__()  # Call the UIDArray constructor
+        
+        if coerce:
+            dtype = check_dtype(dtype, default)
+        
+        if default is None:
+            default = dtype()
+        
+        # Set attributes
+        self.default = default
         self.name = name
         self.label = label or name
+        self._data = ArrayView(dtype=dtype)
         self.values = self._data._view
         self._initialized = False
+        return
 
     def __repr__(self):
         if not self._initialized:
             return f'<State {self.name} (uninitialized)>'
         else:
-            return FusedArray.__repr__(self)
+            return UIDArray.__repr__(self)
 
     def _new_vals(self, uids):
-        if isinstance(self.fill_value, ScipyDistribution):
-            new_vals = self.fill_value.rvs(uids)
-        elif callable(self.fill_value):
-            new_vals = self.fill_value(len(uids))
+        if isinstance(self.default, ss.Dist):
+            new_vals = self.default.rvs(uids)
+        elif callable(self.default):
+            new_vals = self.default(len(uids))
         else:
-            new_vals = self.fill_value
+            new_vals = self.default
         return new_vals
 
-    def initialize(self, sim=None, people=None):
+    def initialize(self, sim):
+        """
+        Initialize state
+
+        This method should be called as part of initialization of the parent class containing the state -
+        specifically, `People.initialize()` and `Module.initialize()`. Initialization of a State object
+        involves two processes:
+
+        - Converting any distribution objects to a Dist instance and linking it to RNGs stored in a `Sim`
+        - Establishing a bidirectional connection with a `People` object for the purpose of UID indexing and resizing
+
+        Since State objects can be stored in `People` or in a `Module` and the collection of all states in a `Sim` should
+        be connected to RNGs within that same `Sim`, the states must necessarily be linked to the same `People` object that
+        is inside a `Sim`. Initializing States outside of a `Sim` is not possible because of this RNG dependency, particularly
+        because the states in a `People` object cannot be initialized without a `Sim` and therefore it would not be possible to
+        have an initialized `People` object outside of a `Sim`.
+        
+        Args:
+            sim: A `Sim` instance that contains an initialized `People` object
+        """
+
         if self._initialized:
             return
 
-        if sim is not None and people is None:
-            people = sim.people
-
-        sim_still_needed = False
-        if isinstance(self.fill_value, rv_frozen):
-            if sim is not None:
-                self.fill_value = ScipyDistribution(self.fill_value, f'{self.__class__.__name__}_{self.label}')
-                self.fill_value.initialize(sim, self)
-            else:
-                sim_still_needed = True
+        people = sim.people
+        assert people.initialized, 'People must be initialized before initializing states'
+        
+        # Connect any distributions in the default to RNGs in the Sim
+        if isinstance(self.default, ss.Dist):
+            self.default.initialize(module=self, sim=sim)
+
+        # Establish connection with the People object
+        people.register_state(self)
+        self._uid_map = people._uid_map
+        self.uid = people.uid
+
+        # Populate initial values
+        self._data.grow(len(self.uid))
+        self._data[:len(self.uid)] = self._new_vals(self.uid)
+        self.values = self._data._view
 
-        people.add_state(self, die=False) # CK: should not be needed
-        if not sim_still_needed:
-            self._uid_map = people._uid_map
-            self.uid = people.uid
-            self._data.grow(len(self.uid))
-            self._data[:len(self.uid)] = self._new_vals(self.uid)
-            self.values = self._data._view
-            self._initialized = True
+        self._initialized = True
         return
 
     def grow(self, uids):
         """
         Add state for new agents
 
         This method is normally only called via `People.grow()`.
 
-        :param uids: Numpy array of UIDs for the new agents being added This array should have length n
+        Args:
+            uids: Numpy array of UIDs for the new agents being added This array should have length n
         """
 
         n = len(uids)
         self._data.grow(n)
         self.values = self._data._view
         self._data[-n:] = self._new_vals(uids)
         return
 
     def _trim(self, inds):
         # Trim arrays to remove agents - should only be called via `People.remove()`
         self._data._trim(inds)
         self.values = self._data._view
         return
+
+    def __getstate__(self):
+        # When pickling, skip storing the `.values` attribute, which should be re-linked after unpickling
+        return {k:getattr(self, k) for k in self.__slots__ if k != 'values'}
+
+    def __setstate__(self, state):
+        # When unpickling, re-link the `.values` attribute
+        for k,v in state.items():
+            setattr(self, k, v)
+        self.values = self._data._view
+        return
```

### Comparing `starsim-0.1.5/starsim/utils.py` & `starsim-0.3.2/starsim/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,155 @@
 """
 Numerical utilities
 """
 
-# %% Housekeeping
-
 import warnings
 import numpy as np
 import sciris as sc
 import starsim as ss
 import numba as nb
-import scipy.stats as sps
 import pandas as pd
 
-# What functions are externally visible -- note, this gets populated in each section below
-__all__ = []
-
-# System constants
-__all__ += ['INT_NAN']
-
-INT_NAN = np.iinfo(
-    np.int32).max  # Value to use to flag invalid content (i.e., an integer value we are treating like NaN, since NaN can't be stored in an integer array)
-
 # %% Helper functions
-__all__ += ['ndict', 'omerge', 'warn', 'unique', 'find_contacts', 'get_subclasses']
+
+# What functions are externally visible -- note, this gets populated in each section below
+__all__ = ['ndict', 'omerge', 'omergeleft', 'warn', 'unique', 'find_contacts', 'get_subclasses', 'all_subclasses']
 
 
 class ndict(sc.objdict):
     """
     A dictionary-like class that provides additional functionalities for handling named items.
 
     Args:
-        name (str): The items' attribute to use as keys.
+        name (str): The attribute of the item to use as the dict key (i.e., all items should have this attribute defined)
         type (type): The expected type of items.
         strict (bool): If True, only items with the specified attribute will be accepted.
+        overwrite (bool): whether to allow adding a key when one has already been added
 
     **Examples**::
 
-        networks = ss.ndict(ss.mf(), ss.maternal())
-        networks = ss.ndict([ss.mf(), ss.maternal()])
-        networks = ss.ndict({'mf':ss.mf(), 'maternal':ss.maternal()})
-
+        networks = ss.ndict(ss.MFNet(), ss.MaternalNet())
+        networks = ss.ndict([ss.MFNet(), ss.MaternalNet()])
+        networks = ss.ndict({'mf':ss.MFNet(), 'maternal':ss.MaternalNet()})
     """
 
-    def __init__(self, *args, name='name', type=None, strict=True, **kwargs):
-        self.setattribute('_name', name)  # Since otherwise treated as keys
+    def __init__(self, *args, nameattr='name', type=None, strict=True, overwrite=False, **kwargs):
+        super().__init__()
+        self.setattribute('_nameattr', nameattr)  # Since otherwise treated as keys
         self.setattribute('_type', type)
         self.setattribute('_strict', strict)
-        self._initialize(*args, **kwargs)
+        self.setattribute('_overwrite', overwrite)
+        self.extend(*args, **kwargs)
         return
 
-    def append(self, arg, key=None):
+    def append(self, arg, key=None, overwrite=None):
         valid = False
         if arg is None:
             return  # Nothing to do
-        elif hasattr(arg, self._name):
-            key = key or getattr(arg, self._name)
+        elif hasattr(arg, self._nameattr):
+            key = key or getattr(arg, self._nameattr)
             valid = True
         elif isinstance(arg, dict):
-            if self._name in arg:
-                key = key or arg[self._name]
+            if self._nameattr in arg:
+                key = key or arg[self._nameattr]
                 valid = True
             else:
                 for k, v in arg.items():
                     self.append(v, key=k)
                 valid = None  # Skip final processing
         elif not self._strict:
             key = key or f'item{len(self) + 1}'
             valid = True
         else:
             valid = False
 
         if valid is True:
-            self._check_type(arg)
-            self[key] = arg
+            if self._strict:
+                self._check_type(arg)
+                self._check_key(key, overwrite=overwrite)
+            self[key] = arg # Actually add to the ndict!
         elif valid is None:
             pass  # Nothing to do
         else:
-            errormsg = f'Could not interpret argument {arg}: does not have expected attribute "{self._name}"'
-            raise ValueError(errormsg)
-
+            errormsg = f'Could not interpret argument {arg}: does not have expected attribute "{self._nameattr}"'
+            raise TypeError(errormsg)
         return
-
+    
+    def _check_key(self, key, overwrite=None):
+        if overwrite is None: overwrite = self._overwrite
+        if key in self:
+            if not overwrite:
+                typestr = f' "{self._type}"' if self._type else ''
+                errormsg = f'Cannot add object "{key}" since already present in ndict{typestr} with keys:\n{sc.newlinejoin(self.keys())}'
+                raise ValueError(errormsg)
+            else:
+                ss.warn(f'Overwriting existing ndict entry "{key}"')
+        return
+    
     def _check_type(self, arg):
         """ Check types """
         if self._type is not None:
             if not isinstance(arg, self._type):
                 errormsg = f'The following item does not have the expected type {self._type}:\n{arg}'
                 raise TypeError(errormsg)
         return
 
-    def _initialize(self, *args, **kwargs):
+    def extend(self, *args, **kwargs):
+        """ Add new items to the ndict, by item, list, or dict """
         args = sc.mergelists(*args)
         for arg in args:
             self.append(arg)
         for key, arg in kwargs.items():
             self.append(arg, key=key)
         return
 
     def copy(self):
-        new = self.__class__.__new__(name=self._name, type=self._type, strict=self._strict)
+        new = self.__class__.__new__(nameattr=self._nameattr, type=self._type, strict=self._strict)
         new.update(self)
         return new
 
     def __add__(self, dict2):
         """ Allow c = a + b """
         new = self.copy()
-        new.append(dict2)
+        if isinstance(dict2, list):
+            new.extend(dict2)
+        else:
+            new.append(dict2)
         return new
 
     def __iadd__(self, dict2):
         """ Allow a += b """
-        self.append(dict2)
+        if isinstance(dict2, list):
+            self.extend(dict2)
+        else:
+            self.append(dict2)
         return self
 
 
 def omerge(*args, **kwargs):
-    """ Merge things into an objdict """
+    """ Merge things into an objdict, using standard order """
     return sc.objdict(sc.mergedicts(*args, **kwargs))
 
 
+def omergeleft(*args, **kwargs):
+    """ Merge things into an odict, using opposite order to allow defaults to be supplied second """
+    if len(args) == 1 and len(kwargs):
+        new = args[0]
+        default = kwargs
+    elif len(args) == 2 and len(kwargs) == 0:
+        new = args[0]
+        default = args[1]
+    else:
+        errormsg = 'Expecting either two arguments, or one argument and kwargs; for any other arrangement, use ss.omerge()'
+        raise ValueError(errormsg)
+    return sc.objdict(sc.mergedicts(default, new))
+
+
 def warn(msg, category=None, verbose=None, die=None):
-    """ Helper function to handle warnings -- not for the user """
+    """ Helper function to handle warnings -- shortcut to warnings.warn """
 
     # Handle inputs
     warnopt = ss.options.warnings if not die else 'error'
     if category is None:
         category = RuntimeWarning
     if verbose is None:
         verbose = ss.options.verbose
@@ -180,31 +205,34 @@
 
 
 def get_subclasses(cls):
     for subclass in cls.__subclasses__():
         yield from get_subclasses(subclass)
         yield subclass
 
+def all_subclasses(cls):
+    """ As above but also returns subsubclases """
+    return set(cls.__subclasses__()).union(
+        [s for c in cls.__subclasses__() for s in all_subclasses(c)])
 
 # %% Seed methods
 
 __all__ += ['set_seed']
 
-
 def set_seed(seed=None):
     '''
     Reset the random seed -- complicated because of Numba, which requires special
     syntax to reset the seed. This function also resets Python's built-in random
     number generated.
 
     Args:
         seed (int): the random seed
     '''
 
-    @nb.njit
+    @nb.njit(cache=True)
     def set_seed_numba(seed):
         return np.random.seed(seed)
 
     def set_seed_regular(seed):
         return np.random.seed(seed)
 
     # Dies if a float is given
@@ -215,58 +243,35 @@
     if seed is None:  # Numba can't accept a None seed, so use our just-reinitialized Numpy stream to generate one
         seed = np.random.randint(1e9)
     set_seed_numba(seed)
 
     return
 
 
-# %% Helper functions related to distributions
-__all__ += ['lognorm_params', 'lognorm']
-
-
-def lognorm_params(mean, stdev):
-    """
-    Returns the shape and scale parameters for scipy's parameterization of the
-    lognormal distribution which will give the specified mean and stdev
-    """
-    s = np.sqrt(np.log(stdev ** 2 / mean ** 2 + 1))
-    mu = np.log(mean ** 2 / np.sqrt(stdev ** 2 + mean ** 2))
-    scale = np.exp(mu)
-    return s, scale
-
-
-def lognorm(mean, stdev):
-    """
-    Wrapper for scipy lognorm but using mean and stdev
-    """
-    s, scale = lognorm_params(mean, stdev)
-    return sps.lognorm(s=s, scale=scale)
-
-
 # %% Simple array operations
 
 __all__ += ['true', 'false', 'defined', 'undefined']
 
 
-@nb.njit
+@nb.njit(cache=True)
 def _true(uids, values):
     """
     Returns the UIDs for indices where the value evaluates as True
     """
     out = np.empty(len(uids), dtype=uids.dtype)
     j = 0
     for i in range(len(values)):
         out[j] = uids[i]
         if values[i]:
             j += 1
     out = out[0:j]
     return out
 
 
-@nb.njit
+@nb.njit(cache=True)
 def _false(uids, values):
     """
     Returns the UIDs for indices where the value evaluates as False
     """
     out = np.empty(len(uids), dtype=uids.dtype)
     j = 0
     for i in range(len(values)):
@@ -278,29 +283,29 @@
 
 
 def true(state):
     """
     Returns the UIDs of the values of the array that are true
 
     Args:
-        state (State, FusedArray)
+        state (State, UIDArray)
 
     **Example**::
 
         inds = ss.true(people.alive) # Returns array of UIDs of alive agents
     """
     return _true(state.uid.__array__(), state.__array__())
 
 
 def false(state):
     """
     Returns the indices of the values of the array that are false.
 
     Args:
-        state (State, FusedArray)
+        state (State, UIDArray)
 
     **Example**::
 
         inds = ss.false(people.alive) # Returns array of UIDs of dead agents
     """
     return _false(state.uid.__array__(), state.__array__())
 
@@ -334,48 +339,73 @@
 
 
 # %% Data cleaning and processing
 
 __all__ += ['standardize_data']
 
 
-def standardize_data(data=None, metadata=None):
+def standardize_data(data=None, metadata=None, max_age=120, min_year=1800):
+    """
+    Args:
+        data (pandas.DataFrame, pandas.Series, dict, int, float): An associative array  or a number, with the
+        input data to be standardized.
+        metadata (dict): The metadata containing information about the columns of the data.
+        max_age (float): The maximum age allowed in the data. Default is 120 years.
+        min_year (float): The minimum year allowed in the data. Default is 1800.
+
+    Returns:
+        df (pandas.DataFrame or sciris.dataframe): The standardized data
+
+    Raises:
+        ValueError: If the columns in `data` do not match the column names in metadata.data_cols
+        or if the index of the data series is not understood.
+    """
+    metadata = sc.objdict(metadata)
 
     if isinstance(data, pd.DataFrame):
         if not set(metadata.data_cols.values()).issubset(data.columns):
             errormsg = 'Please ensure the columns of the data match the values in metadata.data_cols.'
             raise ValueError(errormsg)
         df = data
 
     elif isinstance(data, pd.Series):
-        if (data.index < 120).all():  # Assume index is age bins
-            df = pd.DataFrame({
-                metadata.data_cols['year']: 2000,
-                metadata.data_cols['age']: data.index.values,
-                metadata.data_cols['value']: data.values,
-            })
-        elif (data.index > 1900).all():  # Assume index year
-            df = pd.DataFrame({
+        if metadata.data_cols.get('age'):
+            if (data.index <= max_age).all():  # Assume index is age bins
+                df = sc.dataframe({
+                    metadata.data_cols['year']: 2000,
+                    metadata.data_cols['age']: data.index.values,
+                    metadata.data_cols['value']: data.values,
+                })
+            elif (data.index >= min_year).all():  # Assume index year
+                df = sc.dataframe({
+                    metadata.data_cols['year']: data.index.values,
+                    metadata.data_cols['age']: 0,
+                    metadata.data_cols['value']: data.values,
+                })
+            else:
+                errormsg = 'Could not understand index of data series: should be age (all values less than 120) or year (all values greater than 1900).'
+                raise ValueError(errormsg)
+        else:
+            df = sc.dataframe({
                 metadata.data_cols['year']: data.index.values,
-                metadata.data_cols['age']: 0,
                 metadata.data_cols['value']: data.values,
             })
-        else:
-            errormsg = 'Could not understand index of data series: should be age (all values less than 120) or year (all values greater than 1900).'
-            raise ValueError(errormsg)
 
         if metadata.data_cols.get('sex'):
             df = pd.concat([df, df])
             df[metadata.data_cols['sex']] = np.repeat(list(metadata.sex_keys.values()), len(data))
 
     elif isinstance(data, dict):
         if not set(metadata.data_cols.values()).issubset(data.keys()):
             errormsg = 'Please ensure the keys of the data dict match the values in metadata.data_cols.'
             raise ValueError(errormsg)
-        df = pd.DataFrame(data)
+        new_data = dict()
+        for sim_name, col_name in metadata.data_cols.items():
+            new_data[sim_name] = sc.tolist(data[col_name])
+        df = sc.dataframe(new_data)
 
     elif sc.isnumber(data):
         df = data  # Just return it as-is
 
     else:
         errormsg = f'Data type {type(data)} not understood.'
         raise ValueError(errormsg)
```

### Comparing `starsim-0.1.5/starsim.egg-info/PKG-INFO` & `starsim-0.3.2/starsim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: starsim
-Version: 0.1.5
+Version: 0.3.2
 Summary: Starsim
-Author: Robyn Stuart, Romesh Abeysuriya, Jamie Cohen, Cliff Kerr, Daniel Klein
+Author: Robyn Stuart, Cliff Kerr, Romesh Abeysuriya, Paula Sanz-Leon, Jamie Cohen, and Daniel Klein on behalf of the Starsim Collective
 Keywords: agent-based model,simulation,disease,epidemiology
 Platform: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Starsim
 =======
 
+**Warning! Starsim is still in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used for real research or policy questions.**
+
 Starsim is an agent-based disease modeling framework in which users can design and configure simulations of pathogens that progress over time within each agent and pass from one agent to the next along dynamic transmission networks. The framework explicitly supports co-transmission of multiple pathogens, allowing users to concurrently simulate several diseases while capturing behavioral and biological interactions. Non-communicable diseases can easily be included as well, either as a co-factor for transmissible pathogens or as an independent exploration. Detailed modeling of mother-child relationships can be simulated from the timepoint of conception, enabling study of congenital diseases and associated birth outcomes. Finally, Starsim facilitates the comparison of one or more intervention scenarios to a baseline scenario in evaluating the impact of various products like vaccines, therapeutics, and novel diagnostics delivered via flexible routes including mass campaigns, screen and treat, and targeted outreach.
 
 The framework is appropriate for simulating one or more sexually transmitted infections (including syphilis, gonorrhea, chlamydia, HPV, and HIV), respiratory infections (like RSV and tuberculosis), and other diseases and underlying determinants (such as Ebola, diabetes, and malnutrition).
 
 
-**WARNING! This library is in the early stages of development. It is being shared solely for transparency and to facilitate collaborative development. It is not ready to be used and any results produced using it will be invalid.** 
-
-
 Installation
 ------------
 
 To install, clone this repository, then run ``pip install -e .`` (don't forget the dot!) in this folder to install ``starsim`` and its dependencies. This will make ``starsim`` available on the Python path.
 
 
 Usage and documentation
 -----------------------
 
-Documentation is not yet available. Usage examples are available in the ``tests`` folder.
+Documentation is available at https://docs.starsim.org. 
+
+Usage examples are available in the ``tests`` folder.
 
 
 Contributing
 ------------
 
 If you wish to contribute, please see the code of conduct and contributing documents.
```

### Comparing `starsim-0.1.5/starsim.egg-info/SOURCES.txt` & `starsim-0.3.2/starsim.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 LICENSE
 README.rst
 setup.py
 starsim/__init__.py
-starsim/analyzers.py
 starsim/connectors.py
 starsim/demographics.py
+starsim/disease.py
 starsim/distributions.py
 starsim/interventions.py
 starsim/modules.py
+starsim/network.py
 starsim/parameters.py
 starsim/people.py
-starsim/random.py
+starsim/products.py
 starsim/results.py
+starsim/run.py
+starsim/samples.py
 starsim/settings.py
 starsim/sim.py
 starsim/states.py
 starsim/utils.py
 starsim/version.py
 starsim.egg-info/PKG-INFO
 starsim.egg-info/SOURCES.txt
 starsim.egg-info/dependency_links.txt
 starsim.egg-info/requires.txt
 starsim.egg-info/top_level.txt
 starsim/diseases/__init__.py
-starsim/diseases/disease.py
-starsim/diseases/examples.py
+starsim/diseases/cholera.py
+starsim/diseases/ebola.py
 starsim/diseases/gonorrhea.py
 starsim/diseases/hiv.py
+starsim/diseases/measles.py
+starsim/diseases/ncd.py
+starsim/diseases/sir.py
 starsim/diseases/syphilis.py
-starsim/networks/__init__.py
-starsim/networks/networks.py
-starsim/networks/randnet.py
 tests/test_base.py
 tests/test_baselines.py
+tests/test_dcp.py
 tests/test_demographics.py
-tests/test_distributions.py
-tests/test_examples.py
-tests/test_random.py
-tests/test_rngcontainer.py
+tests/test_diseases.py
+tests/test_dist.py
+tests/test_dists.py
+tests/test_samples.py
+tests/test_simple.py
 tests/test_syphilis.py
```

### Comparing `starsim-0.1.5/tests/test_base.py` & `starsim-0.3.2/tests/test_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Test objects from base.py
 """
 
 # %% Imports and settings
 import sciris as sc
 import numpy as np
 import starsim as ss
-import matplotlib.pyplot as plt
-import scipy.stats as sps
+import matplotlib.pyplot as pl
 
+sc.options(interactive=False) # Assume not running interactively
 
 # %% Define the tests
 
 def test_people():
     sc.heading('Testing people object')
 
     # Base people contains only the states defined in base.base_states
@@ -28,97 +28,104 @@
     # Possible to add a module to people outside a sim (not typical workflow)
     ppl.add_module(ss.HIV())
 
     return ppl
 
 
 def test_networks():
+    sc.heading('Testing networks')
 
     # Make completely abstract layers
     n_edges = 10_000
     n_people = 1000
     p1 = np.random.randint(n_people, size=n_edges)
     p2 = np.random.randint(n_people, size=n_edges)
     beta = np.ones(n_edges)
     nw1 = ss.Network(p1=p1, p2=p2, beta=beta, label='rand')
     nw2 = ss.Network(dict(p1=p1, p2=p2, beta=beta), label='rand')  # Alternate method
 
     sim = ss.Sim()
     sim.initialize()
     
-    nw3 = ss.hpv_network()
+    nw3 = ss.MaternalNet()
     nw3.initialize(sim)
-    sim.people.networks.update(sim.people)  # Update by providing a timestep & current time index
+    nw3.add_pairs(mother_inds=[1, 2, 3], unborn_inds=[100, 101, 102], dur=[1, 1, 1])
 
-    nw4 = ss.maternal()
-    nw4.initialize(sim)
-    nw4.add_pairs(mother_inds=[1, 2, 3], unborn_inds=[100, 101, 102], dur=[1, 1, 1])
+    # HPV NETWORK - NOT FUNCTIONAL
+    # nw3 = ss.hpv_network()
+    # nw3.initialize(sim)
+    # sim.people.networks.update(sim.people)  # Update by providing a timestep & current time index
 
-    return nw1, nw2, nw3, nw4
 
+    return nw1, nw2, nw3
 
-def test_microsim():
-    sc.heading('Test making people and providing them to a sim')
 
-    networks = [ss.mf(), ss.maternal()]
-    ppl = ss.People(100, networks=networks)
+def test_microsim(do_plot=False):
+    sc.heading('Test making people and providing them to a sim')
 
     # Make HIV module
     hiv = ss.HIV()
     # Set beta. The first entry represents transmission risk from infected p1 -> susceptible p2
     # Need to be careful to get the ordering right. The set-up here assumes that in the simple
     # sexual  network, p1 is male and p2 is female. In the maternal network, p1=mothers, p2=babies.
     hiv.pars['beta'] = {'mf': [0.15, 0.10], 'maternal': [0.2, 0]}
 
-    sim = ss.Sim(people=ppl, demographics=ss.Pregnancy(), diseases=hiv)
+    sim = ss.Sim(
+        people=ss.People(100),
+        networks=[ss.MFNet(), ss.MaternalNet()],
+        demographics=ss.Pregnancy(),
+        diseases=hiv
+    )
     sim.initialize()
     sim.run()
 
-    plt.figure()
-    plt.plot(sim.tivec, sim.results.hiv.n_infected)
-    plt.title('HIV number of infections')
+    if do_plot:
+        pl.figure()
+        pl.plot(sim.tivec, sim.results.hiv.n_infected)
+        pl.title('HIV number of infections')
 
     return sim
 
 
 def test_ppl_construction():
 
-    def init_debut(self, sim, uids):
-        #loc = 16
+    def init_debut(module, sim, uids):
+        # Test setting the mean debut age by sex, 16 for men and 21 for women.
         loc = np.full(len(uids), 16)
         loc[sim.people.female[uids]] = 21
         return loc
 
     mf_pars = {
-        'debut_dist': sps.norm(loc=init_debut, scale=2),  # Age of debut can vary by using callable parameter values
+        'debut': ss.normal(loc=init_debut, scale=2),  # Age of debut can vary by using callable parameter values
     }
-    sim_pars = {'networks': [ss.mf(mf_pars)], 'n_agents': 100}
+    sim_pars = {'networks': [ss.MFNet(mf_pars)], 'n_agents': 100}
     gon_pars = {'beta': {'mf': [0.08, 0.04]}, 'p_death': 0.2}
     gon = ss.Gonorrhea(pars=gon_pars)
 
     sim = ss.Sim(pars=sim_pars, diseases=[gon])
     sim.initialize()
     sim.run()
-    plt.figure()
-    plt.plot(sim.tivec, sim.results.gonorrhea.n_infected)
-    plt.title('Number of gonorrhea infections')
+    pl.figure()
+    pl.plot(sim.tivec, sim.results.gonorrhea.n_infected)
+    pl.title('Number of gonorrhea infections')
 
     return sim
 
 
 
 # %% Run as a script
 if __name__ == '__main__':
+    do_plot = True
+    sc.options(interactive=do_plot)
+
     # Start timing
     T = sc.tic()
 
-    ss.options.multirng = True
-
     # Run tests
     ppl = test_people()
-    nw1, nw2, nw3, nw4 = test_networks()
-    sim1 = test_microsim()
+    nw1, nw2, nw3 = test_networks()
+    sim1 = test_microsim(do_plot)
     sim2 = test_ppl_construction()
 
     sc.toc(T)
-    plt.show()
+    pl.show()
     print('Done.')
```

### Comparing `starsim-0.1.5/tests/test_baselines.py` & `starsim-0.3.2/tests/test_baselines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
-Test that the current version of HPVsim exactly matches
+Test that the current version of Starsim exactly matches
 the baseline results.
 """
 
 import numpy as np
 import sciris as sc
 import starsim as ss
 
-do_plot = 1
-do_save = 0
+do_plot = True
+do_save = False
 baseline_filename  = sc.thisdir(__file__, 'baseline.json')
 benchmark_filename = sc.thisdir(__file__, 'benchmark.json')
 parameters_filename = sc.thisdir(ss.__file__, 'regression', f'pars_v{ss.__version__}.json')
-sc.options.set(interactive=False) # Assume not running interactively
+sc.options(interactive=False) # Assume not running interactively
 
 # Define the parameters
 pars = sc.objdict(
     start         = 2000,       # Starting year
     n_years       = 20,         # Number of years to simulate
     dt            = 0.2,        # Timestep
     verbose       = 0,          # Don't print details of the run
     rand_seed     = 2,          # Set a non-default seed
 )
 
 def make_people():
     ss.set_seed(pars.rand_seed)
     n_agents = int(10e3)
-    networks = [ss.mf(), ss.maternal()]
-    ppl = ss.People(n_agents, networks=networks)
+    ppl = ss.People(n_agents=n_agents)
     return ppl
 
 
 def make_sim(ppl=None, do_plot=False, **kwargs):
     '''
     Define a default simulation for testing the baseline, including
     interventions to increase coverage. If run directly (not via pytest), also
     plot the sim by default.
     '''
-    
+
     if ppl is None:
         ppl = make_people()
-    
+
     # Make the sim
     hiv = ss.HIV()
-    hiv.pars['beta'] = {'mf': [0.15, 0.10], 'maternal': [0.2, 0]}
-    sim = ss.Sim(pars=pars, people=ppl, demographics=ss.Pregnancy(), diseases=hiv)
+    hiv.pars.beta = {'mf': [0.15, 0.10], 'maternal': [0.2, 0]}
+    networks = [ss.MFNet(), ss.MaternalNet()]
+    sim = ss.Sim(pars=pars, people=ppl, networks=networks, demographics=ss.Pregnancy(), diseases=hiv)
 
     # Optionally plot
     if do_plot:
         sim.run()
         sim.plot()
 
     return sim
@@ -75,39 +75,31 @@
 
     return
 
 
 def test_baseline():
     ''' Compare the current default sim against the saved baseline '''
     
-    # Do not run with multi-RNG
-    if ss.options.multirng:
-        return
-
     # Load existing baseline
     baseline = sc.loadjson(baseline_filename)
     old = baseline['summary']
 
     # Calculate new baseline
     new = make_sim()
     new.run()
 
     # Compute the comparison
-    ss.diff_sims(old, new, full=True, die=True)
+    ss.diff_sims(old, new, die=True)
 
     return new
 
 
 def test_benchmark(do_save=do_save, repeats=1, verbose=True):
     ''' Compare benchmark performance '''
     
-    # Do not run with multi-RNG
-    if ss.options.multirng:
-        return
-
     if verbose: print('Running benchmark...')
     try:
         previous = sc.loadjson(benchmark_filename)
     except FileNotFoundError:
         previous = None
 
     t_peoples = []
@@ -208,15 +200,15 @@
     return json
 
 
 
 if __name__ == '__main__':
 
     # Start timing and optionally enable interactive plotting
-    sc.options.set(interactive=do_plot)
+    sc.options(interactive=do_plot)
     T = sc.tic()
 
     json = test_benchmark(do_save=do_save, repeats=5) # Run this first so benchmarking is available even if results are different
     new  = test_baseline()
     sim = make_sim(do_plot=do_plot)
 
     print('\n'*2)
```

### Comparing `starsim-0.1.5/tests/test_demographics.py` & `starsim-0.3.2/tests/test_demographics.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,42 +4,46 @@
 
 # %% Imports and settings
 import starsim as ss
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 import sciris as sc
+import pytest
+
 
 do_plot = True
+sc.options(interactive=False) # Assume not running interactively
 
 
 def test_nigeria(which='births', dt=1, start=1995, n_years=15, plot_init=False, do_plot=True):
     """
     Make a Nigeria sim with demographic modules
     Switch between which='births' or 'pregnancy' to determine which demographic module to use
     """
 
     # Make demographic modules
     demographics = sc.autolist()
 
     if which == 'births':
         birth_rates = pd.read_csv(ss.root / 'tests/test_data/nigeria_births.csv')
-        births = ss.births(pars={'birth_rate': birth_rates})
+        births = ss.Births(pars={'birth_rate': birth_rates})
         demographics += births
+
     elif which == 'pregnancy':
         fertility_rates = pd.read_csv(ss.root / 'tests/test_data/nigeria_asfr.csv')
         pregnancy = ss.Pregnancy(pars={'fertility_rate': fertility_rates, 'rel_fertility': 1})  # 4/3
         demographics += pregnancy
 
     death_rates = pd.read_csv(ss.root / 'tests/test_data/nigeria_deaths.csv')
-    death = ss.background_deaths(pars={'death_rate': death_rates})
+    death = ss.Deaths(pars={'death_rate': death_rates, 'units': 1})
     demographics += death
 
     # Make people
-    n_agents = 10_000
+    n_agents = 5_000
     nga_pop_1995 = 106819805
     age_data = pd.read_csv(ss.root / 'tests/test_data/nigeria_age.csv')
     ppl = ss.People(n_agents, age_data=age_data)
 
     sim = ss.Sim(
         dt=dt,
         total_pop=nga_pop_1995,
@@ -54,15 +58,14 @@
         # Plot histograms of the age distributions - simulated vs data
         bins = np.arange(0, 101, 1)
         init_scale = nga_pop_1995 / n_agents
         counts, bins = np.histogram(sim.people.age, bins)
         plt.bar(bins[:-1], counts * init_scale, alpha=0.5, label='Simulated')
         plt.bar(bins, age_data.value.values * 1000, alpha=0.5, color='r', label='Data')
         plt.legend(loc='upper right')
-        plt.show()
 
     sim.run()
 
     end = start + n_years
     nigeria_popsize = pd.read_csv(ss.root / 'tests/test_data/nigeria_popsize.csv')
     data = nigeria_popsize[(nigeria_popsize.year >= start) & (nigeria_popsize.year <= end)]
 
@@ -73,34 +76,34 @@
     cmr_data = nigeria_cmr[(nigeria_cmr.Year >= start) & (nigeria_cmr.Year <= end)]
 
     # Tests
     if which == 'pregnancy':
 
         print("Check we don't have more births than pregnancies")
         assert sum(sim.results.pregnancy.births) <= sum(sim.results.pregnancy.pregnancies)
-        print(f'✓ (births <= pregnancies)')
+        print('✓ (births <= pregnancies)')
 
         if dt == 1:
             print("Checking that births equal pregnancies with dt=1")
             assert np.array_equal(sim.results.pregnancy.pregnancies, sim.results.pregnancy.births)
-            print(f'✓ (births == pregnancies)')
+            print('✓ (births == pregnancies)')
 
     print("Check final pop size within 5% of data")
     assert np.isclose(data.n_alive.values[-1], sim.results.n_alive[-1], rtol=0.05)
     print(f'✓ (simulated/data={sim.results.n_alive[-1] / data.n_alive.values[-1]:.2f})')
 
     # Plots
     if do_plot:
         fig, ax = plt.subplots(2, 2)
         ax = ax.ravel()
         ax[0].scatter(data.year, data.n_alive, alpha=0.5)
         ax[0].plot(sim.yearvec, sim.results.n_alive, color='k')
         ax[0].set_title('Population')
 
-        ax[1].plot(sim.yearvec, 1000 * sim.results.background_deaths.cmr / dt, label='Simulated CMR')
+        ax[1].plot(sim.yearvec, 1000 * sim.results.deaths.cmr / dt, label='Simulated CMR')
         ax[1].scatter(cmr_data.Year, cmr_data.CMR, label='Data CMR')
         ax[1].set_title('CMR')
         ax[1].legend()
 
         if which == 'births':
             ax[2].plot(sim.yearvec, sim.results.births.cbr / dt, label='Simulated CBR')
         elif which == 'pregnancy':
@@ -111,17 +114,40 @@
 
         if which == 'pregnancy':
             ax[3].plot(sim.yearvec, sim.results.pregnancy.pregnancies / dt, label='Pregnancies')
             ax[3].plot(sim.yearvec, sim.results.pregnancy.births / dt, label='Births')
             ax[3].set_title('Pregnancies and births')
             ax[3].legend()
 
-        fig.tight_layout
+        fig.tight_layout()
+
+    return sim
+
 
-        plt.show()
+def test_constant_pop():
+    # Test pars for constant pop size
+    sim = ss.Sim(n_agents=10e3, birth_rate=10, death_rate=10/1010*1000, n_years=200, rand_seed=1).run()
+    print("Check final pop size within 5% of starting pop")
+    assert np.isclose(sim.results.n_alive[0], sim.results.n_alive[-1], rtol=0.05)
+    print(f'✓ (final pop / starting pop={sim.results.n_alive[-1] / sim.results.n_alive[0]:.2f})')
 
+    # Plots
+    if do_plot:
+        sim.plot()
     return sim
 
 
+def test_module_adding():
+    births = ss.Births(pars={'birth_rate': 10})
+    deaths = ss.Deaths(pars={'death_rate': 10})
+    demographics = [births, deaths]
+    with pytest.raises(Exception): # CK: should be ValueError, but that fails for now, and this is OK
+        ss.Sim(n_agents=1e3, demographics=demographics, birth_rate=10, death_rate=10).run()
+    return demographics
+
+
 if __name__ == '__main__':
-    # Test Nigeria demographic consistency
-    sim = test_nigeria(dt=1, which='pregnancy', n_years=15, plot_init=True, do_plot=do_plot)
+    sc.options(interactive=do_plot)
+    s1 = test_nigeria(dt=1, which='pregnancy', n_years=15, plot_init=True, do_plot=do_plot)
+    s2 = test_constant_pop()
+    s3 = test_module_adding()
+    plt.show()
```

### Comparing `starsim-0.1.5/tests/test_examples.py` & `starsim-0.3.2/tests/test_diseases.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,116 @@
 """
-Run simplest tests
+Run tests of disease models
 """
 
 # %% Imports and settings
 import starsim as ss
+import sciris as sc
 import matplotlib.pyplot as plt
-import scipy.stats as sps
-import numpy as np
+
+test_run = True
+n_agents = [10_000, 2_000][test_run]
+do_plot = True
+sc.options(interactive=False) # Assume not running interactively
+
 
 def test_sir():
-    ppl = ss.People(10000)
-    ppl.networks = ss.ndict(ss.RandomNetwork(n_contacts=sps.poisson(mu=4)))
+    ppl = ss.People(n_agents)
+    network_pars = {
+        'n_contacts': ss.poisson(4), # Contacts Poisson distributed with a mean of 4
+    }
+    networks = ss.RandomNet(pars=network_pars)
 
     sir_pars = {
-        'dur_inf': sps.norm(loc=10), # Override the default distribution
+        'dur_inf': ss.normal(loc=10),  # Override the default distribution
     }
     sir = ss.SIR(sir_pars)
 
-    # You can also change the parameters of the default lognormal distribution directly!
-    #sir.pars['dur_inf'].kwds['loc'] = 5 
-    
-    # Or why not put a lambda here for fun!
-    sir.pars['dur_inf'].kwds['loc'] = lambda self, sim, uids: sim.people.age[uids]/10
+    # Change pars after creating the SIR instance
+    sir.pars.beta = {'random': 0.1}
+
+    # You can also change the parameters of the default lognormal distribution directly
+    sir.pars.dur_inf.set(loc=5)
+
+    # Or use a function, here a lambda that makes the mean for each agent equal to their age divided by 10
+    sir.pars.dur_inf.set(loc = lambda self, sim, uids: sim.people.age[uids] / 10)
 
-    sir.pars['beta'] = {'randomnetwork': 0.1}
-    sim = ss.Sim(people=ppl, diseases=sir)
+    sim = ss.Sim(people=ppl, diseases=sir, networks=networks)
     sim.run()
 
     # CK: parameters changed
     # assert len(sir.log.out_edges(np.nan)) == sir.pars.initial # Log should match initial infections
-    df = sir.log.line_list # Check generation of line-list
+    df = sir.log.line_list  # Check generation of line-list
     # assert df.source.isna().sum() == sir.pars.initial # Check seed infections in line list
 
     plt.figure()
     plt.stackplot(
         sim.yearvec,
         sir.results.n_susceptible,
         sir.results.n_infected,
         sir.results.n_recovered,
         sim.results.new_deaths.cumsum(),
     )
     plt.legend(['Susceptible', 'Infected', 'Recovered', 'Dead'])
     plt.xlabel('Year')
     plt.title('SIR')
-    return
+    return sim
+
 
-#@pytest.mark.skip(reason="Haven't converted yet")
 def test_ncd():
-    ppl = ss.People(10000)
-    ppl.networks = None
+    ppl = ss.People(n_agents)
     ncd = ss.NCD()
     sim = ss.Sim(people=ppl, diseases=ncd)
     sim.run()
 
     assert len(ncd.log.out_edges) == ncd.log.number_of_edges()
-    df = ncd.log.line_list # Check generation of line-list
+    df = ncd.log.line_list  # Check generation of line-list
     assert df.source.isna().all()
 
     plt.figure()
     plt.stackplot(
         sim.yearvec,
         ncd.results.n_not_at_risk,
-        ncd.results.n_at_risk-ncd.results.n_affected,
+        ncd.results.n_at_risk - ncd.results.n_affected,
         ncd.results.n_affected,
         sim.results.new_deaths.cumsum(),
     )
-    plt.legend(['Not at risk','At risk','Affected', 'Dead'])
+    plt.legend(['Not at risk', 'At risk', 'Affected', 'Dead'])
     plt.xlabel('Year')
     plt.title('NCD')
-    return
+    return sim
+
+
+def test_gavi():
+    sims = sc.autolist()
+    for disease in ['cholera', 'measles', 'ebola']:
+        pars = dict(
+            diseases = disease,
+            n_agents = n_agents,
+            networks = 'random',
+        )
+        sim = ss.Sim(pars)
+        sim.run()
+        sims += sim
+    return sims
+
+
+def test_multidisease():
+    ppl = ss.People(n_agents)
+    sir1 = ss.SIR(name='sir1')
+    sir2 = ss.SIR(name='sir2')
+
+    sir1.pars.beta = {'randomnet': 0.1}
+    sir2.pars.beta = {'randomnet': 0.2}
+    networks = ss.RandomNet(pars=dict(n_contacts=ss.poisson(4)))
+
+    sim = ss.Sim(people=ppl, diseases=[sir1, sir2], networks=networks)
+    sim.run()
+    return sim
 
 
 if __name__ == '__main__':
-    ss.options(multirng=False)
+    sc.options(interactive=do_plot)
     sim1 = test_sir()
     sim2 = test_ncd()
-    plt.show()
+    sims = test_gavi()
+    sim = test_multidisease()
```

