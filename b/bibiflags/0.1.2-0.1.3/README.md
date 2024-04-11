# Comparing `tmp/bibiflags-0.1.2.tar.gz` & `tmp/bibiflags-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiflags-0.1.2.tar", last modified: Wed Apr 10 08:25:54 2024, max compression
+gzip compressed data, was "bibiflags-0.1.3.tar", last modified: Thu Apr 11 23:10:33 2024, max compression
```

## Comparing `bibiflags-0.1.2.tar` & `bibiflags-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.262809 bibiflags-0.1.2/
--rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2326 2024-04-10 08:25:54.260811 bibiflags-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2024-04-10 08:23:23.000000 bibiflags-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.229810 bibiflags-0.1.2/docs/
--rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.233837 bibiflags-0.1.2/docs/source/
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.234804 bibiflags-0.1.2/docs/source/_static/
--rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.2/docs/source/_static/bibiflags.png
--rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.2/docs/source/install.rst
--rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.2/docs/source/quickstart.rst
--rw-rw-rw-   0        0        0      793 2024-04-10 08:20:51.000000 bibiflags-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 08:25:54.262809 bibiflags-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.220808 bibiflags-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.238840 bibiflags-0.1.2/src/bibiflags/
--rw-rw-rw-   0        0        0      104 2024-04-10 08:20:45.000000 bibiflags-0.1.2/src/bibiflags/__init__.py
--rw-rw-rw-   0        0        0     6660 2024-04-10 08:13:02.000000 bibiflags-0.1.2/src/bibiflags/bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.2/src/bibiflags/bibiflags.yaml
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.258808 bibiflags-0.1.2/src/bibiflags.egg-info/
--rw-rw-rw-   0        0        0     2326 2024-04-10 08:25:54.000000 bibiflags-0.1.2/src/bibiflags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-04-10 08:25:54.000000 bibiflags-0.1.2/src/bibiflags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 08:25:54.000000 bibiflags-0.1.2/src/bibiflags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 08:25:54.000000 bibiflags-0.1.2/src/bibiflags.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-10 08:25:54.000000 bibiflags-0.1.2/src/bibiflags.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.254804 bibiflags-0.1.2/src/examples/
--rw-rw-rw-   0        0        0      176 2024-04-10 08:13:56.000000 bibiflags-0.1.2/src/examples/main.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.2/src/examples/main.yaml
--rw-rw-rw-   0        0        0      376 2024-04-10 08:19:50.000000 bibiflags-0.1.2/src/examples/prog.py
--rw-rw-rw-   0        0        0        0 2024-04-10 06:01:38.000000 bibiflags-0.1.2/src/examples/prog.yaml
-drwxrwxrwx   0        0        0        0 2024-04-10 08:25:54.257804 bibiflags-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0      265 2024-04-10 07:13:27.000000 bibiflags-0.1.2/tests/test_bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.2/tests/test_bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.570620 bibiflags-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3097 2024-04-11 23:10:33.569620 bibiflags-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2519 2024-04-11 23:09:24.000000 bibiflags-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.394650 bibiflags-0.1.3/docs/
+-rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.415650 bibiflags-0.1.3/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.509650 bibiflags-0.1.3/docs/source/_static/
+-rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.3/docs/source/_static/bibiflags.png
+-rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.3/docs/source/install.rst
+-rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.3/docs/source/quickstart.rst
+-rw-rw-rw-   0        0        0      793 2024-04-11 23:09:28.000000 bibiflags-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 23:10:33.571616 bibiflags-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.377621 bibiflags-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.514619 bibiflags-0.1.3/src/bibiflags/
+-rw-rw-rw-   0        0        0      104 2024-04-11 23:09:41.000000 bibiflags-0.1.3/src/bibiflags/__init__.py
+-rw-rw-rw-   0        0        0     6831 2024-04-11 23:02:58.000000 bibiflags-0.1.3/src/bibiflags/bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.3/src/bibiflags/bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.568622 bibiflags-0.1.3/src/bibiflags.egg-info/
+-rw-rw-rw-   0        0        0     3097 2024-04-11 23:10:33.000000 bibiflags-0.1.3/src/bibiflags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2024-04-11 23:10:33.000000 bibiflags-0.1.3/src/bibiflags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 23:10:33.000000 bibiflags-0.1.3/src/bibiflags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 23:10:33.000000 bibiflags-0.1.3/src/bibiflags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-11 23:10:33.000000 bibiflags-0.1.3/src/bibiflags.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.557620 bibiflags-0.1.3/src/examples/
+-rw-rw-rw-   0        0        0      820 2024-04-11 23:05:14.000000 bibiflags-0.1.3/src/examples/initial.py
+-rw-rw-rw-   0        0        0      286 2024-04-11 23:03:50.000000 bibiflags-0.1.3/src/examples/initial.yaml
+-rw-rw-rw-   0        0        0      176 2024-04-10 08:13:56.000000 bibiflags-0.1.3/src/examples/main.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.3/src/examples/main.yaml
+-rw-rw-rw-   0        0        0      376 2024-04-10 08:19:50.000000 bibiflags-0.1.3/src/examples/prog.py
+-rw-rw-rw-   0        0        0        0 2024-04-10 06:01:38.000000 bibiflags-0.1.3/src/examples/prog.yaml
+drwxrwxrwx   0        0        0        0 2024-04-11 23:10:33.567618 bibiflags-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-04-11 22:15:38.000000 bibiflags-0.1.3/tests/test_bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.3/tests/test_bibiflags.yaml
```

### Comparing `bibiflags-0.1.2/LICENSE` & `bibiflags-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/README.md` & `bibiflags-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: bibiflags
+Version: 0.1.3
+Summary: Import YAML configs into Arguments for Python
+Author-email: Chunqi SHI <chunqishi@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bibiparrot/bibiflags
+Project-URL: Issues, https://github.com/bibiparrot/bibiflags/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyYAML>=6.0.1
+
 ![bibiflags](https://github.com/bibiparrot/bibiflags/blob/main/docs/source/_static/bibiflags.png)
 ===
 
 bibiflags is a python tool to import YAML configs into Arguments for Python . 
 
 It provides 2 ways to use it:
 
@@ -11,16 +27,14 @@
 ## Getting Started
 
 ### Requirements and Installation
 
 - Python version >= 3.8
 - libaries:
   * "PyYAML>=6.0.1"
-  * "OmegaConf>=2.3.0"
-  * "loguru>=0.7.2"
 
 ```bash
 pip install bibiflags
 ```
 
 Install from source via:
 
@@ -36,14 +50,68 @@
 cd bibiflags
 pip install -e .
 ```
 
 
 ## Usage
 
+YAML file
+
+
+```
+flags:
+  - default: string-type-arguments
+    dest: str_arg
+    help: string type args
+    option_strings:
+      - --str_arg
+      - -sa
+    type: str
+
+  - const: true
+    default: false
+    dest: bool_arg
+    help: bool type args
+    nargs: 0
+    option_strings:
+      - --bool_arg
+      - -ba
+    type: bool
+
+  - default: 8
+    dest: int_arg
+    help: int type args
+    option_strings:
+      - --int_arg
+      - -ia
+    type: int
+
+  - default: 0.1
+    dest: float_arg
+    help: float type args
+    option_strings:
+      - --float_arg
+      - -fa
+    type: float
+
+  - default:
+      - 1
+      - 2
+      - 3
+      - 4
+    dest: list_arg
+    help: list type args
+    nargs: +
+    option_strings:
+      - --list_arg
+      - -la
+    type: int
+```
+
+
 ### Parse all Arguments from YAML
 ```
 from pathlib import Path
 
 from bibiflags import BibiFlags
 
 if __name__ == '__main__':
@@ -71,8 +139,8 @@
     print(flags.parameters)
 
 
 ```
 
 ## Changelog
 
-### Version 0.1.2 2024-4-10
+### Version 0.1.3 2024-4-12
```

### Comparing `bibiflags-0.1.2/docs/Makefile` & `bibiflags-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/docs/source/_static/bibiflags.png` & `bibiflags-0.1.3/docs/source/_static/bibiflags.png`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/docs/source/conf.py` & `bibiflags-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/docs/source/quickstart.rst` & `bibiflags-0.1.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/pyproject.toml` & `bibiflags-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bibiflags"
-version = "0.1.2"
+version = "0.1.3"
 description = "Import YAML configs into Arguments for Python"
 authors = [
     {name = "Chunqi SHI", email = "chunqishi@gmail.com"},
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `bibiflags-0.1.2/src/bibiflags/bibiflags.py` & `bibiflags-0.1.3/src/bibiflags/bibiflags.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,20 +104,19 @@
                 flags.append(flag)
         config = dict()
         config[key] = flags
         BibiFlags.yaml_dump(config, yaml_file, encoding=encoding)
         # with open(yaml_file, 'w', encoding=encoding) as fp:
         #     OmegaConf.save(config=config, f=fp)
 
-
     @staticmethod
     def contains_yaml(yaml_file: str, encoding='utf-8', key='ArgumentParser'):
         # with open(yaml_file, 'r', encoding=encoding) as fp:
         #     config = OmegaConf.load(fp)
-        config = BibiFlags.yaml_load(yaml_file, encoding=encoding )
+        config = BibiFlags.yaml_load(yaml_file, encoding=encoding)
         return key in config
 
     @staticmethod
     def from_yaml(yaml_file: str, parser=None, encoding='utf-8', key='ArgumentParser') -> argparse.ArgumentParser:
         # with open(yaml_file, 'r', encoding=encoding) as fp:
         #     config = OmegaConf.load(fp)
         #     config = OmegaConf.to_object(config)
@@ -128,15 +127,19 @@
             logger.warning(f"Flags {key} NOT in {os.path.abspath(yaml_file)}")
         parser = argparse.ArgumentParser() if parser is None else parser
         for item in items:
             if item.get('type', 'str') == 'bool':
                 item['type'] = None
             else:
                 item['type'] = getattr(builtins, item.get('type', 'str'))
-            action = argparse.Action(**item)
+            if item.get('option_strings', None):
+                action = argparse.Action(**item)
+            else:
+                item['option_strings'] = []
+                action = argparse._StoreAction(**item)
             if action.dest not in [_action.dest for _action in parser._actions]:
                 parser._add_action(action)
             else:
                 logger.warning(f"CONFLICT ARGS '{action.dest}', NOT USED {os.path.abspath(yaml_file)}")
         return parser
 
     @staticmethod
```

### Comparing `bibiflags-0.1.2/src/bibiflags/bibiflags.yaml` & `bibiflags-0.1.3/src/bibiflags/bibiflags.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/src/bibiflags.egg-info/SOURCES.txt` & `bibiflags-0.1.3/src/bibiflags.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 src/bibiflags/bibiflags.py
 src/bibiflags/bibiflags.yaml
 src/bibiflags.egg-info/PKG-INFO
 src/bibiflags.egg-info/SOURCES.txt
 src/bibiflags.egg-info/dependency_links.txt
 src/bibiflags.egg-info/requires.txt
 src/bibiflags.egg-info/top_level.txt
+src/examples/initial.py
+src/examples/initial.yaml
 src/examples/main.py
 src/examples/main.yaml
 src/examples/prog.py
 src/examples/prog.yaml
 tests/__init__.py
 tests/test_bibiflags.py
 tests/test_bibiflags.yaml
```

### Comparing `bibiflags-0.1.2/src/examples/main.yaml` & `bibiflags-0.1.3/src/examples/main.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.2/tests/test_bibiflags.yaml` & `bibiflags-0.1.3/tests/test_bibiflags.yaml`

 * *Files identical despite different names*

