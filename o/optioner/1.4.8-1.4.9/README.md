# Comparing `tmp/optioner-1.4.8.tar.gz` & `tmp/optioner-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.8.tar", last modified: Wed Apr 10 07:37:46 2024, max compression
+gzip compressed data, was "optioner-1.4.9.tar", last modified: Fri Apr 12 17:12:33 2024, max compression
```

## Comparing `optioner-1.4.8.tar` & `optioner-1.4.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 07:37:46.978065 optioner-1.4.8/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.8/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6465 2024-04-10 07:37:46.977561 optioner-1.4.8/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     4229 2024-04-10 07:33:02.000000 optioner-1.4.8/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-10 07:36:47.000000 optioner-1.4.8/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-10 07:37:46.978124 optioner-1.4.8/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 07:37:46.971458 optioner-1.4.8/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.8/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 07:37:46.976929 optioner-1.4.8/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6465 2024-04-10 07:37:46.000000 optioner-1.4.8/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      311 2024-04-10 07:37:46.000000 optioner-1.4.8/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-10 07:37:46.000000 optioner-1.4.8/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-10 07:37:46.000000 optioner-1.4.8/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     6832 2024-04-10 06:22:05.000000 optioner-1.4.8/src/optioner.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-10 07:37:46.976155 optioner-1.4.8/tests/
--rw-r--r--   0 d33pster   (501) staff       (20)     1200 2024-04-10 07:16:11.000000 optioner-1.4.8/tests/test_basic.py
--rw-r--r--   0 d33pster   (501) staff       (20)      294 2024-04-10 07:00:43.000000 optioner-1.4.8/tests/test_compulsory_args.py
--rw-r--r--   0 d33pster   (501) staff       (20)      306 2024-04-10 07:21:22.000000 optioner-1.4.8/tests/test_ifthisthennotthat.py
--rw-r--r--   0 d33pster   (501) staff       (20)      285 2024-04-10 07:00:46.000000 optioner-1.4.8/tests/test_ignore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 17:12:28.000000 optioner-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-12 17:12:33.126826 optioner-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-12 17:12:28.000000 optioner-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 17:12:28.000000 optioner-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:12:33.126826 optioner-1.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.122826 optioner-1.4.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:28.000000 optioner-1.4.9/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/src/optioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-12 17:12:28.000000 optioner-1.4.9/src/optioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_compulsory_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ifthisthennotthat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ifthisthennotthat_vigorous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ignore.py
```

### Comparing `optioner-1.4.8/LICENSE` & `optioner-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.8/PKG-INFO` & `optioner-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.8
+Version: 1.4.9
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -40,14 +40,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
+[![Continuous Deployment](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml)
 [![Feature Tests](https://github.com/d33pster/optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/pytest.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
 ![PyPI - Version](https://img.shields.io/pypi/v/optioner)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner)
 ![GitHub License](https://img.shields.io/github/license/d33pster/optioner)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.8 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.9 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -22,20 +22,23 @@
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
-[![Feature Tests](https://github.com/d33pster/optioner/actions/workflows/
-pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/
-pytest.yml) [![Build status](https://ci.appveyor.com/api/projects/status/
-qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
-![PyPI - Version](https://img.shields.io/pypi/v/optioner) ![Python Version from
-PEP 621 TOML](https://img.shields.io/python/required-version-
+[![Continuous Deployment](https://github.com/d33pster/optioner/actions/
+workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/
+actions/workflows/cont-dep.yml) [![Feature Tests](https://github.com/d33pster/
+optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/d33pster/
+optioner/actions/workflows/pytest.yml) [![Build status](https://
+ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://
+ci.appveyor.com/project/d33pster/optioner) ![PyPI - Version](https://
+img.shields.io/pypi/v/optioner) ![Python Version from PEP 621 TOML](https://
+img.shields.io/python/required-version-
 toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner) ![Dependents (via
 libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner) !
 [GitHub License](https://img.shields.io/github/license/d33pster/optioner) !
 [GitHub last commit](https://img.shields.io/github/last-commit/d33pster/
 optioner)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
```

### Comparing `optioner-1.4.8/README.md` & `optioner-1.4.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # optioner
+[![Continuous Deployment](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml)
 [![Feature Tests](https://github.com/d33pster/optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/pytest.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
 ![PyPI - Version](https://img.shields.io/pypi/v/optioner)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner)
 ![GitHub License](https://img.shields.io/github/license/d33pster/optioner)
@@ -119,8 +120,8 @@
 >> optionCTRL._argparse()
 
 >>> optionCTRL._what_is_(shortargs[0])
 
 or 
 
 >>> optionCTRL._what_is_(longargs[0])
-```
+```
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-# optioner [![Feature Tests](https://github.com/d33pster/optioner/actions/
-workflows/pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/
-workflows/pytest.yml) [![Build status](https://ci.appveyor.com/api/projects/
-status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/
-optioner) ![PyPI - Version](https://img.shields.io/pypi/v/optioner) ![Python
-Version from PEP 621 TOML](https://img.shields.io/python/required-version-
+# optioner [![Continuous Deployment](https://github.com/d33pster/optioner/
+actions/workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/
+optioner/actions/workflows/cont-dep.yml) [![Feature Tests](https://github.com/
+d33pster/optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/
+d33pster/optioner/actions/workflows/pytest.yml) [![Build status](https://
+ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://
+ci.appveyor.com/project/d33pster/optioner) ![PyPI - Version](https://
+img.shields.io/pypi/v/optioner) ![Python Version from PEP 621 TOML](https://
+img.shields.io/python/required-version-
 toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner) ![Dependents (via
 libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner) !
 [GitHub License](https://img.shields.io/github/license/d33pster/optioner) !
 [GitHub last commit](https://img.shields.io/github/last-commit/d33pster/
 optioner)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
```

### Comparing `optioner-1.4.8/pyproject.toml` & `optioner-1.4.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.8"
+version = "1.4.9"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.4.8/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.9/src/optioner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.8
+Version: 1.4.9
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -40,14 +40,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # optioner
+[![Continuous Deployment](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/cont-dep.yml)
 [![Feature Tests](https://github.com/d33pster/optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/pytest.yml)
 [![Build status](https://ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
 ![PyPI - Version](https://img.shields.io/pypi/v/optioner)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner)
 ![GitHub License](https://img.shields.io/github/license/d33pster/optioner)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.8 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.9 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -22,20 +22,23 @@
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
-[![Feature Tests](https://github.com/d33pster/optioner/actions/workflows/
-pytest.yml/badge.svg)](https://github.com/d33pster/optioner/actions/workflows/
-pytest.yml) [![Build status](https://ci.appveyor.com/api/projects/status/
-qoaeiypaxnonrosv?svg=true)](https://ci.appveyor.com/project/d33pster/optioner)
-![PyPI - Version](https://img.shields.io/pypi/v/optioner) ![Python Version from
-PEP 621 TOML](https://img.shields.io/python/required-version-
+[![Continuous Deployment](https://github.com/d33pster/optioner/actions/
+workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/
+actions/workflows/cont-dep.yml) [![Feature Tests](https://github.com/d33pster/
+optioner/actions/workflows/pytest.yml/badge.svg)](https://github.com/d33pster/
+optioner/actions/workflows/pytest.yml) [![Build status](https://
+ci.appveyor.com/api/projects/status/qoaeiypaxnonrosv?svg=true)](https://
+ci.appveyor.com/project/d33pster/optioner) ![PyPI - Version](https://
+img.shields.io/pypi/v/optioner) ![Python Version from PEP 621 TOML](https://
+img.shields.io/python/required-version-
 toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fd33pster%2Foptioner%2Fmain%2Fpyproject.toml)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/optioner) ![Dependents (via
 libraries.io)](https://img.shields.io/librariesio/dependents/pypi/Optioner) !
 [GitHub License](https://img.shields.io/github/license/d33pster/optioner) !
 [GitHub last commit](https://img.shields.io/github/last-commit/d33pster/
 optioner)
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
```

### Comparing `optioner-1.4.8/src/optioner.py` & `optioner-1.4.9/src/optioner.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,29 +85,47 @@
         # if ifthisthennotthat has pairs
         if len(self._ifthisnotthat)%2==0:
             for i in range(0,len(self._ifthisnotthat), 2):
                 ifthis = self._ifthisnotthat[i]
                 thennotthat = self._ifthisnotthat[i+1]
                 
                 for x in ifthis:
-                    if len(x)>2:
-                        x = '--' + x
+                    # if len(x)>2:
+                    #     x = '--' + x
+                    # else:
+                    #     x = '-' + x
+                    
+                    if "--"+x in self._longargs:
+                        x = '--'+x
+                    elif '-'+x in self._shortargs:
+                        x = '-'+x
                     else:
-                        x = '-' + x
+                        self._argcheck = False
+                        self._argerror = f'undefined argument \'{x}\''
                     
                     if x in self._gotargs:
                         for y in thennotthat:
-                            if len(y)>2:
-                                y = '--' + y
-                            else:
-                                y = '-' + y
+                            # if len(y)>2:
+                            #     y = '--' + y
+                            # else:
+                            #     y = '-' + y
+                            
+                            if '--'+y in self._longargs:
+                                y = '--'+y
+                            elif '-'+y in self._shortargs:
+                                y = '-'+y
                             
                             if y in self._gotargs:
                                 self._argcheck = False
                                 self._argerror = f'\'{x}\' and \'{y}\' cannot be used together.'
+                            else:
+                                # if argument is undefined
+                                self._argcheck = False
+                                self._argerror = f"undefined argument \'{y}\'"
+                                break
         else:
             self._argcheck = False
             self._argerror = 'ifthisthennotthat param value mismatch.'
         
         # if ignore args are present then ignore the errors
         for x in self._ignore:
             if x in self._gotargs:
```

### Comparing `optioner-1.4.8/tests/test_basic.py` & `optioner-1.4.9/tests/test_basic.py`

 * *Files identical despite different names*

