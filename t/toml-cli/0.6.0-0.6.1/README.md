# Comparing `tmp/toml_cli-0.6.0.tar.gz` & `tmp/toml_cli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toml_cli-0.6.0.tar", max compression
+gzip compressed data, was "toml_cli-0.6.1.tar", max compression
```

## Comparing `toml_cli-0.6.0.tar` & `toml_cli-0.6.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-09-28 22:37:02.531165 toml_cli-0.6.0/LICENSE
--rw-r--r--   0        0        0      841 2023-09-28 22:37:02.531165 toml_cli-0.6.0/README.md
--rw-r--r--   0        0        0      728 2023-09-28 22:37:02.531165 toml_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2883 2023-09-28 22:37:02.535165 toml_cli-0.6.0/toml_cli/__init__.py
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 toml_cli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 22:51:56.623251 toml_cli-0.6.1/LICENSE
+-rw-r--r--   0        0        0      842 2024-04-11 22:51:56.623251 toml_cli-0.6.1/README.md
+-rw-r--r--   0        0        0      752 2024-04-11 22:51:56.623251 toml_cli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2883 2024-04-11 22:51:56.623251 toml_cli-0.6.1/toml_cli/__init__.py
+-rw-r--r--   0        0        0     1663 1970-01-01 00:00:00.000000 toml_cli-0.6.1/PKG-INFO
```

### Comparing `toml_cli-0.6.0/LICENSE` & `toml_cli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toml_cli-0.6.0/README.md` & `toml_cli-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# tom-cli
+# toml-cli
 
 ![Build](https://github.com/mrijken/toml-cli/workflows/CI/badge.svg)
 ![Hits](https://hitcounter.pythonanywhere.com/count/tag.svg?url=https%3A%2F%2Fgithub.com%2Fmrijken%toml-cli)
 
 Command line interface for toml files.
 
 This can be usefull for getting or setting parts of a toml file without an editor.
```

### Comparing `toml_cli-0.6.0/pyproject.toml` & `toml_cli-0.6.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toml-cli"
-version = "0.6.0"
+version = "0.6.1"
 description = "Command line interface to read and write keys/values to/from toml files"
 authors = ["Marc Rijken <marc@rijken.org>"]
 license = "MIT"
 repository = "https://github.com/mrijken/toml-cli"
 readme = "README.md"
 packages = [{ include = "toml_cli" }]
 
@@ -13,23 +13,22 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typer = ">=0.3.2"
 tomlkit = ">=0.12.1"
 regex = ">=2020.7.14"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.4.2"
-black = "^23.9.1"
-
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.291"
-
-[tool.black]
-line-length = 120
+pytest = "^8.1.1"
+ruff = "^0.3"
 
 [tool.ruff]
 line-length = 120
+target-version = "py38"
+
+[tool.ruff.lint.isort]
+force-single-line = true
+known-first-party = ["pytest_nlcov"]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `toml_cli-0.6.0/toml_cli/__init__.py` & `toml_cli-0.6.1/toml_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `toml_cli-0.6.0/PKG-INFO` & `toml_cli-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: toml-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Command line interface to read and write keys/values to/from toml files
 Home-page: https://github.com/mrijken/toml-cli
 License: MIT
 Author: Marc Rijken
 Author-email: marc@rijken.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: regex (>=2020.7.14)
 Requires-Dist: tomlkit (>=0.12.1)
 Requires-Dist: typer (>=0.3.2)
 Project-URL: Repository, https://github.com/mrijken/toml-cli
 Description-Content-Type: text/markdown
 
-# tom-cli
+# toml-cli
 
 ![Build](https://github.com/mrijken/toml-cli/workflows/CI/badge.svg)
 ![Hits](https://hitcounter.pythonanywhere.com/count/tag.svg?url=https%3A%2F%2Fgithub.com%2Fmrijken%toml-cli)
 
 Command line interface for toml files.
 
 This can be usefull for getting or setting parts of a toml file without an editor.
```

