# Comparing `tmp/knewkarma-4.0.0.tar.gz` & `tmp/knewkarma-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knewkarma-4.0.0.tar", max compression
+gzip compressed data, was "knewkarma-4.1.0.tar", max compression
```

## Comparing `knewkarma-4.0.0.tar` & `knewkarma-4.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1096 2024-04-03 09:39:44.778229 knewkarma-4.0.0/LICENSE
--rw-r--r--   0        0        0     3902 2024-04-03 09:39:44.778229 knewkarma-4.0.0/README.md
--rw-r--r--   0        0        0      215 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/__init__.py
--rw-r--r--   0        0        0    14388 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_api.py
--rw-r--r--   0        0        0    18824 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_cli.py
--rw-r--r--   0        0        0    26269 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_core.py
--rw-r--r--   0        0        0     8719 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_parsers.py
--rw-r--r--   0        0        0     8694 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/_utils.py
--rw-r--r--   0        0        0     4297 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/docs.py
--rw-r--r--   0        0        0      907 2024-04-03 09:39:44.778229 knewkarma-4.0.0/knewkarma/version.py
--rw-r--r--   0        0        0     1296 2024-04-03 09:39:44.778229 knewkarma-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 knewkarma-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-12 03:24:17.893422 knewkarma-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5695 2024-04-12 03:24:17.893422 knewkarma-4.1.0/README.md
+-rw-r--r--   0        0        0      215 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/__init__.py
+-rw-r--r--   0        0        0    14388 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/_api.py
+-rw-r--r--   0        0        0    18825 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/_cli.py
+-rw-r--r--   0        0        0    26269 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/_core.py
+-rw-r--r--   0        0        0     8719 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/_parsers.py
+-rw-r--r--   0        0        0     8694 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/_utils.py
+-rw-r--r--   0        0        0     4297 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/docs.py
+-rw-r--r--   0        0        0      907 2024-04-12 03:24:17.893422 knewkarma-4.1.0/knewkarma/version.py
+-rw-r--r--   0        0        0     1296 2024-04-12 03:24:17.893422 knewkarma-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6892 1970-01-01 00:00:00.000000 knewkarma-4.1.0/PKG-INFO
```

### Comparing `knewkarma-4.0.0/LICENSE` & `knewkarma-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/_api.py` & `knewkarma-4.1.0/knewkarma/_api.py`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/_cli.py` & `knewkarma-4.1.0/knewkarma/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         action="store_true",
     )
 
     subreddits_parser = subparsers.add_parser(
         "subreddits",
         help="subreddits module ([bold][green]bulk[/][/])",
         description=Markdown(
-            "**Subreddits*: *Pull subreddits from various sources.*",
+            "**Subreddits**: *Pull subreddits from various sources.*",
             style="argparse.text",
         ),
         epilog=Markdown(Docs.examples["subreddits"]),
         formatter_class=RichHelpFormatter,
     )
     subreddits_parser.add_argument(
         "-a",
```

### Comparing `knewkarma-4.0.0/knewkarma/_core.py` & `knewkarma-4.1.0/knewkarma/_core.py`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/_parsers.py` & `knewkarma-4.1.0/knewkarma/_parsers.py`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/_utils.py` & `knewkarma-4.1.0/knewkarma/_utils.py`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/docs.py` & `knewkarma-4.1.0/knewkarma/docs.py`

 * *Files identical despite different names*

### Comparing `knewkarma-4.0.0/knewkarma/version.py` & `knewkarma-4.1.0/knewkarma/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,11 @@
         minor (str): The minor version number, representing minor improvements and significant fixes.
         patch (str): The patch version number, typically used for small fixes and updates.
         full (str): A composite string representing the full version, combining major, minor, and patch.
         release (str): A string representing the release version, combining only the major and minor numbers.
     """
 
     major: str = "4"
-    minor: str = "0"
+    minor: str = "1"
     patch: str = "0"
     full: str = f"{major}.{minor}.{patch}"
     release: str = f"{major}.{minor}"
```

### Comparing `knewkarma-4.0.0/pyproject.toml` & `knewkarma-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "knewkarma"
-version = "4.0.0"
+version = "4.1.0"
 description = "A Reddit Data Analysis Toolkit"
 authors = ["Richard Mwewa <rly0nheart@gagpasta.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://pypi.org/project/knewkarma"
 documentation = "https://knewkarma-wiki.readthedocs.io"
 repository = "https://github.com/bellingcat/knewkarma"
```

