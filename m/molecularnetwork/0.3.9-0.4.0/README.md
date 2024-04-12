# Comparing `tmp/molecularnetwork-0.3.9.tar.gz` & `tmp/molecularnetwork-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.3.9.tar", last modified: Fri Apr 12 19:10:26 2024, max compression
+gzip compressed data, was "molecularnetwork-0.4.0.tar", last modified: Fri Apr 12 20:21:34 2024, max compression
```

## Comparing `molecularnetwork-0.3.9.tar` & `molecularnetwork-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.535608 molecularnetwork-0.3.9/
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.9/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.9/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 19:10:26.535405 molecularnetwork-0.3.9/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     4344 2024-04-12 12:25:50.000000 molecularnetwork-0.3.9/README.md
--rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.9/banner.png
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.531990 molecularnetwork-0.3.9/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2857 2024-04-12 19:00:24.000000 molecularnetwork-0.3.9/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.535128 molecularnetwork-0.3.9/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-12 19:10:26.000000 molecularnetwork-0.3.9/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)    28978 2024-04-09 11:48:31.000000 molecularnetwork-0.3.9/net.png
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.9/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-12 19:10:26.535650 molecularnetwork-0.3.9/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-12 13:12:06.000000 molecularnetwork-0.3.9/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 19:10:26.534764 molecularnetwork-0.3.9/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.9/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.9/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:21:34.146519 molecularnetwork-0.4.0/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.4.0/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.4.0/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 20:21:34.146313 molecularnetwork-0.4.0/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4344 2024-04-12 12:25:50.000000 molecularnetwork-0.4.0/README.md
+-rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.4.0/banner.png
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:21:34.141178 molecularnetwork-0.4.0/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.4.0/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      903 2024-04-12 20:14:18.000000 molecularnetwork-0.4.0/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2857 2024-04-12 19:00:24.000000 molecularnetwork-0.4.0/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.4.0/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.4.0/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:21:34.145884 molecularnetwork-0.4.0/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4767 2024-04-12 20:21:34.000000 molecularnetwork-0.4.0/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-12 20:21:34.000000 molecularnetwork-0.4.0/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-12 20:21:34.000000 molecularnetwork-0.4.0/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-12 20:21:34.000000 molecularnetwork-0.4.0/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-12 20:21:34.000000 molecularnetwork-0.4.0/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)    28978 2024-04-09 11:48:31.000000 molecularnetwork-0.4.0/net.png
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.4.0/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-12 20:21:34.146579 molecularnetwork-0.4.0/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-12 20:21:10.000000 molecularnetwork-0.4.0/setup.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-12 20:21:34.145679 molecularnetwork-0.4.0/test/
+-rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.4.0/test/test.csv
+-rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.4.0/test/test.gpickle
+-rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.4.0/test/test.py
```

### Comparing `molecularnetwork-0.3.9/.gitignore` & `molecularnetwork-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/LICENSE` & `molecularnetwork-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/PKG-INFO` & `molecularnetwork-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.9
+Version: 0.4.0
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `molecularnetwork-0.3.9/README.md` & `molecularnetwork-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/banner.png` & `molecularnetwork-0.4.0/banner.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/molecularnetwork/featurizer.py` & `molecularnetwork-0.4.0/molecularnetwork/featurizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 from .utils import InvalidSMILESError
 
 
 class FingerprintCalculator:
     def __init__(self, descriptor="morgan2"):
         self.descriptor = descriptor
         self.descriptors = {
-            "atompairs": lambda m: Pairs.GetAtomPairFingerprint(m),
             "maccs": lambda m: MACCSkeys.GenMACCSKeys(m),
             "morgan2": lambda m: AllChem.GetMorganFingerprintAsBitVect(m, 2, 2048),
             "morgan3": lambda m: AllChem.GetMorganFingerprintAsBitVect(m, 3, 2048),
-            "rdkit": lambda m: FingerprintMols.FingerprintMol(m),
-            "topo": lambda m: Torsions.GetTopologicalTorsionFingerprint(m),
+            "rdkit": lambda m: Chem.RDKFingerprintMol(m),
         }
 
     def calculate_fingerprint(self, smi):
         mol = Chem.MolFromSmiles(smi)
         if mol:
             fn = self.descriptors[self.descriptor]
             return fn(mol)
```

### Comparing `molecularnetwork-0.3.9/molecularnetwork/graph.py` & `molecularnetwork-0.4.0/molecularnetwork/graph.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/molecularnetwork/similarity.py` & `molecularnetwork-0.4.0/molecularnetwork/similarity.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/molecularnetwork.egg-info/PKG-INFO` & `molecularnetwork-0.4.0/molecularnetwork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.9
+Version: 0.4.0
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `molecularnetwork-0.3.9/net.png` & `molecularnetwork-0.4.0/net.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/setup.py` & `molecularnetwork-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.3.9",
+    version="0.4.0",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

### Comparing `molecularnetwork-0.3.9/test/test.csv` & `molecularnetwork-0.4.0/test/test.csv`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.9/test/test.gpickle` & `molecularnetwork-0.4.0/test/test.gpickle`

 * *Files identical despite different names*

