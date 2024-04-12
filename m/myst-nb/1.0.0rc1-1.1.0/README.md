# Comparing `tmp/myst_nb-1.0.0rc1.tar.gz` & `tmp/myst_nb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myst_nb-1.0.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myst_nb-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myst_nb-1.0.0rc1.tar` & `myst_nb-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      529 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     3264 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1888 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1181 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      259 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/.readthedocs.yml
--rw-r--r--   0        0        0    23178 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0     1529 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     1499 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/README.md
--rw-r--r--   0        0        0      162 2023-11-07 20:39:15.160529 myst_nb-1.0.0rc1/codecov.yml
--rw-r--r--   0        0        0     1130 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/__init__.py
--rw-r--r--   0        0        0      221 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/_compat.py
--rw-r--r--   0        0        0     5086 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/cli.py
--rw-r--r--   0        0        0      647 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/__init__.py
--rw-r--r--   0        0        0    21839 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/config.py
--rw-r--r--   0        0        0     2784 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/execute/__init__.py
--rw-r--r--   0        0        0     5573 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/execute/base.py
--rw-r--r--   0        0        0     4510 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/execute/cache.py
--rw-r--r--   0        0        0     2417 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/execute/direct.py
--rw-r--r--   0        0        0     7528 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/execute/inline.py
--rw-r--r--   0        0        0     5490 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/lexers.py
--rw-r--r--   0        0        0     5230 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/loggers.py
--rw-r--r--   0        0        0     5534 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/nb_to_tokens.py
--rw-r--r--   0        0        0    14280 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/read.py
--rw-r--r--   0        0        0    47062 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/render.py
--rw-r--r--   0        0        0     1978 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/utils.py
--rw-r--r--   0        0        0     6454 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/core/variables.py
--rw-r--r--   0        0        0    15354 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/docutils_.py
--rw-r--r--   0        0        0        0 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/__init__.py
--rw-r--r--   0        0        0     1025 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/download.py
--rw-r--r--   0        0        0     8008 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/eval/__init__.py
--rw-r--r--   0        0        0     5285 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/execution_tables.py
--rw-r--r--   0        0        0     4145 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/__init__.py
--rw-r--r--   0        0        0     4291 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/crossref.py
--rw-r--r--   0        0        0     9378 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/directives.py
--rw-r--r--   0        0        0     1185 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/domain.py
--rw-r--r--   0        0        0     5826 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/roles.py
--rw-r--r--   0        0        0     2607 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/glue/utils.py
--rw-r--r--   0        0        0     2449 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/ext/utils.py
--rw-r--r--   0        0        0    23248 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/sphinx_.py
--rw-r--r--   0        0        0     8690 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/sphinx_ext.py
--rw-r--r--   0        0        0        0 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/static/__init__.py
--rw-r--r--   0        0        0    39364 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/static/mystnb.css
--rw-r--r--   0        0        0     3074 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/myst_nb/warnings_.py
--rw-r--r--   0        0        0     4370 2023-11-07 20:39:15.164529 myst_nb-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1246 2023-11-07 20:39:15.172529 myst_nb-1.0.0rc1/tox.ini
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 myst_nb-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      529 2024-04-12 14:03:17.972656 myst_nb-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3264 2024-04-12 14:03:17.972656 myst_nb-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1888 2024-04-12 14:03:17.972656 myst_nb-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1181 2024-04-12 14:03:17.972656 myst_nb-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      259 2024-04-12 14:03:17.972656 myst_nb-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0    33284 2024-04-12 14:03:17.972656 myst_nb-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1529 2024-04-12 14:03:17.972656 myst_nb-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1499 2024-04-12 14:03:17.972656 myst_nb-1.1.0/README.md
+-rw-r--r--   0        0        0      162 2024-04-12 14:03:17.972656 myst_nb-1.1.0/codecov.yml
+-rw-r--r--   0        0        0     1127 2024-04-12 14:03:17.972656 myst_nb-1.1.0/myst_nb/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-12 14:03:17.972656 myst_nb-1.1.0/myst_nb/_compat.py
+-rw-r--r--   0        0        0     5156 2024-04-12 14:03:17.972656 myst_nb-1.1.0/myst_nb/cli.py
+-rw-r--r--   0        0        0      647 2024-04-12 14:03:17.972656 myst_nb-1.1.0/myst_nb/core/__init__.py
+-rw-r--r--   0        0        0    22005 2024-04-12 14:03:17.972656 myst_nb-1.1.0/myst_nb/core/config.py
+-rw-r--r--   0        0        0     2784 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/execute/__init__.py
+-rw-r--r--   0        0        0     5609 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/execute/base.py
+-rw-r--r--   0        0        0     4540 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/execute/cache.py
+-rw-r--r--   0        0        0     2455 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/execute/direct.py
+-rw-r--r--   0        0        0     7634 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/execute/inline.py
+-rw-r--r--   0        0        0     5496 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/lexers.py
+-rw-r--r--   0        0        0     5252 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/loggers.py
+-rw-r--r--   0        0        0     5534 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/nb_to_tokens.py
+-rw-r--r--   0        0        0    14438 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/read.py
+-rw-r--r--   0        0        0    47560 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/render.py
+-rw-r--r--   0        0        0     1978 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/utils.py
+-rw-r--r--   0        0        0     6474 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/core/variables.py
+-rw-r--r--   0        0        0    15636 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/docutils_.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/download.py
+-rw-r--r--   0        0        0     8046 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/eval/__init__.py
+-rw-r--r--   0        0        0     5395 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/execution_tables.py
+-rw-r--r--   0        0        0     4159 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/__init__.py
+-rw-r--r--   0        0        0     4395 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/crossref.py
+-rw-r--r--   0        0        0     9416 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/directives.py
+-rw-r--r--   0        0        0     1185 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/domain.py
+-rw-r--r--   0        0        0     5902 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/roles.py
+-rw-r--r--   0        0        0     2665 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/glue/utils.py
+-rw-r--r--   0        0        0     2449 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/ext/utils.py
+-rw-r--r--   0        0        0    23724 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/sphinx_.py
+-rw-r--r--   0        0        0     8808 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/sphinx_ext.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/static/__init__.py
+-rw-r--r--   0        0        0    39364 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/static/mystnb.css
+-rw-r--r--   0        0        0     3080 2024-04-12 14:03:17.976656 myst_nb-1.1.0/myst_nb/warnings_.py
+-rw-r--r--   0        0        0     4357 2024-04-12 14:03:17.976656 myst_nb-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1246 2024-04-12 14:03:17.984656 myst_nb-1.1.0/tox.ini
+-rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 myst_nb-1.1.0/PKG-INFO
```

### Comparing `myst_nb-1.0.0rc1/.github/dependabot.yml` & `myst_nb-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/.github/workflows/tests.yml` & `myst_nb-1.1.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
     - uses: pre-commit/action@v3.0.0
 
   tests:
 
     strategy:
@@ -51,15 +51,15 @@
             myst-parser: "~=2.0.0"
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
     - name: Install myst-nb with Sphinx ${{ matrix.sphinx }}
       run: |
         pip install --upgrade pip
         pip install --upgrade "Sphinx${{ matrix.sphinx }}" "myst-parser${{ matrix.myst-parser }}" -e .[testing]
@@ -70,15 +70,15 @@
   coverage:
     needs: [tests]
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.11"
         cache: pip
     - name: Install dependencies
       run: |
         pip install --upgrade pip
         pip install -e .[testing]
@@ -104,15 +104,15 @@
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
       uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
```

### Comparing `myst_nb-1.0.0rc1/.gitignore` & `myst_nb-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/.pre-commit-config.yaml` & `myst_nb-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/LICENSE` & `myst_nb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/README.md` & `myst_nb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/__init__.py` & `myst_nb-1.1.0/myst_nb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """A docutils/sphinx parser for Jupyter Notebooks."""
-__version__ = "1.0.0rc1"
+__version__ = "1.1.0"
 
 
 def setup(app):
     """Sphinx extension setup."""
     # we import this locally, so sphinx is not automatically imported
     from .sphinx_ext import sphinx_setup
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/cli.py` & `myst_nb-1.1.0/myst_nb/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,33 @@
     # create directory
     path.mkdir(parents=True, exist_ok=True)
     # write .gitignore
     (path / ".gitignore").write_text(".ipynb_checkpoints\n_build\n", encoding="utf-8")
     # write conf.py
     (path / "conf.py").write_text(generate_conf_py(), encoding="utf-8")
     # write index.md
-    (path / "index.md").write_text(generate_index(["notebook1", "notebook2"]), encoding="utf-8")
+    (path / "index.md").write_text(
+        generate_index(["notebook1", "notebook2"]), encoding="utf-8"
+    )
     # write notebook1.ipynb
     (path / "notebook1.ipynb").write_text(generate_jupyter_notebook(), encoding="utf-8")
     # write notebook2.md
     (path / "notebook2.md").write_text(generate_text_notebook(), encoding="utf-8")
 
     print(f"Created myst_nb project at: {path}")
 
 
 def create_quickstart_cli():
     cli = argparse.ArgumentParser(description="Create a basic myst_nb project.")
-    cli.add_argument("path", metavar="PATH", type=str, help="Directory to output the project.")
-    cli.add_argument("-o", "--overwrite", action="store_true", help="Overwrite existing files.")
+    cli.add_argument(
+        "path", metavar="PATH", type=str, help="Directory to output the project."
+    )
+    cli.add_argument(
+        "-o", "--overwrite", action="store_true", help="Overwrite existing files."
+    )
     cli.add_argument("-v", "--verbose", action="store_true", help="Increase verbosity.")
     return cli
 
 
 def generate_conf_py() -> str:
     """Generate `conf.py` content."""
     content = (
@@ -156,18 +162,22 @@
     print(f"Wrote notebook to: {outpath}")
 
 
 def create_md_to_nb_cli():
     cli = argparse.ArgumentParser(
         description="Convert a text-based notebook to a Jupyter notebook."
     )
-    cli.add_argument("inpath", metavar="PATH_IN", type=str, help="Path to Markdown file.")
+    cli.add_argument(
+        "inpath", metavar="PATH_IN", type=str, help="Path to Markdown file."
+    )
     cli.add_argument(
         "outpath",
         metavar="PATH_OUT",
         nargs="?",
         type=str,
         help="Path to output to.",
     )
-    cli.add_argument("-o", "--overwrite", action="store_true", help="Overwrite existing files.")
+    cli.add_argument(
+        "-o", "--overwrite", action="store_true", help="Overwrite existing files."
+    )
     cli.add_argument("-v", "--verbose", action="store_true", help="Increase verbosity.")
     return cli
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/__init__.py` & `myst_nb-1.1.0/myst_nb/core/__init__.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/config.py` & `myst_nb-1.1.0/myst_nb/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,39 @@
     output: Dict[str, Tuple[str, dict, bool]] = {}
     for suffix, reader in value.items():
         if not isinstance(suffix, str):
             raise TypeError(f"`nb_custom_formats` keys must be a string: {suffix}")
         if isinstance(reader, str):
             output[suffix] = (reader, {}, False)
         elif not isinstance(reader, Sequence):
-            raise TypeError(f"`nb_custom_formats` values must be a string or sequence: {reader}")
+            raise TypeError(
+                f"`nb_custom_formats` values must be a string or sequence: {reader}"
+            )
         elif len(reader) == 2:
             output[suffix] = (reader[0], reader[1], False)
         elif len(reader) == 3:
             output[suffix] = (reader[0], reader[1], reader[2])
         else:
             raise TypeError(
                 f"`nb_custom_formats` values must be a string, of sequence of length "
                 f"2 or 3: {reader}"
             )
         if not isinstance(output[suffix][0], str):
-            raise TypeError(f"`nb_custom_formats` values[0] must be a string: {output[suffix][0]}")
+            raise TypeError(
+                f"`nb_custom_formats` values[0] must be a string: {output[suffix][0]}"
+            )
             # TODO check can be loaded as a python object?
         if not isinstance(output[suffix][1], dict):
-            raise TypeError(f"`nb_custom_formats` values[1] must be a dict: {output[suffix][1]}")
+            raise TypeError(
+                f"`nb_custom_formats` values[1] must be a dict: {output[suffix][1]}"
+            )
         if not isinstance(output[suffix][2], bool):
-            raise TypeError(f"`nb_custom_formats` values[2] must be a bool: {output[suffix][2]}")
+            raise TypeError(
+                f"`nb_custom_formats` values[2] must be a bool: {output[suffix][2]}"
+            )
     return output
 
 
 def ipywidgets_js_factory() -> Dict[str, Dict[str, str]]:
     """Create a default ipywidgets js dict."""
     # see: https://ipywidgets.readthedocs.io/en/7.6.5/embedding.html
     return {
@@ -252,19 +260,20 @@
             "sections": (Section.global_lvl, Section.file_lvl, Section.execute),
         },
     )
     execution_raise_on_error: bool = dc.field(
         default=False,
         metadata={
             "validator": instance_of(bool),
-            "help": "Raise an exception on failed execution, " "rather than emitting a warning",
+            "help": "Raise an exception on failed execution, "
+            "rather than emitting a warning",
             "sections": (Section.global_lvl, Section.file_lvl, Section.execute),
         },
     )
-    execution_show_tb: bool = dc.field(  # TODO implement
+    execution_show_tb: bool = dc.field(
         default=False,
         metadata={
             "validator": instance_of(bool),
             "help": "Print traceback to stderr on execution error",
             "legacy_name": "execution_show_tb",
             "sections": (Section.global_lvl, Section.file_lvl, Section.execute),
         },
@@ -376,25 +385,29 @@
         },
         repr=False,
     )
     mime_priority_overrides: Sequence[Tuple[str, str, Optional[int]]] = dc.field(
         default=(),
         metadata={
             "validator": deep_iterable(
-                has_items(instance_of(str), instance_of(str), optional(instance_of(int))),
+                has_items(
+                    instance_of(str), instance_of(str), optional(instance_of(int))
+                ),
             ),
             "help": "Overrides for the base render priority of mime types: "
             "list of (builder name, mime type, priority)",
             # TODO how to allow this in docutils?
             "omit": ["docutils"],
             "sections": (Section.global_lvl, Section.file_lvl, Section.render),
         },
         repr=False,
     )
-    output_stderr: Literal["show", "remove", "remove-warn", "warn", "error", "severe"] = dc.field(
+    output_stderr: Literal[
+        "show", "remove", "remove-warn", "warn", "error", "severe"
+    ] = dc.field(
         default="show",
         metadata={
             "validator": in_(
                 [
                     "show",
                     "remove",
                     "remove-warn",
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/execute/__init__.py` & `myst_nb-1.1.0/myst_nb/core/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/execute/base.py` & `myst_nb-1.1.0/myst_nb/core/execute/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         ]
 
     @final
     def __enter__(self) -> NotebookClientBase:
         """Enter the context manager."""
         self.start_client()
         # extract glue data from the notebook
-        self._glue_data = extract_glue_data(self.notebook, self._source_map, self.logger)
+        self._glue_data = extract_glue_data(
+            self.notebook, self._source_map, self.logger
+        )
         return self
 
     @final
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Exit the context manager."""
         self.close_client(exc_type, exc_val, exc_tb)
 
@@ -148,15 +150,17 @@
         metadata = self.notebook.get("metadata", {})
         langinfo = metadata.get("language_info") or {}
         lexer = langinfo.get("pygments_lexer") or langinfo.get("name", None)
         if lexer is None:
             lexer = (metadata.get("kernelspec") or {}).get("language", None)
         return lexer
 
-    def code_cell_outputs(self, cell_index: int) -> tuple[int | None, list[NotebookNode]]:
+    def code_cell_outputs(
+        self, cell_index: int
+    ) -> tuple[int | None, list[NotebookNode]]:
         """Get the outputs of a cell.
 
         :returns: a tuple of the execution_count and the outputs
         :raises IndexError: if the cell index is out of range
         """
         cells = self.notebook.get("cells", [])
         cell = cells[cell_index]
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/execute/cache.py` & `myst_nb-1.1.0/myst_nb/core/execute/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,17 @@
                 "succeeded": True,
                 "error": None,
                 "traceback": None,
             }
             return
 
         if self.path is None:
-            raise ValueError("Input source must exist as file, if execution_mode is 'cache'")
+            raise ValueError(
+                "Input source must exist as file, if execution_mode is 'cache'"
+            )
 
         # attempt to execute the notebook
         read_fmt = self._kwargs.get("read_fmt", None)
         if read_fmt is not None:
             stage_record = cache.add_nb_to_project(str(self.path), read_data=read_fmt)
         else:
             stage_record = cache.add_nb_to_project(str(self.path))
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/execute/direct.py` & `myst_nb-1.1.0/myst_nb/core/execute/direct.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     def start_client(self):
         # setup the execution current working directory
         cwd_context: ContextManager[str]
         if self.nb_config.execution_in_temp:
             cwd_context = TemporaryDirectory()
         else:
             if self.path is None:
-                raise ValueError("Input source must exist as file, if execution_in_temp=False")
+                raise ValueError(
+                    "Input source must exist as file, if execution_in_temp=False"
+                )
             cwd_context = nullcontext(str(self.path.parent))
 
         # execute in the context of the current working directory
         with cwd_context as cwd:
             cwd = os.path.abspath(cwd)
             self.logger.info(
                 "Executing notebook using "
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/execute/inline.py` & `myst_nb-1.1.0/myst_nb/core/execute/inline.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     def start_client(self):
         self._tmp_path = None
         if self.nb_config.execution_in_temp:
             self._tmp_path = mkdtemp()
             resources = {"metadata": {"path": self._tmp_path}}
         else:
             if self.path is None:
-                raise ValueError("Input source must exist as file, if execution_in_temp=False")
+                raise ValueError(
+                    "Input source must exist as file, if execution_in_temp=False"
+                )
             resources = {"metadata": {"path": str(self.path.parent)}}
 
         self.logger.info("Starting inline execution client")
 
         self._time_start = time.perf_counter()
         self._client = ModifiedNotebookClient(
             self.notebook,
@@ -62,15 +64,17 @@
             self._client.start_new_kernel_client()
 
         # retrieve the the language_info from the kernel
         assert self._client.kc is not None
         msg_id = self._client.kc.kernel_info()
         info_msg = self._client.wait_for_reply(msg_id)
         if info_msg is not None and "language_info" in info_msg["content"]:
-            self.notebook.metadata["language_info"] = info_msg["content"]["language_info"]
+            self.notebook.metadata["language_info"] = info_msg["content"][
+                "language_info"
+            ]
         else:
             self.logger.warning("Failed to retrieve language info from kernel")
 
         self._last_cell_executed: int = -1
         self._cell_error: None | Exception = None
         self._exc_string: None | str = None
 
@@ -88,28 +92,32 @@
 
         _exec_time = time.perf_counter() - self._time_start
         self.exec_metadata = {
             "mtime": datetime.now().timestamp(),
             "runtime": _exec_time,
             "method": self.nb_config.execution_mode,
             "succeeded": False if self._cell_error else True,
-            "error": f"{self._cell_error.__class__.__name__}" if self._cell_error else None,
+            "error": f"{self._cell_error.__class__.__name__}"
+            if self._cell_error
+            else None,
             "traceback": self._exc_string,
         }
         if not self._cell_error:
             self.logger.info(f"Executed notebook in {_exec_time:.2f} seconds")
         else:
             msg = f"Executing notebook failed: {self._cell_error.__class__.__name__}"
             if self.nb_config.execution_show_tb:
                 msg += f"\n{self._exc_string}"
             self.logger.warning(msg, subtype="exec")
         if self._tmp_path:
             shutil.rmtree(self._tmp_path, ignore_errors=True)
 
-    def code_cell_outputs(self, cell_index: int) -> tuple[int | None, list[NotebookNode]]:
+    def code_cell_outputs(
+        self, cell_index: int
+    ) -> tuple[int | None, list[NotebookNode]]:
         cells = self.notebook.get("cells", [])
 
         # ensure all cells up to and including the requested cell have been executed
         while (not self._cell_error) and cell_index > self._last_cell_executed:
             self._last_cell_executed += 1
             try:
                 next_cell = cells[self._last_cell_executed]
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/lexers.py` & `myst_nb-1.1.0/myst_nb/core/lexers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     4: "Blue",
     5: "Magenta",
     6: "Cyan",
     7: "White",
 }
 
 
-def _token_from_lexer_state(bold: bool, faint: bool, fg_color: str | None, bg_color: str | None):
+def _token_from_lexer_state(
+    bold: bool, faint: bool, fg_color: str | None, bg_color: str | None
+):
     """Construct a token given the current lexer state.
 
     We can only emit one token even though we have a multiple-tuple state.
     To do work around this, we construct tokens like "Bold.Red".
     """
     components: tuple[str, ...] = ()
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/loggers.py` & `myst_nb-1.1.0/myst_nb/core/loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
         "color",
         "once",
         "line",
         "parent",
     ]
 
     def __init__(self, document: nodes.document, type_name: str = DEFAULT_LOG_TYPE):
-        self.logger: logging.Logger = logging.getLogger(f"{type_name}-{document.source}")
+        self.logger: logging.Logger = logging.getLogger(
+            f"{type_name}-{document.source}"
+        )
         # docutils handles the level of output logging
         self.logger.setLevel(logging.DEBUG)
         if not self.logger.handlers:
             self.logger.addHandler(DocutilsLogHandler(document))
 
         # default extras to parse to sphinx logger
         # location can be: docname, (docname, lineno), or a node
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/nb_to_tokens.py` & `myst_nb-1.1.0/myst_nb/core/nb_to_tokens.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/read.py` & `myst_nb-1.1.0/myst_nb/core/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,17 @@
         metadata = yaml.safe_load("".join(top_matter))
         assert isinstance(metadata, dict)
     except Exception:
         return False
     if "file_format" in metadata and metadata["file_format"] == "mystnb":
         return True
     if (
-        metadata.get("jupytext", {}).get("text_representation", {}).get("format_name", None)
+        metadata.get("jupytext", {})
+        .get("text_representation", {})
+        .get("format_name", None)
         != "myst"
     ):
         return False
 
     return True
 
     # TODO move this to reader, since not strictly part of function objective
@@ -158,15 +160,17 @@
 
 
 def myst_nb_reader_plugin(uri: str) -> nbf.NotebookNode:
     """Read a myst notebook from a string.
 
     Used as plugin for jupyter-cache.
     """
-    return read_myst_markdown_notebook(Path(uri).read_text("utf8"), add_source_map=True, path=uri)
+    return read_myst_markdown_notebook(
+        Path(uri).read_text("utf8"), add_source_map=True, path=uri
+    )
 
 
 def read_myst_markdown_notebook(
     text,
     config: MdParserConfig | None = None,
     code_directive="{code-cell}",
     raw_directive="{raw-cell}",
@@ -185,15 +189,17 @@
     :raises MystMetadataParsingError if the metadata block is not valid JSON/YAML
 
     NOTE: we assume here that all of these directives are at the top-level,
     i.e. not nested in other directives.
     """
     config = config or MdParserConfig()
     # parse markdown file up to the block level (i.e. don't worry about inline text)
-    inline_config = dc.replace(config, disable_syntax=(list(config.disable_syntax) + ["inline"]))
+    inline_config = dc.replace(
+        config, disable_syntax=(list(config.disable_syntax) + ["inline"])
+    )
     parser = create_md_parser(inline_config, RendererHTML)
     tokens = parser.parse(text + "\n")
     lines = text.splitlines()
     md_start_line = 0
 
     # get the document metadata
     metadata_nb = {}
@@ -223,15 +229,17 @@
     def _flush_markdown(start_line, token, md_metadata):
         """When we find a cell we check if there is preceding text.o"""
         endline = token.map[0] if token else len(lines)
         md_source = _strip_blank_lines("\n".join(lines[start_line:endline]))
         meta = nbf.from_dict(md_metadata)
         if md_source:
             source_map.append(start_line)
-            notebook.cells.append(nbf_version.new_markdown_cell(source=md_source, metadata=meta))
+            notebook.cells.append(
+                nbf_version.new_markdown_cell(source=md_source, metadata=meta)
+            )
 
     # iterate through the tokens to identify notebook cells
     nesting_level = 0
     md_metadata: dict = {}
 
     for token in tokens:
         nesting_level += token.nesting
@@ -243,15 +251,17 @@
         token_map = token.map or [0, 0]
 
         if token.type == "fence" and token.info.startswith(code_directive):
             _flush_markdown(md_start_line, token, md_metadata)
             options, body_lines = _read_fenced_cell(token, len(notebook.cells), "Code")
             # Parse :load: or load: tags and populate body with contents of file
             if "load" in options:
-                body_lines = _load_code_from_file(path, options["load"], token, body_lines)
+                body_lines = _load_code_from_file(
+                    path, options["load"], token, body_lines
+                )
             meta = nbf.from_dict(options)
             source_map.append(token_map[0] + 1)
             notebook.cells.append(
                 nbf_version.new_code_cell(source="\n".join(body_lines), metadata=meta)
             )
             md_metadata = {}
             md_start_line = token_map[1]
@@ -329,21 +339,25 @@
             raise MystMetadataParsingError(
                 "Markdown cell {} at line {} could not be read: {}".format(
                     cell_index, token.map[0] + 1, err
                 )
             )
         if not isinstance(metadata, dict):
             raise MystMetadataParsingError(
-                "Markdown cell {} at line {} is not a dict".format(cell_index, token.map[0] + 1)
+                "Markdown cell {} at line {} is not a dict".format(
+                    cell_index, token.map[0] + 1
+                )
             )
 
     return metadata
 
 
-def _load_code_from_file(nb_path: None | str | Path, file_name: str, token, body_lines: list[str]):
+def _load_code_from_file(
+    nb_path: None | str | Path, file_name: str, token, body_lines: list[str]
+):
     """load source code from a file."""
     if nb_path is None:
         raise _LoadFileParsingError("path to notebook not supplied for :load:")
     file_path = Path(nb_path).parent.joinpath(file_name).resolve()
     if len(body_lines):
         pass  # TODO this would make the reader dependent on sphinx
         # line = token.map[0] if token.map else 0
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/render.py` & `myst_nb-1.1.0/myst_nb/core/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,17 @@
         classes = ["cell"]
         for tag in tags:
             classes.append(f"tag_{tag.replace(' ', '_')}")
 
         # TODO do we need this -/_ duplication of tag names, or can we deprecate one?
         hide_cell = "hide-cell" in tags
         remove_input = (
-            self.get_cell_level_config("remove_code_source", token.meta["metadata"], line=cell_line)
+            self.get_cell_level_config(
+                "remove_code_source", token.meta["metadata"], line=cell_line
+            )
             or ("remove_input" in tags)
             or ("remove-input" in tags)
         )
         hide_input = "hide-input" in tags
         remove_output = (
             self.get_cell_level_config(
                 "remove_code_outputs", token.meta["metadata"], line=cell_line
@@ -188,15 +190,17 @@
             cell_container["prompt_show"] = code_prompt_show
             cell_container["prompt_hide"] = code_prompt_hide
 
         self.add_line_and_source_path(cell_container, token)
         with self.current_node_context(cell_container, append=True):
             # render the code source code
             if not remove_input:
-                cell_input = nodes.container(nb_element="cell_code_source", classes=["cell_input"])
+                cell_input = nodes.container(
+                    nb_element="cell_code_source", classes=["cell_input"]
+                )
                 self.add_line_and_source_path(cell_input, token)
                 with self.current_node_context(cell_input, append=True):
                     self._render_nb_cell_code_source(token)
 
             # render the execution output, if any
             if outputs and (not remove_output):
                 cell_output = nodes.container(
@@ -316,15 +320,17 @@
         except AttributeError:
             return self.content  # type: ignore
 
 
 class NbElementRenderer:
     """A class for rendering notebook elements."""
 
-    def __init__(self, renderer: DocutilsNbRenderer | SphinxNbRenderer, logger: LoggerType) -> None:
+    def __init__(
+        self, renderer: DocutilsNbRenderer | SphinxNbRenderer, logger: LoggerType
+    ) -> None:
         """Initialize the renderer.
 
         :params output_folder: the folder path for external outputs (like images)
         """
         self._renderer = renderer
         self._logger = logger
 
@@ -350,15 +356,17 @@
         return self._logger
 
     @property
     def source(self):
         """The source of the notebook."""
         return self.renderer.document["source"]
 
-    def write_file(self, path: list[str], content: bytes, overwrite=False, exists_ok=False) -> str:
+    def write_file(
+        self, path: list[str], content: bytes, overwrite=False, exists_ok=False
+    ) -> str:
         """Write a file to the external output folder.
 
         :param path: the path to write the file to, relative to the output folder
         :param content: the content to write to the file
         :param overwrite: whether to overwrite an existing file
         :param exists_ok: whether to ignore an existing file if overwrite is False
 
@@ -434,15 +442,17 @@
         :param source_line: the line number of the cell in the source document
         """
         mime_type = metadata.get("format")
         if not mime_type:
             # skip without warning, since e.g. jupytext saves raw cells with no format
             return []
         return self.render_mime_type(
-            MimeData(mime_type, content, metadata, cell_index=cell_index, line=source_line)
+            MimeData(
+                mime_type, content, metadata, cell_index=cell_index, line=source_line
+            )
         )
 
     def render_stdout(
         self,
         output: NotebookNode,
         cell_metadata: dict[str, Any],
         cell_index: int,
@@ -595,15 +605,17 @@
             data.string, lexer, source=self.source, line=data.line
         )
         node["classes"] += ["output", "text_plain"]
         return [node]
 
     def render_text_html(self, data: MimeData) -> list[nodes.Element]:
         """Render a notebook text/html mime data output."""
-        return [nodes.raw(text=data.string, format="html", classes=["output", "text_html"])]
+        return [
+            nodes.raw(text=data.string, format="html", classes=["output", "text_html"])
+        ]
 
     def render_text_latex(self, data: MimeData) -> list[nodes.Element]:
         """Render a notebook text/latex mime data output."""
         # TODO should we always assume this is math?
         return [
             nodes.math_block(
                 text=strip_latex_delimiters(data.string),
@@ -627,15 +639,17 @@
         }:
             # data is b64-encoded as text
             data_bytes = a2b_base64(data.content)
         elif isinstance(data.content, str):
             # ensure correct line separator
             data_bytes = os.linesep.join(data.content.splitlines()).encode("utf-8")
         # create filename
-        extension = guess_extension(data.mime_type) or "." + data.mime_type.rsplit("/")[-1]
+        extension = (
+            guess_extension(data.mime_type) or "." + data.mime_type.rsplit("/")[-1]
+        )
         # latex does not recognize the '.jpe' extension
         extension = ".jpeg" if extension == ".jpe" else extension
         # ensure de-duplication of outputs by using hash as filename
         # TODO note this is a change to the current implementation,
         # which names by {notbook_name}-{cell_index}-{output-index}.{extension}
         data_hash = hashlib.sha256(data_bytes).hexdigest()
         filename = f"{data_hash}{extension}"
@@ -643,14 +657,22 @@
         uri = self.write_file([filename], data_bytes, overwrite=False, exists_ok=True)
         image_node = nodes.image(uri=uri)
         # apply attributes to the image node
         # TODO backwards-compatible re-naming to image_options?
         image_options = self.renderer.get_cell_level_config(
             "render_image_options", data.cell_metadata, line=data.line
         )
+        # Overwrite with metadata stored in output
+        image_options.update(
+            {
+                key: str(value)
+                for key, value in data.output_metadata.get(data.mime_type, {}).items()
+                if key in {"width", "height"}
+            }
+        )
         for key, spec in [
             ("classes", options_spec.class_option),
             ("alt", options_spec.unchanged),
             ("height", options_spec.length_or_unitless),
             ("width", options_spec.length_or_percentage_or_unitless),
             ("scale", options_spec.percentage),
             ("align", lambda a: options_spec.choice(a, ("left", "center", "right"))),
@@ -734,15 +756,17 @@
             "render_markdown_format", data.cell_metadata, line=data.line
         )
         return self._render_markdown_base(data, fmt=fmt, inline=True)
 
     def render_text_plain_inline(self, data: MimeData) -> list[nodes.Element]:
         """Render a notebook text/plain mime data output."""
         content = data.string
-        if data.output_metadata.get("strip_text_quotes", False) and _QUOTED_RE.match(content):
+        if data.output_metadata.get("strip_text_quotes", False) and _QUOTED_RE.match(
+            content
+        ):
             content = content[1:-1]
         node = nodes.inline(data.string, content, classes=["output", "text_plain"])
         return [node]
 
     def render_text_html_inline(self, data: MimeData) -> list[nodes.Element]:
         """Render a notebook text/html mime data output."""
         return self.render_text_html(data)
@@ -1187,22 +1211,26 @@
         },
         "text": {"text/latex": 10, "text/markdown": 20, "text/plain": 30},
         "xml": {"text/latex": 10, "text/markdown": 20, "text/plain": 30},
         "pseudoxml": {"text/latex": 10, "text/markdown": 20, "text/plain": 30},
     }
 
 
-def get_mime_priority(builder: str, overrides: Sequence[tuple[str, str, int | None]]) -> list[str]:
+def get_mime_priority(
+    builder: str, overrides: Sequence[tuple[str, str, int | None]]
+) -> list[str]:
     """Return the priority list for the builder.
 
     Takes the base priority list, overrides from the config,
     then sorts by priority in ascending order.
     """
     base = base_render_priority().get(builder, {})
     overrides = list(overrides)
     for plugin in load_mime_renders():
         overrides = list(getattr(plugin, "mime_priority_overrides", [])) + overrides
     for override in overrides:
         if override[0] == "*" or override[0] == builder:
             base[override[1]] = override[2]
-    sort = sorted(((k, p) for k, p in base.items() if p is not None), key=lambda x: x[1])
+    sort = sorted(
+        ((k, p) for k, p in base.items() if p is not None), key=lambda x: x[1]
+    )
     return [k for k, _ in sort]
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/utils.py` & `myst_nb-1.1.0/myst_nb/core/utils.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/core/variables.py` & `myst_nb-1.1.0/myst_nb/core/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,16 @@
     )
     try:
         mime_type = next(x for x in mime_priority if x in output.data)
     except StopIteration:
         if output.data:
             return [
                 create_warning(
-                    "No output mime type found from render_priority " f"(output<{output.index}>)",
+                    "No output mime type found from render_priority "
+                    f"(output<{output.index}>)",
                     document,
                     line,
                     output.vtype,
                 )
             ]
         return []
     else:
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/docutils_.py` & `myst_nb-1.1.0/myst_nb/docutils_.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,40 +138,46 @@
             nb_reader = NbReader(standard_nb_read, md_config)
         notebook = nb_reader.read(inputstring)
 
         # update the global markdown config with the file-level config
         warning = lambda wtype, msg: create_warning(  # noqa: E731
             document, msg, line=1, append_to=document, subtype=wtype
         )
-        nb_reader.md_config = merge_file_level(nb_reader.md_config, notebook.metadata, warning)
+        nb_reader.md_config = merge_file_level(
+            nb_reader.md_config, notebook.metadata, warning
+        )
 
         # Update mystnb configuration with notebook level metadata
         if nb_config.metadata_key in notebook.metadata:
             overrides = nb_node_to_dict(notebook.metadata[nb_config.metadata_key])
             try:
                 nb_config = nb_config.copy(**overrides)
             except Exception as exc:
                 logger.warning(
                     f"Failed to update configuration with notebook metadata: {exc}",
                     subtype="config",
                 )
             else:
-                logger.debug("Updated configuration with notebook metadata", subtype="config")
+                logger.debug(
+                    "Updated configuration with notebook metadata", subtype="config"
+                )
 
         # Setup the markdown parser
         mdit_parser = create_md_parser(nb_reader.md_config, DocutilsNbRenderer)
         mdit_parser.options["document"] = document
         mdit_parser.options["nb_config"] = nb_config
         mdit_renderer: DocutilsNbRenderer = mdit_parser.renderer  # type: ignore
         mdit_env: dict[str, Any] = {}
 
         # load notebook element renderer class from entry-point name
         # this is separate from DocutilsNbRenderer, so that users can override it
         renderer_name = nb_config.render_plugin
-        nb_renderer: NbElementRenderer = load_renderer(renderer_name)(mdit_renderer, logger)
+        nb_renderer: NbElementRenderer = load_renderer(renderer_name)(
+            mdit_renderer, logger
+        )
         # we temporarily store nb_renderer on the document,
         # so that roles/directives can access it
         document.attributes["nb_renderer"] = nb_renderer
         # we currently do this early, so that the nb_renderer has access to things
         mdit_renderer.setup_render(mdit_parser.options, mdit_env)  # type: ignore
 
         # parse notebook structure to markdown-it tokens
@@ -197,15 +203,15 @@
             # if we are using an HTML writer, dynamically add the CSS to the output
             if nb_config.append_css and hasattr(document.settings, "stylesheet"):
                 css_paths = []
 
                 css_paths.append(
                     nb_renderer.write_file(
                         ["mystnb.css"],
-                        import_resources.read_binary(static, "mystnb.css"),
+                        (import_resources.files(static) / "mystnb.css").read_bytes(),
                         overwrite=True,
                     )
                 )
                 fmt = get_formatter_by_name("html", style="default")
                 css_paths.append(
                     nb_renderer.write_file(
                         ["pygments.css"],
@@ -261,25 +267,31 @@
         # render the outputs
         mime_priority = get_mime_priority(
             self.nb_config.builder_name, self.nb_config.mime_priority_overrides
         )
         for output_index, output in enumerate(outputs):
             if output.output_type == "stream":
                 if output.name == "stdout":
-                    _nodes = self.nb_renderer.render_stdout(output, metadata, cell_index, line)
+                    _nodes = self.nb_renderer.render_stdout(
+                        output, metadata, cell_index, line
+                    )
                     self.add_line_and_source_path_r(_nodes, token)
                     self.current_node.extend(_nodes)
                 elif output.name == "stderr":
-                    _nodes = self.nb_renderer.render_stderr(output, metadata, cell_index, line)
+                    _nodes = self.nb_renderer.render_stderr(
+                        output, metadata, cell_index, line
+                    )
                     self.add_line_and_source_path_r(_nodes, token)
                     self.current_node.extend(_nodes)
                 else:
                     pass  # TODO warning
             elif output.output_type == "error":
-                _nodes = self.nb_renderer.render_error(output, metadata, cell_index, line)
+                _nodes = self.nb_renderer.render_error(
+                    output, metadata, cell_index, line
+                )
                 self.add_line_and_source_path_r(_nodes, token)
                 self.current_node.extend(_nodes)
             elif output.output_type in ("display_data", "execute_result"):
                 # Note, this is different to the sphinx implementation,
                 # here we directly select a single output, based on the mime_priority,
                 # as opposed to output all mime types, and select in a post-transform
                 # (the mime_priority must then be set for the output format)
@@ -295,15 +307,17 @@
                             line=line,
                             append_to=self.current_node,
                             # wtype=DEFAULT_LOG_TYPE,
                             subtype=MystNBWarnings.MIME_TYPE,
                         )
                 else:
                     figure_options = (
-                        self.get_cell_level_config("render_figure_options", metadata, line=line)
+                        self.get_cell_level_config(
+                            "render_figure_options", metadata, line=line
+                        )
                         or None
                     )
 
                     with create_figure_context(self, figure_options, line):
                         _nodes = self.nb_renderer.render_mime_type(
                             MimeData(
                                 mime_type,
@@ -324,15 +338,17 @@
                     line=line,
                     append_to=self.current_node,
                     # wtype=DEFAULT_LOG_TYPE,
                     subtype=MystNBWarnings.OUTPUT_TYPE,
                 )
 
 
-def _run_cli(writer_name: str, builder_name: str, writer_description: str, argv: list[str] | None):
+def _run_cli(
+    writer_name: str, builder_name: str, writer_description: str, argv: list[str] | None
+):
     """Run the command line interface for a particular writer."""
     publish_cmdline(
         parser=Parser(),
         writer_name=writer_name,
         description=(
             f"Generates {writer_description} from standalone MyST Notebook sources.\n"
             f"{default_description}\n"
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/eval/__init__.py` & `myst_nb-1.1.0/myst_nb/ext/eval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,17 @@
             data = retrieve_eval_data(self.document, self.arguments[0])
         except RetrievalError as exc:
             return [eval_warning(str(exc), self.document, self.line)]
 
         render: dict[str, Any] = {}
         for key in ("alt", "height", "width", "scale", "class"):
             if key in self.options:
-                render.setdefault("image", {})[key.replace("classes", "class")] = self.options[key]
+                render.setdefault("image", {})[
+                    key.replace("classes", "class")
+                ] = self.options[key]
 
         mime_nodes = render_variable_outputs(
             data, self.document, self.line, self.source, render=render
         )
 
         # note: most of this is copied directly from sphinx.Figure
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/execution_tables.py` & `myst_nb-1.1.0/myst_nb/ext/execution_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from docutils import nodes
 from sphinx.addnodes import pending_xref
 from sphinx.application import Sphinx
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
 
+from myst_nb._compat import findall
 from myst_nb.sphinx_ import NbMetadataCollector, SphinxEnvType
 
 SPHINX_LOGGER = logging.getLogger(__name__)
 
 METADATA_KEY = "has_exec_table"
 
 
@@ -58,48 +59,56 @@
         return None
     to_update = [
         docname
         for docname, data in NbMetadataCollector.get_doc_data(env).items()
         if data.get(METADATA_KEY)
     ]
     if to_update:
-        SPHINX_LOGGER.info(f"Updating {len(to_update)} file(s) with execution table [mystnb]")
+        SPHINX_LOGGER.info(
+            f"Updating {len(to_update)} file(s) with execution table [mystnb]"
+        )
     return to_update
 
 
 class ExecutionStatsPostTransform(SphinxPostTransform):
     """Replace the placeholder node with the final table nodes."""
 
     default_priority = 8  # before ReferencesResolver (10) and MystReferenceResolver(9)
 
     def run(self, **kwargs) -> None:
         """Replace the placeholder node with the final table nodes."""
         self.env: SphinxEnvType
-        for node in self.document.traverse(ExecutionStatsNode):
+        for node in findall(self.document)(ExecutionStatsNode):
             node.replace_self(
-                make_stat_table(self.env.docname, NbMetadataCollector.get_doc_data(self.env))
+                make_stat_table(
+                    self.env.docname, NbMetadataCollector.get_doc_data(self.env)
+                )
             )
 
 
 _key2header: dict[str, str] = {
     "mtime": "Modified",
     "method": "Method",
     "runtime": "Run Time (s)",
     "succeeded": "Status",
 }
 
 _key2transform: dict[str, Callable[[Any], str]] = {
-    "mtime": lambda x: datetime.fromtimestamp(x).strftime("%Y-%m-%d %H:%M") if x else "",
+    "mtime": lambda x: datetime.fromtimestamp(x).strftime("%Y-%m-%d %H:%M")
+    if x
+    else "",
     "method": str,
     "runtime": lambda x: "-" if x is None else str(round(x, 2)),
     "succeeded": lambda x: "✅" if x is True else "❌",
 }
 
 
-def make_stat_table(parent_docname: str, metadata: DefaultDict[str, dict]) -> nodes.table:
+def make_stat_table(
+    parent_docname: str, metadata: DefaultDict[str, dict]
+) -> nodes.table:
     """Create a table of statistics on executed notebooks."""
 
     # top-level element
     table = nodes.table()
     table["classes"] += ["colwidths-auto"]
     # self.set_source_info(table)
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/__init__.py` & `myst_nb-1.1.0/myst_nb/ext/glue/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,17 @@
     display: bool
         Display the object you are gluing. This is helpful in sanity-checking the
         state of the object at glue-time.
     """
     mimebundle, metadata = IPython.core.formatters.format_display_data(variable)
     mime_prefix = "" if display else GLUE_PREFIX
     metadata["scrapbook"] = dict(name=name, mime_prefix=mime_prefix)
-    ipy_display({mime_prefix + k: v for k, v in mimebundle.items()}, raw=True, metadata=metadata)
+    ipy_display(
+        {mime_prefix + k: v for k, v in mimebundle.items()}, raw=True, metadata=metadata
+    )
 
 
 def extract_glue_data(
     notebook: NotebookNode,
     source_map: list[int],
     logger: LoggerType,
 ) -> dict[str, NotebookNode]:
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/crossref.py` & `myst_nb-1.1.0/myst_nb/ext/glue/crossref.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 
     default_priority = 5
 
     def apply(self, **kwargs):
         """Apply the transform."""
         cache_folder = self.env.mystnb_config.output_folder  # type: ignore
         bname = self.app.builder.name
-        priority_list = get_mime_priority(bname, self.config["nb_mime_priority_overrides"])
+        priority_list = get_mime_priority(
+            bname, self.config["nb_mime_priority_overrides"]
+        )
         node: PendingGlueReference
         for node in list(findall(self.document)(PendingGlueReference)):
             data = read_glue_cache(cache_folder, node.refdoc)
             if node.key not in data:
                 SPHINX_LOGGER.warning(
                     f"Glue reference {node.key!r} not found in doc {node.refdoc!r} "
                     f"[{DEFAULT_LOG_TYPE}.glue_ref]",
@@ -94,16 +96,22 @@
             continue
         if mime_type == "text/plain":
             if node.inline:
                 return [nodes.literal(data[mime_type], data[mime_type])]
             else:
                 return [nodes.literal_block(data[mime_type], data[mime_type])]
         if mime_type == "text/html":
-            return [nodes.raw(text=data[mime_type], format="html", classes=["output", "text_html"])]
-    ref_warning(f"No allowed mime type found in {node.key!r}: {list(output['data'])}", node)
+            return [
+                nodes.raw(
+                    text=data[mime_type], format="html", classes=["output", "text_html"]
+                )
+            ]
+    ref_warning(
+        f"No allowed mime type found in {node.key!r}: {list(output['data'])}", node
+    )
     return []
 
 
 def generate_text_nodes(node: PendingGlueReference, output: dict[str, Any]):
     """Generate nodes for a cell, for formatted text/plain."""
     data = output["data"]
     if "text/plain" not in data:
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/directives.py` & `myst_nb-1.1.0/myst_nb/ext/glue/directives.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,17 @@
         try:
             data = retrieve_glue_data(self.document, self.arguments[0])
         except RetrievalError as exc:
             return [glue_warning(str(exc), self.document, self.line)]
         render: Dict[str, Any] = {}
         for key in ("alt", "height", "width", "scale", "class"):
             if key in self.options:
-                render.setdefault("image", {})[key.replace("classes", "class")] = self.options[key]
+                render.setdefault("image", {})[
+                    key.replace("classes", "class")
+                ] = self.options[key]
         paste_nodes = render_variable_outputs(
             [data], self.document, self.line, self.source, render=render
         )
 
         # note: most of this is copied directly from sphinx.Figure
 
         # create figure node
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/domain.py` & `myst_nb-1.1.0/myst_nb/ext/glue/domain.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/roles.py` & `myst_nb-1.1.0/myst_nb/ext/glue/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,22 +117,26 @@
                     f"{exc} (use `path::key`, to glue from another document)",
                     self.document,
                     self.line,
                 )
             ]
         if "text/plain" not in result.data:
             return [], [
-                glue_warning(f"No text/plain found in {key!r} data", self.document, self.line)
+                glue_warning(
+                    f"No text/plain found in {key!r} data", self.document, self.line
+                )
             ]
 
         try:
             text = format_plain_text(result.data["text/plain"], fmt_spec)
         except Exception as exc:
             return [], [
-                glue_warning(f"Failed to format text/plain data: {exc}", self.document, self.line)
+                glue_warning(
+                    f"Failed to format text/plain data: {exc}", self.document, self.line
+                )
             ]
         node = nodes.inline(text, text, classes=["pasted-text"])
         self.set_source_info(node)
         return [node], []
 
 
 class PasteMarkdownRole(RoleBase):
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/glue/utils.py` & `myst_nb-1.1.0/myst_nb/ext/glue/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,21 +56,27 @@
     key: str,
     inline: bool = False,
     gtype: str | None = None,
     **kwargs: Any,
 ) -> PendingGlueReference:
     """Create a pending glue reference."""
     if not is_sphinx(document):
-        raise PendingGlueReferenceError("Pending glue references are only supported in sphinx.")
+        raise PendingGlueReferenceError(
+            "Pending glue references are only supported in sphinx."
+        )
     env: BuildEnvironment = document.settings.env
     _, filepath = env.relfn2path(rel_doc, env.docname)
     refdoc = env.path2doc(filepath)
     if refdoc is None:
-        raise PendingGlueReferenceError(f"Pending glue reference document not found: {filepath!r}.")
-    ref = PendingGlueReference(refdoc=refdoc, key=key, inline=inline, gtype=gtype, **kwargs)
+        raise PendingGlueReferenceError(
+            f"Pending glue reference document not found: {filepath!r}."
+        )
+    ref = PendingGlueReference(
+        refdoc=refdoc, key=key, inline=inline, gtype=gtype, **kwargs
+    )
     ref.source = source
     ref.line = line
     return ref
 
 
 def retrieve_glue_data(document: nodes.document, key: str) -> VariableOutput:
     """Retrieve the glue data from a specific document."""
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/ext/utils.py` & `myst_nb-1.1.0/myst_nb/ext/utils.py`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/sphinx_.py` & `myst_nb-1.1.0/myst_nb/sphinx_.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,17 @@
             return super().parse(inputstring, document)
         notebook = nb_reader.read(inputstring)
 
         # update the global markdown config with the file-level config
         warning = lambda wtype, msg: create_warning(  # noqa: E731
             document, msg, line=1, append_to=document, subtype=wtype
         )
-        nb_reader.md_config = merge_file_level(nb_reader.md_config, notebook.metadata, warning)
+        nb_reader.md_config = merge_file_level(
+            nb_reader.md_config, notebook.metadata, warning
+        )
 
         # potentially replace kernel name with alias
         kernel_name = notebook.metadata.get("kernelspec", {}).get("name", None)
         if kernel_name is not None and nb_config.kernel_rgx_aliases:
             for rgx, alias in nb_config.kernel_rgx_aliases.items():
                 if re.fullmatch(rgx, kernel_name):
                     logger.debug(
@@ -114,27 +116,31 @@
                 nb_config = nb_config.copy(**overrides)
             except Exception as exc:
                 logger.warning(
                     f"Failed to update configuration with notebook metadata: {exc}",
                     subtype="config",
                 )
             else:
-                logger.debug("Updated configuration with notebook metadata", subtype="config")
+                logger.debug(
+                    "Updated configuration with notebook metadata", subtype="config"
+                )
 
         # Setup the parser
         mdit_parser = create_md_parser(nb_reader.md_config, SphinxNbRenderer)
         mdit_parser.options["document"] = document
         mdit_parser.options["nb_config"] = nb_config
         mdit_renderer: SphinxNbRenderer = mdit_parser.renderer  # type: ignore
         mdit_env: dict[str, Any] = {}
 
         # load notebook element renderer class from entry-point name
         # this is separate from SphinxNbRenderer, so that users can override it
         renderer_name = nb_config.render_plugin
-        nb_renderer: NbElementRenderer = load_renderer(renderer_name)(mdit_renderer, logger)
+        nb_renderer: NbElementRenderer = load_renderer(renderer_name)(
+            mdit_renderer, logger
+        )
         # we temporarily store nb_renderer on the document,
         # so that roles/directives can access it
         document.attributes["nb_renderer"] = nb_renderer
         # we currently do this early, so that the nb_renderer has access to things
         mdit_renderer.setup_render(mdit_parser.options, mdit_env)  # type: ignore
 
         # parse notebook structure to markdown-it tokens
@@ -148,22 +154,26 @@
         ) as nb_client:
             mdit_parser.options["nb_client"] = nb_client
             # convert to docutils AST, which is added to the document
             mdit_renderer.render(mdit_tokens, mdit_parser.options, mdit_env)
 
         # save final execution data
         if nb_client.exec_metadata:
-            NbMetadataCollector.set_exec_data(self.env, self.env.docname, nb_client.exec_metadata)
+            NbMetadataCollector.set_exec_data(
+                self.env, self.env.docname, nb_client.exec_metadata
+            )
             if nb_client.exec_metadata["traceback"]:
                 # store error traceback in outdir and log its path
                 reports_file = Path(self.env.app.outdir).joinpath(
                     "reports", *(self.env.docname + ".err.log").split("/")
                 )
                 reports_file.parent.mkdir(parents=True, exist_ok=True)
-                reports_file.write_text(nb_client.exec_metadata["traceback"], encoding="utf8")
+                reports_file.write_text(
+                    nb_client.exec_metadata["traceback"], encoding="utf8"
+                )
                 logger.warning(
                     f"Notebook exception traceback saved in: {reports_file}",
                     subtype="exec",
                 )
 
         # write final (updated) notebook to output folder (utf8 is standard encoding)
         path = self.env.docname.split("/")
@@ -185,15 +195,17 @@
                 self.env, self.env.docname, "glue", list(nb_client.glue_data.keys())
             )
 
         # move some document metadata to environment metadata,
         # so that we can later read it from the environment,
         # rather than having to load the whole doctree
         for key, (uri, kwargs) in document.attributes.pop("nb_js_files", {}).items():
-            NbMetadataCollector.add_js_file(self.env, self.env.docname, key, uri, kwargs)
+            NbMetadataCollector.add_js_file(
+                self.env, self.env.docname, key, uri, kwargs
+            )
 
         # remove temporary state
         document.attributes.pop("nb_renderer")
 
 
 class SphinxNbRenderer(SphinxRenderer, MditRenderMixin):
     """A sphinx renderer for Jupyter Notebooks."""
@@ -228,38 +240,47 @@
         line = token_line(token, 0)
         cell_index = token.meta["index"]
         metadata = token.meta["metadata"]
         # render the outputs
         for output_index, output in enumerate(outputs):
             if output.output_type == "stream":
                 if output.name == "stdout":
-                    _nodes = self.nb_renderer.render_stdout(output, metadata, cell_index, line)
+                    _nodes = self.nb_renderer.render_stdout(
+                        output, metadata, cell_index, line
+                    )
                     self.add_line_and_source_path_r(_nodes, token)
                     self.current_node.extend(_nodes)
                 elif output.name == "stderr":
-                    _nodes = self.nb_renderer.render_stderr(output, metadata, cell_index, line)
+                    _nodes = self.nb_renderer.render_stderr(
+                        output, metadata, cell_index, line
+                    )
                     self.add_line_and_source_path_r(_nodes, token)
                     self.current_node.extend(_nodes)
                 else:
                     pass  # TODO warning
             elif output.output_type == "error":
-                _nodes = self.nb_renderer.render_error(output, metadata, cell_index, line)
+                _nodes = self.nb_renderer.render_error(
+                    output, metadata, cell_index, line
+                )
                 self.add_line_and_source_path_r(_nodes, token)
                 self.current_node.extend(_nodes)
             elif output.output_type in ("display_data", "execute_result"):
                 # Note, this is different to the docutils implementation,
                 # where we directly select a single output, based on the mime_priority.
                 # Here, we do not know the mime priority until we know the output format
                 # so we output all the outputs during this parsing phase
                 # (this is what sphinx caches as "output format agnostic" AST),
                 # and replace the mime_bundle with the format specific output
                 # in a post-transform (run per output format on the cached AST)
 
                 figure_options = (
-                    self.get_cell_level_config("render_figure_options", metadata, line=line) or None
+                    self.get_cell_level_config(
+                        "render_figure_options", metadata, line=line
+                    )
+                    or None
                 )
 
                 with create_figure_context(self, figure_options, line):
                     mime_bundle = nodes.container(nb_element="mime_bundle")
                     with self.current_node_context(mime_bundle):
                         for mime_type, data in output["data"].items():
                             mime_container = nodes.container(mime_type=mime_type)
@@ -300,15 +321,17 @@
     default_priority = 4  # TODO set correct priority
 
     def run(self, **kwargs: Any) -> None:
         """Run the transform."""
         # get priority list for this builder
         # TODO allow for per-notebook/cell priority dicts?
         bname = self.app.builder.name
-        priority_list = get_mime_priority(bname, self.config["nb_mime_priority_overrides"])
+        priority_list = get_mime_priority(
+            bname, self.config["nb_mime_priority_overrides"]
+        )
 
         def condition(node):
             return (
                 isinstance(node, nodes.container)
                 and node.attributes.get("nb_element", "") == "mime_bundle"
             )
 
@@ -358,15 +381,17 @@
     def get_doc_data(env: SphinxEnvType) -> DefaultDict[str, dict]:
         """Get myst-nb docname -> metadata dict."""
         if not hasattr(env, "nb_metadata"):
             env.nb_metadata = defaultdict(dict)
         return env.nb_metadata
 
     @classmethod
-    def set_exec_data(cls, env: SphinxEnvType, docname: str, value: ExecutionResult) -> None:
+    def set_exec_data(
+        cls, env: SphinxEnvType, docname: str, value: ExecutionResult
+    ) -> None:
         """Add nb metadata for a docname to the environment."""
         cls.set_doc_data(env, docname, "exec_data", value)
         # TODO this does not take account of cache data
         cls.note_exec_update(env)
 
     @classmethod
     def get_exec_data(cls, env: SphinxEnvType, docname: str) -> ExecutionResult | None:
@@ -481,15 +506,19 @@
     """Hide input cells in the HTML output."""
 
     default_priority = 199
     formats = ("html",)
 
     def run(self, **kwargs):
         for node in findall(self.document)(nodes.container):
-            if node.get("nb_element") == "cell_code" and node.get("hide_mode") and node.children:
+            if (
+                node.get("nb_element") == "cell_code"
+                and node.get("hide_mode")
+                and node.children
+            ):
                 hide_mode = node.get("hide_mode")
                 has_input = node.children[0].get("nb_element") == "cell_code_source"
                 has_output = node.children[-1].get("nb_element") == "cell_code_output"
 
                 if has_input and hide_mode == "all":
                     # wrap everything and place a summary above the input
                     wrap_node = HideCodeCellNode(
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/sphinx_ext.py` & `myst_nb-1.1.0/myst_nb/sphinx_ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 
     # add myst-nb configuration variables
     for name, default, field in NbParserConfig().as_triple():
         if not field.metadata.get("sphinx_exclude"):
             # TODO add types?
             app.add_config_value(f"nb_{name}", default, "env", Any)
             if "legacy_name" in field.metadata:
-                app.add_config_value(f"{field.metadata['legacy_name']}", _UNSET, "env", Any)
+                app.add_config_value(
+                    f"{field.metadata['legacy_name']}", _UNSET, "env", Any
+                )
     # Handle non-standard deprecation
     app.add_config_value("nb_render_priority", _UNSET, "env", Any)
 
     # generate notebook configuration from Sphinx configuration
     # this also validates the configuration values
     app.connect("builder-inited", create_mystnb_config)
 
@@ -151,15 +153,17 @@
             f"{DEFAULT_LOG_TYPE}.config",
             type=DEFAULT_LOG_TYPE,
             subtype="config",
         )
 
     try:
         app.env.mystnb_config = NbParserConfig(**values)
-        SPHINX_LOGGER.info(bold("myst-nb v%s:") + " %s", __version__, app.env.mystnb_config)
+        SPHINX_LOGGER.info(
+            bold("myst-nb v%s:") + " %s", __version__, app.env.mystnb_config
+        )
     except (TypeError, ValueError) as error:
         SPHINX_LOGGER.critical("myst-nb configuration invalid: %s", error.args[0])
         raise
 
     # update the output_folder (for writing external files like images),
     # and the execution_cache_path (for caching notebook outputs)
     # to a set path within the sphinx build folder
@@ -186,15 +190,17 @@
 
 @contextlib.contextmanager
 def _import_resources_path(package: ModuleType, resource: str) -> Iterator[Path]:
     if sys.version_info < (3, 9):
         with import_resources.path(package, resource) as path:
             yield path
     else:
-        with import_resources.as_file(import_resources.files(package).joinpath(resource)) as path:
+        with import_resources.as_file(
+            import_resources.files(package).joinpath(resource)
+        ) as path:
             yield path
 
 
 def add_css(app: Sphinx):
     """Add CSS for myst-nb."""
     with _import_resources_path(static, "mystnb.css") as source_path:
         hash = _get_file_hash(source_path)
@@ -203,18 +209,22 @@
 
 def add_global_html_resources(app: Sphinx, exception):
     """Add HTML resources that apply to all pages."""
     # see https://github.com/sphinx-doc/sphinx/issues/1379
     if app.builder is not None and app.builder.format == "html" and not exception:
         with _import_resources_path(static, "mystnb.css") as source_path:
             hash = _get_file_hash(source_path)
-            destination = os.path.join(app.builder.outdir, "_static", f"mystnb.{hash}.css")
+            destination = os.path.join(
+                app.builder.outdir, "_static", f"mystnb.{hash}.css"
+            )
             copy_asset_file(str(source_path), destination)
 
 
-def add_per_page_html_resources(app: Sphinx, pagename: str, *args: Any, **kwargs: Any) -> None:
+def add_per_page_html_resources(
+    app: Sphinx, pagename: str, *args: Any, **kwargs: Any
+) -> None:
     """Add JS files for this page, identified from the parsing of the notebook."""
     if app.env is None or app.builder is None or app.builder.format != "html":
         return
     js_files = NbMetadataCollector.get_js_files(cast(SphinxEnvType, app.env), pagename)
     for path, kwargs in js_files.values():
         app.add_js_file(path, **kwargs)  # type: ignore
```

### Comparing `myst_nb-1.0.0rc1/myst_nb/static/mystnb.css` & `myst_nb-1.1.0/myst_nb/static/mystnb.css`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/myst_nb/warnings_.py` & `myst_nb-1.1.0/myst_nb/warnings_.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 
     CELL_METADATA_KEY = "cell_metadata_key"
     """Issue with a key in a cell's `metadata` dictionary."""
     CELL_CONFIG = "cell_config"
     """Issue with a cell's configuration or metadata."""
 
 
-def _is_suppressed_warning(type: str, subtype: str, suppress_warnings: Sequence[str]) -> bool:
+def _is_suppressed_warning(
+    type: str, subtype: str, suppress_warnings: Sequence[str]
+) -> bool:
     """Check whether the warning is suppressed or not.
 
     Mirrors:
     https://github.com/sphinx-doc/sphinx/blob/47d9035bca9e83d6db30a0726a02dc9265bd66b1/sphinx/util/logging.py
     """
     if type is None:
         return False
```

### Comparing `myst_nb-1.0.0rc1/pyproject.toml` & `myst_nb-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[build-system]
+ [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "myst-nb"
 dynamic = ["version"]
 description = "A Jupyter Notebook Sphinx reader built on top of the MyST markdown parser."
@@ -34,18 +34,18 @@
     "docutils",
     "sphinx",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "importlib_metadata",
     "ipython",
-    "jupyter-cache>=0.5,<0.7",
+    "jupyter-cache>=0.5",
     "nbclient",  # nbclient version pinned by jupyter-client
     "myst-parser>=1.0.0",
-    "nbformat~=5.0",
+    "nbformat>=5.0",
     "pyyaml",
     "sphinx>=5",
     "typing-extensions",
     # ipykernel is not a requirement of the library,
     # but is a common requirement for users (registers the python3 kernel)
     "ipykernel",
 ]
@@ -97,15 +97,16 @@
     "ipython!=8.1.0,<8.17",
     "ipywidgets>=8",
     "jupytext>=1.11.2,<1.16.0",
     # Matplotlib outputs are sensitive to the matplotlib version
     "matplotlib==3.7.*",
     "nbdime",
     "numpy",
-    "pandas",
+    "pandas==1.5.*",
+    "pyarrow",
     "pytest~=7.1",
     "pytest-cov>=3,<5",
     "pytest-regressions",
     "pytest-param-files~=0.3.3",
     "sympy>=1.10.1",
 ]
 
@@ -139,17 +140,14 @@
 # can only follow these imports when more of the code is typed
 follow_imports = "skip"
 
 [[tool.mypy.overrides]]
 module = ["docutils.*", "nbformat.*", "jupyter_cache.*", "IPython.*", "pygments.*"]
 ignore_missing_imports = true
 
-[tool.ruff]
-line-length = 100
-
 [tool.ruff.lint]
 ignore = [
     "E203",    # Whitespace before punctuation
 ]
 
 [tool.ruff.lint.isort]
 force-sort-within-sections = true
```

### Comparing `myst_nb-1.0.0rc1/tox.ini` & `myst_nb-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `myst_nb-1.0.0rc1/PKG-INFO` & `myst_nb-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myst-nb
-Version: 1.0.0rc1
+Version: 1.1.0
 Summary: A Jupyter Notebook Sphinx reader built on top of the MyST markdown parser.
 Keywords: markdown,lexer,parser,jupyter,docutils,sphinx
 Author-email: ExecutableBookProject <chrisj_sewell@hotmail.com>
 Maintainer-email: Angus Hollands <goosey15@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,18 +19,18 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Dist: importlib_metadata
 Requires-Dist: ipython
-Requires-Dist: jupyter-cache>=0.5,<0.7
+Requires-Dist: jupyter-cache>=0.5
 Requires-Dist: nbclient
 Requires-Dist: myst-parser>=1.0.0
-Requires-Dist: nbformat~=5.0
+Requires-Dist: nbformat>=5.0
 Requires-Dist: pyyaml
 Requires-Dist: sphinx>=5
 Requires-Dist: typing-extensions
 Requires-Dist: ipykernel
 Requires-Dist: pre-commit ; extra == "code_style"
 Requires-Dist: alabaster ; extra == "rtd"
 Requires-Dist: altair ; extra == "rtd"
@@ -53,15 +53,16 @@
 Requires-Dist: ipykernel>=5.5,<7.0 ; extra == "testing"
 Requires-Dist: ipython!=8.1.0,<8.17 ; extra == "testing"
 Requires-Dist: ipywidgets>=8 ; extra == "testing"
 Requires-Dist: jupytext>=1.11.2,<1.16.0 ; extra == "testing"
 Requires-Dist: matplotlib==3.7.* ; extra == "testing"
 Requires-Dist: nbdime ; extra == "testing"
 Requires-Dist: numpy ; extra == "testing"
-Requires-Dist: pandas ; extra == "testing"
+Requires-Dist: pandas==1.5.* ; extra == "testing"
+Requires-Dist: pyarrow ; extra == "testing"
 Requires-Dist: pytest~=7.1 ; extra == "testing"
 Requires-Dist: pytest-cov>=3,<5 ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
 Requires-Dist: pytest-param-files~=0.3.3 ; extra == "testing"
 Requires-Dist: sympy>=1.10.1 ; extra == "testing"
 Project-URL: Documentation, https://myst-nb.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/myst-nb
```

