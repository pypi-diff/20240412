# Comparing `tmp/install-preserve-0.0.2.tar.gz` & `tmp/install-preserve-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-preserve-0.0.2.tar", last modified: Sat Apr  6 19:15:30 2024, max compression
+gzip compressed data, was "install-preserve-0.0.3.tar", last modified: Fri Apr 12 14:13:28 2024, max compression
```

## Comparing `install-preserve-0.0.2.tar` & `install-preserve-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:15:30.327878 install-preserve-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-06 19:15:27.000000 install-preserve-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-06 19:15:30.327878 install-preserve-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-06 19:15:27.000000 install-preserve-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:15:30.327878 install-preserve-0.0.2/install_preserve/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-06 19:15:27.000000 install-preserve-0.0.2/install_preserve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:15:30.327878 install-preserve-0.0.2/install_preserve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-06 19:15:30.000000 install-preserve-0.0.2/install_preserve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 19:15:30.000000 install-preserve-0.0.2/install_preserve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:15:30.000000 install-preserve-0.0.2/install_preserve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 19:15:30.000000 install-preserve-0.0.2/install_preserve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:15:30.327878 install-preserve-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-06 19:15:27.000000 install-preserve-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:28.064424 install-preserve-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 14:13:24.000000 install-preserve-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 14:13:28.064424 install-preserve-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-12 14:13:24.000000 install-preserve-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:28.064424 install-preserve-0.0.3/install_preserve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-12 14:13:24.000000 install-preserve-0.0.3/install_preserve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:28.064424 install-preserve-0.0.3/install_preserve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 14:13:28.000000 install-preserve-0.0.3/install_preserve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 14:13:28.000000 install-preserve-0.0.3/install_preserve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:13:28.000000 install-preserve-0.0.3/install_preserve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 14:13:28.000000 install-preserve-0.0.3/install_preserve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:13:28.064424 install-preserve-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-12 14:13:24.000000 install-preserve-0.0.3/setup.py
```

### Comparing `install-preserve-0.0.2/LICENSE` & `install-preserve-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `install-preserve-0.0.2/PKG-INFO` & `install-preserve-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-preserve
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library that helps prevent accidental overwrites of hand-compiled libraries
 Home-page: https://github.com/manbehindthemadness/install-preserve
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `install-preserve-0.0.2/README.md` & `install-preserve-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `install-preserve-0.0.2/install_preserve/__init__.py` & `install-preserve-0.0.3/install_preserve/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 
 
 def preserve(requirements: list[str], criteria: list[str], verbose: bool = False) -> list:
     """
     Preserve packages listed in the criteria argument if they are already installed.
     """
     package_names = list()
-    for requirement in requirements:
-        package_names.append(re.sub(r'[^a-zA-Z0-9]+$', '', requirement.split('=')[0]))
+    for idx, requirement in enumerate(requirements):
+        if '@' in requirement:
+            package_names.append(requirement.split('@')[0].strip())
+        else:
+            package_names.append(re.sub(r'[^a-zA-Z0-9]+$', '', requirement.split('=')[0]))
+
     for item in criteria:
         alias = name = item
         if ':' in item:
+
             name, alias = item.split(':')
         if importlib.util.find_spec(alias) is not None:
             if verbose:
                 logging.info(f'excluding package {name} as it is already installed')
             index = package_names.index(name)
             package_names.pop(index)
             requirements.pop(index)
```

### Comparing `install-preserve-0.0.2/install_preserve.egg-info/PKG-INFO` & `install-preserve-0.0.3/install_preserve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-preserve
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library that helps prevent accidental overwrites of hand-compiled libraries
 Home-page: https://github.com/manbehindthemadness/install-preserve
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `install-preserve-0.0.2/setup.py` & `install-preserve-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='install-preserve',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
     author_email='manbehindthemadness@gmail.com',
```

