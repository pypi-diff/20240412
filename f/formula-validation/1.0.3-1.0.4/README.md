# Comparing `tmp/formula_validation-1.0.3.tar.gz` & `tmp/formula_validation-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formula_validation-1.0.3.tar", max compression
+gzip compressed data, was "formula_validation-1.0.4.tar", max compression
```

## Comparing `formula_validation-1.0.3.tar` & `formula_validation-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-08-01 01:04:20.518127 formula_validation-1.0.3/LICENSE
--rw-r--r--   0        0        0     4507 2023-09-19 23:18:29.208971 formula_validation-1.0.3/README.md
--rw-r--r--   0        0        0     9234 2023-09-29 23:50:59.492155 formula_validation-1.0.3/formula_validation/Adduct.py
--rw-r--r--   0        0        0     5336 2023-10-10 19:59:09.202587 formula_validation-1.0.3/formula_validation/Element.py
--rw-r--r--   0        0        0    30644 2023-10-10 20:14:33.695231 formula_validation-1.0.3/formula_validation/Formula.py
--rw-r--r--   0        0        0     2754 2023-08-17 22:21:35.186540 formula_validation-1.0.3/formula_validation/FormulaPrediction.py
--rw-r--r--   0        0        0      869 2023-07-20 23:31:37.044607 formula_validation-1.0.3/formula_validation/IncorrectAdduct.py
--rw-r--r--   0        0        0      914 2023-07-20 23:30:46.906938 formula_validation-1.0.3/formula_validation/IncorrectFormula.py
--rw-r--r--   0        0        0      810 2023-07-19 22:26:13.810873 formula_validation-1.0.3/formula_validation/NotFoundElement.py
--rw-r--r--   0        0        0        0 2023-07-25 23:11:13.607829 formula_validation-1.0.3/formula_validation/__init__.py
--rw-r--r--   0        0        0     1070 2023-10-10 20:17:27.358872 formula_validation-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 formula_validation-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-01 01:04:20.518127 formula_validation-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4337 2023-10-12 19:58:59.902543 formula_validation-1.0.4/README.md
+-rw-r--r--   0        0        0     9234 2023-09-29 23:50:59.492155 formula_validation-1.0.4/formula_validation/Adduct.py
+-rw-r--r--   0        0        0     5336 2023-10-10 19:59:09.202587 formula_validation-1.0.4/formula_validation/Element.py
+-rw-r--r--   0        0        0    30667 2024-04-11 20:55:31.441308 formula_validation-1.0.4/formula_validation/Formula.py
+-rw-r--r--   0        0        0     2754 2023-08-17 22:21:35.186540 formula_validation-1.0.4/formula_validation/FormulaPrediction.py
+-rw-r--r--   0        0        0      869 2023-07-20 23:31:37.044607 formula_validation-1.0.4/formula_validation/IncorrectAdduct.py
+-rw-r--r--   0        0        0      914 2023-07-20 23:30:46.906938 formula_validation-1.0.4/formula_validation/IncorrectFormula.py
+-rw-r--r--   0        0        0      810 2023-07-19 22:26:13.810873 formula_validation-1.0.4/formula_validation/NotFoundElement.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:11:13.607829 formula_validation-1.0.4/formula_validation/__init__.py
+-rw-r--r--   0        0        0     1090 2024-04-12 09:18:14.358202 formula_validation-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 formula_validation-1.0.4/PKG-INFO
```

### Comparing `formula_validation-1.0.3/LICENSE` & `formula_validation-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/README.md` & `formula_validation-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,16 @@
 - Analyze possible fragment masses explained by a formula and adduct.
 
 ## Installation
 
 To use this module, you'll need Python 3.x and the required dependencies. You can install the dependencies using pip:
 
 ```bash
-pip install rdkit urllib3 rpy2
-```
-You should have R installed with the package devtools and 
-```R
-install.packages("devtools")
-devtools::install_github("mjhelf/MassTools")
+pip install rdkit urllib3
 
-library(MassTools)
-```
 ## Usage
 
 ### Creating Formula Objects
 
 You can create a Formula object using various methods:
 
 - `Formula.formula_from_str_hill(formula_str: str, adduct: str) -> 'Formula'`: Create a Formula object from a chemical formula string in Hill notation.
```

### Comparing `formula_validation-1.0.3/formula_validation/Adduct.py` & `formula_validation-1.0.4/formula_validation/Adduct.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/formula_validation/Element.py` & `formula_validation-1.0.4/formula_validation/Element.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/formula_validation/Formula.py` & `formula_validation-1.0.4/formula_validation/Formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
       for element,counts_in_other in self.__elements.items():
         new_formula_dict[element] = new_formula_dict.get(element,0) * num_to_multiply
       return Formula(new_formula_dict, self.__adduct, self.__charge, self.__charge_type)
     else:
         raise IncorrectFormula("other should be a formula and is a " + str(type(Formula)))
     
   @staticmethod
-  def formula_from_str_hill(formula_str: str, adduct: str, metadata: dict=None) -> 'Formula':
+  def formula_from_str_hill(formula_str: str, adduct: str=None, metadata: dict=None) -> 'Formula':
     """
       Static method to create a Formula object from a chemical formula string in Hill notation.
 
       Args:
         formula_str (str): A string representing a molecular formula in Hill notation. Example: 'C4H5N6Na'. Other example 'C4H5N6Na+'
         adduct (str): A string representing an adduct in the form '[M+C2H2O-H]-', '[M-3H2O+2H]2+' or '[5M+Ca]2+' where the charge is specified at the end.
         metadata (dict): Optional argument to include a dict of metadata, defaults to None.
@@ -385,15 +385,15 @@
     else:
       charge = 0
       charge_type = ''
 
     return Formula(elements, adduct, charge, charge_type, metadata=metadata)
   
   @staticmethod
-  def formula_from_str(formula_str: str, adduct: str, no_api: bool=False, metadata: bool=None) -> 'Formula':
+  def formula_from_str(formula_str: str, adduct: str=None, no_api: bool=False, metadata: bool=None) -> 'Formula':
     """
       Static method to create a Formula object from a chemical formula string.
 
       Args:
         formula_str (str): A string representing a molecular formula. Example: 'C4H5N6Na'.
         adduct (str): A string representing an adduct in the form '[M+C2H2O-H]-', '[M-3H2O+2H]2+' or '[5M+Ca]2+' where the charge is specified at the end.
         no_api (bool): Disables api calls for formula resolution.
@@ -428,15 +428,15 @@
       
       mf_hill = data['mf']
       return Formula.formula_from_str_hill(mf_hill, adduct, metadata)
     else:
       return None
     
   @staticmethod
-  def formula_from_smiles(smiles: str, adduct: str, no_api: bool=False, metadata: Dict=None) -> 'Formula':
+  def formula_from_smiles(smiles: str, adduct: str=None, no_api: bool=False, metadata: Dict=None) -> 'Formula':
     """
       Static method to create a Formula object from a SMILES (Simplified Molecular Input Line Entry System) string.
 
       Args:
         smiles (str): A string representing a molecular structure in SMILES notation. Example: CCCCCCC[C@@H](C/C=C/CCC(=O)NC/C(=C/Cl)/[C@@]12[C@@H](O1)[C@H](CCC2=O)O)OC
         adduct (str): A string representing an adduct in the form '[M+C2H2O-H]-', '[M-3H2O+2H]2+' or '[5M+Ca]2+' where the charge is specified at the end.
         no_api (bool): Disables api calls for formula resolution.
@@ -458,15 +458,15 @@
     mol = Chem.MolFromSmiles(smiles)
     if mol is None:
       raise IncorrectFormula(smiles)
     formula = CalcMolFormula(mol)
     return Formula.formula_from_str(formula, adduct, no_api, metadata=metadata)
     
   @staticmethod
-  def formula_from_inchi(inchi: str, adduct: str, no_api:bool=False, metadata: Dict=None) -> 'Formula':
+  def formula_from_inchi(inchi: str, adduct: str=None, no_api:bool=False, metadata: Dict=None) -> 'Formula':
     """
       Static method to create a Formula object from an InChI (International Chemical Identifier) string.
 
       Args:
         inchi (str): A string representing a molecular structure in InChI notation. Example: InChI=1S/C45H73N5O10S3/c1-14-17-24(6)34(52)26(8)37-25(7)30(58-13)18-31-46-29(19-61-31)39-49-45(12,21-62-39)43-50-44(11,20-63-43)42(57)48-32(22(4)15-2)35(53)27(9)40(55)59-36(23(5)16-3)38(54)47-33(28(10)51)41(56)60-37/h19,22-28,30,32-37,51-53H,14-18,20-21H2,1-13H3,(H,47,54)(H,48,57)/t22-,23-,24+,25-,26-,27+,28+,30-,32-,33-,34-,35-,36-,37-,44+,45+/m0/s1
         adduct (str): A string representing an adduct in the form '[M+C2H2O-H]-', '[M-3H2O+2H]2+' or '[5M+Ca]2+' where the charge is specified at the end.
         no_api (bool): Disables api calls for formula resolution.
@@ -680,14 +680,15 @@
         a exception if reference_monoisotopic_mass or ppm are not numbers
 
       Returns: 
         the absolute value of the ppm calculated
     """
     return (reference_monoisotopic_mass / 1000000.0) * ppm
   
+  
 
 if __name__ == '__main__':
   smiles_1 = 'CCCCCCC[C@@H](C/C=C/CCC(=O)NC/C(=C/Cl)/[C@@]12[C@@H](O1)[C@H](CCC2=O)O)OC'
   adduct = '[M+C2H2O-H]-' 
   my_formula = Formula.formula_from_smiles(smiles_1, adduct)
   expected_value =496.24713858
   current_value = my_formula.get_monoisotopic_mass_with_adduct()
```

### Comparing `formula_validation-1.0.3/formula_validation/FormulaPrediction.py` & `formula_validation-1.0.4/formula_validation/FormulaPrediction.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/formula_validation/IncorrectAdduct.py` & `formula_validation-1.0.4/formula_validation/IncorrectAdduct.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/formula_validation/IncorrectFormula.py` & `formula_validation-1.0.4/formula_validation/IncorrectFormula.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/formula_validation/NotFoundElement.py` & `formula_validation-1.0.4/formula_validation/NotFoundElement.py`

 * *Files identical despite different names*

### Comparing `formula_validation-1.0.3/PKG-INFO` & `formula_validation-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formula_validation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package to represent formulas with adducts and process ms data from it. 
 Home-page: https://github.com/Wang-Bioinformatics-Lab/formula_validation
 License: GPL-3.0-only
 Keywords: ms,chemistry
 Author: Alberto Gil de la Fuente
 Author-email: alberto.gilf@gmail.com
 Maintainer: Alberto Gil de la Fuente
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: rdkit (>2023.9.5)
 Requires-Dist: urllib3 (>=1.0,<2.0)
 Project-URL: Repository, https://github.com/Wang-Bioinformatics-Lab/formula_validation
 Description-Content-Type: text/markdown
 
 # Formula Validation Python Module
 
 This Python module contains a `Formula` class for working with chemical formulas, as well as methods for creating, manipulating, and analyzing formulas. It also includes functionality for dealing with adducts and calculating monoisotopic masses.
@@ -49,23 +51,16 @@
 - Analyze possible fragment masses explained by a formula and adduct.
 
 ## Installation
 
 To use this module, you'll need Python 3.x and the required dependencies. You can install the dependencies using pip:
 
 ```bash
-pip install rdkit urllib3 rpy2
-```
-You should have R installed with the package devtools and 
-```R
-install.packages("devtools")
-devtools::install_github("mjhelf/MassTools")
+pip install rdkit urllib3
 
-library(MassTools)
-```
 ## Usage
 
 ### Creating Formula Objects
 
 You can create a Formula object using various methods:
 
 - `Formula.formula_from_str_hill(formula_str: str, adduct: str) -> 'Formula'`: Create a Formula object from a chemical formula string in Hill notation.
```

