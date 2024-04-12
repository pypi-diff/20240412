# Comparing `tmp/monisha-0.0.40.tar.gz` & `tmp/monisha-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.40.tar", last modified: Mon Apr  1 16:36:53 2024, max compression
+gzip compressed data, was "monisha-0.0.41.tar", last modified: Fri Apr 12 07:22:44 2024, max compression
```

## Comparing `monisha-0.0.40.tar` & `monisha-0.0.41.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 16:36:48.000000 monisha-0.0.40/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.210939 monisha-0.0.40/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/functions/function11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/se.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-01 16:36:48.000000 monisha-0.0.40/Monisha/scripts/uo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 16:36:53.214939 monisha-0.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-01 16:36:48.000000 monisha-0.0.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:36:53.214939 monisha-0.0.40/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 16:36:53.000000 monisha-0.0.40/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:36:53.214939 monisha-0.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-01 16:36:48.000000 monisha-0.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 07:22:38.000000 monisha-0.0.41/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.622558 monisha-0.0.41/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 07:22:44.626558 monisha-0.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-12 07:22:38.000000 monisha-0.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:22:44.626558 monisha-0.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-12 07:22:38.000000 monisha-0.0.41/setup.py
```

### Comparing `monisha-0.0.40/LICENSE` & `monisha-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/Monisha/functions/function01.py` & `monisha-0.0.41/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/Monisha/functions/function02.py` & `monisha-0.0.41/Monisha/functions/function02.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..scripts.uo import Humon
+from ..scripts.es import Humon
 from ..scripts.en import Scripted
 #=============================================================================
 
 def Dbytes(sizes, second=Scripted.DATA01):
     if not sizes or (sizes == Scripted.DATA02):
         return Scripted.DATA09
     nomos = 0
```

### Comparing `monisha-0.0.40/Monisha/functions/function03.py` & `monisha-0.0.41/Monisha/functions/function03.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..scripts.se import Symb
+from ..scripts.eo import Symb
 #===================================================================================
 
 def progress(percentage, b01=Symb.DATA02, b02=Symb.DATA01, l01=10, l02=20):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
```

### Comparing `monisha-0.0.40/Monisha/functions/function04.py` & `monisha-0.0.41/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/Monisha/functions/function06.py` & `monisha-0.0.41/Monisha/functions/function06.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     DATA02 = str("duration")
     DATA03 = str("format_id")
     DATA04 = str("format_note")
     DATA07 = str("filesize_approx")
 
 #================================================================================
 
-class Hkeys(object):
+class Skeys(object):
 
     DATA01 = "0123456789"
     DATA02 = "abcdefghijklmnopqrstuvwxyz"
     DATA03 = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
     DATA04 = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
 
 #================================================================================
```

### Comparing `monisha-0.0.40/Monisha/functions/function07.py` & `monisha-0.0.41/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/Monisha/functions/function10.py` & `monisha-0.0.41/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/PKG-INFO` & `monisha-0.0.41/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.40
+Version: 0.0.41
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.40 Summary: python helper
+Metadata-Version: 2.1 Name: monisha Version: 0.0.41 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,clinton,abraham Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: ~=3.8 Description-Content-Type:
+python,clinton,abraham Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: License :: OSI Approved :: GNU Lesser General
+Public License v3 (LGPLv3) Requires-Python: ~=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                                  ð¦ _M_O_N_I_S_H_A
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install monisha ```
```

### Comparing `monisha-0.0.40/README.md` & `monisha-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `monisha-0.0.40/monisha.egg-info/PKG-INFO` & `monisha-0.0.41/monisha.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.40
+Version: 0.0.41
 Summary: python helper modules
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.40 Summary: python helper
+Metadata-Version: 2.1 Name: monisha Version: 0.0.41 Summary: python helper
 modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,clinton,abraham Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: ~=3.8 Description-Content-Type:
+python,clinton,abraham Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: License :: OSI Approved :: GNU Lesser General
+Public License v3 (LGPLv3) Requires-Python: ~=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE
                                  ð¦ _M_O_N_I_S_H_A
                _[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]_[_t_e_l_e_g_r_a_m_ _b_a_d_g_e_]
 ## INSTALLATION ```bash pip install monisha ```
```

### Comparing `monisha-0.0.40/setup.py` & `monisha-0.0.41/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as o:
     long_description = o.read()
 
 DATA01 = "clintonabrahamc@gmail.com"
-
-DATA02 = ['Development Status :: 5 - Production/Stable',
+DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
-        'Topic :: Internet',
         'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules']
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
-    version='0.0.40',
+    version='0.0.41',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.8',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='python helper modules',
```

